# 审核流组件

## 一.引入方式

### html代码
````html
<div ms-widget="getflow,$,$getflow" ms-duplex="你绑定的uid"></div>
````



### js代码
````js
 require(['flow/avalon.getflow'])
var flowVM = null


/*配置参数*/
$getflow :{
        node : "" ,  //当前审核节点名称 , 注意跟node.php中配置的节点一致  ， 注意此为非常关键参数,例如Sale.Index.audit
        auth_node:"" , /*权限的节点，是节点数组的key，例如Sale_audit,20170505陈孔毅新增 */
        step:null , //当前审核步骤，从申请人开始0 ，1，2,3,4,5   最多为5 ， 注意此为非常关键参数 , 不配置step就默认选择有权限的员工
        is_showFlow : true ,  //是否显示审核流程图
        onInit : function(vmodels){
             flowVM  = vmodels ; 
        },
        //用于是否显示提交下一步审核按钮, flow_type流程类型0自由类型心，1固定类型，
        //is_last是否最后一个人，1是，0否，为1时就没有提交给下一个人审核的按钮了！！！！！！ 
        //is_in 是否进入了审核流里面，0没有就自己处理，1走审核步骤 
       btnChange:function(flow_type , is_last,is_in){
              if(flow_type==1 && is_last == 1){
                 //把提交下一步审核按钮的按钮隐藏掉.
           }
        } ,     
}
````


## 二.使用方法

### 1.提交时获取当前的审核人及流程（申请人提交时使用）
````html
    <div ms-widget="getflow,$,$getflow" ms-duplex="你绑定的uid"></div>
````
### 2.判断是否有提交下一步审核（是否显示下一步审核按钮）
     如上面的    btnChange回调

### 3.显示下一个审核人（通过并提交给下一个人审核使用）
````js
/*
                     * 获取审核流，通过后台获取数据
                     * uid   审核发起人的uid , 注意是发起人，不一定是当前人的
                     * current_step  当前审核步骤，从申请人开始0 ，1，2,3,4,5   最多为5 ， 注意此为非常关键参数
                     * con_id [interger] [应用里面该条审核记录的主键id]
                     * condition  当前审核的条件，格式为数组, 如condition['money'] = 500 ， condition['number'] = 20
                     */
   flowVM.getFlowNew(current_step,uid,con_id)  
                  
````


##  在应用里面调用流程设置（注意引用的组件不一样了！）
  ````html
<div ms-widget="flow,$,$flow"></div>
````

````
````js
 require(['flow/flow'])
var flowVM = null


/*配置参数*/
$getflow :{
        node : "" ,  //当前审核节点名称 , 注意跟node.php中配置的节点一致  ， 注意此为非常关键参数,例如Sale.Index.audit
        auth_node:"" , /*权限的节点，是节点数组的key，例如Sale_audit,20170505陈孔毅新增 */
        onInit : function(vmodels){
             flowVM  = vmodels ; 
        }


//触发layer弹出框事件：
flowVM.setFlow_one();

```

## 三. 应用中为每条审核订单增加审核流：

````php
//在新建订单时，获取审核人, 注意要带0：
   flow_vm.getFlowNew(0);
````

````php
//在新建订单时，更改订单条件，获取审核人：
//* condition  当前审核的条件，格式为数组, 如condition['money'] = 500 ， condition['number'] = 20 , 没有就留空
   flow_vm.changeFlow(condition);
````

````php
   //在提交订单成功后，使用下面的回调
   /* @param  $con_id int[此审核订单在你自己应用中的主键id] */
   flow_vm.addFlow(con_id);
````

## 四.首页审核引入审核流，增加了审核流的注意：
````php
在详情返回数据$result中【顶层】添加如下：
 
/*
 * @param  $node string [节点标示，如Produce.Index.pq_list]
 * @param  $current_step  int[当前的审核人是第几个，从1开始]
 * @param  $uid int [审核最开始发起人的uid，是订单的创始人哦]
 * @param  $con_id int[此审核订单在你自己应用中的主键id]
 */
$result['flow'] = model('FlowPub')->flowInfo($node,$current_step,$uid,$con_id) ;
 
````


### 首页详情接口中增加一个返回值：
````php
   /* 增加data.flow,结构如下
    flow_type:1    //由上面的一个接口model('Flow')->flowInfo($node);提供
    node: ""   //node
    is_last:1   //是否是最后一个审核人，由接口返回的$data['step']和当前应用的第几个审核人比较判断 ，1是最后一个，0不是
    step:2    //当前应用的第几个审核人
    uid:"1"   //审核发起人的uid , 注意是发起人，不一定是当前人的，
*/
````
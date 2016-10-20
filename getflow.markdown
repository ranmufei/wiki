# 审核流组件

## 引入方式

### html代码
````html
<div ms-widget="getflow,$,$getflow" ></div>
````



### js代码
````js
 require(['flow/getflow'])
var flowVM = null


/*配置参数*/
$getflow :{
        node : "" ,  //当前审核节点名称 , 注意跟node.php中配置的节点一致  ， 注意此为非常关键参数
        step:null , //当前审核步骤，从申请人开始0 ，1，2,3,4,5   最多为5 ， 注意此为非常关键参数
        is_showFlow : true ,  //是否显示审核流程图
        onInit : function(vmodels){
             flowVM  = vmodels ; 
        },
        //用于是否显示提交下一步审核按钮, flow_type流程类型0自由类型心，1固定类型，is_last是否最后一个人，1是，0否，为1时就没有提交给下                   一个人审核的按钮了！！！！！！
       btnChange:function(flow_type , is_last){
              if(flow_type==1 && is_last == 1){
                 //把提交下一步审核按钮的按钮隐藏掉.
           }
        } ,     
}
````


## 使用方法

### 提交时获取当前的审核人及流程（申请人提交时使用）
````html
    直接在引入<div ms-widget="getflow,$,$getflow" ms-duplex="你绑定的uid"></div>
````
### 判断当前人审核人及流程（申请人提交时使用）
````html
    直接在引入<div ms-widget="getflow,$,$getflow" ms-duplex="你绑定的uid"></div>
````

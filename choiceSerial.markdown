#  序列号查询组件 choiceSerial/choiceSerial

## 说明

  > 该组件供查看 选择 带序列号的产品 的序列号。
  > 组件可 查看全部产品的序列号
  > 组件可 根据产品规格  ，仓库的id 参数 获取指定产品规格的 序列号

## 使用方法

  > 引入 Avalon组件地址 choiceSerial/choiceSerial

   [在线预览案列 DEMO ](http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget) http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget


## 配置参数说明
        width:'500px', 
        height:'300px',
        title:'规格管理',
        ckid:'', //仓库id
              formatid:'',//产品规格id
              globle:true,  //显示全部产品 使用该参数后 ckid  formatid 失效
        callbackfun:avalon.noop //回调函数Init

## 基本属性配置

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
| width  | 否 |  默认组件宽度  |
| height |否| 默认高度 |
|title|否| 默认表题 |
|ckid|否| 仓库id |
|formatid|否| 产品规格id |
|globle|否| 开启全部查看/搜索 使用该参数后 ckid  formatid 失效 |

##  接口方法

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|callbackfun()|否| 分类修改 删除 增加后  自动回调函数  |
|show()|否| 弹出规格选择窗口 传入对应的参数后 弹出对应的数据  |



## 案例html 


```
<script src="/App/Invoicimg/AvalonAction/avalon_test.js"></script>


<h1>avalon  组件测试 demo </h1>
<div ms-controller="root">
 

  <div ms-widget="choiceSerial,choiceSerialdsds,$choiceSerialOpt"> </div>


</div>





```


``` javascript

/**
* test
* 
*/
require(['avalon','choiceSerial/choiceSerial','domReady!'],function(avalon){
   var serial=null;
   var model=avalon.define({ 
        $id:'root',        
            $serialopt:{
            onInit:function(smodel){
                serialmodel=smodel;
            },
            title:'序列号管理',
            globle:true,
            },
            serial:function(){
                //查看序列号
                avalon.log('serialmodel:',serialModel);
                serialmodel.show('*');
            }

   })
   avalon.scan();


})

```



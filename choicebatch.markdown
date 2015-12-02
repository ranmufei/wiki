# 批次选择组件  choicebatch/choicebatch

## 说明

  > 该组件供查看 选择 批次
  > 组件提供 规格规格 仓库 参数 查看改仓库 规格的 批次  

## 使用方法

  > 引入 Avalon组件地址 choicebatch/choicebatch

   [在线预览案列 DEMO ](http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget) http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget


## 配置参数说明
        width:'500px', 
        height:'300px',
        title:'规格管理',
        ckid:'', //仓库id
        formatid:'',//产品规格id
      
        callbackfun:avalon.noop //回调函数Init

## 基本属性配置

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
| width  | 否 |  默认组件宽度  |
| height |否| 默认高度 |
|title|否| 默认表题 |
|ckid|否| 仓库id |
|formatid|否| 产品规格id |

##  接口方法

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|callbackfun()|否|  自动回调函数  |
|show()|否| 弹出规格选择窗口 传入对应的参数后 弹出对应的数据  |
|getSelected()|否| 勾选的行产品信息  |



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
require(['avalon','choicebatch/choicebatch','domReady!'],function(avalon){
   var serial=null;
   var model=avalon.define({ 
        $id:'root',        
             $batchchoiceopt:{
               onInit:function(choicedata){
                  batchoicemodel=choicedata;
               },
               title:'批次选择',
               type:0,
               callbackfun:function(){
                   var xz= batchoicemodel.getSelected();
                    avalon.log('选择的产品：',xz);
               },
            },
            choicecp2:function(ckid,subid){                 
                  batchoicemodel.show(ckid,subid)
            },

   })
   avalon.scan();


})

```



# 批次管理组件 formatbatch/formatbatch

## 说明

  > 管理产品有规格的产品 的批次， 可对批次生成序列号； 可修改序列号

## 使用方法

  > 引入 Avalon组件地址 formatbatch/formatbatch

   [在线预览案列](http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget) http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget

``` javascript

/**
* test
* 
*/
require(['avalon','creatclass/creatclass','unit/unit','warehouse/warehouse','createproduct/createproduct','format/format','domReady!'],function(avalon){
   var classmodel=null;
   var model=avalon.define({ 
        $id:'root',
         $formatbatchopt:{
               onInit:function(choicedata){
                  batmode=choicedata;
               },
               title:'pici',
               type:0,
               callbackfun:function(){
                   var xz= batmode.getSelected();
                    avalon.log('选择的产品：',xz);
               },
            },
            choicecp:function(ckid,subid){                 
                  batmode.show(ckid,subid)
            }
   })
   avalon.scan();


})

```


## 配置参数说明
        width:'500px', 
        height:'300px',
        title:'规格管理',
        callbackfun:avalon.noop //回调函数Init

## 基本属性配置

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
| width  | 否 |  默认组件宽度  |
| height |否| 默认高度 |
|title|否| 默认表题 |
|ckid|否| 仓库id |
|formatid|否| 规格id |
|type|否| 0 查看  1 编辑  ； 是否可编辑序列号 |

##  接口方法

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|callbackfun()|否| 分类修改 删除 增加后  自动回调函数  |
|show(ckid,formatid)|否| 调用弹出层 显示 仓库 ，规格 对应的 批次列表 |



## 案例html 


```
<script src="/App/Invoicimg/AvalonAction/avalon_test.js"></script>


<h1>avalon  组件测试 demo </h1>
<div ms-controller="root">
 

 <span ms-on-click=choicecp('1',119)> 武汉仓库 规格119 批次测试1</span>


</div>





```





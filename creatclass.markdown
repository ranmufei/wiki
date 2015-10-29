# 分类管理组件 creatclass/creatclass

## 说明

  > 供全局调用 新建Avalon 弹出层 新建分类  可修改分类  删除 

## 使用方法

  > 引入 Avalon组件地址 creatclass/creatclass

   [在线预览案列](http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget) http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget

``` javascript
/**
* test
* 
*/
require(['avalon','creatclass/creatclass','domReady!'],function(avalon){
   var classmodel=null;
   var model=avalon.define({ 
   			$id:'root',
   			$classopt:{
   				onInit:function(cmodel){
   					console.log('oninit:',cmodel);
   					classmodel=cmodel;
   				},
   				callbackfun:function(){
   					avalon.log('callbackfun 被调用');
   				},
   				width:'400px',
   				height:'500px',
   				title:'测试分类管理',
   				


   			}
   })
   avalon.scan();


})

```

## 配置参数说明
 width:'500px', 
        height:'300px',
        title:'分类管理',
        callbackfun:avalon.noop //回调函数Init

## 基本属性配置

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
| width  | 否 |  默认组件宽度  |
| height |否| 默认高度 |
|title|否| 默认表题 |

##  接口方法

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|callbackfun()|否| 分类修改 删除 增加后  自动回调函数  |






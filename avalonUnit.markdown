# 单位理组件 unit/unit

## 说明

  > 供全局调用 新建Avalon 弹出层 新建单位  可修改单位  删除单位 

## 使用方法

  > 引入 Avalon组件地址 unit/unit

   [在线预览案列](http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget) http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget

``` javascript
/**
* test
* 
*/
require(['avalon','creatclass/creatclass','unit/unit','warehouse/warehouse','domReady!'],function(avalon){
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
        },
            $warehouseopt:{
               width:'600px',
               height:'500px',
               title:'仓库',
               callbackfun:function(){
                  avalon.log('callbackfun 回调仓库');
               },
            },
            $unitopt:{
               width:'500px',
               height:'500px',
               title:'单位管理',
               callbackfun:function(){
                  avalon.log('callbackfun 回调单位');
               },
            }
   })
   avalon.scan();


})

```

## 配置参数说明
        width:'500px', 
        height:'300px',
        title:'仓库管理',
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



## 案例html 


```

<script src="/App/Invoicimg/AvalonAction/avalon_test.js"></script>
<div ms-controller="root">
  <div ms-widget="creatclass,testapi,$classopt">class add</div>



  <div ms-widget="warehouse,warehousenew,$warehouseopt"> 仓库</div>
  <div ms-widget="unit,unitset,$unitopt"> 单位</div>


</div>


```





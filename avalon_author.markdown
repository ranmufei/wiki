# 单独应用权限配置组件 author/author

## 说明

  >  通过本应用可以独立的配置 独立应用的节点权限

## 使用方法

  > 引入 Avalon组件地址 author/author

   [在线预览案列](http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget) http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget



## 配置参数说明
        width:'500px', 
        height:'300px',
        title:'权限管理',
        key:'Invoicing',
        callbackfun:avalon.noop //回调函数Init

## 基本属性配置

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
| width  | 否 |  默认组件宽度  |
| height |否| 默认高度 |
|title|否| 默认表题 |
|key|必须| 应用的key |


##  接口方法

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|callbackfun()|否|  自动回调函数  |
|show(uid)|必须| 打开弹出应用权限管理层  参数 uid （int） 如果给用户的uid 默认显示该用户的权限 |



## 案例html 


``` javascript

/**
* test
* 
*/
require(['avalon','creatclass/creatclass','unit/unit','warehouse/warehouse','createproduct/createproduct','format/format','domReady!'],function(avalon){
   var accModel=null;
   var model=avalon.define({ 
        $id:'root',
          ,$accessOpt:{
               title:'产品权限管理',
               width:'800px',
               height:'500px',
               onInit:function(model){
                  accModel=model;
               }
               ,key:'InvoicimgProduct'
            }
            ,accshow:function(){
               accModel.show();
            }
   })
   avalon.scan();


})

```


```
<div class="col-md-4">
<div class="panel panel-success">
      <div class="panel-heading">
        <h3 class="panel-title">查应用权限</h3>
      </div>
      <div class="panel-body">

  <div ms-widget="author,choiceSerialsdasddsds,$accessOpt"> </div>
   <span ms-on-click="accshow" class="btn">产品应用权限</span>
</div>
</div>
</div>





```





# 单独应用权限配置组件 author/author

## 说明

  >  - 通过本组件可以独立的配置 独立应用的节点权限

  >  - 本组件 的核心作用 是 独立配置 独立应用，而系统中的权限管理 是集中管理全部应用

  >  - 组件的作用是在 之前系统权限基础上的 延伸

  > - `使用该功能的权限节点 还是以前的权限节点 ，也就是说 只要有以前的 分配 权限 ，就可以使用本组件的权限`

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

## 应用开发者 设置 说明

  > - 为统一界面 集中按照如下说明来配置 menu.html 

  ``` html

      {
          id: "9",
          name: "权限设置",
          hide: '<?php echo !access_r($userInfo["uid"],"Admin","Sett","changeauthor");?>', //集中使用系统的权限配置 来开启/关闭 菜单。也就是说只要有系统中的应用权限配置 就可以使用本组件
          lock: false,
          icon:'icon-bar-chart', 
          url: "/index.php?app=InvoicimgWarehouse&m=Index&a=authorSetting", //自己的控制器路径
          title: "权限设置",
          frame: {
            name: 'admin_user_goout_setting'
          }
          
        },



  ```





## Avalon  案例


``` javascript

/**
* test
* 
*/
require(['avalon','author/author','domReady!'],function(avalon){
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
            },accshow2:function(){
              // 如果想单独指定 某个人的权限  可以给show()方法传uid参数 会默认显示用户
               var uid=1001
               accModel.show(uid);
            }
   })
   avalon.scan();


})

```

## 界面部分参考

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





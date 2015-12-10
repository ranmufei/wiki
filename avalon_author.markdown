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
|full|否| 权限配置窗口是否最大化 默认开启  true/false |


##  接口方法

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|callbackfun()|否|  自动回调函数  |
|show(uid)|必须| 打开弹出应用权限管理层  参数 uid （int） 如果给用户的uid 默认显示该用户的权限，为空正常开启全部 |

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
* 批次管理
*/
require([
  'avalon',
  'apppublic/apppublic',
  'author/author',
  'layer/layer',  
  'domReady!'],function(avalon,apppublic){  
   var authorModel=null;
   var model=avalon.define({
      $id:'authroot',
      $accessOpt:{
           title:'仓库管理权限设置',
               onInit:function(model){
                  authorModel=model;
               }
               ,key:'InvoicimgWarehouse'
        }
        ,show:function(){
             //avalon.log('public:',apppublic);
               authorModel.show();
        }
   })

   avalon.scan();


}) // end 

```

## 界面部分参考

```
<layout name="layout" />
<script  src="/App/InvoicimgWarehouse/AvalonAction/avalon_authorSetting.js"></script>

<script>
  $(function ($) {
    // $("#formatbuttom").addClass('btn btn-lg btn-primary');
    $("#formatbuttom").addClass('guige_style');
  });
</script>

<div class="m-top-menu">
    <span class="list-name">权限设置</span>
</div>
   <!--/顶部菜单-->


<div class="table_header_1" ms-controller="authroot">


  <div class="guige_body">
    <div>

      <button class="fenlie_style fenlie_style2" ms-click="show" type="button"></button>
      <p>权限设置</p>

      <div ms-widget="author,dddasdas,$accessOpt" class="sp_fl_dialog"></div>

    </div>
    
  </div>
</div>





```





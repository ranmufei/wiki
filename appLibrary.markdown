# 关联应用 avalon组件  appLibrary/avalon.appLibrary

## 说明

  > 直接在一个应用里面关联另外的应用

  > 应用场景例如： 关联工作流（可以直接新增工作流）、关联项目  ；

  > js引入方式：require(['appLibrary/avalon.appLibrary'])

## 具体使用

一. 引入
````js
//js引入方式
    require(['appLibrary/avalon.appLibrary'])
````
````html
<!-- html引入-->
      <div ms-widget="appLibrary,$,$appLibrary"></div>
````
#### 配置方式：
````js
// 在定义avalon模板前 
 var appVM = null;

//组件配置
   $form:{
     set_name :你的app_name加上id , //你的app_name加上id , id从0开始，注意不能重复，一旦定义后不能修改
     itemChange: function(data){  //获取已关联应用的列表,这里是回调
          console.log('data' , data)
      } ,
     onInit: function(vmodels){
         appVM = vmodels ;

     }
}
````
#### 接口调用:

## 1. 可以关联的应用的列表( 触发 弹出layer框)
````js
//aid 当前行的主键id,比如销售订单的主键id、项目的id等 
appVM.info("showAppList",aid) 

````

## 2. 已关联应用的列表 （ 返回的是一个json对象 ，需要你自己展示）
````js
//aid 当前行的主键id,比如销售订单的主键id、项目的id等 
appVM.info("realtedList"  , aid) 

````

## 3. 查看某条已关联应用的详情（点击事件时使用，以layer展示）
````js
//$index   当前行的索引，从0开始
appVM.info("detail" ,"" , $index) 

````


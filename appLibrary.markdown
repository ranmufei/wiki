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
   $apps:{
     set_name :你的app_name加上id , //你的app_name加上id , id从0开始，注意不能重复，一旦定义后不能修改
     selectApps:"all" , // 默认关联所有已有的的app , 关联单个应用的应写单个应用的key值，如只关联售后:'AfterSalers'，Workflow:工作    流，Pmanager:项目管理
     itemChange: function(data){  //获取已关联应用的列表,这里是回调
          console.log('data' , data)
      } ,
     onInit: function(vmodels){
         appVM = vmodels ;

     },
    selectInfo : function(data){  //获取当前选中的数据,这里是回调
          console.log('data' , data)
          //data.title  关联的标题
           //data.wid   关联的主键
      } ,
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

//在组件配置中调用回调方法获取数据
itemChange：function(data){
   console.log("data",data); 
}
````

## 3. 查看某条已关联应用的详情（点击事件时使用，以layer展示）
````js
//$index   当前行的索引，从0开始
appVM.info("detail" ,"" , $index) 

````

## 4. 关闭关联应用弹出框的回调 （用于触发刷新已关联的应用列表）
````js
//在组件配置中调用回调方法获取回调事件
closeAppLibrary:function(){
   //你刷新已关联应用的事件 
}
````

## 5.获取某个应用的数据接口changeApps
````js
//$key应用的key
//售后:'AfterSalers'，Workflow:工作流，Pmanager:项目管理
appVM.changeApps($key)
````
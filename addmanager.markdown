# 新增项目avalon组件   pmanager/avalon.pmanager



## 具体使用

一. 引入
````js
//js引入方式
    require(['pmanager/avalon.pmanager'])
````
````html
<!-- html引入-->
      <div ms-widget="pmanager,$,$pmanager"></div>
````
#### 配置方式：
````js
// 在定义avalon模板前 
 var pmanagerVM= null;
 
//调出新增项目的弹出框
        //pro_name /*项目名称,可填*/   
        //objective /*项目描述,可填*/
 pmanagerVM.create(pro_name,objective);


//组件配置
   $pmanager:{
        onInit: avalon.noop ,
        add_callback:function(pid,url){  /*添加项目的回调 , 回调两个参数，一个是项目pid，一个项目的详情页面url*/

        } , 
       
   }
````




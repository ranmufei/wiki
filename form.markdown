# 万能表单 avalon组件  form/avalon.form

## 说明

  > 提供新增表单，表单编辑，数据输入，数据读取api接口

  > 应用场景例如： 只需存储info_id , 就可以读取表单内容  ；

  > js引入方式：require(['form/avalon.form'])

## 具体使用

一. 引入
````js
//js引入方式
   require(['form/avalon.form'])
````
````html
<!-- html引入-->
      <div ms-widget="form,$,$form"></div>
````
#### 配置方式：
````js
// 在定义avalon模板前 
 var form_vm ;

//组件配置
   $form:{
     set_id: 0 ,
     info_id:0 , 
     set_name :你的app_name加上id , //--注意不能重复，一旦定义后不能修改--
     form_show_className : '' ,  //显示表单时的类
     form_info_className : '' ,  // 显示数据时的类
     onInit: function(vmodel){
         form_vm = vmodel ;

     }
}
````
#### 接口调用:

## 1. 添加、编辑表单字段
````js
form_vm.addForm() 

````


## 2. 保存提交的的表单信息
````js

form_vm.saveFormInfo().done(function(data){
                      console.log("继续执行其他字段的保存" , data)
          }).fail(function(e){
                      console.log("ajax无返回" ,e) 
         })


````

## 3. 查看表单信息
````js

form_vm.info_id = 你数据库存的的万能表单的数据ID ; 
form_vm.readFormInfo(form_vm.set_id,form_vm.info_id); 

````

##  注意：
### 保存表单 ， 需要把form_vm.addForm() 返回的 set_id 存到你自己的表中  ，下次就读这个set_id

###  保存数据 ， 需要把 form_vm.saveFormInfo() 返回的set_id 和info_id 存入到你自己的表中，读取数据需要用到这2个字段
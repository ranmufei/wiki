# 万能表单 avalon组件  form/avalon.form

## 说明

  > 提供新增表单，表单编辑，数据输入，数据读取api接口

  > 应用场景例如： 只需存储info_id , 就可以读取表单内容  ；

  > 引入方式：require(['form/avalon.form'])

## 具体使用

一. 引入
````php
      <div ms-widget="form,$,$form"></div>
````
#### 配置方式：
````js
// 在定义avalon模板前 
 var form_vm ;
   $form:{
     set_id: 0 ,
     info_id:0 , 
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
## 2. 查看生成的表单字段
````js
form_vm.createForm();
````

## 3. 保存提交的的表单信息
````js

form_vm.saveFormInfo();

````

## 4. 查看表单信息
````js

form_vm.info_id = 你数据库存的的万能表单的数据ID ; 
form_vm.readFormInfo(form_vm.set_id,form_vm.info_id); 

````
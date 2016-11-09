# 导入 avalon组件  uploadnew/uploadnew



## 具体使用

一. 引入
````js
//js引入方式
    require(['uploadnew/uploadnew'])
````
````html
<!-- html引入-->
      <div ms-widget="uploadnew,$,uploadnew"></div>
````
#### 配置方式：
````js
// 在定义avalon模板前 
 var uploadnewVM= null;

//组件配置
   uploadnew:{
     downUrl:'/App/Invoicimg/static/moban.xls',  //下载模板地址
     uploadUrl:'/index.php?app=Invoicimg_Suppliers&m=Product&a=suppliesLoade_new' // 导入exexl后台php处理路径
     onInit: function(vmodels){
         uploadnewVM= vmodels ;

     }
   }
````
#### 注意事项:

## 1. 导入提交的方式 'post' 
````js
后台接受参数   path   //导入文件的路劲

````

## 2. 后台处理数据后的返回格式
````js

      $result['wrongData']['data']=$wrongData;  //错误数据
      $result['wrongData']['header']=array('原料编码/料号','原料名称/品名规格','原料分类','供应商','成本','单位','备注','错误提示');   //导出文档的表头
      $result['wrongData']['title'] ='原料错误数据导出'; //导出文件名 
      $result['wrongData']['list']  ='H';              //显示错误的单元格列
      $result['rightnum'] =$rightnum;                  //导入成功的数量
      $result['wrongnum'] =$wrongnum;                  //导入失败的数量
      $result['status']=1;                                
      $result['type']=1;     // 1 非严格模式，成功导入，错误导出；   0 只要出现错误就返回  


````


### **判断是否有下属**

### **请求接口**
/index.php?app=Customer&m=MLegwork&a=getZhiweiLeader




### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Legwork&m=MLegwork&a=getZhiweiLeader&access_token=

http://www.apps.com/index.php?app=Legwork&m=MLegwork&a=carcustom   //汽车客户列表

http://www.apps.com/index.php?app=Legwork&m=MLegwork&a=isopen   //判断客户和汽车客户管理应用是否开启


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string  |请求状态         |
|info       |   有下属 /没有下属   |string  |      |


``` javascript

{
info: "没有下属",                            
status: "error",                     
}




{
count: "81",      //总条数
totalPages: 5,    //页数
nowPage: 1,       //当前页
data:[
  {
     id: "7",      
     name: "test9",        //客户名称
     phone: "13349888009",  //电话
     source_id: "2",
     nsale_id: "1",
     orginal_status: "5",  
     source: "老客户介绍",   //来源
     status: "已成交",      //状态
     sale_name: "庆丰包子",   //负责人
     time: "03-29 16:48",    //创建时间
     app: "Car"
   }
]
}

************判断客户和汽车客户管理应用是否开启*******************
{
Customer: 1,
Car: 1
}
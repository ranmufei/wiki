### **我的客户列表**

### **请求接口**
/index.php?app=Customer&m=MLegwork&a=custom_list

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MLegwork&a=custom_list&lng=114.279249&lat=30.55&access_token=
### **公共参数** 
`p`

### **其他参数**
lng(签到的经度)lat(签到的维度)

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |请求状态         |
|data       |array         |array  | count:总数据量 , totalPages:总页数 ， nowPage:当前页 , data:[]数据列表(具体查看以下代码) |
|info       | '' | string | 接口状态说明  |

``` javascript
{
data: {
     count: "3",
     data: [
       {
             id: "386",
             custom_company: "uuuuu",
             lng: "114.279249",
             lat: "30.563056",
             custom_address: "湖北省 武汉市 汉阳区 龟山北路 8号"
       }
    ]
},
info: "",
status: "success"
}

### **我的联系人**
### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MLegwork&a=contacts_list&access_token=
### **公共参数** 
`p`



``` javascript
{
    data: {
      count: "70",
      totalPages: 3,
      nowPage: 1,
      data: [
            {
                 id: "211",
                 custom_id: "382",
                 name: "GSD555",
                 custom_val: "wwwww"
              }
      ]
    },
    info: "",
    status: "success"
}
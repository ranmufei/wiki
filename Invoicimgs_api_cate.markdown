### **请求接口**
/index.php?app=Invoicimg_Suppliers&m=ProductApi&a=getCate

### **接口说明**
`无分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg_Suppliers&m=ProductApi&a=getCate&access_token=e133ac84d35628422ca6c2c408667a

### **参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data      |         | array |返回数组 |


``` javascript
{
data: [
{
id: "1",//分类id
name: "原料" //分类名
},
{
id: "3",
name: "辅料"
}
]
}
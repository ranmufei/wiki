### **请求接口**
/index.php?app=Invoicimg&m=InstockApi&a=get_storage_info

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=get_storage_info&ckid=1&access_token=e133ac84d35628422ca6c2c408667a

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|ckid       |              |string |仓库id|
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data|         | object |仓库基本信息数组 |
|storage|         | aray | 库位信息|


``` javascript
{
statu: 1,
info: "仓库信息",
data: {
id: "1",
storehouse: "武汉仓库",
pym: "",
mark: "武汉3",
defaultStore: true,
admin: "老梁",
adminPhone: "158241714510",
storeAddress: "龟北路30懂t",
isdelete: "0",
default1: "0",
defualt2: "0",
defaultT1: "0",
defaultT2: "0"
},
storage: [
{
id: "27",
storehouse: "库位C",
pym: "",
mark: "建材",
defaultStore: "1",
admin: "",
adminPhone: "0",
storeAddress: null,
isdelete: "0",
default1: "1",
defualt2: "0",
defaultT1: "0",
defaultT2: "0"
},
{
id: "28",
storehouse: "库位B",
pym: "",
mark: "房地产",
defaultStore: "0",
admin: "",
adminPhone: "0",
storeAddress: null,
isdelete: "0",
default1: "1",
defualt2: "0",
defaultT1: "0",
defaultT2: "0"
}
]
}
### **请求接口**
/index.php?app=Invoicimg&m=InstockApi&a=get_storn_list

### **接口说明**
`无分页`


### **浏览器查看**
获取仓库列表 /http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=get_storn_list&access_token=

获取仓库列表 /http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=get_storage_list&ckid=1&access_token=
### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|ckid|         | int|仓库id |

### **其他参数**
| --------- |--------      |--------|--------       |
|isParent      |         | int|1 有库位 0 无库位 |
### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data      |         | array |返回数组 |

### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=share_lists

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=share_lists

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   用户id   |
| p | 是 |   本接口传入此参数表示分页,不传表示默认第一页 |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|info       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|id         |              |int    |文件（夹）唯一ID  |
|name       |              |string |文件（夹）名称   |
|size       |              |String |文件大小  |
|inputtime  |              |int    |文件（夹）创建时间 |
|file_extension |          |String |文件类型id |
|type       |              |int    |file or folder |


### 实例

``` javascript
{
status: "success",
info: [
{
id: "261",
name: "工作流应用测试模板 (王子超).doc",
inputtime: "1970-01-01 08:33",
type: "file",
file_extension: "4",
size: "167.5 K",
downloadUrl: "http://1.03in.com:8082/./Uploads/2015/0528/09/55666f1f26187.jpg",
},

{
id: "234",
name: "GoAgentCT.rar",
inputtime: "1970-01-01 08:33",
type: "file",
file_extension: "99",
size: "7.4 M",
downloadUrl: "http://1.03in.com:8082/./Uploads/2015/0528/09/55666f1f26187.jpg",
}
]
}

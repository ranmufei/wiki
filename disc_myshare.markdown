### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=getMyShare

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=getMyShare

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   用户id   |
| p | 是 |   本接口传入此参数表示分页,默认第一页 |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|info       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|id         |              |int    |文件（夹）唯一ID  |
|name       |              |string |文件（夹）名称   |
|size       |              |String |文件大小  |
|inputtime  |              |int    |文件（夹）创建时间 |
|file_extension |          |int |文件类型id |
|type       |              |string    |文件（夹）类型file or folder |
|share_name |              |string    |文件（夹）分享人 |
|size|              |string    |文件大小 |
|downloadUrl|              |string    |文件下载地址 |


### 实例

``` javascript
{
status: "success",
info: [
{
id: "263",
name: "文件夹",
inputtime: "2015-06-09 10:20",
type: "folder",
file_extension: "",
size: "",
},
{
id: "261",
name: "工作流应用测试模板 (王子超).doc",
inputtime: "1970-01-01 08:33",
type: "file",
file_extension: "4",
size: "167.5 K",
},
{
id: "237",
name: "QQ截图2015050515140'4.png",
inputtime: "1970-01-01 08:33",
type: "file",
file_extension: "1",
size: "24.4 K",
},
{
id: "234",
name: "GoAgentCT.rar",
inputtime: "1970-01-01 08:33",
type: "file",
file_extension: "99",
size: "7.4 M",
}
]
}

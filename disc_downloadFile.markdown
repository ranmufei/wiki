### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=uploadify

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=downloadFile

### **请求参数**

| 参数名称   |必填 |     说明   |
|----------- |-----|------------|
| idstr        | 是  |   文件id集合（1,2,3）   |

### **如果有错误，返回结果 不然直接下载**
|字段       |值             |类型    |说明        |
| --------- |--------       |--------|--------   |
|status     |success/error|string  |返回状态    |
|info       |               |array  |    |

### 实例

``` javascript
{
status: "success",
info: [
{
file_id: "250",
file_name: "文档1.doc",
downloadUrl: "http://1.03in.com:8082/./Uploads/2015/0610/11/5577b24c4c45b.doc"
},
{
file_id: "251",
file_name: "文档1.doc",
downloadUrl: "http://1.03in.com:8082/./Uploads/2015/0610/11/5577b418d1146.doc"
}
]
}


{
status: "error",
info: {
errorDesc: "未查找到文件数据"
}
}
### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=company_lists

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=company_lists

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid  |  是 |   用户id   |
| folder_id     | 是 |   目录id   |
| p | 是 |   本接口传入此参数表示分页 |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|id         |              |int    |文件（夹）唯一ID  |
|name       |              |string |文件（夹）名称   |
|file_type  |              |string |folder=文件夹 file=文件   |
|inputtime  |              |string |创建时间   |
|isAdministrator  |        |int    |是否为管理员（1=是 2=否）当folder_id=0,isCreater可以进行创建目录 删除等操作 不可上传文件 当folder_id > 0,isAdministrator可以进行创建目录 删除 上传等操作 isCreater是isAdministrator的上级 拥有isAdministrator的所有权限  |
|isCreater  |              |int    |是否为创建人（1=是 2=否）   |
|file_extension|           |string |文件扩展名|
|is_image   |              |int    |是否为图片（1=是 2=否）|
|downloadUrl|              |string |下载链接|
### 实例

``` javascript
folder_id > 0
{"data":[{"id":"3","name":"\u7ba1\u7406\u54581","inputtime":"2015-12-01 10:46:56","file_type":"folder"},{"id":"2","name":"55822356.jpg","inputtime":"2015-11-28 17:47:48","file_type":"file","is_image":"1","file_extension":"jpg"}],"info":"{\"isCreater\":0,\"isAdministartor\":1}","status":"success"}

folder_id = 0
{"data":[{"id":"1","name":"\u7ba1\u74061","inputtime":"2015-11-28 16:27:49","file_type":"folder"}],"info":"{\"isCreater\":0,\"isAdministartor\":0}","status":"success"}
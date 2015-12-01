### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=xxxxx

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=xxxxx

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| folder_id     | 是 |   目录id   |
| p | 是 |   本接口传入此参数表示分页 |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|info       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|id         |              |int    |文件（夹）唯一ID  |
|name       |              |string |文件（夹）名称   |
|file_type  |              |string |folder=文件夹 file=文件   |
|inputtime  |              |int    |创建时间   |
|isAdministrator  |        |int    |是否为管理员（1=是 2=否）当folder_id=0,isCreater可以进行创建目录 删除等操作 不可上传文件 当folder_id > 0,isAdministrator可以进行创建目录 删除 上传等操作   |
|isCreater  |              |int    |是否为创建人（1=是 2=否）   |
### 实例

``` javascript

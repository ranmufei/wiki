### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=Appaccessory

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=_REQUEST

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   用户id   |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|id         |              |int    |文件（夹）唯一ID  |
|name       |              |string |文件（夹）名称   |
|size       |              |String |文件大小  |
|inputtime  |              |int    |文件（夹）创建时间 |
|file_extension |          |String |文件类型id |
|type       |              |int    |file or folder |


### 实例

``` javascript

{"count":0,"folders_count":6,"data":[{"file_type":"folder","folder_node_id":1,"id":"1","inputtime":"2016-09-06 14:57:37","name":"\u4f01\u4e1a\u5fae\u5708","type":"folder","file_extension":"","icon":"icon-folder","size":"","imgUrl":"","file_extension_icon":""},{"file_type":"folder","folder_node_id":1,"id":"4","inputtime":"2016-09-06 15:00:21","name":"\u9879\u76ee\u7ba1\u7406","type":"folder","file_extension":"","icon":"icon-folder","size":"","imgUrl":"","file_extension_icon":""},{"file_type":"folder","folder_node_id":1,"id":"10","inputtime":"2016-12-02 10:32:36","name":"\u8fdb\u9500\u5b58","type":"folder","file_extension":"","icon":"icon-folder","size":"","imgUrl":"","file_extension_icon":""},{"file_type":"folder","folder_node_id":1,"id":"13","inputtime":"2016-12-02 10:45:10","name":"\u62a5\u9500\u7ba1\u7406","type":"folder","file_extension":"","icon":"icon-folder","size":"","imgUrl":"","file_extension_icon":""},{"file_type":"folder","folder_node_id":1,"id":"18","inputtime":"2016-12-02 11:22:48","name":"\u9500\u552e\u7ba1\u7406","type":"folder","file_extension":"","icon":"icon-folder","size":"","imgUrl":"","file_extension_icon":""},{"file_type":"folder","folder_node_id":1,"id":"79","inputtime":"2017-03-22 20:10:27","name":"\u90ae\u7bb1\u4ee3\u7406","type":"folder","file_extension":"","icon":"icon-folder","size":"","imgUrl":"","file_extension_icon":""}]}
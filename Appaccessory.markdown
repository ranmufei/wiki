### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=Appaccessory

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=Appaccessory

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
|file_extension_icon|              |string|文件类型图片 |
|imgUrl|              |string|文件缩略图 |


### 实例

``` javascript

{"count":0,"folders_count":6,"data":[{"id":"1","name":"\u4f01\u4e1a\u5fae\u5708","inputtime":"2016-09-06 14:57:37","type":"folder","file_extension":"","icon":"icon-folder","size":"","imgUrl":"","file_extension_icon":""},{"id":"4","name":"\u9879\u76ee\u7ba1\u7406","inputtime":"2016-09-06 15:00:21","type":"folder","file_extension":"","icon":"icon-folder","size":"","imgUrl":"","file_extension_icon":""},{"id":"10","name":"\u8fdb\u9500\u5b58","inputtime":"2016-12-02 10:32:36","type":"folder","file_extension":"","icon":"icon-folder","size":"","imgUrl":"","file_extension_icon":""},{"id":"13","name":"\u62a5\u9500\u7ba1\u7406","inputtime":"2016-12-02 10:45:10","type":"folder","file_extension":"","icon":"icon-folder","size":"","imgUrl":"","file_extension_icon":""},{"id":"18","name":"\u9500\u552e\u7ba1\u7406","inputtime":"2016-12-02 11:22:48","type":"folder","file_extension":"","icon":"icon-folder","size":"","imgUrl":"","file_extension_icon":""},{"id":"79","name":"\u90ae\u7bb1\u4ee3\u7406","inputtime":"2017-03-22 20:10:27","type":"folder","file_extension":"","icon":"icon-folder","size":"","imgUrl":"","file_extension_icon":""}]}
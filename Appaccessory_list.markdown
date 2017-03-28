### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=Appaccessory_list

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=Appaccessory_list

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   用户id   |
| folder_id| 是 |  文件夹id   |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|id         |              |int    |文件（夹）唯一ID  |
|name       |              |string |文件（夹）名称   |
|size       |              |String |文件大小  |
|inputtime  |              |string    |文件（夹）创建时间 |
|file_extension |          |String |文件类型id,文件类型（1=图片 2=音乐 3=视频 4=文件） |
|type       |              |string    |file or folder |
|file_extension_icon|              |string|文件类型图片 |
|imgUrl|              |string|文件缩略图 |
|icon|              |string|文件夹标示图,文件夹类型返回此字段 |
|downloadUrl|              |string|文件下载地址，文件类型返回此字段 |
|preview_url|              |string|文件类型返回此字段 |

### 实例

``` javascript

{"count":1,"folders_count":0,"data":[{"name":"\u5ba3\u4f20\u518c-6.jpg","id":"11380","type":"file","inputtime":"2016-09-06 14:57:20","file_extension_icon":".\/App\/Wangpan\/static\/images\/jpg.png","file_extension":1,"imgUrl":".\/Uploads\/2016\/0906\/14\/57ce68d0e838d.jpg","downloadUrl":"http:\/\/www.apps.com\/Uploads\/\/2016\/0906\/14\/57ce68d0e838d.jpg","preview_url":".\/Uploads\/\/2016\/0906\/14\/57ce68d0e838d.jpg","size":"449.1 K"}]}
### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=classify_share_lists

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=classify_share_lists

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   用户id   |
| classify_id | 否 |   1=图片 2=音乐 3=视频 4=文档 5=文本 99=其它|
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
|file_extension |          |String |文件扩展名 |
|share_name|          |String |分享人 |
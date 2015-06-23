### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=folder_lists

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=folder_lists

### **请求参数**

| 参数名称   |必填 |     说明   |
|----------- |-----|------------|
| uid        | 是  |   用户id   |
| folder_id   | 否  |   目录id，没有则为0   |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|info       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|id         |              |int    |文件（夹）唯一ID  |
|name       |              |string |文件（夹）名称   |


{
status: "success",
info: [
{
id: "267",
name: "xxxx"
},
{
id: "266",
name: "新建文件夹1111"
},
{
id: "261",
name: "wangzichao"
},
{
id: "259",
name: "vvvvvvvvvvv"
},
{
id: "246",
name: "46464"
},
{
id: "236",
name: "无敌测试"
},
{
id: "119",
name: "22222"
},
{
id: "118",
name: "1111121212"
},
{
id: "42",
name: "北北"
},
{
id: "40",
name: "马露特"
},
{
id: "35",
name: "哈哈哈哈"
}
]
}

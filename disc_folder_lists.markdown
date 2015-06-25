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
|inputtime       |              |string |时间   |

### 实例

``` javascript
{
status: "success",
info: [
{
id: "267",
name: "xxxx",
inputtime: "2015-06-16 10:07:32"
},
{
id: "266",
name: "新建文件夹1111",
inputtime: "2015-06-12 11:56:38"
},
{
id: "261",
name: "wangzichao",
inputtime: "2015-06-08 17:02:43"
},
{
id: "259",
name: "vvvvvvvvvvv",
inputtime: "2015-06-04 21:43:34"
},
{
id: "246",
name: "46464",
inputtime: "2015-06-03 19:28:10"
},
{
id: "236",
name: "无敌测试",
inputtime: "2015-06-03 18:56:26"
},
{
id: "119",
name: "22222",
inputtime: "2015-05-28 10:23:33"
},
{
id: "118",
name: "1111121212",
inputtime: "2015-05-28 10:23:23"
},
{
id: "42",
name: "北北",
inputtime: "2014-05-26 18:22:39"
},
{
id: "40",
name: "马露特",
inputtime: "2014-05-26 18:02:34"
},
{
id: "35",
name: "哈哈哈哈",
inputtime: "2014-05-26 18:01:13"
}
]
}
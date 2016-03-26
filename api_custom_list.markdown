# PublicCustomid/custom_list
----
获取公司基本信息
## URL
----
https://www.apps.com/index.php?app=Customer&m=Precustom&a=cshi
## 支持格式
----
* JSON
## HTTP请求方式
----
GET/post



### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|count      |              |int|客户的总数量         |
|totalPages|       |int|总页数   |
|nowPage|  | int | 当前页  |
|data   | '' | array(数组)| 数据列表(具体查看以下代码)  |

           
``` javascript
data: [
{
id: "277"                       //客户ID
custom_company: "武汉大学",    //客户名称
level :''                     //重要级别
apportion_id: "庆丰包子"      //负责人
custom_type: "代理商",        //客户类型
company_phone: "1852364595"    //电话          
is_leave: "0"                //是否离职  ，1为离职（庆丰包子（离职））,0为（庆丰包子）   

},
.....
]

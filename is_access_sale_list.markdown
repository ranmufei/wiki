## 首页 管理管理 今天所有日程
### **请求接口**
/index.php?app=Invoicimg&m=SaleMobile&a=is_access_r

/index.php?app=Account&m=ExpenseApi&a=select_auditlist&apps=Sale&ms=Index&as=audit 选择的审核人列表

### **接口说明**
无需传参数


### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=is_access_r&access_token=




### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|statu      |1/0 | int   |返回结果 1显示有权限的栏目（销售订单、退货订单、对账单）        |
|data       |  ''  |       | |
|info       | 'ok/error' | string |   |

``` javascript
[
{
uid: "753",
audit: "753",       //审核人的id
name: "冉帅91",     //名称
zname: "无职位",    //职位
img: "./Uploads/avatar/default.gif"   //头像
}
]
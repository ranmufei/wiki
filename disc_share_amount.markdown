### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=share_amount

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=share_amount

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   用户id   |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status       |success      |  |成功  |
|info       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |



### 实例

``` javascript
{
status: "success",
info: {
all: "(0)",
picture: "(0)",
word: "(0)",
txt: "(0)",
other: "(0)"
}
}
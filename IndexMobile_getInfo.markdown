### **请求接口**
index.php?app=Car&m=IndexMobile&a=getInfo


### **公网测试**
http://www.apps.com/index.php?app=Car&m=IndexMobile&a=getInfo&access_token=

### **请求方式**
get


### **参数**
无

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|data|-------   |array  |首页提醒  |

经理：

    addno: "0",            需要建卡的接待记录
    passaddno: "0",        逾期未建卡的接待记录
    tracknum: "0",         需要跟进的客户
    visit: "0",            需要回访的客户
    trackno: "2",          无跟进计划的客户
    weitrack: "7",         逾期未跟进的客户
    visitno: "2",          逾期未回访的客户
    defeatno: "6",         需要处理的战败请求
    recepnum: "0",         接待客户批次
    finish: "1"            成交客户

销售顾问：

    recepnum: "10",         接待客户批次
    finish: "0",            成交客户
    needrecep: "0",         需要处理的接待记录
    needpassrecep: "8",     逾期未处理的接待记录
    tracknum: "0",          需要跟进的客户
    weitrack: "2",          逾期未跟进的客户
    needVisit: "0",         需要回访的客户
    novisit: "16",          逾期未回访的客户
    trackno: "2",           无跟进计划客户
    defeatnum: "0"          战败请求

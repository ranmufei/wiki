### **请求接口**
/index.php?app=Asset&m=AsserApi&a=right_view



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=right_view

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| id     | 是 |   申请列表的id   |


### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|apply        |-------   |int    |所申请的编号信息   |
|state| -------     |varchar  |申请物品状态      |
|applymen|-------     |varchar   |申请人名称    |
|goods| -------     |   varchar        | 申请该物品的详细信息（参照易耗品物品列表字段）|



### **示例**
````php
{
apply: {
0: "ls_59150035093",
1: "ls_59751335092",
2: "ls_59835335091",
state: "待审批",
applymen: "庆丰包子"
},
goods: {
id: "59",
number: "shenzhu_00211",
names: "电脑",
type: "",
num: "3",
already_num: "0",
unit: "",
remark: "电脑",
gunit: "4",
cateid: "2",
buytime: "1430561178",
ntime: "1425312000",
old: "",
is_old: "2",
is_delete: "1",
cat: "外接",
one: "",
two: "",
three: "",
price: "3652",
now_tprice: "0",
img: "./Uploads/2015/0502/18/5544a19a129a2.jpg"
}
}
### **请求接口**
/index.php?app=Asset&m=AsserApi&a=asset_serch



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=asset_serch

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| type     | 是 |   搜索的类型1.为易耗品 2.为申租品   |
| data| 是 |   搜索的类容   |




### **示例**
````php

data: [
{
id: "1",
number: "sz_20151026102229",
names: "测试电脑",
type: null,
num: "8",
already_num: "3",
unit: null,
remark: "范德萨范德萨",
gunit: "台",
cateid: "2",
buytime: "1445826942",
ntime: "1433347200",
old: null,
is_old: "2",
is_delete: "1",
cat: "其他",
one: null,
two: null,
three: null,
price: "102.1",
now_tprice: null,
img: "./Uploads/2015/1026/17/562df05fea3d8.jpg",
supplier: "请选择供应商",
loca: "仓库",
good_type: "A-124",
branch: "公关",
keeper_uid: "337",
online: "0",
offline: "0",
good_status: "完好"
},
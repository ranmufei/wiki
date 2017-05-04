### **请求接口**
index.php?app=AfterSalers&m=FxdMobile&a=fenpeiClue



### **公网测试**
http://www.apps.com/index.php?app=AfterSalers&m=FxdMobile&a=fenpeiClue&access_token=

### **请求方式**
post


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| ids| 是 |array 选择的维修单id（选择了一个维修单也是以数组传）|
| cate_id| 是 |分类id|
| cate_per| 是 |分类负责人|

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
$res['info']="线索分配成功!";
$res['status']=1;


$res['info']="线索分配失败!";
          $res['status']=0;
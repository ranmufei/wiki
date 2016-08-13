### **请求接口**
index.php?app=Car&m=DefeatMobile&a=defeatInfo



### **公网测试**
http://www.apps.com/index.php?app=Car&m=DefeatMobile&a=defeatInfo&access_token= 

### **请求方式**
get


### **参数**
|参数        |必填          |类型    |说明        |
| ---------  |--------    |-------- |--------  |   
|perPages|否  |int  |每页显示条数 默认10  |
|status|否  |int  |1 显示全部  |

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|data|-------   |array  |战败列表  |

      data['data']：array  战败列表
            
            id                战败表id
            client_id         客户id
            phone             电话
            reason            主要原因
            apply_time        申请时间
            defeat_explain    战败说明
            brand_id          意向车型
            process_time      处理时间
            status            处理状态  7 新建  8 驳回  9 同意  10 分配其他
            sale_name         销售顾问

      data['sale']:array 销售顾问列表
            
           uid   销售顾问id
           name  销售顾问姓名
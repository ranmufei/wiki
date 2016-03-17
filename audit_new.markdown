# **审核/消息新消息 数量、最近一条的标题**


### **请求接口**
/index.php?app=Home&m=AuditApi&a=getNewsCount


### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   员工id   |
| cid     | 是 |   公司id   |







## 返回结果
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|ywCount.count     | 0 |num |  新消息数量    |
|ywCount.data       |最新的一条标题        |string  |count =0时此值为空    |
|bgCount.count     | 0 |num |  新消息数量    |
|bgCount.data       |最新的一条标题        |string  |count =0时此值为空    |
|xxCount.count     | 0 |num |  新消息数量    |
|xxCount.data       |最新的一条标题        |string  |count =0时此值为空    |
|rcCount.count     | 0 |num |  新消息数量    |
|rcCount.data       |最新的日程一条标题        |string  |count =0时此值为空   20160223新加   |
|myCount.count     | 0 |num |  新消息数量    |
|myCount.data       |我发起的未审核的最新的一条标题        |string  |count =0时此值为空   20160317新加   |
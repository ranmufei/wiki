# 客户管理API接口列表

### **公共**
 - [选择客户](public_custom_list)

### **首页**
 - [客户管理今天所有日程](index_schedule_list) 
 
### **售前管理**
#### 线索管理
 - [线索列表(我的)](pre_thread_list)
 - [新增](pre_thread_add)
 - 详细信息
  - [线索动态](pre_thread_dynamics)
  - [资料](pre_thread_info)
  - [日程](pre_thread_schedule)
  - [转为客户](pre_thread_convert)
 - [新增线索日程](pre_thread_schedule_add)
 - [转移给他人](pre_thread_giveto)(NEW 四个接口线索、客户、联系人、机会)
 - [修改](pre_thread_edit)

#### 客户管理
 - [我的客户列表](pre_custom_list)
 - [新增](pre_custom_add)
 - 详细信息
  - [客户动态](pre_custom_dynamics)
  - [资料](pre_custom_info)
  - [联系人列表](pre_custom_contacts_list)
  - [机会列表](pre_custom_chance_list)
  - [日程](pre_custom_schedule)
  - [收货地址](pre_custom_address)
  - [联合跟进人列表](pre_custom_share)(new 三个接口)
  - [选择已有联系人、机会关联联系人](pre_custom_lxr_add)(new 两个接口)
 - 其他
  - [查询客户](pre_custom_search_like)
  - [全部客户分类](pre_custom_type_list)
 - [新增客户日程](pre_custom_add_schedule)
 - [修改](pre_custom_edit)

#### 联系人管理   
 - [我的联系人列表](pre_contacts_list)  
 - [新增联系人](pre_contacts_add)
 - 详细信息
  - [客户动态](pre_contacts_dynamics)
  - [资料](pre_contacts_info)
  - [机会列表](pre_contacts_chance)
  - [日程](pre_contacts_schedule)
 - [新增联系人日程](pre_contacts_add_schedule)
 - [修改](pre_contacts_edit)
 - [取消关联客户](pre_contacts_del_relate)（NEW）
 

#### 机会管理   
 - [我的机会列表](pre_chance_list)  
 - [新增机会](pre_chance_add)
 - 详细信息
  - [客户动态](pre_chance_dynamics)
  - [资料](pre_chance_info)
  - [日程](pre_chance_schedule)
  - [跟进记录](pre_chance_record_list)
 - [新增机会日程](pre_chance_add_schedule)
 - [修改](pre_chance_edit)
 - [机会通过、驳回、赢单、战败申请操作](pre_chance_operate)


#### 动态   
 - [新增动态(客户、线索)](pre_dynamics_add) 

#### 添加   
 - [关联(联系人的共享联系人、客户的联合跟进人、机会的联合跟进人)](pre_relate_add)

### **售中管理**

#### 订单管理  
  - [我的订单列表](mid_order_list)
  - 详细信息
   - [资料](mid_order_info)
   - [支付详情](mid_order_payinfo) 

### **报表**
  - [销售机会阶段](report_chance_state)
  - [客户类型](report_custom_all)
  - [订单时段](report_order_time)
  - [新增客户](report_add_custom)

### **外勤签到**
 - [添加](add_legwork) 
 - [附近的客户（2000米）](custom_list) 
 - [外勤签到列表](legwork_list) 
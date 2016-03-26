# 元数据接口列表

> 元数据接口列表 在此整理。 

## 公司基础数据

| 权限 | 接口名称 |  接口  |  接口描述  |
|:-- | :-- | ----:| :--: |
|读| [公司信息](company_info) | [/v1/company/info](company_info)  | 公司基本信息 |
|读| [公司员工列表](user_list)| [/v1/user/list](user_list)  | 公司员工列表  |
|读| [公司员工详细信息](user_userinfo) | [/v1/user/userinfo/12](user_userinfo)  | 公司员工具体信息  |
|读| [公司部门列表](department_list) | [v1/department/list](department_list) |公司部门列表|
| 读|[公司部门详细](department_info) | [v1/department/info](department_info) |公司某部门详细|

## 客户基础数据
| 权限 | 接口名称 |  接口  |  接口描述  |
|:-- | :-- | ----:| :--: |
|读| [客户名称](custom_name)|Custom/get_custom_name| 通过客户id获取客户名称 |
|读| [客户资料](custom_info)|PublicCustom/getInfo | 通过客户id获取客户资料  |
|读| [客户列表](api_custom_list)|PublicCustomid/custom_list  | 客户列表 |

## 在线会计--科目--基础数据
| 权限 | 接口名称 |  接口  |  接口描述  |
|:-- | :-- | ----:| :--: |
|读| [科目列表](treasurer_cate)|[Treasurer/getSubjectList](treasurer_cate)| 获取科目列表信息 |
|读| [科目详情](treasurer_cate_detail)|[Treasurer/getSubjectDetail](treasurer_cate_detail)| 通过科目编码或科目名称获取科目详情信息  |
|读| [辅助核算列表](treasurer_accounting)|[Treasurer/getSubjectAccounting](treasurer_accounting)| 辅助核算列表信息 |
|读| [辅助核算详情信息](treasurer_accounting)|[Treasurer/getSubjectAccountingDetail](treasurer_accounting_detail)| 辅助核算详情信息 |
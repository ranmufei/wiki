调用 公共数据 的模型
apppublic/apppublic

**`本 模块文件 和应用父窗体的公共布局文件耦合`**

**@version 20160527 建议使用 [系统设置的全局数据调用](pcd_system_to_globaldata)** 

| 接口名称  | 类型 | 参数  |说明     |
| :--------  |  ------- | ------| -------- |
|windows | function | id : 对窗口的唯一性标识 ;url:窗口地址; name:窗口名称; title:窗口描述; lock:是否锁定 | 新窗口配制参数|
|appinfo`不建议使用` | object || 当前应用信息 |
|login(`不建议使用`)| object || 登录者信息 |
|company`不建议使用`| object || 公司信息 |
|pages`不建议使用`|object|| 分页信息 |
|others|object||预留接口|


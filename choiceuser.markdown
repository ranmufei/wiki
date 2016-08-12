`<div ms-widget="choiceuser"  ></div>`   
可以使用duplex双绑， 不建议使用duplex 双绑，建议用getChoiceData（）获取现在的员工;    
 require(["choiceuser/avalon.choiceuser"], function() {});

| 参数名称  |     类型|  默认值  |说明     |
| :--------  |  ------- | ------| -------- |
|mix      | string| 1 | 选择的职员数量|
|depart| boolean| true | 是否可以选择部门|
|tipText|string|"选择发送范围…"|默认显示的文本|
|placeholder|string|"输入同事或部门名称"|搜索表单显示的文本|
|privilege| boolean|false |是否选择有权限的员工 |
|open| function|  | 打开选择员工下拉框 |
|getChoiceData| function| |获取选择的员工 |



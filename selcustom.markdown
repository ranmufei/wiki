<input type="text" ms-widget="selcustom" ms-duplex="customval" />
选择客户可以使用duplex双关绑定 或用户自己 通过回调处理选择的客户

| 参数名称  |     类型|  默认值  |说明     |
| :--------  |  ------- | ------| -------- |
|mix      | string| 1 | 选择的客户数量|

|isparent | boolean| false  | 是否只允许选择顶级公司 |

|sureCallback| function | null | 选择客户确认后的回调函数 |
|onInit| function| null | 组件初始化后的回调 |
| triTemplate | string | null | 触发组件的模块 |
|dialog| object | {} | 尽量不要修改该参数 | 
|smartgrid| object | {} | 尽量不要修改该参数 |


`<input type="text" ms-widget="optmember" ms-duplex="memberval" />`

可以使用duplex双关绑定 或用户自己 通过回调处理选择的职员

| 参数名称  |     类型|  默认值  |说明     |
| :--------  |  ------- | ------| -------- |
|mix      | string| 1 | 选择的客户数量|
|width | int| 450  | 组件宽度 |
|height| int| 250 | 组件高度 |
|expand| boolean| true | 默认是否展开 所有部门|
|aline| ele | null | 人员选择框 对齐的对象|
|boolBodyClickHide | boolean | true | 点击body其他部分是否关闭组件 | 
|onInit|function|null|组件初始化后的回调|
|itemChange| function| {} | 选中队列发生改变的回调 |


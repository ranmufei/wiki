现金流 对 其他应用 提供现金交易 及 订单 审核 的功能接口。
`考虑应用的复杂性及扩展性，应用为每一种现金流来源创建一种工厂，用来区别现金流来源，现金流的接口只有那么几个 : 创建、审核、现金交易详细、查看详情，开发者通过接口调用自己的工厂，就可以使用以上接口了`

<strong>接口列表</strong>

| 参数名称  |     类型|  默认值  |说明     |
| :--------  |  ------- | ------| -------- |
|mix      | string| 1 | 选择的职员数量|
|width | int| 450  | 组件宽度 |
|height| int| 250 | 下拉选择panel高度 |
|expand| boolean| true | 默认是否展开 所有部门(`废弃`)|
|aline| ele | null | 人员选择框 对齐的对象(`废弃`)|
|boolBodyClickHide | boolean | true | 点击body其他部分是否关闭组件 (`废弃`)| 
|onInit|function|null|组件初始化后的回调|
|itemChange| function| {} | 选中队列发生改变的回调 |
|getTemplate| function| |修改模板 |
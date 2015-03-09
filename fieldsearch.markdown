`<input type="text" ms-widget="fieldsearch" ms-duplex="searval" />`

可以使用duplex双关绑定 或用户自己 通过回调处理选择的职员

| 参数名称  |     类型|  默认值  |说明     |
| :--------  |  ------- | ------| -------- |
|items | array| [] | 不能为空|初始化检索条件|
|field| array| []  | 检索字段数据, [ { key : 'company' , name : '公司名称' , search : 'option' , option : [ '国有企业' , '外资企业' , '合资企业' ]  } ,{ key : 'contact' , name : '联系人' , search : 'string' } ]如果 option 里的元素是对象类型，默认会将第一个属性 当成 <option>标签 的 value  第二个属性当作<option>的显示字串 |
|onInit|function|null|组件初始化后的回调|
|getSearchRet| function| {} | 点击确认后的回调 参数为查询条件组成的数组 |


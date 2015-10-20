`<div ms-widget="logistics"></div>`


define(['logistics/logistics'], function(){})

| 参数名称  |     类型|  默认值  |说明     |
| :--------  |  ------- | ------| -------- |
|status| int| 1,2,3 | 1：进销存，2：连锁经营，3：电商|
|array| array | ['1'] | 单个订单发货的判断 | 
|onInit|function|null|组件初始化后的回调|
|datainfo|array|['1']|单个订单发货需要更新的数组|
|SetData|function（需要修改传递的数组）||调用重新赋值的函数|
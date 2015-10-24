`<div ms-widget="maintenance"></div>`

define(['maintenance/avalon.maintenance'], function(){})

| 参数名称  |     类型|  默认值  |说明     |
| :--------  |  ------- | ------| -------- |
|onInit|function|null|组件初始化后的回调|
|callbackfun|function|null|组件调用操作成功后的回调|
|datainfo|array|[]|单个订单发货需要更新的数组|
|SetData|function(gid,cat_id)||调用重新赋值的函数|
|_open|function()||触发组件layer弹出层|

配置案例
,$maintenance:{
   onInit:function(vm){
     maintenanceVM=vm;
   },
   callbackfun:function(data){
	avalon.log('回调数据',data);
   },
  
}
# 云采购产品选择组件 choseproduct/choseproduct

## 说明

  > 供全局调用 新建Avalon 弹出层 选择产品

## 使用方法

  > 引入 Avalon组件地址 choseproduct/choseproduct


``` javascript
/**
* test
* 
*/
require(['avalon','jquery','layer/layer','avalon/choseproduct/choseproduct'], function(avalon,$,layer) {
	var tabProduct=[];
	var choseproductVM =[];
	var tab = avalon.define({
			$id: 'test',
			$skipArray: ["smartgrid",'tree'],
			
			choseproduct:{
				//初始化函数，定义组件model
				onInit:function(vmodel){
					choseproductVM=vmodel;
				},
				callbackfun:function(data){

					console.log('返回我得到的数据',data);
				}
			},


    })

 avalon.scan();

})
```


##  接口方法

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|callbackfun()|否| 分类修改 删除 增加后  自动回调函数  |


## 案例html 


```
  <div class="main-body">
   
      <div ms-widget="choseproduct">调用组件</div>

  </div>
 <script src="__PUBLIC__/src/js/order/text.js"></script>

```






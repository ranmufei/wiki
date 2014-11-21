# 选择发货地址控件

## 调用函数

 >   {:widget('ChoiceAddress',array('cid'=>$data['custom_id'],'where'=>0,'callbackfun'=>'ds'))}
 
     


## 参数解释 

 - cid : 客户cid  
 - where : 来源 0/1  网络客户/本地添加
 - callbackfun : 自定义回调函数

## 回调函数参数解释

> 回调函数参数 为地址对象

*回调函数返回数据参考

``` javascript
address: "湖北省武汉市武昌区街道口10号"
adds: function () {
name: "张耀辉"
phone: "24587454"

```
## 回到函数 案例参考

``` javascript
 <script>
      function ds(data){
		  console.log(data);
		  $('#contact').val(data['name']);
		  $('#phone').val(data['phone']);
		  $('#suppliers').val(data['address']);
		   $('#to_address').val(data['address']);
		  }
      </script> 

```

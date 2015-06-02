# 新建销售订单弹出组件 creatsellorder/creatorder

## 说明

  > 供全局调用 新建Avalon 弹出层 新建销售订单

## 使用方法

  > 引入 Avalon组件地址  creatsellorder/creatorder

   [在线预览案列](http://www.apps.com/index.php?app=Invoicimg&m=Sale&a=a) http://www.apps.com/index.php?app=Invoicimg&m=Sale&a=a

``` javascript
require(['avalon','creatsellorder/creatorder'],function(avalon,creatorder){
      avalon.define({
        $id:'creatorder',
        title:'创建订单',
        $opt:{

          callbackfun:function(a,b){
             avalon.log('a',a);
             avalon.log('b',b);
             
          }
        }
      });
      avalon.scan();
   })

```

## 配置参数说明


 max : 90000
        ,min : 1
        ,onInit : avalon.noop
        ,callbackfun:avalon.noop //回调函数Init

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
| max  | 否 |  默认销售产品的最大数量  |
|onInit()| 否| 应用初始化回调函数 |
|callbackfun(vmodel , data)|否| 提交成功订单后 回调函数 ，参数vmodel 返回组件视图模型。 data 为提交成功后 返回的数据 ，采购订单id |


## 回调函数说明

onInit()


callbackfun(a,b)


```` javascript

data: {orderid: 112, settstatu: 1}
orderid: 112
settstatu: 1
info: "订单提交成功"
statu: 1

````



## 返回说明

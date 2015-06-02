# 新建销售订单弹出组件 creatsellorder/creatorder

## 说明

  > 供全局调用 新建Avalon 弹出层 新建销售订单

## 使用方法

  > 引入 Avalon组件地址  creatsellorder/creatorder

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

## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
| p  | 否 |  分页不填安装默认数   |

## 返回说明

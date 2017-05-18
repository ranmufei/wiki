# 消息推送组件 socktMassage/push

## avalon 组件名称 socktMassage/push


## 组件说明

  > 该组件用于试试监听后台消息推送，传统获取消息的方式是 定时ajax 轮询 ，缺点是不够实时 并且浪费请求资源 ，时间就了对浏览器的内存资源也大大浪费。

  > 本消息组件是 基于 socket 连接的长连接 实时消息监听。 开发者只需要在组件的回调方法中 自行处置 有消息推送来的业务处理。 callbackfun:function(data){ } 详细请看后面的案例


## 组件配置参数说明

              title:'sockt111',              
              key:'Index',
              

## 基本属性配置

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|title|否| 定义抄送标题 有默认值 但建议填写 |
|key|否|  监听接收消息    Index:'默认主页接受'; 应用内部接收请填写 应用key |

##  接口方法

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|callbackfun(data)|是| 回调接口  参数为监听到的推送结果 ，开发者自行处理消息发送过来的数据 可以做相关业务开发  |



## 使用方法

  > 引入 Avalon组件地址 socktMassage/push

   [在线预览案列 发送 向用户uid =1 的首页发送测试](http://www.apps.com//index.php?app=Invoicimg&m=TestApi&a=testsentpush&uid=1&type=1&location=Index) http://www.apps.com//index.php?app=Invoicimg&m=TestApi&a=testsentpush&uid=1&type=1&location=Index

   [结果预览]（http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget）http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget#

``` javascript

/**
* test
* 
*/
require(['avalon','twitterCopy/twitterCopy','domReady!'],function(avalon){
   var cpmodel=null;
   var model=avalon.define({ 
        $id:'root',
         $copy:{
               onInit:function(cmodel){
                  console.log('oninit:',cmodel);
                  cpmodel=cmodel;
               },
               callbackfun:function(){
                  avalon.log('callbackfun 被调用');
               },
               width:'400px',
               height:'500px',
               title:'产品采购审批结果',
               content:'新产品打折季节洗碗大家炉里看实现去啊年的销售而',
               form:'InvoicimgProduct',
               msgtype:'2'
            },
              ,tijiao:function(){
               //提交抄送
               cpmodel.sendmsg();
            }
            
   })
   avalon.scan();


})

```
## HTML
```
<script src="/App/Invoicimg/AvalonAction/avalon_test.js"></script>


<h1>avalon  组件测试 demo </h1>
<div ms-controller="root">
 
<div ms-widget="twitterCopy,dasdasd,$copy"></div>
 <span ms-on-click=tijiao()> 测试发送</span>


</div>





```





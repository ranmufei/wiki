# 抄送消息到企业微圈 avalon组件 twitterCopy/twitterCopy

## 说明

  > 该组件提供接口 开发者可以吧 有需要分享到微圈的的信息 发布到微圈中去。

  > 应用场景例如： 各种需要发通知的信息都可以抄送 到微圈  ；
  
  > 该组件最大的特点 就是要指定消息的抄送范围



## 配置参数说明
               title:'产品采购审批结果',
               content:'新产品打折季节洗碗大家炉里看实现去啊年的销售而',
               form:'InvoicimgProduct',
               msgtype:'2'

## 基本属性配置

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|title|否| 定义抄送标题 有默认值 但建议填写 |
|content|是| 抄送内容 发送内容  |
|form|是| 来源 一般填写应用的 key  |
|msgtype|是|    0:'默认分享';1：'微圈动态'; 2 抄送消息 3 @我的 4 我@的 5 我回复的 6 回复我的 7 带我回执 |

##  接口方法

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|sendmsg()|是| 触发 发送消息 ；注意： `该接口会制动判断是否选择抄送范围 如果选择抄送范围 即可发送 如果未选择抄送范围 不会发送抄送`  |



## 使用方法

  > 引入 Avalon组件地址 twitterCopy/twitterCopy

   [在线预览案列](http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget) http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget

``` javascript

/**
* test
* 
*/
require(['avalon','creatclass/creatclass','unit/unit','warehouse/warehouse','createproduct/createproduct','format/format','domReady!'],function(avalon){
   var classmodel=null;
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





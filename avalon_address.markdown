# 选择发货地址组件 Prewidget/Prewidget

## 说明

  > 选择客户之后才能选择收货地址、若无客户地址可以新增客户地址




## 配置参数说明
           ,Prewidget:{
                        width:250,//自定义宽度  
			onInit:function(vm){//初始化
			    PrewidgetVM=vm;

			},
			callbackfun:function(data){
                               
			}//回调
		}

## 基本属性配置

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
| width  | 否 |  默认组件宽度  |

##  接口方法

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|callbackfun()|否| 点击确定按钮后  自动回调函数  |
|getSelected()|否| 获取选择的产品接口  |



## 案例html 


```

<div ms-controller="root">


     <div class="form-group ">
		<label for="inputPassword " class="col-xs-2 control-label ">选择发货地址：</label>
		   <div class="col-xs-10 " ms-widget="Prewidget"></div>
     </div>
</div>


```


## 使用方法

  > 引入 Avalon组件地址 Prewidget/Prewidget

   [在线预览案列](http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget) http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget

``` javascript

/**
* test
* 
*/
require(['avalon','Prewidget/Prewidget','domReady!'],function(avalon){
   var classmodel=null,choice=[];
   var model=avalon.define({ 
        $id:'root',
        $classopt:{
          onInit:function(cmodel){
            console.log('oninit:',cmodel);
            classmodel=cmodel;
          },
          callbackfun:function(){
            avalon.log('callbackfun 被调用');
          },
          width:'400px',
          height:'500px',
          title:'测试分类管理',
        },
            $warehouseopt:{
               width:'600px',
               height:'500px',
               title:'仓库',
               callbackfun:function(){
                  avalon.log('callbackfun 回调仓库');
               },
            },
            $unitopt:{
               width:'500px',
               height:'500px',
               title:'单位管理',
               callbackfun:function(){
                  avalon.log('callbackfun 回调单位');
               },
            },
            $createproductOpt:{
               width:'730px',
               height:'500px',
               title:'添加产品',
               callbackfun:function(){
                  avalon.log('回调了 添加产品');
               },
            },
            $formatopt:{
               width:'580px',
               height:'500px',
               title:'规格管理2',
               callbackfun:function(){
                  avalon.log('回调了 规格光临222');
               },
            },
            $choiceproductopt:{
               onInit:function(choicedata){
                  choice=choicedata;
               },
               title:'选择产品3',
               callbackfun:function(){
                   var xz= choice.getSelected();
                    avalon.log('选择的产品：',xz);
               },
            },
            choicecp:function(){

            }
   })
   avalon.scan();


})

```


## 选择批次 返回的数据结构说明



![111110](http://192.168.1.240/uploads/ranmufei/apps/38c6dc2974/111110.png)


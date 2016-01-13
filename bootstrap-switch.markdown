# Bootstrap 开关（switch）组件 bootstrap-switch/avalon.switch

## 说明
#### 1, 使用效果可以查看这里(http://www.bootcss.com/p/bootstrap-switch)

#### 2, 在html中引用
```html
<div  ms-widget="bootstrap-swtich,$,$bootstrapSwtich"> </div>
```


## 配置参数说明
       $bootstrapSwtich : {
              onSwitchChange : function(event,state){  //点击切换的回调函数，event是事件，state是返回的状态， true为开，false为关
                   avalon.log(state)   
               } ,
              onInit : function(){},   //初始化的操作
              state: true,     // 开始的状态, true 为开  ，  false为关
              size: null,       //默认为normal   , large大 ,small小 ， mini最小
              disabled: false,   //禁用 ,默认关
              readonly: false,  //  只读 ，默认关
              onColor: "primary",    //可选颜色风格primary,info,success,warning,danger
              offColor: "default",   //可选颜色风格primary,info,success,warning,danger
              onText: "ON",          // 开时选中的文字
              offText: "OFF",        // 关时选中的文字
              labelText: "&nbsp;",     //开与关之间的字

      } ,


##  接口方法

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|onInit()|否| 组件初始化  |
|onSwitchChange()|是| 点击后的回调，event是事件，state是返回的状态， true为开，false为关  |






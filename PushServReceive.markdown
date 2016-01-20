# PushServReceive（PUSH）组件 WebSocket/WebSocket

## 说明
#### 1, 使用前先咨询作者：BaoDongXing

#### 2, 在html中引用
```html
<div  ms-widget="WebSocket,$test,$testOpts"> </div>
```


## 配置参数说明
                    $testOpts: {
                        UserAuthorize:{
                            uid:1,
                            style:3,
                        },
                        resetWs:{
                            number:3,
                            time:3,
                        },
                        showLoading: function(){

                        },
                        hideLoading: function(){

                        },
                        wsOpen: function(evt){

                        },
                        wsClose: function(evt){

                        },
                        wsError: function(evt){

                        },
                        wsMessage: function(evt){

                        },
                    },


##  接口方法

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|onInit()|否| 组件初始化  |
|onSwitchChange()|是| 点击后的回调，event是事件，state是返回的状态， true为开，false为关  |
#### 通过 avalon.vmodels[id].setState(true) 可以改变为开的状态
#### 通过 avalon.vmodels[id].setState(true) 可以改变为关的状态



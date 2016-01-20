# PushServReceive（PUSH）组件 WebSocket/WebSocket

## 说明
#### 1, 使用前先咨询作者：BaoDongXing

#### 2, 在html中引用
```html
<div  ms-widget="WebSocket,$test,$testOpts"> </div>
```


## 配置参数说明
                    $testOpts: {
                        //注册PushServ的身份信息：uid:为自己的用户UID,
                        //style:为连接PushServ类型（2.为首页，3.为应用头部），值都必须为integer类型
                        UserAuthorize:{
                            uid:1,
                            style:3,
                        },
                        //重启PushServ连接，number:重启连接的最大次数，time:重启间隔时间单位为秒，值都必须为integer类型
                        resetWs:{
                            number:3,
                            time:3,
                        },
                        //准备开始连接 PushServ 的回调，可以加上动画（在wsOpen之前）
                        showLoading: function(){
                        },
                        //成功连接 或 连接失败 PushServ 的回调，可以加上动画（在wsClose同时）
                        hideLoading: function(){
                        },
                        //成功连接 PushServ 的回调
                        wsOpen: function(evt){
                        },
                        //关闭连接 PushServ 的回调
                        wsClose: function(evt){
                        },
                        //连接 PushServ 出错的回调（如果是服务器断掉连接，那么会先触发 wsError 后触发 wsClose）
                        wsError: function(evt){
                        },
                        //当 PushServ 服务器发送信息过来，触发的回调
                        wsMessage: function(evt){
                            console.log("回调的连接对象",evt.data)
                        },
                    },


##  接口方法

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|UserAuthorize|是| 当前组件的PushServ 注册信息  |
|resetWs|否| 组件重启配置，如不写，将用默认配置（number:5,time:3）  |
|showLoading()|否| 准备开始连接 PushServ 的回调  |
|hideLoading()|否| 成功连接 或 连接失败 PushServ 的回调  |
|wsOpen()|否| 成功连接 PushServ 的回调  |
|wsClose()|否| 关闭连接 PushServ 的回调  |
|wsError()|否| 连接 PushServ 出错的回调  |
|wsMessage()|是| 当 PushServ 服务器发送信息过来，触发的回调  |
#### 通过 avalon.vmodels[id].setState(true) 可以改变为开的状态
#### 通过 avalon.vmodels[id].setState(true) 可以改变为关的状态



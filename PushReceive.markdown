# PushReceive（WebSocket）组件 pushReceive/pushReceive

## 说明
#### 1. 使用前先咨询作者：BaoDongXing

#### 2. 在html中引用
```html
<div  ms-widget="WebSocket,$test,$testOpts"></div>
```


## 配置参数说明
                    $testOpts: {
                        //注册PushServ的身份信息：uid:为自己的用户UID,
                        //style:为连接PushServ类型（2.为首页，3.为应用头部），值都必须为integer类型
                        //app:为当前应用的名称如 URL ~index.php?App=Home~~ 取App的值为应用名称
                        UserAuthorize:{
                            uid:1,
                            style:3,
                            app:"Home",
                        },
                        //重启PushServ连接，number:重启连接的最大次数，time:重启间隔时间单位为秒，值都必须为integer类型
                        resetWs:{
                            number:13,
                            time:2,
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
|UserAuthorize|是是| 当前组件的PushServ 注册信息  |
|resetWs|否| 组件重启配置，如不写，将用默认配置（number:13,time:2）  |
|showLoading()|否| 准备开始连接 PushServ 的回调  |
|hideLoading()|否| 成功连接 或 连接失败 PushServ 的回调  |
|wsOpen()|否| 成功连接 PushServ 的回调  |
|wsClose()|否| 关闭连接 PushServ 的回调  |
|wsError()|否| 连接 PushServ 出错的回调  |
|wsMessage()|是是| 当 PushServ 服务器发送信息过来，触发的回调  |

## PHP端 Send Method:详细请见公共模型里的（PushServModel.class.php）

* [PushMessage 普通消息Push服务类型为 (1)]
* @param [int   ] $Suid    [发送消息者UID]
* @param [array ] $Rlimits [消息发送的类型：1.应用主页连接，2.应用里的头部连接]
* @param [array ] $AppNames[指定要发送的应用名称 "URL里的 index.php?App=Home 这个Home就是主页的应用名称"]
* @param [array ] $Ruids   [消息的接收者UID；注意：必须索引数组]
* @param [string] $SData   [消息的具体内容]
* @param [string] $NData   [只用于通知提醒显示，没有业务数据结构，一般用于 手机提醒]

* @demo  {$obj->PushMessage( 100, array(2,3,4), array('Home','Lore'), array(12,13,5,2,1), '消息的具体内容', '通知提醒' )}


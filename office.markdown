# onlyoffice（在线office）组件 onlyoffice/onlyoffice

## 说明
#### 1. 使用前先咨询作者：BaoDongXing

#### 2. 在html中引用
```html
<div  ms-widget="office,$,$officeOpt"></div>
```


## 配置参数说明
    $officeOpt: {
        // 指定文档路径是否是完整路径，就否带有域名路径（默认）
        isDocUrlFull: true,
        // 指定要操作的文件输出模式，如：stream:就是流方式输出的。 path: 就是文档的绝对路径输出的（默认）
        docUrlType: "path",
        // onlyoffice服务的连接地址，用来拼接API.js请求地址（默认）
        onlyofficeAddr: window.location.protocol + "//" + window.location.hostname + ":8282",
        // 存放要打开的文档绝对地址，的属性名（默认，但要跟据你的路径元素来修改）
        setAttribute: "office-src",
        // 打开office窗口的默认大小（默认，可修改它打开的默认窗口大小）
        viewInitHD: ['1000px', '800px'],
        // 是否截取当前元素的click事件，用自带click触发openOffice()在线操作事件（默认）
        bindClickStatu: false,

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
* @param [array ] $Rlimits [消息发送的类型[看 self::$PushConnType ]：[2].应用主页连接，[3].应用里的头部连接，[4].为手机端通知连接]
* @param [array ] $AppNames[指定要发送的应用名称 "URL里的 index.php?App=Home 这个Home就是主页的应用名称"]
* @param [array ] $Ruids   [消息的接收者UID；注意：必须索引数组]
* @param [string] $SData   [消息的具体内容]
* @param [string] $NData   [只用于通知提醒显示，没有业务数据结构，一般用于 手机提醒]

* @demo  {$obj->PushMessage( 100, array(2,3,4), array('Home','Lore'), array(12,13,5,2,1), '消息的具体内容', '通知提醒' )}


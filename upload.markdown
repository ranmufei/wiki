实现上传附件的统一调用接口,虽然使用avalon组件模式，但不涉及扫描。(目前仅实现上传的简单功能)  
### 调用方式  
调用组件的元素目前只是起一个触发调出上传组件域的功能，所以开发者可以自由设计。  
HTML中：`<a href="#" ms-widget="upload">上传文件</a>` ,define依赖define(['upload/upload'])  

| 配制参数 |  类型| 默认值 |  描述  |
| :-- | :-- | ----:| :--: |
|num|int|50|一次上传文件数量|
|allow|string| 云盘后台设置 |允许的文件类型 如'jpg,jpeg,png'|
|filesize|int| 云盘后台设置 |允许的单文件最大值 目前只支持bit单位即如果限定1M应是1*1024*1024|
|onInit|function| 空函数 |组件初始化回调|
|width|int|670|弹出框宽度|
|height|int|410|弹出框高度|
|completeMethod|function|  |用户点击完成上传的回调。|

实现上传附件的统一调用接口,虽然使用avalon组件模式，但不涉及扫描。(目前仅实现上传的简单功能)  
### 调用方式  
调用组件的元素目前只是起一个触发调出上传组件域的功能，所以开发者可以自由设计。  
HTML中：`<a href="#" ms-widget="upload">上传文件</a>` ,define依赖define(['upload/upload'])  

| 配制参数 |  类型| 默认值 |  描述  |
| :-- | :-- | ----:| :--: |
|`mode`|string|'simple'|上传UI主题,目前默认'simple'及'image'|
|`completeMethod`|function|  |用户点击完成上传的回调。|
|`num`|int|50|一次上传文件数量|
|`allow`|string| 云盘后台设置 |允许的文件类型 如'jpg,jpeg,png'|
|filesize|int| 云盘后台设置 |允许的单文件最大值 目前只支持bit单位即如果限定1M应是1*1024*1024|
|formdata|object||要上传到后台的参数，配套serverurl参数使用，否则不意义|
|serverurl|string|''|上传提交地址(一般网盘可能会用到)|
|responseMethod|function|null|配合serverurl接口使用,上专成功的回调函数, 参数为response（返回值），false上传失败 否则程序员要返回上传成功后自己要用的数据 |
|trigger|boolean|true|点击组件element是否弹出上传组件|
|onInit|function|  |组件初始化回调，参数为vmodel,vmodel有几个有用的属性:uploader上传实例（可用于动态为formdata赋值，详细请看webuploader文档） open()打开上传组件框|
|width|int|670|弹出框宽度|
|height|int|410|弹出框高度|
|getTemplate|function| |模板修改回调函数,目前不可用|
|globalMethods|function||开发者自定义上传UI的回调,估计现在不会用的，组件已经通过该回调函数定制了两套Ui，‘simple’及‘image'|
||||

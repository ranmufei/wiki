实现上传附件的统一调用接口,虽然使用avalon组件模式，但不涉及扫描。(目前仅实现上传的简单功能)  
### 调用方式  
调用组件的元素目前只是起一个触发调出上传组件域的功能，所以开发者可以自由设计。  
HTML中：<a href="#" ms-widget="upload">上传文件</a> ,define依赖define(['upload/upload'])

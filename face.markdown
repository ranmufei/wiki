`<div ms-widget="face"  ></div>`   
 require(["face/avalon.face"], function() {});

| 参数名称  |     类型|  默认值  |说明     |
| :--------  |  ------- | ------| -------- |
|textareaid| string| 'msg' | 表情插入的文本域 ID|
|top| number| 25| 表情弹出层 与 出发表情的按钮的top距离|
|left| number|-5| 表情弹出层 与 出发表情的按钮的left距离|
|motionsToHtml| function|| 表情过滤函数，就是将 对应的表情标识转变成 对应的图片地址 使用方法：{{"需要转换的文   本"|motionsToHtml|html}}|

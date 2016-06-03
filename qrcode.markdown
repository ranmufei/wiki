`<div ms-widget="qrcode"  ></div>`   
widget 中间的id不要给'$id'，直接给id或者'$'

 require(['qrcode/qrcode'], function() {});

| 参数名称  |     类型|  默认值  |说明     |
| :--------  |  ------- | ------| -------- |
|width| int| 100 | 二维码图形宽度 |
|height| int| 100 |  二维码图形宽度 |
|render| string|'canvas' |默认为canvas渲染，可选table渲染 如果需要下载请选canvas渲染 |
|str| str|'www.linksame.com' |默认编码的内容 |
|showDownload| boole|true | 是否显示下载按钮 true为显示，false为不显示|
|change| function(value){}| | 二维码进行重新编码渲染|
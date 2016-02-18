# 关于开发中用到下载功能的说明

    > 在我们的客户端界面中经常用到文件下载 数据导出等需求，客户端的下载与在开发的浏览器中有所不同 请注意看下面说明


## - 注意点1

  // 弃用 ：：- 下载必须 用 a 链接 加 属性 “target='_blank'”属性   (不需要加_blank  )

```` html
   <a href="" >

````

## - 注意点2（默认已封装 不需要开发中做操作）

   > - 要监听文件是否下载完成 调用回调函数 downloadsuccess(arg) 该函数会被自动执行调用，前提是要在第一屏幕

```` html
@param arg  下载文件路径
function downloadsuccess(arg){ 
    alert(arg);
    console.log(arg);
} 

```` 
# onlyoffice（在线office）组件 onlyoffice/onlyoffice

## 说明
#### 1. 使用前先咨询作者：BaoDongXing

#### 2. 在html中最简单的引用但还不能正常使用
```html
<a ms-widget="office,$,$officeOpt"></a>
```

### 3. docUrlType配置为"path"的时候，简单例子（里面最重要的是属性"office-statu"的值为“view OR edit”用来判断这个文档是否只是查看或可以修改文档权限）
```html
<a office-statu="view" ms-href="./uploads/20160809/这是一个测试文档.doc" ms-widget="office,$,$officeOpt">这是一个测试文档A.doc</a>
```

### 4. 如果其它使用需求，可跟我讨论 0.0

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




## 制作`发行版本` 注意事项
- 清空项目项目附件
 -  根目录`Uploads`文件下附件,avatar[头像]、datums[资料]、qrcode[二维码]文件件不要删除
- 清除缓存文件（`Cache`下所有文件）
- 初始化文件(`baseset_data.php`)中 `版本信息`部分的更新
- 项目设置
 - `debug`要关闭
 - 客户端`右键`屏蔽
- 加密`Addons`及`App`文件夹下文件 (其中 `应用/Common/common.php`、`应用/Conf/config.php` `不可加密`)
- 哪些应用是要单独做升级处理,不能使用到发行版的
- `授权地址` 及 `升级包下载地址`是否已改成网络的
- `mobile 端`测试账号清除 Home/Lib/Action/MobileauthAction.class.php 

## 制作`升级包` 注意事项
- 有些文件不可直接覆盖（ThinkPHP/appconfig.php/ExternalApp.php）
- 对Addons及App文件夹的加密(其中 `应用/Common/common.php`、`应用/Conf/config.php` `不可加密`)
- 升级包中`可执行文件`是否需要进行一些`缓存更新`操作
- 哪些应用是要单独做升级处理,不能使用系统升级的
- 如果是配制文件 ,`授权地址` 及 `升级包下载地址`是否已改成网络的
- 版信息的更正(`upgrade/config.php`)
- 是直接压缩`utf-8这个文件夹`成`zip`格式,压缩文件名称是否正确(`patch_上次日期_本次升级日期.zip`)
- 类似字段还有`ttf`、`.svg`、`eot`、`woff`等格式 用工作搜索时别忘记设置
- `mobile 端`测试账号清除 Home/Lib/Action/MobileauthAction.class.php 
- `数据表升级检测,是否导入了测试数据,自增是否从1开始`



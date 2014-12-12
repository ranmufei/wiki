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

## 制作`升级包` 注意事项
- 有些文件不可直接覆盖（ThinkPHP/appconfig.php/ExternalApp.php）
- 对Addons及App文件夹的加密(其中 `应用/Common/common.php`、`应用/Conf/config.php` `不可加密`)
- 升级包中`可执行文件`是否需要进行一些`缓存更新`操作
- 哪些应用是要单独做升级处理,不能使用系统升级的




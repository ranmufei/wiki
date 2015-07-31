# 实现定时任务步骤：

### TP实现定时任务的原理是 每当有人访问控制器时，会触发App_start执行我们设置好的php代码，如数据库的备份、缓存的清除、数据的更新等等，并且可以设置更新时间间隔。

` 必要条件：
- TP的核心文件引入CronRunBehavior.php ，文件夹位置如下图一

- 在应用的conf文件下，引入tags.php 和 crons.php 2个配置文件

 ```` php
//tags.php文件
<?php
return array(
'app_begin' => array('CronRun'),
);

````


```` php
//crons.php文件
// myplan文件的地址在 应用下Lib/Cron/myplan.php
// 这里是一天间隔执行myplan.php中的代码
<?php
return array(
    'cron_1' => array('myplan', 24*60*60),
 );

````
--  myplan.php中就可以写你的业务需求了

![图一](http://192.168.1.240/uploads/ranmufei/apps/a80e72906c/lename_2.png)
![图二](http://192.168.1.240/uploads/ranmufei/apps/c12176ce52/lename_3.png)

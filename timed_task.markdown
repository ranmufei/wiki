# 实现定时任务步骤：

#### TP实现定时任务的原理是 每当有人访问控制器时，会触发app_begin执行我们设置好的php代码，如数据库的备份、缓存的清除、数据的更新等等，并且可以设置更新时间间隔。


##  必要条件：
#### TP的核心文件引入CronRunBehavior.php ，文件夹位置如下图一

#### 在应用的conf文件下，引入tags.php 和 crons.php 2个配置文件，文件夹位置如下图二

### tags.php文件
 ```` php
//tags.php文件
// 任何情况出发本应用时，会执行CronRunBehavior.php ，进而执行crons.php
<?php
return array(
'app_begin' => array('CronRun'),
);
````

### crons.php文件
````php
//crons.php文件
// myplan文件的地址在 应用下Lib/Cron/myplan.php
// runtime目录下会产生~crons.php缓存文件
// 这里是一天间隔执行myplan.php中的代码
// 有多个任务，可以接着写数组
<?php
return array(
    'cron_1' => array('myplan', 24*60*60),
 );
````
###  在myplan.php中就可以写你的业务需求了，这其实是事件不能称为计划任务，但能达到我们的定时任务的目的

![图一](http://192.168.1.240/uploads/ranmufei/apps/a80e72906c/lename_2.png)
![图二](http://192.168.1.240/uploads/ranmufei/apps/c12176ce52/lename_3.png)

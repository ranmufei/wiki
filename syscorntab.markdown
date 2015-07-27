# 系统定时任务

`禁止执行wdcp上面的 更新计划任务 否则会删除我配置的定时任务 切忌！！！！`


``` bash
20 17 * * * /www/wdlinux/wdphp/bin/php /www/wdlinux/wdcp/task/wdcp_mysql_backup.php
20 18 * * * /www/wdlinux/wdphp/bin/php /www/wdlinux/wdcp/task/wdcp_task.php 10
01 13 * * * /www/web/default/nodeim/shellbeifenMysql.sh
*/5 * * * * /www/web/default/nodeim/testNetStatu.sh
*/5 * * * * curl localhost/system/dns/dnns.php?ac=ToDNS
10 * * * * ntpdate us.pool.ntp.org

```


# 系统启动加载 /etc/rc.d/rc.local

``` bash
#!/bin/sh
#
# This script will be executed *after* all the other init scripts.
# You can put your own initialization stuff in here if you don't
# want to do the full Sys V style init stuff.

touch /var/lock/subsys/local

#=========================================
export PATH=$PATH:/usr/local/bin
forever start /www/web/default/nodeim/run.js

/usr/bin/dnspodsh.sh user pass & >/dev/null  #账号密码
#/www/web/default/nodeim/dnspodsh.sh xxx 000 & >/dev/null   #账号密码注释掉了
/www/web/default/nodeim/getIp.sh
ntpdate us.pool.ntp.org

```
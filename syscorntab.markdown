# 系统定时任务

``` bash
20 17 * * * /www/wdlinux/wdphp/bin/php /www/wdlinux/wdcp/task/wdcp_mysql_backup.php
20 18 * * * /www/wdlinux/wdphp/bin/php /www/wdlinux/wdcp/task/wdcp_task.php 10
01 13 * * * /www/web/default/nodeim/shellbeifenMysql.sh
05 *  * * * /www/web/default/nodeim/testNetStatu.sh
05 *  * * * curl localhost/system/dns/dnns.php?ac=ToDNS


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

/usr/bin/dnspodsh.sh 909954500@qq.com 1984lf9g25g & >/dev/null
#/www/web/default/nodeim/dnspodsh.sh 909954500@qq.com 1984lf9g25g & >/dev/null
/www/web/default/nodeim/getIp.sh


```
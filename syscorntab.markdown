# 系统定时任务

``` bash
20 17 * * * /www/wdlinux/wdphp/bin/php /www/wdlinux/wdcp/task/wdcp_mysql_backup.php
20 18 * * * /www/wdlinux/wdphp/bin/php /www/wdlinux/wdcp/task/wdcp_task.php 10
01 13 * * * /www/web/default/nodeim/shellbeifenMysql.sh
05 *  * * * /www/web/default/nodeim/testNetStatu.sh
05 *  * * * curl localhost/system/dns/dnns.php?ac=ToDNS


```
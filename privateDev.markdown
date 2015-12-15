# 私有盘系统开发 版本说明

## dnspod授权方式更新

 > dnspod域名检查 修改  为token 验证，原理：dnspod后台生成 授权 token ; pcd 程序 dnspod 登录调用 这个token,这个token放在远程的 www.linksame.com/token.txt 下， 以后只需要维护好这个文件的token即可。

## vision6.4 

系统初始化程序刷机到 6.0.9 版本 7-25

## vision6.2 



-  给 ngix添加端口监听 8082 .有了该功能以后不需要做路由器映射了 只需要设置 dmz 主机即可。   **用处很大的更新**



/www/wdlinux/nginx/conf/vhost/00000.default.conf

``` bash
     server {
        listen       8082;
        listen       80;
        server_name  localhost;
        root /www/web/default;
        index index.php index.html index.htm;


        location ~ \.php$ {
		proxy_pass http://127.0.0.1:88;
		include naproxy.conf;
        }
        location ~ .*\.(gif|jpg|jpeg|png|bmp|swf)$ {
                expires      30d;
        }

        location ~ .*\.(js|css)?$ {
                expires      12h;
        }
    }  

```

## vision6.1  系统新增加功能 

- 新增加dns 动态域名 检测程序 php 版本  /路径  localhost/system/dns/dnns.php?ac=ToDNS

- 增加系统定时更新dns 动态ip curl localhost/system/dns/dnns.php?ac=ToDNS

- 增加功能 自动更新网络时间 （开机自动同步网络时间/ 定时每小时更新一次）

- 增加功能 恢复出厂设置 /system//?App&m=Index&a=allreset 

## vision6.0

- dnspod 改回 /usr/bin/dnspodsh.sh 启动


## vision4.0

- nodeim 移动到网站目录下

- /etc/rc.local  修改 启动系统初始化 getIp.sh   dnspodsh.sh 文件位置路径到网站目录的nodeim下


## vision3.3

- 增加对当前系统空间的合理利用，1T，2T的硬盘空间挂载到 根目录

- 增加disk.sh 实现自动挂载新硬盘空间到 目录/backup 文件夹下

- 修正优化 备份机制，备份数据库 和 附件目录 到网站目录的 backup下，实现自动判断是否有备份硬盘 并备份到硬盘的挂载目录；数据库文件保存十天以内的，附件保存两天以内的


## vision3.2

- 新增加定时备份功能,备份数据库 和 程序附件目录 到网站的backup目录  `shellbeifenMysql.sh`

- 优化开机自动获取IP 网关 等功能【实现可兼容大多数普通路由器，注意 自动获取网关还待进一步优化 实现任意网关 目前可以实现获取网关的前三段+1】 

- 新增定时任务 检查网络连接功能 `testNetStatu.sh`

## vision2.1 

- 开机自动获取网关 配置环境

# 系统模型图
 

![QQ图片20141223172808](http://192.168.1.240/uploads/ranmufei/apps/250a6e5295/QQ%E5%9B%BE%E7%89%8720141223172808.png)

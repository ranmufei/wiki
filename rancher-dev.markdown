# rancher 开发相关说明

##  基础容器

|名称| 接口 | 说明 |
|:--:|:--|:--|
|base 重启 | model("RancherRan")->base_restart()| base容器重启 |
|ngxlua 重启 | model("RancherRan")->ngx_restart()| ngxlua容器重启 |


## 容器升级说明

> 容器升级 我们用shell  来实现  ，用php 来触发

- 规定 shell 脚本的的位置为  /system/sh/rancher/ 目录下

- php 函数  exec("/bin/sh xxxx") 来调用

- 可以写模型 或者 控制器 来供升级调用

> 需要注意 由于是在容器中运行 故 开头 用 bin/sh 切记； exec("/bin/sh")  ，shell 文件头也要用 #!/bin/sh来声明

```

#参考案例

	function run_shell_file(){
          exec('/bin/sh /app/web/system/sh/rancher/crontab_upgrade.sh');
    }



```



> shell 文件参考案例 

>> 升级容器

```
#!/bin/sh
curl -u "CA536FF6119B49B21403:z5KLJ5RVH9gqzL5rrZw45G5LdKP9r5GeFpNAV6ZT" \
-X POST \
-H 'Accept: application/json' \
-H 'Content-Type: application/json' \
-d '{"inServiceStrategy":{"batchSize":1, "intervalMillis":2000, "launchConfig":{"capAdd":[], "capDrop":[], "count":null, "cpuSet":null, "cpuShares":null, "dataVolumes":["/home:/home", "/etc/httpd/conf/httpd.conf:/home/www/maindata/system/httpd.conf", "/etc/httpd/conf/httpd.conf:/home/www/maindata/system/httpd2.conf"], "dataVolumesFrom":[], "description":null, "devices":[], "dns":[], "dnsSearch":[], "domainName":null, "hostname":null, "imageUuid":"docker:hub.03in.com:5002/ranmufei/crontab:v2.0.7", "kind":"container", "labels":{}, "logConfig":{"config":{}, "driver":""}, "memory":null, "memoryMb":null, "memorySwap":null, "networkMode":"managed", "pidMode":null, "ports":[], "privileged":false, "publishAllPorts":false, "readOnly":false, "requestedIpAddress":null, "startOnCreate":true, "stdinOpen":true, "tty":true, "user":null, "userdata":null, "version":"df318165-cc57-489b-b136-e9d94f8927fa", "volumeDriver":null, "workingDir":null, "dataVolumesFromLaunchConfigs":[], "networkLaunchConfig":null, "vcpu":1}, "previousSecondaryLaunchConfigs":[], "secondaryLaunchConfigs":[], "startFirst":false}, "toServiceStrategy":null}' \
'http://172.17.0.1:8080/v1/projects/1a5/services/1s43/?action=upgrade'

```
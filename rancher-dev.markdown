# rancher 开发相关说明

##  基础容器

|名称| 接口 | 说明 |
|:--:|:--|:--|
|base 重启 | model("RancherRan")->base_restart()| base容器重启 |
|base 重启 | model("RancherRan")->ngx_restart()| ngxlua容器重启 |
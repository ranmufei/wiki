# 选择写同人的权限判断
## 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=check_mangerwork

>  method : get

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=check_mangerwork
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|id| 是| 当前操作的工作id  |
|workerid| 是|选择协同的工作id （以','形式分割）  |


## 返回结果

|info|array | array | 返回数据 数组|
|----|----|----|-----|
|statu|0/1 |int|返回状态 1：成功，0：失败|
|info|返回成功失败提示|string|返回提示|



# 选择审核人的权限判断
## 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=check_mangerid

>  method : get

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=check_mangerid
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|id| 是| 当前操作的工作id  |
|userid| 是|选择审核人的id  |


## 返回结果

|info|array | array | 返回数据 数组|
|----|----|----|-----|
|statu|0/1 |int|返回状态 1：成功，0：失败|
|info|返回成功失败提示|string|返回提示|

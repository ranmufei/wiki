# 测试发送消息接口

> www.apps.com/index.php?app=Im&m=Im&a=testapi&s_uid=1232&type=3  

> s_uid  收消息人的 uid   ;;    type  消息类型   0：全平台 1：pc  2 移动  3 Im

> apps 上开发 iphone 收消息  oa_member_mobile_push  用户的type 手机类型 1 为IPHONE 0 位安卓； uid为一 默认为冉幕飞的IPhone 手机

# （1）消息推送 ＰＨＰ开发 模型

## model("Im")->push($s_uid,$massage,$type,$localtion)

## 说明

  > 
  > 


##  参数说明

| 参数名称  type    |    必填 | 说明  |
| :-------- | --------:| :--: |
|$s_uid   int|是| 收消息人的uid  |
|$massage   array|是| 发送的消息  可以是一个数组结构（`注意：请和移动开发者讨论好格式`）  |
|$type   int|否|  消息推送平台 0：全平台 1：pc  2 移动； 默认为1 电脑端 |
|$location string| no | 消息推送位置 Index 首页 ； 应用key 表示应用内置页面 ：针对PC 端选择 |


## 案例

```` php

    $massage['title']='title helloworld'.time();
    $massage['contant']='你好这是内容'.time();
    $massage['description']='你好这是内容'.time();
    $massage['info']='dis'.time();
    $type=I("type");// 0：全平台 1：pc  2 移动 3 IM
    $result=  model("Im")->push($s_uid,$massage,$type);

````


# （2）移动端登录成功后回调 注册手机型号 以及（token）到系统

### API    del_notice

### HTTP URL   /index.php?app=Im&m=User&a=mobileInfo

### 携带参数
| 参数名称  type    |    必填 | 说明  |
| :-------- | --------:| :--: |
|access_token       string|是| 手机端登录授权token  |
|token              string|是| 手机端token 专指IPhone 官方分配的手机唯一token(安卓端不需要)  |
|type                int|是|  1：IPhone  0：安卓  |

# （3）移动端收到消息后回调 标记本消息已收取

### API    del_notice

### HTTP URL   /index.php?app=Im&m=User&a=del_notice

### 携带参数
| 参数名称  type    |    必填 | 说明  |
| :-------- | --------:| :--: |
|access_token       string|是| 手机端登录授权token  |
|id              int|是| 收取消息的json 字符串中 id  |


### curl  请求案例 

> http://www.apps.com/index.php?app=Im&m=User&a=del_notice&access_token=2c3b84599fcee0081496d827912c4a&id=94


### 参考消息收取数据结构

```
{
    "user": "173",
    "msg": {
        "title": "title helloworld1494321375",
        "contant": "你好这是内容1494321375",
        "description": "你好这是内容1494321375",
        "info": "dis1494321375"
    },
    "myuid": "1",
    "pushtype": "2",
    "id": 94
}

```



# （1）消息推送 ＰＨＰ开发 模型

## model("Im")->push($s_uid,$massage,$type)

## 说明

  > 
  > 


##  参数说明

| 参数名称  type    |    必填 | 说明  |
| :-------- | --------:| :--: |
|$s_uid   int|是| 收消息人的uid  |
|$massage   array|是| 发送的消息  可以是一个数组结构（`注意：请和移动开发者讨论好格式`）  |
|$type   int|否|  消息推送平台 0：全平台 1：pc  2 移动； 默认为1 电脑端 |



# （2）移动端登录成功后回调 注册手机型号 （token）到系统

## API   

## HTTP URL   /index.php?app=Im&m=User&a=mobileInfo

## 携带参数
| 参数名称  type    |    必填 | 说明  |
| :-------- | --------:| :--: |
|access_token       string|是| 手机端登录授权token  |
|token              string|是| 手机端token 专指IPhone 官方分配的手机唯一token(安卓端不需要)  |
|type                int|是|  1：IPhone  0：安卓  |




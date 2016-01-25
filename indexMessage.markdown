# 首页消息接口说明

### php后台添加消息接口调用方式：
```` php
 // $data为添加的数据数组
    $result = model('Notify')->add_notify($data); 
/** 返回格式如下
$result['status'] = 1 ; 
$result['info'] = "Success" ; 
*/ 
````


### data的格式如下 ， 请选择对应的类型
1. 提交只查看的消息（无任何操作）
```` php
        $data['title'] = $arr['title'];  
        $data['content'] = $arr['content'];
        $data['link'] = $arr['link'];
        $data['type'] = $arr['type']; 
````
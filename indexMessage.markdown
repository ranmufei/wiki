# 首页消息接口说明

- **手机端接口说明**
   手机端对应的接口需要把原来的pc端的接口复制一份，在对应的控制器名称后面加上Mobile(即把原来的控制器A，名称改为AMobile)


## 一. php后台添加消息接口调用方式：
```` php
/**
* @param $data为添加的数据数组
* @return 返回格式如下
* $result['status'] = 1 ; 
* $result['info'] = "Success" ; 
*/ 

    $result = model('Notify')->add_notify($data);
 
````


## 二. data的格式如下 ， 请选择对应的类型

###  1.提交只查看的消息（无任何操作）

```` php
/** 
* 提交的$data 格式  
*/
        $data['title'] = $arr['title'];       // 标题说明 
        $data['content'] = $arr['content'];  // 大概内容描述
        $data['from'] = ""   ,   //应用的key值 ，注意拆分的应用必填，一定要填写拆分后的应用的key ，非拆分的应用可自动获取key  20160221新增
        $data['link'] = $arr['link'];       //查看详情跳转地址
        $data['receive'] = $arr['receive'];       //接受者uid
        $data['menu_id'] = 0 ;  // menu.html中左侧菜单对应的id ;
        $data['type'] = 1;     //类型必须为1

        $data['con_id'] = 数据id ;  //数据ID，用于后续数据分析用 ， 2016-01-31新加
        // 获取审核详情地址，具体说明见下面五
        $data['detail_url'] = $arr['detail_url'];   

```` 

###  2.有操作的消息（协同 $type=4）

```` php
/** 
* 提交的$data 格式  
*/
        // 必填
        $data['title'] = $arr['title'];       // 标题说明
        $data['content'] = $arr['content'];  // 大概内容描述
        $data['from'] = ""   ,   //应用的key值 ，注意拆分的应用必填，一定要填写拆分后的应用的key ，非拆分的应用可自动获取key  20160221新增
        $data['link'] = $arr['link'];       //查看详情跳转地址
        $data['type'] = 4 ; 
        $data['check_url'] = $arr['check_url'] ;    // 点击确定的php处理地址
        $data['is_reject'] = 0 ;   //没有取消 
        $data['receive'] = $arr['receive'];       //接受者uid
        $data['menu_id'] = 0 ;  // menu.html中左侧菜单对应的id ;
        $data['con_id'] = 数据id ;  //数据ID，用于驳回同意操作时的识别 ， 2016-01-31新加
       
       // 获取历史记录地址， 格式index.php?app=Kaoqin&m=Index&test ，地址返回json格式  , 注意不用在后面带id参数
        $data['check_history_url'] = $arr['check_history_url'] ;

       // 获取审核详情地址，具体说明见下面五
        $data['detail_url'] = $arr['detail_url'];   

       // 选填	
        $data['check_name'] = $arr['check_name'] ;   //审核的按钮的名称，默认：审核
```` 

###  3.有操作的消息（业务审批($type = 2)/办公审批($type = 3) ）

```` php
/** 
* 提交的$data 格式  
*/
        // 必填
        $data['title'] = $arr['title'];       // 标题说明
        $data['content'] = $arr['content'];  // 大概内容描述
        $data['from'] = ""   ,   //应用的key值 ，注意拆分的应用必填，一定要填写拆分后的应用的key ，非拆分的应用可自动获取key  20160221新增
        $data['link'] = $arr['link'];       //查看详情跳转地址
        $data['receive'] = $arr['receive'];       //接受者uid
        $data['type'] = 2或者3 ;  //业务审批($type = 2) ; 办公审批($type = 3) 
        $data['check_url'] = $arr['check_url'] ;  //点击审核操作php处理地址
        $data['reject_url'] = $arr['reject_url'] ;   //点击驳回操作php处理地址
        $data['next_check_url'] = $arr['next_check_url'] ;   //点击提交下一个人审核的php处理地址

        $data['con_id'] = 数据id ;  //数据ID，用于驳回同意操作时的识别 ， 2016-01-31新加

        $data['menu_id'] = 0 ;  // menu.html中左侧菜单对应的id ;

        // 获取历史记录地址， 格式index.php?app=Kaoqin&m=Index&test ，地址返回json格式   , 注意不用在后面带id参数
        $data['check_history_url'] = $arr['check_history_url'] ;	
        
        // 获取审核详情地址，具体说明见下面五
        $data['detail_url'] = $arr['detail_url'];   


        // 选填
        $data['is_reject'] = $arr['is_reject'] ;   //是否有驳回按钮 ，默认1：有   ，0：无
        $data['is_next_check'] = $arr['is_next_check'] ;   //是否有提交下一步审核的按钮， 默认1：有   ，0：无
        $data['check_name'] = $arr['check_name'] ;   //审核的按钮的名称，默认：审核
        $data['reject_name'] = $arr['reject_name'] ;   //审核的按钮的名称，默认：驳回
        $data['next_check_name'] = $arr['next_check_name'] ;   //审核的按钮的名称，默认：提交下一步审核	
        
        	
````

## 三. 审核和驳回php处理后返回的格式(包含提交下一步审核后再次点击审核的操作)： 

```` php
/** 点击审核/不通过按钮   首页给应用的参数通过post方式
* @return 传输格式
*  status  状态  1同意  0驳回  2提交给下一个人
*  reply_text   审批意见
*  next_uid  下一个人的 next_uid  ， 没有默认为0
*/ 
post url : index.php?app=Kaoqin&m=Index&a=ce
post data : {id=数据的ID&reply_text=我同意了&next_uid=6}


    
````

```` php
/** 审核成功
* @return 返回格式
* 
*/ 

 $result['status'] = 1 ; 
 $result['info'] = "Success" ;  //可以填您处理程序的结果的文字，会在首页显示 
 $result['mystatus'] = 0或1、2        // 0没有审核   1审核同意 2 审核没同意  ,用于判断应用里面审核了，首页再次操作审核
    
````

```` php
/** 驳回
* @return 返回格式
*/ 

 $result['status'] = 0 ; 
 $result['info'] = "Error" ;  //可以填您处理程序的结果的文字，会在首页显示 
$result['mystatus'] = 0或1、2        // 0没有审核   1审核同意 2 审核没同意  ,用于判断应用里面审核了，首页再次操作审核
    
````


## 四. 历史记录的地址返回的数据格式： 


- 方式 : post
- post data : {id: 当前消息的内容con_id  , notify_id : 当前消息的id }

```` php
/** 
* @return 返回格式
* $result['data']     返回的数据 格式为数组
* $result['status']   返回状态 1正常  0没有或者失败
* $result['info']   返回状态的文字说明
*/ 

 $result['data'][0]['grade_uid'] =  0 ;   //审核人的uid 
 $result['data'][0]['grade_name'] =  "" ;   //审核人的名字
 $result['data'][0]['inserttime'] = "2015-12-19 12:00:00" ;  //处理时间  ，用友好时间处理过的 
 $result['data'][0]['status'] = 0或者1 、2;  //1 已审核 0待处理   2驳回
 $result['data'][0]['reply_text'] = "处理意见";  //填写处理意见
 $result['data'][0]['apply_uid'] = 0;  //上一个发起人的uid ，最近的是谁提交的
 $result['data'][0]['apply_name'] = "";  //上一个发起人的名字 
 $result['data'][0]['img'] = "";  //上一个发起人的头像
    
$mystatus = 0或1、2        // 0没有审核   1审核同意 2 审核没同意  ,用于判断显示按钮

//注意：工作流协同额外加了1个字段is_last，与data平级
$is_last = 0或1   //0没有最终审核    1已结最终审核了 ,用于判断关掉审核输入框

````

##  五. 审核详情说明： 
   审核详情的url打开是个完整的页面，可供首页调用，url里面的参数决定详情的不同
#### 方式 : post
   post data : {id: 当前消息的内容con_id  , notify_id : 当前消息的id }
#### 返回:
- data 详细的数据 
- status  状态  0失败  1成功
- mystatus    0或1、2        // 0没有审核   1审核同意 2 审核没同意
- audit_status  当前审核的状态，如 “报销中，待审核，已通过，已驳回，待确认，带归还 ， 已作废 ，已报销 ， ......”


##  六. PHP更改消息状态接口
  注意：在已审核情况下才能用
   model('Notify')->changeStatus(I('notify_id')) ;
返回true false

· 20160520新增：
  电脑端审核通过后，手机端在查看审核详情时，需要通过判断历史记录接口返回的mystatus字段，当mystatus>=1时，通过接口更改这条信息的状态为已审核并且不能操作了


##  七. 在应用中审核后调用接口
 > 注意：在已审核情况下才能用
```` php
   # $con_id ： 发送通知的数据id，为你的应用审核表的主键
   model('Notify')->changeNotifyStatus($con_id) ;
````
返回成功 :+1: 
```` php
 array("status"=>"修改状态成功！" ,'notify_id'=>$id) ;
````
返回失败 :+1: 
```` php
 array("status"=>"修改状态失败！" ,'notify_id'=>$id) ;
````
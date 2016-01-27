# 首页消息接口说明


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
        $data['link'] = $arr['link'];       //查看详情跳转地址
        $data['receive'] = $arr['receive'];       //接受者uid
        $data['menu_id'] = 0 ;  // menu.html中左侧菜单对应的id ;
        $data['type'] = 1;     //类型必须为1

        // 获取审核详情地址，具体说明见下面五
        $data['detail_url'] = $arr['detail_url'];   

```` 

###  2.有操作的消息（协同，只有一个确定按钮）

```` php
/** 
* 提交的$data 格式  
*/
        // 必填
        $data['title'] = $arr['title'];       // 标题说明
        $data['content'] = $arr['content'];  // 大概内容描述
        $data['link'] = $arr['link'];       //查看详情跳转地址
        $data['type'] = 3 ; 
        $data['check_url'] = $arr['check_url'] ;    // 点击确定的php处理地址
        $data['is_reject'] = 0 ;   //没有取消 
        $data['receive'] = $arr['receive'];       //接受者uid
        $data['menu_id'] = 0 ;  // menu.html中左侧菜单对应的id ;
       
       // 获取历史记录地址， 格式index.php?app=Kaoqin&m=Index&test ，地址返回json格式 
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
        $data['link'] = $arr['link'];       //查看详情跳转地址
        $data['receive'] = $arr['receive'];       //接受者uid
        $data['type'] = 2或者3 ;  //业务审批($type = 2) ; 办公审批($type = 3) 
        $data['check_url'] = $arr['check_url'] ;  //点击审核操作php处理地址
        $data['reject_url'] = $arr['reject_url'] ;   //点击驳回操作php处理地址
        $data['next_check_url'] = $arr['next_check_url'] ;   //点击提交下一个人审核的php处理地址
   
        $data['menu_id'] = 0 ;  // menu.html中左侧菜单对应的id ;

        // 获取历史记录地址， 格式index.php?app=Kaoqin&m=Index&test ，地址返回json格式 
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
/** 点击审核/不通过按钮   首页给应用的参数通过get方式
* @return 传输格式
*  status  状态  1同意  0驳回  2提交给下一个人
*  reply_text   审批意见
*  next_uid  下一个人的 next_uid  
*/ 
  index.php?app=Kaoqin&m=Index&a=ce&status=1&reply=我同意了&next_uid=6

    
````

```` php
/** 审核成功
* @return 返回格式
* 
*/ 

 $result['status'] = 1 ; 
 $result['info'] = "Success" ;  //可以填您处理程序的结果的文字，会在首页显示 
    
````

```` php
/** 驳回
* @return 返回格式
*/ 

 $result['status'] = 0 ; 
 $result['info'] = "Error" ;  //可以填您处理程序的结果的文字，会在首页显示 
    
````


## 四. 历史记录的地址返回的数据格式： 
 
```` php
/** 驳回
* @return 返回格式
*/ 

 $result['grade_uid'] =  0 ;   //审核人的uid 
 $result['grade_name'] =  "" ;   //审核人的名字
 $result['inserttime'] = "2015-12-19 12:00:00" ;  //处理时间  ，用友好时间处理过的 
 $result['status'] = 0或者1 、2;  //1 已审核 0待处理   2驳回
 $result['replay_text'] = "处理意见";  //填写处理意见
 $result['apply_uid'] = 0;  //上一个发起人的uid ，最近的是谁提交的
 $result['apply_name'] = "";  //上一个发起人的名字 
 $result['img'] = "";  //上一个发起人的头像
    
````

##  五. 审核详情说明： 
   审核详情的url打开是个完整的页面，可供首页调用，url里面的参数决定详情的不同


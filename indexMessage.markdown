# 首页消息接口说明

## php后台添加消息接口调用方式：
```` php
/**
* @param $data为添加的数据数组
* 返回格式如下
* $result['status'] = 1 ; 
* $result['info'] = "Success" ; 
*/ 

    $result = model('Notify')->add_notify($data);
 
````


## data的格式如下 ， 请选择对应的类型

###  1.提交只查看的消息（无任何操作）

```` php
/** 
* 提交的$data 格式  
*/
         $data['title'] = $arr['title'];       // 标题说明
        $data['content'] = $arr['content'];  // 大概内容描述
        $data['link'] = $arr['link'];       //查看详情跳转地址
        $data['menu_id'] = 0 ;  // menu.html中左侧菜单对应的id ;
        $data['type'] = 1;     //类型必须为1
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
        $data['menu_id'] = 0 ;  // menu.html中左侧菜单对应的id ;
       
       // 获取历史记录地址， 格式index.php?app=Kaoqin&m=Index&test ，地址返回json格式 
       $data['check_history_url'] = $arr['check_history_url'] ;

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
        $data['type'] = 2或者3 ;  //业务审批($type = 2) ; 办公审批($type = 3) 
        $data['check_url'] = $arr['check_url'] ;  //点击审核操作php处理地址
        $data['reject_url'] = $arr['reject_url'] ;   //点击驳回操作php处理地址
        $data['next_check_url'] = $arr['next_check_url'] ;   //点击提交下一个人审核的php处理地址

        $data['menu_id'] = 0 ;  // menu.html中左侧菜单对应的id ;

        // 获取历史记录地址， 格式index.php?app=Kaoqin&m=Index&test ，地址返回json格式 
       $data['check_history_url'] = $arr['check_history_url'] ;	


        // 选填
        $data['is_reject'] = $arr['is_reject'] ;   //是否有驳回按钮 ，默认1：有   ，0：无
        $data['is_next_check'] = $arr['is_next_check'] ;   //是否有提交下一步审核的按钮， 默认1：有   ，0：无
        $data['check_name'] = $arr['check_name'] ;   //审核的按钮的名称，默认：审核
        $data['reject_name'] = $arr['reject_name'] ;   //审核的按钮的名称，默认：驳回
        $data['next_check_name'] = $arr['next_check_name'] ;   //审核的按钮的名称，默认：提交下一步审核	
        
        	
```` 
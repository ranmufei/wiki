


## 三. 审核和驳回php处理后返回的格式(包含提交下一步审核后再次点击审核的操作)： 

```` php
/** 点击审核/不通过按钮   首页给应用的参数通过get方式
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
    
````

```` php
/** 驳回
* @return 返回格式
*/ 

 $result['status'] = 0 ; 
 $result['info'] = "Error" ;  //可以填您处理程序的结果的文字，会在首页显示 
    
````


## 四. 历史记录的地址返回的数据格式：
 
 type : post ;
postdata : {id: 当前消息的内容con_id  , notify_id : 当前消息的id }
```` php
/** 驳回
* @return 返回格式
*/ 

 $result['grade_uid'] =  0 ;   //审核人的uid 
 $result['grade_name'] =  "" ;   //审核人的名字
 $result['inserttime'] = "2015-12-19 12:00:00" ;  //处理时间  ，用友好时间处理过的 
 $result['status'] = 0或者1 、2;  //1 已审核 0待处理   2驳回
 $result['reply_text'] = "处理意见";  //填写处理意见
 $result['apply_uid'] = 0;  //上一个发起人的uid ，最近的是谁提交的
 $result['apply_name'] = "";  //上一个发起人的名字 
 $result['img'] = "";  //上一个发起人的头像
    

//注意：工作流协同额外加了2个字段，与data平级
$is_last = 0或1   //0没有最终审核    1已结最终审核了 ,用于判断关掉审核输入框
$mystatus = 0或1、2        // 0没有审核   1审核同意 2 审核没同意  ,用于判断显示按钮
````

##  五. 审核详情说明： 
   审核详情的url打开是个完整的页面，可供首页调用，url里面的参数决定详情的不同
  type : post ;
  postdata : {id: 当前消息的内容con_id  , notify_id : 当前消息的id }
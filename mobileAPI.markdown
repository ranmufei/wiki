# API接口列表

>    私有盘的移动端的API接口以后统一放到这里

### 登陆
* [用户登陆](load_user)

### 客户管理
* [接口列表](custom_api_list)

### 现金流接口
* [现金流报表](cws_cashflow_report)
* [经营业绩报表](cws_achieve_report)

### 通讯录
* [通讯录列表](contacts_list)
* [通讯录用户详情](contacts_user_message)
* [通讯录是否有更新](comtxl_get_status)

### 通知公告
* [公告列表](notice_list)
* [公告详情](notice_message)

### 网盘

##### 个人网盘

* [文件分类数量统计](disc_amount)
* [文件夹列表 （所有）](disc_lists)
* [文件分类列表 （图片 文档 文本 其它）](disc_classify_lists)
* [文件上传](disc_uploadify)
* [文件下载](disc_downloadFile)
* [文件夹创建](disc_create_folder)
* [文件（夹）删除](disc_delete)
* [文件（夹）重命名](disc_rename)
* [文件分享 (个人)](disc_share)
* [文件分享 (部门)](disc_share__depart)
* [文件夹列表](disc_folder_lists)
* [分享列表（自己）](disc_myshare)

##### 共享网盘
* [文件夹列表 （所有）](disc_share_lists)
* [文件分类列表 （共享：图片 文档 文本 其它）](disc_classify_share_lists)
* [文件分类数量统计](disc_share_amount)

##### 公司网盘
* [文件(夹)列表](company_lists)

### 进销存
* [产品列表](productList)
* [产品具体详情](productInfo)
* [订单列表](orderList)
* [订单详情](orderInfo)

### 项目管理
* [项目列表](projectList)
* [项目详情](projectInfo)
* [项目我的任务列表](myprojectList)
* [项目我的任务详情](myprojectInfo)

### 考勤管理
* [公司考勤时间](companySett)
* [移动考勤](playKa)
* [移动考勤状态](MyKaoqin)
* [查看提交给自己的考勤申请列表](get_shenh_list)
* [提交给下一个人审核](shenh_check_next)
* [考勤直接审核](shenh_check)
* [审核的人权限判断](shenh_power)

### 工作流
* [工作流思维流程](my_luoji)
* [我的全部工作流](my_workflow)
* [我待处理的任务](my_task)
* [任务详情](mytask_Info)
* [工作流详情](workflow_Info)
* [审核工作流](workflow_shenhe)
* [发送催促](workflow_msg)
* [操作记录](workflow_history)
* [获取选择下一个审核人列表](workflow_member)
* [提交下一个审核人](workflow_user)


### 日程
* [个人日程](Calendar_index)
* [受邀日程](Calendar_request)
* [日程详情](Calendar_Info)
* [添加日程](Calendar_add)
* [日程分类](Calendar_category)
* [日程回复](Calendar_answer)

### 报销管理
* [报销列表](bxlist)
* [报销单详情](bxinfo)
* [票据列表](pjlist)
* [票据详情](pjinfo)
* [报销选择票据](userpj)
* [报销单的上传接口](addbx)
* [报销审核](passbx)
* [新建票据的上传接口](addpj)
* [类别、项目列表](pclist)
* [报销选人（只显示有权限的）](selectaudit)

### 资产管理
* [易耗品及详细](consumable_list)
* [历史详细](goods_history)
* [我的申请易耗列表](consumable_Myapply_list)
* [易耗品申请操作](consumable_apply)
* [未出租申租品列表以及详细信息](rent_list)
* [我的申租品申请列表](rent_Myapply_list)
* [未出租的申租品详细编号](number_not_rent)
* [申租品申请操作](rent_apply)
* [易耗品需要审核列表](consumable_check_list)
* [申租品需要审核列表](rent_check_list)
* [审核通过操作](pass_save)
* [审核驳回操作](save_reject)
* [物品审核申租品里的详细信息](right_view)
* [验证是否拥有审核权限](permission)
* [申租品归还操作](state_save)
* [物品审核中申租品确认归还操作](sure_return)
* [提交下一步审核](goods_next_check)
* [易耗品确认申领操作](easy_sure)

### Eboss
* [考勤前一天情况比例](kaoqin_percent)
* [进销存Eboss数据概况](invoicing_data)
* [Eboss的权限接口](promisson_eboss)

### 知识分享
* [所有知识分页列表](lore_list)
* [分享新知识](add_lore)
* [获取知识详细信息](get_lore_detaile)
* [添加知识评论返回评论树](add_comment_tree)
* [获取标签和有权限的分类列表](get_label_category)
* [附件上传接口](set_files)
* [回复评论返回评论树](add_reply_comment)

### 项目管理
* [项目管理动态内容列表](p_notice_list)
* [项目管理添加动态](p_notice_add)
* [全部项目列表](p_project_list)
* [我的项目列表](p_project_list_my)
* [项目详细动态列表](p_project_notice)
* [项目里需求动态](p_project_need)
* [任务列表](p_project_task)
* [测试列表](p_project_test)
* [服务列表](p_project_server)
* [创建项目](creatProject)
* [删除项目](delete_pro)
* [编辑项目提交参数](edit_proing)
* [附件上传接口](fj_upload)
* [附件取消接口](fj_remove)
* [团队成员删除操作](delete_user)
* [项目添加团队成员操作](add_user)
* [我的任务列表](my_task_list)
* [我的测试列表](my_test_list)
* [我的服务列表](my_serve_list)
* [创建开启需求](creatneed)
* [获取项目参与人员](get_project_user)
* [回复动态的接口](add_revert)
* [设为讨论结果](set_zj)
# API接口列表

>    私有盘的移动端的API接口以后统一放到这里

### 登陆
* [用户登陆](load_user)

### 客户管理
* [接口列表](custom_api_list)

### 销售管理
* [接口列表](sale_api_list)

### 售后管理
* [接口列表](AfterSalers_api_list)

### 抢单
* [抢单列表](Grab_api_index)
* [抢单详情](zixiu_info)
* [抢单](Grab_api_grab)

### 进销存
* [产品管理](Invoicimg_api_product)
* [采购管理](Invoicimg_api_Purchase)
* [库存管理](Invoicimg_api_Instock)
* [二维码扫描信息](Invoicimg_api_erweima)
* [二维码扫描入库接口](Invoicimg_api_into_erweima)


### 生产ERP
* [原料管理](Invoicimgs_api_product)
* [原料采购](Invoicimgs_api_Purchase)
* [原料库存](Invoicimgs_api_Instock)


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

### 首页审核/消息
* [审核列表](audit_list)
* [审核新消息](audit_new)
* [审核操作、历史记录、详情](audit_other)
* [日程新消息数据](audit_rc)
* [更改1条消息状态](audit_status)
* [更改多条消息状态](audit_status_mulit)
* [发送回执](audit_twitter)
* [我发起的审核](my_audit)


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

##### 应用附件
* [当前用户是否有权限进入应用附件](app_accessor)
* [应用附件 首页应用文件夹列表](Appaccessory)
* [应用附件 下属文件夹内容详情](Appaccessory_list)

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
* [查看当前所有人的考勤记录](kaoqin_report)
* [查看本人的考勤记录](kaoqin_history)
* [接收提交的考勤申请数据（非补卡申请）](add_kaoqin_record)
* [接收提交的补卡申请数据](add_qiandao_record)
* [获取当前这个人的考勤设置](get_my_set)
* [考勤审核权限的人员列表](power_kaoqin)

### 工作流
* [工作流思维流程](my_luoji)
* [应用权限](power_list)
* [我的全部工作流](my_workflow)
* [我待处理的任务](my_task)
* [任务详情](mytask_Info)
* [工作流详情](workflow_Info)
* [审核工作流](workflow_shenhe)
* [发送催促](workflow_msg)
* [操作记录](workflow_history)
* [操作记录详情](workflow_history_info)
* [全公司列表](manager)
* [流程列表](liucheng_list)
* [表单列表](form_list)
* [重新选择审核人](check_user_change)
* [重新选择写同人](check_workerid)
* [获取选择下一个审核人列表](workflow_member)
* [提交下一个审核人](workflow_user)
* [判断选择审核人和协同人](workflow_check)
* [删除工作](workflow_delete)


### 日程
* [个人日程](Calendar_index)
* [受邀日程](Calendar_request)
* [日程详情](Calendar_Info)
* [添加日程](Calendar_add)
* [日程分类](Calendar_category)
* [日程回复](Calendar_answer)
* [日程新界面](Calendar_list)

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
* [获取项目管理列表](get_pmanager_list)

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
* [易耗品分类](easy_cat)
* [申租品分类](rent_cat)
* [搜索](easy_serch)
* [数量](asset_num)
* [我的审核（待审批/审批）](consumable_check_list_part)
* [易耗品分类的相关数据](easy_cat_data)
* [申租品分类的相关数据](rent_cat_data)

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
* [编辑讨论](need_editing)
* [发送任务](creatTask)
* [发送测试](creattest)
* [发送服务](creatserver)
* [任务点击详细](taskview)
* [测试点击详细](testview)
* [服务点击详细](serveview)
* [总数](get_all_count)
* [开启讨论](set_need_on)
* [关闭讨论](set_need_off)
* [发测试里的任务列表](fromtest)
* [反馈至任务的测试](returntotask)
* [测试组处理意见](task_solve)
* [根据id来查询项目详细内容](project_info)
* [获取项目附件的接口](getNewfj)
* [刚进入项目时候的判断](get_all_judge)
* [删除任务接口](delete_task)
* [删除测试接口](delete_test)
* [编辑测试](test_editing)
* [编辑任务](task_editing)

### 询盘报价管理
* [需求报价/获取所有需求报价列表](IndexMobile_getDataLists)
* [需求报价/查看需求详情](VersionMobile_getDetailes)
* [需求报价/查看版本基本物料](VersionMobile_getVersionBasicMaterial)
* [需求报价/新增需求](VersionMobile_requireAdd)
* [需求报价/需求信息修改](IndexMobile_editRequire)
* [需求报价/新增版本](VersionMobile_addVersion)
* [需求报价/版本操作/新增附件](VersionMobile_fileAdd)
* [需求报价/版本操作/删除附件](VersionMobile_fileDel)
* [需求报价/版本操作/版本状态修改操作](VersionMobile_versionStatusOpt)
* [需求报价/新增版本获取物料API](VersionMobile_getRawMaterial)
* [技术核价/获取所有版本列表](TechnologyMobile_getDataLists)
* [技术核价/获取版本详情](TechnologyMobile_getDetailes)
* [技术核价/获取基本物料数据](TechnologyMobile_getVersionBasicMaterial)
* [需求核价/获取所有版本列表](TechnologyMobile_getDataLists)
* [需求核价/获取版本详情](TechnologyMobile_getDetailes)
* [需求核价/获取基本物料数据](TechnologyMobile_getVersionBasicMaterial)
* [报价审核/获取所有版本列表](TechnologyMobile_getDataLists)
* [报价审核/获取版本详情](TechnologyMobile_getDetailes)
* [报价审核/获取基本物料数据](TechnologyMobile_getVersionBasicMaterial)
* [物料操作/Bom 添加](VersionMobile_addStructBOM)
* [物料操作/新增物料](VersionMobile_addVersionMaterial)
* [物料操作/物料删除](TechnologyMobile_delVersionMaterial)
* [物料操作/物料单耗修改](TechnologyMobile_save_data)
* [物料操作/修改其他成本/利润](TechnologyMobile_save_total_price)
* [版本操作/版本状态修改](TechnologyMobile_changeVersionStatus)
* [产品定型/获取所有版本列表](ProductApprovalMobile_getDataLists)
* [产品定型/获取版本详情](ProductApprovalMobile_getDetailes)
* [产品定型/获取基本物料数据](TechnologyMobile_getVersionBasicMaterial)
* [产品定型/获取规格物料数据](TechnologyMobile_getVersionBasicMaterial2)
* [订单管理/获取所有订单列表](OrderManageMobile_getDatasList)
* [订单管理/获取订单详情](OrderManageMobile_getDetailes)
* [订单管理/获取子订单列表](OrderManageMobile_getChildOrderDatasList)
* [订单管理/订单审核操作](OrderManageMobile_shStatusOpt)
* [订单管理/订单操作历史记录](OrderManageMobile_getLogList)

* [选人列表](OrderManageMobile_getShList)
* [得到重新报价详情](TechnologyMobile_get_price)
* [驳回](OrderManageMobile_bh)
* [订单修改](OrderManageMobile_editGoodsOpt)
* [订单删除](OrderManageMobile_delGoodsOpt)
* [附件删除](OrderManageMobile_fileDel)
* [系统单位列表](IndexMobile_getUnit)

### 汽车4S店客户管理
* [跟进提醒（销售顾问）/获取七天跟进客户](TrackMobile_Select)
* [跟进提醒（销售顾问）/获取跟进客户列表](TrackMobile_record)
* [回访提醒（销售顾问）/获取七天回访客户](VisitMobile_Select)
* [回访提醒（销售顾问）/获取回访客户列表](VisitMobile_record)
* [战败请求（销售顾问）/获取战败列表](DefeatMobile_record)
* [客户查询（销售顾问）/潜在客户列表](SelectMobile_record)
* [客户查询（销售顾问）/订单客户列表](OrderMobile_record)
* [客户查询（销售顾问）/我的车主列表](OwnerMobile_record)
* [客户查询（销售顾问）/我的客户列表](ClientInfoMobile_clientInfo)
* [客户查询（销售顾问）/无跟进计划客户列表](VersionMobile_clientPlan)
* [专营店客户查询（经理）/接待记录列表](ManageRecordMobile_record)
* [专营店客户查询（经理）/历史跟进列表](ManageHtrackMobile_record)
* [专营店客户查询（经理）/历史回访列表](ManageHvisitMobile_record)
* [专营店客户查询（经理）/潜在客户列表](ManagePotentialMobile_record)
* [专营店客户查询（经理）/我的客户列表](ManageClientMobile_clientInfo)
* [专营店客户查询（经理）/我的车主列表](ManageOwnerMobile_record)
* [专营店客户查询（经理）/订单管理列表](ManageOrderMobile_record)
* [专营店客户查询（经理）/退换车列表](ManageExchangeMobile_clientInfo)
* [专营店客户查询（经理）/无跟进计划客户列表](ClientInfoMobile_managePlan)
* [接待记录列表筛选](ManageRecordMobile_getSelect)
* [得到接待记录处理状态列表](ManageRecordMobile_status)
* [获取战败明细](DefeatMobile_getDefeatInfo)
* [获取客户详情](TrackMobile_info)
* [获取订单信息](OrderMobile_getAduit)
* [获取跟进信息](TrackMobile_getChanceInfo)
* [修改跟进信息](TrackMobile_editTrack)
* [获取战败原因列表](DefeatMobile_reason)
* [添加战败请求](DefeatMobile_adddefeat)
* [获取回访信息](VisitMobile_getChanceInfo)
* [修改回访信息](TisitMobile_editVisit)
* [订单成交](OrderMobile_setCar)
* [成交信息](OrderMobile_getOrderStatus)
* [退单申请](OrderMobile_setdownAduit)
* [订单申请](OrderMobile_setAduit)
* [意向品牌下的车型](OrderMobile_brand)
* [车型下的规格](OrderMobile_product)
* [回访计划列表](OwnerMobile_getVisitInfo)
* [退换车信息](OwnerMobile_getbackCar)
* [提车](OwnerMobile_addVisit)
* [退换车](OwnerMobile_exchange)
* [无跟进计划客户跟进列表](ClientInfoMobile_trackType)
* [无跟进计划客户跟进](ClientInfoMobile_addTrack)
* [退单审核](ManageOrderMobile_aduit)
* [退换车审核信息](ManageExchangeMobile_getExchange)
* [退换车审核](ManageExchangeMobile_aduit)
* [客流量统计](IndicatorMobile_selectFlow)
* [建卡量统计](IndicatorMobile_addClient)
* [今天](IndexMobile_date)
* [客户跟进统计](TrackManageMobile_getData)
* [客户回访统计](VisitManageMobile_getData)
* [销售指标统计](IndicatorMobile_saleFlow)
* [权限](IndexMobile_level)
* [战败列表（经理）](DefeatMobile_defeatInfo)
* [战败处理（经理）](DefeatMobile_level)
* [展厅温度分析](IndicatorMobile_galleryFlow)
* [展厅营业报表](ExhibitionMobile_getData)
* [逾期统计分析](OverdueMobile_getData)
* [客户来源分析](SourceMobile_getData)
* [首页提醒](IndexMobile_getInfo)
* [检测手机号码是否存在](ClientInfoMobile_verification)
* [建卡初始化信息](ClientInfoMobile_exploit)
* [提交客户信息](ClientInfoMobile_addClient)
* [客户跟进](ClientInfoMobile_track)
* [查询待完善客户](ClientInfoMobile_wanshan)
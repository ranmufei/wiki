### **需求报价/新增版本**
index.php?app=InquiryManageClothing&m=VersionMobile&a=addVersion

### **公网测试**
http://www.apps.com/index.php?app=InquiryManageClothing&m=VersionMobile&a=addVersion&access_token=67f244a585df480f51e9b81037f6d4

### **请求方式**
get


### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| rid| 是 | int|需求id|
| version| 是 | array|版本数据|
| parentStruct| 是 | array|Bom 结构|
| supDatas| 是 | array|物料|

       version   :   array 新增数据 
                                    rid    : 0,     //需求rid
                                    rname  : '',    //需求名
                                    rnumber: '',    //需求号
                                    vnumber: '',    // 子版本号
                                    name   : '',    // 子版本名
                                    remark : '',    // 备注
                                    files  : [],    // 附件   array 
                                                                 [0][name]       // 附件名
                                                                 [0][file]       // 附件地址 
                                                                 [0][show_file]  //附件展示地址
                                                                 [0][type]       // 类型
                                                                 [0][downurl]    // 下载id  
                                    parentVersionNumber:'',  // 父版本名
                                    p_vid :0,                // 父版本id
                                

        parentStruct : array Bom 结构 [0][id]            // id
                                      [0][name] 
                                      [0][pid] 
                                      [0][path]
                                      [0][is_semi_pro]
       
        supDatas     : array 物料     [0][sid]           //  Bom id
                                      [0][sname]         //  Bom 名
                                      [0][is_semi_pro]   //  是否是半成品
                                      [0][cat_id]        //  物料分类id
                                      [0][proname]       //  物料名
                                      [0][class_id]      //  物料分类id
                                      [0][class_name]    //  物料分类名
                                      [0][code]          //  物料编码
                                      [0][name]          //  物料名
                                      [0][f_id]          //  物料规格id
                                      [0][stornNum]      //  物料库存
                                      [0][unit]          //  物料单位id
                                      [0][unitName]      //  物料单位名
                                      [0][id]            //  索引id
                                      [0][is_stock]      //  是否是新的物料(1,是;0,不是)
                                      [0][purchasePrice] //  成本价
                                      [0][num]           //  物料数量
                                      [0][price]         //  价格
                                      [0][wastage]       //  损耗
                                      [0][total_price]   //  物料总价
                                      [0][batchid]       //  批次id
                                      [0][batchname]     //  批次名
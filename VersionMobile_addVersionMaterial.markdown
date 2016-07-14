### **物料操作/新增物料**
index.php?app=InquiryManageClothing&m=VersionMobile&a=addVersionMaterial

### **公网测试**
http://www.apps.com/index.php?app=InquiryManageClothing&m=VersionMobile&a=addVersionMaterial&access_token=67f244a585df480f51e9b81037f6d4

### **请求方式**
get


### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| vid| 是 | int|版本vid|
| sid| 是 | int|规格sid|
| data| 是 | array|物料|

     data  : array 物料     
                      [0][sid]           //  Bom id
                      [0][sid_t_id]      //  Bom 索引id
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


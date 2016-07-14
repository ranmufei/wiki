### **需求报价/新增需求**
index.php?app=InquiryManageClothing&m=VersionMobile&a=requireAdd

### **公网测试**
http://www.apps.com/index.php?app=InquiryManageClothing&m=VersionMobile&a=requireAdd&access_token=67f244a585df480f51e9b81037f6d4 

### **请求方式**
post


### **参数**
| 参数名称  |必填|     类型     | 说明 |
|------|-----|------|------|
| data| 是 | array  |{ //添加的数据  
                                    rnumber: '',  //  需求号 必须
                                    name: '',     //  需求名 必须
                                    cid: 0,       //  客户cid 必须 
                                    data: '',     //  内容   
                                    remark: '',   //  备注
                                    unit_id:0,    //  单位id  (系统单位id)
                                }|
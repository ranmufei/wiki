### **请求接口**
/index.php?app=Lore&m=LoreApi&a=getStorehouseDetailed

### **请求方式**
post

### **公网测试**
http://www.apps.com/index.php?app=Lore&m=LoreApi&a=getStorehouseDetailed

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| id     | 是 |   知识唯一ID   |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|id     |int |int |知识唯一ID         |
|uid      |int         |int  |分享人ID    |
|category_id      |int         |int  |知识分类ID    |
|add_time      |int         |int  |分享知识时间    |
|edit_time      |int         |int  |修改知识时间    |
|edit_uid      |int         |int  |修改人ID    |
|share      |int         |int  |是否分享    |
|title      |string         |string  |知识标题    |
|titlepinying      |string         |string  |知识标题拼音码    |
|content      |string         |string  |知识内容    |
|label_id      |int         |int  |标签ID    |
|nice_count      |int         |int  |点赞数    |
|comment_count      |int         |int  |评论数    |
|like_count      |int         |int  |关注数    |
|down_id      |int         |int  |附件ID    |
|u_name      |string         |string  |分享人名称    |
|category_name      |string         |string  |分类 名称    |
| --------- |--------      |--------|--------       |
|comment      |array         |array  |评论树    |

### **示例**
````php
{
    data: {
        detailed: {
            id: "21",
            uid: "1",
            category_id: "1",
            add_time: "07-20 18:28",
            edit_time: 0,
            edit_uid: 0,
            share: "0",
            title: "wang",
            titlepinyin: "wang",
            content: "<p> <img src="/Uploads/2015/0720/18/55acd08796404.png" alt="" /> </p> <p> <span style="color: #E53333;"><img src="/Uploads/2015/0720/18/55accd8c368f1.png" alt="" /></span> </p> <p> <span style="color: #E53333;">2222222222222222222222</span> </p>",
            label_id: [
                {
                    id: "2",
                    label_name: "技术",
                    label_color: "#428BCA"
                }
            ],
            nice_count: "0",
            comment_count: "1",
            like_count: "0",
            down_id: [
                {
                    id: "2761",
                    attach_type: "Home",
                    pic_url: "",
                    userId: "1",
                    uploadTime: "1437388082",
                    name: "wang.png",
                    type: "image/png",
                    size: "12451",
                    extension: "png",
                    hash: "d59401fa05649076fe54e774ed889227",
                    private: "0",
                    isDel: "0",
                    savepath: "2015/0720/18/",
                    savename: "55accd3217e2c.png",
                    savedomain: "0",
                    persistentId: "",
                    persistentState: "10",
                    url: "./Uploads/2015/0720/18/55accd3217e2c.png",
                    download: "http://www.apps.com/index.php?app=Home&m=Visitor&a=download&val=2761"
                }
            ],
            is_del: "1",
            u_name: "庆丰包子",
            category_name: "测试分享"
        },
        comment: [
            {
                id: "49",
                lore_id: "21",
                uid: "1",
                uid_name: "庆丰包子",
                uid_avatar: "./Uploads/avatar/0/1.jpg",
                add_time: "07-20 18:43",
                reply_uid: null,
                reply_name: null,
                parent_id: "0",
                content: "123123123",
                attr: [
                    
                ]
            }
        ]
    },
    info: "",
    status: "success"
}

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
            id: "9",
            uid: "1",
            category_id: "11",
            add_time: "07-15 10:06",
            edit_time: 0,
            edit_uid: 0,
            share: "1",
            title: "12312311111",
            titlepinyin: "12312311111",
            content: "12312312312312312312",
            label_id: [
                {
                    id: "4",
                    label_name: "市场",
                    label_color: "#8E44AD"
                }
            ],
            nice_count: "1",
            comment_count: "0",
            like_count: "1",
            down_id: "",
            is_del: "1",
            u_name: "庆丰包子",
            category_name: "语言知识"
        },
        comment: [
            {
                id: "5",
                lore_id: "9",
                uid: "1",
                uid_name: "庆丰包子",
                uid_avatar: "./Uploads/avatar/0/1.jpg",
                add_time: "06-15 20:04",
                reply_uid: "0",
                reply_name: "",
                parent_id: "0",
                content: "评论一个 不错不错",
                attr: [
                    {
                        id: "6",
                        lore_id: "9",
                        uid: "1",
                        uid_name: "庆丰包子",
                        uid_avatar: "./Uploads/avatar/0/1.jpg",
                        add_time: "06-15 20:04",
                        reply_uid: "1",
                        reply_name: "庆丰包子",
                        parent_id: "5",
                        content: "范德萨发范德萨范德萨",
                        attr: [
                            
                        ]
                    },
                    {
                        id: "7",
                        lore_id: "9",
                        uid: "1",
                        uid_name: "庆丰包子",
                        uid_avatar: "./Uploads/avatar/0/1.jpg",
                        add_time: "06-15 20:04",
                        reply_uid: "1",
                        reply_name: "庆丰包子",
                        parent_id: "6",
                        content: "范德萨发的萨芬",
                        attr: [
                            
                        ]
                    }
                ]
            },
            {
                id: "8",
                lore_id: "9",
                uid: "1",
                uid_name: "庆丰包子",
                uid_avatar: "./Uploads/avatar/0/1.jpg",
                add_time: "06-15 20:04",
                reply_uid: "0",
                reply_name: "",
                parent_id: "0",
                content: "范德萨发的萨芬",
                attr: [
                    
                ]
            },
            {
                id: "9",
                lore_id: "9",
                uid: "1",
                uid_name: "庆丰包子",
                uid_avatar: "./Uploads/avatar/0/1.jpg",
                add_time: "06-15 20:05",
                reply_uid: "0",
                reply_name: "",
                parent_id: "0",
                content: "范德萨范德萨范德萨",
                attr: [
                    
                ]
            }
        ]
    },
    info: "",
    status: "success"
}
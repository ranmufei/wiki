### **请求接口**
/index.php?app=Lore&m=LoreApi&a=getStorehouseList

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Lore&m=LoreApi&a=getStorehouseList

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| p     | 是 |   当前页数   |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|id     |int         |int |知识唯一ID         |
|uid       |string         |str  |知识分享人    |
|category_id       |int         |int  |知识分类ID    |
|add_time       |int         |int  |分享知识时间    |
|edit_time       |int         |int  |知识修改时间    |
|title       |string         |string  |知识标题    |
|titlepinyin       |string         |string  |标题拼音码    |
|label_id       |array         |array  |标签数组集    |
|nice_count       |int         |int  |点赞数    |
|comment_count       |int         |int  |评论数    |
|like_count       |int         |int  |关注数    |
|down_id       |int         |int  |附件ID    |

### **示例**
````php
{
    data: {
        detailed: {
            id: "3",
            uid: "1",
            category_id: "10",
            add_time: "07-15 09:04",
            edit_time: 0,
            edit_uid: 0,
            share: "1",
            title: "12312312312",
            titlepinyin: "12312312312",
            content: "123123123123123123123123123123",
            label_id: [
                {
                    id: "2",
                    label_name: "技术",
                    label_color: "#428BCA"
                },
                {
                    id: "5",
                    label_name: "端午策划方案",
                    label_color: "#5CB85C"
                }
            ],
            nice_count: "0",
            comment_count: "0",
            like_count: "0",
            down_id: "",
            is_del: "1",
            u_name: "庆丰包子",
            category_name: "知识3"
        },
        comment: [
            {
                id: "10",
                lore_id: "3",
                uid: "1",
                uid_name: "庆丰包子",
                uid_avatar: "./Uploads/avatar/0/1.jpg",
                add_time: "06-16 09:09",
                reply_uid: "0",
                reply_name: "",
                parent_id: "0",
                content: "2222222222222",
                attr: [
                    {
                        id: "34",
                        lore_id: "3",
                        uid: "307",
                        uid_name: "东距",
                        uid_avatar: "./Uploads/avatar/default.gif",
                        add_time: "06-26 17:00",
                        reply_uid: "1",
                        reply_name: "庆丰包子",
                        parent_id: "10",
                        content: "123123123123",
                        attr: [
                            
                        ]
                    },
                    {
                        id: "35",
                        lore_id: "3",
                        uid: "307",
                        uid_name: "东距",
                        uid_avatar: "./Uploads/avatar/default.gif",
                        add_time: "06-26 17:00",
                        reply_uid: "307",
                        reply_name: "东距",
                        parent_id: "34",
                        content: "12312312",
                        attr: [
                            
                        ]
                    }
                ]
            },
            {
                id: "31",
                lore_id: "3",
                uid: "307",
                uid_name: "东距",
                uid_avatar: "./Uploads/avatar/default.gif",
                add_time: "06-26 17:00",
                reply_uid: null,
                reply_name: null,
                parent_id: "0",
                content: "123123123123",
                attr: [
                    {
                        id: "33",
                        lore_id: "3",
                        uid: "307",
                        uid_name: "东距",
                        uid_avatar: "./Uploads/avatar/default.gif",
                        add_time: "06-26 17:00",
                        reply_uid: "307",
                        reply_name: "东距",
                        parent_id: "31",
                        content: "123123123",
                        attr: [
                            
                        ]
                    }
                ]
            },
            {
                id: "32",
                lore_id: "3",
                uid: "307",
                uid_name: "东距",
                uid_avatar: "./Uploads/avatar/default.gif",
                add_time: "06-26 17:00",
                reply_uid: null,
                reply_name: null,
                parent_id: "0",
                content: "123123123123",
                attr: [
                    
                ]
            }
        ]
    },
    info: "",
    status: "success"
}
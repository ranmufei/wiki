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
        count: "24",
        totalPages: 2,
        nowPage: 1,
        data: [
            {
                id: "8",
                uid: "庆丰包子",
                category_id: "11",
                add_time: "07-15 10:06",
                edit_time: 0,
                edit_uid: 0,
                title: "12312312312",
                titlepinyin: "12312312312",
                label_id: [
                    {
                        id: "3",
                        label_name: "重要",
                        label_color: "#F0AD4E"
                    }
                ],
                nice_count: "0",
                comment_count: "0",
                like_count: "0",
                down_id: 1
            },
            {
                id: "7",
                uid: "庆丰包子",
                category_id: "11",
                add_time: "07-15 09:27",
                edit_time: 0,
                edit_uid: 0,
                title: "213123",
                titlepinyin: "213123",
                label_id: [
                    {
                        id: "2",
                        label_name: "技术",
                        label_color: "#428BCA"
                    }
                ],
                nice_count: "0",
                comment_count: "0",
                like_count: "0",
                down_id: 1
            },
            {
                id: "6",
                uid: "庆丰包子",
                category_id: "10",
                add_time: "07-15 09:09",
                edit_time: 0,
                edit_uid: 0,
                title: "11111112222",
                titlepinyin: "11111112222",
                label_id: [
                    {
                        id: "4",
                        label_name: "市场",
                        label_color: "#8E44AD"
                    }
                ],
                nice_count: "0",
                comment_count: "0",
                like_count: "0",
                down_id: 1
            },
            {
                id: "5",
                uid: "庆丰包子",
                category_id: "1",
                add_time: "07-15 09:09",
                edit_time: 0,
                edit_uid: 0,
                title: "3123123",
                titlepinyin: "3123123",
                label_id: [
                    {
                        id: "3",
                        label_name: "重要",
                        label_color: "#F0AD4E"
                    }
                ],
                nice_count: "1",
                comment_count: "2",
                like_count: "253",
                down_id: 1
            }
        ]
    },
    info: "",
    status: "success"
}
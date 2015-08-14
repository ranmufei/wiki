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
                id: "31",
                uid: "庆丰包子",
                category_id: "3",
                add_time: "08-12 17:02",
                edit_time: 0,
                edit_uid: 0,
                title: "tu6u",
                titlepinyin: "tu6u",
                label_id: [
                    {
                        id: "2",
                        label_name: "技术",
                        label_color: "#428BCA"
                    }
                ],
                nice_count: "0",
                comment_count: "7",
                like_count: "0",
                down_id: 1
            },
            {
                id: "30",
                uid: "庆丰包子",
                category_id: "3",
                add_time: "08-10 11:24",
                edit_time: 0,
                edit_uid: 0,
                title: "123456789",
                titlepinyin: "123456789",
                label_id: [
                    {
                        id: "1",
                        label_name: "工作",
                        label_color: "#F0AD4E"
                    }
                ],
                nice_count: "0",
                comment_count: "1",
                like_count: "0",
                down_id: 1
            },
            {
                id: "29",
                uid: "庆丰包子",
                category_id: "12",
                add_time: "08-10 10:58",
                edit_time: 0,
                edit_uid: 0,
                title: "武汉",
                titlepinyin: "WH",
                label_id: [
                    {
                        id: "4",
                        label_name: "市场",
                        label_color: "#8E44AD"
                    }
                ],
                nice_count: "1",
                comment_count: "1",
                like_count: "0",
                down_id: 1
            },
            {
                id: "26",
                uid: "庆丰包子",
                category_id: "12",
                add_time: "08-10 10:30",
                edit_time: 0,
                edit_uid: 0,
                title: "测试机",
                titlepinyin: "CSJ",
                label_id: [
                    {
                        id: "1",
                        label_name: "工作",
                        label_color: "#F0AD4E"
                    },
                    {
                        id: "2",
                        label_name: "技术",
                        label_color: "#428BCA"
                    },
                    {
                        id: "4",
                        label_name: "市场",
                        label_color: "#8E44AD"
                    },
                    {
                        id: "5",
                        label_name: "端午策划方案",
                        label_color: "#5CB85C"
                    },
                    {
                        id: "6",
                        label_name: "10月",
                        label_color: "#428BCA"
                    }
                ],
                nice_count: "0",
                comment_count: "1",
                like_count: "0",
                down_id: 1
            },
            {
                id: "24",
                uid: "庆丰包子",
                category_id: "11",
                add_time: "07-25 10:45",
                edit_time: 0,
                edit_uid: 0,
                title: "33333333333",
                titlepinyin: "33333333333",
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
                down_id: 1
            },
            {
                id: "23",
                uid: "庆丰包子",
                category_id: "10",
                add_time: "07-20 19:08",
                edit_time: 0,
                edit_uid: 0,
                title: "656",
                titlepinyin: "656",
                label_id: [
                    {
                        id: "2",
                        label_name: "技术",
                        label_color: "#428BCA"
                    }
                ],
                nice_count: "1",
                comment_count: "0",
                like_count: "0",
                down_id: 1
            },
            {
                id: "22",
                uid: "庆丰包子",
                category_id: "3",
                add_time: "07-20 18:57",
                edit_time: 0,
                edit_uid: 0,
                title: "5656",
                titlepinyin: "5656",
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
                id: "20",
                uid: "庆丰包子",
                category_id: "3",
                add_time: "07-16 10:07",
                edit_time: 0,
                edit_uid: 0,
                title: "asdasd",
                titlepinyin: "asdasd",
                label_id: [
                    {
                        id: "5",
                        label_name: "端午策划方案",
                        label_color: "#5CB85C"
                    }
                ],
                nice_count: "0",
                comment_count: "0",
                like_count: "0",
                down_id: 1
            },
            {
                id: "18",
                uid: "庆丰包子",
                category_id: "1",
                add_time: "07-15 16:30",
                edit_time: 0,
                edit_uid: 0,
                title: "11111111111",
                titlepinyin: "11111111111",
                label_id: [
                    {
                        id: "1",
                        label_name: "工作",
                        label_color: "#F0AD4E"
                    }
                ],
                nice_count: "1",
                comment_count: "0",
                like_count: "1",
                down_id: 1
            },
            {
                id: "17",
                uid: "庆丰包子",
                category_id: "10",
                add_time: "07-15 11:56",
                edit_time: 0,
                edit_uid: 0,
                title: "jytjtyjty",
                titlepinyin: "jytjtyjty",
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
                id: "16",
                uid: "庆丰包子",
                category_id: "1",
                add_time: "07-15 10:48",
                edit_time: 0,
                edit_uid: 0,
                title: "12312311111",
                titlepinyin: "12312311111",
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
                id: "15",
                uid: "庆丰包子",
                category_id: "10",
                add_time: "07-15 10:48",
                edit_time: 0,
                edit_uid: 0,
                title: "2222222",
                titlepinyin: "2222222",
                label_id: [
                    {
                        id: "3",
                        label_name: "重要",
                        label_color: "#F0AD4E"
                    }
                ],
                nice_count: "0",
                comment_count: "0",
                like_count: "1",
                down_id: 1
            },
            {
                id: "14",
                uid: "庆丰包子",
                category_id: "11",
                add_time: "07-15 10:10",
                edit_time: 0,
                edit_uid: 0,
                title: "11111222222",
                titlepinyin: "11111222222",
                label_id: [
                    {
                        id: "5",
                        label_name: "端午策划方案",
                        label_color: "#5CB85C"
                    }
                ],
                nice_count: "0",
                comment_count: "0",
                like_count: "0",
                down_id: 1
            },
            {
                id: "13",
                uid: "庆丰包子",
                category_id: "11",
                add_time: "07-15 10:09",
                edit_time: 0,
                edit_uid: 0,
                title: "12312312312",
                titlepinyin: "12312312312",
                label_id: [
                    {
                        id: "5",
                        label_name: "端午策划方案",
                        label_color: "#5CB85C"
                    }
                ],
                nice_count: "0",
                comment_count: "0",
                like_count: "0",
                down_id: 1
            },
            {
                id: "12",
                uid: "庆丰包子",
                category_id: "11",
                add_time: "07-15 10:08",
                edit_time: 0,
                edit_uid: 0,
                title: "213123123",
                titlepinyin: "",
                label_id: [
                    {
                        id: "4",
                        label_name: "市场",
                        label_color: "#8E44AD"
                    }
                ],
                nice_count: "1",
                comment_count: "0",
                like_count: "0",
                down_id: 0
            },
            {
                id: "9",
                uid: "庆丰包子",
                category_id: "11",
                add_time: "07-15 10:06",
                edit_time: 0,
                edit_uid: 0,
                title: "12312311111",
                titlepinyin: "12312311111",
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
                down_id: 1
            },
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
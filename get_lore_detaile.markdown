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
        labels: [
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
                id: "3",
                label_name: "重要",
                label_color: "#F0AD4E"
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
            },
            {
                id: "7",
                label_name: "修改",
                label_color: "#D9534F"
            }
        ],
        category: [
            {
                id: "3",
                name: "技术部门",
                sort: "50",
                category_count: "6"
            },
            {
                id: "10",
                name: "知识3",
                sort: "50",
                category_count: "6"
            },
            {
                id: "11",
                name: "语言知识",
                sort: "50",
                category_count: "9"
            },
            {
                id: "12",
                name: "历史名著",
                sort: "50",
                category_count: "2"
            },
            {
                id: "1",
                name: "测试分享",
                sort: "40",
                category_count: "3"
            }
        ]
    },
    info: "",
    status: "success"
}
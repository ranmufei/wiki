### **请求接口**
/index.php?app=Lore&m=LoreApi&a=getLabelsCategory

### **请求方式**
post

### **公网测试**
http://www.apps.com/index.php?app=Lore&m=LoreApi&a=getLabelsCategory


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|labels     |array |array |标签集         |
|category      |array         |array  |分类集    |


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

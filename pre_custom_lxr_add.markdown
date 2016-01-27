### **请求接口**
列表
/index.php?app=Customer&m=MPrecontacts&a=no_relate_gsy

添加
/index.php?app=Customer&m=MPrecontacts&a=add_select_con


### **请求方式**
get


### **其他参数**
p、chance（为机会id）

add
客户的   themeid为客户的id，ids为一维数组，chanceid为0
机会的   themeid为0，ids为一维数组，chanceid为机会id

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data       |             |  array  |   |



``` javascript
Array
(
    [count] => 1
    [totalPages] => 1
    [nowPage] => 1
    [data] => Array
        (
            [0] => Array
                (
                    [id] => 179
                    [name] => youting123_lxr1111       //姓名
                    [custom_id] => uuuuu
                    [mobile] =>                         //手机
                    [sex] =>                              //性别
                    [createtime] => 15-11-19 14:58       //创建时间 
                )

        )

)

{
data: ""
info: "操作成功!"
status: "success"
}

{
0: 159
1: 120

}
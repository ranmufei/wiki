# 邮件接口说明
一.[邮件列表]()
---
+ url :/index.php?app=Email&m=Index&a=get_email
+ type:"post"
+ data:{
````
 folder:0,  //文件夹类型 0收件夹 1草稿夹 2发件夹 3删除夹 4垃圾箱  

 seen:0,  // 是否查看  0未看 1已看 2所有的 ，默认为所有的  

 flagged:0 , //是否星标 0未星标的  1已星标的  


 eid:vm.listMail[vm.current_index]['id'] , //账户id


 account:vm.listMail[vm.current_index]['account'],  //账户


 perPage:20       //每页多少条

````
}
+ 返回：
![1](http://192.168.1.240/uploads/ranmufei/apps/47a463c624/1.jpg)

---
二.[获取新邮件]()
---
+ url :/index.php?app=Email&m=Index&a=get_email
+ type:"get/post"
+ data:{new:1,eid:vm.listMail[vm.current_index]['id'],account:vm.listMail[vm.current_index]['account']}
+ 返回：
````
{
    errNum: 0,
    sucNum: 26,
    status: 1,
    info: "更新邮件成功！！"
    }
````
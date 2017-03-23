# 邮件接口说明
一.[邮件列表]()
---
+ url :/index.php?app=Email&m=Index&a=get_email
+ type:"post"
+ data:{folder:0,seen:0,eid:vm.listMail[vm.current_index]['id'] ,account:vm.listMail[vm.current_index]['account']}
+ 返回：
![1](http://192.168.1.240/uploads/ranmufei/apps/47a463c624/1.jpg)

---
二.[获取新邮件]()
---
+ url :/index.php?app=Email&m=Index&a=get_email
+ type:"get/post"
+ data:{new:1,eid:vm.listMail[vm.current_index]['id'],account:vm.listMail[vm.current_index]['account']}
+ 返回：
````php
    {
    errNum: 0,
    sucNum: 26,
    status: 1,
    info: "更新邮件成功！！"
    }
````
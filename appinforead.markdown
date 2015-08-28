# 应用配置说明#

- node.php 说明

>    权限配置应用  切忌不能和别人的应用有重复 ，但复制别人的应用 来创建自己的应用的时候 切忌不能吧node.php配置也给复制



- info.php


>   应用基本信息 请按照具体情况填写

```` php

   return array(
        'name' => '系统管理aa',
        'key'  => 'Adminaaaa',
        'type' =>'sys',
        'use' =>'c',
        'is_hide' =>0,      //是否隐藏
		'timer' => 0,
        //'level'=> '0',
        //'version'=>'1',
        'description'=>'系统管理面板，对当前系统中所有应用统一管理',
        'url'=>'index.php?app=Admin&m=Index&a=defaultIndex',  //默认进入应用路径
    );



```` 
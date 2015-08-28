# 应用配置说明#

- node.php 说明

>    权限配置应用  切忌不能和别人的应用有重复 ，但复制别人的应用 来创建自己的应用的时候 切忌不能吧node.php配置也给复制


``` php

<?php
    return array(
       'INVOIV_ceshi1df'=>array(
                'name'=>'进入进销存',
                'nodeType'=>'c',
                'nodes'=>array('Invoicimg.Index.index')
        ),
        'INVOIV_ceshi1'=>array(
                'name'=>'产品管理',
                'nodeType'=>'c',
                'nodes'=>array('Invoicimg.Product.editproduct','Invoicimg.Product.updataFormat')
        ),

)

```

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


-  initTable.php   `2015-08-28 新增加`

>  初始化应用数据专用  ，请在此配置中 填写可以被清空表的名称，特别注意的是 如果自己的表中有初始化数据的 请别添加否则会被清空的


```` php
   <?php
/**
 * 这里填写可以被清空的表，
 * 注意 如果有初始化数据的表 切忌不要填写
 */
    return array(
            'oa_jinxiao_gm_content',
            'oa_jinxiao_gm_order',
            'oa_jinxiao_ordersetting',
    );


````

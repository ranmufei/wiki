关于公司模型的说明,请对模型作出详细说明，并可以对主要的方法进行说明，具体的调用规则开发者请自己去看接口说明

#### 消息模型 (NotifyModel.class.php)
- 注: add方法添加消息已 `不推荐使用`
- addUserNews 添加个人消息 model('Notify')->addUserNews( $toUid , $title , $link , $content = '' , $d =array( ) )
- addAppNews 添加应用消息  model('Notify')->addAppNews( $toApp , $title , $link , $content = '' ,$d =array( ) )

# 案列

```` php

/**
         * 新增 个人消息
         * 
         * 本函数用来 替代 $this->add( ) 将发送 个人消息 的接口独立出来 。 本函数最后会调取 $this->add()方法完成消息的添加
         * 
         * @param $toUid 接收消息者的 uid   *
         * @param $title 消息标题
         * @param $link 链接地址
         * @param $content 消息简介 100字内
         * @param $d array 要修改一些 模型默认字段时使用


 /**
         * 添加 应用消息
         * 本函数用来 替代 $this->add( ) 将发送 应用消息 的接口独立出来 。 本函数最后会调取 $this->add()方法完成消息的添加
         * 
         * @param $toApp 接收消息的App
         * @param $title 消息标题
         * @param $link 链接地址
         * @param $content 消息简介 100字内

model('Notify')->addAppNews('Cws' , '采购订单（'.$order_num.'）等待财务审核！' , '/index.php?app=Cws&m=Index&a=others_pay_order&type=5' ,'订单'.$order_num.'等待财务审核！！！');//添加应用消息


````


* [进销存添加订单](jinxiaoaddorder)
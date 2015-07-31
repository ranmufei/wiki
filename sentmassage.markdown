# model('Notify')->addUserNews( $toUid , $title , $link , $content = '' , $d =array( ) ) #
      
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
         * 
         * @author guop
         * 
         * @version $time 2014/12/12 
         * 
         * @return bool true发送成功 false发送失败
         */ 


==        model('Notify')-> addAppNews( $toApp , $title , $link , $content = '' ,$d =array( ) )==

        /**
         * 添加 应用消息
         * 本函数用来 替代 $this->add( ) 将发送 应用消息 的接口独立出来 。 本函数最后会调取 $this->add()方法完成消息的添加
         * 
         * @param $toApp 接收消息的App
         * @param $title 消息标题
         * @param $link 链接地址
         * @param $content 消息简介 100字内
         * @param $d array 要修改一些 模型默认字段时使用
         * 
         * @author guop
         * 
         * @version $time 2014/12/12 
         * 
         * @return bool true发送成功 false发送失败
         * 
         */

        
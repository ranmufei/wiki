<?php
	
	/**
	 * 移动端 api接口  父类
	 */
    abstract class MobileAction extends Action {
        
        protected $uid;
        
        protected $num    =25 ;        //分页: 默认每页10条
        protected $page   =0 ;        //分页参数值
        protected $pName  ='p';       //分页参数名
        
        protected $startNum;       //分页 limit 第一个参数
        
        protected $response;
        
        function __construct() {
            $this->response =model('Response');     //数据返回模型类
            
            $this->initParams(); 
            
            if( method_exists( $this, '_initialize' ) )   
                $this->_initialize();
                
        }
        
        //初始化一些基本参数
        private function initParams(){
            (int)$_GET['num'] > 0 and $this->num =(int)$_GET['num'];  
            
            $pv =(int)$_GET[$this->pName];
            $pv <=1 and $pv =1;          
            
            $this->startNum =( $pv - 1 )*$this->num;
            
            $this->uid = isset( $_GET['uid'] ) ? (int)$_GET['uid'] : (int)$_POST['uid'] ;
        }       
    }
?>
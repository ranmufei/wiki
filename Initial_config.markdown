## 优势：
#### 初始化数据写到应用的配置文件中，不用写到数据库中，方便清空数据库。调用、修改与存数据库一样方便

## 步骤：
#### 1. 在应用的config.php中添加你新增的配置文件，注意最后加入到array_merge函数中
```` php
<?php
$config =array(
    
    'LAYOUT_ON'=>false,// 开启模版布局
);

$sysconfig =require_once(THINK_PATH.'appconfig.php');
$config_shop_set =require_once('App/Shouyin1/Conf/config_shop_set.php');
$config_shop_type_set =require_once('App/Shouyin1/Conf/config_shop_type_set.php');
$config_print =require_once('App/Shouyin1/Conf/config_print.php');
return array_merge($sysconfig,$config,$config_shop_set,$config_shop_type_set,$config_print);

````

#### 2. 新增的配置文件格式如下（返回一个数组）：
```` php
<?php 
 return array( 
  'shop_type_set' => array (
  'guimo' => 
  array (
    0 => '小型店铺',
    1 => '中型店铺',
    2 => '大型店铺',
  ),
  'pro_status' => 
  array (
    0 => '无货',
    1 => '部分缺失',
    2 => '库存良好',
    3 => '库存满足',
  ),
  'status' => 
  array (
    0 => '未经营',
    1 => '经营中',
  ),
  'shop_type' => 
  array (
    0 => '直营店',
    1 => '加盟店',
  ),
  'is_recharge_active' => false,
  'is_sale' => false,
) 
 );
````
#### 3. 使用C('pro_status')就可以调用配置，返回的是一个数组
```` php
array (
    0 => '无货',
    1 => '部分缺失',
    2 => '库存良好',
    3 => '库存满足',
  ),
````

#### 4. 修改配置文件
```` php
//修改配置文件
//$new_config为数组 , 格式为$new_config['a'] = 123 ;
//$config_file 为配置文件地址 ， 如'Home/Conf/config_shop_set.php' , 需要放在配置文件下面
protected function update_new_config($new_config, $config_file = '' ) {
     if(file_exists($config_file)){
              $config = require $config_file;
              
                if (is_writable($config_file) ) {

                 $config = array_merge($config, $new_config);
              //  dump($config);
                  $text = "<?php \n" . "return \n  " .stripslashes(var_export($config, true)) . ";"  ;
 
                file_put_contents($config_file, $text , LOCK_EX);
                return true;
                } else {
                return false;
              }
               
                 

        }else{
            $config = $new_config ;
            fopen($config_file , "a") ;
            $text = "<?php \n" . "return   \n  " .stripslashes(var_export($config, true)) . ";"  ;
            file_put_contents($config_file, $text , LOCK_EX);
            return true ;
        }
 
}
````
#### 在其他的地方通过ajax获取修改的值后调用：
```` php
/*打印设置*/
public function save_print_page(){

     $config_file = 'App/Shouyin1/Conf/config_print.php' ; 
     C('print_a', I('print_a')) ;
     C('print_b', I('print_b')) ;
     $new_config['print_a'] =  C('print_a') ; 
     $new_config['print_b'] =  C('print_b') ; 

     $res = $this->update_new_config($new_config , $config_file);

     $this->ajaxReturn($res);
}
````

## 注意事项:
  通过代码该的文件，git是不能进行版本控制的，所以修改后的配置文件时拉取不到最新的！
调试请通过C函数读取，上传新增的配置后注意不要本地修改后再上传！
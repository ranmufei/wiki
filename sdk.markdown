# 一.  云应用授权SDK说明

  * 云应用授权SDK是由程序自动化生成的代码包，其中包含了已经开放的API和相应的请求、验证、加密、返回解析等一些必要的功能。

  * 云应用授权SDK分为PCD上的SDK和云应用的SDK两部分。

  * 云应用授权SDK文件夹建议放在根目录下。

  * 支持的开发环境 ： 支持php5.3及以上；

# 二.  云应用授权SDK使用步骤

  1. 将pcd的sdk复制到程序目录(已复制的请忽略这一步)；
 
  2. 在需要的控制器中加入如下代码，将代码引入到

```` php
public function _initialize(){
      require_once "Linksame-sdk-pcd/PcdClient.php";	
      $PcdClient = new PcdClient();
      $this->PcdClient = $PcdClient ;
}
````
 3. 通过如下代码同步数据
```` php
$url = "http://shop.apps.com/index.php?g=Member&c=Index&a=member_list" ;	
			
			$res = $this->PcdClient->checkAccessToken() ; 

			$result = json_decode($res,true) ; 
			if($result && $result['status'] == 1001) {
					//可以同步数据了！！！
					$res = $this->PcdClient->pcdSendByPost($url)  ; 

					echo $res ;exit ; 
			}else{
					echo $res ;exit ; 
			} 
````
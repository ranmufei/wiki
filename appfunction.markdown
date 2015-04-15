``` php
<?php
// 实例化hook
function hook($name,$params=array()) {
    return X($name,$params,'Hook');
}

// 实例化插件
function plugin($name,$params=array()) {
    return X($name,$params,'Plugin');
}

// 实例化服务
function service($name,$params=array()) {
    return X($name,$params,'Service');
}

// 实例化widget
function widget($name,$params=array(),$return=false) {
    
    $class = $name . 'Widget';
    require_cache(ADDON_PATH . '/widgets/' . $class . '.class.php');
    if (!class_exists($class))
        throw_exception(L('_CLASS_NOT_EXIST_') . ':' . $class);
    $widget = Think::instance($class);
    $content = $widget->render($params);
    if ($return)
        return $content;
    else
        echo $content;
}

// 实例化model
function model($name,$params=array()) {
    
    return X($name,$params,'Model');
}

// 调用接口服务
function X($name,$params=array(),$domain='Service') {
    static $_service = array();
	$class = $name.$domain;
	if(file_exists(ADDON_PATH.'/'.$domain.'/'.$class.'.class.php')){
		require_cache(ADDON_PATH.'/'.$domain.'/'.$class.'.class.php');
	}else{
	   exit(ADDON_PATH.'/'.$domain.'/'.$class.'.class.php不存在');
	}
    
	//服务不可用时 记录日志 或 抛出异常
	if(class_exists($class)){
		$obj   =  new $class($params);
		$_service[$domain.'_'.$app.'_'.$name] =  $obj;
		return $obj;
	}else{
		throw_exception(L('_CLASS_NOT_EXIST_').':'.$class);
	}
}
//

function getIP()
{
if (isset($_SERVER)) {
if (isset($_SERVER['HTTP_X_FORWARDED_FOR'])) {
$realip = $_SERVER['HTTP_X_FORWARDED_FOR'];
} elseif (isset($_SERVER['HTTP_CLIENT_IP'])) {
$realip = $_SERVER['HTTP_CLIENT_IP'];
} else {
$realip = $_SERVER['REMOTE_ADDR'];
}
} else {
if (getenv("HTTP_X_FORWARDED_FOR")) {
$realip = getenv( "HTTP_X_FORWARDED_FOR");
} elseif (getenv("HTTP_CLIENT_IP")) {
$realip = getenv("HTTP_CLIENT_IP");
} else {
$realip = getenv("REMOTE_ADDR");
}
}
return $realip;
}

function url($url,$parms,$domain='',$echo=''){
  
    $linkarr =explode(':',$url);        //是否有app参数名
    $first =trim($linkarr[0]);
    if(!$first){        //补充完整地址
        global $_APP; 
        $url =$_APP['now']['key'].$url; 
    }
    
    if(1===2){
        $arr = include('router.inc.php');
        if(isset($arr['router'][$url])){
            $router = $arr['router'][$url];
            if($parms){
                parse_str($parms, $r);
                foreach ($r as $k => $v) {
					if (strpos($router, '['.$k.']'))
						$router = str_replace('['.$k.']', $v, $router);
					else
						$lr[$k]	= $v;
				}
                if (is_array($lr) && count($lr) > 0)
					$router .= '?' . http_build_query($lr);
                
            }
            $url = $router;
        }else{
            $arr = explode(':',$url);
            $url = 'index.php?app='.$arr[0].'&m='.$arr[1].'&a='.$arr[2];
            if($parms){
                $url .='&'.$parms;
            }
        }
        
        
    }else{
        $arr = explode(':',$url);
        $url = 'index.php?app='.$arr[0].'&m='.$arr[1].'&a='.$arr[2];
        if($parms){
            $url .='&'.$parms;
        }
    }
    
    $url =$domain.$url;
    
    if(!$echo){
        return $url;
    }else{
        echo $url;
    }
}


/**
 * 会员 头像
 * @param $uid 用户id
 */ 
function get_avatar($uid){
    !$uid and $uid =cookie('uid');
    
    //每个文件夹存入500张图片
    $menu=intval($uid/1500);
            
    $photo_name = $uid.'.jpg';
			
	$photo_path = AVATAR.$menu.'/'.$photo_name;

    if(file_exists($photo_path))
        return $photo_path; 
    else return AVATAR.'default.gif';
}

function friendlyDate($sTime,$type = 'normal',$alt = 'false') {
    if(!$sTime) {
        return '';
    }
    //sTime=源时间，cTime=当前时间，dTime=时间差
    $cTime = time();
    $dTime = $cTime - $sTime;
    $dDay = intval(date("Ymd",$cTime)) - intval(date("Ymd",$sTime));
    $dYear = intval(date("Y",$cTime)) - intval(date("Y",$sTime));
    //normal：n秒前，n分钟前，n小时前，日期
    if($type=='normal') {
        if( $dTime < 60 ) {
            return $dTime."秒前";
        }elseif( $dTime < 3600 ) {
            return intval($dTime/60)."分钟前";
        }elseif( $dTime >= 3600 && $dDay == 0  ) {
            return intval($dTime/3600)."小时前";
        }elseif($dYear==0) {
            return date("m-d H:i",$sTime);
        }else {
            return date("y-m-d H:i",$sTime);
        }
    //full: Y-m-d , H:i:s
    }elseif($type=='full') {
        return date("y-m-d H:i",$sTime);
    }elseif($type=='month') {
        return date("m-d H:i",$sTime);
    }else {
        if( $dTime < 60 ) {
            return $dTime."秒前";
        }elseif( $dTime < 3600 ) {
            return intval($dTime/60)."分钟前";
        }elseif( $dTime >= 3600 && $dDay == 0  ) {
            return intval($dTime/3600)."小时前";
        }elseif($dYear==0) {
            return date("y-m-d H:i",$sTime);
        }else {
            return date("y-m-d H:i",$sTime);
        }
    }
}

function addons($name,$data,&$res){
    $list = S('hooks');$list= $list[$name];
    foreach($list as $key =>$value){
        	
            $f = explode('.',$value);
            if(file_exists('App/'.$f[0].'/Lib/Hooks/'.$f[1].'Hooks.class.php')){
                include_once('App/'.$f[0].'/Lib/Hooks/'.$f[1].'Hooks.class.php');
                $s = $f[1].'Hooks';
   
                $a = new $s;
                
                $d = $a->$f[2]($data,$res);
            }

    }
    
}

//姓名
function getName($uid){
    $info = model("Member")->getUserInfo($uid);
    return $info[name];
}

//用户名
function getUserName($uid){
    $info = model("Member")->getUserInfo($uid);
    return $info[username];
}
//部门
function getUserbm($jid){
    
    
    static $jgs =array();
    
    !$jgs and $jgs =F('company_jiegou');
    
    if(!$jid){
        global $_OA; 
        return $jgs[$_OA[user][jid]][name];          
    }
    
    return $jgs[$jid][name];
    
}

//职位
function getUserzw($zid){
    
    static $zws =array();
    
    !$zws and $zws =F('company_zhiwei');
    
    if(!$zid){
        global $_OA;
        return $zws[$_OA[user][zid]][name];       
    }
    
    return $zws[$zid][name];
    
}


//获取公司头像,名字  效率低，建议优化

function getCompanyImage($cid){
    $info = model("Company")->getCompanyInfo($cid);
    return $info[image];
}
function getCompanyName($cid){
    $info = model("Company")->getCompanyInfo($cid);
    return $info[name];
}

function filter_text($text, $badstring){
    $siteInfo = model('Xdata')->lget('site');
    if($badstring == 'c'){
        $filter = S('site_ljgjz');
    }else{
        $badstring = $siteInfo['usergzj'];
        $filter = explode('|', $badstring);
    }

 foreach ($filter as $key) {
 if(strpos($text, $key) !== false){
 return $key;
 }
 }
 return false;
}

//将数据写入文件(php 语法

function fileWrite($file,$dir,$data,$isphp=1){

    $dfile = $dir.'/'.$file;
    
	!is_dir($dir)?mkdir($dir,0777):'';
	if(is_file($dfile)) unlink($dfile);
	if($isphp == 1){
		$data = "<?php\nreturn ".var_export($data,true).";";
	}
	
	file_put_contents($dfile,$data);
	
	return true;
}

/*
 *读取文件 
 *$dfile 文件
 */
function fileRead($dfile){
	
		if(is_file($dfile)) return include $dfile;
	
}

// linux时间戳函数
// return  返回当前时间戳
function linuxtime(){
    //linux 时间戳
        $time=date("Y-m-d H:i:s",time());
        $now=strtotime($time);
        return $now;
}

//递归创建目录
function createFolders($path){  
	//递归创建  
	if (!file_exists($path)){  
	   
		createFolders(dirname($path));//取得最后一个文件夹的全路径返回开始的地方  
		mkdir($path, 0777);  
	}  
}


//针对app各个的插件部分，修改自Emlog
/**
* 该函数在插件中调用,挂载插件函数到预留的钩子上
*
* @param string $hook
* @param string $actionFunc
* @param string $access 权限,如'Home:Index:index',则只对首页起作用
* @return boolearn
*/
function addAction($hook, $actionFunc, $access=''){
	global $tsHooks;
	if (!@in_array($actionFunc, $tsHooks[$hook])){
		$tsHooks[$hook][] = array('fun'=>$actionFunc,'access'=>$access);
	}

	return true;
}

/**
* 执行挂在钩子上的函数,支持多参数 eg:doAction('post_comment', $author, $email, $url, $comment);
*
* @param string $hook
*/
function doAction($hook){
	global $tsHooks;
    
	$args = array_slice(func_get_args(), 1);
	if (isset($tsHooks[$hook])){
   
        $plugins =model('Xdata')->get("plugin:list");         
        foreach ($tsHooks[$hook] as $v){   
            if($v['access']){        //验证权限
                $aArr =explode(':',$v['access']);
                
                if($aArr[0] && $aArr[0] !=APP_NAME )continue; 
                if($aArr[1] && $aArr[1]!=MODULE_NAME)continue;
                if($aArr[2] && $aArr[2]!=ACTION_NAME)continue;       
                
            }   
           if( function_exists( $v['fun'] ) ){          //只有开启的插件 才会加载对应index.php 文件
                call_user_func_array($v['fun'], $args); 
           } 
	       
	   }
	}
}

//取出二维数组中的一个字段,组成新的一维数组 cover:是否清除重复
function array2_field_array($array,$field='id',$cover=true){
    
    if(!is_array($array))return;
    
    $resArray =array();
    foreach($array as $v){
        if(!$cover)
            $resArray[] =$v[$field];
        else{
            if(in_array($v[$field],$resArray))
                continue;  
            else
                $resArray[] =$v[$field];      
        }   
    }
    return $resArray;
        
}

//二维数据根据字段生成新的关联数组($field 值唯一)
function keyArray2($array,$field='id'){
    if(!is_array($array))return;  
    
    $resArray =array();
    foreach($array as $v){
        $resArray[$v[$field]] =$v;        
    }
    
    return $resArray;
          
}

/**
  * 二维数组 根据某个字段排序
  * @param $arr 目标数组
  * @param $key 要排序的字段
  * @param $soft 默认为顺序
  */ 
function softArray2($arr,$key,$soft='asc'){
    
    $cacheArray =$resArray =array();
    
    foreach($arr as $k => $v){
        $cacheArray[$k] =$v[$key];    
    }
    $sMethod =$soft=='asc'?'asort':'arsort'; 
    $sMethod($cacheArray);
    
    foreach($cacheArray as $k => $v){
        $resArray[$k] =$arr[$k];        
    }
    
    return $resArray;    
}

//去除数组中 空值 或空字符串值
function clearArray($arr,$clearIdx =true){
    if(!$arr)
        return;
    $resArr =array();
    foreach($arr as $k => $v){
        $v =h($v);
        if($v=='' || $v === false)
            continue;
        
        if($clearIdx)   //是否重新排序
            $resArr[] =$v;     
        else 
            $resArr[$k] =$v;
    }
    
    return $resArr;    
}

/**
 * 获取应用 根据应用范围类别  
 * 
 * @author guop
 * 
 * @deprecated 2014/12/03 调用太复杂 要封装 S('appListInfo')缓存 请使用 公共模型 App 对应的方法
 * 
 */    
function getApp($key='use',$val='c'){
    static $apps =array();
    
    if(!$apps)
        $apps =S('appListInfo');
    
    if(!$key)
        return $apps;
     
    $resArr =array();   
    
    foreach($apps as $v){
            
        if( !$v[$key] || $v[$key]!=$val)continue;
        $resArr[$v['key']] =$v; 
           
    }
    
    return $resArr;    
}


/**
 * 应用详细信息(如果有 'field'，只返回相应的字段)
 * 
 * @author guop
 * 
 * @deprecated 2014/12/03 为了封装 S('appListInfo')缓存 请使用 公共模型 App->appInfo()
 * 
 */ 
function appInfo($appkey,$field){
    static $apps =array();
    if(!$apps)
        $apps =S('appListInfo');
    
    if(!$field)
        return $apps[$appkey];
    else
        return $apps[$appkey][$field];    
}

//获取 应用图标 80,32,16
function appIcon($key,$size){
    
    static $allAppInfos =array();
    if(!$allAppInfos)
        $allAppInfos =S('appListInfo');
    
    $thisApp =$allAppInfos[$key];
    
    $size =(int)$size;        
                
    $sizeArr =array(80,32,16);
    $size =in_array($size,$sizeArr) ? $size : $sizeArr[0];
    
    if(!$thisApp[is_exturl]){
    
        $file =APPS_PATH.$key."/icon_{$size}.png";
        
        if(!file_exists($file))
            $file ='Public/images/app.png';
                
        return $file;
    }else{
        $file ="Public/images/extApp/{$key}_{$size}.png";
        if(!file_exists($file))
            $file ='Public/images/app.png';
                
        return $file;                 
    }
}

//获取应用链接地址
function appLink($key){
    
    static $allAppInfos =array();
    if(!$allAppInfos)
        $allAppInfos =S('appListInfo');      
          
    $thisApp =$allAppInfos[$key]; 
    //print_r($thisApp);exit();
        
    if(!$thisApp[is_exturl]){
        return $thisApp['url'] ? $thisApp['url'] : url("{$key}:Index:index");    
    }
    else
        return $thisApp[url];   
}


/**
 * 发关消息
 * @param $data   array 消息内容(title,content,link)
 * @param $echo   int   是否直接输出
 * 
 */ 
function notify($data,$echo=1){
    
    if(!$echo)
        echo json_encode($data);
        
    $url =url('Home:Index:read_notify',"id={$data[id]}");
        
    $default =<<<EOT
                
                <div id="pop" style="display:none;">
                
                <style type="text/css">
                   *{margin:0;padding:0;}
                   #pop{background:#fff;width:260px;border:1px solid #e0e0e0;font-size:12px;position: fixed;right:10px;bottom:10px; box-shadow: 1px 1px 10px #333; }
	               #popHead{line-height:26px;background:#f6f0f3;border-bottom:1px solid #e0e0e0;position:relative;font-size:12px;padding:0 0 0 10px;margin-top:0px}
	               #popHead h2{font-size:14px;color:#666;line-height:26px;height:26px;margin: 0px;}
                   #popHead #popClose {position:absolute;right:10px;top:8px; display:block; width:8px; height:8px; background:url(Public/images/pop_close01.png) no-repeat;}
				   #popHead #popClose:hover{background:url(Public/images/pop_close02.png) no-repeat;}
	               #popHead a#popClose:hover{color:#f00;cursor:pointer;}
	               #popContent{padding:5px 10px;}
				   #popTitle{text-align:center}
	               #popTitle a{line-height:24px;font-size:14px;font-family:"Microsoft YaHei", "微软雅黑", "SimSun", "宋体" ,"sans-serif";text-decoration:none; color:#2F4F5E; }
	               #popTitle a:hover{color:#f60;}
	               #popIntro{text-indent:24px;line-height:160%;margin:5px 0;color:#48524A;}
	               #popMore{text-align:right;border-top:1px dotted #ccc;line-height:24px;margin:8px 0 0 0;}
	               #popMore a{color:#f60;}
	               #popMore a:hover{color:#f00;}
				   #popContent dl{ height:105px; overflow:hidden;}
	            </style>
                    
                    <div id="popHead">
	                   <a id="popClose" title="关闭"></a>
	                   <h2>温馨提示</h2>
	               </div>
	               <div id="popContent">
	               <dl>
		              <dt id="popTitle"><a href="http://www.03in.com" target="_blank">标题</a></dt>
                      <dd id="popIntro">内容</dd>
	               </dl>
	               <p id="popMore"><a href="http://www.03in.com" target="_blank">查看 »</a></p>
	               </div>
                    
                </div>
                <script>
                    var pop=new Pop("{$data[title]}","{$url}","{$data[content]}");
                </script>
EOT;
    
    switch($data['style']){
        case 'default':
            echo json_encode(array('data'=>$default));
            break;
        case 'gritter':
            $appicon =appIcon("$data[from]",32);
            echo json_encode(array('data'=>"<script>$.gritter.add({title:'{$data[title]} &nbsp;-<a style=\"font-weight:normal;color:#468847\" href=\"{$url}\">查看</a>',text:'{$data[content]}',image:'{$appicon}',sticky:false,time:300000});</script>"));
            break;
        default:
            echo json_encode(array('data'=>$data[title])); 
                        
    }
    
                      
}

//配合 上传文件控件 解析 上传附件数组变量 
function analysis_upload_widget($val,$split=false){
    if(!$val)
        return '';

    if(!$split)
        return serialize($val);
    else 
        return implode('#',$val);
    
}
//将存储的附件id 转换为id数组
function unanalysis_upload_widget($val, $split=false){
    if(!$val)   
        return '';
    
    if($split)
        return explode('#',$val);
        
    try{
        return unserialize($val);            
    }catch(Exception $e){
        return $val;    
    }   
}

/**
 * 组合计算(二维数组) 上限1000
 * $arr 格式如 Array ( [0] => Array ( [name] => 颜色 [value] => Array ( [0] => 红 [2] => 蓝 [3] => 黑 ) ) ) 
 */
function combination($arr){
    if(!$arr)
        return '';
    
    $relArr =array();            //关联名数组
    $max =1;    //最大值
    foreach($arr as $k => $v){
        $max *=count($v[value]);  
        $relArr[] =$v[name];       
    }
    if($max>1000)
        return 'More than 1000';
    
    $valArr =array();   //返回值(标题)
    //$idxArr =array();   //返回值(下标) 确保每个属性数组的标题不重复就可以用标题组进行判断
    $i =0;                      
	foreach($arr as $k => $v){
		
		if(!$i)
			$valArr =$v[value];
		else{
            $newUpArr =$v[value];   //要加上的循环数组
            
            $arr2 =$valArr;  // 将结果结果数组值保存为临时数组arr2 重置结果数组
			$valArr =array();
            
			foreach($arr2 as $v1){   //计算本次组合 返回组 结果数组
				foreach($newUpArr as $v2){
					$valArr[] =$v1.'*'.$v2;    
				}        
			}        
		}
		$i++;                          
	}
    
    return array($relArr,$valArr);        
} 
  
/**
 * 组合计算(二维数组) 上限1000
 * $arr 格式如 Array ( [0] => Array ( [name] => 颜色 [value] => Array ( [0] => 红 [2] => 蓝 [3] => 黑 ) ) )
 * 2015-1-20 修改链接的符号 为‘-’ 
 */
function combination2($arr){
    if(!$arr)
        return '';
    
    $relArr =array();            //关联名数组
    $max =1;    //最大值
    foreach($arr as $k => $v){
        $max *=count($v[value]);  
        $relArr[] =$v[name];       
    }
    if($max>1000)
        return 'More than 1000';
    
    $valArr =array();   //返回值(标题)
    //$idxArr =array();   //返回值(下标) 确保每个属性数组的标题不重复就可以用标题组进行判断
    $i =0;                      
    foreach($arr as $k => $v){
        
        if(!$i)
            $valArr =$v[value];
        else{
            $newUpArr =$v[value];   //要加上的循环数组
            
            $arr2 =$valArr;  // 将结果结果数组值保存为临时数组arr2 重置结果数组
            $valArr =array();
            
            foreach($arr2 as $v1){   //计算本次组合 返回组 结果数组
                foreach($newUpArr as $kk => $v2){
                    $valArr[] ='-'.$v1.'-'.$v2;    
                     
                }        
            }        
        }
        $i++;                          
    }
    
    return array($relArr,$valArr);        
} 

//原料种类调用  id
function yuanliaoCate($id){
    if($id){
        return M('YuanliaoCate')->where(array('id'=>$id))->getField('cate_name');
    }else{
        return "";
    }    
}

//原料分类调用  id
function yuanliaoClass($id){
    if($id){
        return M('YuanliaoClass')->where(array('id'=>$id))->getField('name');
    }else{
        return "";
    }    
}
//产品型号
function xinhao($id){
    return M('YuanliaoContent')->where(array('id'=>$id))->getField('name');
}
// 单位调用
function danwei($id){
    return M('YuanliaoCate')->where(array('id'=>$id))->getField('danwei');
}
//计算原料库存总算 $id 产品种类id

function count_cat($id){
    $D_content=M('YuanliaoContent');
    $where['cat_id']=$id;
   
    return  $D_content->where($where)->sum('num');
}
//如果为负数 转换为正数

function notf($id=0){
   $id=intval($id);
    if($id<0){
        return 0;
    }else{
        return $id;
    }
}

//产品id  获取名称
function proIdToName($pro_id){
    return M('ProduceProlist')->where(array('pro_id'=>$pro_id))->getField('name');
}
//产品型号  获取名称
function proIdToXinhao($xinhao){
   // return M('ProduceProlist')->where(array('pro_xinhao_id'=>$xinhao))->getField('xinhao');
  return model('StoreProduct')->get_comb_name($xinhao);
}
//改型号产品生产结果 包括多家生产的
function jgpro($d_id,$xinhao_id){
    $d_pqlist=M('ProducePqlist');
    $where['d_id']=$d_id;
    $where['xinhao_id']=$xinhao_id;
    $where['num_ci']=M('ProduceProlist')->where(array('d_id'=>$d_id))->Max('num');
    $list['xinhao_name']=proIdToXinhao($xinhao_id);
    $list['xinhao']=$xinhao_id;
    $list['num']=$d_pqlist->where($where)->sum('num');//理论生产数
    $list['relly_num']=$d_pqlist->where($where)->sum('relly_num');//实际生产数

    return $list;

}
//产品对应的型号
function cpxh($d_id,$pro_id){
    $d_pqlist=M('ProducePqlist');
    $where['d_id']=$d_id;
    $where['pro_id']=$pro_id;
    $where['num_ci']=$d_pqlist->where(array('d_id'=>$d_id))->max('num_ci');
    $jg=$d_pqlist->where($where)->field('xinhao_id')->select();
    foreach ($jg as $key => $value) {
        $dd[]=$value['xinhao_id'];
    }
    return array_unique($dd);
}

/*
*权限判定函数
*/
function access_r($uid,$app,$m,$a){
//global $_APP;
    

     $nodes=include("./App/".$app."/node.php");

    $thisNode =$app.'.'.$m.'.'.$a;
    //dump($thisNode);
    foreach($nodes as $key=>$value){
               // dump($value['nodes']);
          // dump($value['nodes']);
                if(in_array($thisNode,$value['nodes'])){
                    $no = array('key'=>$key,'name'=>$value['name'],'nodeType'=>$value['nodeType']);
                }
            }
           // dump($no);
           // exit;
    if(!is_array($no)){return true;}//没有这个节点跳出    
   //检查是否是管理员
   
    if(M('member')->where(array('uid'=>$uid))->getField('uid')==cookie('r_uid')){return true;}
    $userInfo = M('member')->where(array('uid'=>$uid))->find();
    
   // if($userInfo['cid'] =='' || $userInfo['cid'] ==0){return false;}
   // $cinfo = M('company')->where(array('cid'=>$userInfo[cid]))->find();
   // if($cinfo['uid'] == $uid){return true;}
   
   //检查是否分配权限
    $where['uid']    = $uid;
    $where['zid']    = $userInfo['zid'];
    $where['jid']    = $userInfo['jid'];                
    $where['_logic'] = 'or';
    $map['_complex'] = $where;
   //$map['cid']      = $userInfo[cid];
    $map['key']      = $no['key'];
                         
    if(is_array(M('access')->where($map)->find())){return true;}//有赋予权限跳出    

   return false;
}

//输出友好的json化的汉字  (只支持utf-8编码字符串) 
function jsonCode(&$arr){
	
	foreach($arr as $k => $v){
		
		if(is_array($v)){
			jsonCode($arr[$k]);	
		}else{
			
			$arr[$k] =urlencode($v);	
			
		}
	}
	
	return urldecode(json_encode($arr));	
}

//获取 根据公司id 获取 03in公司名称
function get_03in_companyinfo($cid,$field ='*'){
    
    $cache =F('companyFriend');

    if(! $info = $cache[$cid]){
        $info =SnsApi::cApi('Company/info',array('cid'=>$cid));        
        if(!$info)
            return false;
        
        $info =json_decode($info,true);
    }
    
    return $field =='*' ? $info : $info[$field];
    
                   
}

//判断应用 是否满足依赖关系
function app_relyon($name){
    
    $relyinfo =appInfo($name,'relyon');
    
    if(!$relyinfo)
        return true;
    $relyinfo =explode(',', $relyinfo);
    
    $applist =S('applist');
    
    foreach($relyinfo as $v){
        
        if(!in_array($v, $applist))    
            return false;
    }
    
    return true;
    
            
}

//应用是关闭(false) 还是开启(true)
function bool_app_open($key){
    
    static $bool_opens =array();
    if(!$bool_opens)
        $bool_opens =model('Xdata')->get('app:close');
    
    return $bool_opens[$key] ? false : true;
         
    
}

//获取当前登录人id 模型自动完成 作创建人赋值使用
function get_userid(){
    ///return cookie('uid');    
    return model('Member')->getLoginUid( ); 
}

/**
 * 导航组装 
 * 二种模式 : 1二维数组,链接信息由其中的数组组成,第一个元素为链接名,第二个元素为链接地址; 2一维数组,链接信息由字符串组成,由分隔符隔开,分隔符默认为#号
 */ 
//导航组装 $array 二维数组,元素中第一个参数为导航名,第二个为链接地址,如果元素中没有链接,则a=javascript:
function nav_string($array,$split ='#'){
    $str ='';
    if(!is_array($array))
        return "<a href='javascript:'>{$array}</a>";
        
    foreach($array as $v){
        
        if(!$v)
            continue;
        
        if(! is_array($v))
            $v =explode($split, $v);
              
        
        $link =$v[1] ? $v[1] : 'javascript:';
        
        
        $str .="<a href='{$link}' >{$v[0]}</a>";
    }
    
    return $str;        
}

/**
 * 将具体天的时间字符 转换成  中文时间
 * @param string $day 格式 2012-12-22 或时间戳
 * @return string
 */
function chineseDay( $day ){
	if( !preg_match( '/^\d{4}-\d{1,2}-\d{1,2}$/' , $day ) ){
		$day = date( 'Y-m-d' ,$day );	
	}
	
	$array = array(
			date('Y-m-d' , strtotime( '+1 day' ) ) => '明天',
			date('Y-m-d' , strtotime( '+2 day' ) ) => '后天',
			date('Y-m-d') => '今天',
			date('Y-m-d' , strtotime( '-1 day' ) ) => '昨天',
			date('Y-m-d' , strtotime( '-2 day' ) ) => '前天'

	);
	 
	return !!$array[ $day ] ? $array[ $day ] : $day;
}
 

//用于打印 有格式的数组
function print_rr($array){
    
    echo "<pre>";
    print_r($array);
    exit();
}


/**
* 删除目录以及目录下所有的文件
* @param $dir 目录路径
*/
  function deldir($dir) {
  //先删除目录下的文件：
  $dh=opendir($dir);
  while ($file=readdir($dh)) {
    if($file!="." && $file!="..") {
      $fullpath=$dir."/".$file;
      if(!is_dir($fullpath)) {
          unlink($fullpath);
      } else {
          deldir($fullpath);
      }
    }
  }
 
  closedir($dh);
  //删除当前文件夹：
  if(rmdir($dir)) {
    return true;
  } else {
    return false;
  }
}


/**
*@access 汉字转换为拼音简写函数
*@param $string
*/
function ToPinyinFist($string){
  Vendor('ChinessToE.PinYin');
  return  zh2py::conv($string);//Chinese ZHRMGHG
 // $py->getFirstPY($string);  
}

/**
 * 获取指定月份的第一天开始和最后一天结束的时间戳
 *
 * @param int $y 年份 $m 月份
 * @return array(本月开始时间，本月结束时间)
 */
function mFristAndLast($y="",$m=""){
 if($y=="") $y=date("Y");
 if($m=="") $m=date("m");
 $m=sprintf("%02d",intval($m));
 $y=str_pad(intval($y),4,"0",STR_PAD_RIGHT);
 
 $m>12||$m<1?$m=1:$m=$m;
 $firstday=strtotime($y.$m."01000000");
 $firstdaystr=date("Y-m-01",$firstday);
 $lastday = strtotime(date('Y-m-d 23:59:59', strtotime("$firstdaystr +1 month -1 day")));
 return array("firstday"=>$firstday,"lastday"=>$lastday);
}






```
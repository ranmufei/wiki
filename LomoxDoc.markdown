# Lomox 文档

> lomox 是指私有盘软件的那个界面程序 ，其功能是 可以用html制作软件界面

> *官网http://www.lomox.org/LomoX_Kernel_APIs.pdf* 


# 使用方法

> 1 引入 js ,建议下载 框架js /LxExt-1.0.dev.js 到自己项目中；

     	<script src="http://www.linksame.com/Public/js/js/jquery-1.7.2.min.js"></script>
    
        <script type="text/javascript" src="http://www.linksame.com/Public/js/LxExt-1.0.dev.js"></script> 

> **下载地址 http://www.linksame.com/Public/js/LxExt-1.0.dev.js**

### 调试环境 

> 调试只在lomox下看得到效果 请下载lomox项目

> 本地调试 网页资源放到 Resources/ 文件夹下

> 网络在线调试 请修改配置文件

```  python

[cfg]
url=http://baidu.com //网络调试地址 自定义  ，本地调试请删除此行
mainframe=0
maintop=0
title=邻商智能云管理系统
childframe=0
[maindialog]
hrefincurrent=0
[childdialog]
hrefincurrent=1

# lomox常用接口

``` javascript
 // 窗口初始化配置
var WindowSettings = {
	minWidth: 538,
	minHeight: 600,
	width:538,
	height: 600,
	center: true,
	debug: true
}


//基本功能
 $(function(){
	
	    //第二 如果报错不执行继续隐藏 			
	     LxExt.Dialog.dragRegion($('#MyTitle')); // 拖动元素 
	     //console.log(LomoX.setupJsAPIObject());
		     
		 LxExt.Dialog.setMinimumSize(WindowSettings.minWidth, WindowSettings.minHeight); //设置窗口大小
		 
		 //添加 最小化，关闭事件
		var _max = function() {
			if($("#lx-max").hasClass('lx-normal')) {
				$("#lx-max").removeClass('lx-normal');
				LxExt.Dialog.showNormal(); //显示最小化
			} else {
				$("#lx-max").addClass('lx-normal');
				LxExt.Dialog.showMaximized(); //显示最大化
			}
		}
		$("#lx-max").on('mouseup', _max);
		$('#MyTitle').dblclick(_max);
		$("#lx-min").on('mouseup', function(){
			LxExt.Dialog.showMinimized();
		});
		$("#lx-close").on('mouseup', function(){
			//提醒
					LxExt.Dialog.closeWnd(); //窗口关闭
		});
		 
	
	});  






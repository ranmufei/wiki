# avalon 组件开发 模板参考



```

/**
 * widget name  add product 
 * author ranmufei
 * date 2015 11 2
 * 
 */

define(
  ['avalon'
  , 'jquery'
  ,'text!./class.html'
  ,'layer/layer'   
  ,'apppublic/apppublic'
  ], function( avalon , $ , classTpm ,LAYER,apppublic){

  		var widget = avalon.ui.warehouse = function(element, data, vmodels) {

  			//element (组件元素), data（组件配置）, vmodels（自定义视图模型）
             var options = data.warehouseOptions//★★★取得配置项
             var id = data.warehouseId //组件ip
             var tmpls = classTpm.split('MS-TEMPLATE-SPLIT')
 			 var vmodel = avalon.define(avalon.mix( {
            		 $id : id,
            		 $init:function(){            		 	
            		 	avalon.log(options);
            		 	avalon.log('hello world this is a widget ,by creatclass with ranmufei');
            		 	avalon.scan( element , vmodels.concat(vmodel) )  
		                if( avalon.isFunction( vmodel.onInit )){
		                 var init= vmodel.onInit.call( element , vmodel , options, vmodels )
		                }  		               

		                $( element ).click( function( ){
			              vmodel.show( );     
			            })
            		 },
                               		
            		 show:function(){
            		   getClassData();
            		   $dialog=$(tmpls[0]).appendTo( $('body') ).hide();	
  			           avalon.log('dialog:',$dialog); 			          
  			           avalon.scan($dialog[0] , vmodel )  
  			           layer.open({
      						    type: 1,
      						    title:options.title,
      						    area: [options.width,options.height],
      						    //skin: 'layui-layer-demo', //样式类名
      						    // closeBtn: true, //不显示关闭按钮
      						    shift: 2,
      						    shadeClose: false, //开启遮罩关闭

      						    content:$dialog,
      						    cancel: function(index){ 
      						    	avalon.log('layer open close');
      						    	//$('#tree').remove();	
      						    }
						        }); 

            		 	//显示新开对话框 加载已有的分类树
            		 },
            		            		 
            		 add:function(data){
            		 	 var $dialogname=$(tmpls[1]).appendTo( $('body') ).hide();
            		 	 avalon.scan($dialogname[1] , vmodel )  
            		 	 //触发验证
            		 	//增加新的分类
            		 	layer.open({
            		 		type:1,
            		 		title:'增加一个仓库',
            		 		area:['320px','370px'],    
            		 		shade: false,        		 		
            		 		shift:2,
            		 		content:$dialogname,
            		 		btn: ['确定添加', '取消']
    						    ,yes: function(index, layero){ //或者使用btn1
    						       var statu=editClass(1);
    						       if(statu){						     				       	          
    						           avalon.scan(); 
                          
    						       }
    						       layer.close(index);
    						    },cancel: function(index){ //或者使用btn2
    						       vmodel.classname='';
    						    }
            		 	});
            		 },
            		 
            		 $remove:function(){
            		 	//system default remove methed
            		 	console.log('creatclas end remove  组件结束调用');
            		 },
            		 

            		},options)
             ) // end vmodel



			 return vmodel //必须返回组件VM	 
		}// end widget


	widget.defaults = {//默认配置项
        width:'550px', 
        height:'450px',
        title:'仓库管理',
        callbackfun:avalon.noop //回调函数Init
        /**
         * // 成功后 回调
                    if( typeof vmodel.callbackfun == 'function' ){
                      vmodel.callbackfun.call( element , vmodel , data  )    
                   }  
         */
        
    }
    
    return avalon



  })// end define



```
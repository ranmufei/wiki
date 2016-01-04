js:
require(["baiduMap/baiduMap"], function() { 
	var baiduMap;
	var vm=avalon.define({
		 $id:'uitest',
		 address:'',
		 $opt:{
		 	onInit: function(vm) {
			    baiduMap=vm;	
			},
			callbackfun:function(data){
				console.log('回调数据',data);
			    vm.address=data['address'];
			}
		 },
		 show:function(){
		 	baiduMap.show();
		 }   

	})

	avalon.scan();

});

html:
<layout name="layout" />
<script src="/App/Maintenance/static/js/map.js"></script>
<script type="text/javascript" src="http://api.map.baidu.com/api?v=2.0&ak=LCNhf8EbIO00dF8ZjgCnpCK5"></script>
<div ms-controller="uitest"> 
      <input  ms-duplex="address" ms-click="show"/><div ms-widget="baiduMap,test,$opt" style="display: inline"><i class="icon-search"></i></div>
</div>
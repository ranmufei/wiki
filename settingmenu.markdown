# 自定义右键

- 自己项目引入 
    
     > {:widget('SmartMenu')} 

```` php

<script>

var bodyMenuData = [[
{ text: "刷新",
  func:function(){
    window.location.reload();
  }
 },{
    text:'前进',
    func:function(){
        window.history.forward();
    }
 },{
    text:'后退',
    func:function(){
        window.history.back();
    }
 }
 ]];

$("#body_min_height").smartMenu(bodyMenuData, {
    name: "body"    
});
</script>

````
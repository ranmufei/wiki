实现页面展示的smartgrid表格元素导出，导出格式可以是excel和doc 
### 调用方式  
HTML中：`<div class="table_header_1 new_top_110 yp_table_1">
             <div ms-widget="smartgrid,$"></div>
        </div>` ,
define依赖define(['tableExport/tableExport'])  

| 配制参数 |  类型| 默认值 |  描述  |
| :-- | :-- | ----:| :--: |
|`consoleLog`|boolean|false|是否开启测试：输出导出数据 ,默认false|
|`tableName`|string|  |导出文件名，默认为"列表"。|
|`type`|string| 'excel'或者'doc' |导出文件类型，默认为excel。|

||||

举个例子：
导出按钮绑定的事件 function outExcul(){
                     var defaults = {
                              consoleLog:false,   // 是否开启测试：输出导出数据 ,默认false
		              tableName: '表名',   // 导出文件名，表名
                	      type: 'excel',   // excel、doc;导出文件类型 : 默认为excel() 
                          }
                      $(".yp_table_1").tableExport(defaults);    // "yp_table_1"是需要导出的表格的选择器，建议保证唯一性
                  }
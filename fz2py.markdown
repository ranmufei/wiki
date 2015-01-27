
# 汉字转拼音码

## 使用说明

   
   引入js文件  Public1/js/f2PY.js

   >> 函数 returnFist(str)  str为文字参数 

   >> 返回拼音码大写
   
## 举例

 >> 输入字段 id=txtChinese

 >> 拼音码字段 id=py

### html

````   html
   
   <label for="inputEmail" class="col-lg-2 control-label">仓库名称<span>*</span></label>
    <div class="col-lg-10">
    <input type="text" class="form-control" ms-duplex-string="newdata.storehouse" placeholder="仓库名称" id="txtChinese">
{{newdata.storehouse}}
        </div>
                        </div>
                          
   <div class="form-group">
   <label for="inputPassword" class="col-lg-2 control-label">拼音码</label>
    <div class="col-lg-10">
    <input type="text" class="form-control" ms-duplex-string="newdata.pym"  placeholder="拼音码"  id='py'>
                          </div>
                        </div>

````

### javascript  avalon 调取

```` javascript
 // 函数returnFist(str) 返回汉字拼音码 该函数在引入的的js文件中 一如文件直接调用即可
 //avalon 监听输入汉字转换拼音码 returnFist(a);

              vmodel.product.$watch("productName", function(a) {
                 vmodel.product.code=returnFist(a);
                
			  })

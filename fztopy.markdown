# 汉字转拼音模型（PHP）

## 模型 (PublicPinyinModel.class.php)

### - 转成带无声调的汉语拼音 model('PublicPinyin')->TransformWithoutTone($input_char,$delimiter='',$outside_ignore=true)
```` php
 /*
	* 转成带无声调的汉语拼音
	* param $input_char String  需要转换的汉字
	* param $delimiter  String   转换之后拼音之间分隔符
	* param $outside_ignore  Boolean     是否忽略非汉字内容
        * 案例  "小明"  转换后  "xiaoming" 
	*/	
````
### - 转成汉语拼音首字母 model('PublicPinyin')->TransformUcwords($input_char,$delimiter='')
```` php
/*
	* 转成汉语拼音首字母
	* param $input_char String  需要转换的汉字
	* param $delimiter  String   转换之后拼音之间分隔符
        * 案例  "小明"  转换后  "XM"
	*/	
````
### - 转成带有声调的汉语拼音 model('PublicPinyin')->TransformWithTone($input_char,$delimiter=' ',$outside_ignore=false)
```` php
/*
	* 转成带有声调的汉语拼音
	* param $input_char String  需要转换的汉字
	* param $delimiter  String   转换之后拼音之间分隔符
	* param $outside_ignore  Boolean     是否忽略非汉字内容
        * 案例  "小明"  转换后  "xiǎo míng"
	*/
````

## 测试地址：http://www.apps.com/index.php?app=Kaoqin&m=Index&a=test



# 备注
### 可以通过 model('Member')->get_pinyin("小玲");
```` php
* 返回  $data数组
* $data['spelling']全拼和$data['abbreviation']首字母，根据需要调用
````
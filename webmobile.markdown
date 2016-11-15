# 手机端引用Linksame接口列表

## 1. 手机端全部应用列表

**接口**: 
````php 
/index.php?app=Appstore&m=Api&a=mobileFilterApp ; 
````

**获取方式**： get;

*  @param cid  integer 必填 [公司cid]
*  @param type  string  可选 [应用类型]
*  @return array [data 应用列表， status 1成功 0失败]


## 2. 手机端个人的应用列表页

**接口**: 
````php 
/index.php?app=MobileUserApps&m=Api&a=list; 
````

**获取方式**： get;

* @param cid integer [公司cid]
* @param uid integer [用户uid]
* @return data array [列表]
* @return status integer [状态 0失败 1成功]
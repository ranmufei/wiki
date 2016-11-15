# 手机端引用Linksame接口列表

## 1. 手机端全部应用列表

   **接口**: 
````php 
/index.php?app=Appstore&m=Api&a=mobileFilterApp ; 
````

   获取方式： get;

  *  @param cid  integer 必填 [公司cid]
  *  @param type  string  可选 [应用类型]
  *  @return array [data 应用列表， status 1成功 0失败]
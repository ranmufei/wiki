## 富文本编辑器资源转换（PHP）

### 模型 (FilterTextModel.class.php)

#### 说明：
#### 1.采用正则非贪婪匹配，最小化索引的原子性
#### 2.资源图片下载，采用curl的多并发模式，最大化多资源的下载响应速度
#### 3.进行重复 文本过滤 避免因业务问题重复使用exec().

### - 使用方法很简单

```php

$newTextHTML = model("FilterText")->exec( $textHTML );

```

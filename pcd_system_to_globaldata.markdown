##系统设置的全局数据调用
### 如上传附件的一些设置、默认分页参数等，调用按形式分前端和后端。
### 后端调用：model('StaticData')->getInfo()
### 前端调用：模块 globalinfo/globalinfo


#### 前后端数据格式相同
|字段  |类型  |说明  |
|--------|--------|------- |
|page  | array|分页|
|attach   | array| 附件|
### GraphQL 
使用composer默认的集成方式，组件位于根目录的composer组件文件夹里，只需要导入"`./vendor/autoload.php`"自动加载文件，就可以使用GraphQL组件生成新的API。

### 应用定义类型文件
在GraphQL中自定义类型应该使用命名空间前缀`GraphQL\App\` + 应用名 + `\自己的目录结构结构`。

### 公共的类型
目前定义了一些公共的类型文件，位于`Addons\GraphQL`目录，对应的命名空间前缀`GraphQL\Project\`。类型命名空间为`GraphQL\Project\Type`，公共的GraphQL文件目录如下：

* Addons\GraphQL\
 * SysTypes.php `(公共类型注册表，可以用此注册表类直接引用`user`(员工) , `post`(职位) , `dept`(部门) 等类型 )`
 * Type <small>(目录中存放的是所有公共类型)</small>
     * UserType.php
     * PostType.php
     * …


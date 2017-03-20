### GraphQL 
使用composer默认的集成方式，组件位于根目录的composer组件文件夹里，只需要导入"`./vendor/autoload.php`"自动加载文件，就可以使用GraphQL组件生成新的API。

### 应用定义类型文件
在GraphQL中自定义类型应该使用命名空间前缀`GraphQL\App\` + 应用名 + `\自己的目录结构结构`。

### 公共的类型
目前定义了一些公共的类型文件，位于`Addons\GraphQL`目录，对应的命名空间前缀`GraphQL\Project\`。类型命名空间为`GraphQL\Project\Type`，公共的GraphQL文件目录如下：

* Addons\GraphQL\
 * SysTypes.php
 * Type <small>(目录中存放的是所有公共类型)</small>
     * UserType.php
     * PostType.php
     * …
 * Data
     * DataSource.php
 * Vo
     * User.php
     * Post.php
     * …

SysTypes.php是公共类型的注册表类，建议从这里使用公共类型（`SysTypes::user()、SysTypes::post()…`）,同时也对系统的标量类型进行了封装（`SysTypes::id()、SysTypes::string()…`）。

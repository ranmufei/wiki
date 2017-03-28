### GraphQL 
使用composer默认的集成方式，组件位于根目录的composer组件文件夹里，只需要导入"`./vendor/autoload.php`"自动加载文件，就可以使用GraphQL组件生成新的API。

### 写法示例
获取员工信息的接口，可以在`GraphIQL Feen`看到效果

`http://www.apps.com/index.php?app=Home&m=Organ`

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

SysTypes.php ：是公共类型的注册表类，建议从这里使用公共类型（`SysTypes::user()、SysTypes::post()…`）,同时也对系统的标量类型进行了封装（`SysTypes::id()、SysTypes::string()…`）。

Data\DataSource.php ：提供了对公共类型数据的查询，并且封装成对了对应 `Vo` 对象，如查询指定 `id` 的用户信息，如果用户自己对公共类型提供数据，则必须转换成对应的 `Vo` 对象。

Vo\User.php… ：为了统一规范化对类型的赋值，如果是自己对类型提供的数据需要转换成对应的 `Vo`类型。 

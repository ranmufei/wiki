## 进销存 商品选择控件 说明

- ### 调用方法
 
> 在模板中调用

```` html
 {:widget('ChoiceProduct')}
 
```` 
- ### 回调 

> 在网页中回用getSelectProduct(data){} 处理选中商品

> data 参数 为返回选择商品的对象 object



``` javascript

// 请在该函数过程中写 自己业务过程

   getSelectProduct(data){

    }

  data 数据格式参考

[
{ Object$id: "smartgridTr3"cat_id: "74"class_id: "30"code: "TLS5"format: "黄色*90L*13"id: "5"name: "塔拉斯5"selected: truestornNum: null}
,{ Object$id: "smartgridTr4"cat_id: "74"class_id: "30"code: "TLS5"format: "黄色*90L*15"id: "6"name: "塔拉斯5"selected: truestornNum: null
}
]


   
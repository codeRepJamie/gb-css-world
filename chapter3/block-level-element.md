#块级元素

** 重点** 块级元素特征：一个水平流上只能单独显示一个元素，多个块级元素则换行

##块级元素和dispaly:block不是一个概念
常见块级元素有：`<div>`、`<li>`、`<table>`,该元素默认的display值分别为 blcok,list-item,table,但是他们均为“块级元素”，因都符合块级元素特征，即“一个水平流上只能单独显示一个元素”

##块级元素常用特性
因为块级元素有换行特征，因此理论上配合clear属性来清除浮动带来的影响
```css
.clear::after{
    content: '';
    display: table; // 也可以block或者list-item
    clear:both;
}
```
#术语

```css
/* 例子 */
.foo{
    height:99px;
    color:transparent;
    background: url('src/cover.jpg');
    border: 1px solid rgba(0,0,0,.5)
}
```

##属性名
对css样式称谓，例如height和color

##值
“99px”就是典型值，值有下面几个类型：
1.  整数值：z-index:1 属于`<integer>`或`<number>`
1.  数值：line-height:1.5 属于`<number>`
1.  百分比：50% 属于`<precent>`
1.  长度：99px
1.  颜色值：#333

##关键字
特指css特殊的关键字，如 `transparent`、`solid`、`inherit`
其中`inherit`是所有css属性都可使用的泛关键字

##变量
css `currentColor` 就是变量

##单位
1. 时间单位 `s`、`ms`
1. 角度单位 `deg`、`rad`
1. 长度单位 `px`、`em`, 细分：相对字体长度单位(em,ex,rem) 相对视区长度单位(vh,vw)/绝对长度单位(px,pt,cm,mm)
1. `<number>+长度单位=<length>`
注：2% 不是长度单位，是一个完整值

##功能符
值以函数形式表示`background: url('src/cover.jpg')`
1. 颜色(rgba,hsla)
1. 图片地址(url)
1. 元素属性值，计算,过渡效果(calc(100%-80px),translate(0,25),scale(-1))

##属性值
冒号后面所有内容，如`1px solid rgba(0,0,0,.5)`

##声明
属性名+属性值，如`border: 1px solid rgba(0,0,0,.5)`

##声明块
花括号内容，如：
```css
{
    height:99px;
    color:transparent;
    background: url(src/cover.jpg);
    border: 1px solid rgba(0,0,0,.5)
}
```
##选择器
描述目标元素
1. 类选择器：‘.’开头，对应html的class属性
1. id选择器：‘#’开头，对应html的id属性，可以渲染多个相同id的元素
1. 属性选择器：含有‘[]’，对应含有该属性的html元素
1. 伪类：含有‘:’选择器，如:first-child
1. 伪元素：含有‘::’选择器，如::brefore,对应html的隐藏元素

##关系选择器
1.  后代选择器" "(空格)：所有合符规则的后代元素
1.  相邻后代选择器">"：仅合符规则的子元素
1.  兄弟选择器"~"：仅合符规则的且在元素之后出现的兄弟元素
1.  相邻兄弟选择器"+"：仅合符规则的所有兄弟元素

##规则或规则集
选择器+声明块内容，如：
```css
.foo{
    height:99px;
    color:transparent;
    background: url(src/cover.jpg);
    border: 1px solid rgba(0,0,0,.5)
}
```

##规则
以@字符开始的一些规则，如`@media`,`@font-face`

#未定义行为
当出现Web定义标准规范描述以外的场景，各大厂商根据自己理解与喜好实现的行为，即出现“浏览器兼容问题”，专业的术语应是“未定义行为”
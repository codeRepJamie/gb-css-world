#内容盒子概念
由于出现了inline-block盒子模型，在css2.1中定义了：
一个block元素，实际是由一个外在的“块级盒子”和内在的“块级容器盒子”组成。
一个inline-block元素，实际是由一个外在“内联盒子”和内在的“块级容器盒子”组成
一个inline元素，则是内外都是“内联盒子”

##元素内的附加盒子概念
*   css属性为display:list-item的元素，实际包含一个叫“标记盒子”（marker box），专门放原点、数字这些项目符号，外面才是一个block-level盒子
*   css属性为display:inline-box的元素，实际包含一个“容器盒子”是一个block-level盒子，外面是一个inline-level的盒子
*   css属性为display:table的元素，实际包含一个“容器盒子”是一个table布局的盒子，外面是一个block-level的盒子
*   css属性为display:inline-table的元素，实际包含一个“容器盒子”是一个table布局的盒子，外面是一个inline-level的盒子
*   css属性为display:inline的元素，实际包含一个内外均是inline-level盒子
*   css属性为display:block的元素，实际包含一个内外均是block-level盒子
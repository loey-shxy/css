## CSS 关键字
### initial
默认值
### inherit
继承
#### 可继承的属性
- 所有元素可继承：visibility, cursor
- 内联元素可继承：letter-spacing, word-spacing, white-space, line-height, color, font, font-family, font-size, font-style, font-variant, font-weight, text-decoration, text-transform, direction
- 块状元素可继承：text-indent, text-align
- 列表元素可继承：list-style, list-style-type, list-style-position, list-style-image
- 表格元素可继承：border-collapse
### unset
不设置，是`initial`和`inherit`的组合
- 如果该属性是默认继承属性，等同于`inherit`
- 如果该属性是非继承，等同于`initial`
### revert
与`unset`非常类似，大部分情况下，作用是一模一样的，唯一的区别：
- revert：属性应用了该值之后，将还原到具有由浏览器或用户创建的自定义样式表（在浏览器侧设置）设置的值
- unset：属性应用了该值后，样式将完全被还原

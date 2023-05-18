## 盒子模型与背景的关系
`background` 在盒子模型中，是布满整个元素的盒子区域的，并不是从 `padding` 内部开始（也就是说是从 `border` 开始的）。

## 改变背景填充规则 `background-clip` 
设置元素的背景图片/背景颜色是否延伸到边框下面。
```
background-clip: border-box; /* 背景延伸到边框外沿（但是在边框之下） */
background-clip: padding-box; /* 边框下面没有背景，即背景眼神到内边距外沿 */
background-clip: content-box; /* 背景裁剪到内容区外沿 */
```

## background image 绘图区域
1. background positioning area: `background-origin` 属性决定了这个**相对定位位置**，默认为`padding-box`。 因此默认的背景图片是从 padding box 的左上顶点开始的。
2. background painting area: `background-clip` 属性决定了**绘制区间**，默认为`border-box`。因此在`background-repeat: repeat`（default）的情况下：*The image is repeated in this direction as often as needed to cover the background painting area*


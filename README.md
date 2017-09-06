# CSS 常见布局方式

------

>  1. flex   一维布局
>  2. grid   二维布局



flex布局：

>弹性布局
>
>水平的主轴（main axis）和垂直的交叉轴（cross axis）
>
>属性:
>flex-direction：主轴的方向。
> flex-wrap：超出父容器子容器的排列样式。
> flex-flow：flex-direction 属性和 flex-wrap属性的简写形式。
> justify-content：子容器在主轴的排列方向。
> align-items：子容器在交叉轴的排列方向。
> align-content：多根轴线的对齐方式。
>
> 子容器属性：
> order：子容器的排列顺序    数值越小，排列越靠前，默认为 0。
> flex-grow：子容器剩余空间的拉伸比例
> flex-shrink：子容器超出空间的压缩比例
> flex-basis：子容器在不伸缩情况下的原始尺寸   定义了子容器在不伸缩情况下的原始尺寸，主轴为横向时代表宽度，主轴为纵向时代表高度。
> align-self：允许单个项目有与其他项目不一样的对齐方式。



grid布局：

> css fr
> 单位是一个自适应单位，fr单位被用于在一系列长度值中分配剩余空间，如果多个已指定了多个部分，则剩下的空间根据各自的数字按比例分配。
>
> minmax()
> 函数来创建行或列的最小或最大尺寸，第一个参数定义网格轨道的最小值，第二个参数定义网格轨道的最大值。可以接受任何长度值，也接受 auto值。auto 值允许网格轨道基于内容的尺寸拉伸或挤压。
>
> repeat()
> 函数可以创建重复的网格轨道。这个适用于创建相等尺寸的网格项目和多个网格项目。 repeat()
> 也接受两个参数：第一个参数定义网格轨道应该重复的次数，第二个参数定义每个轨道的尺寸。
>
> grid-column-gap：创建列与列之间的距离。
> grid-row-gap：行与行之间的距离。
> grid-gap 是 grid-row-gap 和 grid-column-gap两个属性的缩写。
>
> grid-row 是 grid-row-start 和 grid-row-end 的简写。
> grid-column 是grid-column-start 和 grid-column-end 的简写。
>
> 这四个值可以用
> grid-area缩写，分别对应grid-row-start、grid-column-start、grid-row-end、grid-column-end：
> grid-area: 2 / 2 / 3 / 3;
>
> grid-row: 2 / span 3;  grid-column: span 2; 也可以使用 grid-row 和
> grid-column 简写的形式，关键词 span 后面紧随数字，表示合并多少个列或行，/ 前面是从第几行/列开始。

[grid学习PPT][1]
注：本文主要是学习了“渔人码头”的“5分钟学会 CSS Grid布局“这篇文章，🔗：www.css88.com/archives/8506

CSS Grid 布局由两个核心组成部分是 Wrapper (父元素) 和 items (子元素)。wrapper 是实际的 grid（网格），items 是 grid (网格) 内的内容。

1、创建一个 grid 布局
首先，我们开始写一个 wrapper 父元素，然后在 warpper 内容包含 6 个 items 元素：

![grid_1](https://github.com/virgil66/example/blob/master/example4/images/grid_1.png)

这里 wrapper 元素变为一个 grid (网格), 只要将 wrapper 的 display 属性设置为 grid 即可：

![grid_2](https://github.com/virgil66/example/blob/master/example4/images/grid_2.png)

至此，我们已经将 wrapper 元素变为一个 grid (网格)了，但是这里也只是简单的 div 盒子的叠加，没有其他的任何效果。

![grid_3](https://github.com/virgil66/example/blob/master/example4/images/grid_3.png)

2、grid 布局新增 rows (行) 和 columns (列)
为了让 grid 布局成为二维的网格容器，我们需要定义行和列。这里我们将创建2行和3列，我们将使用 grid-template-rows 和 grid-template-columns 属性：

![grid_4](https://github.com/virgil66/example/blob/master/example4/images/grid_4.png)

3、grid-column 和 grid-row
这里我们如果要定位和调整 items 子元素的大小和位置，我们将借助 grid-column 和 grid-row 属性。
首先我们将给每一个 items 子元素一个 class：

![grid_5](https://github.com/virgil66/example/blob/master/example4/images/grid_5.png)

比如我们现在要想让第一个 items 子元素独占一行：

![grid_6](https://github.com/virgil66/example/blob/master/example4/images/grid_6.png)

这里我们设置了 grid-column-start: 1 和 grid-column-end: 4，它们所表示的含义为：grid (网格) 从第1列网格线开始到第4列网格线结束。同理，grid-row
在这里，我们还可以对 grid-column-start: 1 和 grid-column-end: 4进行简写：

![grid_7](https://github.com/virgil66/example/blob/master/example4/images/grid_7.png)

最后，我们来给 items 子元素一个简单的布局：

![grid_8](https://github.com/virgil66/example/blob/master/example4/images/grid_8.png)

![grid_9](https://github.com/virgil66/example/blob/master/example4/images/grid_9.png)


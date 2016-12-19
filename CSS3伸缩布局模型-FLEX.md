# CSS3伸缩布局模型-FLEX

- display：flex|inline-flex

  > 当元素float||absolute时候，inline-flex会block化

- flex-direction

  - row
  - row-reverse
  - column
  - column-reverse

- flex-wrap

  - no-wrap
  - wrap
  - wrap reverse

- flex-flow:flex-direction||flex-wrap

- justify-content

  - flex-start
  - flex-end
  - center
  - space-between：平均隔开，两边不留白
  - space-around：平均隔开，两边留一半的空白

  > 用于伸缩容器，即伸缩项目的父元素，意思是主轴方向

- align-items

  - flex-start
  - flex-end
  - center
  - stretch：填充整个容器
  - baseline：根据基线对齐，基线是伸缩项目内容的底部，比如文字就是一行文字的底部就是基线

  > 用于伸缩容器，就是父元素

- align-self

  - start
  - end
  - center
  - baseline
  - stretch

  > 用于伸缩项目，就是容器里，单独的一项运用

- align-content

  - flex-start
  - flex-end
  - center
  - space-between
  - space-around
  - stetch：填充满

  > 这个与align-items的区别在于，这是是在伸缩行方向，整个一起走的

- flex

  - none
  - flex-grow
  - flex-shrink
  - flex-basis

  > flex-grow是伸缩容器中剩余空间分配
  >
  > flex-basis是伸缩项目的的基本大小
  >
  > flex：none==flex：0 0 auto
  >
  > flex：auto==flex：1 1 auto
  >
  > 用于伸缩项目

- order

  - number

  > 用于伸缩项目的顺序，在同一个父元素下，order可以比较；不同父元素下，order不可以比较。

---

**实战应用**

实现三列等高和页脚黏附效果


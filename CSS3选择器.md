# CSS3选择器

**分类**

- 基本选择器
- 层次选择器
- 伪类选择器
  - 动态伪类选择器
  - 目标伪类选择器
  - 语言伪类选择器
  - UI元素状态伪类选择器
  - 结构伪类选择器
  - 否定伪类选择器
- 伪元素
- 属性选择器

**基本选择器**

- *：通配选择器


- E：元素选择器


- id：ID选择器


- .class：类选择器


- select1，select2：群组选择器

**层次选择器** 

- E F：后代选择器

  >E的所有后代F，包括F的后代

- E>F：子选择器

  > E的直接子元素F

- E+F：相邻兄弟选择器

  > E后面的第一个兄弟F

- E~F：通用兄弟选择器

  > E后面所有兄弟F们

**伪元素**

- ：：first-letter

  > 第一个字母

- ：：first-line

  > 第一行文本

- ：：before

- ：：after

  > 在某元素前后，搭配content，可以应用样式，但是不属于文本流

- ：：selection

  > 被选择元素，只能应用background和color

**属性选择器**

- E[attr]

- E[attr=val]

- E[attr|=val]

  > attr=val或者以val开头的属性

- E[attr~=val]

  > attr中有多个属性，其中有val的那个

- E[attr*=val]

- E[attr^=val]

- E[attr$=val]

  *通配符*   

  - ^：起始符
  - $：结束符
  - *：任意符

**伪类选择器**

- 动态伪类

  - ：link

  - ：visit

  - ：hover

  - ：active

  - ：focus

    > love/hate原则去背

- 目标伪类

  - ：target

- 语言伪类

  - ：lang（lang）

- UI元素伪类

  - ：checked
  - ：enabled
  - ：disabled

- 结构伪类

  - ……

    > 功能强大，但实在太多

- 否定伪类

  - ：not




































# 媒体特性与Responsive设计

- Media Type类型

  - All
  - Handheld：手持
  - Print
  - Screen
  - Projection：投影
  - Speech：语音
  - Tv
  - Tty：固定密度字母栅格媒介，如电传打字机和终端
  - Braille：盲人触觉回馈设备
  - Embossed：盲文打字机

- 引用方法

  - link

  - xml

    > ```html
    > <?xml-stylesheet rel="stylesheet" media="screen" href="style.css" ?>
    > ```

  - @import

    > ```css
    > @import url(print.css) screen;
    > ```

  - @media

    > ```css
    > @media screen and (max-width:960px){
    >   //....
    > }
    > ```

- 媒体特性

  - max-width

  - min-width

  - device-width

  - not

    > ```css
    > @media not print and (max-width:960px){
    >   //
    > }
    > ```
    >
    > 对not后面的整个表达式取反，就是非打印设备且宽度小于960px

  - only

    >  隐藏样式表

- **Responsive布局**

  - 流体网格
  - 弹性图片
  - 媒体查询
  - 屏幕分辨率
  - 主要断点
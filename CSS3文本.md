# CSS3文本

- text-overflow

  - clip：裁剪

  - ellipsis：缩略

    > text-overflow单独应用是没有样式的，要结合
    >
    > - width
    > - white-space：nowrap 不换行
    > - overflow；hidden
    > - text-overflow：ellipsis


    > 单独应用只会把容器撑高而已

- word-wrap

  - normal

  - break-word

    > 实现长单词和URL自动换行

- word-break（针对一些亚非语言）

  - normal

  - break-all

    > 强行截断英文单词

  - keep-all

    > 保留整个英文单词和汉字，但会撑破容器

- white-space空白符

  - normal

  - pre

    >保留文本间的空白和换行符

  - nowrap

  - pre-line

    > 不保留文本间空白，但保留换行

  - pre-wrap

    > 保留文本间空白和换行

**技巧** 

```css
*{
  word-wrap:break-word;
  overflow:hidden;
}
//可以得到一个良好的文本效果
```




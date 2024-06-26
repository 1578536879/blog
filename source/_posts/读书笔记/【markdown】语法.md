---
title: 【markdown】语法
categories: 额外内容
tag: 额外内容
---


***、---、___可以显示横线效果

***
---
___

## 链接

除了最基本的[]()外，还包含以下

- 引用链接

[link]

[link]: htttps://

- 网址链接

<https://>

## 扩展语法GFM

- 删除线～

~~删除~~

- 下划线

<u>a</u>

- 上标

这是^上标^

- 下标

这是~下标~

- 表情

:smile:

[表情地址](https://www.webfx.com/tools/emoji-cheat-sheet/)

- 任务列表
- [ ] list 1

- [x] list2

- 锚点

[point](#point)

## 排版

### 空格

- 中英文之间、中英文与数字之间、英文标点符号与后面的文字之间

## 其他

### 语言转换工具

Pandoc

### vs code语法增强插件

markdown preview enhanced

#### 语法

- 引用文件

```
@import “文件名”
```

可以将文件内容直接显示，包括图片、csv表格

- 幻灯片

```
<!— slide—>
First
<!— slide—>
Second
```

* 使用库：reveal.js


## 交互性工具

交互性md工具可以直接执行代码

- jupyter notebook

- r markdown


### 锚点
其实呢，每一个标题都是一个锚点，和HTML的锚点（`#`）类似，比如我们

|语法|效果|
|---|---|
|`[回到顶部](#readme)`|[回到顶部](#readme)|

不过要注意，标题中的英文字母都被转化为**小写字母**了。
> 以前GitHub对中文支持的不好，所以中文标题不能正确识别为锚点，但是现在已经没问题啦！


### 复选框列表
- [x] 需求分析
- [x] 系统设计
- [x] 详细设计
- [ ] 编码
- [ ] 测试
- [ ] 交付

您可以使用这个功能来标注某个项目各项任务的完成情况。
> Tip:
>> 在GitHub的**issue**中使用该语法是可以实时点击复选框来勾选或解除勾选的，而无需修改issue原文。

## 块引用

### 常用于引用文本
#### 文本摘自《深入理解计算机系统》P27
　令人吃惊的是，在哪种字节顺序是合适的这个问题上，人们表现得非常情绪化。实际上术语“little endian”（小端）和“big endian”（大端）出自Jonathan Swift的《格利佛游记》一书，其中交战的两个派别无法就应该从哪一端打开一个半熟的鸡蛋达成一致。因此，争论沦为关于社会政治的争论。只要选择了一种规则并且始终如一的坚持，其实对于哪种字节排序的选择都是任意的。
> **“端”（endian）的起源**
以下是Jonathan Swift在1726年关于大小端之争历史的描述：
“……下面我要告诉你的是，Lilliput和Blefuscu这两大强国在过去36个月里一直在苦战。战争开始是由于以下的原因：我们大家都认为，吃鸡蛋前，原始的方法是打破鸡蛋较大的一端，可是当今的皇帝的祖父小时候吃鸡蛋，一次按古法打鸡蛋时碰巧将一个手指弄破了，因此他的父亲，当时的皇帝，就下了一道敕令，命令全体臣民吃鸡蛋时打破较小的一端，违令者重罚。”

### 块引用有多级结构
> 数据结构
>> 树
>>> 二叉树
>>>> 平衡二叉树
>>>>> 满二叉树



### 对齐
表格可以指定对齐方式

| 左对齐 | 居中 | 右对齐 |
| :------------ |:---------------:| -----:|
| col 3 is | some wordy text | $1600 |
| col 2 is | centered | $12 |
| zebra stripes | are neat | $1 |

表情
----------
Github的Markdown语法支持添加emoji表情，输入不同的符号码（两个冒号包围的字符）可以显示出不同的表情。

比如`:blush:`，可以显示:blush:。

具体每一个表情的符号码，可以查询GitHub的官方网页[http://www.emoji-cheat-sheet.com](http://www.emoji-cheat-sheet.com)。

但是这个网页每次都打开**奇慢**。。所以我整理到了本repo中，大家可以直接在此查看[emoji](./emoji.md)。

diff语法
---------
版本控制的系统中都少不了diff的功能，即展示一个文件内容的增加与删除。
GFM中可以显示的展示diff效果。使用绿色表示新增，红色表示删除。

其语法与代码高亮类似，只是在三个反引号后面写diff，
并且其内容中，以 `+ `开头表示新增，`- `开头表示删除。

效果如下：

```diff
+ 鸟宿池边树，僧敲月下门
- 鸟宿池边树，僧推月下门
```

## 为何需要本指南

我们经常需要书写教程、题解等。因而必须学习文本、公式编辑的技术。

由于绝大部分网页无法支持 word / pdf 格式的内容，而 html 过于繁杂，故需要使用本站及大部分网站所支持的带有 mathjax 公式插件的 markdown 格式。

## 一个编辑器

请在电脑端安装 typora 软件。

**第一次使用时，请单击工具栏“文件”->“偏好设置”，在 markdown 设置模块中勾选“内联公式”。**

## 您需要学习的

百度 markdown 和 $\LaTeX$ 。并在 typora 中利用前二者的格式编辑您的文本，保存为 .md 文件。

由于很多人抗拒百度，因此我不得不写下相关的教程。如果您已经熟知这些东西，请跳过即可。

!!! warning "注意"
    如果您懂得 markdown 和 LaTeX 的语法，请点击typora左下角第二个按钮，进入源代码模式，并直接键入您的 markdown 源码。

### markdown

0.换行

按两次空格Shift+回车是单行距换行，效果如下：

行1  
行2

按回车是双行距换行，效果如下：

行1

行2

需要注意的是，对于单行距换行，一定要在行最后加两个空格。

1.标题

在typora中输入以下内容：

```text
# 一级标题
## 二级
### 三级
#### 四级
##### 五级
###### 六级
```

显示效果：

（此处为一级标题，因为一级标题会影响渲染，故不显示，大家自行脑补）

## 二级
### 三级
#### 四级
##### 五级
###### 六级

需要注意：**绝对不允许在此 Wiki 中使用一级标题**！！！

2.引用

在typora中输入以下内容：

```text
> XXX
```

> XXX

这便是引用。需要注意，在typora中，按一次换行会出现这种效果：

> XXX
>
> 

这时，必须再按一次换行才能跳出引用区。

事实上，在typora输入：

```text
> xxx
xxx
233

233
```

效果如下：

> xxx
> xxx
> 233

233

3.插入图片、超链接

在typora中输入 `[XXX](某网址)` ,会显示为[XXX](某网址)，点进去就可以转到相应网址。

在typora中输入 `![这里面随便填](图片网址)` ，就能显示出这个图片。

需要注意的是，切不可在typora中直接粘贴图片，或者引用本地图片。必须使用**无水印图床**（例如[路过图床](https://imgchr.com/)）上传图片。这时候，网页上会出现一个图片。下面一堆链接不用管。然后用下面的方式获取这个图片的地址。

在浏览器中，右键某个网页的图片，选择“复制图片地址”即可。

4.其他格式

输入

```text
**233**  
~~233~~
```

**233**  
~~233~~

5.无序列表

在typora中输入如下内容：

```text
- XXX
YYYYYY  //行末有2个空格
YYYYYY
- XXX
    - YYY
    - YYY
    666  //行末2空格
- ee
```

- XXX
YYYYYY  
YYYYYY
- XXX
    - YYY
    - YYY
    666  //行末2空格
- ee

6.文本区

在typora中输入

```text
​```text
XXXXXXXX      //此时换行行末不需要有空格！
asd~~233~~
**233**
​```
```

效果：

```text
XXXXXXXX
asd~~233~~
**233**
```

事实上，你在文本框输入什么，显示出来就是什么。文本框里的内容不会经过markdown渲染。

在typora中，如果你编辑到了文本框的末尾，可以按Ctrl+回车跳出文本框。

对于行内嵌套的文本框，输入如下：

```text
这是行内文本框：`XXXXXXXXXXXXX`
```

显示为：

这是行内文本框：`XXXXXXXXXXXXX`

7.插入 LaTeX 公式

在typora中输入 `这是行内公式：$\sqrt2$` ，会显示为：

这是行内公式：$\sqrt2$

输入：

```text
//这里需要有空行
$$
\sqrt2   //这里写 LaTeX 代码
$$
//这里需要有空行
```

效果：
$$
\sqrt2
$$

### $\LaTeX$

参考：https://www.luogu.com.cn/blog/IowaBattleship/latex-gong-shi-tai-quan

LaTeX 的格式规范：https://oi-wiki.org/intro/htc/#latex
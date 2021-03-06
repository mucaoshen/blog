# **Markdown的基本语法**
## **_斜体_**和**粗体**
```
*斜体*或_斜体_  
**粗体**
***加粗斜体***
~~删除线~~
```  
view  
*斜体*或_斜体_    
**粗体**  
***加粗斜体***  
~~删除线~~
## 分级标题
```markdown
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题

```
view  
不方便展示
## 超链接
Markdown 支持两种形式的链接语法：行内式和参考式两种形式，行内式一般
使用较多。
### 行内式
语法说明：  
[]里写链接文字，()里写链接地址，()中的""中可以为链接指定的title属性，
title属性可加可不加。title属性的效果是鼠标悬停在链接上会出现指定的
title文字。链接地址与链接标题前有一个空格。
```markdown
这里是[Jack Huang的github博客空间](https://mucaoshen.github.io/blog/)  
这里是[Jack Huang的github博客空间](https://mucaoshen.github.io/blog/, "Jack Huang的博客空间")
```
view  
这里是[Jack Huang的github博客空间](https://mucaoshen.github.io/blog/)  
这里是[Jack Huang的github博客空间](https://mucaoshen.github.io/blog/, "Jack Huang的博客空间")
### 参考式
参考式超链接一般用于学术论文上面，或者另一种情况，如果某个链接在文章中多处使用
，那么使用引用的方式创建链接将非常好，它可以让你对连接进行统一的管理。   
语法说明：参考式链接分为两部分，稳重的写法为[链接文字][链接标记]，在文本的任意位置添加
[链接标记]:链接地址 "链接标题"，链接地址与链接标题中间有一个空格。  
如果链接文字本身可以作为链接标记，你也可以写成[链接文字][] [链接文字]：链接地址的形式，见代码
```markdown
我经常上的几个网站有[Google][1]，[Baidu][2]和[Jack Huang的github博客空间][]。

[1]:http://www.google.com
[2]:http://www.baidu.com "百度搜索的地址"
[Jack Huang的github博客空间]:https://mucaoshen.github.io/blog/
```
view  
我经常上的几个网站有[Google][1]，[Baidu][2]和[Jack Huang的github博客空间][]。

[1]:http://www.google.com
[2]:http://www.baidu.com "百度搜索的地址"
[Jack Huang的github博客空间]:https://mucaoshen.github.io/blog/
### 自动链接
语法说明：Markdown支持以比较简短的自动链接形式来处理网址和电子邮件信箱，只要用<>包起来，Markdown就会自动
把它转成链接。一般网址的链接文字就和链接地址一样，如
```markdown
<http://exmaple.com/>
<address@example.com>
```
view  
<http://exmaple.com/>  
<address@example.com>
## 锚点
在网页中，锚点其实就是页内超链接，也就是链接本文档内部的某些元素，实现当前页面中的跳转。比如我在这里写下一
个锚点，点击回到目录，就能跳转到目录。在目录中点击这一节，就能跳过来。还有下一届的注脚。这些根本上都是用锚
点来实现的。  
注意：  
    1.Markdown Extra只支持在标题后插入锚点，其他地方无效。  
    2.Leanote编辑器右侧显示效果区域暂时不支持锚点跳转，所以点来点去发现没有跳转不必惊慌，但是你发布成笔记
      或博文后是支持跳转的。
      
```markdown
## 0.跳转测试
//github中的markdown写法
跳转到[跳转测试](#0跳转测试)
```
view  
#### 0.跳转测试

跳转到[跳转测试](#0跳转测试)
## 列表
### 无序列表
使用*,+,-表示无序列表，多级无序列表则是在某个列表下tab键加上新的无序列表。
```markdown
- 无序列表 一
- 无序列表 二
- 无序列表 三
    - 无序列表 三 的子无序列表
```
view  
- 无序列表 一
- 无序列表 二
- 无序列表 三
    - 无序列表 三 的子无序列表
### 有序列表
有序列表则使用数字接着一个英文句点再加空格，多级有序列表是在列表下加上tab键再加有序列表。
```markdown
1. 有序列表 一
2. 有序列表 二
3. 有序列表 三
    1. 有序列表 三的子列表
```
view  
1. 有序列表 一
2. 有序列表 二
3. 有序列表 三
    1. 有序列表 三的子列表

### 定义型列表
语法说明：  
定义型列表由名词和解释组成。一行协商定义，紧跟一行协商解释。解释的写法为：
紧跟一个缩进tab。
```markdown
代码块 1 Markdown
:   轻量级文本标记语言，可以转成html，pdf等格式(左侧有一个可见的冒号和四个不可见的空格)

代码块 2
:    这是代码块的定义(左侧有一个可见的冒号和四个不可见的空格)
```
view  
注意github的markdown好像并不支持这种类型的定义，并未有相关生效

### 列表缩进
语法说明：  
列表项目标记通常是放在最左边，但是其实也可以缩进，最多3个空格，项目标记后面则一定要接着至少一个空格或制表符。
```markdown
*   轻轻的我走了，正如我轻轻的来；我轻轻的招手，作别西天的云彩。
那河畔的金柳，是夕阳红的新娘；波光里的艳影，在我的心头荡漾。软泥上的青荇，油油的在水底招摇；在康河的柔波里，我甘心做一条水草！
*   那榆阴下的一潭，不是清泉，是天上虹；揉碎在浮藻间， 沉淀着彩虹似的梦。 
寻梦？撑一支长篙， 向青草更青处漫溯； 满载一船星辉， 在星辉斑斓里放歌。 
但我不能放歌， 悄悄是别离的笙箫； 夏虫也为我沉默， 沉默是今晚的康桥！ 
悄悄的我走了， 正如我悄悄的来； 我挥一挥衣袖， 不带走一片云彩。
```
view  
* 　　轻轻的我走了，正如我轻轻的来；我轻轻的招手，作别西天的云彩。
那河畔的金柳，是夕阳红的新娘；波光里的艳影，在我的心头荡漾。软泥上的青荇，油油的在水底招摇；在康河的柔波里，我甘心做一条水草！
* 　　那榆阴下的一潭，不是清泉，是天上虹；揉碎在浮藻间， 沉淀着彩虹似的梦。 
寻梦？撑一支长篙， 向青草更青处漫溯； 满载一船星辉， 在星辉斑斓里放歌。 
但我不能放歌， 悄悄是别离的笙箫； 夏虫也为我沉默， 沉默是今晚的康桥！ 
悄悄的我走了， 正如我悄悄的来； 我挥一挥衣袖， 不带走一片云彩。
### 包含段落的列表
语法说明：  
列表项目可以包含多个段落，每个项目下的段落都必须缩进4个空格或是一个制表符(必须是全角模式)：
```markdown
* 　轻轻的我走了，正如我轻轻的来；我轻轻的招手，作别西天的云彩。
那河畔的金柳，是夕阳红的新娘；波光里的艳影，在我的心头荡漾。软泥上的青荇，油油的在水底招摇；在康河的柔波里，我甘心做一条水草！
　　那榆阴下的一潭，不是清泉，是天上虹；揉碎在浮藻间， 沉淀着彩虹似的梦。 
寻梦？撑一支长篙， 向青草更青处漫溯； 满载一船星辉， 在星辉斑斓里放歌。 
但我不能放歌， 悄悄是别离的笙箫； 夏虫也为我沉默， 沉默是今晚的康桥！ 
悄悄的我走了， 正如我悄悄的来； 我挥一挥衣袖， 不带走一片云彩。
*   悄悄的我走了，正如我悄悄的来；我挥一挥衣袖，不带走一片云彩。
```
view  
* 　　轻轻的我走了，正如我轻轻的来；我轻轻的招手，作别西天的云彩。
那河畔的金柳，是夕阳红的新娘；波光里的艳影，在我的心头荡漾。软泥上的青荇，油油的在水底招摇；在康河的柔波里，我甘心做一条水草！  
　　那榆阴下的一潭，不是清泉，是天上虹；揉碎在浮藻间， 沉淀着彩虹似的梦。 
寻梦？撑一支长篙， 向青草更青处漫溯； 满载一船星辉， 在星辉斑斓里放歌。 
但我不能放歌， 悄悄是别离的笙箫； 夏虫也为我沉默， 沉默是今晚的康桥！ 
悄悄的我走了， 正如我悄悄的来； 我挥一挥衣袖， 不带走一片云彩。
* 　　悄悄的我走了，正如我悄悄的来；我挥一挥衣袖，不带走一片云彩。
### 包含引用的列表
语法说明：
如果要在列表项目内放进引用，那>就需要缩进：
```markdown
* 阅读的方法：
　 > 打开书本。　　
　 >> 打开电灯。
```
view  
* 阅读的方法：
    > 打开书本。
    >> 打开电灯。

### 包含代码区块的引用
语法说明：  
如果想要在引用中放代码区块的话，该区块就需要tab缩进两次，也就是8个空格或是两个tab：  
```markdown
>\t\t（or        ）ctrl-v
```
view  
* 代码列表
  >     ctrl-v,int i = 1;
  >>        ctrl-c,int a = 1;

### 一个特殊情况
在特许情况下，项目的列表很可能会不小心产生，像下面这样的写法：  
```markdown
1986. How are you.
```
view  
1986. How are you.  

换句话说，在行首出现数字-句点-空格，要避免这样的状况，可以在句点前面加上反斜杠：  
```markdown
1986\. How are you.
```
view  
1986\. How are you.  
这样才会显示正常

## 引用
语法说明：  
引用需要在被引用的文本前加上>符号，多级引用则多加>符号。
```markdown
> 这是一个有两段文字的引用,
无意义的占行文字1.
无意义的占行文字2.

> 无意义的占行文字3.
无意义的占行文字4.
```
view  
> 这是一个有两段文字的引用,
无意义的占行文字1.
无意义的占行文字2.

> 无意义的占行文字3.
无意义的占行文字4.

### 引用的多层嵌套
语法说明：
区块引用可以嵌套(例如：引用内的引用)，只要根据层次加上不同数量的>：
```markdown
>>> 请问 Markdwon 怎么用？ - 小白

>> 自己看教程！ - 愤青

> 教程在哪？ - 小白
```
view  
>>> 请问 Markdwon 怎么用？ - 小白

>> 自己看教程！ - 愤青

> 教程在哪？ - 小白
### 引用其他要素
引用的区块内也可以使用其他的Markdown语法，包括标题、列表、代码区块等:
```markdown
> 1.   这是第一行列表项。
> 2.   这是第二行列表项。
> 
> 给出一些例子代码：
> 
>     return shell_exec("echo $input | $markdown_script");
```
view  
> 1.   这是第一行列表项。
> 2.   这是第二行列表项。
> 
> 给出一些例子代码：
> 
>       return shell_exec("echo $input | $markdown_script");

## 插入图像
图片的创建方式与超链接的相似，而且和超链接一样也有两种写法，行内式和参考式写法。  
语法中图片Alt的意思是如果图片因为某些原因不能显示，就用定义的图片Alt文字来代替
图片。图片的title则和连接中的tilte一样，表示鼠标悬停于图片上时出现的文字。Alt
和title都不是必须的，可以省略，但建议写上。
### 行内式
语法说明： 图片Alt
```markdown
美丽风景：
![美丽风景](https://yuhongjun.github.io/assets/media/scenery.jpeg "美丽风景")
```
view  
美丽风景： 
![美丽风景](https://yuhongjun.github.io/assets/media/scenery.jpeg "美丽风景")

### 参考式
语法说明：  
在文档要插入图片的地方写![图片Alt][标记]  
在文档的最后写上[标记]:图片地址 "title"
```markdown
![美丽风景][scenery]

[scenery]:https://yuhongjun.github.io/assets/media/scenery.jpeg "美丽风景"
```
view  
![美丽风景][scenery]

[scenery]:https://yuhongjun.github.io/assets/media/scenery.jpeg "美丽风景"

## 内容目录
在段落中填写[TOC]以显示全文内容的目录结构  
貌似github中并不支持TOC  
view  
全文目录  
[TOC]
## 注脚
语法说明：  
在需要添加注脚的文字后加上脚注名字[^注脚名字]，称为加注。然后在文本的任意位置(一般在最后)添加脚注，
脚注前必须有对应的脚注名字。  
注意：经测试注脚与注脚之间必须空一行，不然会失效。成功后会发现，即使你没有把注脚写在文末，经Markdown转换
之后，也会自动归类到文章的最后  
又注意：github的markdown是不支持这种方式的注脚的，可以采用另外一种办法-超链接来解决，如下所示
```markdown
使用 Markdown[^1]可以效率的书写文档, 直接转换成HTML<sup>[\[1\]](#myfootnote1)</sup>, 你可以使用Leanote编辑器进行书写。

[^1]:Markdown是一种纯文本标记语言
<a name="myfootnote1"> \[1\] </a> HyperText Markup Language 超文本标记语言
```
view  
使用 Markdown[^1]可以效率的书写文档, 直接转换成HTML<sup>[\[1\]](#myfootnote1)</sup>, 你可以使用Leanote编辑器进行书写。

[^1]:Markdown是一种纯文本标记语言
<a name="myfootnote1">\[1\]</a> HyperText Markup Language 超文本标记语言

## Latex公式
<script type="text/javascript"
src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>
语法说明：  
因为github的markdown不再支持latex公式渲染，因此现在的方式是1.通过latex编辑器网址[latex编辑器网址]获取图片，并放到相应目录中，在github内引用相应的图片
2.在文章的头部加入如下的script脚本，然后再去latex编辑器网址[latex编辑器网址]获取html的代码，直接引用。如下：

[latex编辑器网址]: https://www.codecogs.com/eqnedit.php "latex编辑器网址"
```markdown
<script type="text/javascript"
src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>
// E=mc^2
<a href="https://www.codecogs.com/eqnedit.php?latex=E=mc^2" target="_blank"><img src="https://latex.codecogs.com/gif.latex?E=mc^2" title="E=mc^2" /></a>
```
### 行内公式
```markdown
质能守恒方程可以用一个很简洁的方程式 $E=mc^2$ 来表示
对github已经不起作用了
```
view  
质能守恒方程可以用一个很简洁的方程式 <a href="https://www.codecogs.com/eqnedit.php?latex=E=mc^2" target="_blank"><img src="https://latex.codecogs.com/gif.latex?E=mc^2" title="E=mc^2" /></a> 来表示
### $$表示整行公式
```markdown
$$\sum_{i=1}^n a_i=0$$
$$f(x_1,x_x,\ldots,x_n) = x_1^2 + x_2^2 + \cdots + x_n^2 $$
$$\sum^{j-1}_{k=0}{\widehat{\gamma}_{kj} z_k}$$
对github已经不起作用
```

## 流程图
github的markdown暂时不支持流程图

## 表格
语法说明：  
不管是哪种方式，第一行为表头，第二行分割表头和主体部分，第三行开始每行为一个表格行。列与列之间用管道符|隔开。
原生方式的表格每一行的两边也要有管道符。第二行还可以为不同的列指定对齐方向。默认为左对齐。
github要求要至少3条-符号，并且写表格应与上文有回车相隔。表格中居中为:---:，右对齐为---:。
1. 简单方式写表格
    ```markdown
    
    学号|姓名|分数
    ---|---|---
    小明|男|75
    小红|女|79
    小陆|男|92
 
    ``` 
2. 原生方式写表格：
    ```markdown
    
    |学号|姓名|分数|
    |---|---|---|
    |小明|男|75|
    |小红|女|79|
    |小陆|男|92|
 
    ```
3. 为表格第二列指定方向：
    ```markdown
    
    产品|价格
    :---:|---:
    Leanote 高级账号|60元/年
    Leanote 超级账号|120元/年
 
    ```
view  
1. 简单方式写表格:

    学号|姓名|分数
    ---|---|---
    小明|男|75
    小红|女|79
    小陆|男|92
  
2. 原生方式写表格：
  
    |学号|姓名|分数|
    |---|---|---|
    |小明|男|75|
    |小红|女|79|
    |小陆|男|92|
  
3. 为表格第二列指定方向：
      
    产品|价格
    :---:|---:
    Leanote 高级账号|60元/年
    Leanote 超级账号|120元/年

## 分隔线
语法说明：  
可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。下面是每种写法：
```markdown
* * *

***

*****

- - -

---------------------------------------
```
view  
显示效果都一样
* * *

***

*****

- - -

---------------------------------------

## 代码
语法说明：
插入程序代码的方式有两种，一种是利用缩进(Tab)，另一种是利用`符号包裹代码。

### 行内式
```markdown
C语言里的函数 `scanf()` 怎么使用？
```
view  
C语言里的函数 `scanf()` 怎么使用？

### 缩进式多行代码
缩进4个空格或一个制表符,一个代码区块会一直持续到没有缩进的哪一行(或是文件结尾)。  
注意：必须在缩进前先回车一行
```markdown

    #include <stdio.h>
    int main(void)
    {
        printf("Hello world\n");
    }
```
view
  
    #include <stdio.h>
    int main(void)
    {
        printf("Hello world\n");
    }

### 用六个`包裹多行代码，可以额外申明修饰的语言
```markdown
\```(这里可以申明代码语言，比python，注意去掉\符号)
#include <stdio.h>
int main(void)
{
    printf("Hello world\n");
}
\```
```
view
```C
#include <stdio.h>
int main(void)
{
    printf("Hello world\n");
}
```

### html原始码
语法说明：  
在代码区块里面， & 、 < 和 > 会自动转成 HTML 实体，这样的方式让你非常容易使用 Markdown 插入范例用的 HTML 原始码，只需要复制贴上，剩下的
 Markdown 都会帮你处理，例如：
 ```html
<div class="footer">
   © 2016 ***
</div>
```
view
<div class="footer">
   © 2016 ***
</div>

## 任务列表
语法说明：  
这个是github markdown的一个特性，可以通过建立任务表来展示当前的任务执行情况
```markdown
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
```
view  
- [x] @mentions, #refs, [links](), **formatting**, and ~~tags~~ supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
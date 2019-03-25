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
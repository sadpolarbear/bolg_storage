---
title: markdown 知识总结
categories:
  - 知识总结
  - markdown
tags:
  - 知识

date: 2023-08-11 
---

# 1 打对号 或者 叉号  以及特殊符号

1. 可以使用 HTML 实体来插入符号。例如，可以使用` ✔` 来插入一个对号，`✖` 来插入一个叉号。

```
- 任务1 &#x2714;
- 任务2 &#x2716;

```

-  任务1 &#x2714;

-  任务2 &#x2716;

2. 使用-+空格+[空格]+空格 

   使用-+空额+[x]+空格

- [ ] 

- [ ] 西瓜

  	梅花 &clubs;

​		黑桃 &spades;

​			红心&hearts;

​				方片&loz;

​			五角星&#9956;

​		雪人&#9731;



[特殊符号网页大全]<https://symbl.cc/cn/unicode/blocks/miscellaneous-symbols/>






# 2 字体大小

照着这个代码书写，就能调节字体大小

1. <small>word</small>

2. <big>hello</big>

   

# 3 字体 颜色 大小  形式 的代码使用

1. 改变颜色(color)，这个颜色代码就是html颜色代码

 	<font color =blue>hello world</font>

​	<font color=#008000>我是绿色</font>

2. 改变字体样式(face)

​	<font face="微软雅黑">我是微软雅黑</font>

<font face="STCAIYUN">	我是华文彩云</font>

3. 改变尺寸(size)

​	<font size=5>尺寸5</font>

4. 一起使用

   例如 <font face="黑体" color=green size=5>我是黑体，绿色，尺寸为5</font>

5. 调节字体背景

​			<font style="background-color:green">绿色小标签</font>

6. 全部一起使用

   <font style="background-color:#00FFFF" font face="黑体" color=green size=5>我是黑体，绿色，尺寸为5</font>

`注意 颜色既可以用英语单词,也可以用html代码`

# 4 一般书写格式

1. *hello* 斜体

2. **world** 粗体

3. `hello world` 标记

   <kbd>hello</kbd> 或者可以通过转义字符代码来获得

4. ==fighting== 高亮

5. ***hello world*** 粗斜体

6. <u>hello</u> 下划线

   

7. ---

   分界线 自己ctrl + / 看代码

8. ~~hello~~ 删除线

9. > 引用 
   >
   > > 多级引用

10. 链接 <https://markdown.com.cn>

    或者 可以[链接](https://markdown.com.cn)

    只要按住ctrl键，再点击以下链接，就可以直接网页跳转。

11. + 靠tab enter(退出某级,直接回到正文)  shift+tab backspace(回到上一级) 一起来调节级数 

      - 多级
        - 列表 

      1. hello
      2. world

      

12. ^hello^ 上标

13. ~hello~ 下标

14. 

15. <!-- 这是 html 注释， 在 markdown 中也不会被编译， 可以作为注释的方法 --> 注释

    <!--hello-->

# 5 特殊符号的快捷键

1. 在中文输入法状态下，可使用「Shift + 6」输入省略号。注意是 6 个点，而非 3 个点，如 ……
2. 在中文输入法状态下，可使用「Shift + -」输入破折号。注意该符号应占两个汉字宽度，如——
3. 在中文输入法状态下，可使用「Shift + `（ESC 键下方）」输入波浪线。可用波浪线表示数值的区间，如~

# 6 图片的处理

## 1 直接引用



![picture](https://pic2.zhimg.com/80/v2-f6b017b641e322028b68bf15ce54f299_1440w.webp)


默认 直接从网络中获取 ，不考虑尺寸，位置的问题

___





## 2 添加注释和改变位置

<div alt="fig">可以在此给图片添加注释</div><img align="left" src="https://pic2.zhimg.com/80/v2-f6b017b641e322028b68bf15ce54f299_1440w.webp"/><div alt="fig">也可以在下方添加注释</div>



调节了 位置 ，但是尺寸太大，所以没有多少区别 有三种 center right left






<div alt="fig">图释说明</div> 这个代表添加注释 放在链接图片之前的标签







___



## 3 调节大小 位置和题注



<div alt="fig">图释说明,同时你也可以写写 
你想写的东西</div><div align="right"><img width="350" height="250" src="https://pic2.zhimg.com/80/v2-f6b017b641e322028b68bf15ce54f299_1440w.webp"/></div><div alt="fig">题注</div>


图片调整了大小，和位置





---







# 7 内容折叠

<details>
<summary>展开查看</summary>
<pre><code>你是谁;</code></pre>
</details>




---

或者

<details>
    <summary>折叠标签</summary>
    <p>邮件地址标签 （<code>3080733673@qq.com</code>）：</p>
    <iframe src="https://zhixingo.github.io/plays/pdfv/?url=https://files.catbox.moe/5iz1r9.pdf" height="400" frameborder="0" scrolling="no"></iframe>
</details>




这里面的pdf文件是外链标签

---




注意 

其中<br>是换行 ,无法在他后面写东西

<details>
<summary><b>See what's inside &darr;</b></summary>
  <table border="1">
    <tr>
      <th>题目</th>
    </tr>
    <tr>
      <td>
        这个样子<br>
        多行内容<br>
        不至于让分不清哪里是折叠内容的结束<br>
        链接<a href='url'>hello worlld</a><br>
<table><tr><td bgcolor=yellow>自己的思考</td></tr></table>
      </td>
    </tr>
  </table>
</details>














# 8 锚点

使用方法ctrl+右键 且注意 id 必须使用英语 ，例如prefae 和text这种

第一步：添加链接		<a href="#preface">前言</a>
第二部：添加锚点		<a id="preface">前言</a>

<a href="#test1">点我跳转到：测试1</a>
<a href="#end">点我跳转到：末位</a>



<a id="test1">测试1</a>








# 9 表格背景色





<table><tr><td bgcolor=green>背景色green</td></tr></table>



# 10 文字排版

<center>居中</center>
<p align="left">左对齐</p>
<p align="right">右对齐</p>





# 11 gif插入

插入gif图片

![Alt Text](https://media.giphy.com/media/vFKqnCdLPNOKc/giphy.gif)







或者可以调整其大小和调整其位置

<div align="middle"><img  src="https://media.giphy.com/media/vFKqnCdLPNOKc/giphy.gif" width="40" height="40" /></div>









以下是我用github图库所推送的gif图片，gif图片你可以上网下载，用pic来推送
![Alt Text](https://github.com/sadpolarbear/picture/raw/main/blogImg/202309171022991.gif)









这是居中模式下的gif图片，因为不好判断图片尺寸，所以只要知道这个middle right 和left 就行<img align="right" src="https://github.com/sadpolarbear/picture/raw/main/blogImg/202309171022991.gif"/>

通过调节位置，就可以达到这种侧边书写的逻辑。





# 12 音乐插入


<audio id="audio" controls="" preload="none">
      <source id="mp3" src="https://github.com/sadpolarbear/picture/raw/main/blogImg/202309171040315.mp3">
</audio>



这是通过用pic导入视频，推送到github仓库中，然后用html 语句来导入





直接通过网易云中的生成外链播放器[^2]



，iframe模块


<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width=330 height=86 src="//music.163.com/outchain/player?type=2&id=16435049&auto=1&height=66"></iframe>



# 13 表格



直接就是插入默认 就可以了 [^1]





|      |      |      |
| ---- | ---- | ---- |
|      |      |      |
|      |      |      |
|      |      |      |



# 14 脚注与文末链接













<a id="end">末尾</a>



[^1]: 这是脚注跳转的链接,记住用ctrl加上右击
[^2]: 脚注用[^数字]来定义,之后点击跳转,你来书写确认

[3]: https://www.zhihu.com/question/316039999	"参考文献,我这里懒的去找,所以直接就引用了一个壁纸网站"


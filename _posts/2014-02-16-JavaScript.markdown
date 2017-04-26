---
layout: post
title:  "JavaScript基础"
date:   2014-02-16 09:39:27 +0800
categories: jekyll update
---



1.javascript定义：javascript是基于对象和事件驱动，并具有安全性能的弱类型脚本语言。

2.Javascript格式

<script type="text/javascript">

 <!--

       

 //-->

 </script>

3.window对象(窗口对象)

4.window.alert(“”):弹出一个带有确定的对话框.

5.window.status:窗口的状态栏

6.document对象(文档对象)

7.document.write():页面输出     echo “html”;

8.对象调用方法格式   方法  函数

  对象.方法名();

9.对象调用属性格式

  对象.属性名;

10.注释  //单行注释      /*    */多行注释   

 

11.定义变量格式： var 变量名=值  例如：var a=10; 

  定义变量的关键字var,在定义变量的时候可以省略var  例如:var a=1; 或者a=1;

12.javascript数据类型

基本数据类型：数值类型number、布尔类型boolean、字符串类型string

       特殊数据类型：空null、未定义undefined

       复合数据类型：数组Array、对象object

13.typeof():获取变量的数据类型  判断变量的数据类型

14Javascript语言结构

   顺序

   选择  if     if...else     switch

   循环  for   for...in   while  do...while  

15.javascript自定义函数格式

function 函数名([参数列表]){  

Javascript语句;

} 

16.javascript自定义函数的调用格式：window.函数名();   函数名();

注：参数不能加var

例如：

//自定义两数相加函数

function add(a,b){

              var sum = a+b;

              return sum;

       }

//调用函数

       var sum = add(100,2);

//输出

       document.write("sum="+sum);

17.var obj =document.getElementById(id):通过id获取对象

18.innerHTML:设置或者获取标签内的html

19.innerText:设置或者获取标签内的文本

20.onclick:单击事件

21内置对象有哪些？

字符串对象String  

数组对象Array  

数学对象Math  

日期对象Date  

22字符串对象的属性：

length：取字符串长度

23字符串对象的方法(函数)  7个

charAt():通过索引值找字符

indexOf():查找第一次出现的字符的下标

lastIndexOf():查找最后一次出现的字符的下标

substr(索引值,个数):截串，返回一个从指定位置开始的指定长度的子字符串。

substring(开始索引值,结束索引值):截串，返回位于 String 对象中指定位置的子字符串。

replace('搜索串','替换串'):替换字符串.如果搜索串不在字符串中，不替换(原串)  

split():把字符串变成数组

24数组对象的属性

length:取数据元素个数

25数据对象的方法(函数)  1个

join():把数组元素连接成一个字符串

26数学对象的方法   4个

ceil():向上取整

floor():向下取整

round():四舍五入

random():0－1的随机浮点数

27日期对象的方法

getYear():获取年

getMonth():获取月

getDate():获取日

getHours():获取时

getMinutes():获取分

getSeconds():获取秒

getTime():获取时间戳

方方法返回一个整数值，这个整数代表了从 1970 年 1 月 1 日开始计算到 Date 对象中的时间之间的毫秒数法返回一个整数值，这个整数代表了从 1970 年 1 月 1 日开始计算到 Date 对象中的时间之间的毫秒数

toLocaleString():把日期格式化成本地时间

 

28.创建当前时间 var now = new Date();

                                                    

周六下午，背写五遍

29.DOM:document object model 文档对象模型

30.document.getElementById(“id”):通过id找对象(一个)

31.document.getElementsByName(“name”):通过name属性的值找对象数组

32.document.getElementsByTagName(“tagName”):通过标签找对象数组

33.getAttribute(属性):获取属性的值

34.setAttribute(属性,值):设置属性的值

35.document.getElementsByName(“name”)[0]:通过name属性的值找到第一个对象

36.document.getElementsByTagName(“tagName”)[0]:通过标签找到第一个标签对象

37.对象.style.样式属性=值:设置对象的样式

___________________________________________________________________________

周日上午，背写五遍

38.BOM:browser object model:浏览器对象模型

39.window对象方法6个

alert():弹出一个带有确定按钮的对话框(警告框)

confirm():弹出一个带有确定和取消按钮的对话框(确认框)

prompt():弹出一个带有输入框的对话框

open():打开一个新窗口

setInterval(‘函数名()’,毫秒):计时器,每隔多少秒，执行某函数

setTimeout(函数名()’,毫秒):计时器,过了多少秒，执行某函数，只执行一次。

40.location对象的属性   操作url

location.href:链接，跳转

41.history对象  操作用过(历史)url

history.go(1):前进

history.go(-1):后退

history.go(0):刷新

history.forward():前进

history.back():后退

 

 

                                                 

 

42.javascript事件

onload:页面加载事件

onunload:页面卸载事件

onfocus:获得焦点事件

onblur:失去焦点事件

onchange:内容改变事件

鼠标事件

onclick:鼠标单击事件

onmousemove:鼠标移动事件

onmouseover:鼠标移上事件

onmouseout:鼠标移开事件

onmousedown:鼠标按下事件

onmouseup:鼠标抬起事件

键盘事件

onkeydown:键盘按下事件

onkeyup:键盘抬起事件

表单事件

onsubmit:表单提交事件

43.event对象:事件对象

44.event.srcElement:通过事件找对象

45.Javascript常用函数

encodeURI():url编码

decodeURI():url转码

eval():执行字符串内的内容

parseInt():剖析字符串成int型

parseFloat():剖析字符串成float型

isNaN(“字符串”):测试字符串是不是数字，返回值为true,说明该字符串不是数字，返回值为false,说明字符串为数字

                                      

 

 

javascript正则表达式

1.定义:匹配某个句法规则的字符串

2.组成:正则表达式由普通字符与元字符组成    

3.格式：/   /

4.元字符

[]:匹配任意单个字符

\d:匹配数字

\w:匹配字母、数字和_

.:匹配除换行符以外的任意单个字符

^：开始

$：结束

*：重复任意次，相当于{0,}

+：至少重复,相当于{1,}

?：重复0或者1次,相当于{0,1}

{n}：重复n次

{n,}：重复n次以上

{n,m}：重复n到m次

转义字符\

( ) :子字符集

|：或者

5.模式修正符

 g:全文搜索

 i:忽略大小写

 gi:全文搜索且忽略大小写

 

6.正则表达式方法

 test():测试正则表达式

                                           

javascript思路：

1  建页面

2  找事件

3  找对象

4   对象操作属性(取值，赋值)

5   对象操作样式(取值，赋值)





[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/

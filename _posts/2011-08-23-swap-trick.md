---
layout: post
title: 掉换变量小trick
date: 2011-08-23 12:38
comments: true
categories: []
---
如果你需要掉换两个变量的值，通常需要一个临时变量（当然，前提是没用类似Python的语言，他们支持a,b=b,a这种语法）就像这样做：
<pre class="brush: r; gutter: true">temp = a;
a = b;
b = temp;</pre>
但是如果这些都是整型变量，有一个小trick可以节省一点内存。使用算术代替临时变量：
<pre class="brush: r; gutter: true">a = a + b;
b = a - b;
a = a - b;</pre>
如果你的机器上整型占32字节，那么恭喜你节省了4比特的内存，哈哈。

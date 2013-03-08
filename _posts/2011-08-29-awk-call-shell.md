---
layout: post
title: Awk中使用shell命令调用系统资源或数据
date: 2011-08-29 02:05
comments: true
categories: []
---
ex1. '{”shell命令" | getline}' shell命令（如date可取当前日期）并用getline记录进$0；
ex2. '{system( "shell命令" )}' 该办法的缺点是awk与shell命令之间不能存在数据的交互；
ex3. 在awk语句的最后形如data&gt;newdata之前赋值（如IF_NUM=$if_num），可将shell中现有数据传给awk使用，如果脚本中需要根据入参做条件判断则该办法很好用。

<strong>update </strong>看到了一篇文章&lt;awk引用外部变量的六种方法&gt;比这里总结的更好
ex1. awk -v awkvar=$extvar ... #使变量的作用域扩展至BEGIN{}
ex2. awk '' "awkvar=$extvar" filename #BEGIN段不可用
ex3. 在awk表达式中使用'$extvar'
ex4. 模式引用(在正则表达式中引用外部变量) '"$extvar"'
ex5. 遍历外部数组(用于BEGIN段处理) awk -f 'BEGIN{for(i=1;i ex6. 引用环境变量 ENVIRON["environment variable"]
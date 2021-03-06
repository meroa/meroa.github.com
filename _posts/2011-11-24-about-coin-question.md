---
layout: post
title: 两道硬币面试题
date: 2011-11-24 14:26
comments: true
categories: 概率统计
---
Q1: 一个均匀硬币不断抛啊抛，假如抛个100次，那么连续抛出同一面的次数，这个次数最多是多少？
<pre class="brush: r; gutter: true">coin.len = function(v) {
    x = rbinom(1:v, 1, 0.5)
    len = 1
    for (i in 1:v)
      {
      for (j in 1:(v-i+1))
        {
        if ((sum(x[i:(i+j-1)]) == 0) | (sum(x[i:(i+j-1)]) == j))
          {
          len = max(len, j)
          }
        }
      }
    return(len)
}
set.seed(1024)
mean(len &lt;- replicate(1000, coin.len(1000))
# [1] 10.288</pre>
Q2: 一个均匀硬币不断抛啊抛，一直抛到出现HTT（正反反）和HTH（正反正），哪个需要抛的次数多？
<pre class="brush: r; gutter: true">coin.seq = function(v) {
    x = NULL
    n = 0
    while (!identical(x, v)) {
        x = append(x[length(x) - 1:0], rbinom(1, 1, 0.5))
        n = n + 1
    }
    n
}
set.seed(1024)
mean(htt &lt;- replicate(1e+05, coin.seq(c(1, 0, 0))))
# [1] 8.003
mean(hth &lt;- replicate(1e+05, coin.seq(c(1, 0, 1))))
# [1] 10.006</pre>

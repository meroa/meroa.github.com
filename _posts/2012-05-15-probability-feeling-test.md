---
layout: post
title: 概率论感觉测试（转）
date: 2012-05-15 14:45
comments: true
categories: 概率统计
---
<strong>概率论感觉测试（一）</strong>

1. 假设考试周为1个礼拜（周一到周日），且考试时间为均匀分布，<wbr>假使你有3门考试，则最后一门考试大约在
A 周五
B 周六
C 周日</wbr>

<span style="color: #ffffff;">Answer: B. 一般的讲在[0,1]</span><wbr><span style="color: #ffffff;">之间n个均匀分布的随机变量最大值期望为n/(n+1),</span><wbr><span style="color: #ffffff;">也就是可以认为这n个随机变量分别大约在</span>
<span style="color: #ffffff;"> 1/(n+1),2/(n+1),…,n(n+1)。</span><wbr><span style="color: #ffffff;">这道题那么算一下大概就是在周六的上午。</span></wbr></wbr></wbr>

2. 如果你去参与一项赌博，每次的回报为正态分布，<wbr>假设你赌了100把发现赢了10000块（明显是很小概率事件，<wbr>但假设确实发生了），那么你觉得你最有可能是因为</wbr></wbr>

A 有一把赢了巨多
B 一直在慢慢的赢
C 两种情况都有可能

<span style="color: #ffffff;">Answer: B. 也许答案对很多人有些出乎意料。在这种情况下，</span><wbr><span style="color: #ffffff;">可能有人觉得能够连续赢很多把很难，但是实际上赢一把大的更难。</span><wbr><span style="color: #ffffff;">这个问题是随机问题中的长尾和短尾的问题。</span><wbr><span style="color: #ffffff;">长尾的意思就是取大的值的概率不是很小，而短尾正好相反。</span><wbr><span style="color: #ffffff;">但是题目中的正态分布属于短尾，因为密度函数是指数下降的，</span><wbr><span style="color: #ffffff;">如果稍微改一下题目中的分布，</span><wbr><span style="color: #ffffff;">则有可能是因为一次赢了很大而最后赢的。另外说一句，</span><wbr><span style="color: #ffffff;">有一本书叫《长尾理论》，</span><wbr><span style="color: #ffffff;">里面说明了现在的经济中有很多东西是长尾的，</span><wbr><span style="color: #ffffff;">比如说一年销量排在100000名之后的歌曲仍然能占据市场的一</span><wbr><span style="color: #ffffff;">部分。这是电子商务流行的很重要原因，</span><wbr><span style="color: #ffffff;">因为不必支付储存这个长尾的cost。</span></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr>

3. 有一根密度不均匀的绳子，<wbr>你想通过测量多点的密度来估计他的重量（你知道截面积）。<wbr>则如果给你n次测量密度的机会的话，如果n很大，（<wbr>估算质量就通过这些点取平均然后乘以截面积）</wbr></wbr></wbr>

A 按规律等间隔选取测量点会测得准些
B 随机选取测量点会测得准些
C 两种方法差不多

<span style="color: #ffffff;">Answer: A. 也许这个也略有些意外。对于一维的情况，方法A略好于方法B。</span><wbr><span style="color: #ffffff;">但是在高维的情况下方法A就一般情况下不如方法B了，</span><wbr><span style="color: #ffffff;">原因是要想获得相同的效果，这个“有规律的点”需要选取太多。</span><wbr><span style="color: #ffffff;">这是所谓的Quasi-Monte</span>
<span style="color: #ffffff;"> Carlo Sampling 和 Monte Carlo Sampling之间的关系</span></wbr></wbr></wbr>

4. 台湾大选，假定马英九最终得到600000票，<wbr>谢长廷得到400000票，如果一张一张的唱票，<wbr>则过程中马英九一直领先谢长廷的概率为</wbr></wbr>

A 0.1
B 0.2
C 0.3
D 0.4

<span style="color: #ffffff;">Answer: B. 直觉上讲这个概率并不会太大，</span><wbr><span style="color: #ffffff;">而且尤其是在前面几张的时候多少会出现一些反复。</span><wbr><span style="color: #ffffff;">实际上这个结果跟一共多少人投票没什么关系，如果得票比例为a:</span><wbr><span style="color: #ffffff;">b(a&gt;b),则这个概率为(a-b)/(a+b)。</span></wbr></wbr></wbr>

5.  你拿10块钱去赌场赌大小，你有两种玩法，一种是每次赌10块，<wbr>一种每次赌1块，你决定都是输光或者赢到100块就走，则</wbr>

A 两种方法输光的概率一样
B 第一种输光的概率较大
C 第二种输光的概率较大

<span style="color: #ffffff;">Answer: A. 不管什么赌法都不会改变这个概率。</span><wbr><span style="color: #ffffff;">我认为这是随机过程中一个比较简单但是很有意义的结论，</span><wbr><span style="color: #ffffff;">意思就是说you can’t</span>
<span style="color: #ffffff;"> beat the system。这件事情说明了对于像股市，赌博这种系统，</span><wbr><span style="color: #ffffff;">如果你假设了随机性，则其实怎么操作结果都是一样的。</span><wbr><span style="color: #ffffff;">因此重要的在于发掘其中的非随机性。另外，</span><wbr><span style="color: #ffffff;">到100的概率很容易计算，因为初始值是10，</span><wbr><span style="color: #ffffff;">假设到100的概率为p，则有100p*0(1-p)=10，</span><wbr><span style="color: #ffffff;">也即p=0.1</span></wbr></wbr></wbr></wbr></wbr></wbr></wbr>

6. 100个球随机的放在100个箱子里，最后空箱子的数量大约是

A.  0-0.1
B.  0.1-0.2
C.  0.2-0.3
D.  0.3-0.4

<span style="color: #ffffff;">Answer: D.这个题可以用简单的概率论计算。结论是不管多少个球，c*</span><wbr><span style="color: #ffffff;">n个球放到n个箱子里，最后空箱子的个数约为e^-c，</span><wbr><span style="color: #ffffff;">现在的情况是箱子数和球数一样多，那么就约为e^-1.</span></wbr></wbr>

7、打10000副拱猪，总共持有9500-<wbr>10500个A的概率大约在</wbr>

A.  80%-90%
B.  90%-95%
C.  95%-99%
D.  99%以上

<span style="color: #ffffff;">Answer: D. 这个可以用中心极限定理计算。事实上这个题也不需要计算，</span><wbr><span style="color: #ffffff;">只是要考察大家的一个感觉，实际上这个概率大于0.99…9，</span><wbr><span style="color: #ffffff;">一共有9个9，尽管有时候我们打牌仍然觉得牌总是很差。。</span><wbr><span style="color: #ffffff;">只是我们不注意我们抓好牌的时候罢了。</span></wbr></wbr></wbr>

8. 有以下几个国家，每个国家有自己的习俗。<wbr>问哪个国家长期以后男人最多</wbr>

A.  每个家庭不断的生孩子直到得到第一个男孩为止
B.  每个家庭不断的生孩子直到得到第一个女孩为止
C.  每个家庭不断的生孩子直到得到一男一女为止
D.  以上几个国家最后男女比例基本一样

<span style="color: #ffffff;">Answer: D. 我们只需要考察一个家庭最后产生多少男女即可以。</span><wbr><span style="color: #ffffff;">用概率的方法可以得到不管哪个方法都是1:1。事实上，</span><wbr><span style="color: #ffffff;">我们只是把一个很长的男女的序列按照不同的方式来截断。</span><wbr><span style="color: #ffffff;">当然这个序列本上包含多少男女是不变的。</span><wbr><span style="color: #ffffff;">我每次都愿意以另外一个例子来说明，那就是如果我们在网上下棋，</span><wbr><span style="color: #ffffff;">可以每天下到第一盘输为止或是第一盘赢为止或是有输有赢为止，</span><wbr><span style="color: #ffffff;">显然不管怎样，因为你的实力是恒定的，</span><wbr><span style="color: #ffffff;">你永远都是你本来应有的胜率。</span></wbr></wbr></wbr></wbr></wbr></wbr></wbr>

9. 实验室测试灯泡的寿命。在灯泡坏的时候立刻换新灯泡。<wbr>灯泡寿命约为1小时。考察10000小时时亮着的那个灯泡</wbr>

A.  那个灯泡的寿命期望也约为1小时
B.  那个灯泡的寿命期望约为其他灯泡的2倍
C.  那个灯泡的期望寿命约为其他灯泡的1/2
D.  以上说法都不对

<span style="color: #ffffff;">Answer: B. 这个题可能稍难。如果具体的算需要一点本科高年级的知识。</span><wbr><span style="color: #ffffff;">不过我们仍然可以从直觉得到结果。事实上，</span><wbr><span style="color: #ffffff;">当每个灯泡或是我们观测的事物的生命是随机的时候。</span><wbr><span style="color: #ffffff;">在时间足够久以后的一点，</span><wbr><span style="color: #ffffff;">那个事物的寿命要长于这个事物本身平均的寿命。</span><wbr><span style="color: #ffffff;">因为正是因为它寿命长导致我们容易观测到。简单的说，</span><wbr><span style="color: #ffffff;">如果灯泡有两种，一种只能坚持</span>
<span style="color: #ffffff;"> 1小时，一种能坚持100小时，那我们在后面观测到的99%</span><wbr><span style="color: #ffffff;">都可能是100小时那个。所以观测到的平均寿命较长。</span><wbr><span style="color: #ffffff;">通常我们认为灯泡的寿命是指数分布的，在这个情况下，</span><wbr><span style="color: #ffffff;">答案是2倍。对于一般的分布，甚至有可能平均寿命有限，</span><wbr><span style="color: #ffffff;">而观测的那个寿命期望是无限的。</span><wbr><span style="color: #ffffff;">这个问题在美国一次监狱调查中被发现，</span><wbr><span style="color: #ffffff;">即被调查的囚犯的平均判刑年数要远大于全美平均判刑的年数</span></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr>

10. 如果一个群体里，每个个体以0.2的概率没有后代，0.<wbr>6的概率有1个后代，0.2的概率有两个后代，则</wbr>

A.  这个群体最后会灭绝
B.  这个群体最后将稳定在一个分布，即种群大小在一定范围内震荡
C.  这个群体最后将爆炸，人口将到无穷
D.  不一定会发生什么

<span style="color: #ffffff;">Answer: A. 这是个简单的人口模型。这个可能直觉比较困难，</span><wbr><span style="color: #ffffff;">但是这个实际上和后面的一道题道理是一样的。</span><wbr><span style="color: #ffffff;">注意到每一代的期望总是1。因此根据上次的答案，</span><wbr><span style="color: #ffffff;">这个群体最后会灭绝。对于这种模型，</span><wbr><span style="color: #ffffff;">当每一代的期望小于等于1时，最后的结果都是会灭绝。</span><wbr><span style="color: #ffffff;">对于期望大于1的情况，</span><wbr><span style="color: #ffffff;">我们也可以很简单的通过解方程得到灭绝的概率。</span></wbr></wbr></wbr></wbr></wbr></wbr>

11. 给一个1-n的排列，与原来位置相同的数字的个数的期望大约是 （如 n=5 则51324 与原来位置只有3是相同的）

A.  1
B.  log n
C.  ln n

<span style="color: #ffffff;">Answer: A. 这个题要去算有几个相同的概率是比较难的，</span><wbr><span style="color: #ffffff;">不过实际上有一个很简单的方法。在第1个位置，</span><wbr><span style="color: #ffffff;">这个排列的第1个数字为1的概率为1/n，而期望是可加的，</span><wbr><span style="color: #ffffff;">所以总共与原来位置相同的数字的个数的期望应该是1。</span><wbr><span style="color: #ffffff;">也就是说不管是多少的数字，平均总是有一个数与顺序是相同的。</span><wbr><span style="color: #ffffff;">这个题会非常经常出现在考试和习题中。</span></wbr></wbr></wbr></wbr></wbr>

12. 如果有3个门，有一个背后有大奖。你选中一个，<wbr>主持人知道哪个门后面有奖，<wbr>并且总会打开另外两个中的某个没奖的。现在你有一次换得机会，<wbr>你应该</wbr></wbr></wbr>

A.  换
B.  不换
C.  换不换都一样

<span style="color: #ffffff;">Answer: A. 这个是网上非常经典的一个问题了。不换正确的概率是1/3，</span><wbr><span style="color: #ffffff;">换正确得概率是2/3。我比较喜欢这样去想，</span><wbr><span style="color: #ffffff;">试想一下如果有100个门，你先选定1个，</span><wbr><span style="color: #ffffff;">然后主持人打开98个空的，然后给你机会换不换。我想如果这样，</span><wbr><span style="color: #ffffff;">你不难做出正确的选择。</span></wbr></wbr></wbr></wbr>

13.  以下那件事情发生的期望时间最短

A.  在第0秒，一个物体从原点出发，每一秒以概率1/2向左走，1/<wbr>2向右走，第一次回到原点的时间
B.  一只猴子，每秒种随便按键盘上的一个键，第一次打出"<wbr>Beijing WelcomesYou"的时间
C.  在第0秒，一个物体从原点出发，每一秒以概率1/2向左走，1/<wbr>2向右走，第一次到达1的时间</wbr></wbr></wbr>

<span style="color: #ffffff;">Answer: B. A和C两个事件发生的时间的期望都是+inf.</span>
<span style="color: #ffffff;"> 只有B是有限的。A和C说明了等概率的赌博不可能赢钱（</span><wbr><span style="color: #ffffff;">如果C是有限的则参加赌大小的游戏总能赢钱了）。</span><wbr><span style="color: #ffffff;">而B说明的是另外一条概率上的定理,"What</span>
<span style="color: #ffffff;"> always stands a reasonable chance of happening will almost surely</span>
<span style="color: #ffffff;"> happen, sooner rather than</span>
<span style="color: #ffffff;"> later",也就是说从任何时刻开始，</span><wbr><span style="color: #ffffff;">总有一个固定的概率发生的事情(比如一个猴子打出beijing welcomes you,</span>
<span style="color: #ffffff;"> 这个概率可能是 1/26^20左右)，不过这个概率是多少，</span><wbr><span style="color: #ffffff;">这件事情早晚能发生。</span></wbr></wbr></wbr></wbr>

14,  美国的25分硬币共有50种，上面有50个州的图案，<wbr>如果我们每次得到的硬币是随机的，则大约收集多少可以收集全</wbr>

A.  200
B.  300
C.  400
D.  500

<span style="color: #ffffff;">Answer: A. 这是所谓的收集硬币问题。具体解法不是很容易。</span><wbr><span style="color: #ffffff;">不过结论是要收集齐n种硬币，需要大约nlogn个。</span><wbr><span style="color: #ffffff;">大约思路是收集第k个时候需要大约n/(n-k)次。</span><wbr><span style="color: #ffffff;">平时我们收集一些食品里的卡片，也都遵循这个规律，</span><wbr><span style="color: #ffffff;">不过多数时候每种卡片的数量都是很不同的。</span><wbr><span style="color: #ffffff;">还记得小时候可乐里收集到苹果加蜡烛可以得到到头等奖，</span><wbr><span style="color: #ffffff;">不过最后也没收集到任何一个苹果。</span></wbr></wbr></wbr></wbr></wbr></wbr>

15.  假设有1000次100m短跑大赛，每次比赛的冠军成绩都在9.<wbr>7-10之间均匀分布，问期望有多少次比赛比赛能够破纪录</wbr>

A.  7
B.  10
C.  15
D.  32

<span style="color: #ffffff;">Answer: A. 这是所谓的破纪录问题。假设均匀分布,</span><wbr><span style="color: #ffffff;">则最后n次比赛之后这n个成绩形成一个排列。</span><wbr><span style="color: #ffffff;">第k次创纪录的概率是这个排列中第k个在前k-1个之前的概率，</span><wbr><span style="color: #ffffff;">也即1/k，所以n次比赛大约有1+1/2+1/3+…1/</span><wbr><span style="color: #ffffff;">n次破纪录，也即约为logn次。</span></wbr></wbr></wbr></wbr>

16. 在打桥牌的时候，如果你和对家共持有某门花色的9张牌，<wbr>则剩余的4张牌怎样分布的概率最大</wbr>

A.  2-2
B.  3-1
C.  4-0

<span style="color: #ffffff;">Answer: B. 可以简单计算得到这个结果。3-1的概率应该是50%。2-</span><wbr><span style="color: #ffffff;">2的概率是37.5%。4-0的概率是12.5%。</span><wbr><span style="color: #ffffff;">但是如果有奇数张，则最平均的就是最可能的</span></wbr></wbr>

17. 如果一个物体在3维随机游动，也即每一刻他可以向左，右，上，<wbr>下，前，后等概率的走，长久来看，则会发生什么情况</wbr>

A.  此物体无穷多次回到原点
B.  此物体无穷多次回到任何一条坐标轴上，但不会无穷多次回到原点
C.  此物体不会无穷多次回到任何一条坐标轴上

<span style="color: #ffffff;">Answer: B. 1维和2维的随机游动是常返的，也就是说会无穷多次回到起点（</span><wbr><span style="color: #ffffff;">尽管回来的平均时间不是有限的），</span><wbr><span style="color: #ffffff;">而3维以上的随机游动是非常返的。因此对于2维的某改革坐标，</span><wbr><span style="color: #ffffff;">此物体会无穷多次经过，但是不会无穷多次经过原点。</span></wbr></wbr></wbr>

18. 扔10000次硬币，其中最长一次连着正面的次数大约会是多少

A.  100
B.  13
C.  9
D.  4

<span style="color: #ffffff;">Answer: B.这也是一个特殊的概率问题，叫做Head Runs.答案应该是log_2^n.大约为13.</span>

19. 有一支股票，初始价为1，每天的价值变化率独立同分布，<wbr>且期望为0，不恒为0。则</wbr>

A.  股票在任何时刻期望价值为1
B.  股票以概率1变成0
C.  A和B都对
D.  A和B都不对

<span style="color: #ffffff;">Answer: C.这个可以参见我转载的文章The Flaw of Average和我写的文章Life is a Martingale.</span>
<span style="color: #ffffff;"> 也就是说对于很多投机的东西，平均值总是不变的，</span><wbr><span style="color: #ffffff;">但是多数人都会倾家荡产。其实仔细想想很有道理，</span><wbr><span style="color: #ffffff;">比如说你的股票第一天涨10%。第二天跌10%</span><wbr><span style="color: #ffffff;">或是第一天跌10%，第二天涨10%，最后的结果都是跌了1%。</span><wbr><span style="color: #ffffff;">所以要保持增长所需要的是远大于0的平均变化率，</span><wbr><span style="color: #ffffff;">这个才是一般人难以做到的。</span></wbr></wbr></wbr></wbr></wbr>

20. 当我们考虑一种可能重复发生的事件时，哪种方式更科学

A.  按照第一次发生这个事件的时间作为一个起点，<wbr>考虑从其本身出发之后的性质
B.  按照最后一次发生这个事件的时间作为一个起点，<wbr>考虑从其本身出发之后的性质
C.  以上都可以
D.  以上都不可以</wbr></wbr>

<span style="color: #ffffff;">Answer: A. 这个问题深一些的背景在于Kolmogorov向前向后微分方程</span><wbr><span style="color: #ffffff;">。很多人知道向后微分方程更通用，但是并不知道原因。事实上，</span><wbr><span style="color: #ffffff;">向后微分方程是基于A的方法对事件进行分解得到的，</span><wbr><span style="color: #ffffff;">而向前微分方程是基于B的方法对事件进行分解的。</span><wbr><span style="color: #ffffff;">但是有很多重复发生的事情会越发生越频繁，</span><wbr><span style="color: #ffffff;">以致没有最后一次发生的事件。</span><wbr><span style="color: #ffffff;">但是我们总能找到第一次发生的时间。所以A更科学。</span></wbr></wbr></wbr></wbr></wbr></wbr>

<strong>概率论感觉测试（二）</strong>

1、   100个球随机的放在100个箱子里，最后空箱子的数量大约是
A.  0-0.1(0)
B.  0.1-0.2(0)
C.  0.2-0.3(0)
D.  0.3-0.4(20)

<span style="color: #ffffff;">Ans：D.这个题可以用简单的概率论计算。</span><wbr><span style="color: #ffffff;">结论是不管多少个球，c*n个球放到n个箱子里，</span><wbr><span style="color: #ffffff;">最后空箱子的个数约为e^-c，</span><wbr><span style="color: #ffffff;">现在的情况是箱子数和球数一样多，那么就约为e^-1.</span></wbr></wbr></wbr>

2、  打10000副拱猪，总共持有9500-<wbr>10500个A的概率大约在
A.  80%-90%(0)
B.  90%-95%(0)
C.  95%-99%(0)
D.  99%以上(20)</wbr>

<span style="color: #ffffff;">Ans. D. 这个可以用中心极限定理计算。事实上这个题也不需要计算，</span><wbr><span style="color: #ffffff;">只是要考察大家的一个感觉，实际上这个概率大于0.99…9，</span><wbr><span style="color: #ffffff;">一共有9个9。不过有时候我们打牌仍然觉得牌总是很差。。</span></wbr></wbr>

3、  有以下几个国家，每个国家有自己的习俗。<wbr>问哪个国家长期以后男人最多
A.  每个家庭不断的生孩子直到得到第一个男孩为止(0)
B.  每个家庭不断的生孩子直到得到第一个女孩为止(0)
C.  每个家庭不断的生孩子直到得到一男一女为止(0)
D.  以上几个国家最后男女比例基本一样(20)</wbr>

<span style="color: #ffffff;">Ans. D. 我们只需要考察一个家庭最后产生多少男女即可以。</span><wbr><span style="color: #ffffff;">用概率的方法可以得到不管哪个方法都是1:1。事实上，</span><wbr><span style="color: #ffffff;">我们只是把一个很长的男女的序列按照不同的方式来截断。</span><wbr><span style="color: #ffffff;">当然这个序列本上包含多少男女是不变的。</span><wbr><span style="color: #ffffff;">我每次都愿意以另外一个例子来说明，那就是如果我们在网上下棋，</span><wbr><span style="color: #ffffff;">可以每天下到第一盘输为止或是第一盘赢为止或是有输有赢为止，</span><wbr><span style="color: #ffffff;">显然不管怎样，因为你的实力是恒定的，</span><wbr><span style="color: #ffffff;">你永远都是你本来应有的胜率。</span></wbr></wbr></wbr></wbr></wbr></wbr></wbr>

4、  实验室测试灯泡的寿命，在灯泡不断的换新灯泡。<wbr>灯泡寿命约为1小时。考察10000小时时亮着的那个灯泡
A.  那个灯泡的寿命期望也约为1小时(0)
B.  那个灯泡的寿命期望约为其他灯泡的2倍(20)
C.  那个灯泡的期望寿命约为其他灯泡的1/2(0)
D.  以上说法都不对(0)</wbr>

<span style="color: #ffffff;">Ans. B. 这个题可能是这5个题里面稍难的。</span><wbr><span style="color: #ffffff;">如果具体的算需要一点本科高年级的知识。</span><wbr><span style="color: #ffffff;">不过我们仍然可以从直觉得到结果。事实上，</span><wbr><span style="color: #ffffff;">当每个灯泡或是我们观测的事物的生命是随机的时候。</span><wbr><span style="color: #ffffff;">在时间足够久以后的一点，</span><wbr><span style="color: #ffffff;">那个事物的寿命要长于这个事物本身平均的寿命。</span><wbr><span style="color: #ffffff;">因为正是因为它寿命长导致我们容易观测到。简单的说，</span><wbr><span style="color: #ffffff;">如果灯泡有两种，一种只能坚持1小时，一种能坚持100小时，</span><wbr><span style="color: #ffffff;">那我们在后面观测到的99%都可能是100小时那个。</span><wbr><span style="color: #ffffff;">所以观测到的平均寿命较长。</span><wbr><span style="color: #ffffff;">通常我们认为灯泡的寿命是指数分布的，在这个情况下，</span><wbr><span style="color: #ffffff;">答案是2倍。对于一般的分布，甚至有可能平均寿命有限，</span><wbr><span style="color: #ffffff;">而观测的那个寿命期望是无限的。</span><wbr><span style="color: #ffffff;">这个问题在美国一次监狱调查中被发现，</span><wbr><span style="color: #ffffff;">即被调查的囚犯的平均判刑年数要远大于全美平均判刑的年数</span></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr>

5、  如果一个群体里，每个个体以0.2的概率没有后代，0.<wbr>6的概率有1个后代，0.2的概率有两个后代，则
A.  这个群体最后会灭绝(20)
B.  这个群体最后将稳定在一个分布，即种群大小在一定范围内震荡(<wbr>0)
C.  这个群体最后将爆炸，人口将到无穷(0)
D.  不一定会发生什么(0)</wbr></wbr>

<span style="color: #ffffff;">Ans: A. 这是个简单的人口模型。这个可能直觉比较困难，</span><wbr><span style="color: #ffffff;">但是这个实际上和上次的一道题是一样的。</span><wbr><span style="color: #ffffff;">注意到每一代的期望总是1。因此根据上次的答案，</span><wbr><span style="color: #ffffff;">这个群体最后会灭绝。对于这种模型，</span><wbr><span style="color: #ffffff;">当每一代的期望小于等于1时，最后的结果都是会灭绝。</span><wbr><span style="color: #ffffff;">对于期望大于1的情况，</span><wbr><span style="color: #ffffff;">我们也可以很简单的通过解方程得到灭绝的概率。</span></wbr></wbr></wbr></wbr></wbr></wbr>

<strong>概率论感觉测试（三）</strong>

1、1000枚硬币里有一个硬币两面都是国徽，<wbr>其他的硬币都是一面是国徽，一面是数字。<wbr>如果你从中选出了一个硬币，随机掷了10次，结果全部都是国徽，<wbr>问这个硬币是那个两面都是
国徽的概率大约有多大？</wbr></wbr></wbr>

A:   99%
B:   90%
C:   75%
D:   50%

<span style="color: #ffffff;">Answer: D.  这个问题是一个比较简单的问题，</span><wbr><span style="color: #ffffff;">只需要用Bayes公式计算一下即可。</span>
<span style="color: #ffffff;"> 但是人们有时候感觉这个概率比实际中的大。</span><wbr><span style="color: #ffffff;">类似的问题还出现在比如当你检测出来患有某种疾病的时候，</span><wbr><span style="color: #ffffff;">假设检测错误的概率只有千分之一，</span><wbr><span style="color: #ffffff;">但是如果那个患有那个疾病的人本身只有万分之一或者更少，</span><wbr><span style="color: #ffffff;">则你实际得这种病的几率也要比10%</span>
<span style="color: #ffffff;"> 要略少。另外的一个情况我在我的另外一篇日志&lt;&lt;Do say love to</span>
<span style="color: #ffffff;"> her&gt;&gt;中也提到了。总的来说，</span><wbr><span style="color: #ffffff;">人们通常更多的关注到了事情的变化，而忽略了一些事物的本质。</span></wbr></wbr></wbr></wbr></wbr></wbr>

2、三国杀游戏里周泰的技能是当没有血的时候，<wbr>可以从牌堆里抽取一张牌，如果和其前面的牌的数字都不同，<wbr>则可以继续活着；否则就死了。<wbr>假设牌堆里的牌是完全随机的一副扑克牌（52张一副牌），<wbr>问期望他大约一共要抽多少张牌才能死？</wbr></wbr></wbr></wbr>

A: 3-4张
B: 4-5张
C: 5-6张
D: 6-7张

<span style="color: #ffffff;">Answer.  C. 这个也没有什么算的技巧，</span><wbr><span style="color: #ffffff;">只需要把各种情况列举一下即可得到大约需要5.7张牌。</span></wbr>

3、接上题，如果玩家可以给周泰增加一个技能，叫做重生。<wbr>即在抽取第k张牌时如果这张牌和以前的牌数字相同，<wbr>则周泰获得满血。但是玩家必须在使用角色前声明k。<wbr>如果你是玩家，你会声明k为多少（仍然假设是52张的一副牌）？</wbr></wbr></wbr>

A. 4
B. 5
C. 6
D. others

<span style="color: #ffffff;">Answer: B. 与上题的计算方法一样，k为5的时候最优，大约有17%</span><wbr><span style="color: #ffffff;">的可能性可以获得重生。</span></wbr>

3、一位篮球运动员罚球100次。已知他前两个球罚中了一个。<wbr>从第3个球开始，<wbr>他罚每一个球的命中率为其前面所罚所有球的命中率，<wbr>比如他前50个球罚中了40个，则下一个球的命中率为80%。<wbr>问以下哪种情况发生的可能性较大</wbr></wbr></wbr></wbr>

A. 他最终罚中了50-60个球
B. 他最终罚中了60-70个球
C. 他最终罚中了70-80个球
D. 以上3个可能性一样

<span style="color: #ffffff;">Answer: D. 这个题也许有人会认为他要么罚中很多球，要么罚中很少球，</span><wbr><span style="color: #ffffff;">因为一旦开始罚中的多，则后面命中率会倾向于越来越高，</span><wbr><span style="color: #ffffff;">反之亦然。但是实际上这名运动员最后罚中1-</span><wbr><span style="color: #ffffff;">99个球的可能性都是相等的。简单的证明方法可以用数学归纳法。</span></wbr></wbr></wbr>

4、接以前的收集硬币问题。 美国共有50种25分的硬币，在上次的题中，<wbr>我们已经求过收集全他们所需要的大约次数（<wbr>假设每种硬币出现的概率相同）。<wbr>现在假设你已经收集了80枚硬币，你期望大约已经收集了多少种？</wbr></wbr></wbr>

A. 30
B. 35
C. 40
D. 45

<span style="color: #ffffff;">Answer: C. 上次我们问过期望需要集多少个才可以集齐，答案大约是200个。</span><wbr><span style="color: #ffffff;">实际上这个集的过程开始都是很快的，</span><wbr><span style="color: #ffffff;">大约在40个的时候就用将近30种，在80个的时候有40种，</span><wbr><span style="color: #ffffff;">而只有最后面几个需要很漫长的时间。这个公式是N-N(N-1/</span><wbr><span style="color: #ffffff;">N)^n,</span>
<span style="color: #ffffff;"> 其中N是一共要收集的数目，n为已收集的数目。</span></wbr></wbr></wbr></wbr>

5、假设在一根长为1米的绳子上随机的分布5只蚂蚁，<wbr>他们的位置和初始的方向都是均匀随机的。从时刻0开始，<wbr>他们朝着他们初始的方向以每分钟1米的速度开始爬，<wbr>直到离开绳子或者碰到另外一只蚂蚁。当他们碰到另外一只蚂蚁时，<wbr>两只蚂蚁会分别转向然后继续前进。<wbr>问期望大约多少时间之后所有蚂蚁都将离开绳子?</wbr></wbr></wbr></wbr></wbr>

A． 50秒
B．  1分钟
C．  2分钟
D． 5分钟

<span style="color: #ffffff;">Answer:  A. 从某种意义上来讲，这个题不能被认为是一道概率问题，</span><wbr><span style="color: #ffffff;">因为其真正的难度不在于概率。似乎看起来这道题完全无法计算，</span><wbr><span style="color: #ffffff;">因为你完全不知道每只蚂蚁的方向以及所处的位置，</span><wbr><span style="color: #ffffff;">但是关键在于注意到当两只蚂蚁碰面时，虽然实际中他们互换了</span>
<span style="color: #ffffff;"> 方向，但是从运动的角度来讲，</span><wbr><span style="color: #ffffff;">可以认为两只蚂蚁继续保持了前进但互换了代号。</span><wbr><span style="color: #ffffff;">所以这个题相当于在0-1之间有5个随机数，</span><wbr><span style="color: #ffffff;">问其中最大的期望是多少。这个数为5/6，</span>
<span style="color: #ffffff;"> 所以答案为A。</span></wbr></wbr></wbr></wbr></wbr></wbr>

6、两个人玩一个硬币游戏。在游戏之前，<wbr>第一个人选择一个长度为3的序列，比如说“国徽，国徽，数字”，<wbr>在第一个人选择之后，另外一个人选择另外一个序列（<wbr>必须是不同的）。
在两个人都选定序列之后游戏开始。两个人反复掷硬币，<wbr>直到一个人所选择的序列出现为止。出现所选择此序列的人获胜。<wbr>问先选择的人如果做出最正确的选择大约可以有多大的可能性获胜？</wbr></wbr></wbr></wbr></wbr>

A.      30%
B.      50%
C.     70%
D.     90%

<span style="color: #ffffff;">Answer: A.  也许有些人会对这个答案感到有些吃惊。先选的人居然如此吃亏。</span><wbr><span style="color: #ffffff;">因为人们可能会认为，在这些序列中，有一个最优的序列，</span><wbr><span style="color: #ffffff;">它出现的平均时间最早。这确实不错，但是序列之间不是独立的，</span><wbr><span style="color: #ffffff;">也就是说如果A比B好，B比C好，并不一定能保证A比C好。</span><wbr><span style="color: #ffffff;">比如第一个人选了“国徽，国徽，数字”这个序列，那我选择“</span><wbr><span style="color: #ffffff;">数字，国徽，国徽”</span><wbr><span style="color: #ffffff;">就可以保证在他这个序列出现之前的那3个情况中，我大约有1/</span><wbr><span style="color: #ffffff;">2的概率可以获胜（也即在这个序列之前的那次硬币为数字即可）。</span><wbr><span style="color: #ffffff;">这个题只能用Markov链去计算任何两个序列对抗时分别的获胜</span><wbr><span style="color: #ffffff;">率，然后用博弈论的方法去求解。对于第一个人来说，</span><wbr><span style="color: #ffffff;">最佳的选择可使他有1/3的概率获胜。</span></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr>

7、 假设有100个人排队买一个5块钱的电影票，<wbr>其中50个人只有5块钱，50个人只有10块钱。<wbr>问电影院在整个过程中一直可以找开钱的可能性大约有多大？（注：<wbr>这和在之前的测试中的台湾大选问题有一定的类似之处，<wbr>但并不相同）</wbr></wbr></wbr></wbr>

A. 1%
B. 2%
C. 5%
D. 10%

<span style="color: #ffffff;">Answer: B. 在上一系列的概率论感觉测试的题目中，我们问在整个过程中，</span><wbr><span style="color: #ffffff;">某一方一直领先另一方的概率。这个题只要求一方（有5块钱的人）</span><wbr><span style="color: #ffffff;">不落后另外一方（有10块钱的人）。</span><wbr><span style="color: #ffffff;">这个的算法是需要用brownian</span>
<span style="color: #ffffff;"> motion的reflection</span>
<span style="color: #ffffff;"> principle。实际上的比例为从0开始每一步为-1,</span><wbr><span style="color: #ffffff;">1运动最后停到-2的路径数除以停到0的路径数，为1/51.</span></wbr></wbr></wbr></wbr>

8.  假设你掷一枚硬币，<wbr>问你期望需要掷大约多少次才能获得连续10个正面？</wbr>

A. 100 次
B. 500 次
C. 1000 次
D. 2000 次

<span style="color: #ffffff;">Answer: D. 在上一系列的概率论感觉测试中，</span><wbr><span style="color: #ffffff;">我们说掷n次大概连续证明的数量为log_2^n.</span><wbr><span style="color: #ffffff;">现在问的是要获得一定量的正面，需要掷多少次。</span><wbr><span style="color: #ffffff;">结果比较接近但是仍然不是很相同，准确的数字为2^(k+1)-</span><wbr><span style="color: #ffffff;">2，也就是2046次。简单的证明方法可以用数学归纳法。</span><wbr><span style="color: #ffffff;">而比较推荐学过martingale的同学用martingal</span><wbr><span style="color: #ffffff;">e的方法证明：假设每一时刻有1个人来赌，如果正面，</span><wbr><span style="color: #ffffff;">他的资金翻倍，否则就为0；当连续出现10个正面的时候，</span><wbr><span style="color: #ffffff;">所有来赌的人的钱为2046。根据Optional</span>
<span style="color: #ffffff;"> Stopping Theorem, 所需要时间的期望也是2046。</span><wbr><span style="color: #ffffff;">Martingale方法的好处是可以计算达到任何序列所需要的</span><wbr><span style="color: #ffffff;">时间。</span></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr>

9．赌场里有这样一个游戏：你掷一枚色子。在任意时刻，<wbr>如果6从来没有出现，你可以选择获得你所掷出的总点数或者继续；<wbr>若6出现，则游戏结束，你获得0块钱。（比如，你掷出了2，3，<wbr>5；则你可以选择立刻获得10块钱或继续，<wbr>但是如果你下次掷出6你就什么都没有了，<wbr>如果是其他你还可以继续）问这个游戏你的平均收益大概是多少（<wbr>换句话说你愿意付多少钱去玩一次这样的游戏）？</wbr></wbr></wbr></wbr></wbr></wbr>

A. $4
B. $6
C. $8
D. $10

<span style="color: #ffffff;">Answer: B. 这个题需要用动态规划进行计算。</span><wbr><span style="color: #ffffff;">这种动态规划在任何管理和金融的应用中都非常常见。</span><wbr><span style="color: #ffffff;">准确地值大约为$6.15.</span></wbr></wbr>

10. 假设一个飞机上有100个座位。<wbr>100名乘客中第一名乘客喝醉了酒，<wbr>就随机在飞机上找了一个座位坐下。<wbr>其他的乘客如果自己的座位没有被占，则会坐在自己的座位上，<wbr>否则也将在剩余的座位上随机的找一个座位。<wbr>问最后一名乘客坐在自己座位上的概率有多大？</wbr></wbr></wbr></wbr></wbr>

A．50%
B．10%
C．5%
D．1%

<span style="color: #ffffff;">Answer: A. 这个题应该算比较经典的一道题目，</span><wbr><span style="color: #ffffff;">但是并不能算是一道纯粹的概率题。</span><wbr><span style="color: #ffffff;">这种类似于脑筋急转弯的题目需要人们能注意到一些简化的方法。</span><wbr><span style="color: #ffffff;">思考的方法大约如下：对于第一名乘客，</span><wbr><span style="color: #ffffff;">如果他恰好坐在自己的座位上，</span><wbr><span style="color: #ffffff;">则最后一名乘客肯定也能坐在自己的座位上，</span><wbr><span style="color: #ffffff;">如果他恰好坐在了最后一名乘客的作为上，</span><wbr><span style="color: #ffffff;">那最后一名乘客无论如何也无法坐在自己的位子上，</span><wbr><span style="color: #ffffff;">而这两个概率是相等的；对于其他情况，</span><wbr><span style="color: #ffffff;">如果他坐了第k个乘客的座位，则从第2到第k-1个乘客，</span><wbr><span style="color: #ffffff;">他们都会坐在自己的位子上，问题变相当于飞机一共有101-</span><wbr><span style="color: #ffffff;">k个座位，第一个乘客（原来的第k个）随机选一个座位。</span><wbr><span style="color: #ffffff;">这样递归下去可以得到不管有多少座位，以上的问题的概率都是1/</span><wbr><span style="color: #ffffff;">2。</span></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr></wbr>

（答案Ctrl+a可见）

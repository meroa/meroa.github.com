---
layout: post
title: 标准建模流程之样本选择
date: 2011-10-04 14:52
comments: true
categories: []
---
<p align="left">建模过程中，一个好的通用性模型对建模样本就有一定的要求：</p>
<p align="left">1)   样本个数:</p>
<p align="left">作为建模样本，首先涉及样本个数的问题。样本个数应根据各项因子的变动范围和精度要求、置信程度按照数理统计原理确定。一般来说，当所研究的现象越复杂，差异越大时，样本量要求越大；当结果的精度要求和置信程度要求越高时，样本量要求越大。比如，对于精度要求为beta以下的，样本量应不少于F(beta)， F是依据某种原则写下的样本个数关于精度要求的函数，一般情况下可默认F服从高斯分布函数。</p>
<p align="left">2)   样本维度:</p>
<p align="left">模型样本维度应考虑横截面数据及时间序列数据2个维度。在建模过程中，考虑合适的等效时间窗宽内，对横截面数据进行精确的建模。</p>
<p align="left">3)   样本构成:</p>
<p align="left">样本资料的收集是建模的首要环节，其质量好坏直接影响建模效果。样本构成是指样本个数的分布情况，它涉及每一个子样本中具体建模样本的选取。选取时应掌握如下原则：最小、中等和最大者必选，然后再在其间适当增选；目标变量变化规律未知时考虑等距均匀分布，变化规律已知时宜典型选取，但其中变曲率点必选。在我们模型中，应按照时间、地区、行业等维度区分，不同维度上的数据应该同时收集，数据量过大时应采取分层随机抽样方法，必要时也可考虑分别建模。</p>
<p align="left">4)   校验样本:</p>
在建立通用性模型时，一般要求在收集训练样本的同时，还需另收一套校验样本。同时收集训练和校验两套样本，前者作为训练集，后者作为校验集：用训练集样本建模，用校验样本检验所建模型的精度。校验集样本的收集原则和方法应该与训练集样本相同，也就是说，校验集样本与训练集样本无论在分布空间还是同一分布的参数空间都是一致的。如果采集阶段没有刻意区分训练集和校验集，那么可以将总样本按照需求合理拆分为训练集和校验集。当样本足够多时，可以将数据分成三份。训练集：估计模型的参数；校验集：估计模型的预测误差；测试集：计算最终选定的模型的泛化误差。但通常没有足够多的样本，而且也很难说明究竟多少数据是足够的，因此模型的好坏十分依赖于基础数据的信噪比和模型的复杂程度。
<table width="431" border="0" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td valign="top" width="216">
<p align="center">训练集</p>
</td>
<td valign="top" width="108">
<p align="center">校验集</p>
</td>
<td valign="top" width="108">
<p align="center">测试集</p>
</td>
</tr>
</tbody>
</table>
<p align="left">5)   校验是校验模型是否可接受而非模型泛化误差（预估误差）:</p>
<p align="left">    整个校验行为并不能提出一个反映所建模型泛化误差（泛化误差基于测试集，简单来说就是预估误差）的指标值，而只是作出一个可否接受模型的判定。可以推断，只要建模样本的收集符合要求，就基本上能以(1-α)的概率作为接受模型的判定，也即作出否决模型的判定只是一个小概率事件。万一真是出现此种情况，也只能按要求去完善样本资料重新建模。因此，与其花费一部分工作量去收集校验样本，还不如在收集训练样本时多花点功夫以确保其质量。真正体现模型预测精度的，主要还是预估误差这一指标。</p>
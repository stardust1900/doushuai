---
title: CH2-捕获点子
description: fishing of ideas
author: 王一刀
categories: [量化交易]
---

## 从何处获取策略

> This is the surprise: Finding a trading idea is actually not the hardest part of building a quantitative trading business. There are hundreds, if not thousands, of trading ideas that are in the public sphere at any time, accessible to anyone at little or no cost. Many authors of these trading ideas will tell you their complete methodologies in addition to their backtest results. There are finance and investment books, newspapers and magazines, mainstream media web sites, academic papers vailable online or in the nearest public library, trader forums, blogs, and on and on.

你可能会奇怪：寻找交易点子不是建立量化交易事业最难的部分。在公共领域有成千上万的交易点子，任何个人任何时间都可以免费或者用一点点花费就能获取到。很多交易点子的作者，不仅会完全告诉你实现的方法，还会附上他们的回测结果。有很多金融投资的书籍，报纸，杂志，主流媒体的网站，在线的学术期刊，或者最近的公共图书馆，交易者论坛，博客等等。

| 类型 | 网址 |
|-|-|
| **Academic** |  |
| Business schools’ finance professors’ websites | [www.hbs.edu/research/research.html](http://www.hbs.edu/research/research.html) |
| Social Science Research Network | [www.ssrn.com](http://www.ssrn.com) |
| National Bureau of Economic Research | [www.nber.org](http://www.nber.org) |
| Business schools’ quantitative finance seminars | [www.ieor.columbia.edu/seminars/financialengineering](http://www.ieor.columbia.edu/seminars/financialengineering) |
| Buttonwood column in the Economist magazine’s finance section | [www.economist.com](http://www.economist.com) |
|**Financial web sites and blogs**  |  |
| Yahoo! Finance | finance.yahoo.com |
| TradingMarkets | www.TradingMarkets.com |
| Seeking Alpha | www.SeekingAlpha.com |
| TheStreet.com | www.TheStreet.com |
| The Kirk Report | www.TheKirkReport.com |
| Alea Blog | www.aleablog.com |
| Abnormal Returns | www.AbnormalReturns.com |
| Brett Steenbarger Trading Psychology | www.brettsteenbarger.com |
| 本书作者 | epchan.blogspot.com |
| **Trader forums** |  |
| Elite Trader | www.Elitetrader.com |
| Wealth-Lab | www.wealth-lab.com |
| **Newspaper and magazines** |  |
| Stocks, Futures and Options magazine | www.sfomag.com |

> No, the difficulty is not the lack of ideas. The difficulty is to develop a taste for which strategy is suitable for your personal circumstances and goals, and which ones look viable even before you devote the time to diligently backtest them. This taste for prospective strategies is what I will try to convey in this chapter.

困难不是缺少点子。困难是培养出一种敏锐的嗅觉，能分辨出哪些策略是适合你的环境和目标的，并能在对策略进行回测前发觉其是否可行。这种预见策略的嗅觉正是我要在本章试图阐明的。

## 如何辨别策略是否适合你

有如下几个评判依据：
* 你的工作时间
* 你的编程技能
* 你的交易资本
* 你的目标


## 识别可用的策略及其陷阱

用这些方法快测试策略，确保你不会浪费你的时间和金钱

* 这个策略和基准比较表现如何?它的回报有多持久?
> Though a strategy may have the same average return as the benchmark, perhaps it delivered positive returns every month while the benchmark occasionally suffered some very bad months. In this case, we would still deem the strategy superior. This leads us to consider the information ratio or Sharpe ratio (Sharpe,1994), rather than returns, as the proper performance measurement of a quantitative trading strategy.

虽让一个策略可能和基准有相同的回报，但在基准下跌的月份里它仍然有正收益。我们仍然认为这个策略是优越的。这促使我们考虑用信息比率或者夏普比率，而不是回报来，作为衡量量化交易策略业绩的指标。


> $ Information Ratio = \frac {Average of Excess Returns}{Standard Deviation of Excess Returns}$ 

$ 信息比率 = \frac {超额收益率的均值}{超额收益率的标准差}$


(其中：超额收益率 = 组合收益率 - 基准收益率)


> As a rule of thumb, any strategy that has a Sharpe ratio of less than 1 is not suitable as a stand-alone strategy. For a strategy that achieves profitability almost every month, its (annualized) Sharpe ratio is typically greater than 2. For a strategy that is profitable almost every day, its Sharpe ratio is usually greater than 3.

一般来说，任何夏普率小于1的策略不适合作为单独策略。对于每月都有收益的策略，它的年化夏普率通常大于2.对于每天有收益的策略，他的夏普率通常大于3.

* 下挫有多深多久？

你要问自己，你能承受多深多久的下挫而不清算你的投资组合关闭你的策略。

* 交易成本如何影响策略？

交易成本不仅包括券商收取的佣金，还有流动成本和机会成本。

* 数据是否存在生存者偏差

历史数据库中的股票报价不包含破产退市的股票。

* 为什么策略的业绩过几年会发生改变？

策略回测要关注近几年的表现，久远的数据会包含交易成本和幸存者偏差的影响。

* 策略是否收到数据范围偏差影响？

策略含有过多参数可能会对历史数据产生过度拟合。

* 策略是否在基金经理的盲区

> you should look for those strategies that fly under the radar of most institutional investors, for example, strategies that have very low capacities because they trade too often, strategies that trade very few stocks every day, or strategies that have very infrequent positions.

你应该去寻找被机构投资者忽视的策略，比如，交易频繁容量很低的策略，每天只交易很少股票的策略，持仓时段稀少的策略。这样的特色策觉才有利可图，因为他们还没有完全被巨型的对冲基金套利掉。



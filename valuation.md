## 35. Introduction to Valuation
## 35. 估值简介
1 分钟
了解了财务建模后，我们可以继续讨论估值。到本节的最后，您将对增长估值和价值估值的方法以及估计的的最佳实践有更全面的了解。我们将研究如何在用几种不同的方法估值：市盈率、市销率和现金流贴现。因为
第一：不同类型的投资者对公司的估值方式也不同。在为公司定目标价格时，一个价值投资者就不会像增长投资者那样对公司进行估值。
第二：不同的估值方向中，有一个会是错的，但我不知道是哪一个。但是，如果如果我们用三种不同的方法进行估值并取平均值，可以将错误最小化。
我将深入讨论增长估值与价值估值。我们将比较通用和特斯拉，他们是典型的价值型公司和成长型公司。

## 36. More Detail on Growth Versus Value and P/E + P/R + DCF Overview
## 36. 基于成长性的估值 vs 基于价值的估值及P/E + P/R + DCF概述
4 分钟
这是我最喜欢的估值部分。我们首先需要知道自己是哪种类型的投资者，有及我们的客户是哪种类型的投资者，这经常会有非常大的差异。我们来看两个真实的例子。
![](https://i.loli.net/2020/05/14/WE6lOCtkhzXVju1.jpg)

通用电气在天平的一端，特斯拉则在另一端。通用电气是为价值投资者服务的，这意味着投资者希望买相对便宜的股票，并获得股息收益。另一端的特斯拉，它适合成长型投资者，而成长型投资者则热衷于那些高速成长的公司，他们不需要这些公司今天就盈利，他们希望公司雇用很多销售人员来迅速增加营收，然后在很多年后的某一天可以盈利，例如亚马逊。你需要知道你是哪种类型的投资者是。价值投资者的典型代表就是沃伦·巴菲特先生。因此，你需要知道你在上的位置。有些人在天平的中间，有时他们被称为GARP(growth at reasonable price)。他们既不是完全的价值投资者，中也不是完全的成长型投资者，他们需要以合理的价格增长。所有增长投资最终都会变成价值投资。多年来微软一直是令人难以置信的增长投资对象，然后他进入炼狱般的十年。既不是增长型，也不是价值而是停滞在中间。现在他终于更像一个价值投资对象了。被卡在中间的股票永远都不值得投资。

下面这张图是我们的最后产出，暂时不用陷进去。我只想告诉大家，在本节中我们将要介绍三种不同的估值方法。首先是价格市销率分析，这是针对没有盈利的公司，显然增长型投资者喜欢它。第二种是市盈率分析，这是我的最爱。最后是所谓的现金流贴现，这是价值投资者所喜欢的。如果愿意，我们可以看到无数种不同类型的估值方法, 如市净率（price to book ratio）估值法，企业价值/EBITDA乘数估值法等。
![](https://i.loli.net/2020/05/14/d4kVbirXzfUM3oq.jpg)


暂时只看上面的三种。市销率估计法是成长型投资者喜欢的一个指标。这对于尚未盈利的公司而言非常有价值，也适合用来和同类公司做比较，尤其是那些还没有盈利的公司。市盈率估值法对评估相对利润增长率确很有用。成长型投资者喜欢市销率。然后是市盈率估值法，这可以用来计算相对的利润增长率，这称被为本益成长比或动态股份收益比（PEG比）。因此，如果一家公司的利润增长了10％，且市盈率是10倍，PEG比率就1。如果市盈率是20倍，那PEG比例就是2。如果一家公司的收入增长率为10％，市盈率是20倍，那么PEG是2。成长型投资者和价值投资者都喜欢PE。然后最后一个是现金流贴现。这里的现金是关键，这种估值法是要估计公司未来的盈利在今天值多少钱，因此我们需要把未来的利润贴现到今天。价值投资者喜欢DCF，而成长型投资者则不喜欢。因此，我们要做的实际上是获取所有这三种方法的平均值，以得出我们的目标价格。市销率定价 + 市盈率定价 + 现金流贴现定价 / 3，就是我们的目标定价，而我之所以选择至少三种不同的估值方法（投资银行对在IPO时经常这样做），是因为存在误差率。您的估值会有误差，但是你不知道是哪一个，这样做可以让减少总体的误差率。

## 37. 25 Valuation and Modeling Best Practices
## 37. 25条建模和估值的最佳实践
1 分钟
见resources文件夹“ModelingAndValuationBestPractices.pdf”

# 第 10 节： Valuation Part 2 of 6: Discounted Cash Flow (DCF)
# 第 10 节： 估值6-2：贴现现金流（DCF) 
2 / 7|55 分钟

## 38. What is DCF, Why is it Important and How Does it Work?
## 38. 什么是DCF(贴现现金流), DCF为何重要？如何运行？
6 分钟
让我们谈谈现金流量折现或DCF估值。在本节中，您将了解DCF，以及为什么他对公司进行估值很重要以及整个过程是怎样的。

举个简单的例子假设今天我们有5块钱，而10年后也有5块钱。那年10年后的这5块钱，在今年值多少钱呢。如果我们假设年化的利率7％，我们就可以把10年后的5块钱，折成到今天用以下公式表示。
$$  未来的现金 \div (1 + 利率\%)^{时间} $$

以5块钱为例，10年后的5块钱，如果利率是7%则，$  5 \div (1 + 7\%)^{10} = 2.54 $


先忽略这个，我们接下往下说。我们每年能赚到口袋里的钱是多少？我们知道净收入减去我买东西的的钱是我们每年赚到口袋里的钱。拿公司来说就是 
$$ 净收入 - 对自己公司进行投资的钱 $$
也可以说是 $ 净利润 - 厂房和设备 $ 或者 $ 净利润 - 资本支出 $

回顾一下，之前我们说：
$$ 净利润 + 非现金支出 = 运营现金流 $$
$$ 运营现金流 - 资本支出 = 自由现金流 $$

因此，每年我们赚到口袋里的现金等于营业现金流（即现金流量表的第一部分减去资本支出）减去资本支出。也即自由现金流。
![](https://i.loli.net/2020/05/15/7Ppy8rlKIGUY3as.jpg)

看看怎么和折现结合起来。前面我们讲过怎么把10年后的5块钱折现到今天。我们要对linkedin未来每年的自由现金流都做一样的事情，这是也我们为公司估值的方法。我们把一家公司未来的现金流，都折现到今天，就是公司的价值。我们看下图。Excel里我们有一个NPV(净现值)公式，输入折现率和需要折现的年份的单元格，就可以计算这些年份的钱折现到今天的价值。拿我们的linkedin的模型看，未来4年的自由现金流，折现到今天，总共就是20.98亿元。
![](https://i.loli.net/2020/05/15/6JyRbEkUWjX49Iw.jpg)



## 39. Calculating the Terminal Value
## 39. 计算终值
3 分钟
从上一堂课的基础开始，上次我们计算了NPV（净现值)。但我们的自由现金流，在模型上只预测到2020年，我们认为这是个五年周期的模型。但企业的经营是持续的。这时候我们要怎么办呢？这就要引出“终值”的概念了。终值的计算比我们想的要容易。有以下几个要素：
1. 利率，在我们的例子里是7%。这里要注意的是，我们这个例子中的“利率”指的是这家具体公司的利率，通常要高于政府的利率。
2. 长期的增长率，我们假设是2%。不要去假设一家公司可以以高于1%、2%、3%的速度无限增长。看一下美国经济，他像是一个大公司，他GDP占全球的25％，但增长无法超过几个百分点只是因为它很大。因此，大公司的成长并不十分迅速。因此，长期增长通常为1%或2%，最好的情况是3%。
我们的终值公式如下：
$$ 终值 = 最后一年的自由现金流 \times (1 + 长期增长率) \div (利率 - 长期增长率)$$
你可能会问，如果长期增长率高于利率怎么办？这个基本上不可能，因为利率不可能永远像今天这些操持在这么低的水准，利率通常要高得多，并且长期增长率不会太高。我们代入公式$ 1110.4 \times (1+0.02) /div (0.07 - 0.02) = 22652 $。最后还有一小步，我们需要把终值折现到今天，如何折现，我们已经知道如何做了。

## 40. Calculating the Weighted Average Cost of Capital (WACC)
## 40. 计算加权平均资本成本 (WACC)
6 分钟
到这里，DCF其实差不多完成了。不过，还有一件重要的事是利率。之前我们用了7％，这是个假设。接下来我们需要计算利率，这也被称为加权平均资本成本(WACC)。之前7%的利率，我称其为折现率。因此，现在我们提到了WACC，折现率也称为WACC。从现在开始，当我们谈论利率时，他们与贴现率是一回事，也就是是WACC，加权平均资本成本。那么加权平均资本成本如何计算呢?
$$ W.A.C.C = 公司的债务成本 + 公司的股权成本$$
别担心，我们后面会详细解释。拿公司使用债务的成本，然后将其乘以将要使用这笔债务的资本占总资本的百分比。资本不是债务就是权益。所以公式变成下面这样。这里我们考虑了税率，因为当我们负债时我们同时享受了税收的优惠。
$$  W.A.C.C. = 债务成本 \times (1 - 税率） \times 债务比重 + 股权成本 \times 股本 $$

然后我们假设我们的资产负债率（债务比重）是40%，股本占60%，税率是30%（税率不用计算，直接问这家公司，或者使用财报中的历史税率），我们假设银行贷款的利率是5%。这样对负债部分，也就是公式的前一半，我们可以代入 $ 5\% \times (1 - 30\%) \times 40\% = 1.4\% $ ，1.4%是我们的负债部分。

接下来我们重点看看如何计算股权成本。

$$股权成本 = 60\% \times 最低利率 + 股价的相对市场的波动性相 \times (我们认为股票市场的表现 - 最低利率)$$

我们补充并简化一下。
$$股权成本 = 60\% \times 无风险利率 + beta \times (股票市场平均收益率 - 无风险利率)$$
最低利率实际上是无风险利率，一般就是央行的利率，我们可以用1%、2%、3%。我们用2.5%。然后是股份相对市场的波动性，这被叫做Beta。Beta是什么呢，Beta用户衡量你正在分析的股票，相对于市场的走势。让我们看一个例子，下图的横轴是时间，纵轴是股价。白色的曲线是标准普尔500指数，我们认为他的beta是1。然后再画上我们的股票的走势，有很大的波动，说明这确实是一家比较高风险的公司。我们的波动性是市场的两倍，这可以股价随x轴的移动在y轴的波动率和市场比较来计算。在这个例子中，我们的股票的beta就是2。一般我们可以从一些免费的数据源得到beta值，我们甚至可以自己来计算，不过不太值得。
![](https://i.loli.net/2020/05/17/gbM3sUQpY4NiX2O.jpg)
因此我们会把2代入公式的beta中。如果我们的股票波动性没那么大，比如说是0.8，那么他们降低我们整体的股权成本成本。可见我们考虑了市场的波动性。接下来是“我信认为股票市场的表现”，这其实值得讨论一下，坦率讲我不是DCF的拥趸，因为这里面有太多的独立变量。比如这里股票市场平均收益率，我们就定一个8.5%，全部代入得到
$$2.5\% + 2 \times (8.5\% - 2.5\%) = 14.5\% $$

这就是我们的股权成本，14.5%，这其实挺高的，非常高。当然如果我们的beta小一些（即我们的股票的波动性要低于市场），那我们的股权成本会低很多。然后代入完整的WACC公式，最后得到我们的WACC为10.1%，也就是我们的折现率，或者说利率，都是一回事。
 $$ 14.5\%（股权成本） \times 60\%（股本占比） + 1.4\%(债务成本 \times 债务占比） = 10.1\% $$

我们已经介绍了如何计算自由现金流、终值以及加权平均资本成本（WACC），我们接下来就可以看一下DCF估值。我们会用LinkedIn为例子，在下一节中进行介绍。

## 41. DCF Example
## 41. 贴现现金流案例
8 分钟
回到我们的模型，我们来进行DCF估值。在现金流量表的最下面，我们计算出来了自由现金流。让我们看一下贴现现金流的计算。
###**第1步**、获取自由现金流
从现金流量表中获取自由现金流，如下图。
![](https://i.loli.net/2020/05/17/cVfKLWRgFy5JvCH.jpg)

###**第2步**、计算所谓的加权平均资本成本(WACC)
即我们将用来折现这些自由现金流量的折现率。这些自由现金流在今天（2016）的价值应该比他们在体现在报表上未来的价值要低，因为有利率，我们需要支付利息，因此我们需要将这些自由现金流折现。但是折现的利率应该是多少呢？这里我们要考虑两件事。股权成本和债务成本。
#### **第2.1步**、讲股本成。
公式如下图，我们上一节介绍过。无风险利率基本上是政府利率（国债利率？）。beta是linkedin股票相对市场的波动，是0.95，这表示他比S&P500指数波动更小，股市长期回报率假设是8.5%。因此股权成本计算得到8.2%。然后回到上面的图，我们还需要知道股本占市值的比重，linkedin的市值大约是159亿，资产负责表中的负责是11.3亿。因此股本的占比是 159 / (11.3 + 159) = 93.4%，债务的比例就是6.6%。

$$\begin{split} &股权成本 \\ &= \\&无风险利率 \\&+ \\&beta \times (股票市场长期收益率 - 无风险利率) \\&= \\&2.5\% \\&+ \\&0.95 \times(8.5\% - 2.5\%) \\&= \\&8.2\%
\end{split} $$

![](https://i.loli.net/2020/05/17/d3ICG1TynAMU8wq.jpg)



####**第2.2步**、债务成本。
基本上是债务本身的成本（贷款利率）减去税收，因为我们确实通过债务得到了税收优惠，这从税收的角度来看的。不过从模型的注释我们看到，linkedin的所有债务都是可转债（可以被转换为股权）。因此，我假设债务成本与股权成本相同，即8.2％。这样我们就计算得到负债成本是5.5%

$$\begin{split}&债务成本 \\&= \\&负债成本 \times (1 - 税率）\\&= 8.2\% \times (1   - 0.33) \\&= \\&5.5\%
\end{split}$$
![](https://i.loli.net/2020/05/17/OHIFqTShGAUdrkt.jpg)

回到上面的公式, 把我们计算出来的各项代入， 即可得到下面的结果，得到了8.02%。这就是我们的资金成本，我们将用它来作为上面所有自由现金流的折现率。

$$\begin{split} &加权平均资本成本(W.A.C.C)  \\&= \\&股权成本 \times 股本占市值比重 \\&+ \\&负债成本 \times 负债占市值比重 \\&= \\&8.2\% \times 93.4\% \\&+ \\&5.5\% \times 6.6\% \\&= \\&8.02\%
\end{split}$$

###**第3步**、我们开始折现。
我们用Excel的NPV公式，我太喜喜欢他了。 
$$ 净现值 = NPV(8.02\%, \$296,\$410,\$756,\$1110,\$1547) = \$3092 $$
![](https://i.loli.net/2020/05/17/54zyfv8OWlr2whi.jpg)

然而2021年及以后的自由现金流怎么办？我们必须得考虑他们，并且要占不小的比重，因为我是linked未来N年的自由现金流。

###**第4步**、计算终值。
2020年的自由现金流是$1547我们先选一个长期增长率，大公司的长期增长率一般不会太高，1%，2%，3%最多。我们这里就取2%, 然后WACC已经计算好了，8.02%，代入以后就得到了终值$26207。然后我们要把终值也折现到现在。公式如下。
$$\begin{split}
\\终值 &= \$1547 \times \frac {(1 + 长期增长率)} { (WACC - 长期增长率) }  \\&= \$1547 \times \frac{(1 + 2\%)}  {(8.02\% - 2\%)} \\&=\$26207 \\折现终值 &= \frac{终值} {(1 + W.A.C.C) ^ 4}\\&=\\&=\frac{\$26207}{(1 + 8.02\%)^4}\\&=\$19247\end{split}$$
![](https://i.loli.net/2020/05/17/3JQoucxEfeWOUdz.jpg)


###**第五步**、计算目标价格
**倪焱石注** 由于采用的是自由现金流，因此净现值 + 折现终值算出来的结果中是公司的价值，不是股权价值，算股价的时候，还是要减去负债(从资产负债表里找）。
拿前面4步的结果，再从资产负债表里找出长期负债的值，结合下面的公式 ，就可以计算出来目标股价了。
$$\begin{split}
目标公司价值 &= 净现值 + 折现终值 \\&= \$3092 + \$19247 \\&= \$22340\\
目标股坐 &= \frac{目标股权价值}{股数} \\&= \frac{(目标公司价值 - 负债)}{股数}\\&=\frac{(\$22340 = \$1127)}{134.91}\\&=\$154.27
\end{split}$$

![](https://i.loli.net/2020/05/17/FlCQNEdjaTLqPn3.jpg)
###**额外步骤**###敏感性分析
看下面的图，我们的目标价格是基于长期增长率在2%，WACC在8.02的基础上计算出来的。这是我们的基准值。这个表格被称为敏感分析表，很多分析师会使用这个表格。这样我们可以在给客户展示时，按未来是熊市或者牛市的不同预期，计算出不同的价格。在这个表格中，如果我们认为未来经济向好（牛市），那么长期增长率可以算成3%，WACC可以低到6%，这样我们可以得到左下角的目标价格，$328。如果我们比较悲观（熊市），右上角的linkedin的股价就只有$101（增长率1%，WACC到10%）。 
![](https://i.loli.net/2020/05/18/7H2vqKwYg43JfDu.jpg)
这三个价格会体现在我们最终的估值指标的Sheet中（如下图的25~28行）。
![](https://i.loli.net/2020/05/18/wrMBLQyj7AmVaHf.jpg)



## 42. DCF Exercise
## 42. 贴现现金流习题
2 分钟

## 43. DCF Exercise Answer Explanations Part 1 of 2
## 43. 贴现现金流习题解析 2 - 1
19 分钟

## 44. DCF Exercise Answer Explanations Part 2 of 2
## 44. 贴现现金流习题解析 2 - 2
11 分钟
# 第 11 节： Valuation Part 3 of 6: Price to Revenue
# 第 11 节： 估值6 - 3：价格 / 营收 (市销率）
0 / 4|9 分钟

## 45. What is Price / Revenue and Why Do We Need to Base a Target Price on this Ratio?
什么市销率，为什么需要基于市销率来确定目标价格？
2 分钟

## 46. Price to Revenue Example
## 46. 市销率案例

2 分钟

## 47. Price to Revenue Valuation Exercise
## 47. 市销率估值习题
1 分钟

## 48. Price to Revenue Exercise Answer Explanations
## 48. 市销率估值习题qes
5 分钟
# 第 12 节： Valuation Part 4 of 6: Price to Earnings & Additional Valuation Methodologies
# 第 12 节： 估值 6 - 4：市盈率及其他估值方法
0 / 5|13 分钟

## 49. Introduction to P/E and Why it Matters
## 49. 市盈率介绍及其重要性
3 分钟

## 50. Price to Earnings Example
## 50. 市盈率案例
2 分钟

## 51. Price to Earnings Valuation Exercise
## 51. 市盈率估值习题
1 分钟

## 52. Price to Earnings Exercise Answer Explanations
## 52. 市盈率估值习题解析
6 分钟

## 53. Additional Valuation Methodologies
## 53. 其他估值方法
2 分钟
# 第 13 节： Valuation Part 5 of 6: Final Target Price Calculation & "TAM Sanity Check"
# 第 13 节： 估值6-5：最终目标价格及TAM（潜在总市场规模）一致性验证
0 / 1|1 分钟

## 54. Our Final Price Target Calculation
## 54. 我们的最终目标价格计算
1 分钟
# 第 14 节： Valuation Part 6 of 6: Valuation Part 6 of 6 Comparing TAM to the Target Price
# 第 14 节： 估值6-6：比较TAM（潜在总市场规模）和目标价格

0 / 1|1 分钟

## 55. Using the TAM to Verify How Realistic Our Target Price Is
## 55. 用TAM来验证我们的目标价格是否合理
1 分钟
# 第 15 节： Assessing Financials with Formulas
# 第 15 节： 用公式评估财务数据
0 / 4|19 分钟

## 56. Introduction to Formulas
## 56. 公式介绍
1 分钟

## 57. Amazing Formulas to Assess Financials
## 57. 评估财务数据的神奇公式
8 分钟

## 58. Exercise on Using Formulas
## 58. 公式习题
1 分钟

## 59. Discussion of the Answers to the Formulas Exercise
## 59. 公式习题讨论
10 分钟
# 第 16 节： Course Conclusion
# 第 16 节： 课程总结
0 / 1|2 分钟

## 60. Conclusion
## 60. 总结
2 分钟
# 第 17 节： Bonus Materials
# 第 17 节： 奖励材料
0 / 1|2 分钟

## 61. Bonus Lecture
## 61. 奖励课时
2 分钟

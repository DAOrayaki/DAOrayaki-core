

价格与预言机
======




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



9 Aug 2021
• 15 min read






![价格与预言机](/content/images/size/w2000/2021/07/b3119313b07eca80cec4605b223f0adaa0448369.png)



#### DAOrayaki DAO研究奖金池：

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee /7 通过

赏金总量：120 USDC

研究种类：DAO, Oracles, Price Snapshots,Flash Loans, Uniswap

原文作者:  Doug Hoyte

贡献者： Dewei, DAOctor @DAOrayaki

原文: Prices and oracles

![](http://daorayaki.org/content/images/2021/07/----_20210426113809-1.png)Euler基于Uniswap的时间加权平均价格（TWAP）预言，允许用户借出和借入几乎任何可替代的代币。这是一系列文章的第1部分，在这些文章中，我们描述了这些TWAP预言机的工作原理，以及它们给我们的去中心化借贷协议的用户带来的优势。

**“价格”的概念**

有时相同的资产可以在不同的市场以不同的价格出售。例如，一个小部件的价格会随着它从工厂到批发商再到你附近的零售商的供应链而上涨。由于人们为同一件东西支付不同的价格，这表明谈论某件东西的单一价格是没有意义的。

当然，并没有什么能阻止你们去工厂，买一堆小部件，站在零售商外面以折扣价直接卖给顾客。如果你这么做的话，你就在进行所谓的套利交易，可能会迫使零售商降低产品价格（或者让你因游荡而被捕）。

套利是引导全球市场向共同价格趋同的力量。它的优点是不需要协调。只要交易成本和交易风险不太高，有足够多的实体出于自身利益行事，就足以确保黄金价格在纽约、伦敦和其他地方的几乎同步波动。

**交易规模**

因此，套利可能是创造资产价格的原因。另一方面，你有没有从附近的零售商那里购买过小部件，而不是直接去中国的工厂？你当然有。如果你买的是小批量的，由于运输成本和中间商的原因，你很自然会认为单价会更高（中国工厂的）。

有点令人困惑的是，除非你学过经济学或在实践中与金融市场互动，否则价格的自然状态实际上恰恰相反：如果你购买的是少量金融工具，你通常可以期望得到比购买大量金融工具更优惠的价格。

为了认识到价格在某种程度上是交易规模的函数，经济学家提到了“边际”价格。这只是一个资产的无限小数额的最佳可用价格。当然，你买不到无限小的部件：价格曲线很少是经济学家研究的漂亮、平滑、可微的函数。取而代之的是，它们通常是免费的，由任何人填写的所有订单都可以进行交易（如股票交易所），或者是更为常规的定价区间结构（如外汇市场）。另一方面，像Uniswap这样的系统更接近于平滑的定价功能，但我们正在超越自己。

**竞争还是合作？**

价格中包含大量信息。这是金融市场帮助社会的一种方式。即使你无意购买或出售小部件，也能够实时观察到它们在世界另一端的价格正在上涨，这可能是许多有价值的信号之一，将有助于你规划你的经济活动。

但请记住，价格是抽象的，缺少重要的背景。想想你所在城镇的加油站：它们的汽油价格几乎相同，而且它们几乎同步波动。这显然是一个竞争市场力量将价格集中到其共同最低可行水平的例子，对吗？

没那么快。如果加油站经营者串通调价，以避免竞争的负面影响，不也会出现这种情况吗？是的，单就价格而言，很难分辨出是哪一种。

**预言机**

就像在所谓的现实世界中一样，许多区块链系统需要访问资产的价格：

·购买或销售某种商品或服务的系统需要确保使用准确的市场价格，无论是产品定价还是投入成本，或两者兼而有之

·衍生品交易系统使参与者能够有效地相互打赌价格是涨是跌。

·贷款系统必须监控贷款和抵押品的价值，以确保贷款永远不会抵押不足

为智能合约提供价格的系统被称为预言机。广义上讲，预言机有两类：链下预言机和链上预言机。各有利弊。

**链下预言机**

在这种设计中，价格是从区块链外部的来源收集的，比如交易交易所，然后这些价格被信任方嵌入到区块链中

一个著名的链下预言机今天是chainlink。在较高的层次上，Chainlink通过向控制一定数量link接代币的节点分配特殊权限来工作。这些节点通过协调在一系列有时间限制的轮次中创建链上价格。每一轮，每个节点提交一个价格，然后智能合约取这些价格的中间值，并将此值提供给链上智能合约。

这种方法的一个非常强大的优点是，所收集的信息可以是任何东西。事实上，在Chainlink上，可以将真实世界的天气统计数据，甚至是纯随机生成的数字等数据带到链上。

另一方面，一些区块链用户对这种方法感到不舒服，因为这样的系统不提供所谓的“客观”数据。从这个意义上意味着用户可以通过查看区块链的运行来验证数据是如何到达的。

例如，您可以通过下载区块链的历史记录并（在确保您没有使用恶意分叉之后）重放到目前为止的所有交易，客观地验证地址钱包的余额。钱包的余额现在是一个不言而喻的客观事实，你不需做出任何超出区块链本身安全的额外安全假设，即可确定这个事实。

**伦敦银行同业拆借利率**

除了理论上的纯粹性，客观性这个概念重要吗？我想是的。让我们考虑一个真实的例子。

伦敦银行同业拆借利率（LIBOR）是“伦敦银行间同业拆借利率”（londoninter bank Offered Rate）的缩写，应该代表短期借款时将采用的现行利率。从某种意义上说，这个价值可以看作是金钱的价格。它是整个金融体系中最重要的数字之一。无论你何时办理抵押贷款、持有信用卡利息或与金融系统发生任何互动，你都可能受到这个数字的影响。但这个数字是怎么产生的呢？

伦敦银行同业拆借利率（LIBOR)本身可以被认为是一个预言机。每天，一组大银行中的每一家都会估算出借款的成本，如果他们愿意的话。银行应该去看看他们的经纪人所报的价格，并以某种方式对其进行汇总，尽管这在很大程度上取决于他们如何做。一旦每个银行都给出了自己的数字，它就会将其提交给负责汇总的协会。在假设它们可能是不具代表性的异常值的情况下，关联抛出最高和最低估计值，然后平均剩余的估计值。这一平均值随后被公布为每日伦敦银行同业拆借利率。

银行对它们的价格有很大的影响力，它们对自己提交的利率在财务上不承担任何责任。在一个纯市场驱动的系统中，如果一家银行公布了一个“坏”价格，那么交易对手将以此价格进行交易，直到价格通过套利收敛。

更糟糕的是，正如2008年一桩重大丑闻所揭示的那样，许多提交价格的银行对基于公布的伦敦银行同业拆借利率（LIBOR）价值的衍生品有着重大的敞口。银行的交易员将与负责提交伦敦银行同业拆借利率(LIBOR)报告的银行人员以及其他银行的交易员协调，推动伦敦银行同业拆借利率(LIBOR)朝着有利于其交易的方向发展。

问题有两个方面：首先，除了市场驱动的套利系统所能提供的以外，不存在资产的单一价格这一概念，任何试图编制这种价值的做法在某种程度上都是虚构的。但更严重的是，伦敦银行同业拆借利率（LIBOR）价格的来源并不透明，银行发布错误数据也不会产生市场驱动的后果。

**链上预言机**

有了智能合约，交易系统可以完全建立在链条上。这就自然而然地产生了这样一种观念，即资产价格可以作为客观事实提供给其他智能合约。通过使用报价作为信号，需要报价的系统可以在区块链的范围内完全封闭和独立（这样的系统是否应该被称为“预言机”是一个我们将忽略的争论）

最有名的纯连锁交易系统是Uniswap。Uniswap的智能合约实现了一个自动做市商，允许流动性提供者将两种资产存入智能合约，交易员通过提供另一种资产来交换一种资产。这种交换的价格取决于交易时池中每个部分的消耗程度。

**价格快照**

由于可以随时通过查看资产的相对数量来确定Uniswap池中资产的当前边际价格，因此很有可能将其用作价格信息的来源。然而，这一点应谨慎行事。池数量的快照可以在任何特定时刻被操纵。

当然，这不是Uniswap的问题，甚至是区块链特有的问题。请注意共同基金年终“粉饰”的现象。由于基金通常是按其年度业绩来评估的，因此有一种强烈的动机，那就是在年底以较高的资产净值结束这一年，即使第二天早上资产净值会立即恢复。在一个季度末，或者在市场收盘前的最后一个滴答声中，还有许多其他异常交易活动的例子表明，人们正在操纵价格以影响市场。

**闪贷**

考虑一下你的支票账户。即使你的账户里没有足够的资金，你也可以开支票。只要你在支票结清前把这些钱存入你的支票账户，你的付款就会成功(传统上，在每天结束时，银行都会先申请所有的日贷项，然后再进行借记——这样被拒付的支票就更少了。

你可以把这种支票当作短期无抵押贷款。假设有人想尽快卖掉一辆车，而且要价很低。你开支票买这辆车，马上把它交给经销商，然后以更高的价格卖掉。然后，在原始支票结清之前，您将经销商给您的支票存入银行，从而使您在交易中获得净利润。你可以用一个完全空的支票账户

在以太坊上，这更进一步：通过采用原子数据库事务模型，一旦检测到操作无利可图，就可以撤消操作。在上述情况下，就好像经销商不想买这辆车，你可以保证把车还给原来的卖家，拿回你的支票，假装什么都没发生过(尽管人们很容易将其描述为区块链所独有的，但这也不完全正确——许多经纪平台提供类似原子交易的应急订单）。

**时间加权平均价格**

在存在快速贷款的情况下，价格快照问题变得更糟。有了巨额贷款，Uniswap市场的资金池规模可能会发生足够大的变化，从而严重扭曲价格快照

正因为如此，Uniswap版本1不适合作为预言机的价格标准（尽管许多项目确实使用了它，但常常是灾难性的）。幸运的是，Uniswap版本2包含了快照问题解决方案的构建块：时间加权平均价格（TWAP）

不用当前价格，TWAPs让我们计算一段时间内的平均价格。它们的工作方式是，每个Uniswap池都有一个连续的总和，每秒钟就有一个当前价格。给定其中的两条记录，将它们相减，然后除以经过的秒数，得到这段时间的平均价格。

·短期价格上涨不会显著影响价格，因为平均值会增加抑制效果。潜在的价格操纵者不仅需要提高价格，而且还需要在一段时间内将价格保持在峰值水平。

·因为闪贷必须在同一笔交易中偿还，从区块链的角度来看，它们根本不花时间。这意味着它们不能用于操纵TWAP：它们在0秒内更改价格，因此不会向运行总和中添加任何内容

**TWAP的挑战**

尽管Uniswap 2非常流行，但是它的TWAP支持并没有像一些人预期的那样广泛使用。事实证明，在生产系统中使用它有几个挑战。

最重要的是，Uniswap智能合约不会在其存储中保留运行价格总和的历史值，而只是当前值。这意味着要检索价格，合同必须在一个事务中记录一个值，然后等待一段时间再记录下一个事务。除了花费额外的汽油，这意味着可能会有一段时间由于记录值太旧而无法获得价格。

在Euler，我们一直在研究一些更有效地使用Uniswap的TWAP的方法，我们将很快更详细地描述我们的系统，因此请订阅本系列第2部分可用时的通知。

**结论**

没有一个单一的“价格”概念对所有交易方都同样有用。价格因计算方式、计量地点、资产交易方式以及某人想购买或出售多少资产而有所不同。获取链上资产的“价格”并非易事，大多数解决方案都会在分散性和准确性方面做出妥协。Uniswap提供了一个去中心化的价格链上预言机，让用户访问平均价格在一段时间间隔。这些预言机抵抗价格操纵，但有自己的权衡。



---

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）  
  
详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)

历史文章：

[DAOrayaki 解读|奥斯特罗姆：公共事务的治理之道](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484580&idx=1&sn=1d1c5412ab24b34242912813041c138a&chksm=c1d80571f6af8c67fbfac08c52c900562a4328f65c7b7a05d09ba3473704ff22aa7153bbefe0&scene=21#wechat_redirect)

[DAOrayaki 研究｜Badger: 加速比特币在DeFi中的发展](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484583&idx=1&sn=ce3513d785537c63563a2a6f4b0f255c&chksm=c1d80572f6af8c64dc90942ec0094915267df5b768dbdc3566eb01a03861a05d85f6bd2d1fec&scene=21#wechat_redirect)

[DAOrayaki 研究｜OpenLaw：自动化法律协议](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484582&idx=1&sn=399fb6eb57009a841d42b686202b6c8c&chksm=c1d80573f6af8c652254e94b62f8b0caa85a5ae22f8ffa745c2fd093e3028e3b0c45768f4674&scene=21#wechat_redirect)

[DAOrayaki 研究｜Orca Protocol：轻量级的社区铸造和管理平台](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484580&idx=1&sn=1d1c5412ab24b34242912813041c138a&chksm=c1d80571f6af8c67fbfac08c52c900562a4328f65c7b7a05d09ba3473704ff22aa7153bbefe0&scene=21#wechat_redirect)

[DAOrayaki 研究｜Badger: 加速比特币在DeFi中的发展](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484583&idx=1&sn=ce3513d785537c63563a2a6f4b0f255c&chksm=c1d80572f6af8c64dc90942ec0094915267df5b768dbdc3566eb01a03861a05d85f6bd2d1fec&scene=21#wechat_redirect)

[Synthetix：去中心化治理结构](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484318&idx=1&sn=ebea1216fb8bdaa17de340aec02274a5&chksm=c1d8024bf6af8b5dcc504cefe8129bd910cc6234a2bd6828f6d9e375a97048209149d1b19e8a&scene=21#wechat_redirect)

[DAOrayaki 研究｜Orca Protocol：轻量级的社区铸造和管理平台](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484581&idx=1&sn=89d7600ed7b2ce945b85f8a3fe73bd73&chksm=c1d80570f6af8c6679920e7e0ea5e42ac253ffa028367881f5d542edb690d613e21b30ab5a88&scene=21#wechat_redirect)

[详解Radicle：去中心化社区的代码协作基础设施](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484495&idx=1&sn=eb91cfc99d2de5fd8a2e4b069abad13c&chksm=c1d8059af6af8c8c9d3a6559505eb8e7dad087b93255f1eaac78222f3497ceff7b0c400a9684&scene=21#wechat_redirect)

[详解Vocdoni: 去中心化的投票系统](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484529&idx=1&sn=1b5c7043115435a09d4241e5d4962230&chksm=c1d805a4f6af8cb2f1570b3cb9bc5e9bd9d396304a247e8447a6bcbc99f26c51dca3161efa6d&scene=21#wechat_redirect)[$WORK 奖励、利益相关者经济学和就业共享的代币化](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484579&idx=1&sn=e52f69e1e926eed1f2d895ad3c23df47&chksm=c1d80576f6af8c60a9f3f0e21d713a61e55ffbad904f0701634aba2f28b9ae746bc2ddd5f046&scene=21#wechat_redirect)

[DAOrayaki 解读|奥斯特罗姆：公共事务的治理之道](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484580&idx=1&sn=1d1c5412ab24b34242912813041c138a&chksm=c1d80571f6af8c67fbfac08c52c900562a4328f65c7b7a05d09ba3473704ff22aa7153bbefe0&scene=21#wechat_redirect)





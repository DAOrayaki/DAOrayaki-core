

Dora Factory Eric Zhang：使用累进税系统提高二次方资助的公平性
==========================================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



18 Jun 2021
• 7 min read






![Dora Factory Eric Zhang：使用累进税系统提高二次方资助的公平性](/content/images/size/w2000/2021/06/1-14.png)



### DAOrayaki DAO研究奖金池：

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 4/7 通过

赏金总量：75 USDC

研究种类：DAO, Price Exposure, Voting Power

原文作者:  Eric, Felix@DoraFactory

贡献者：Yofu, Eric @DAOrayaki

原文: Mitigate Quadratic Funding Inequality with a Progressive Tax System

![](http://daorayaki.org/content/images/2021/06/----_20210426113809-22.png)### 用累进税系统缓解二次方资助中的不平等问题

![](http://daorayaki.org/content/images/2021/06/1-13.png)二次方资助机制已经被许多主要的区块链生态广泛采用: 以太坊、Filecoin、BSC、Solana、HECO、Flow等。到目前为止，二次方资助机制被证明可以有效分配公共资金，以支持开源开软件项目(Open Source Ventures)和更通用的公共项目(Public Goods)。

二次方资助机制允许人们进行多次投票，同时减少大户的影响。在最近的DoraHacks Austin Web3黑客马拉松中，二次方融资机制有效地限制了一次性大额捐赠的影响。（https://hackerlink.io/en/grant/Hack%20Austin/1）

到目前为止，主要的二次方融资资助平台（HackerLink， Gitcoin， clr.fund）都使用了Vitalik Buterin的文章《Quadratic Payments》中描述的算法。对二次方资助的一个中文的描述可以参考Eric Zhang的文章《二次方投票和二次方资助》(https://www.matataki.io/p/6113)。

该论文讨论了二次方资助过程，并概述了女巫攻击、共谋和选民激励等问题。截至目前，二次方资助平台一直在试图解决女巫攻击(Sybil Attack)和共谋(Collusion)的问题。HackerLink正在新一版的二次方资助产品中使用DoraID， DoraID是来自Dora Factory（DAO-as-a-Service基础设施）的身份协议证明，提供基于质押的身份服务。Gitcoin刚刚发布了其GTC治理代币和反女巫Staking机制。clr.fund实现了MACI。所有这些做法都很有前景，使得二次方投票和二次方资助可以在更大的场景中使用。

然而，还有一个很少被现有的文章和平台提及的问题，即匹配资金分配不平等的问题。

### 二次方资助中公共资金池分配的公平性问题

二次方资助在实践中放大了不平等问题。拥有多数选票的项目将获得更大比例的匹配池。在大多数情况下，这不仅会在分配资金时对早期项目造成不平等，还会抑制参与度（并有可能进一步鼓励女巫攻击，例如Gitcoin GR9）。

在最近HackerLink上的HECO Grant中，排名第一的一个项目获得了大量的选票（>HECO Grant Round-1总票数的70%），并在当时得到了总匹配资金池的95%。经过一些调查（数据分析），大多数捐款并非来自女巫攻击，而是来自于真实的投票。

在该项目以绝对优势占据排行榜后，HECO 的Grant在近两周内几乎没有收到任何提交，因为没有人认为自己可以与排名第一的项目竞争。最终，排名第一的项目团队宣布放弃不超过50%的匹配池配额，以支持本轮Grant中其他项目可以得到奖金池中的资助。最终，HECO Grant决定将该项目的支持区（support area） 平均重新分配给所有获得投票 >=10 的项目。这是一个一次性的解决方案，但它启发了我们进一步解决不平等问题。

**解决不平等问题最直接的机制是使用累进税制(Progressive Taxation)。**

累进税是第一次世界大战之前的一个重要的发明。它在20世纪的战后时期被广泛采用，并成为许多国家减少收入不平等的最重要机制之一。正如托马斯•皮凯蒂（Thomas Piketty）在其著作中所指出的那样，累进税“提供了一种方法，其限制工业资本主义造成的不平等，同时保持对私人财产和竞争力量的尊重”。

![](http://daorayaki.org/content/images/2021/06/7772fb2a8c5ad97887a1cfe6a5a6edf-1.jpg)** 一战前和二战后最高的收入所得税税率 (Source: One World in Data)

在二次方资助中，累进税制的实施有多种方法。当然，最简单的方法是设计一个静态累进税阶梯。每一轮之后，每个项目都要缴纳一定数额的税款到一个公共资金池。然后，公共资金池就可以按照社区认为公平的规则进行分配。

### 动态二次方累进税算法

![](https://mmbiz.qpic.cn/mmbiz_png/ovYfePibhjTuxfO7ERjIds6x8cxMNqpZg0IwhzZ3QBgLRUsv5pVrzpUdhhozZGYf6OPwtvQsE2nE4SULibU9lXag/640?wx_fmt=png)根据公式，满足以下条件的项目将被征收重税:

1. **该项目排名靠前**

该项目在总支持区中占主导比例

在这种情况下，对支持区征税，就可以防止垄断。我们可以对包含累进税收的二次方资助机制进行模拟。可以看到，累进税制平滑了公共资金的分配结果。在实际使用中，我们可以通过调节算法中的参数，改变税收曲线的形状，以达到公平性目标。

RULES ===================================

![](http://daorayaki.org/content/images/2021/06/1aab912da790533a3992af8642b0235.jpg)用于模拟的Javascript代码：

![](http://daorayaki.org/content/images/2021/06/1-15.png)![](http://daorayaki.org/content/images/2021/06/2-10.png)![](http://daorayaki.org/content/images/2021/06/3-11.png)![](http://daorayaki.org/content/images/2021/06/4-4.png)

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





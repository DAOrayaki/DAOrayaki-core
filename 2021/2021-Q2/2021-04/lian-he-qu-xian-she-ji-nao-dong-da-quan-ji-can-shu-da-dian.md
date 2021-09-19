


[联合曲线](/tag/lian-he-qu-xian/)

联合曲线设计脑洞大全及参数大典
===============


作为策展市场（curation market）的一个重要组成部分，代币联合曲线作为一种巧妙的新加密经济设计机制广受欢迎，它几乎可以为所有事物实现价格发现和构建自主市场（autonomous market）。




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



28 Apr 2021
• 16 min read






![联合曲线设计脑洞大全及参数大典](/content/images/size/w2000/2021/04/640--1--2.png)



![](http://daorayaki.org/content/images/2021/04/640-1.png)### **DAOrayaki DAO研究奖金池：**

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 5/7 通过

赏金总量：150 USDC

研究种类：DAO, Bonding Curve, Predict Market

原文作者: Paul Kohlhaas

贡献者：Demo, DAOctor, Trinity@DAOrayaki

原文: Token Bonding Curve Design Parameters

### 联合曲线的设计空间、参数和使用案例的映射

作为策展市场（curation market）的一个重要组成部分，代币联合曲线作为一种巧妙的新加密经济设计机制广受欢迎，它几乎可以为所有事物实现价格发现和构建自主市场（autonomous market）。主网（main-net）上已经有一些实时的实现（implementation），其中包括一些被广泛使用的DApp，如PoWH3D、Bancor以及测试网（testnet）上的众多alpha实现。领略Memelordz的精彩，在Rinkeby上创建联合曲线的模因市场（meme market）。

虽然这个概念有了越来越多的拥趸，但其势头比代币管理的注册中心（TCRs）要慢一些。联合曲线依然有太多潜力没有被探索发掘，而且根据我的经验，人们对其理解远不够充分。我认为其主要原因是联合曲线的设计空间宽广，而且由于有太多的参数可以被探索，因此很难被充分探索。

在这篇帖子中，我试图勾画出联合曲线的广阔设计空间和参数，并指出注意事项和用例。我们还探讨了如何缓冲（mitigate）一些攻击矢量（attack vectors），如“拉高出货”（pump and dumps）。此外，我还描述了一个可以应用于各种用例的简单框架。每个用例的理想谢林点参数（ideal Schelling point）可能都有所不同。**本帖旨在发挥一个代币工程工具集（token engineering toolset）的作用，以激励社区中的实验和创新，并创建一个更全面的思考联合曲线设计的方式。**

![](http://daorayaki.org/content/images/2021/04/640--1--1.png) *进入虚拟做市商的兔子洞。来源: https://imgur.com/gallery/HlI68*

在其最简单的形式中，代币联合曲线是一个自动化的做市商（automated market maker），用于交易几乎所有的东西。该合约接受抵押品并以发行其原生代币（native token）作为回报，反之亦然。

我们首先要问，哪些关键参数可以调整来创造新的有趣的属性以服务于不同的用例？下面我提出了从名称中衍生出的6个设计参数，并对每一个参数进行了深入的解释，之后是实际应用。

**1. 代币指标（the token metrics）：**由A)代币发行和B)供应量决定。

**2. 联合（the bond(s)）：**由C)**联合的抵押品**（bonded collateral）和D)交易目标或资产定义。

**3. 曲线（the curve）：**由其E)数学函数和F)价格结构来定义。

![](http://daorayaki.org/content/images/2021/04/640--2-.png)                                                    图 1 联合曲线分类法

（一）代币
-----

### A.发行：由联合曲线产生的代币类型

**参数：**

**1，可互换（Fungibles），ERC20**

**2，非同质化（Non-Fungibles），ERC721**

**3，担保（Securities），ERC1400, ERC1410**

**4，组合（Composables），ERC998**

**注意事项**：合约发行的代币本质上是一种数字资产，它可以提供效用，也可以不提供效用。它可以授予另一个合约的访问权，或者以证券的形式代表现实世界的资产。创建者可能希望代币是可互换的，也可能是不可互换的。实际上，还没有研究涉及发行非可互换物（ERC721s）或其他类型的代币的联合曲线。（Topbidder在做这方面的尝试）这方面的用例可能包括软件产品、收藏品或证券化的许可证。

### B.供应量：该合约可发行的代币总数

**参数：**

**1，有限（Finite）：**有上限的代币供应。

**2，无限（Infinite）：**无上限的“无限”发行。

**3，归属（Vesting）：**发行的代币如何由参与者或创作者归属。

目前提出的许多联合曲线设计都没有对发行的代币数量实施上限，也没有考虑归属期。对于那些在现实世界中难以定价的商品，无上限发行可能是一种很好的价格发现机制，它避免了创建一个潜在的市场价值评估。然而，对于达到确定价值的商品，无限的供应可能会对代币持有者和市场动态产生不利影响。

此外，可以想象，联合曲线也可以有不同的铸造函数来表示曲线上的负利益，以代表曲线上买卖正利息之外的负利息，这可能是一个新的参数。例如，这种机制可以用于做空。我将在以后的文章中解释这方面的可能性。

**注意事项**：代币供应和联合曲线的归属尚未被广泛探索，但对联合曲线上任何市场的未来效用有非常大的影响。例如，我们可能希望对一个数字艺术品的总交易供应量进行封顶，并包含早期买家的归属，但我们可能不希望限制一个模因（meme）的代币供应量。

**（二）联合**C.抵押品：对合约及其储备参数（reserve parameters）所投入的价值或关注（attention）。
-----------------------------------------------------------------

注：Bancor在合同中把抵押物称为准备金，有潜在的设计参数和功能实现会改变准备金/抵押物的比例。

**参数：**

**1. 本地协议代币（Native protocol tokens）：**以太坊（ETH）或海洋协议（OCN）。

**2. 稳定币（Stablecoins）：**DAI或类似的ERC20稳定币（stabletokens）。在最近的#cryptolife黑客马拉松上，我们首次验证了这一概念，并计划构建一个开源实现。

**3. 非同质化代币（Non-fungibles）：**由小猫（kittens）或其他神经纤维形成的连接曲线。

**4. 多重抵押物（Multi-collateralized）：**ERC20s或本机协议代币（native protocol tokens）的组合。

来自其他联合曲线的代币，称为嵌套联合曲线（nested bonding curves）。将联合曲线标记嵌入到进一步的联合曲线中，本质上就是创建衍生品。例如，用例可以是衍生出另一个模因（meme）的子模因，或者是从最初的先导化合物发展而来的衍生分子结构。这种情况下的波动性（Volatility）是复合的，嵌套曲线只有部分抵押品在其原始曲线上。对“母”曲线与其子曲线之间的相互作用要认真建模。嵌套曲线最早由Slava Balasanov在此提出。

**注意事项**：联合曲线的交易本身将具有波动性，这取决于曲线的实施方式。如果基础抵押品在此基础上表现出波动性，就会限制效用，并造成市场低效率和套利。

### D. 交易资产或目标

所发行的合约和代币需要代表某种资产、本金、状态、注意力（attention）甚至效用权的所有权。这种资产或状态可以与合同联系起来，甚至与合同挂钩。它本质上代表了连接到真实或数字世界的联合曲线。

**参数：**

**1. 作为可重新替换的资产（Staked as an Re-Fungible）：**NFT（通过可重新替换的代币），就像一个加密猫或与NFT相关的资产，比如知识产权。

**2. 链接：**IPFS链接，模因（meme），或连接契约，类似于Memelordz。

**法律注意事项**：交易资产将在很大程度上定义监管机构对代币的法律分类。例如，如果我们将现实世界的资产（如房地产）放入联合曲线，代币持有者从该房地产的租金收入中获得股息，那么该代币很像是一种证券。另一方面，如果该代币代表了艺术节的有限入场券，在艺术节上，有限数量的代币按照线性价格曲线被出售，那么该代币更像是一种消费商品。

（三）曲线
-----

### E.曲线函数：通过绘制供应与价格之间的算法关系，实现合约的自动做市功能。

**参数：**

**1. 多项式函数、指数函数和对数函数**

**2. 线性函数**

**3. 基于规则（rule-based）的范式**

**4. Sigmoid函数**

数学函数有多种形式，Wilson Lau写了一篇关于一些潜在功能和实现的文章。Slava Balasanov最近也发表了一篇关于曲线函数和公式的各种参数的文章。

**注意事项**：可以说，函数是最重要的参数，因为它定义了整个市场结构，其效用和未来。这里很重要的一点是，如果曲线创造者希望自己保留一个初始供给，就需要编码到曲线中，例如，作为一个水平函数到某一点。从实操的角度看，我们发现在实体代码中实现曲线类型是相当具有挑战性的，需要进行大量的测试才能得到正确的曲线和相应的界面。

有一个很大的问题是，一旦合约上线，比如出现新的信息，是否可以或应该改变功能。一个现行的流行想法是关于使用oracle来调整功能参数或实现代币持有者治理。曲线的上升和下降可能不适合许多正常的市场参与者，因此曲线的研究应该在实施之前进行，最好是模拟，包括测试供应的最大和最小范围。作为一个简单的练习，你可以考虑在纸上或excel中描绘出你想要的市场行为，考虑哪条曲线最契合你想要的激励方案。

### F.定价：合同如何构造买卖。

迄今为止，许多作者提出了不同的买进和卖出机制，这些机制要么是通过不同的价差函数实现的，要么是通过固定的税收实现的，其使得新的融资和价格稳定机制成为可能。

**参数：**

**1. 静态定价（Static pricing）：**定义市场的一条曲线。作为一种纯粹的注意力（attention）机制，其没有资金需求，但有清晰的市场结构。

**2. 动态定价、价差和税收（Dynamic pricing, spreads and taxation）：**在税收或价差则是从出资者那里抽取的情况下，不同的买入价和卖出价可以用经常性现金流的形式来开发资产。我在这里草拟了一份关于曲线征税的初衷解释：可以简单地通过对每笔购买取一小笔税，或者通过执行不同的进出价曲线来实施税收。引入税收或不同的定价机制会给市场带来摩擦，其好处是会抑制“拉高出货”（Pump and Dump）或市场操纵。因为任何购买都有一定的损失，因此，买方有动力在一定时间内至少持有一段时间，直到再次达到盈亏平衡的价格，并从中获利。例如，Thibauld最近提出了一个利用税收继续资助各组织的实际案例。https://medium.com/@thibauld/introducing-continuous-organizations-22ad9d1f63b7

最近，PentaLaunch也在进行这方面的尝试，详情参见[极客与画家 | 开源项目、NFT和简化的哈伯格税。](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484111&idx=1&sn=6d4128de5b5c7347a3be96c773eaa5ae&chksm=c1d8031af6af8a0c29ede64c2fe7d0e8780ef1a37543c80e3bb23cdb09788d0fed588bf806ee&scene=21#wechat_redirect)

**3. 个体动态定价**

https://tokeneconomy.co/dynamic-token-bonding-curves-41d36e43befa

**4. 均衡定价：**当买家购买时会设定一个预先确定的售价。一旦达到均衡，这些售价就开始触发。https://blog.oceanprotocol.com/introducing-the-equilibrium-bonding-market-e7db528e0eff

“时间是宝贵的”
--------

另一个迄今尚未正式确定的参数是时间概念。Convergent团队在第二次策展市场社区电话会议（curation markets community call）中提出了这一点。具体来说，在创作者预铸代币的情况下，时间可以用来构建锁定期和释放期（lock-up and release periods），或者作为早期贡献者的锁定期。同样，这将降低与联合曲线相关的一些投机风险，提高退出的风险和相关的波动性，并对早期投资者的抛售行为风险进行管理。

在阶段联合曲线（staged bonding curves）的背景下，时间也是一个值得考虑的有趣概念。例如，阶段曲线可以在某个时间点之后实现新的曲率，以反映项目的新阶段。

一个简要框架
------

最后，我们来看一个简单的用例，在这个用例中，这些参数是在一个循序渐进的框架中付诸实践的。想象一下，你是一位艺术家，正在创作一件新的数字艺术品。你设想一个社区共同拥有这件艺术品的一部分，并在资金和艺术上为其发展做出贡献。

![](http://daorayaki.org/content/images/2021/04/640--3-.png)                                                 图 2 联合曲线的音乐口琴框架

艺术品及其权利，以NFT的形式在一条联合曲线上。（1）曲线的目标是通过使NFT可替换和可交易来分配艺术品的所有权，以及衡量其受欢迎程度的关注度，并实现融资。创建者对合同（2）进行决议，发行ERC20代币来代表资产的所有权，有可能被用作许可证等。（3）总代币供应量固定在10万枚，以引入稀缺性来确定整体市值。参与者以DAI的形式向（4）资产提供稳定的抵押品。曲线（5）函数为线性函数，为参与者提供公平、清晰的市场结构。（6）价格结构是动态的，而为支持艺术家，每次购买都会收取一小笔费用。该费用抑制了市场操纵，建立长期承诺，并确保艺术品的未来发展。

结论与展望
-----

六个参数和大量的选项确实给我们留下了大量的设计选择和潜在组合，这其中的大部分依然给人以科幻性和实验性之感，但是一旦你开始研究一些实际的使用案例，许多设计选择就是合理和必要的。具体来说，其中一些设计选择可以帮助减轻某些函数功能所带来的“拉高出货”性质。

这里提供的参数似乎很全面，但每周还都会有新的想法冒出来。许多这些设计细微差别都依赖于用例，并取决于市场工程的目标：市场增长、交易行为、分销、代币效用、市场波动等等。

在我看来，最有趣的参数设计和挑战是围绕着曲线以及买卖价格是如何被程序化构建的。具体来说，这些机制可以实现新的融资方案，引入平衡设计，以减轻对联合曲线的一些定价问题，或实施哈伯格税（Harberger taxes）。至此，我们还只看到冰山一角。最后，改变联合曲线的供应动态来表示负利率，还可以拓宽市场参与者与曲线互动的范围，例如允许参与者缩短曲线。

我相信，在抽象的设计参数上达成共识，将有助于为这个新的设计空间做一个清晰的定义，而为联合曲线定义一个ERC可能非常有价值，它可以使其中的一些参数标准化，并使实验容易进行。如果你正在寻找围绕个别设计模式的具体代码库，或者只是想深入研究，请随时给我发信息.

向Simon de la Rouviere, Florian Bühringer,推文中所有提到的作者以及我在Linum实验室的团队致谢。

### 扩展阅读：

1. WilsonLau：<https://medium.com/thoughtchains/on-single-bonding-curves-for-continuous-token-models-a167f5ffef89>

2. Slava Balasanov：<https://blog.relevant.community/bonding-curves-in-depth-intuition-parametrization-d3905a681e0a>

3. IPFS链接，模因，或连接契约，类似于Memelordz: <https://tokeneconomy.co/token-bonding-curves-in-practice-3eb904720cb8>

  
欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）

### *详情请参考：*

*[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)*

### *历史文章：*

*[罗宾·汉森经典论文（一）|Futarchy：我们应该价值投票、对赌信仰吗？](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484154&idx=2&sn=5562e8b04ffd450720a7b9a49b8dbcd3&chksm=c1d8032ff6af8a39d7a4bb58d97833829ee97ee8969703ea41c31231818997e6e79a1cba0d7f&scene=21#wechat_redirect)*

*[DAOs的设计再思考：信任与决策权、风险、剩余索取权的分配](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484100&idx=1&sn=336bdc7b92314aeea4f24fcddaf2d165&chksm=c1d80311f6af8a07a18fd5e9aa0226d011283575c6707d2bd241afc93258a72c13e38d84ba27&scene=21#wechat_redirect)*

*[DAOrayaki首发| SEC.gov代币安全港提案2.0](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484100&idx=2&sn=34ecbf7ecfa2e32646d69026c550c555&chksm=c1d80311f6af8a0726e84cf990c874002fead7a5f6f3cedd45a216064a4f7ae80185a1356172&scene=21#wechat_redirect)*

*[深度回顾币安智能链BSC Grant HackerLink第一期](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484046&idx=1&sn=72f298e4d41833d6f39340deed5bf424&chksm=c1d8035bf6af8a4de7934291b2f6cff23bd0f808b57d65ccc177266bdf7649516e103cf35cbe&scene=21#wechat_redirect)*

*[Futarchy | 价值投票，对赌信仰，用钱说话，口说无凭](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484004&idx=1&sn=433b36bc5b077011f5abdd8b83c802b2&chksm=c1d803b1f6af8aa74094f3c2d14ca2b9d22d807a5fdc4374cbe6f5f55b8e33d585d61604f07e&scene=21#wechat_redirect)*

*[平行世界｜DeFi无缝集成全球最性感资产—BTC，特斯拉和茅台](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483954&idx=1&sn=d0a5a470a969e9aa9d9f6a6b2bb89232&chksm=c1d803e7f6af8af1574df947cb8be6710937f0a5f30978c255acf81ec02b989b86d184a2e205&scene=21#wechat_redirect)*

*[「激进市场」和二次方投票 | 用市场本身去监管市场](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483861&idx=1&sn=4e8b5b58a53a942df10fd7e38147ae61&chksm=c1d80000f6af8916f92328a4dc051a92c6836fe6b35bdd762dcb002e944d7663a94b63254e59&scene=21#wechat_redirect)*





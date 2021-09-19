

DAOrayaki｜最受热捧的合成资产平台之间区别
=========================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



16 Aug 2021
• 16 min read







**DAOrayaki DAO研究奖金池：**

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee3/7

通过赏金总量：200 USDC

研究种类：DAO, Synthetic Assets

贡献者： Demo, DAOctor @DAOrayaki

![](http://daorayaki.org/content/images/2021/08/----_20210426113809-10.png)合成资产（synthetic assets）只是DeFi的一部分，它模仿传统金融，但移动了链上的一切。虽然交易的产品仍然是一样的：股票、黄金和衍生品，但它们背后的逻辑是全新的。

合成资产的创建将传统金融工具的流动性引入了DeFi世界。任何人都可以发行新的合成资产并在链上进行交易，使用智能合约技术复制所有传统产品。它使现实世界的金融和去中心化的金融都更加可扩展和高效。本文我们将看看几个主要的合成资产平台，比较和对比它们的差异，并介绍Duet协议——一个全新的合成资产协议，具有“过度抵押和算法挂钩的混合机制”。Duet结合了过度抵押的稳定性和算法挂钩的敏捷性。它极大地提高了用户的资金效率，稳定了系统的性能。

截至2021年7月19日，Synthetix在所有上市项目中拥有最高的锁定总价值（TLV）和24小时交易量，尽管它并没有最大的活跃地址数，而且只在以太坊推出，但Synthetix的一般交易策略已经吸引了比普通Defi零售用户更多的组织。

像类似的项目可能会吸引更多的组织，UMA似乎对散户有更高的进入门槛，但根据UMA的用户群，与其他三个项目相比，它应该是最稳定的。

![](http://daorayaki.org/content/images/2021/08/image-129.png)Linear是唯一一家在Binance.com上上市，并在以太坊和币安智能链上同时推出协议的公司。在成交量和用户上保持了相对良好的平衡，也迈出了跨链合成资产无缝交易的第一步，吸引了以太坊内大量成熟的DeFi玩家，同时也通过币安Smart Chain降低了交易成本，提高了交易效率。然而，BSC的总交易量比以太坊小。

下面的图表分别显示了Synthetix和Linear.finance上合成资产铸币量的分布情况，其中加密货币资产占绝对主导比例。

![](http://daorayaki.org/content/images/2021/08/image-134.png)![](http://daorayaki.org/content/images/2021/08/image-138.png)镜像协议（Mirror protocol) 目前只提供美国股票资产，我们已经看到了其交易量和TVL（低速度）之间的显著差异。  
  
我们可以推测，传统金融交易员的潜在市场确实存在，去中心化合成资产可以缓解现实世界中的一些可能的痛苦。然而，与传统加密资产的速度相比，它们可能不是高频交易产品。  
合成资产及其交易者需要一个更有针对性的、完整的逻辑。

**Synthetic（SNX）：Synthetic为多头，iSynths为空头**
------------------------------------------

* 参与者：Stakers

一旦你参与到Synthetix系统中，你就扮演了储存者、铸造者和交易对手的角色，承担了系统整体债务的承销风险。这意味着，如果用户的合成资产升值，你的债务就会增加。

* 合格的抵押品 a) SNX (750%)存入SNX并获得sUSD，以市场价格购买其他合成物，有交易费，但可获得SNX的押注奖励和手续费减免。b) ETH (150%)存入ETH并直接借入sUSD/sETH，不获得交易费或任何奖励，因为他们不承担债务池的风险c) renBTC (150%)存入renBTC并直接借用sUSD/sBTC，不收取费用或任何其他奖励，因为他们不承担债务池的风险。
* 当前持有者：80,399没有订单簿，这意味着所有交易都是针对合同执行的（P2C）。这为系统中全部抵押品提供了无限的流动性，而无需许可的链上交易则为零滑移，并收取固定利率的交易费用。  
然而，所有的协同体持有者都是所有协同体交易的对手方，这使得所有用户面临整个市场的波动风险。  
Synthetix在以太坊的每日活跃用户约为**1400人**，平均交易数为**7000**，历史上唯一的活跃交互者超过**19万**，作为较老的协议之一，这是有一定意味的。

![](http://daorayaki.org/content/images/2021/08/image-139.png)**镜像（MIR），提供针对所反映资产价格方向的空头头寸**
------------------------------

* 活跃参与者a) 交易员（trader) ：在mAssets和UST之间进行买卖。b) 矿工（Minter）：通过UST进入抵押债务头寸(CDP)，以获得新铸造的mAsset的代币。c) 流动性提供者（Liquidity Provider）：向相应的Terraswap池中添加等量的mAsset和UST，从而增加该市场的流动性。d) 股权持有者（Staker）：持股LP代币（使用抵押合同）或MIR代币（使用Gov合同），以获得MIR代币的持股奖励。
* 合格的抵押品（抵押率）a) UST (150%)b) mAsset（150%）
* 当前持有者：24,474对于Mirror来说，大多数活跃的地址都在Terra （Luna）上，它没有可供使用的总地址。Terra上最新的24H交易计数是24,462，几乎是以太坊协议计数的100倍，所以最终的代币持有者总数应该比我们目前的数字的要多得多。

Mirror于2021年1月在币安智能链（BSC）上的PancakeSwap推出了一个UST资金池，尽管造币协议还没有在BSC上推出，但MIR资金池的总锁定价值超过1亿美元。迄今为止，它有超过24K的活跃用户和超过3M的交易。MIR于2021年4月19日在币安上市，这有助于提高MIR流量。

交易由流动性池处理，其相比于Synthetix降低了生态系统中活跃玩家的个人角色风险，但增加了提供流动性所需的资本。该模式使Mirror能够无限制地追踪现实世界中的任何不同资产，而对挖矿者来说风险较小。

**通用市场准入（UMA）**
---------------

* 参与者

a) 代币赞助商（Token sponsors）在智能合约中锁定资金以支持铸造的合成代币的价值的用户。

b) 清算者（Liquidators）监测和清算抵押不足的头寸。

c) 争端解决者（Disputers）使用UMA的无价金融合约监控合约，以确定清算是有效还是无效的。

d) 数据验证机制（Data Verification Mechanism，DVM）引入一个简单的经济安全框架来评估oracles，确保破坏DVM的成本将超过潜在的利润。这样就率先消除了破坏DVM的经济动机。

e) UMA 代币持有者帮助运营DVM，并通过对使用DVM的金融合约的价格请求进行投票，以及通过对参数变化进行投票和批准系统升级来管理UMA生态系统来获得奖励。

* 符合条件的抵押品

共有43种抵押品。

* 迄今为止的持有人

15,063 

UMA目前只专注于以太坊，但正在扩展，以进入其他EVM链。从下图可以看出，自2020年10月以来，UMA的日活跃地址一直保持稳定。

![](http://daorayaki.org/content/images/2021/08/image-140.png)**线性金融（Linear Finance，LINA）**
-----------------------------

合格抵押品

a) LINA + 其他加密货币为了生成一个合成资产，用户需要存入LINA和其他加密货币的混合物。比例必须是80:20，其中80%的抵押品必须是LINA，另外20%是其他加密货币。  


截至目前的持有人：12,840

Linear.finance显示了类似的使用水平，与以太坊和币安智能链的使用水平相似。  
当LINA在币安网上市时，活跃地址在以太坊和币安智能链上都有明显增加，但之后又恢复正常，这与MIR上市后的效果类似。看来，即使DeFi很受欢迎，大多数活跃的贡献者仍然倾向于选择主要的中心化交易所。

![](http://daorayaki.org/content/images/2021/08/image-141.png)![](http://daorayaki.org/content/images/2021/08/image-142.png)总而言之，目前的合成资产协议都面临着类似的瓶颈，如活跃用户的限制、资本效率、抵押品清算风险、资产价格挂钩、合成资产的硬性上限等。Duet决心为加密货币领域的更多资产引入一种创新的方法。

什么是二重奏协议（Duet Protocol），为何与众不同？
-------------------------------

 Duet是一个基于混合机制（过度抵押和算法挂钩模式，over-collateralization and algo-pegged model）的合成资产协议，实现了传统的真实资产（降调资产，Flat Assets）和高增长的加密资产（升调资产，Sharp Assets）之间的转化。

与上述现有的方法相比，Duet提供了一个独特的设计来优化造币和交易。

* 开放性和用户友好：与Binance或FTX CM股权方法相比，链上合成资产铸造对投资者来说更容易且友好，没有进入障碍、程序成本、或单一现货风险。

* 多种抵押品头寸：Synthetix和Linear采用单一资产存款与共享债务的方法。与之相比，Duet选择了多个抵押品，并将CDP分开，这降低了造币商的风险，提高了可扩展性。

* 资产的多样性和兼容性：与MakerDAO的DAI和Mirror的UST相比，Duet接受各种类型的合成资产，拥抱更广泛的生态系统，并支持以太坊、BSC和其他EVM兼容区块链。

* 兼容性。相比与一个只支持多头或空头的永续协议，Duet提供了可转让的dAssets，可以在其他DeFi协议中利用。

![](http://daorayaki.org/content/images/2021/08/image-144.png)**Duet和竞争者的比较：**

**第一个区别是开放性和用户友好**。与Duet的竞争对手相比，目前开发不足的核心造币模块具有类似于Mirror和Synthetix的过度抵押模式，而Duet接受多种加密货币资产作为抵押品。与对手相比，他们大多只接受自己发行的代币作为抵押品，这非常不友好，因为矿工购买系统代币作为抵押品，要承担额外的风险，更何况如果是Synthetix的模式，大家共享债务池，**铸造人无法预计己会欠系统多少钱**。Duet还整合了Farming模块，自动提高用户抵押物的利息，**减少用户的迁移成本**。

**第二是资本效率**。Duet有一个独特的算法挂钩模式，允许用户烧DUET代币，而不需要拿出抵押品来创造合成资产。这种模式下的造币商不会承担任何强制清算的风险，资本利用率达到100%，它彻底解决了资本效率问题。

**第三是资产种类**。基于我们的模式设计（这是一个所有Duet持有人和合成资产持有人之间的博弈局面），可以很容易地在系统中创建新的合成代币，但我们的竞争对手如Mirror仍然只是模仿真实的现有基础资产，这或许在某种程度上对加密货币玩家的吸引力较小。例如，我们不仅可以创建杠杆或反向代币，还可以创建跟踪金融指数的代币，如VIX指数，但在Mirror中只是模仿VIX跟踪ETF，有管理费和仓位滚动费，即内在价值不断下降，这不是一个好的波动对冲工具。

**最后一个是整体设计**。Duet的目标从一开始就不是一个简单的金融应用程序，而是一个平行世界，使现实世界的资产铸造、重组和重建，并允许用户从任何地方分配资本到任何主要资产。Synthetix在现实世界的资产同步化方面，不知为何进展相当缓慢，他们只有很少的合成股票（synth stocks）。我们会有自己的互换、借贷、跨链合成资产流动性聚合器、杠杆套利协议、保险池、清算基金协议、自动复利工具，以及围绕我们的合成资产的更多有用的链上协议，这些被称之为DuFi（Duet Fi）生态系统。

**什么是Zerogoki，为什么它是一个实验性的合成资产协议？**
----------------------------------

![](http://daorayaki.org/content/images/2021/08/image-145.png)Zerogoki是来自Duet协议的实验性协议，它只拥有Duet协议的Lite-minting和算法pegged模块。Zerogoki为各种资产和实验机制提供了一个游乐场，以面对真实交易环境的考验。

Zerogoki在日语中是“零号机”的音译，代表实验模型Unit-00，其代币REI是日语中‘零（れい）’的发音。Zerogoki是一个部署在以太坊上的杠杆代币铸币平台，基于算法挂钩机制，可以为用户提供外汇、黄金、债券等传统资产的杠杆工具。用户可以使用平台代币REI来铸造杠杆代币，也可以使用该协议的合成美元-zUSD来直接购买杠杆资产。

像Kusama（KSM）和Polkadot（DOT）一样，**Zerogoki是开放的，作为一个独立项目运行。Zerogoki的目的是承担Duet的某种压力测试功能**，由于机制设计的不同，其风险和利润结构明显不同。合成资产只通过破坏协议资产-REI产生，并选择波动较大的杠杆代币作为上市资产以增加系统测试压力。同时，采用成本较低的以太坊主网来测试Duet是否能在恶劣的环境下顺利运行。

![](http://daorayaki.org/content/images/2021/08/image-146.png)REI和zUSD主要面向传统投资标的的衍生资产，为加密货币市场提供了许多原始投资标的，如：zGOVT 美国国债ETF 20倍、zXAUUSD 10L黄金现货10倍、zEURUSD 20L欧元/美元20倍等衍生品。Duet目前主要用于美股的合成资产。Zerogoki将继续保持并稳定运营。如果后续Duet的合成资产模块协议升级，也会先在Zerogoki上测试。

结语
--

很明显，Mirror改进了抵押品逻辑，使其对散户更加友好，并采取了比Synthetix更积极的方法。考虑到币安上市的MIR，在PancakeSwap推出mAssets的UST对可能有助于Mirror在BSC和币安网之间建立良性循环，吸引新的DeFi用户。

另外，oracles是所有合成系统的核心，其信息的准确性至关重要，因为它决定了CDP是否有足够的抵押资产被锁定，否则就会触发清算。Mirror在Terraswap Price推出了UST pair，以增加资产的流动性，但这并没有解决AMM价格和真实oracles价格之间的较大差距。例如mGOOGL，其Terraswap Price价格是2484.93 UST，与真实的oracles价格约有0.56%的差距，这表明这个模型仍然值得更多的设计改进。

![](http://daorayaki.org/content/images/2021/08/image-147.png)合成资产的设计越来越强大，我们相信用户定制的和跨链兼容的逻辑将构建一个更可持续的合成Defi世界。

Zerogoki是Duet的一个创新版本，支持更大类别的金融资产，包括加密货币、商品、外汇、债券、股票和金融指数。再进一步，Zerogoki还将提供新颖的金融衍生品，为用户提供更多的造币或交易工具，为项目的其他参与者提供更多的赚钱策略。



---

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）  
  
详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)

历史文章：

[DAOrayaki｜针对高度不可能事件押注的预测市场设计](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485192&idx=1&sn=fc0f043a055e70c7a69592d6d0d4aea0&chksm=c1d806ddf6af8fcb9326e37ac8e55b7fdc285b3023406ce44ad1854697698849cf4fa844cd44&scene=21#wechat_redirect)

[DAOrayaki｜关于改善配对协调补贴的一个方法探讨](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485197&idx=1&sn=b28b0f7450999d040fdc322ba9148bda&chksm=c1d806d8f6af8fce8e56b1206d431fcf3f18799dbe1afd08bfbac2dc456530bc759440bc40de&scene=21#wechat_redirect)

[DAOrayaki｜DAO 国库多元化的范围代币](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485191&idx=1&sn=25c47e7c527cb48d4ce97bf2785bd4d0&chksm=c1d806d2f6af8fc4f84e53e06cd301cc35a24518c66c91246e3937ed6b0ef7483c8a1b9ea231&scene=21#wechat_redirect)

[DAOrayaki｜二次方投票：机制设计如何使民主激进化](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485100&idx=1&sn=c9da137fd19efa8d342b69dab3de524c&chksm=c1d80779f6af8e6ffc76352b779653d9283f9b00057a122f6b3e6ac61ec9cbdcf7f204c7777a&scene=21#wechat_redirect)

[DAOrayaki｜DAO 国库多元化的范围代币](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485191&idx=1&sn=25c47e7c527cb48d4ce97bf2785bd4d0&chksm=c1d806d2f6af8fc4f84e53e06cd301cc35a24518c66c91246e3937ed6b0ef7483c8a1b9ea231&scene=21#wechat_redirect)

[DAOrayaki｜元数据、数据堆栈、数据目录3.0](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485099&idx=2&sn=2d3f8933133b1231c5b6d57cccbb738b&chksm=c1d8077ef6af8e68634421946416f3d1c3508c28bd8fed63fed844d1777d4f02f747ee44c8bc&scene=21#wechat_redirect)

[DAOrayaki｜二次方投票和区块链治理](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485046&idx=1&sn=21c5550753bb5405ba838eeb7857f2d6&chksm=c1d807a3f6af8eb57ebb1ad7a1b1ba8079ed40e4f60ef36d11930d472d233c8ee3d7b6b88ac3&scene=21#wechat_redirect)

[DAOrayaki｜可追溯公共物品融资](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485099&idx=1&sn=59c46a5a5b44dbf3c74c902a2d7c33bd&chksm=c1d8077ef6af8e68247e4557d52e8c7435563ebc25aef988f9986f8881eb244a12a360c82303&scene=21#wechat_redirect)

[DAOrayaki｜二次方投票与公共物品](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485045&idx=1&sn=aff37e0951631c79f7e660f7adf888d0&chksm=c1d807a0f6af8eb656250e092d56aa93dac7f6df9358ec6cf7a9848fac3ee3d3c12d10c47a8e&scene=21#wechat_redirect)

[二次方资助V2协议: 抗女巫攻击、公平和规模化的链上二次方投票](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485044&idx=1&sn=1c0ea021684fc2c8e00cee3c3be83659&chksm=c1d807a1f6af8eb772b7892f23c525ac912ee6a448c8362ca44b2ffb6ae1eeeb42747c0f9e74&scene=21#wechat_redirect)

[DAOrayaki｜全面综述：女巫攻击和防御方法](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484986&idx=1&sn=2e9df8b7db1ccd488eb161428354e146&chksm=c1d807eff6af8ef938a76d7ec10dc91b81414339173b8931aec08a7616f5eae94d95d06c9d3c&scene=21#wechat_redirect)

[DAOrayaki ｜代币经济学导论](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484979&idx=1&sn=ba636f6be333c3a74bf9c9dd49dbd16b&chksm=c1d807e6f6af8ef024ee28871129a35879e2f742f20e902c492e27610313f0cbc1035c87f890&scene=21#wechat_redirect)

[DAOrayaki｜价格与预言机](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484807&idx=1&sn=273c664de6afa9c263f4be0c595d080a&chksm=c1d80452f6af8d44c5c12a9b33313cc3d5df3128d06921ae61c90fd6f494817a91beb29d5508&scene=21#wechat_redirect)

[DAOrayaki｜去中心化自治组织（DAO）行业发展月报（2021.6）](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484806&idx=1&sn=28088c05ecf1c26dcd94ccdc8347be23&chksm=c1d80453f6af8d45040b58692b61c2e2d9bdaf1894d51382ea9042e66fe134f7173c2c5687cd&scene=21#wechat_redirect)





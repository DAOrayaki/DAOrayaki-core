

可追溯公共物品融资
=========




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



3 Aug 2021
• 10 min read







DAOrayaki DAO研究奖金池：

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 3/7 通过

赏金总量：90 USDC

研究种类：DAO, Retroactive Public Goods Funding

原文作者:  Ethereum Optimism

贡献者： Demo, DAOctor @DAOrayaki

原文: Retroactive Public Goods Funding

![](http://daorayaki.org/content/images/2021/08/----_20210426113809.png)注：Optimism 团队长期以来一直在寻找为公共物品（Public Goods）提供资金的可持续解决方案。感谢 Vitalik Buterin 的出色设计，我们现在有了第一个实验结构。本文是 Optimism 与 Vitalik（在第二部分作为特邀作者） 合作完成的。

![](http://daorayaki.org/content/images/2021/08/image.png)在没有商业模式的情况下，要创建一个雄心壮志的项目是极其困难的。项目方很难获得资金，很难聘请到最优秀的人才，也很难坚持克服困难和障碍，创造出伟大的作品。

即使有充足的资金，初创企业也是出了名的困难挑战——失败者占绝大多数。但是他们有一个重要的优势，那就是退出的可能性。退出通过股权（退出中的份额）为前期资金、招聘和调整创造激励。然而，对于非营利组织、自由/开源（FOSS）软件和公共物品项目来说，这种“隧道尽头的光”并不存在。

有鉴于此，许多最优秀、最聪明的明星建筑师，甚至那些真正想做最大善事的人，最终走上了营利的道路，即使最终在使命上做出了妥协，这也不足为奇。对许多人来说，这不仅仅是财富的问题，也是公平的问题。为什么要辛辛苦苦地建设自由软件，让别人从中赚取巨额利润，而自己却没有任何收益？

那么......如果突然间，公共产品项目确实存在退出，会发生什么？一个由项目创造了多少公共利益而不是季度利润决定的退出，会使我们会看到更多的投资和创新技术，使社区利益最大化吗？我们是否会看到更多的非营利组织茁壮成长，而不是苟延残喘？

如下，我们提出了一个实现上述目标的机制。借助协议产生的收入、追溯公共物品融资以及结果预言机（Results Oracle），我们将为公共品项目创造一个初创公司式的融资周期。****Optimism团队承诺将我们从测序中获得的所有利润（在去中心化测序器之前）给予公共物品资助实验，包括第一个公共物品退出（the first public goods exit）。****虽然现在还没有任何利润可以资助，而且细节还在开发中，但我们很高兴现在就做出这个承诺，并分享我们第一个实验的基本想法。

![](http://daorayaki.org/content/images/2021/08/image-1.png)****1 可追溯公共物品融资 DAO 如何运作****
----------------------------

作者：Vitalik Buterin

可追溯公共物品融资（retroactive public goods funding）概念背后的核心原则很简单：****就“过去有用的内容”达成一致，要比对“未来有用的内容”达成一致更容易****。前者仍然经常是分歧的来源，但这种类型的分歧，你仍然可通过使用一些现有的投票机制（例如二次方投票甚至常规投票）获得合理判断。而后者更具挑战性，对营利性领域来说，我们能做到的最好就是建立一个生态系统，其中可以创建初创公司并对其进行投资，并在最终正确时获得奖励。因此，与其完全重新发明轮子，我们还不如创建一个机制全相同的但是适用于公共物品的版本。

一个我们可称之为“结果预言机”（the Results Oracle）的 DAO可以为公共物品项目提供资金。长期来看，这个结果预言机可以由协议费用资助（例如，如果由 L2 项目实施，排序器拍卖是一个候选来源）。但与其他公共品融资 DAO 不同，这个结果预言机会追溯性地进行项目资助，奖励它认为已经提供价值的项目。

这个预言机的设计是一个非常复杂的问题（另见：已知的像硬币投票这样的天真方法来解决长期问题），最好以迭代的方式处理。一个简单的早期版本可能是从正在实施这个方案的生态系统中精心挑选的20-50名技术熟练的长期贡献者。随着时间的推移，随着我们对去中心化治理的理解的提高，该计划会不断改进。

这个结果预言机可以发送奖励到任何地址。以下是它可以向哪些地址发送奖励的一些可能想法：

1. 主要负责项目实施的个人或组织；

2. 代表固定分配表的智能合约，其在为项目贡献时间和 / 或资金的多个个人和 / 或组织之间分配资金；

3. 一种项目token，其供应分配给为项目贡献时间和 / 或金钱的一个或多个个人和 / 或组织，并且它可交易；

在第一种和第二种情况下，结果预言机只会向接收者发送资金。它们都可以作为分配表来实现，合约接受资金并根据特定拆分立即将资金重新分配给接收者。

项目代币（Project tokens）是一个更激进的想法，本质上是为结果预言机的资金创造一个预测市场。结果预言机可以用它的资金为代币设定一个价格底线：如果它分配了X美元的奖励，而项目有N个代币的总供应量，那么它就发布一个公开订单，以每个代币X/N美元的价格购买最多的这些代币的全部供应。

![](http://daorayaki.org/content/images/2021/08/image-2.png)通过设置价格下限（相对于一次性结算）进行资助，允许预言机对同一个项目进行多次奖励。它还允许项目代币既能从结果预言处获得奖励，也能从其他来源获得奖励（例如，其他拨款机制、类似NFT的可收集价值、项目自己的经济模型，如果它后来得到了一个）。制作多个奖励可以通过从预先存在的订单中提取资金，并使用合并的资金制作一个新的订单，设定一个更高的价格底线。

![](http://daorayaki.org/content/images/2021/08/image-3.png)图 1 价格轨迹示例

因为任何人都可以为任何东西创建分配表或项目代币，所以在一个项目中就贡献级别产生分歧的可能性会导致同一个项目出现多个相互竞争的分配表（或项目代币）。在这种情况下，结果预言机不仅必须决定哪个项目是有价值的，还必须决定哪个项目代币或分配表（或在多个代币/表之间划分什么）是衡量谁贡献的更好指标。这类判断不能完全避免，尽管希望只在例外情况下才有此需要。

致谢Vitalik！

****2 种子投资（seed funding）****
----------------------------

我们上面提出的是一个多层次的生态系统，而要让一个新的生态系统从零开始迅速建立起来是很困难的！不同的参与者可以采取几种策略来帮助生态系统的启动。

1. 项目方和基金会的补助金计划；

2. 在Uniswap上出售其公共物品代币的项目；

3. 二次方融资。

****3 结论****
------------

非盈利模式对于维护一个已经建成的代码库可能很有效，但启动一个项目的开始阶段非常困难。绝大多数的初创公司都无法实现任何形式的退出，而对于FOSS项目来说，这就更难了。它往往是一小群高度敬业的人的缓慢的“爱的劳动”。捐赠不是一个足够稳定的资金来源，不足以让一个团队上道。而补助金不足以提供有竞争力的薪水。为了“正确的理由”工作并不能支付账单。

这些英雄们的利他主义固然是一种美德，但作为他们所创造的东西的狂热用户，我们难道不应该希望他们也能得到报酬？

通过FOSS项目提供一个退出方式，我们实际上也激励了融资来源，开源项目现在也可以盈利了！



---

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）  
  
详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)  


历史文章：

[DAOrayaki｜二次方投票和区块链治理](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485046&idx=1&sn=21c5550753bb5405ba838eeb7857f2d6&chksm=c1d807a3f6af8eb57ebb1ad7a1b1ba8079ed40e4f60ef36d11930d472d233c8ee3d7b6b88ac3&scene=21#wechat_redirect)

[DAOrayaki｜二次方投票与公共物品](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485045&idx=1&sn=aff37e0951631c79f7e660f7adf888d0&chksm=c1d807a0f6af8eb656250e092d56aa93dac7f6df9358ec6cf7a9848fac3ee3d3c12d10c47a8e&scene=21#wechat_redirect)

[二次方资助V2协议: 抗女巫攻击、公平和规模化的链上二次方投票](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485044&idx=1&sn=1c0ea021684fc2c8e00cee3c3be83659&chksm=c1d807a1f6af8eb772b7892f23c525ac912ee6a448c8362ca44b2ffb6ae1eeeb42747c0f9e74&scene=21#wechat_redirect)

[DAOrayaki｜全面综述：女巫攻击和防御方法](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484986&idx=1&sn=2e9df8b7db1ccd488eb161428354e146&chksm=c1d807eff6af8ef938a76d7ec10dc91b81414339173b8931aec08a7616f5eae94d95d06c9d3c&scene=21#wechat_redirect)

[DAOrayaki ｜代币经济学导论](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484979&idx=1&sn=ba636f6be333c3a74bf9c9dd49dbd16b&chksm=c1d807e6f6af8ef024ee28871129a35879e2f742f20e902c492e27610313f0cbc1035c87f890&scene=21#wechat_redirect)

[DAOrayaki｜价格与预言机](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484807&idx=1&sn=273c664de6afa9c263f4be0c595d080a&chksm=c1d80452f6af8d44c5c12a9b33313cc3d5df3128d06921ae61c90fd6f494817a91beb29d5508&scene=21#wechat_redirect)

[DAOrayaki｜去中心化自治组织（DAO）行业发展月报（2021.6）](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484806&idx=1&sn=28088c05ecf1c26dcd94ccdc8347be23&chksm=c1d80453f6af8d45040b58692b61c2e2d9bdaf1894d51382ea9042e66fe134f7173c2c5687cd&scene=21#wechat_redirect)

[DAOrayaki｜DAO 通过财政多元化为下一个加密冬天做准备](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484808&idx=1&sn=f089e891fe0c8d0ba6a0c5cf208b9c9b&chksm=c1d8045df6af8d4b37cd79d4efb40d2e0c71d4e2aeb5f322615eecbc06664f452c927a75ae90&scene=21#wechat_redirect)

[加密技术的全面论述—开放金融系统](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484742&idx=1&sn=711607523b7112e1f6dd5dcd855894cf&chksm=c1d80493f6af8d8558574439a91347b54e0a9410cf6a711ed9e75bf2e68543f2d1df8970e640&scene=21#wechat_redirect)[D2D：面向去中心化的谈判协议](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484740&idx=1&sn=ab336ebc7b925d01e547c14f18f5a8df&chksm=c1d80491f6af8d874266b2b365b0e5847fa5ed12f064b9ac0eb5c8c8a72628afb1b0ccf822df&scene=21#wechat_redirect)

[DAOrayaki解读｜价格敞口和投票权](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484712&idx=1&sn=674e8305b9899f73343eae5d68be6a99&chksm=c1d804fdf6af8deb14b0fb4ae8debb6abef6e96ec0a638768f06da475e097a97cf3f00ea5c8f&scene=21#wechat_redirect)

[Muse Museum率先加入DAOrayaki Funders MolochDAO并开展联合研究](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484739&idx=1&sn=7a15f813ff8ca419221bcba9b14cf2f8&chksm=c1d80496f6af8d8038bc222f8ce4eecf9a4ddf47477fdc12233797e48495884334a23322cce5&scene=21#wechat_redirect)  
[D2D：面向去中心化的谈判协议](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484740&idx=1&sn=ab336ebc7b925d01e547c14f18f5a8df&chksm=c1d80491f6af8d874266b2b365b0e5847fa5ed12f064b9ac0eb5c8c8a72628afb1b0ccf822df&scene=21#wechat_redirect)

[DAOrayaki | 去中心化仲裁：Kleros、Aragon、Jur](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484741&idx=1&sn=6dd674ebc05296fa3fe21acada6c1d5f&chksm=c1d80490f6af8d86f57987537135f059d8b95be2267c7f5fb0a1f4af297eea6cdf95daacfe16&scene=21#wechat_redirect)

[DAOrayaki解读｜8步实现去中心化](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484713&idx=1&sn=3b76441db3d940c4ea33fcc7e440e276&chksm=c1d804fcf6af8dea80f1e3bec50b06915e603a5927dac9e255ba3e61f4002c4df27191efb835&scene=21#wechat_redirect)[$WORK 奖励、利益相关者经济学和就业共享的代币化](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484579&idx=1&sn=e52f69e1e926eed1f2d895ad3c23df47&chksm=c1d80576f6af8c60a9f3f0e21d713a61e55ffbad904f0701634aba2f28b9ae746bc2ddd5f046&scene=21#wechat_redirect)

[DAOrayaki解读｜价格敞口和投票权](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484712&idx=1&sn=674e8305b9899f73343eae5d68be6a99&chksm=c1d804fdf6af8deb14b0fb4ae8debb6abef6e96ec0a638768f06da475e097a97cf3f00ea5c8f&scene=21#wechat_redirect)

[DAOrayaki解读｜DAO与全球经济秩序-新自由主义的黄昏（一）](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484684&idx=1&sn=f38e7f8f884f4c6b997506c3c49ca688&chksm=c1d804d9f6af8dcf7e2b8aa629846b60b783d410057e50797ee9b697434f7183d40f04b5f461&scene=21#wechat_redirect)

[DAOrayaki 解读|奥斯特罗姆：公共事务的治理之道](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484580&idx=1&sn=1d1c5412ab24b34242912813041c138a&chksm=c1d80571f6af8c67fbfac08c52c900562a4328f65c7b7a05d09ba3473704ff22aa7153bbefe0&scene=21#wechat_redirect)

[DAO治理中的同构性](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484493&idx=1&sn=4169ed86c19a17a063dc97c9f6b9b87e&chksm=c1d80598f6af8c8e6cac5807f59a01c8e7d062ee3b9806c18b9a5cb139377a7b3c5b55d0dd1d&scene=21#wechat_redirect)

[自动化奥斯特罗姆（Ostrom）以实现有效的DAO管理](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484492&idx=1&sn=a664c1791f6c5c15dbf7a70bff95f1fa&chksm=c1d80599f6af8c8fbb7de3a133867adc4416db070eafe730fce5ff8510aa8c0b10332ae3c75a&scene=21#wechat_redirect)

[海外最新研讨：数字货币与货币体系的未来](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484492&idx=2&sn=9c5526b818a67958cbfa190b7bbd9ed7&chksm=c1d80599f6af8c8f26c1ac5aecdecb1787d1649ca888b73e8d0d82095bf36c876c72ccdb0a49&scene=21#wechat_redirect)





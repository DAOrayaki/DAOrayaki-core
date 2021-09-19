


[API3 DAO](/tag/api3-dao/)

API3 DAO | DAO和质押的意义 Part 1
===========================


API3 发布官方文章介绍即将启动的权威 DAO 治理和质押机制，根据该文章，即将启动的权威 DAO 目前正在进行二次审计，一旦启动将取代目前的 DAOv1，DAOv1 是基于 Aragon 的常规 DAO，投票权是基于代码实现。不过，DAO 的迁移过程将会是渐进式的，也就是说，DAOv1 和权威 DAO 将在一段时间内共存，在这段期间 DAOv1 将作为权威 DAO 的从属角色进行政策辅助。




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



22 Apr 2021
• 8 min read







![](http://daorayaki.org/content/images/2021/04/----_20210422091307.png)DAOrayaki DAO研究奖金池：


> *资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71*


> *投票进展：DAO Committee 5/7 通过*


> *赏金总量： 50 USDC*


> *研究种类：DAO项目进展更新，API3 DAO*


> *原文作者: Burak Benligiray*


> *贡献者：Yofu, DAOctor@DAOrayaki*


> *原文：https://medium.com/api3/significance-of-the-dao-and-staking-b8feeaf93804*

![](http://daorayaki.org/content/images/2021/04/1.jpg)### 前言

*API3 发布官方文章介绍即将启动的权威 DAO 治理和质押机制，根据该文章，即将启动的权威 DAO 目前正在进行二次审计，一旦启动将取代目前的 DAOv1，DAOv1 是基于 Aragon 的常规 DAO，投票权是基于代码实现。不过，DAO 的迁移过程将会是渐进式的，也就是说，DAOv1 和权威 DAO 将在一段时间内共存，在这段期间 DAOv1 将作为权威 DAO 的从属角色进行政策辅助。*

 *此外，API3 还解释了部署质押奖励的原因，其一是为了实现去中心化治理激励，通过在 DAO 池中直接或通过委派质押代币才能参与投票治理，这是以机会成本为代价的，因此需要发放奖励给质押者作为补偿。API3 将对质押奖励实行 1 年锁定期，这可最大化激励利益相关者履行治理职责。此外，质押的另一个作用是为 API3 的保险服务形成抵押品池，这些抵押品将以可量化的方式保护 API3 服务。*

### 简短更新

我们目前正在对权威DAO和质押进行审核。我们已经完成了第一次审核，正在等待其余审核完成。当前的市场状况极大地推动了审计的需求，这导致了审计周期的不确定性。由于阻碍主要来源于外部因素，并且预计将在不确定的但可能很短的时间内解决。因此，DAO＆Stake会在发布声明之后短时间内发布，恕不另行通知，敬请期待。

随着权威DAO及其质押池的推出时间越来越近，我们将发布一系列的帖子来讨论在白皮书中他们是如何被制定的、我们在DAOv1治理的过渡时期学到的东西、以及最终版本是如何实现的。

### 为什么需要DAO？

大多数区块链项目要么由中央管理，要么具有所谓的去中心化治理机制。这样的去中心化治理机制其实是外强中干，社区更像一个被牵着线的木偶。 然而，对于一个要实现真正的去中心化治理的项目来说，它的资产需要保持在一个足够去中心化的区块链上，并以一种无许可和去中心化的方式进行治理。预算控制赋予主权，而缺乏这一点的去中心化治理仅仅是一种表演。

这对于oracle解决方案尤其重要，因为它们不可避免地具有链下组件（因为它们将链下集成到链上）。这些链下组件使它们出现预算的不透明、腐败和欺诈性商业行为。因此，oracle解决方案的设计方式应使其链下（集中控制）的组件服从于给链上（去中心化控制）的组件，而不是相反。在链上且掌握金库密钥的去中心化治理是实现这一目标的最终方法。

过去严格禁止在代币合约中使用mint方法。这是因为缺少去中心化的替代方案，因此创始团队将需要管理此类功能。不难看出，如果有去中心化治理结构值得我们把预算托付给它，那么项目的货币政策我们也可以信任它。这为项目的工具箱又增加了一个工具，并使其摆脱自己设置的困局。

在这里，一个潜在的争论是“ API3在没有权威DAO的情况下表现不错，请继续做正在做的事情。” 问题在于，API3（在DAOv1的管理下）在目前的规模下做得很好，但在我们期望能达到的规模（所有API，所有链，所有用例，公共，许可，企业等）上却无能为力。我们优先考虑去中心化和无许可的治理，期望这种增长将使后来由于权力结构固化而无法进行过渡。也就是说，DAOv1通过实施仁慈的治理积累了大量的合法性，这是API3即使迁移到权威的DAO之后也应该利用的重要资源。

### DAOv1和权威DAO

该项目目前由DAOv1管理，这是一个传统的基于aragon的DAO，其投票权是为创始成员硬编码的。这实现了近似于基于代币的治理，因为投票权持有者的代币是时间锁定的，因此维护项目在长期的成功对他们来说有很大的既得利益。除此之外，权威的DAO将通过无许可提供一个显著的改进。

### 名称“权威DAO”是指以下内容

它是一个更完整的版本，将取代DAOv1。但是，我们没有将其称为最终版或终极版之类的，因为它计划以分级的方式进行扩展。

DAOv1和权威DAO将在逐步迁移过程中共存。在这里，“权威性”是指DAOv1在政策上将作为新DAO的从属角色。从DAOv1到权威DAO的迁移过程将在以后的帖子中进行扩展。

### 为什么需要质押？

就像许多项目都有没有实用价值的代币一样，它们也实现了并不真正需要(或者没有提供所声称的好处)的质押机制。这种盲目的货币扩张只会导致通货膨胀。因此，质押奖励应该要深思熟虑。

在API3的背景下，质押奖励主要是项目为实现去中心化治理而付出的代价（如上所述，这是没有商量余地的）。代币持有者通过在DAO池中质押而直接或间接地参与治理。这是有机会成本的，因为他们可以将其代币押在另一个平台上，或以任何其他方式利用其资本。然后，项目需要用奖励来补偿利益相关者。通过在一年后收回这些奖金，激励股东尽其所能履行其治理责任。奖励金额将自我调节以保持市场价格，这将在另一篇文章中进一步讨论。

当然，质押的另一个用途是为保险服务形成抵押品池，以可量化的方式保护API3服务。人们通常只考虑质押的这种作用，而忘记其充当在去中心化治理中作为代表的作用。实际上，应始终在DAO池中投入与代币总供应量相当的金额，以确保治理充分去中心化，这将是质押目标和为实现该目标而付出报酬的重要驱动因素。

### 总结

在这篇文章中，我们简要介绍了DAO和质押机制对API3的意义，以及它们为何至关重要。接下来几天，我们将发布一系列的帖子，以更深入地探讨细节。

### Reference

API3 将渐进过渡至权威 DAO，质押奖励有 1 年锁定期 by 链闻

Significance of the DAO and staking by Burak Benligiray

*欢迎提交你的DAO研究到邮箱*


> *daorayaki@dorafactory.org，瓜分10000USDC赏金池！*


> 欢迎访问DAOrayaki官网（daorayaki.org）

*详情请参考*


> *[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)*

*历史文章*


> *[DAOs的设计再思考：信任与决策权、风险、剩余索取权的分配](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484100&idx=1&sn=336bdc7b92314aeea4f24fcddaf2d165&chksm=c1d80311f6af8a07a18fd5e9aa0226d011283575c6707d2bd241afc93258a72c13e38d84ba27&scene=21#wechat_redirect)*


> *[DAOrayaki首发| SEC.gov代币安全港提案2.0](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484100&idx=2&sn=34ecbf7ecfa2e32646d69026c550c555&chksm=c1d80311f6af8a0726e84cf990c874002fead7a5f6f3cedd45a216064a4f7ae80185a1356172&scene=21#wechat_redirect)*


> *[深度回顾币安智能链BSC Grant HackerLink第一期](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484046&idx=1&sn=72f298e4d41833d6f39340deed5bf424&chksm=c1d8035bf6af8a4de7934291b2f6cff23bd0f808b57d65ccc177266bdf7649516e103cf35cbe&scene=21#wechat_redirect)*


> *[Futarchy | 价值投票，对赌信仰，用钱说话，口说无凭](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484004&idx=1&sn=433b36bc5b077011f5abdd8b83c802b2&chksm=c1d803b1f6af8aa74094f3c2d14ca2b9d22d807a5fdc4374cbe6f5f55b8e33d585d61604f07e&scene=21#wechat_redirect)*


> *[平行世界｜DeFi无缝集成全球最性感资产—BTC，特斯拉和茅台](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483954&idx=1&sn=d0a5a470a969e9aa9d9f6a6b2bb89232&chksm=c1d803e7f6af8af1574df947cb8be6710937f0a5f30978c255acf81ec02b989b86d184a2e205&scene=21#wechat_redirect)*


> *[「激进市场」和二次方投票 | 用市场本身去监管市场](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483861&idx=1&sn=4e8b5b58a53a942df10fd7e38147ae61&chksm=c1d80000f6af8916f92328a4dc051a92c6836fe6b35bdd762dcb002e944d7663a94b63254e59&scene=21#wechat_redirect)*





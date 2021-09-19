

二次方资助V2协议:链上反女巫、公平性和可扩展性
========================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



16 Jul 2021
• 8 min read






![二次方资助V2协议:链上反女巫、公平性和可扩展性](/content/images/size/w2000/2021/07/src-http___p6.itc.cn_images01_20210624_714132dc3f844d6ea402fc38f8f8d4f4.jpeg-refer-http___p6.itc.jpg)



**DAOrayaki DAO研究奖金池：**

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee /7 通过

赏金总量：100 USDC

研究种类： Dora Factory, HackerLink, DAO, Quadratic Funding V2

原文作者:  Eric Zhang

贡献者： Yofu, DAOctor @DAOrayaki

原文: Quadratic Funding V2 Protocol: Anti-Sybil, Fairness, and Scalability On-Chain

![](http://daorayaki.org/content/images/2021/07/----_20210426113809-9.png)经过几个月的研究和工程实现，我们准备在今天发布二次方资助V2协议。

HackerLink是第一个实现链上二次方投票和资助并使其具有可扩展性的产品。在过去的一年中，大多数主要生态系统都在HackerLink上获得了二次方资金资助，数百万美元的加密货币被分配给了来自世界各地的数千名开发者创建的近1000个项目。

现在我们有三个二次方资助基础设施。

1. 稳固的二次方资助适用于所有与 EVM 兼容的链

2. Substrate上的二次方资助pallet，可部署在所有基于Substrate的区块链上

3. Solana上的二次方资助智能合约，由Solana开发者社区贡献

来自其他几个区块链的开发者正在创建他们版本的二次资金资助，并积极与HackerLink集成。当这些版本准备好时，我们将发布这些版本。

与此同时，当前的二次方资助机制也存在一些亟需解决的问题。这些问题可以分为四个机制设计问题:女巫攻击、共谋、欺诈和不公平。

幸运的是，所有这些问题都在Dora社区和其他社区研究和讨论了好几个月。我们也非常感谢Gitcoin和Vitalik Buterin在Gitcoin GR9期间的讨论。所有这些讨论和研究都为二次方资助V2协议的提出做出了贡献。

**如果你不熟悉二次方资助机制，请阅读Vitalik Buterin的《二次支付:入门》(https://vitalik.ca/general/2019/12/07/quadratic.html)或我的中文文章(https://www.matataki.io/p/6113)。熟悉HackerLink (https://hackerlink.io/en/grant)和Gitcoin (https://gitcoin.co/grants/)上的二次方资助也很有帮助，以便理解二次方资助在实践中是如何工作的。

二次方资助v2协议是在HackerLink二次方资助v1协议上构建的，具有以下特点:

**1. 使用 DoraID 进行反女巫质押**

女巫攻击是所有投票系统的主要问题。事实上，大多数投票机制都需要某种身份系统。由于HackerLink 二次方资助资助发生在链上(去中心化)，因此需要一个链上身份解决方案。

在二次方资助V2协议中，集成了 DoraID 以基于质押验证选民身份（在这种情况下，我们称之为反女巫质押）。DoraID是质押的通用框架。它允许用户以自定义的数量和时间持有DORA代币。它最初是由Dora Factory的开发者在3月底提出的，现在部署在以太坊和BSC上。

如果您不熟悉DoraID，请阅读以下关于它的文章:https://dorafactory.medium.com/doraid-a-solution-for-did-and-staking-on-dora-factory-1fe2f4d942cf

在以往的二次方资助中，轮后分析在调整最终结果和维护公平方面发挥了重要作用。通过DoraID集成，可以大大减少轮后分析的工作量。反女巫质押的原理不是像中心化解决方案那样检查每个投票的合法性，而是通过一个很大的因子将女巫攻击的成本大大增加，进而使其在实际中不可行。

**2. 反欺诈**

虽然二次方资助协议是免许可的，但可以通过一定程度的智能合约管理控制和前端审查添加反欺诈功能。HackerLink已经实现了一个审查机制来验证项目身份。首先，有两个功能允许项目所有者自动验证他们的GitHub和Twitter所有权。此外，它允许管理员删除一个被证明是欺诈的项目，匹配的资金将自动重新计算，并重新分配给社区的其他成员。到目前为止，这种方法对于消除欺诈是非常有效的。批评者可能会说这不是去中心化的，但我们会说它是有效的。

反欺诈功能可以在必要时在DAO机制中实现——允许社区投票，以便列出或删除某个项目。然而，这将在很大程度上减缓决策的进程，就像效率和权力下放之间总是要进行权衡一样。

**3. 用二次累进税收缓解不公平**

之前，我们讨论了匹配资金分配的不公平如何阻碍参与并可能鼓励更多的女巫攻击。为了解决这个问题，我们设计了一个二次方资助累进税制。

关于讨论和算法的详细信息请参考这篇文章:https://ethresear.ch/t/mitigate-quadratic-funding-inequality-with-a-progressive-tax-system/9859

该算法在每次调用vote()函数后分配tax。在二次方资助V2协议中，我们将累进税函数纳入到投票过程中。

**关于共谋**

二次方资助V2协议没有解决共谋问题。Vitalik对共谋进行了非常深入的讨论，并推广了MACI(最小反共谋基础设施)。基础设施的实现并不困难，但困难的是做到用户友好。此外，共谋不是链上治理问题，它实际上发生在所有治理系统中，包括主要民主国家的真实选举。

防止链上治理中共谋的一个一般想法是将投票过程变成非协作博弈的情况。例如，MACI阻止选民之间的投票验证，因此缺乏信任将消除共谋。尽管这个解决方案在技术上很有经验，但它太强大了，并且忽略了社会层面上的一些个人和组织之间的互动。未来共谋问题的真正解决需要借助MACI等算法来“调节”某些协作行为的机制设计。

**结论**

我们希望看到这些新机制设计能够使二次方投票和二次方资助变得稳健、公平和安全。新协议将在未来的HackerLink 二次方资助回合中使用，并帮助将二次方资助规模扩大到一个新的水平，这样我们就可以将开源资金增长到一个新的水平。

随着机制设计的不断完善，传统(链下)投票系统的许多缺点可以被克服。在某个时候，我们可能会看到二次方投票和二次方资助在 DAO 以及民主决策和资金分配的主流机构中被广泛采用。



---

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）  
  
详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)

历史文章：

[DAOrayaki｜DAO 通过财政多元化为下一个加密冬天做准备](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484808&idx=1&sn=f089e891fe0c8d0ba6a0c5cf208b9c9b&chksm=c1d8045df6af8d4b37cd79d4efb40d2e0c71d4e2aeb5f322615eecbc06664f452c927a75ae90&scene=21#wechat_redirect)

[DAOrayaki ｜依靠钱包追踪鲸鱼活动](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484965&idx=1&sn=a1b3b144d0df863e8b1e68a4eaf86f0b&chksm=c1d807f0f6af8ee6c0c5992cd3317714cbff02554e790181233d627bdc8d58ea493bc86988cb&scene=21#wechat_redirect)

[DAOrayaki ｜加密货币里的吸血鬼攻击](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484939&idx=1&sn=3c76bbaef8b1c1637530e1a16f8272a2&chksm=c1d807def6af8ec85bdaf2d7c3cbc2e11e475906d933f4da9f484b713521994366db32383183&scene=21#wechat_redirect)

[DAOrayaki｜价格与预言机](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484807&idx=1&sn=273c664de6afa9c263f4be0c595d080a&chksm=c1d80452f6af8d44c5c12a9b33313cc3d5df3128d06921ae61c90fd6f494817a91beb29d5508&scene=21#wechat_redirect)

[DAOrayaki｜去中心化自治组织（DAO）行业发展月报（2021.6）](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484806&idx=1&sn=28088c05ecf1c26dcd94ccdc8347be23&chksm=c1d80453f6af8d45040b58692b61c2e2d9bdaf1894d51382ea9042e66fe134f7173c2c5687cd&scene=21#wechat_redirect)

[加密技术的全面论述—开放金融系统](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484742&idx=1&sn=711607523b7112e1f6dd5dcd855894cf&chksm=c1d80493f6af8d8558574439a91347b54e0a9410cf6a711ed9e75bf2e68543f2d1df8970e640&scene=21#wechat_redirect)

[DAOrayaki | 去中心化仲裁：Kleros、Aragon、Jur](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484741&idx=1&sn=6dd674ebc05296fa3fe21acada6c1d5f&chksm=c1d80490f6af8d86f57987537135f059d8b95be2267c7f5fb0a1f4af297eea6cdf95daacfe16&scene=21#wechat_redirect)

[D2D：面向去中心化的谈判协议](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484740&idx=1&sn=ab336ebc7b925d01e547c14f18f5a8df&chksm=c1d80491f6af8d874266b2b365b0e5847fa5ed12f064b9ac0eb5c8c8a72628afb1b0ccf822df&scene=21#wechat_redirect)

[DAOrayaki解读｜价格敞口和投票权](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484712&idx=1&sn=674e8305b9899f73343eae5d68be6a99&chksm=c1d804fdf6af8deb14b0fb4ae8debb6abef6e96ec0a638768f06da475e097a97cf3f00ea5c8f&scene=21#wechat_redirect)

[Muse Museum率先加入DAOrayaki Funders MolochDAO并开展联合研究](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484739&idx=1&sn=7a15f813ff8ca419221bcba9b14cf2f8&chksm=c1d80496f6af8d8038bc222f8ce4eecf9a4ddf47477fdc12233797e48495884334a23322cce5&scene=21#wechat_redirect)

[D2D：面向去中心化的谈判协议](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484740&idx=1&sn=ab336ebc7b925d01e547c14f18f5a8df&chksm=c1d80491f6af8d874266b2b365b0e5847fa5ed12f064b9ac0eb5c8c8a72628afb1b0ccf822df&scene=21#wechat_redirect)

[DAOrayaki | 去中心化仲裁：Kleros、Aragon、Jur](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484741&idx=1&sn=6dd674ebc05296fa3fe21acada6c1d5f&chksm=c1d80490f6af8d86f57987537135f059d8b95be2267c7f5fb0a1f4af297eea6cdf95daacfe16&scene=21#wechat_redirect)

[DAOrayaki解读｜8步实现去中心化](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484713&idx=1&sn=3b76441db3d940c4ea33fcc7e440e276&chksm=c1d804fcf6af8dea80f1e3bec50b06915e603a5927dac9e255ba3e61f4002c4df27191efb835&scene=21#wechat_redirect)[$WORK 奖励、利益相关者经济学和就业共享的代币化](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484579&idx=1&sn=e52f69e1e926eed1f2d895ad3c23df47&chksm=c1d80576f6af8c60a9f3f0e21d713a61e55ffbad904f0701634aba2f28b9ae746bc2ddd5f046&scene=21#wechat_redirect)

[DAOrayaki解读｜价格敞口和投票权](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484712&idx=1&sn=674e8305b9899f73343eae5d68be6a99&chksm=c1d804fdf6af8deb14b0fb4ae8debb6abef6e96ec0a638768f06da475e097a97cf3f00ea5c8f&scene=21#wechat_redirect)

[DAOrayaki解读｜DAO与全球经济秩序-新自由主义的黄昏（一）](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484684&idx=1&sn=f38e7f8f884f4c6b997506c3c49ca688&chksm=c1d804d9f6af8dcf7e2b8aa629846b60b783d410057e50797ee9b697434f7183d40f04b5f461&scene=21#wechat_redirect)

[DAOrayaki 解读|奥斯特罗姆：公共事务的治理之道](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484580&idx=1&sn=1d1c5412ab24b34242912813041c138a&chksm=c1d80571f6af8c67fbfac08c52c900562a4328f65c7b7a05d09ba3473704ff22aa7153bbefe0&scene=21#wechat_redirect)[DAO治理中的同构性](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484493&idx=1&sn=4169ed86c19a17a063dc97c9f6b9b87e&chksm=c1d80598f6af8c8e6cac5807f59a01c8e7d062ee3b9806c18b9a5cb139377a7b3c5b55d0dd1d&scene=21#wechat_redirect)





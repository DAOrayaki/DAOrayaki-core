


[NFT pricing](/tag/nft-pricing/)

极客与画家 | 开源项目、NFT和简化的哈伯格税
========================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



18 Apr 2021
• 11 min read






![极客与画家 | 开源项目、NFT和简化的哈伯格税](/content/images/size/w2000/2021/04/-----2021-04-17---9.25.47-1.png)



![](http://daorayaki.org/content/images/2021/04/DAOrayaki-Guidelines-08-4.png)**DAOrayaki DAO研究奖金池：**

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 6/7 通过

赏金总量：50 USDC

研究种类：NFT Pricing, Harberger Tax

原文作者: Eric Zhang

贡献者：Architect@Dora Factory, DAOctor，Trinity@DAOrayaki

原文: Hackers & Painters, Open Source Projects, NFTs, and Simplified Harberger Tax  


**前言：**

对于开源项目发起者、原创内容的创作者、独立艺术家来说，如何既保持内容和作品的独立性和深度，又实现可持续性的盈利，一直是个难题。在依靠流量和广告变现主导的商业模式下，创作者总是被流量平台的所有者“绑架”。之前在社区众筹进行书籍创作时，我们面临的一个困惑点，就是如何使原创者在历次销售中都能够获得相应比例的收益分成，同时又能激励人们主动传播，之前也进行过一些机制设计，但是创作者和传播者的利益仍然是割裂的。

  
哈勃格税最早由美国经济学家阿诺德·哈柏格的理论推导得出。2019年4 月，以太坊创始人Vitalik Buterin在个人博客中也对哈伯格税进行了一定的探讨。哈伯格税的核心规则有两点：1）为私人拥有的财产公开一个标价，并每年提交根据该估价某个百分比的税；2）市场上的任何人都可以按该公开标价从你手中购买该财产。其核心的制衡因素在于：标价开高了，交税要交更多；开低了，别人可以轻易买走你的财产。这两点迫使每个理性人趋向合理范围估价。  


Eric提出的，通过将非同质化代币（NFTs）和简化哈伯格税（Simplified Harberger Tax）相结合的新的价格发现机制，将创作者和传播者链接起来并简化了他们的协作关系。  




---

**极客与画家 | 开源项目、NFT和简化的哈伯格税**

Author：Eric Zhang，Architect @Dora Factory  


在本文中，我们将讨论一种服务于**开源开发者项目的新的融资模式和价格发现机制——基于NFT和简化的Harberger税的开源项目价格发现机制。**

随着开源开发者群体越来越勇于冒险，它们已经成为推动新技术发展和创业的重要力量，激励开源项目变得异常重要。一直以来，黑客马拉松和赏金是其直接的激励手段—开发者通过在黑客马拉松上构建新的项目或者解决一些问题，从而获得赏金奖励。

现在，已经出现新的机制来资助开发者。例如，GitCoin、clr.fund和HackerLink（DoraHacks的开发者平台）开发的**二次方融资捐助（quadratic funding grants）**。大多数的头部的区块链生态系统正在使用二次方融资机制，将其作为与社区共同资助开源开发者项目的一种方式。到目前为止，GitCoin grants资助了以太坊生态系统上的许多项目，而HackerLink grants 则资助了BSC、Flow、Filecoin、Solana、TRON、HECO生态的众多项目。

**另一方面，所有这些方案都是在一定范围内对项目进行排名的方式**，因此，也是从人群中识别有潜力的项目的一种方法。Hackathons通常是根据评委意见（评委多为相关领域的专家或投资人）来产生排名，而二次方融资捐助则是基于社区人气排名。例如，在HackerLink平台上，风投基金会会观察黑客马拉松排名和捐赠排行榜（grant leaderboards）来寻找排名靠前的项目进行投资。

![](http://daorayaki.org/content/images/2021/04/russia.jpeg)黑客马拉松排名和捐赠排行榜效果非常好。但是，它们都依赖于组织者，因此，也非常受限 -- 即必须组织黑客马拉松，而 grants 必须分轮进行。资助和排名是在每个活动中产生的，因此价值/价格发现并不是一个内生的机制。

那么，如何设计一个不受外部组织者制约的开源项目基金和价格发现机制呢？在这里，我提出了一种方法供社区探讨，通过将非同质化代币（NFTs）和简化的哈伯格税（Simplified Harberger Tax）相结合来实现这一目标。

NFTs很直观 -- 它们是非同质化代币，代表独特的资产。哈伯格税是一种财产税，它有两个特点：

1. 人们对自己的资产价值进行评估，并根据自己的评估结果缴税。

2. 任何人都可以以评估价从业主手中买下资产，强行出售

有一些基于哈伯格税的Dapps受到了极大的关注和有趣的反馈。**2019年3月，南非艺术家Simon de la Rouviere创作的《This Art work Is Always On Sale》**，基于哈勃格税的理念和以太坊，以 ERC 721 的形式做了一个数字艺术品，意在探索哈勃格税在艺术领域的应用。这些实验具有开创性和启发性。2019年7月初，BES区块链实验室分叉了该项目，将 Harberger 税应用到“线上广告”这一资产类别上，并在经济机制，应用场景，社区治理形式上做了进一步的创新，**项目名为“一块广告牌”**。在NGO领域，Wildcards也在利用哈伯格税为保护环境筹集资金。

![](http://daorayaki.org/content/images/2021/04/-----2021-04-17---10.26.06.png)This artwork is always on sale：https://thisartworkisalwaysonsale.com/

**区块链和智能合约这一技术手段的出现，使得哈伯格税终于被发现在某些领域是可行和有用的。**

然而，我们需要深刻的认识到，哈伯格税的背景与现在不同。之前的假设下，实体资产有两个特点。

1. 运营成本巨大，比如政府需要大量的资源来运营和管理公共空间，所以征收不动产税是必须的；

2. 稀缺性在不动产中很常见。

**在虚拟空间中，这些假设并不重要。例如，创建和持有数字艺术NFT不会产生任何运营成本，在虚拟空间中，我们可以无限的创建NFT。**

正因为如此，按资本收益征税比收取赞助税(patronage tax)更合理。例如，一个艺术品收藏家不希望因为拥有一幅画就一直缴税，事实上也没有必要这样做，因为艺术品--终究不是一种不动产。但是，**艺术家可以通过最初的销售加上未来每次转售的一定比例的资本收益税，获得充足的资金**。同样的逻辑也适用于数字艺术家，作家及我们本案例中提到的开源开发者。

哈伯格税的强制销售特征非常有用。通过智能合约，我们可以做两件事：(1)登记所有的NFT，(2)任何人都可以在没有得到前所有者许可的情况下强行出售。

我们可以利用哈伯格税的一些特点和我们以上讨论的内容，设计一个开源项目资助和价格发现的替代机制。该机制的工作原理如下：

**1.** **每个项目都可以发行一个含有初始价格的独特的非同质化代币（****NFT****）。**铸造代币的地址成为代币的第一拥有者。

**2.** **只要价格高于先前的价格，任何人都可以根据他****/****她自己对资产的评估，从先前所有者手中购买代币。**

**3.** **出售的资本收益将被征税。**例如，如果一个OSS / BUIDL NFT以 20 $DORA的价格出售，而之前的销售价格是10 $DORA，那么20%的税收意味着2 $DORA将分配给项目所有者，18 $DORA将分配给前所有者。

** OSS = Open Source Software 

Dora团队目前正在HackerLink上部署一个功能，并尝试实验这个机制。下周将会在出现在HackerLink BUIDL上。在实践中，我们可以为该机制添加一些其他的规则。

![](http://daorayaki.org/content/images/2021/04/nft-hackerlink.jpeg)1. 任何货币都可以用来给NFT定价, 例如ETH, BNB。
2. 为了避免系统受到小金额攻击，为每次销售添加费用（例如添加0.000001 $DORA，所有权就会转移）。
3. 为每个NFT添加一条消息，并参考HackerLink BUIDL ID和GitHub 存储库链接。

除了OSS BUIDL之外，这种机制还可以应用于其他领域的资金来源和价格发现。**例如，它可以成为加密艺术发行****NFT****的另一种方式，在继续奖励艺术家的同时，帮助艺术进行价格发现。**它还可以帮助环境保护组织为野生动物卡定价，并从卡的交易中募集资金。例如，Project Ark最近申请了DoraHacks新加坡黑客马拉松的捐款，他们为了保护野生动物正在生成NFT卡。我们可以把它想象成一个工厂，允许任何OSS项目发行自己的 "UniSwap袜子”代币，用NFT和简化的哈伯格税自由交易。

最后，内容创作DAO或许可以使用同样的机制，为每一篇文章定价，同时完成贡献者DAO的资金筹集。目前，DAOrayaki贡献者DAO正在研究这种方式在去中心化媒体中的可行性。

![](http://daorayaki.org/content/images/2021/04/-----2021-04-18---4.10.24.png)**英文版：**

https://ericdorafactory.medium.com/hackers-painters-open-source-projects-nfts-and-simplified-harberger-tax-778e2c435b0f  


**另附上文推荐的参考链接：**

**论文链接：****https://papers.ssrn.com/sol3/papers.cfm?abstract\_id=3243656**

**V 神 medium 发文：** **https://medium.com/@VitalikButerin/liberation-through-radical-decentralization-22fc4bedc2ac**

**橙皮书** **https://orange.xyz/tag/5**

[**微信文章：**Mable 2019 <一块广告牌——二十一世纪的共享广播站？>](https://mp.weixin.qq.com/s?__biz=MzA5Nzk4MDMxMg==&mid=2247484122&idx=1&sn=4f8fbaeadbef5f4bf82f85a1361800d5&scene=21#wechat_redirect)

**Harberger Tax 和 Radical Markets 的书：****Eric A. Posner & E. Glen Weyl 2018,** **, Princeton University Press**

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）

详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)

历史文章：

[DAOs的设计再思考：信任与决策权、风险、剩余索取权的分配](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484100&idx=1&sn=336bdc7b92314aeea4f24fcddaf2d165&chksm=c1d80311f6af8a07a18fd5e9aa0226d011283575c6707d2bd241afc93258a72c13e38d84ba27&scene=21#wechat_redirect)

[DAOrayaki首发| SEC.gov代币安全港提案2.0](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484100&idx=2&sn=34ecbf7ecfa2e32646d69026c550c555&chksm=c1d80311f6af8a0726e84cf990c874002fead7a5f6f3cedd45a216064a4f7ae80185a1356172&scene=21#wechat_redirect)

[深度回顾币安智能链BSC Grant HackerLink第一期](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484046&idx=1&sn=72f298e4d41833d6f39340deed5bf424&chksm=c1d8035bf6af8a4de7934291b2f6cff23bd0f808b57d65ccc177266bdf7649516e103cf35cbe&scene=21#wechat_redirect)

[Futarchy | 价值投票，对赌信仰，用钱说话，口说无凭](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484004&idx=1&sn=433b36bc5b077011f5abdd8b83c802b2&chksm=c1d803b1f6af8aa74094f3c2d14ca2b9d22d807a5fdc4374cbe6f5f55b8e33d585d61604f07e&scene=21#wechat_redirect)

[平行世界｜DeFi无缝集成全球最性感资产—BTC，特斯拉和茅台](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483954&idx=1&sn=d0a5a470a969e9aa9d9f6a6b2bb89232&chksm=c1d803e7f6af8af1574df947cb8be6710937f0a5f30978c255acf81ec02b989b86d184a2e205&scene=21#wechat_redirect)

[「激进市场」和二次方投票 | 用市场本身去监管市场](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483861&idx=1&sn=4e8b5b58a53a942df10fd7e38147ae61&chksm=c1d80000f6af8916f92328a4dc051a92c6836fe6b35bdd762dcb002e944d7663a94b63254e59&scene=21#wechat_redirect)





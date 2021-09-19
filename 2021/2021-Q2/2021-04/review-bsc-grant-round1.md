


[hackerlink](/tag/hackerlink/)

深度回顾币安智能链BSC Grant HackerLink第一期
================================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



4 Apr 2021
• 9 min read






![深度回顾币安智能链BSC Grant HackerLink第一期](/content/images/size/w2000/2021/04/quadratic-funding-1.png)



![](http://daorayaki.org/content/images/2021/04/Dora-Factory-logo.png)**DAOrayaki DAO研究奖金池：**

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 5 /7 通过

赏金总量：100 USDC

研究种类：链上治理，二次方投票和二次方资助（Quadratic Voting & Funding）

贡献者们：Architect，Melody，Trinity

### Review of BSC Grant Round-1 on HackerLink by Architecht

原文链接：https://hidorahacks.medium.com/review-of-bsc-grant-round-1-on-hackerlink-283d477f78b0

现在是时候回顾BSC二次方资助拨款第一轮了。几周前，我在DoraHacks Hackathon上查看了二次方资助的情况，详细信息在这里：https://ethresear.ch/t/quadratic-voting-and-funding-at-eth-hackathon-beijing/8910

2021年1月20日，Binance Smart Chain在DoraHacks的区块链开发者平台HackerLink上启动了第一笔二次资助。这是部署到BSC主网的第一笔二次方资助，我猜，这也是对链上二次方资助（Quadratic Funding Grant）的首次尝试之一。

在开始之前，下面的图说明了链上二次资助的工作原理：

![](http://daorayaki.org/content/images/2021/04/quadratic-funding.png)二次方资助从2021年1月20日持续到2021年3月15日。在此期间，DoraHacks推广了该活动，并邀请了出色的开发人员和开发团队在DoraHacks的Bilibili上进行演示（https://space.bilibili.com/445312136 /）。来自许多国家的团队参加了活动，并在DoraHacks上展示了他们的产品和进展，活动广受好评。

共有108个项目的BUIDL提交给HackerLink以获得BSC资助，有92个项目在链上进行了注册（由于资助是基于智能合约运行的，因此项目必须位于注册表中才能获得投票和资金）。

这些项目涵盖了区块链行业最热门的赛道-Defi，去中心化保险，NFT游戏，BSC基础设施，DAO，zk rollup，去中心化社交网络，去中心化内容平台等。

![](http://daorayaki.org/content/images/2021/04/bsc-grant.png)活动期间我们结交了很多朋友，并从中获得了很多乐趣。币安智能链基金会提供了很多帮助（我们决定今年共同举办更多的赠款和黑客马拉松比赛）。

现在，我想分享一些经验。在我以前的文章中，我讨论了诸如女巫攻击（Sybil Attack），串通，选民动机和投票行为等主题。在这里，我想进一步讨论这些主题。

**1、进一步防止女巫攻击（Sybil Attack）的机制**

在上一篇文章中，我们讨论了大规模的社区参与和收费如何能够抑制女巫攻击。但是，收费不能阻止女巫攻击。人们可以计算可用于攻击并获得最大回报的Token数量。

那么有没有办法防止女巫攻击进行链上二次投票？我不这么认为（就像在中心化的结构中也是不可能的一样）。但是，我们可以在未来的活动中实施一些机制，以进一步改善流程。

我们讨论了四种方法：

**1）通过Staking增加女巫攻击的成本**

简而言之，真正的链上ID是你的资产。我们可以创建智能合约，并要求投票者在特定时间之前将一定数量的BNB放入智能合约中，然后才有资格投票。回合结束后，智能合约将释放BNB，用户可以将其收回。

例如，如果我们要求每个帐户要放10个BNB才有资格投票（如果有人要创建10个投票地址，则需要放100个BNB）。这自然可以在某种程度上阻止女巫攻击。

但是，抵押要求增加了进入壁垒。如果某人没有10个BNB，则该机制将完全阻止该人投票。显然，还有另一个问题是，人们仍然可以借BNB进行抵押，这样就可以获得更多的投票地址。

**2）使用中心化ID**

解决此问题的最简单方法可能是引入一些中心化机制。例如，GitCoin赠款要求用户使用GitHub登录，这样GitHub就自动为投票提供了身份。

HackerLink和GitCoin之间的区别之一是HackerLink Grant运行在智能合约上，而不是多签钱包。因此，即使HackerLink要求用户从前端登录，”科学家”仍然可以通过直接与智能合约进行交互。

当前的去中心化身份解决方案（DID）普遍不够成熟，并且增加用户的使用成本，无法有效解决问题。

在刚刚结束的GitCoin GR9中，即使使用了中心化的身份方案，GitCoin依然受到了普遍的女巫攻击。因此我们可以认为，中心化的解决方案并不是最终的解决方案。

**3）使用白名单注册成为投票者**

白名单可能是链上投票的最可靠方法。如果投票者在投票期之前被列入白名单，则将自动阻止女巫攻击。这种解决方案的缺点是，投票者必须在看到项目之前就进行注册。在二次方Grant中，它导致用户可能需要在看到项目之前就先参与到白名单中，这会减少参与捐赠和投票的人数。在这个Futarchy辩论投票实验中就出现了类似的问题。**[「首个Futarchy辩论投票实验」虚拟空间的资产和实体资产数字化，未来哪个价值更大？](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484030&idx=1&sn=f9767686ca322d30b8701100af15c738&chksm=c1d803abf6af8abd40fa7dbaf7cca6f154c4b0feac613f8f98a140483eb582f155c835474f30&scene=21#wechat_redirect)**

**4）累进税（Progressive Tax）**

抑制女巫攻击的另一个方式是使用累进税（fee）系统。更多的社区捐赠将导致更高的税收（费用）。例如，如果单个项目的社区捐款超过200个BNB，则将收取40％的费用，那么女巫攻击的成本将急剧增加。这种方法的问题再次出现-**当捐款超过一定水平时，会压制选票的数量（depressing votes when a donation is above a certain level）**。如果我们可以估算任何项目的最大社区捐款，那么我们可以设计一个合理的累进税制。

鉴于我们通常会在开放环境中进行二次方投票，因此很难一开始就估算出来自社区的最大捐款。

**2、宽限期**

由于最后几天项目之间的激烈竞争，我们在以后的活动中会增加更严格的宽限期。在宽限期内，我们将做两件事：

**A.验证项目身份**

**B.对活动中的投票记录进行分析并检测女巫攻击**

宽限期使我们能够识别进行女巫攻击的骗子和项目。找到它们后，我们可以将它们从注册表中删除，并取消其获得匹配资金的权利。对于诈骗项目，我们必须将社区捐赠返还给用户。

实际上，我们添加了身份验证，仅在HackerLink的前端上显示经过验证的项目。

**3、空投会增强系统还是破坏系统？**

承诺向捐助者空投的项目在二次资助中更为成功。我们已经在ETH Hackathon Beijing，BSC Grant Round-1和GitCoin GR9中看到了这种现象。

只要承诺，空投肯定会帮助项目筹集更多的社区捐款。但是，它实际上与二次方资助规则相冲突。如果将空投合法化，那么二次资助将成为空投活动的竞赛，因此完全违反了社区从心底选择他们想要支持的项目的初心。

这个问题GitCoin GR9 Finale的直播活动中，社区进行了一些有趣的讨论，人们实际上是在谈论空投是否可以为GitCoin平台带来有效的经济模型。

问题是-如果免费允许空投，那么二次资助就变成了另一回事，也许建立空投捐赠平台可能更直接。

另一个提案是，让项目在空投但不能获得配对资金（matching fund）之间进行选择，或者在不空投但可以使用配对资金中进行选择。这可能是一个合理的提案，尽管实际上可能很难阻止项目暗中承诺空投，因为最终很难追踪到。

另一方面，我们可以通过对二次方融资实施MACI（minimal anti collusion infrastructure，最小防贿选基础设施）来完全阻止空投，因为所有投票消息都将使用运营商的公钥加密，并且除了ZKP（zero knowledge proof，零知识证明）之外，运营商将不会透露更多信息。但是人们可能会对这种方式提出质疑-这真的我们想要的吗？

**致谢**

我们感谢Vitalik Buterin在“Quadratic Payment”文章中最早对Quadratic Funding的描述，将激进市场的原则带到以太坊上。同时感谢所有其他二次方投票和二次方资助实践者们，例如GitCoin Grants，clr.fund，科罗拉多州议会等。

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！  


详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)





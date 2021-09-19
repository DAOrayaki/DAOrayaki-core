

DAOrayaki｜针对高度不可能事件押注的预测市场设计
============================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



13 Aug 2021
• 14 min read







DAOrayaki DAO研究奖金池：

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee /7 通过

赏金总量：150 USDC

研究种类：DAO, Prediction Market, Prediction Market

原文作者: vbuterin 讨论者：sheegaon, samueldashadrach, ryanberckmans

贡献者： Natalie, DAOctor @DAOrayaki

原文: Prediction market design for betting on many highly improbable events

![](http://daorayaki.org/content/images/2021/08/----_20210426113809-5.png)### 问题提出

如果人们要对发生概率极不平衡的事件（即要么非常接近0，要么非常接近1）进行押注，预测市场会使资本效率变得尤为低效。打个比方，如果某事件A发生的概率为90%，那么为这件事下注的人就得投入0.9美元来获得1美元的头寸，但是如果有人下注该事件不会发生，那么仅仅需要投入0.1美元作为资本。这样的机制可能导致或者已经导致了对此类事件的预测市场系统性地提供与0和1的极端相去甚远的概率。

因此，能够读取极不可能事件的概率具有非常重要的社会价值（如果事件极有可能，我们会认为该事件不会发生为不可能事件）：对此类事件的错误估计是公众非理性的重要来源。“不要太担心/兴奋，事情会照常进行”的立场在现实生活中经常被低估，不幸的是，由于资本效率问题，预测市场很难表达这一立场。

### 尝试解决问题的方案

因为解决这一问题会有很大的社会价值，所以我们要对预测市场的设计进行优化。假定该预测市场存在N个极不可能事件，我们可以轻松地打赌它们都不会发生。该设计允许总资本锁定为1美元的情况下，针对N个不可能事件中的任何一个都持有1美元的头寸。在多个不可能的事件同时发生的情况下，该设计通过使市场具有某种不寻常的行为而做出妥协；特别是，如果发生了一个不太可能发生的事件，那么在该事件上下注的每个人都会对其他所有事件产生负面影响，因此无法在所有 N 个事件同时发生时赢取N 美元。

**可以现在N=2的情况下推导：**

我们首先描述两个不可能发生的事件的情况，将这两件事命名为a 和 b。用1-a来指代a没有发生的情况，同理，用1-b来命名b没有发生的情况。注意，你应该考虑a和b都发生的情况，和a与b都不发生的情况。我们考虑“结果窗口”，于是就分为四个象限：ab, a(1-b),(1-b)a,(1-a)(1-b)，这些象限加起来是 1。

![](http://daorayaki.org/content/images/2021/08/image-63.png)现在我们将这结果空格分为三个代币：（i）“yes A”代币（ii）“yes B”代币和“两个都不是”代币

![](http://daorayaki.org/content/images/2021/08/image-64.png)“两个都不是”代币在a和b都没有发生的时候支付1美元，如果只发生了a事件，则支付“yes A”代币，如果只有b发生了，那么支付“yes B”代币。如果两个事件都发生了，那么“yes A”与“yes B”五五开。

也可以从另外的思路思考这个问题：如果我们估计事件A发生的概率是a，事件B发生的概率是b，那么会有如下的结果：

l “两个都不是”代币的价格是（1-a）（1-b）

l “yes A”代币的价格是a（1-b/2）

l “yes B”代币的价格是b（1-a/2）

将这些表达式展开，你会发现如你所料，它们加起来等于1。这样设计的目标是如果a与b的概率很低，而且这些事件是足够孤立，那么认为“yes A”代币代表a，“yes B”代表b（因为ab/2会非常小）。

我们再假设，当N＞2，用X1,X2,…Xn来表示这N个事件，用（1-Xi）（i∈｛1,2,3，…n｝）来表示某件事没有发生的情况。

那么就有这样的代数式：（1-X1）（1-X2）…（1-Xn），这一代数式是“什么也不是”代币，代表N个事件同时未发生。YES代币则表示这一表达式的互补情况，即1-（1-X1）（1-X2）…（1-Xn）。这样就会得到一个总和为2n-1的单项式：X1+…+Xn-X1X2-…Xn-1Xn+X1X2X3-…

每个YES xi代币都可以简单地代表所有单项式中的公平份额xi：全部xi的份额，每个xixj的一半，xixjxk的三分之一，等等。这是因为，如果只有事件xi发生，那么YES xi的持有者会得到一个完整的美元，但是如果m代表着xi,xj…xz都发生了，那么相应YES代币的持有者都可以得到1/m个美元。

在几何上，我们可以将N＞2的情况由N=2时的空格扩展为一个超立方体。最大的（1-X1）（1-X2）…（1-Xn）子超立方体为“什么都不是”代币，然后通过给出最接近于“什么都不是”代币的“xi面”部分来分配其余部分xi 。我们很容易看到这样的结果：

l 不同的份额实际上总计为 1 美元（因此资金不会漏进或流出该机制）

l 所有事件被公平对待（没有任何一个xi 会比任何一个xj得到更好地对待）

l 该机制在给予每个 YES xi 代币持有者尽可能地多接触xi方面做得很好，而且也保证了在给定条件下尽可能少地接触其他事件。

****此外我们还可以在两种情况下扩展该机制：****

1. 如果事件Xi有两种以上的可能性（例如Augur的“NVALID”），那么最简单的扩展就是简单地将除主要事件之外的所有可能性都视为孤立事件。特别要注意的是，如果我们在一个事件的不同不可能结果上使用上述技术，那么它就会精确地简化为一个简单的市场，每个可能的结果都有不同的份额。

2. 还有一种情况是，我们发现给定事件Xi的某一边是不可能的，此时我们可以将某些天然能够发现某事件的某一侧是不可能的方法、机制囊括进来。这样我们就不需要在市场创建的时候提供这类信息了。不过这个工作可以暂缓解决。

### 对这一优化设计的探讨

**1. **鉴于存在“抽象漏洞定律”，从这一设计方案总获得的资本效率可能会被交易者的用户体验与整体交易成本抵消。****

因为预测市场的预测能力是有数量效应的，随着交易量增加，预测能力会上升，尤其是随着交易者重新评估他们的头寸而持续的交易量。在目前的成熟水平下，预测市场是一种娱乐产品。我们看到的是，在所有其他条件相同的情况下，更简单的市场会推动交易量。具有娱乐意识的交易者希望自己了解市场。有一个反射性的常识方面，因为她想相信交易员会在市场上交易，因此购买的股票具有社会效用成分。如果她相信其他交易者了解市场，她就更有可能相信市场会广泛交易。但这一优化方案中存在一些棘手的用户体验问题会影响数量效应。

l 向交易者解释为什么捆绑这些事件，以及捆绑的选择

l 向交易者解释为什么如果罕见事件同时发生，那么大赔率的“YES”一方必须分摊底池

l 围绕交易者有价格映射问题的事实进行管理，因为她可能只关心事件 A 而不是事件 B，认为是 A 将发生的概率为a，但要购买 YES A，她必须处理 YES A 的价格a(1-b/2)

l 在较小程度上解释为什么如果发生任何罕见事件，“NO”方会失败

**从catnip.exchange的角度来看，此优化方案还值得继续往下讨论。**

如它是否可以建立在Augur v2 上。事实上它可以建立在Augur v2 之上，只是需要以不同的方式定义事件。它们都需要是范围事件（即，如价格），其定义为“如果事件 A 且集合 {A, B … Z} 中没有其他事件发生，则该市场应解析为 1，如果 k是包含在 {A, B … Z} 中的事件，包括 A发生了，则市场解析应该为1/k，否则为 0”。

**2. **通过UI机制+消息传递，能够解决上述的用户体验带来的寒蝉效应，可是UI机制+消息传递进行的优化是将罕见事件捆绑进市场，那么此时应该把复杂性加到YES代币一边，还是加到NO代币一边？****

按照该优化模型，复杂性转移到YES代币会更好。因为该设计仍然需要N美元的抵押品来押注N个事件，这可以保证YES选民的简单性，因为这一抵押品能够在获胜时基于YES选民1美元的额无条件保证。因此这一设计自带了不对称的情况，所以只能让YES一方承担更多的复杂性。

但是无论在寻求保险还是赌博的情况下，偏好YES代币的人更可能是普通交易者，而偏好NO代币的人可能是大的基金，它们能够为较低的回报提供保险，因此，将更多的复杂性捆绑到NO代币中是更合适的。

还可以考虑将复杂性捆绑到第三方，TradFi 可能最喜欢的那种模型。因为不是每个人都想为每个市场提供保险，所以我们得允许偏好NO代币的人使用他们的 NO 代币作为抵押品，随心所欲地在更多市场上购买 NO 代币。如果两个NO代币市场同时波动，导致抵押品没有及时清算，则让清算人作为第三方承担损失。清算人将从不使用任何抵押品的人中获利，无论是通过留出用于清算的资本保证金还是利率。

不过也应该看到，在这一机制下，第三方“清算人”只不过是另外一个等级的NO方，它吸收了复杂性，清算人仍需要有大量资金准备吸收损失。但并没有改变这一方案自带的不对称性可能引发的后果。

事实上，这是一个经典的保险问题，“YES”投注者类似于保险保单持有人，而“NO”投注者是发行人或保险公司。保险公司持有的抵押品远远少于支付所有索赔所需的抵押品。尽管如此，大多数普通人相信他们有足够的钱来兑现他们的要求，几乎 100% 的时间。对于极不可能发生的事件，正确的预测市场设计在功能上等同于基于区块链的保险的市场设计。这种保险的一些模式已经存在，但目前还没有证明是投保人还是保险公司获利更多。

**3. **在预测市场中，下注决议可能是按顺序而不是同步发生的，或许可以通过分辨下注决议的顺序，来提高资本效率？****

对此可以采取分批的思想，比如可以通过添加“<= 1 个事件将发生”的部分来调整设计，以便在任何结果中都有两个获胜者，如果出现最多（包括）两个事件的情况，则事件投注者将得到全额补偿地方。

如果事件按顺序解决，一种方法是按如下方式构建资产：

YES代币赋1

NO代币赋1但 YES代币赋 2

NO 代币属于 {1, 2}合集 但是代币 YES 赋 3

…

NO 代币赋 {1, 2...n-1}合集 但 YES赋 n

NO TO ALL

通过这种方式，我们可以通过将其关联资产的价格与列表中晚于它的所有资产的价格总和的比率来获得每个事件的几率（当然，假设该事件独立于顺序较早的事件）。但这种市场建构的方式也存在问题，一个人必须等待事件1和2结算后，才能在事件上进行下注。这种市场构建的方式，固定了对不同事件下注发生的顺序。在这种市场设计下，只下注第三种资产将会有比较大的风险，特别是代币的定价不合理且买方无法分析市场。

事实上，按照如此设计的市场，这类赌注被称为“过关”，在体育博彩中很常见，不过体育博彩中对过关进行了大量的标记，这让这类“过关”是赢面很小的赌注。只有当这些事件相当接近彼此孤立的时候，过关才会是好的赌注。有两种策略：第一种是找到比体育博彩所理解的更相关的投注，例如，当一场低分比赛更偏向 A 队而不是 B 队时；第二种是下注大于体育博彩提供的下注限制。



---

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）  
  
详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)

历史文章：

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

[DAOrayaki｜DAO 通过财政多元化为下一个加密冬天做准备](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484808&idx=1&sn=f089e891fe0c8d0ba6a0c5cf208b9c9b&chksm=c1d8045df6af8d4b37cd79d4efb40d2e0c71d4e2aeb5f322615eecbc06664f452c927a75ae90&scene=21#wechat_redirect)

[加密技术的全面论述—开放金融系统](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484742&idx=1&sn=711607523b7112e1f6dd5dcd855894cf&chksm=c1d80493f6af8d8558574439a91347b54e0a9410cf6a711ed9e75bf2e68543f2d1df8970e640&scene=21#wechat_redirect)

[D2D：面向去中心化的谈判协议](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484740&idx=1&sn=ab336ebc7b925d01e547c14f18f5a8df&chksm=c1d80491f6af8d874266b2b365b0e5847fa5ed12f064b9ac0eb5c8c8a72628afb1b0ccf822df&scene=21#wechat_redirect)







通证工程共享（Token Engineering Commons）：分析权益持有者、通证和治理过程
=================================================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



16 Aug 2021
• 14 min read







**DAOrayaki DAO研究奖金池：**

资助地址:   0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 3/7 通过

赏金总量：120 USDC

研究种类：DAO, Hatch DAO, Token Engineering Commons, Token Model Design

原文作者:  Shermin Voshmgir

贡献者：Shawn@DAOrayaki

原文: Token Engineering Commons

![](http://daorayaki.org/content/images/2021/08/----_20210426113809-8.png)本文将解释和概括围绕TEC（Token Engineering Commons）的各种活动，TEC的目标，机制，以及共同创造的过程。通过这个过程，TEC集体设计未来DAO的治理参数。然而，因为TEC的复杂性，所以本文仍然只是摘要性的介绍。我花了很长时间去浏览TEC海量在线文档，去理解他们为了表述权益所有者、过程、通证等而创建的术语，以及全新的治理原语。我希望本文能够帮助大家理解TEC。感谢Tamara Helenius，chuygarcia92，Griff Green和Jessica Zartler的包括意见和反馈！

**本文章节如下：**

**•** **TEC DAO****的治理机制**

-增强联合曲线 （Augmented Bonding Curve）

-信念投票和争议投票

**•** **TEC DAO****的创建过程**

**•** **TEC****通证（代币）**

Token Engineering Commons（TEC）是一个脱胎于Commons Stack的DAO，它得到了仍处于起步阶段的通证工程领域的许多活跃成员的支持。TEC DAO的目标是资助开发通证系统建模、模拟和部署所需的工具栈，包括围绕这个”通证工程”工具栈的社区建设和教育。TEC DAO将使用各种自动化治理机制来资助”通证工程”工具栈的研发。TEC DAO 治理机制的具体参数将在TEC社区的共同创建过程中确定。社区计划在TEC DAO创建和部署过程的3个阶段，分别使用不同的通证（代币）来进行治理。

Token Engineering Commons是一个社区设计的DAO，目前正在孵化阶段。它是由通证工程师们构建的DAO，用于资助未来通证工程项目的研发。在过去一年，TEC的创始成员一直在构思未来TEC DAO的治理规则，这些规则将在不同阶段部署，第一个阶段将很快完成（更多内容见下文）。这些治理规则的设计理念基于埃莉诺·奥斯特罗姆 （Elinor Ostrom） 的研究。埃莉诺·奥斯特罗姆是一位政治经济学家，她由于“对经济治理，尤其是公地的分析”而获得诺贝尔经济学奖。

创始社区成员目前正在共同定义TEC DAO的治理参数。核心治理机制是"Augmented Bonding Curve“，它将使用各种不同投票机制来实现社区对资金分配的决策。TEC的许多自动化治理机制都是首次被使用——例如Augmented Bonding Curve（市场机制）、信念投票和争议投票（投票机制）。

**增强联合曲线 （****Augmented Bonding Curve****，A****BC****）**

Augmented Bonding Curve （ABC）是一种代币Bonding Curve的修改版本，它可以为任何类型的DAO产生持续的资金。该机制将众筹的要素与一系列针对公共资金的集体决策过程相结合，以实现共同的目标。Augmented Bonding Curve有一个额外的项目资金池、一个代币解锁机制和系统间反馈循环。DAO的所有资金都由一个特殊的智能合约（ABC） 管理。

在TEC DAO中，ABC将为公共资金池的管理提供市场机制，该机制使用各种不同投票机制将资金分配给需要捐赠的TE项目。Augmented Bonding Curve的概念是由迈克尔·扎格姆（Michael Zargham）提出。与标准的Bonding Curve机制相比，ABC更不容易受到操纵攻击，例如追求投机回报的“暴涨暴跌”。

**•额外资金池**:

资金被智能合约分配到两个不同的资金池：“储备池”和“资金池”。就像在其他bonding curve，储备代币（贡献者为DAO提供的资金代币）保存在智能合约中作为新发行代币的抵押品，新发行代币的价格由bonding curve公式决定。然而，与传统的bonding curve合约不同，储备池中只持有所有募集资金的一部分。其余部分以社区税的形式分配给一个额外的“资金池”，这个“资金池”将资金分配给需要捐赠的TE项目。

**•投资者收益**：

任何人都可以成为投资者并购买 TEC DAO 代币。交易价格由Augmented Bonding Curve （ABC）公式决定。ABC公式基于以下假设进行设计：随着越来越多的人向 TEC DAO 提供资金，对 TEC 代币的需求将会上升，价格也会随之上升。这时候，TEC 代币持有者就可以通过出售代币获得投机回报。然而，与任何bonding curve一样，代币不是在公开市场上出售，而是卖回给bonding curve智能合约（也就是燃烧）。

**•退出税**：

TEC DAO投资者把TEC代币兑换成wxDAI时需要支付社区税。这部分税金被送回资金池（用于资助社区项目）。

**•****孵化阶段**：

由ABC智能合约管理的DAO分两个阶段启动：孵化阶段和开放阶段。在孵化阶段，初始贡献者（例如创始成员、忠诚的贡献者、初始投资者或“孵化者”）参与孵化众筹过程。目的是聚集那些可以投入“智力资本”、“汗水资本”和“金融资本”的贡献者，他们将根据投入获得TEC-H代币。

**•****锁定期**：

跟典型的bonding curve不同，TEC孵化阶段铸造的TEC-H代币是锁定的（禁止燃烧）。因为前期炒作/套利会影响“储备池”的稳定性，所以解锁期可以减少这种影响。锁定的TEC-H仍然可以用于对DAO的未来治理规则和资本分配进行投票。通过这种方式，社区专家可以在不受外界干扰的情况下制定治理规则。

**•****开放阶段**：

在这个阶段，任何人都可以投资DAO，并通过持有代币成为TEC DAO的成员。他们的财务贡献将流入"储备池"，他们获得新铸造的“TEC代币”。这些代币可以被持有、卖回给bonding curve智能合约（也就是燃烧）或用于投票。

**•****系统间反馈循环**：

在开放阶段，孵化期获得的TEC-H代币缓慢解锁，解锁速度取决于资助项目的资金量。这意味着如果想解锁TEC-H代币，必须将“资金池”中的资金分配给对公地（commons）产生积极影响的项目。通过这种解锁过程和引入特殊投票机制（例如信念投票），经济上激励代币持有者参与系统的治理过程，将资金分配给对TEC DAO最有利的项目。

Augmented Bonding Curve公式的具体参数正在由TEC社区定义。为了更直观理解改变ABC的参数将如何影响市场动态，Commons Stack 开发了一个在线模拟工具。

**信念投票和争议投票**

在信念投票过程中，选民通过抵押代币来支持他们希望获得批准的提案，不断表达他们的投票偏好，并且他们投票的信念（即权重）会随着时间的推移而增长。这不是传统的时限性投票机制。信念投票中，任何人都可以随时更改他们的投票偏好，但一个人对同一提案的偏好保持的时间越长，投票的“信念”就越强（权重也越高）。在这种机制下，偏好有一致性的长期社区成员比短期参与者（只想影响一次投票）具有更大的影响力。

争议投票是另一种提供额外投票功能的机制，例如 （i） 投票授权，（ii） 争议提案的框架，以及 （iii） 防止最后一刻投票结果翻转。相关的设计参数包括（a）“委托投票期”的持续时间， “所需的最低法定人数”，“静默结束期”的长度，“需要多少赞同票”，“投票持续时间”。争议投票最初设计用于 Aragon Network DAO，但是最终并没有在Aragon实现。

**TEC DAO 创建过程**

TEC 社区的创始成员目前正在共同定义TEC DAO的治理参数。

**•****阶段****1 — 孵化DAO**：

阶段1的目的是准备孵化DAO。 “孵化者”负责定义和投票决定最终TEC DAO的治理参数。

孵化阶段，需要确定两类人。一类是活跃社区成员，他们在阶段1贡献了时间和专业知识（以“影响时间”衡量）；另一类是“孵化者“。“孵化者“都是来自Commons Stack瑞士基金会的正式会员，这样做是为了避免投机者在社区初期就进入TEC DAO。而且瑞士基金会的会员身份可以保护"“孵化者“免于承担个人责任。

**（译者注： C****ommons Stack****瑞士基金会为会员提供法律支持）**

**•****阶段****2 — 公地（Commons）升级**：该阶段的第一部分是 4 周孵化期：“孵化者”为孵化DAO提供一定数额的wxDAI（有上限）作为资金。这4周结束后，“孵化者”将有几周的时间来讨论和投票决定自动化政策制定工具的最终参数，例如Augmented Bonding Curve、信念投票和争议投票。在这个过程中，“孵化者”拥有与其持有代币同比例的投票权。

![](http://daorayaki.org/content/images/2021/08/image-125.png)**•****阶段****3 — TEC DAO上线**：投票过程结束后，DAO将正式上线。上线后，TEC DAO向所有人开放。任何人都可以成为支持者，为公共资金池提供资金，并投票决定资助哪些项目。任何TE项目都可以来申请资助，用于项目的研发。

**TEC生态系统中的****通证（****代币)**

在创建TEC DAO的过程中，三个阶段分别有不同类型的代币：

**阶段****1**：

DAO成员在阶段2使用TEC-H代币进行投票。如何在阶段2获得TEC-H代币？有2种方法，方法一：在阶段1通过社区活动证明（Praise System）赚取影响时间 （IH） 代币，（IH） 代币可以在阶段2兑换成TEC-H代币；方法二：持有CSTK代币的Commons Stack社区成员能够在阶段2购买TEC-H代币。在阶段1，IH代币和CSTK代币可以共同用于治理投票。

**IH代币****（阶段****1****）**

**•****目的**：声誉代币，根据社区活动按比例奖励早期贡献者（建设者）

**•****铸币**：贡献证明（以影响时间衡量），由社区成员的“赞美”（Praise）数量决定。Impact Hour 代币 （IH） 可以在阶段2兑换成TEC-H代币

**•****供应**： 无限

**•****价格稳定性**：没有货币价值（但是兑换为TEC-H后具备货币价值，价格取决于总量）

**•****可转让**：否

**•****同质化****（Fungible）**：是

**•****过期日期****/事件**：孵化成功后，IH 可以兑换成 TEC-H，IH代币在孵化初始化前被冻结。

**•****权利**：IH兑换成TEC-H后，声誉代币也转换成投票权

**CSTK代币****（阶段****1****）**

**（译者注：C****ommons Stack****最初提供****CSTK T****o****ken****。瑞士基金会成立后，根据律师的建议，不再称为T****oken****，因此把原代币销毁，改成了C****STK Score****。原文中称为C****STK** **S****core Token）**

CSTK是Commons Stack生态使用的代币，作为社区的声誉代币。TEC DAO引入了CSTK，因为没有经济上的必要性，再去设计一个新的声誉代币。TEC的孵化者必须拥有CSTK，这主要是出于法律原因，因为只有Trusted Seed联盟的成员才有CSTK，这将减少孵化者个人承担的法律责任。

**（译者注：T****rusted Seed****联盟的成员自动成为C****ommons Stack****瑞士基金会会员，所以两者经常被混用）**

**•****目的**：声誉代币，TEC的孵化者必须拥有CSTK

**•****铸币**：Commons Stack发行

**•****供应**： 无限

**•****价格稳定性**：没有货币价值，声誉代币

**•****可转让**：否

**•****同质化****（Fungible）**：是

**•****过期日期****/事件**：在TEC社区，CSTK只在孵化结束前有作用

**•****权利**：拥有CSTK才能成为孵化者。在阶段1用于投票

**wxDAI代币（所有阶段）**

wxDAI是由xDAI链管理的稳定币。它被TEC社区定义为支付代币，在孵化DAO和最终的TEC DAO上线后使用。

**阶段2**：只要在4周时间内达到最低募资额度，孵化DAO就成功。这时候，所有wxDAI将兑换为TEC-H代币。IH代币也会兑换为TEC-H代币（占25%）。如果没有达到最低募资额度，孵化失败，wxDAI会返还给孵化者。

**TEC-H（****孵化代币，阶段2****）**

**•****目的**：用于阶段2的治理投票

**•****供应**：最小供应（1,066,666 TEC-H + 25% 额度给IH代币）

**•****可转让**：否。但是孵化者可以随时退出DAO孵化，TEC-H会兑换成wxDAI（需要交社区税）

**•****同质化****（Fungible）**：是

**•****过期日期****/事件**：公地（Commons）升级后，TEC-H会按照1:1的比例兑换成TEC

**•****权利**：产权（投资代币）和投票权

**TEC****代币****（****D****AO****正式上线，阶段****3）**

**•****目的**：投资代币、治理代币

**•****供应**：由Augmented Bonding Curves决定

**•****价格稳定性**：或许不能，具体由Augmented Bonding Curves参数决定

**•****可转让**：或许可以，具体由Augmented Bonding Curves参数决定

**•****同质化****（Fungible）**：是

**•****权利**：产权和投票权，具体由Augmented Bonding Curves参数决定



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





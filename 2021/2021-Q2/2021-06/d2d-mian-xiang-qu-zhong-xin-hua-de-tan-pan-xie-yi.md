

D2D：面向去中心化的谈判协议
===============




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



28 Jun 2021
• 19 min read






![D2D：面向去中心化的谈判协议](/content/images/size/w2000/2021/06/--1-14.png)



**DAOrayaki DAO研究奖金池：**

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee /7 通过

赏金总量：150 USDC

研究种类：DAO, D2D, Decentralized Negotiation Protocols, Game Theory

原文作者:  Max Hampshire & Cem Dagdelen

贡献者： Demo, DAOctor @DAOrayaki

原文: D2D: Towards Decentralized Negotiation Protocols

![](http://daorayaki.org/content/images/2021/06/----_20210426113809-25.png)DAO2DAO（D2D）是Curve实验室和BlockScience受PrimeDAO委托进行的一项研究合作。本文旨在分享关于去中心化谈判协议设计的理论和技术见解。

在过去的几个月里，研究团队分析了谈判协议方面的文献，并调查了加密货币生态系统的适用基元，以便为DAO空间的潜在部署提出设计模式。该工作组正在策划一个实时更新的文献集（living literature），用于定位对设计方法论的理论理解，调整多个研究领域，如网络中的社会选择（social choice）、组合博弈理论（compositional game theory）、适应性结构理论（adaptive structuration theory）和复杂合约谈判（complex contract negotiation）。

**1.背景**

本研究旨在明确不同的去中心化自治组织之间的协调机制。这些互动的范围可以从合资企业（即为公共产品提供资助）到代币交换或分布式货币政策。为了围绕这个问题确定理论认识，研究团队就谈判协议（negotiation protocols）的研究进展进行梳理。

**什么是谈判协议？**

“一般来说，谈判是由两方或多方共同决定的过程。各方首先将相互矛盾的要求用语言表达出来，然后通过妥协或寻找新的替代方案的过程来达成协议。”—— **Jin, Lu, 2004**

谈判无处不在。为了降低交易成本，社会倾向于围绕这些过程制定规范和协议。在国际关系、社会选择和网络理论等领域都有谈判。拍卖（auctions）、投票模块（voting modules）和策展清单（curated lists）都是可以被视为生成性谈判协议（generative negotiation protocols）的博弈。

通过D2D研究的实施，我们希望将上述形式化的东西带到组织间的框架中。一旦DAO能够通过这些谈判机制相互对接，我们预计会出现诸如合并（****mergers****）、合资（j****oint ventures****）、社区互换（communityswaps）和多中心政策模式（****polycentric policy patterns****）等用例。

**2.文献回顾**

接下来让我们着眼于一些理论坐标，来围绕去中心谈判的问题定位我们的理解。

**我们的目标是：**

1. 制定一个去中心的自治组织的可操作定义；

2. 建立博弈论和社会选择的坐标；

3. 收集关于简单和复杂合约的谈判协议的相关研究。

在讨论主要是DAO的实体之间的谈判时，为了从实操上理解参与协调游戏的代理人，需要一个分类学的基础（taxonomical grounding）。由Wittgenstein推广的家族相似性的概念（family resemblances popularized）使我们能够从一个非单一的角度来看待这些组织实体。纵观游戏的分类学变化，他得出结论：

“我们可以用同样的方式去看很多其它的博弈组；我们可以看到相似性是如何出现和消失的。而这种检查的结果是：我们看到了一个复杂的相似性网络，相互重叠，纵横交错：有时是整体的相似性。”

近年来，确定组织分类学中这些重叠的相似性取得了进展。Kei Kreutler在《去中心化自治组织的八个特征》（**Eight Qualities of Decentralized Autonomous Organizations**）中探讨了DAO中作为家族相似性的典型特征。为了适应这种多样化的行为者本体，本研究提出了一种行为者无关的设计模式，后文将讨论。

不出所料，谈判分析大量运用了博弈论。我们相信DAO之间（DAO to DAO）的互动可以用博弈论的具体框架进行适当的分析和整合。特别是，冯·诺伊曼和莫根斯坦的合作博弈理论（cooperative game theory）为洞察合谋的行为方式奠定了基础，也就是玩家的一部分是如何就哪些行动进行谈判的。斯特林最近对网络社会选择理论（Theory of Social Choice on Networks）的迭代是另一种更高级的形式，它完善了“个人理性行为的概念，即影响网络的成员将他们的利益扩大到他们自己狭隘的个人福利之外，以便将他人的影响纳入自己的理性范围”。

也许在实操上最相关的是在谈判协议领域进行的研究。这方面的工作主要集中在简单合约上——由一个或几个独立问题组成的合约。然而，复杂合约谈判协议（Protocols for Negotiating Complex Contracts）扩展到具有大量相互依赖的问题的复杂合约。考虑到相互依赖的偏好排序（inter-dependent preference orderings）的复杂性，这一特点使这种框架更适用于现实世界。

如前所述，文献综述旨在成为一份实时的文献集，并将在本研究计划的过程中进行更新，为技术设计和实施过程提供参考和背景。

**3.技术研究**

除了将文献综述中所涉及的材料作为创建一个通用技术框架的概念性铺垫外，技术研究还受益于两个研究子目标的约束：创建一个尽可能（1）模块化（modular）和（2）不可知（agnostic）的框架。

**3.1 设计目标**

模块化（****Modularity****）是软件开发的一个标准目标，也是去中心化应用设计（decentralized application design）的一个关键方面。创建一个尽可能模块化的机制，并利用已经存在的（和审计过的）代码模块，可以适当地关注应用层面的安全模型，并确保该机制易于交接；减少代码的复杂性通常也会减少攻击面（attack surfaces）。此外，可重复使用和模块化的代码减少了将该模块集成到现有的智能合约架构中所需要的时间和精力，增加了潜在的使用量。

不可知性（****Agnosticism****）是指软件或硬件的一种特性，它不依赖于（或仅与）特定的系统或设备一起工作。在我们的机制中，我们的目标是通过创建一个模块来降低集成和用户体验的复杂性，该模块既与代理无关（agent agnostic），也与在创建共享协议之前发生的过程无关（这里称为条件背后的不可知论，behind-the-condition agnosticism）。

代理不可知性（****Agent-agnosticism****）指的是需要创建一个机制，无论使用它的DAO的规模和复杂性如何，都能发挥作用：每个DAO被抽象为类型代理的实例。该机制必须能够说明由外部拥有的账户（EOAs）或合约地址所代表的DAO，以仅通过调用智能合约函数来创建协议，而不管它们所代表的成分数量和它们建立在上面的DAO框架（如果有的话）。

“条件背后”（****Behind**** theCondition，****BtC****）的不可知论规定，使用该机制的技术障碍必须极低。只要DAO能够调用智能合约功能，它就应该能够使用该机制。如果需要一个专门的接口合约，那么就必须作为机制实例化的一部分创建一个合约工厂，以允许合约与机制互动，而不必进行代码修改。这方面的一个例子是合约地址必须实现接收ERC-1155代币，并与Gnosis的条件代币框架（Conditional Tokens Framework,）互动，而EOA则没有。这一点必须在机制中加以说明，即创建接口合约工厂，由不实现这些方法的DAO拥有，以便在涉及条件代币时与D2D机制对接。

**3.2 用例**

D2D机制有许多潜在的用例，从简单的合资企业到为白名单参与者（各自DAO的成员）创建（本质上的）临时市场。虽然简单的D2D合作已经发生，但这些合作依赖于社会和法律协议。而本文概述的D2D机制旨在创建一个机制，通过该机制，这些协议被链上协议所取代，用安全的、基于网络3（web3-based）的合作协议形式取代这些混乱和耗时的做法。

在确定这些用例的范围时，协定被简单定义为A和B同意X发生。这已经发生在DAO内部（例如对提案进行投票时）、多签名钱包（例如N个成员中的M个同意签署交易）和去中心化的第三方托管中；这个机制的目的是在外部代码模块中正式确定这些现有谈判过程的关键之处。

在现实世界中，第三方托管是在满足某种条件之前，通过受信任的第三方来保管贵重物品。智能合约能够承担通常由中间人承担的调解作用，从而大大降低执行成本。通过链上托管机制的迭代，可以满足一个简单的谈判协议，每个社区的选民通过在各自的组织中投票来表达他们对交易的意愿。

托管模式严重依赖DAO所产生的单一共识（monolithic consensus）。这样做的一个后果是反对派在这些社区中被边缘化。我们相信可以有不同的机制来允许更广泛的表达。例如，市场允许并奖励细颗粒度的互动。一个资产的独立谈判越多，这个市场就越有深度和信息。因此，我们可以推测，通过D2D机制，有可能创建封闭的市场，只有社区的各自成员可以购买或出售彼此的本地代币（或任何其他资产）。这样，两个（或更多）社区可以进行有机的价值渗透，这可以被视为一种民主合并。然而，这种机制要复杂得多，在实施之前，需要记忆不研究。

**3.3 技术概述**

以下是在我们研究被评估的基元的概述。需要注意的是，虽然近年来整个生态系统取得了许多发展，但本文只讨论与D2D机制本身有关的方面：特别是促进抵押协议和oracle的代码模块和智能合约。本研究不涉及DAO的具体进展，因为D2D机制的目的是尽可能地对参与合作工作的组织形式不可知，因此具体进展在此并不重要。

![](http://daorayaki.org/content/images/2021/06/--1-13.png)生态系统基元

Gnosis的条件代币框架（CTF），虽然主要是为预测市场（prediction markets）的创建提供一个基础，但也为任何人提供都了“在特定事件发生的条件下交易任何资产（[t]rade any asset under the condition that a specific event happens）”的可能性。可以利用这一点，使D2D合作的关键要素（如共同融资）在链上“锁定”，避免了对昂贵和冗长的法律协议的需要或对诚信的依赖。虽然简单的D2D合作可以由其他模块来促进，如托管合约，但CTF允许更复杂的条件环境，并使用相同的核心基元（条件代币合约）来创建，不需要为复杂协议编写自定义托管智能合约。此外，CTF允许在DAO之间创建新的安排（见Market Logic用例），这些安排目前还没有被现有的代码模块所推动，同时还提供多层条件的创建，这可以用来在DAO之间更大的伞状协议（umbrella agreements）中创建子合约。CTF已经被预测市场Omen（使用Kleros作为一个Oracle）和社会影响平台Alice使用。

上述依赖CTF的用例的简化版本是一个去中心化的托管服务，如Kleros提供的服务，其中双方可以锁定开发基金，用于一个合资企业的创建过程。一旦双方达成协议，这些资金将可用于商定的账户，例如由两个DAO的成员控制的多重签名。

API3的Airnode是一个“完全无服务器的Oracle节点，专门为API供应商运营自己的Oracle而设计”，其旨在激励第一方Oracle（即运营商）也维护他们的服务。Airnode的一个优势是，它依靠建立Oracle节点的沉没成本和节点运营商的声誉来加强对其决定的信任，以及与其他Oracle服务相比相对较少的维护（和停机时间）。Reality.eth采取了相反的方法，而是提供了一个“众包的链上智能合约Oracle系统（crowd-sourced on-chain smart contract oracle system）”，作为一个独立的dapp和可以直接互动的智能合约。问题必须遵守他们的模板才能被接受。

Kleros（以及经营托管服务）还经营“一个开源的在线争端解决协议，该协议使用区块链和众包来公平裁决争端”，并有可能有助于将决策外包给一个专门设计的协议，而不是为D2D合作寻找裁决者，进一步简化开发。Omen利用它作为他们的CTF实现的Oracle角色。他们使用ERC-1497证据标准和ERC-792仲裁标准。

Keep3r为项目创造了将某些工作外包给项目之外的账户的可能性，无论这些账户是合约、机器人还是EOA。这是一个主要与开发和功能调用/工作有关的用例，“他们希望执行的行动是‘善意的’而不是恶意的结果”，因此可能不适合CTF所使用的大规模Oracle功能。然而，对于可能出现的较小的“内务”功能，这个可以保留。

**3.4 高阶装配**

这个高层次的概述简要描画了一个D2D合作，其允许通过托管智能合约进行迭代谈判和共享基金。该机制可以清楚地分成两个阶段。

**阶段1：D2D谈判**

1. DAO1在内部讨论其成员之间的潜在合资企业，然后写一份提案。

2. DAO1的成员根据DAO利用的任何共识模型对该提案进行投票。

3. 假设投票通过，DAO1就会将该提案发送给DAO2（如果没有，那么该提案就会在再次投票前重新修改，否则该过程结束）。

4. DAO2内部讨论该提案。

5. 然后DAO2对这个提案进行投票。如果这次投票通过，第二阶段开始。如果没有，那么DAO2就有可能向DAO1提出相反建议（过程从第1步重新开始），或者DAO完全拒绝，过程结束。

**第二阶段：托管资金**

1. 两个DAO中的一个（例如DAO1）从工厂智能合约中创建一个托管合约，该合约以商定的提案中指定的合约参数进行初始化。来自这个DAO的资金也被发送到托管合约中，时间锁定期（timelock period）开始。

2. 另一个DAO（例如DAO2）必须在时间锁定结束前用他们商定的代币数量为托管提供资金。如果不这样做，则时间锁定期可能会被延长，或者操作被中止，锁定的资金返回到DAO1。如果资金在时间锁定结束前发生，那么谈判是成功的，并发生指定为“操作X”的功能（例如，流动性池的联合供资，将共享的开发基金转移到一个多义词，等等）。

在设计上述第一个抽象概念时，我们优先考虑已经在D2D合作空间内发生的过程，创建一个独立的机制，可以很容易地取代对法律或社会协议的需求。为了模块化、安全性和参与的DAO的整体易用性，我们采用了一个托管模型。

将机制的互动分离成两个不同的阶段，主要是为了促进两个DAO之间的迭代建议谈判，允许双方之间交换相反的建议，直到双方成员对合作条款感到满意。

在未来，这个模型可以很容易地被修改，来创建一个机制，其中一方单独创建时间锁定的托管，消除相反建议的可能性，并通过合作以更类似于赏金或公开任务的方式提出建议。

**4. 未来研究主题**

在需要Oracle（即共享期货或公共商品）的情况下，如果机制要利用多结果条件，可能会出现对Oracle分类学的需求。这些差异可能取决于正在读取的数据的位置（链上或链下），数据的类型（客观与主观信息），或者（例如）在一个非常主观的条件下，条件的答案是否可以众包。此外，某些方面可能希望指定用于特定决策的Oracle（见API3对第一和第三方oracle的区分）。在以下D2D互动的情况下，对于所使用的Oracle类型有明显的偏好。

l 合资企业：首选情况是与双方都有基于声誉的联系的第一方oracle，因为合资条款涉及链上和链下的主观和客观信息。

l 交换：第三方oracle就足够了，因为只用链上信息就可以确定，即检查DAO1和DAO2的代币余额是否在预定的时间X前按约定的金额变化。

关于该机制的安全性：尽管用于许多D2D协作的代码库非常简单，通过减少可能的攻击面，减轻了许多安全问题，利用与不同资产价格相关的条件进行更大规模的D2D交互的更广泛的影响可能会打开类似于过去一年中所看到的涉及闪贷（flash loans）的攻击向量。在D2D协议中纳入基本保险或限制有条件赔偿可能有助于减轻这些风险。对蜜罐（honeypot）的创建和减轻以及更广泛的脆弱性进行适当建模还有待进一步推进。

**5.结论**

由于谈判协议无处不在，以及“协定（agreements）”分类发的无限多样性，实现的可能性空间非常大。多数情况下，可以在D2D机制中概述的每个阶段利用多个基元中的一个。进一步的研究和经验迭代应为实现更完整的设计产生切实的协同作用。

为了制定可实现的目标，我们已经应用了一些选择标准，以提高可用性和引导实施研究的重点。在我们的范围界定中，将每个DAO定义为一个单一的代理，大大降低了机制的复杂性，同时为创建DAO可以与之交互的单个接口契约提供可能。通过利用整个以太坊堆栈的现有基元，我们想要创建一个开放的谈判环境，在其中可以满足DAO生态系统的多种需求。



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





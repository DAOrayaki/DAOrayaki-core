

Orca Protocol：轻量级的社区铸造和管理平台
===========================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



14 Jun 2021
• 11 min read






![Orca Protocol：轻量级的社区铸造和管理平台](/content/images/size/w2000/2021/06/--1-4.png)



**DAOrayaki DAO**研究奖金池：

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee /7 通过

赏金总量：200 USDC

研究种类：BarnBridge, SquadDAO, TradFi,  DeFi, Structured Market Adjusted Risk Tranches (SMART), Bounty Hunters, yield bonds, SMART Alpha Bonds, yield-based derivatives

贡献者：Jones, Julie, DAOctor @Daorayaki

发布时间：Orca Protocol 于 2020 年 12 月加入区块链社区，本应在 2021 年春季推出，但据团队称将于今年晚些时候推出，时间尚未确定。

![](http://daorayaki.org/content/images/2021/06/----_20210426113809-10.png)**Orca 协议的简要概述**

Orca 协议是一个轻量级的社区铸造和管理平台，授权链上社区根据其价值观进行创建、塑造和工作。 这些组织的需求和形式千差万别，现有的 DAO 框架缺乏足够的系统或灵活性来适应各种用例。

**I.背景**

关于 Orca 协议的信息并不多，因为它是一个尚未确定的新项目。从已有的信息可知，它是一个涉及 DAO 治理和提案管理的协议。 关于DAO 可用性问题，已不是什么秘密。DAO 结构要么过于复杂，要么不够强大。 同时，当前的治理框架缺乏有效管理结构和权限，导致选民不积极参与和选民奖励的错位。 以至于，链上治理没有发挥其全部潜力。 传统的 DAO对单个空间中的数千甚至数百万个参与者的管理感兴趣，而 Orca 协议团队对通过称为“pods”的模块化工作组来管理参与者更感兴趣。

通过将组织构建为更小、更有效的单元（模块化、类似乐高积木的 pod），社区可以更好地治理、组织和管理。 在这个模块化系统中，组织（通过集体决策）决定自己的制衡系统，同时还允许存在集体所有权、群体自治和灵活的等级结构。此外，治理是极其复杂的，它通常是一种主观/有偏见的机制。通过 Orca 协议，可以为组织提供一个客观的模块化治理工具来构建自己的治理系统。

**II.团队成员**

-       Julia Rosenberg – Orca Protocol 的联合创始人和 Overlly 的创始人，曾在 Acreage Holdings 负责企业发展、并购工作近一年，并在 Lloyd Harbour Capital Management, LLC 和 Archutas Ventures 研发部门任职。

-       Twitter Account: https://twitter.com/JulzRoze

-       John Sterlacci –Orca Protocol 的联合创始人目前在宾厄姆顿大学担任兼职讲师。

-       Twitter Account: https://twitter.com/johnsterlacci?lang=en

-       Daniel Thompsom – Orca Protocol 的软件工程师，有研究和语言背景。Daniel 将语言和技术交叠的魅力运用在其编码中，提供了创造和创新的解决方案。区块链爱好者，以及运用去中心化应用程序的创新性，旨在使Web3 技术重塑数字社区。

-       Twitter Account: https://twitter.com/fl0ridadan

-       Steven Valeri – 关于 Stephen Valeri 的信息不多，但从他的 Github 个人资料中可以看出，他目前很有可能是 Orca Protocol 的软件工程师。

-       Github profile: https://github.com/stevenvaleri

-       Gressha Mehta – Orca Protocol 的产品设计，之前在 Apple、Uber 和 Spotify 工作。 Mehta 擅长利用故事的力量为人们创造唤起情感和互动的体验。目前，她在 Orca Protocol 担任产品设计师，而过去她在 Apple 担任技术项目协调员，在 Uber 担任 UX 设计师，在 Spotify 担任品牌设计师。

-       LinkedIn Account: https://www.linkedin.com/in/gresshaa

**III. Orca 协议背后是什么**

简单地说，Orca 协议被用于 ERC1155 的as-efficient, Sybil-resistant 的 DAO 工具。该协议有一个简单的 UI 仪表盘（dashboard）来管理 DAO 提案并允许对链上资产进行链上投票，所有这些都使用 Gnosis Safe 进行保护。

1.   Orca Pods:

Orca 由 pod 组成：社区由固定数量的成员代币组成，每个代币代表一次投票。 每个 Pod 都链接到多重签名保险库，以安全地保存共享的链上资产。

Pod 灵活且模块化构建，用来容纳更多的使用案例，包括项目治理、联合投资、社区管理等等。

![](http://daorayaki.org/content/images/2021/06/--1-2.png)2.   Orca如何构建的

这个项目是使用 Javascript 和 Solidity 构建的。 为了设置 Orca 协议的开发环境，Orca 协议团队使用了 Hardhat/Waffle 和主网分叉。 除了用于追踪用户代币的 ERC1155 ，当涉及到规则时，它们被存储为Structs，并被打包交易及执行。 每个 pod 都连接到一个 Gnosis Safe 实例，交易通过保险箱进行。 此外，第一次集成包括 ERC 代币所有权、AAVE 投票委托和 AAVE 提案委托。 每一项都被编码成规则，由 pod 执行，并针对 AAVE 主网叉进行测试。 此外，做一些相对复杂的微调。

3. Orca 协议和 NFT：

今年 3 月，某些交易市场上的 NFT 艺术交易量猛增超过 2 亿美元，但在 4 月下降了 50%。对于批评者来说，这是“NFT 的终结”。然而，艺术只是冰山一角， NFT 的新用户案例正在迅速出现。

NFT 的增长导致 NFT 出现了五个新前沿，将 NFT 的创建转移到了使用阶段，下面我们简要列出了这些前沿：

赞助证明：NFT 是获得独家内容和机会的关键。

共同创造和协作所有权：粉丝现在创造内容，而不是被动消费内容。

链上声誉和身份：唯一识别过去行为和效忠的 NFT。

发现和策展平台：查找、发现和组织 NFT 的平台。

NFT 的金融化：NFT 是金融资产​​。

NFT 的五个新领域之一是如上所述的“链上声誉和身份”，它们是唯一标识过去行为和效忠的 NFT，人们将根据他们采取的行动获得不可转让的 NTF，例如“徽章” .人们拥有的 NFT 将是一个独特的指纹，可以根据他们过去的活动来识别他们。此声誉历史将用作链上身份以解锁新机会。因此，Orca 协议已将这种声誉历史用作“成员资格证明（Proof of Membership）”，它将基于 NFT 的成员资格授予工作组，例如治理协议的资助委员会。这些 NFT 可用作解锁链上权限或活动的凭据，例如预算成员可以命令的类型。

**IV. 联系信息**

Official website: https://www.orcaprotocol.org/

Discord: https://discord.gg/SuwhTX4s

Twitter: https://twitter.com/orcaprotocol

**Orca Protocol: A  lightweight community minting and management platform**

DAOrayaki DAO Research Grant：

Fund Address: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

Voting Result：DAO Committee /7 Yes

Grant Amount：200 USDC

Category: Orca Protocol, DAO, Governance, PODs, proposal management, gas efficiency, on-chain voting, Aave Credit Delegation, Aave Governance, Solidity, ENS

Contributor：Jones, Julie, DAOctor @Daorayaki

Launch time: Orca Protocol joined the blockchain community on December, 2020, and supposed to be launched in 2021 spring season, but according to the team it coming later this year.

**Brief Overview about Orca Protocol**

The Orca Protocol is a lightweight community minting and management platform, empowering on chain communities to create, shape, and act in ways according to their values. The needs and shapes of these organizations vary dramatically and existing DAO frameworks lack the adequate systems or flexibility to accommodate the range of use cases.

**I.Background:**

There is not that much information about the Orca Protocol since it’s a new project that has not been settle down yet clearly it is a protocol that concerns DAO governance and proposals management. It is no secret that existing DAOs have a usability problem. DAOs have traditionally been either overly complicated or not robust enough. Moreover, the current governance framework lacks ways to meaningfully manage hierarchy and permissions leading to voter apathy and misaligned voter incentives. On-chain governance has simply not reached its full potential. While traditional DAOs are interested in managing the thousands and potentially millions of actors in a single space, Orca protocol team is more interested in managing the many actors through modular working groups called “**pods**”.

By structuring an organization into smaller, more effective action units, (pods in a modular, lego-like build), organizations can better govern, organize, and manage themselves. In this modular system, organizations (through collective decision-making) decide their own checks and balances system while also allowing for collective ownership, group autonomy, and flexible hierarchical structures. Furthermore, Governance is an extremely complicated and usually a subjective/biased mechanism. Through the Orca Protocol, an objective modular governance tools are possible to build for organizations to build their own governance system.

**II.Team members:**

-       **Julia Rosenberg –** Co-Founder of Orca Protocol and the Founder of Overlly, previously worked as Corporate Development, M&A at Acreage Holdings for nearly one year, and as research and development part for Lloyd Harbor Capital Management, LLC and Archutas Ventures.

-       Twitter Account: <https://twitter.com/JulzRoze>

-       **John Sterlacci** – Co-Founder of Orca Protocol Currently, worked as an adjunct instructor at Binghamton University.

-       Twitter Account: <https://twitter.com/johnsterlacci?lang=en>

-       **Daniel Thompsom** – Software Engineer at Orca Protocol with a background in research and languages. Daniel uses his fascination with the intersection of language and technology in his approach of coding, delivering creating and innovative solutions. An enthusiast of blockchain, as well as the disruptive nature of decentralized applications, and aim to use Web3 technologies to reshape digital communities.

-       Twitter Account: <https://twitter.com/fl0ridadan>

-       **Steven Valeri –** there is not much information available about Steven Valeri but as far as we can see from his Gitub profile he is more likely to be a Software Engineer at Orca Protocol currently.

-       Github profile: <https://github.com/stevenvaleri>

-       **Gressha Mehta** – Product Design at Orca Protocol, previously at Apple, Uber, and Spotify. Mehta is skilled in creating emotion-invoking and interactive experiences for people using the power of story. Currently, she is working as a product designer at Orca Protocol, while in the past she worked at Apple as a Technical Project Coordinator, Uber as a UX Designer, and Spotify as a Brand Designer.

-       LinkedIn Account: <https://www.linkedin.com/in/gresshaa>

**III. What is coming behind Orca protocol?**

Simply put Orca Protocol is designated for gas-efficient, Sybil-resistant DAO implementation using ERC1155. The protocol features a simple UI dashboard to manage DAO proposals and allow on-chain voting for on-chain assets, all secured using Gnosis Safe.

**1.   Orca Pods:**

Orca is made up of pods: organizations that consist of a fixed number of member tokens each representing a single vote. Each pod is linked to a multi-sig vault to securely hold shared on-chain assets.

Pods are flexible and built modularly to accommodate infinite use cases including project governance, pooled investing, community management, and so much more.

![](http://daorayaki.org/content/images/2021/06/--1-3.png)**2.   How it’s made:**

This project is build using Javascript and Solidity. To set up the Orca Protocol dev environment, Orca Protocol team used Hardhat/Waffle, and mainnet forking. In addition to ERC1155 to track the membership tokens, and when it comes to rules, they are stored as Structs that get packed into transactions and executed at runtime. Each pod is connected to a Gnosis Safe instance, and transactions are relayed through the safe. Furthermore more, the first integration included ERC token ownership, AAVE vote delegation, and AAVE proposal delegation. Each of these was encoded into rules to be executed by pods and tested against AAVE Mainnet fork. Additionally, tenderly was used for some of the more complex debugging.

**3.Orca Protocol and NFTs:**

NFT art volume shot up over $200M in March this year on some of the largest marketplaces, only to fall 50% in April. To detractors, this is the "end of NFTs". However, art is the tip of the iceberg and we are rapidly seeing new user cases for NFTs.

The growth of NFTs led to the appearance of five new frontiers for NFTs that shift NFTs creating to a usage phase, below we brielfy list these frontiers:

* **Proof of Patronage:** NFTs are keys to exclusive content & opportunities.
* **Co-creation & Collaborative Ownership:** Rather than passively consuming content, fans now create content.
* **On-Chain Reputation & Identity:** NFTs that uniquely identify past actions & allegiances.
* **Discovery & Curation Platforms:** Platforms to find, discover, and organize NFTs.
* **Financialization of NFTs**: NFTs are financial assets.

One of the five new frontiers for NFTs is the **"On-Chain Reputation & Identity"** as mention above, which are NFTs that uniquely identify past actions & allegiances, people will earn non-transferrable NTFs like "badges" based on actions they have taken. The NFTs that people own will be a unique fingerprint that identifies them based on their past activities. This reputation history will be used as an on-chain identity to unlock new opportunities. Thus, Orca protocol has become used this kind of reputation history as a **"Proof of Membership"** where it gives out NFT-based membership to working groups like a grants commitee for a governance protocol. These NFTs ca be used as credentials to unlock on-chain permissions or activities, like type of budger members can command.

**IV. Contact Information:**

Official website: <https://www.orcaprotocol.org/>

Discord: <https://discord.gg/SuwhTX4s>



---

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）  
  
详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)  
历史文章：

[Synthetix：去中心化治理结构](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484318&idx=1&sn=ebea1216fb8bdaa17de340aec02274a5&chksm=c1d8024bf6af8b5dcc504cefe8129bd910cc6234a2bd6828f6d9e375a97048209149d1b19e8a&scene=21#wechat_redirect)

[Alchemy：预算、协作和DAO管理的去中心化应用程序](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484491&idx=2&sn=d5349b33e7a787156151376914ac22a6&chksm=c1d8059ef6af8c88ba86b617f15373254a62712fb7f1ba2b3bb5d476aac339e2b429426c0ad7&scene=21#wechat_redirect)

[详解Gnosis Safe: 灵活、安全的数字资产管理工具](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484494&idx=1&sn=e2f89b473594c066e30c81e8c737a674&chksm=c1d8059bf6af8c8d2bfaef9a398bad203d4ca95844bd69c55d0703394cadd0cac24aa77c5716&scene=21#wechat_redirect)

[详解Radicle：去中心化社区的代码协作基础设施](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484495&idx=1&sn=eb91cfc99d2de5fd8a2e4b069abad13c&chksm=c1d8059af6af8c8c9d3a6559505eb8e7dad087b93255f1eaac78222f3497ceff7b0c400a9684&scene=21#wechat_redirect)

[DAOMaker: 代币化的创业孵化器和募资平台](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484380&idx=1&sn=c6b092df9c03839de357626b9a167209&chksm=c1d80209f6af8b1fe100bda68669993ede2058b3495df82b0463f5bf50ea567c344137212dbe&scene=21#wechat_redirect)

[SourceCred：基于贡献的计算信用工具](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484383&idx=1&sn=67f820312396793b6aa143159d38c04c&chksm=c1d8020af6af8b1ceb21fb35bc49aa9e289ab7b38bc733283dd7945e2c5df55b729e61847ce5&scene=21#wechat_redirect)

[全面解读｜Colony v2：有效降低市场交易成本的DAO基础设施](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484386&idx=1&sn=9e321dfea0e1a7755464f7b844708a05&chksm=c1d80237f6af8b21ab290d3318c1816dd85a21d91057c3c5abe6a600c7c67aa23a2467481ef1&scene=21#wechat_redirect)

[DAO治理中的同构性](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484493&idx=1&sn=4169ed86c19a17a063dc97c9f6b9b87e&chksm=c1d80598f6af8c8e6cac5807f59a01c8e7d062ee3b9806c18b9a5cb139377a7b3c5b55d0dd1d&scene=21#wechat_redirect)

[自动化奥斯特罗姆（Ostrom）以实现有效的DAO管理](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484492&idx=1&sn=a664c1791f6c5c15dbf7a70bff95f1fa&chksm=c1d80599f6af8c8fbb7de3a133867adc4416db070eafe730fce5ff8510aa8c0b10332ae3c75a&scene=21#wechat_redirect)

[海外最新研讨：数字货币与货币体系的未来](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484492&idx=2&sn=9c5526b818a67958cbfa190b7bbd9ed7&chksm=c1d80599f6af8c8f26c1ac5aecdecb1787d1649ca888b73e8d0d82095bf36c876c72ccdb0a49&scene=21#wechat_redirect)

[可选用的DAOs投票机制汇总](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484491&idx=1&sn=9ec1d8bc2f5c5daa17a439c5196c59be&chksm=c1d8059ef6af8c881434adf485b1394775a35a90dd675348b575c98c986684d0380d48e2b101&scene=21#wechat_redirect)





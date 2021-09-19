


[SourceCred](/tag/sourcecred/)

SourceCred：基于贡献的计算信用工具
======================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



31 May 2021
• 18 min read






![SourceCred：基于贡献的计算信用工具](/content/images/size/w2000/2021/05/1-26.png)



### DAOrayaki DAO研究奖金池：

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 5/7 通过

赏金总量：200 USDC

研究种类：DAO, SourceCred, Contribution Graph, Grain, Tools

贡献者：朱莉白, DAOctor@Daorayaki

代币名称：Grain

代币类型：ERC20

![](http://daorayaki.org/content/images/2021/05/----_20210426113809-15.png)### 1. 介绍

 **SourceCred是一项使个人在参与项目或社区工作时的贡献可量化且有回报性的技术**。SourceCred的目标是使用技术来奖励融入到工作当中。SourceCred希望能在未来可以系统服务社区成员，财务最大化并不是项目的最终目标，而是将财富流向创造价值的人。

### 2.  团队成员

SourceCred是一个开放社区，关于SourceCred开发团队的信息并不多，下面列出了SourceCred项目的主要贡献者：

——Michael Zargham：创始人，研究员，决策工程师，数据科学家；系统工程博士学位，擅长网络治理。

Twitter 账号：<https://twitter.com/mZargham?s=09>

—— Dandelion Mané：软件工程师，融合舞者，务实的理想主义者。

账号地址：<https://medium.com/@decentralion>

—— LB：艺术家，擅长非二进制，负责SourceCred项目第三期“社区孵化”@LBS on Discord

——一些贡献者：

![](http://daorayaki.org/content/images/2021/05/1-25.png)### 3.  **治理和激励机制**

1） Cred

Cred是SourceCred的核心思想。Cred通过参与者为项目做出贡献而获得的分数。参与者的分数反映了他们对该项目的贡献。然后，根据参与者的Cred奖励其Grain代币。

****Cred的特性：****

·Cred面向特定社区

每个使用SourceCred的社区都有其自己的独立“实例”以及特有的Cred分数。他们拥有有“项目共识”，而不仅仅是“整体共识”。每个社区都可以控制Cred在其社区中的流动方式。

·Cred不可转让

参与者的信用评分类似于声誉。这是与他们相关的体系，但不是拥有的资产。Cred不能转让，买卖。

·Cred具有追溯力

Cred分数可以追溯更新以反映新的信息。例如，某人可能写了一篇很棒的论坛帖子，而被忽略。最初，他的Cred收入很少，但是一旦被发现，Cred分数将增加。这使参与者可以将精力集中在工作上，而不必担心没有立刻获得奖励。

·Cred透明度

Cred由算法执行计算，该算法是开源的，所有数据和参数都是公开的。这意味着Cred分数是透明的：始终可以检查Cred分数并找出其计算方式。

**计算Cred**

从高层次看：我们通过首先定义“贡献图”来计算Cred值，该图是贡献、参与者与其之间的联系网络。每个贡献都表示为图中的一个节点。项目选择某些贡献来铸造（mint）Cred，这意味着这些贡献是新Cred的来源。这可以通过自动规则来实现，或者通过人工审核进行。最后，Cred在图中的连接之间“流动”。结果是，如果每个贡献都与赚取Cred的其他事物相关或受其依赖，那么每个贡献都将赚取Cred。如果参与者创作或贡献高信誉贡献，他们将获得Cred。

2）**贡献图**

贡献图是一个数据结构，可跟踪对项目的所有贡献。它是一个图，或者网络的节点和边界。在贡献图中，每个节点代表一个贡献或一个参与者。边代表对象之间的连接。

![](http://daorayaki.org/content/images/2021/05/640.jpg)贡献图，**@**节点代表参与者。为了使SourceCred正常工作，它需要有关存在哪些贡献以及如何连接的数据。主要通过GitHub，Discourse和Discord插件获取数据，这些插件从社区运营的平台导出数据。

**选择权重**

SourceCred的主要原则是让社区决定价值。使用的工具之一是选择“权重”，权重是算法的重要参数。

**权重有两种主要类型：节点权重和边缘权重**

**节点权重**

节点权重决定在节点上铸造多少Cred。例如，如果希望论坛中的每个帖子都添加一些Cred，则可以在论坛帖子上设置正节点权重。但是，这可能不是一个好的决定。由于发布大量帖子非常容易，因此人们可以通过散布大量省力的帖子来获得Cred分数。相反，你可以在论坛上设定一个积极的权重。与帖子不同，“赞”表示其他人认为该帖子很有价值，以此充当对该帖子是否有价值的轻量级评审。进一步的启发式方法可以修改权重，例如确保只有经过验证或信任的用户才能创建Cred，并且如果用户喜欢自己的帖子，则不会铸造Cred。

**边缘权重（Edge Weights）**

边缘权重确定Cred在图形中的流动方式。每个插件都带有默认权重，并将根据团队经验进行校准。但是，用户可以根据需要进行更改。

### 4.  代币

1）Grain

 **Grain是基于Cred分数发行的社区数字货币。**

每个社区使用 Grain的方式不同。在我们的社区中，Grain目前可兑换为USDC，这是一种稳价值1美元的货币。没有基金的社区可能会将其视为未来收入的一部分。也可看作是对社区成员投票的支持。

值得注意的是，Grain不必与任何实际奖励挂钩。使用SourceCred的项目可以将其命名为“points”，除Cred值外，还可以单独用作评分系统。 

 **每个社区都可以选择自己的Grain价格。他们可以选择固定价格，也可以选择将Grain变成浮动金融资产，由市场决定价格。然后，他们的Grain价格将根据供求关系而波动。或者还可以选择让Grain不具有货币价值，而只能在其社区内使用它，例如用于治理或优先排序。**

Grain是针对特定项目的，而不是通用的。每个使用SourceCred的项目都会创建自己的独立Grain代币，并根据社区的选择对其进行调用。

在SourceCred社区中，每枚Grain的固定价格为$ 1。项目可以选择以加密货币或代币形式发行Grain，例如通过在以太坊上发行Grain作为ERC-20代币。这使Grain成为项目向参与者付款或奖励参与者的渠道。

Grain是建立经济和治理机制的基础设施。这里包含两个思想：

·根据cred的信誉分数来支付给贡献者。

·生成使用Grain分数作为背书的应用程序。例如，任何质押一定数量Grain分数的人都将获得Google Docs的编辑权限。

2）**代币分配政策**

Grain分配分为两个步骤，重新计算Cred（最新的分数），然后根据这些Cred分数进行Grain分配。SourceCred对项目如何分配Grain有3个策略：

**·即时（immediate）**

根据每位参与者在上周获得的Cred收入平均分配Grain。（此政策将忽略前几周的Cred，旨在为活跃的参与者提供快速奖励）。

**·均衡（balanced）**

根据全部的信用和收入对Grain进行划分。Balanced尝试确保项目中的每个人都收到与他们的Cred总得分一致的Grain。均衡的政策认为此贡献者的薪水较低，因此它将向他们支付额外的费用，以“赶上”项目中的其他人。相反，贡献者可能被“超额支付”。

**·近期（recent）**

根据最近的Cred使用指数衰减对Grain进行分割，以优先处理最近的cred值。最近一周的衰减率（recent Weekly DecayRate）**参数使得贡献者要将注意力放在最新贡献上。**

3）**Grain的关键特性**

**Grain 的可转让和可交易**

用户可以将其Grain免费发送给其他人，也可以作为协议的一部分进行交换。在项目中，Grain是可替代的。如果将Grain放到区块链上（例如作为ERC20代币），则可以像其他任何ERC20代币一样通过Uniswap或0x等协议进行交易。

**选择获得Grain**

由于Grain具有金融价值，接受Grain可能会给参与者带来法律和/或税收上的麻烦。因此可以自由选择获得Grain；只有明确选择加入的参与者才有资格获得任何Grain。

4）**信任等级（Trust Levels ）**

SourceCred的目的是使社区能够通过Cred和Grain向贡献者分配奖励。但是，这种分配会带来投机性，而这并不是社区价值的部分。为了维持社区安全，它必须能够抵抗投机。

 **SourceCred团队开发了“信任等级”的概念，以试图确定SourceCred准备支持哪些社区，为使用SourceCred的社区提供一个可以选择的架构，并考虑社区在此过程中可能遇到的问题。**

·信任级别3（TL3）：协作。

最高的信任级别。基于社区成员真诚的参与的共识下， 当问其他人相同的问题时，对意外或潜在的投机讨论被视为要共享和分析的宝贵数据，绝不作为任何不当行为的证据。

·信任级别2（TL2）：警惕。

社区的核心贡献者致力于共同的目标，但有些成员可能更着重于提升自己的回报。TL2与TL3的主要区别在于，诚信不再是统一的设想。在别人的帮助下，人们期望投票记录有偏差，并对归属或分配产生争执。

·信任级别1（TL1）：警报。

社区控制着稀缺的资源。社区外部的某些人认为该资源具有内在价值，他们愿意花时间来获取该资源，而无需过多顾虑。TL1与TL2的主要区别在于投机，而不是机会主义的“副业（side hustle）”企图破坏领导和治理结构。

### 5.  合约

SourceCred合约可在Github存储库中找到：<https://github.com/sourcecred/sourcecred>

### 6.  联系方式

Official Website:<https://sourcecred.io/>

**Social Media:**

Twitter：<https://twitter.com/sourcecred>

Discourse：<https://discourse.sourcecred.io/>

GitHub：<https://github.com/sourcecred>

### SourceCred: a contribution-based Calculating Cred tool

### 1.Introduction:

SourceCred is a technology that makes the labor of individuals more visible and rewardable as they work together in a project or community. The goal of SourceCred is to use this technology to make rewarding labor as nuanced as human contribution often is. SourceCred hope to be one piece in the puzzle of a healthier future where systems serve community members, where financial maximization isn’t the end-all be-all goal, and where wealth actually flows to those who are creating the value in the world.

### 2.Team members：

The SourceCred working area is widely opened and There is not that much information about the SourceCred dev team as far as we know, major contributors on the SourceCred project are listed below:SourceCred

——Michael Zargham：Founder, Researcher, Decision Engineer, Data Scientist; PhD in systems engineering, control of networks.

Twitter Account: <https://twitter.com/mZargham?s=09>

—— Dandelion Mané：Software engineer, fusion dancer, pragmatic idealist.

Account: <https://medium.com/@decentralion>

—— LB：an artistic, nonbinary human who heads the “Community Cultivation” third of the SourceCred project.

@LBS on Discord

—— Some contributors

![](http://daorayaki.org/content/images/2021/05/1-27.png)### 3. SourceCred governance and incentive mechanisms:

1）Cred

Cred is the core idea of SourceCred. Cred is a score which is earned by making contributions to a project. A participant's score reflects how valuable their contributions were to the project. Participants are then rewarded with digital currency, or "Grain", based on their Cred.

**Properties of Cred**

· Cred is community-specific

Every community using SourceCred has its own independent "instance", along with its own Cred scores. They have "cred in a project", not just "cred overall". Every community can control how Cred flows within its instance.

· Cred is not transferable

A participant's Cred score is like their reputation. It's something that is associated with them, but it's not an asset that they own. Cred scores can't be transferred, or bought or sold.

· Cred is retroactive

Cred scores can retroactively update to reflect new information. For example, someone might write a great forum post that goes initially overlooked. At first, it earns little Cred, but once it gets discovered, the Cred score will retroactively increase. This frees participants to focus on doing great work, without needing to worry that all of it gets appreciated right away.

· Cred is transparent

Cred is computed by an algorithm. The algorithm is open-source, and all of the data and parameters are public. This means that Cred scores are transparent: it's always possible to inspect a Cred score and find out how it was computed.

**Calculating Cred**

At a high level:calculate Cred by first defining a "Contribution Graph", which is a network of contributions, participants, and connections between them.

Every contribution is represented as a node in that graph. Then, the project chooses certain contributions to "mint" Cred, which means that those contributions are a source of new Cred. This could happen through automatic rules,Or the minting could happen through manual human review. Finally, Cred "flows" across the connections in the graph.

The result is that every contribution earns Cred if it was connected to, or depended on by, other things that earned Cred. Participants earn Cred if they author or contribute to high-cred Contributions.

**2）** The Contribution Graph

The Contribution Graph is a data structure that tracks all of the contributions to a project. It's a Graph, or a network of nodes and edges. In a Contribution Graph, every node represents either a contribution, a participant. Edges then represent connections between these objects.

![](http://daorayaki.org/content/images/2021/05/640-1.jpg)*A stylized Contribution Graph. @-nodes represent participants.*

For SourceCred to work, it needs data on what contributions exist, and how they are connected. It gets this data primarily via GitHub，Discourse and Discord plugins that export data from platforms where the community operates.

**Choosing Weights**

A key tenet for SourceCred is to let communities decide what they value. One of the tools for doing so is choosing "weights", which are important parameters to the algorithm.

There are two major types of weights: node weights and edge weights.

· Node Weights

Node weights determine how much Cred is minted at a given node. For example, if you want every post in a forum to mint some Cred, you could set a positive node weight on forum posts.

However, that would probably not be a good decision. Because it's very easy to make lots of forum posts, people might game the Cred scores by spamming lots of low-effort posts.

Instead, you might set a positive weight on likes on the forum. Unlike a post, a like indicates that someone else found the post valuable, and acts as a lightweight review pass on whether the post was valuable.

Further heuristics can modify the weights, e.g. ensuring that only verified or trusted users' likes will mint Cred, and that if a user likes their own post, it won't mint Cred.

· Edge Weights

Edge weights determine how Cred flows once it is in the graph. Each SourceCred plugin comes with default weights, which is calibrated based on the tem experiments. However, users can change it according to their needs.

### 4. Token:

1. Grain

Grain is a community-specific digital currency that is issued on the basis of Cred scores.

Every community will use Grain differently. In the SourceCred community, Grain is currently redeemable for USDC, a stable coin that is worth 1 US Dollar. Communities without funds might treat this as a share of future income. Another might treat it as weight behind a community member's vote.

Note that Grain does not have to be tied to any actual monetary reward. A project using SourceCred can name it “Points” and use it solely as a scoring system in addition to Cred values.

Each community can choose the price of their own Grain. They can choose a fixed price, or choose to make their Grain a floating financial asset and let the market decide the price; their Grain would then fluctuate in price based on supply and demand. They can also choose for Grain to have no monetary value, and instead only use it within their community, such as for governance or prioritization.

Grain is project-specific, not universal. Every project that uses SourceCred creates its own independent Grain token and calls it whatever their community chooses.

In the SourceCred community, Grain stays at a fixed price of $1 per Grain.

Projects can choose to issue their Grain as a cryptocurrency or token, such as by issuing Grain as an ERC-20 token on Ethereum. This allows Grain to be a conduit with which a project can pay or financially reward participants.

Grain is foundational infrastructure for building economics and governance mechanisms. here's two ideas:

· Pay contributors based on their cred scores.

· Build apps that use Grain scores as certificates. For instance, anyone who stakes some amount of Grain score gets edit permissions on Google Docs.

2.Token Distribution Policies

Grain distribution is a two-step process in which the Cred is recomputed (so scores are fresh as possible), and Grain is then distributed based on those Cred scores.

SourceCred currently has three policies for how a project distributes Grain:

· IMMEDIATE

splits Grain evenly based on how much Cred each participant earned in the last week. (This policy ignores all Cred from previous weeks, and is intended to give fast rewards to active participants).

· BALANCED

splits Grain based both on lifetime Cred and on lifetime Grain earnings. Balanced tries to ensure that everyone in the project receives a total Grain payment which is consistent with their total Cred score. The balanced policy sees that this contributor is underpaid, so it will pay them extra to "catch them up" to others in the project. Conversely, contributors might be "overpaid".

· RECENT

splits Grain based on recent Cred using an exponential decay to prioritize more recent cred. The recentWeeklyDecayRate parameter determines to what degree users want to focus on recent contributions.

3.key properties of Grain

· Grain is transferable and tradeable

Users can send their Grain freely to others, or exchange it as part of an agreement. Within a project, Grain is fungible. If Grain has been put on a blockchain (e.g. as an ERC20 token), it can be swapped or traded via protocols like Uniswap or 0x, just like any other ERC20 token.

· Grain is opt-in

Since Grain can have financial value, receiving Grain might create legal and/or tax complications for participants. As such, Grain is opt-in; only participants that have explicitly opted in will be eligible to receive any Grain.

4.Trust Levels

SourceCred's purpose is to empower communities to allocate rewards to contributors, through Cred and Grain. However, this allocation leads to gaming opportunities which are not part of the community values. For SourceCred to help sustain community safety, it must be resilient to such gaming.

The SourceCred team has developed the concept of "Trust Levels" in an attempt to determine which communities SourceCred is ready to support, provide a structure for communities using SourceCred to use if they choose, and consider what kinds of problems communities might encounter along the way.

· Trust level 3 (TL3): Collaborative.

This is the highest trust level. It is taken as common knowledge that everyone in the community is acting in good faith. Discussions of accidental or subconscious gaming are treated as precious data to be shared and analyzed, never as evidence of any kind of wrongdoing.

· Trust level 2 (TL2): Wary.

The community has a core backbone of contributors that are focused on common goals, but some members may be more focused on optimizing their own rewards. TL2 is primarily distinguished from TL3 by good faith is no longer a uniform assumption. Expect skewed voting records, underrecognition of others’ help, and quarrels over attribution or allocation.

· Trust level 1 (TL1): Alert.

This community controls a scarce resource. That resource is considered intrinsically valuable by some people outside the community, who are willing to devote their time to acquiring that resource without much thought for scruples.

TL1 is primarily distinguished from TL2 by gaming being the main goal rather than an opportunistic “side hustle.” Expect voting cliques, sybils, chains of obfuscated self-dealing, and attempts to corrupt structures of leadership and governance.

### 5. Contracts:

SourceCred contracts are available under following Github repository：

<https://github.com/sourcecred/sourcecred>

### 6. Contact information:

Official Website:<https://sourcecred.io/>

Social Media:

Twitter：<https://twitter.com/sourcecred>

Discourse：<https://discourse.sourcecred.io/>

GitHub：<https://github.com/sourcecred>



---

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）

详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](#wechat_redirect)

历史文章：

[Synthetix：去中心化治理结构](#wechat_redirect)

[DAOMaker: 代币化的创业孵化器和募资平台](#wechat_redirect)

[一份前瞻性暂停使用The DAO的呼吁（2016.5.27）](#wechat_redirect)

[二次方融资（Quadratic Funding）的攻击与防守](#wechat_redirect)

[道德作为通证工程共享（Token Engineering Commons）的使命与动机](#wechat_redirect)

[DAO 联盟|Open DeFi DAO 治理结构](#wechat_redirect)

[策展市场|一种构建联合关注网络的机制](#wechat_redirect)

[Farming机制是否代表着代币分配的进步？](#wechat_redirect)

[全方位解读PANVALA：去中心化的以太坊资助平台](#wechat_redirect)

[Social token与DAO思潮下微观经济体的崛起](#wechat_redirect)

[什么是社区贡献机会（CCO）？](#wechat_redirect)

[万字解读| Upshot One 对等预测协议](#wechat_redirect)








[molochDAO](/tag/molochdao/)

​DAOrayaki研究｜MolochDAO v1、v2、v3
===============================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



21 Jun 2021
• 52 min read






![​DAOrayaki研究｜MolochDAO v1、v2、v3](/content/images/size/w2000/2021/06/o4YBAF05IQSADFd9AAHGbT9Pqpc050.png)



DAOrayaki DAO研究奖金池：

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 4/7 

通过赏金总量：200 USDC

研究种类：MolochDAO, Commons, Public Infrastructures, Minimum Viable DAO, Ragequitting, MolochLAO, Eth 2.0

贡献者：Jones ,黑白QB, DAOctor@Daorayaki

![](http://daorayaki.org/content/images/2021/06/----_20210426113809-23.png)**MolochDAO v1、v2、v3**

**MolochDAO**是一个旨在资助以太坊2.0grants而创建的去中心化自治组织（DAO）。它被设计成一个最小可行的DAO，并使用简单的智能合约功能来减少潜在的攻击。这些智能合约已被分叉，以开发许多其他DAO，如MetaCartel Ventures和Marketing DAO。

**Moloch v2**是MolochDAO的升级版本，旨在将Molchdao的业务范围从单纯的单一代币公共物品资助扩展到收购和投资（或投资）无限资产组合。它使DAO可以获取并使用多个不同的代币，而不仅仅是一种。v2版本中引入了公会踢（Guild Kick）机制，该机制允许成员强行删除另一个成员（他们的资产会被全额退还）。它还允许以战利品的形式发行无投票权的股份。最后，v2修复了最初的Nomic Labs审核中提出的“不安全批准”问题。

**Moloch v3**：即使Moloch非常有用且功能强大，它也具有许多不必要的功能。此外，还有一些功能缺失，并且很难更改。因此Moloch3将可插拔的模块化的方法引入体系结构，该方法将提供：

* 更简单的代码，每个部分都会做一些更具体的事情，这意味着更容易理解。
* 适应性强，DAO的每个部分都可以适应使用它的人的需要，而不需要每次都对整个代码进行审计。
* 可升级，一旦需求发生变化，应该更容易进行部分升级。最好的例子是投票，也许投票的方式会随着时间的推移而变化，可升级性的经济性很强，比如一些模块可被多个DAO使用而不需要重新部署。

Moloch v3的灵感来自于六边形的架构模式，除了将主合约分解成小合约外，还可以提供额外的安全层。有了这个松散耦合的模块/合约，就创造了更容易审计的模块/合约，并很容易地连接到DAO。

**MolochDAO运转**

MolochDAO并没发行代币。成员将Eth贡献给一个池子，同时钱包地址被授予在DAO中的权限和投票份额，这些份额与ERC-20不兼容，以防止它们被买卖。

**I. 背景**

MolochDAO背后的故事

在古代，迦太基人认为在战争中向摩洛克献祭一个孩子会增加他们的胜利，而不参与这一活动的成员则被视为对部落生存的威胁。尽管他们付出了高昂的代价，但因为部落的激励结构，这种做法持续了多年。由此，我们从迦南神“摩洛克”这个名字得到了启发，他代表迦南人牺牲儿童的上帝。

创作者第一次知道摩洛克神是在斯科特-亚历山大的《关于摩洛克的沉思》中，他谈到了艾伦-金斯伯格（Allen Ginsberg）的诗歌《嚎叫-howl》中的同名人物。在《沉思》中，亚历山大指出，虽然金斯伯格通常被解释为讨论资本主义的陷阱，但诗人很可能指的反而是人类在群体协调问题上一贯选择次优方案的倾向。亚历山大给出了一个无独裁者的反乌托邦的例子：

 “想象一个有两个规则的国家：

首先，每人每天必须花费八小时给自己强烈的电击。

其次，如果任何人不遵守某项规则（包括该规则），公开反对，或不执行该规则，则所有公民必须团结起来杀害该人。

假设这些规则已经由每个人都希望它们能够能够强制执行的传统很好的确立了。”

随着时间的流逝，自我强烈电击在所有个人看来都很合理，因为如果他们不这样做，他们将面临死亡。但是，如果我们抛硬币，并假设每个人突然停止电击自己，我们可以肯定，这将为每个人带来更好的社会。亚历山大继续举例说明了一些实际情况，例如过度捕捞，军备竞赛和国会。 

所有这一切都是采纳亚历山大的理由，将摩洛克视为与集体行动相关的一类问题，在这种问题中，个人动机与全局最优结果不一致，需要被打破，以确保人类的长期生存。在MolochDAO的背景下，“摩洛克”这个名字是一个讽刺性的笑话，试图解决协调问题可能都是徒劳的。它本身也是一种模因（meme），希望被视为解决核心问题和认识现实生活中的摩洛克问题的方法。

**需要解决什么？**

将区块链公域（commons）视为一种技术，即该技术对社区产生的总收益大于对任何特定实体的个性化收益，这意味着任何实体投资于开发基础设施的成本与其所产生的收益不成比例。这迟早会导致激励问题，以造成根本无法开发基础设施的问题。

这类问题通常存在于以太坊平台内，更准确地说，是在Eth 2.0的发展中长期存在。正如最近的 “ETH 2.0现状（The State of ETH 2.0） "报告中提到的那样，Eth 2.0的进展缓慢，主要由于研究人员和实施者人数较少且资金有限。尽管所有以太坊项目都能从升级中受益，但只有少数利益相关者直接投入了资金和开发时间。**不幸的是，这是理性的经济行为：为以太坊建设基础设施意味着耗费大量的个人成本，但利益却被整个以太坊生态系统所瓜分。**

**在这种情况下，有什么动力去承担这种成本呢？**

这些类型的问题（称为“ Moloch问题”）需要重新调整激励措施来解决。实现这一目标的方法之一是使用DAO结构来汇集资金并就资金分配进行投票，利益相关者可以更有效地共享以分担成本，从而带来更大的整体生态系统收益。这是作为MolochDAO的一个假设建立起来的，以提供所需的 "激活能量"，触发利益冲突团体间的协调。

MolochDAO愿景

MolochDAO主要致力于资助和增加与Eth 2.0相关的公共基础设施的开发，这是通过激励各个Eth2.0项目与协调主要生态系统利益相关者来完成的。

此外，MolochDAO还考虑对集体激励的研究，并进一步发展适用于更广泛次优化问题的Moloch更通用版本。

**II. 团队成员**

James Young：联合创始人，曾是Ablabed\_io的创始人，Collab\_land的构建者。参与了Prev Zynga（FarmVille），AdToken，Spankchain，DAOs：Moloch，metaCartel。

Arjun Bhuptani：MolochDao的联合创造者，曾是Connext的创始人，Ethreum开发人员，博弈论爱好者。

Ameen Soleimani：Moloch Ventures的创始人，曾是SpankChain的联合创始人兼首席执行官，在离开创建SpankChain之前曾在ConsenSys担任软件工程师近一年。Ameen在Rensselaer Polytechnic Institute任职，创建了Filter的Potomac Code Camp）。 

III. MolochDAO背后机制的想法

为了保持与最小可行DAO架构的一致性，没有设置链上治理机制。相反，如果他们希望参与升级，协议的升级是通过部署新的DAO智能合约和退出Moloch来协调链下的升级。

MolochDAO的机制被认为是深受启发的机制之一，其中对核心问题的各种讨论，如 "公地悲剧--Garret Hardin"、"囚徒困境"、"集体行动逻辑--Mancur Olson"、"公地治理--Elinor Ostrom "都是这个DAO的发展支柱。

统一激励措施

要想找到解决这个问题的办法，就需要对激励机制进行重组，使成本和收益在所有参与者中平均分配。

MolochDAO通过汇集用户资金并将其锁定在一个名为公会银行(Guild Bank)的合约中来实现这一点，另一方面，公会银行的出资者在如何使用这些资金方面拥有投票权，这与他们的贡献/总池的比例是一致的。

该机制被定义为MolochDAO的核心机制，简单明了。然而，还包括了其他机制，使DAO更有趣:

DAO的成员可以清算他们的选票，从公会取回一定比例的资金份额。这为成员提供了强大的经济激励，使他们通过增加他们在资金池中的比例所有权或增加池子的整体价值来最大化他们的选票价值。请注意，清算他们的投票权意味着牺牲整个投票池未来的决策能力。

**个人VS群组利益** 

例如，如果成员需要建设共享的基础设施，这将带来集体利益（以资源价值的增加为代表），那么，是否建设基础设施的价值计算是基于群组的总成本将低于群组的总收益的概率。

换句话说，对于一个理性的投资者来说，当一个提案有可能使资金池的价值增加的幅度超过所有成员分摊的成本时，投资该提案是有意义的。

表示这种成本的最简单的方法是**膨胀指数代币的供应，使所有成员按比例被稀释。**

作为一个类比，想象一下，如果S&P500所代表的50%的公司需要一些开源的会计基础设施。

这个基础设施将花费任何一家公司股票价格的5%来建立，并且只能让每家公司的股票价值提高1%。对于任何一家公司来说，建立这种基础设施在经济上是不合理的，因为成本将远远超过任何好处。 

然而，如果标准普500指数的投资者仅仅增加0.01%(即5%除以500)，通过稀释自己的价值，他们可以支付给一个独立的组织来构建和开源技术，并让每家公司使用新技术。

这将为指数中50%的公司带来1%的股价收益(标普500指数整体收益为0.5%)，这意味着投资者将从指数中获得0.49%的价值。

在此请注意，基础资产（在第一个版本中，以太币）的价值实际上并没有膨胀，只是代表该资产的指数（在MolochDAO中的投票份额）。这很重要，因为投资者（即该指数的主要受益者）是那些支付协调费用的人。在MolochDAO中也是如此。

**限制访问**

DAO的成员被假定至少在某种程度上与总体目标一致——无论是为Eth2.0开发提供资金还是其他一些基础设施目标。第二，假设成员愿意牺牲短期利益来达成DAO的目的。对于ETH 2.0，它的假设是，理性的长期ETH持有者和在该平台上开发的项目将看到其为持续发展做出贡献的价值，避免出现利益者权益下降，技术过时的情况。在真正的无许可范式中，这是不能接受的假设。**取而代之的是，通过让现有成员投票决定是否加入公会，就像资助提案一样。**

这解决了以上两个问题。

首先，现有成员自然会受到激励，他们只接受与行会利益保持一致的新进入者，以便与他们分担费用。对于第二个假设，预计在考虑新申请人时，现有成员将考虑与该申请人以前的互动，这将推动申请人寻求长期利益策略。在下面的“ Ragequitting”中将对此进行更深入的介绍。

**Rage quitting（怒退）**

在任何基于投票的系统中，由于利益相关者可能合谋或不可用产生了许多极端情况。为了处理这些问题，建立一种包罗一切的机制，允许参与者在不同意投票结果的情况下带着他们的资金退出。在对提案进行投票后，同时在成员的所有权受到该提案影响之前，**“宽限期内”允许成员“怒退。** 

比如，99%的公会成员串通一气，提交了一份提案，向他们自己多发行99%的股份，并将剩余的1%稀释到实际为零。在这种情况下，这1%的人将在宽限期内愤怒地退出公会，否定大多数投票集团的攻击。

请注意，宽限期结束后，剩余成员将承担建议的费用。在有争议的投票中，如果有大量少数方退出(例如51%的攻击)，这意味着留下来的人的成本会大大增加。为了执行这一规定，只有在提案通过时投了反对票的成员才会被允许怒退。这些迫使“赞成”通过的人将承担恶意提案的代价。这将为相互合作创造额外有趣的元激励机制，因为公会成员将没有足够的动力提交可能导致其他成员愤怒退出的提案。

读者可能会注意到，**存在一种攻击向量，参与者可以反复Ragequit，来避免稀释或伤害公会。**

这是避免支付单个提案成本的有效方法。但是，如果会员想避免付款，则必须Ragequit全部股份，完全从公会中删除。然后，**他们将不得不重新申请成为会员，并且期望现有会员会重新接纳有缺陷的申请人。从现有的博弈论研究的角度来看，这将促使会员不要滥用该机制。**

**超级竞争与分叉进化**

当有争议分歧时，Ragequit机制可以推动Moloch分裂成多个子实体。

而且，通过让所有成员都退出并重新开始，Moloch得以升级。

这是一个特点，不是一个缺陷。**我们希望Moloch能够被快速分叉、升级和迭代，包括新的链上和链下机制。一个主要的驱动因素是公会规模——成员会被激励去增加资金池价值，因为这意味着每个提案的人均成本会更低，但同时也会被激励去保持公会规模足够小以保持投票权，并保持公会理念与特定目标一致。**一旦这个平衡被打破，新的申请者就会有强大的动机去分叉核心公会并创建自己的公会。由于代码是开源的，而且他们可以很容易地为自己公会的早期参与者添加奖励，最终导致MolochDAOs创造了一个竞争激烈的市场。

**搭便车者**

如果不讨论搭便车的问题，任何解决公地悲剧的方案都是不完整的。简单地说，当成本只由一个或一小部分项目支付时，如何确保其他实体不分享生态系统的利益？当公会银行只用wETH抵押时，解决这个问题是不可能的，因为所有ETH持有者总是会分享到以太坊升级和ETH价格/效用增加的一些好处。然而，有足够多的利益相关者关心Eth 2.0的协调，使molochDAO能够验证其技术和核心博弈理念。

**学老建新**

在构建MolochDAO时，首要考虑的是始终确保存款资金的安全性，创始人将以太坊上过去的重大安全漏洞（如2016年的The DAO黑客攻击和两次Parity multisig黑客攻击）纳入安全开发的设计原则。

首先，也是最重要的一点是，我们设定了一个目标，即只在链上放置绝对最小的功能集。在绝大多数边缘案例中，社会协调机制（离线协调）可以作为问题的迂回解决方案。通过最小化链上协调，减少潜在的攻击面。

第二，创始人决定遵循迭代开发方法，选择只在验证核心博弈理论和技术假设后增加复杂性。

例如，在DAO MVP中，只有wETH被允许使用。虽然这样做并不能让我们验证上面提出的博弈理论的完整性，但通过这种方式构建MVP可以让MolochDAO立即对生态系统有用。

**最后，我们观察到了合约中可升级性的复杂性权衡。因此，我们对基于库的体系结构进行了实验**，但是额外的使用摩擦和增加的攻击面不足以将精力集中在验证核心用例上。因此，从最简单的角度进行升级：参与者可以在需要升级时通过部署新的DAO智能合约来协调脱链，并在他们选择参与升级时退出Moloch。 

**Moloch股份/权益**

MolochDAO使用股份来满足博弈论的条件。股份是按提案要求发行的，预计发行的股份将与申请人的捐款金额（与总资金相比）成比例。**股份授予对如何分配行会银行资源的提案进行表决的权利。他们还可以随时通过Ragequit不可逆转地赎回一部分公会银行的持有资金，与所有权成正比。**

例如，如果行会银行持有100 wETH，并在10个成员之间分配股份，而每个成员都有10股股份，则每股价值为1 wETH，每个成员拥有银行的10％。

如果单个成员离开并清算其10股股票，则行会银行的总价值将降至90 wETH。

但是，每个成员仍然拥有10股股份，因此仍然拥有10 wETH。他们对银行的相对所有权（以及他们的投票权）从10％→11.11％变化。  

股份不可转让。这意味着它们不符合ERC20标准，也就是说，要确保投票不能在公开市场上买卖，因此，如果成员被贿赂提交提案或投票，仍然可以更容易地归咎于他们。 

**加入Moloch**

加入公会需要提交一份入会提案和一份wETH的贡品。入会提案要求以一定数量的股份作为贡品的回报。公会的现有成员对该提案进行投票，包括是否给予所要求的股份。如果入会提案被接受，贡品将被存入公会银行，**新的股票将被铸造并发放给申请人。如果会员提案被拒绝，贡品将被退回。为了减少垃圾邮件，会员提案只能由现有公会成员提交。这意味着申请人在申请时必须说服现有成员支持他们的提案。**此外，会员提案需要10个ETH押金，其中9.9个ETH将在提案处理完毕后返还，无论结果如何。剩余的0.1ETH将用于激励提案的处理。

**中止会员提案**

此结构中讨论的一个漏洞是，成员可能会向申请者恭敬地提交提案，并恶意地请求比申请者期望的预期更少的份额。如果提案通过，则意味着该公会以大幅折扣购买申请者的wETH。

为了解决这个问题，**新申请人可以在“中止期”中止其成员提案资格，该期限自提案提交后立即开始。**在此期间中止将阻止对该提案提交任何投票，并且无论已投多少票，都会导向投票失败。中止将自动将所有贡品退还给申请人，就像他们的提案被拒绝一样。但是，10wETH提案保证金将仅在提案被处理后才退还给提交提案的成员。由于他们在提交提案时要求的股份数量不正确是他们的错，他们不应该从申请人中止提案中获益（通过提前退还他们的保证金）。

请注意，默认情况下，molochao将有一个中止期，持续到投票期的1天。这可以阻止潜在的悲痛因素，即申请人为了浪费会员的时间而恶意地创建提案，并将其中止。会员可以放心地对已经进入投票期至少1天的提案进行投票，因为他们知道这些提案不能再被取消了。

**提交资助（grant）提案**

提交资助提案时，采用与会员提案使用的基本合约机制相同。如上所述，该提案只能由公会成员提交。在这种情况下，提案将载有一些工作，以换取所要求的数量的股份。为了保存记录，建议详细信息可以哈希化并存储在IPFS上。

成员们随后对该提案进行表决。如果被接受，公会银行将发行新股并交给资助申请人。

**提案投票**

提案按照提交的顺序进行投票，并可以在某些限制下进行并行投票。对于MVP，每个提案的投票期为7天。每天最多可以提交5个提案，因此在任何时候最多可以有35个提案被投票（每个提案错开4.8小时）。此外，**投票是以简单多数获胜，没有法定人数要求。与其他投票系统不同的是，Moloch提供了一个宽限期**，在此期间，投反对票的成员可以退出。

另一方面，成员只能对提案进行一次表决。投票在投票期结束时，但在宽限期开始之前或随后发行新股之前进行计票并最终确定。这意味着新股发行的申请将不会增加对积极提案的赞成票或反对票。此外，在一项提案上愤怒退出的成员不会从另一项积极提案的投票中移除他们的选票。因为投反对票的会员不会被扣分，而投赞成票的会员不能“怒退”，提案的投票结果在投票结束后即为最终结果。

**宽限期**

投票结束后，宽限期开始。如“Ragequitting”中所述，宽限期为7天，允许会员在强烈反对投票结果时退出公会。成员只有在对提案投反对票时才能自由退出。对通过的提案投赞成票的成员将被迫承担该提案的稀释费用。在宽限期结束时，**通过调用processProposal函数来处理提案。**从10 ETH提案保证金中扣除0.1 ETH作为奖励，发给调用该函数的会员，以激励其及时处理。 

因为提案是并行的，所以有一些关于愤怒退出和宽限期的边缘案例。首先，退出一个提议意味着所有正在进行的(即正在投票的)提议和所有其他目前在宽限期内的提议都不会影响成员。这可能会导致一个不好的结果，如果他们同时发行的另一个提案正在处理股份(从而抑制他们ragequing)。也可能出现这样的情况: 新申请人在加入并发行股票后，立即受到稀释，因为在他们之后就有恶意的提议排队等候。这些类型的案例由交错队列处理。在最坏的情况下，会员最多有4.8个小时的时间来处理之前所有的提案，他们仍然可以愤怒退出。

**稀释约束**

作为一种安全机制，稀释约束的建立是为了阻止一大批串通的行为者通过所有怒退的方式迫使少数公会成员在一次打击中经历大规模稀释。ADilution Bound字段是在合同中指定的（默认=3），它限定了一个成员可能遭受的最大稀释。  

例如，如果公会中80%的投票权同时Ragequit，剩下的成员将遭受5倍的稀释。当提案被处理时，稀释约束将被触发，提案将失败，即没有新的股份被发行。由于Ragequitters将获得他们所持有的eth比例，公会银行的总余额将减少，但其余成员将拥有与提案处理前完全相同的eth。如果未退出的成员愿意，他们可以重新提交提案。 

**初始化公会**

由于向公会添加新成员和铸造新投票权股份的过程需要所有公会参与者投票，因此向公会添加最初的一组参与者需要不同的过程。

然后，该成员利用手中的一票表决权，通过发行股票以固定入场贡品，将一组初始创始人手动添加到公会中。

**IV. Moloch v2**

Moloch v2是MolochDAO的升级版本，它使DAO可以获取并使用多个不同的代币，而不仅仅是一种。它引入了公会剔（Guild Kick）提案类型，该类型允许成员强行删除另一个成员（他们的资产会被全额退还）。它还允许以战利品的形式发行无投票权的股份。最后，v2修复了最初的Nomic Labs审核中提出的**“不安全批准**”问题。

**设计原则**

在开发Moloch v2的过程中，molochDAO坚持其无情的极简主义，在大幅提高实用性的同时，尽可能少地偏离原作。因此，许多功能被再次跳过，该设计代表了一个最小可行的营利性DAO，但它足够灵活，可以支持各种使用去中心化的情况，包括风险基金、对冲基金、投资银行和孵化器。

概述

**Moloch v2旨在将Molchdao的业务范围从单纯的单一代币公共物品资助扩展到收购和投资（或投资）无限资产组合。**Moloch v2中的提案现在指定了 贡品 和一个 支付代币，可以是任何列入白名单的ERC20。提供贡品代币以换取股份的会员提案现在可以提供任何代币，可能有助于平衡DAO投资组合。资助方案现在可以以股份和稳定币支付，以消除波动性风险，甚至可以完全跳过股份支付外部承包商而不授予成员资格。成员也可以提议交易与公会银行交换场外代币，可用于投资、主动投资组合管理、抛售，或仅用于补充用于支付计划费用的稳定币储备。除上述标准提案外，还有两项特别提案。第一种是将新的代币作为贡品列入白名单，第二种是通过公会踢移除DAO成员。两者都遵循与标准提案相同的投票机制（无法定人数，简单多数规则）。

**MolochLAO** 

**为了限制对营利性部署Moloch v2的成员的法律责任，成员可以选择成立LAO。LAO是包装在合法合规实体（如LLC或C-Corp）中的DAO。**LAO可以签订法律合同，托管离线资产（例如SAFT）并分配股息。LAO的投资者必须获得认可，但是以LAO股份补偿的服务提供商可以赚取其LAO投资组合中的股份。当前的Moloch v2合约标准是通过MetaCartel，ConsenSys的The LAO和Moloch之间的协同努力而设计的。MetaCartel Venture DAO是Moloch v2的首次部署，为其他营利性DAO开辟了道路。 

**安全代币**

为了与SAFT等链下证券对接，MolochLAO将发行遵循债权代币标准ERC-1843和简单受限代币标准ERC-1404的安全代币。在分发SAFT代币时，LAO托管人将把它们发送到债权代币合约，以分发给债权代币持有人。

对于股权、债务或其他收益证券，LAO托管人将收到收益，清算为适合股息的代币（如DAI），然后将股息代币发送到债权代币合约，以分配给债权代币持有人。

怒退并收到他们在所有LAO持有的证券索赔代币中的一部分的成员，仍然能够使用他们的各种索赔代币，从每个索赔代币合约中提取他们的股息。转让限制将被强制执行，即安全索赔代币只能转让给其他DAO成员，或其他由LAO管理员白名单的地址。 

**V. Moloch v3**

即使Moloch非常有用且功能强大，它也具有许多不必要的功能。此外，还有一些功能缺失，并且很难更改。这就是为什么将更模块化的方法引入Moloch体系结构的原因，该方法将提供：

* 更简单的代码，每个部分都会做一些更具体的事情，这意味着更容易理解。
* 适应性强，DAO的每个部分都可以适应使用它的人的需要，而不需要每次都对整个代码进行审计。
* 可升级，一旦需求发生变化，应该更容易进行部分升级。最好的例子是投票，也许投票的方式会随着时间的推移而变化，可升级性的经济性很强，比如一些模块可被多个DAO使用而不需要重新部署。

Moloch v3的灵感来自于六边形的架构模式，除了将主合约分解成小合约外，还可以提供额外的安全层。有了这个松散耦合的模块/合约，就创造了更容易审计的模块/合约，并且可以很容易地连接到DAO。V3架构主要由3种主要类型的组件组成： **核心模块**

* 核心模块跟踪DAO的状态变化。
* 每个核心模块通过接口定义，实现，并在DAO创建时注册到DAO注册表模块。
* 核心模块名称注册表跟踪所有注册的核心模块，因此在调用执行时可以验证它们。
* 只有适配器或其他核心模块才允许调用核心模块的功能。
* 核心模块不直接与外部世界通信，它们需要通过一个适配器。
* 每个核心模块都是一个智能合约，在其功能上应用了 "onlyAdapter "和/或 "onlyModule "修改器，它不应该以公开的方式暴露其功能（外部或公共修改器不应该被添加到核心模块的功能中，除了只读的功能）。

**适配器**

* 从外部世界调用的公共/外部可访问函数。
* 适配器不跟踪DAO的状态，他们可能会使用存储，但理想的情况是，任何DAO相关的状态变化都会传播到核心模块中。
* 适配器只是执行智能合约逻辑，通过调用核心模块来改变DAO的状态，它们也可以组成复杂的调用，与外部世界互动，拉动/推送额外的数据。
* 每个适配器都是一个非常专业的智能合约，旨在很好地做一件事。

适配器可以有公共访问权，也可以只对DAO的成员进行访问（onlyMembers修改器）

![](http://daorayaki.org/content/images/2021/06/640-9.png)**外部世界**

RPC客户端负责调用适配器的公共/外部函数，与DAO核心模块进行交互。

主要的想法是根据每一层来限制对合约的访问。外部世界（例如：RPC客户端）只能通过适配器访问核心模块，决不能直接访问。每个适配器将包含所有必要的逻辑和数据，在调用过程中提供给核心模块，而核心模块将跟踪DAO中的状态变化。这个想法的初稿在融资适配器中实现，它允许个人提交grant的请求。信息总是从外部世界流向核心模块，而不是反过来。如果一个核心模块需要外部信息，应该通过一个输出适配器提供，而不是直接调用外部世界信息。

**VI. Contracts**

Github repository: <https://github.com/Moloch-Mystics>

**VII****. **参考文献****

[Moloch Wikipedia Page](https://en.wikipedia.org/wiki/Moloch)

[Meditations on Moloch - Scott Alexander](https://slatestarcodex.com/2014/07/30/meditations-on-moloch/)

[Howl - Allen Ginsberg](https://www.poetryfoundation.org/poems/49303/howl)

[Logic of Collective Action - Mancur Olson](https://www.hup.harvard.edu/catalog.php?isbn=9780674537514)

[The State of Ethereum 2.0 - Kyokan](https://docs.google.com/document/d/1PS0k9MaKPdPwEw3Uh9rq7USjq7LcSpT6ICQUXRij4YE/edit)

[Funding the Evolution of Blockchains - Fred Ehrsam](https://medium.com/@FEhrsam/funding-the-evolution-of-blockchains-87d160988481)

[The Tragedy of the Commons - Garrett Hardin](https://science.sciencemag.org/content/162/3859/1243.full)

[The Prisoner’s Dilemma](http://pespmc1.vub.ac.be/PRISDIL.html)

[Governing the Commons - Elinor Ostrom](https://www.amazon.com/Governing-Commons-Evolution-Institutions-Collective/dp/1107569788)

[Iterated Prisoner’s DIlemma Strategies - Juriˇsi ́c et al.](https://bib.irb.hr/datoteka/583494.1818-A-Review-of-Iterated-Prisoner-s-Dilemma-Strategies-v1_2.pdf)

[Accelerating Evolution Through Forking - Fred Ehrsam](https://medium.com/@FEhrsam/accelerating-evolution-through-forking-6b0bba85a2ba)

**V. Contact informations:**

Official Website: <https://www.molochdao.com/>

Twitter: <https://twitter.com/molochdao>

Discord: <https://discord.gg/M3AkgBxs>

Github: <https://github.com/Moloch-Mystics>

**MolochDAO v1、v2、v3**

DAOrayaki DAO Research Grant：

Fund Address: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

Voting Result：DAO Committee 4/7  Yes

Grant Amount：200 USDC

Category: (MolochDAO, Commons, Public Infrastructures, Minimum  Viable DAO, Ragequitting, MolochLAO, Eth 2.0)

Contributor：Jones ，黑白QB DAOctor@Daorayaki

****What is MolochDAO?****

MolochDAO is a decentralized autonomous organization ([DAO](https://messari.io/resource/dao)) created to fund Ethereum 2.0 grants. It was designed as a minimum viable DAO and uses simple smart contract functions to reduce the potential attack surface. These smart contracts have been forked to develop numerous other DAOs such as [MetaCartel Ventures](https://messari.io/asset/metacartel-ventures/profile) and [Marketing DAO](https://messari.io/article/ethereum-marketingdao-launches)

****How it works?****

MolochDAO does not utilize a token. Members contribute Eth to a pool and the coinciding wallet address is granted access and voting shares into the DAO, which are ERC-20 incompatible to prevent them from being bought and sold.

**I. **Background****

****Purpose****

****What is the story behind Moloch?****

In ancient times, Carthaginians believed that sacrificing a child to Moloch during the war would increase their victory, while members who doesn’t participate are seen as a risk for the tribe’s survival. This practice continued for years, despite the high price they are giving and that is because the tribe incentive structure played a huge roll in this. From this the name “Moloch” was inspired which signifies to the Canaanite God of child sacrifice.

The first-time knowing Moloch for the creators was in “Meditations on Moloch” by Scott Alexander, where he talks about the eponymous character from Allen Ginsberg’s poem, Howl. In Meditations, Alexander points out that, while Ginsberg is typically interpreted as discussing the pitfalls of capitalism, the poet is likely instead referring human beings’ tendency to consistently choose suboptimal solutions to group coordination problem. Alexander gives the following example of a dictatorless dystopia:

****“Imagine a country with two rules: first, every person must spend eight hours a day giving themselves strong electric shocks. Second, if anyone fails to follow a rule (including this one), or speaks out against it, or fails to enforce it, all citizens must unite to kill that person. Suppose these rules were well-enough established by tradition that everyone expected them to be enforce.”****

With time self-shocking becomes rational to all individuals because if they don’t eventually, they will face death. However, if we flip the coin and assumed that everyone suddenly stops shocking themselves all at once, we are quite sure that this will result a better society for everyone. Alexander goes on to give similar examples from several real-world situations, such as overfishing, arm races, and congress.

All of this was an inspiring reason to adopt Alexander by seeing Moloch as the category of problems associated with collective action, where individual incentives are misaligned with globally optimal outcomes, which needs to be beaten to ensure the long-term survival of humankind. In the context of the MolochDAO, the name “Moloch” is an ironic joke about the possible futility of attempting to solve coordination problems. It is also a meme in and of itself one which is hopefully seen as a solution for the core problem and the recognition of real-life Moloch problems.

****What needs to be solved?****

Seeing the blockchain “commons” as technology where the total benefit generated by the technology to the community is greater than the individualized benefit to any particular entity, means that the cost for anyone entity to invest in developing infrastructure is disproportionate to the benefit accrued by it, which soon or later will lead to an incentivization problem, often resulting the infrastructure to not be developed at all.

These kinds of problems usually reside within the Ethereum industry, more accurately along the development of Eth 2.0. As the recent “The State of ETH 2.0” report mentioned that the progress towards Eth 2.0 has been slow and conducted mostly by a relatively small group of researchers and implementers with limited funding. Despite the fact that all Ethereum projects stand to benefit from the upgrade, only a few major stakeholders are directly involved in funding and development. Unfortunately, this is rational economic behavior: building infrastructure for Ethereum means incurring a large personal cost but benefit is split between the entire Ethereum ecosystem. What is the incentive to bear that cost while that is the case?

These types of problems, known as the “Moloch problems”, require realigning incentives to solve. One of the ways to do that is using a DAO structure to pool funds and vote on fund allocation, stakeholders share more effectively coordinate to share costs, resulting in a greater overall ecosystem benefit. This was built up as a hypothesis for MolochDAO to provide the required “activation energy” to trigger widespread coordination between groups which otherwise may have competing interests.

****MolochDAO vision****

MolochDAO mainly concentrates on funding and increasing the development of public infrastructures related to Eth 2.0, which is done by incentivizing coordination between the various Eth 2.0 projects and major ecosystem stakeholders. Additionally, MolochDAO takes into consideration researching collective incentivization and going further to a more generalized version of Moloch that is applicable to an even wider range of suboptimization problems.

**II. **Team members****

**- **James Young:**** VP of Engineering (James is the founder of Abriged\_io, Makers of Collab\_land. Prev Zynga (FarmVille), AdToken, Spankchain. DAOs: Moloch, metaCartel).

**- **Arjun Bhuptani:**** Co-founder of Connext (Arjun is the Founder of Connext, an Ethreum developer, game theory enthusiast). Currently, he is the Co-creator of MolochDao

**- **Ameen Soleimani:**** Co-founder and CEO of SpankChain (Ameen worked as a software engineer at ConsenSys for almost a year before leaving to start SpankChain. Ameen studied chemical engineer at Rensselaer Polytechnic Institutem founded Potomac Code Camp, Filter). Currently, he is the founder of Moloch Ventures.

**III. **The ideas Behind MolochDAO’s mechanism****

To maintain consistency with the minimum viable DAO architecture there is no on-chain governance mechanism. Instead, upgrades to the protocol are coordinated off-chain by deploying a new DAO smart contract and exiting Moloch if they wish to participate in the upgrade.

MolochDAO’s mechanism is considered one of the heavily inspired mechanisms, where various historical discussions of the core problem such as “Tragedy of the Commons – Garret Hardin”, “The Prisoner’s Dilemma”, “Logic of Collective Action – Mancur Olson”, “Governing the Commons – Elinor Ostrom” was used to identify the pillars of such a DAO.

****Aligning Incentives****

Finding a solution to this problem requires restructuring incentives so that costs and benefits are split equally amongst all participants. The MolochDAO does this by pooling user funds and locking them up in a contract called the Guild Bank, from the other hand the Guild Bank contributors are given voting rights over how those funds should be spent, proportional to their contribution relative to the total pool.

![](file:///C:/Users/user/AppData/Local/Temp/ksohtml23196/wps1.jpg)This mechanism is defined as a core mechanism of MolochDAO which is simple and straightforward. However, additional mechanisms are also included to make the DAO much more interesting:

Members of the DAO are able to liquidate their votes to retrieve a proportional share of the funds from the guild. This gives a strong financial incentive to members to try to maximize the value of their votes either by increasing their proportional ownership of the pool or by increasing the value of the pool overall. Note that liquidating their votes means sacrificing decision-making capabilities over the future of the pool.

****Self vs. Group Interest****

If, for instance, members need to build shared infrastructure which would result in collective benefit (represented by an increase in the value of the resource), then the value calculus for whether to build the infrastructure is now based on the probability that the group’s total cost would be lower than the group’s total benefit. In other words, for a rational investor, it makes sense to invest in a proposal when that proposal is likely to increase the value of the pool by more than the cost that is split amongst all members. The simplest way of representing this cost is to inflate the supply of the index token so that all members are diluted proportionally. As an analogy, imagine if 50% the companies represented by the S&P500 need some open source accounting infrastructure. This infrastructure would cost any individual company 5% of their stock price to build and would only improve each company’s stock value by 1%. Building the infrastructure would not be economically rational for any company individually, because the cost would far outweigh any benefit. However, if the investors in the S&P500 inflated the supply of the index by just 0.01% (i.e. 5% divided by 500), diluting themselves down by that amount, they could pay that to an independent organization to build and open source the technology and have each company integrate it. This would yield a stock price benefit of 1% across 50% of the companies the index (0.5% benefit to the S&P500 overall) meaning that the investors would have gained 0.49% value on the index.

Note here that the value of the underlying asset (ether, in this first version) is not actually inflating, just of the index (voting shares in the MolochDAO) which represents the asset. This is important because the investors, i.e. the primary beneficiaries of the the index, are the ones who pay the cost of coordination. This holds true in the MolochDAO as well.

****Restricting Access****

Members of the DAO are assumed to be at least somewhat aligned on overarching purpose - whether it be to fund Eth2.0 development or some other infrastructural goal. Second, it is assumed that members will be willing to sacrifice short term benefit in order to pursue the purpose of the DAO. For ETH 2.0 its assumed that rational long-term ETH holders and projects building on the platform will see the value in contributing to its ongoing development, lest they see the value of their holdings drop and their platform be technologically surpassed. In a truly permissionless paradigm, this would not be acceptable assumptions to make. Instead choosing to restrict access to joining the guild by having existing members vote on new entrants in a similar fashion to funding proposals.

This solves both of the above problems. For the first, existing members are naturally incentivized to only admit new entrants who are aligned with the guild’s interests in order to share costs with them. For the second assumption, it is expected that when considering a new applicant, existing members will consider previous interactions with that applicant which will drive applicants towards longer-term benefit strategies. This is covered more in depth in “Ragequitting” below.

****Ragequitting****

In any voting-based system, there are a large number of edge cases created by possible collusion or unavailability of stakeholders. To handle these, a catch-all mechanism is builtthat allows participants to exit with their funds if they did not agree with the result of a vote. This is done by allowing members to “Ragequit” the guild within a “grace period” after voting on a proposal completes but before those members’ ownership is affected by that proposal.

Let’s say for instance that 99% of the guild colludes and submits a proposal to issue 99% more Shares to themselves and dilute the remaining 1% down to effectively zero. In this case, the 1% would Ragequit the guild during the grace period, negating the majority voting bloc’s attack.

Note that the remaining members after the grace period ends bear the cost of the proposal. In the case of a contentious vote where a large minority exits (e.g. a 51% attack), this means that cost is greatly increased for those who stay. To enforce this, a restriction for Ragequitting is made to only members who voted “No” in a given proposal if the proposal passes. These forces “Yes” voters to bear the cost of a malicious proposal. This is expected to create an interesting additional meta-incentive for mutual cooperation, since guild members would be strongly disincentivized to submit proposals that might cause a large proportion of other members to ragequit.

Readers may note that an attack vector exists where participants can repeatedly Ragequit to either avoid dilution or grief the guild. This would be an effective method to avoid paying the cost of a single proposal. However, if the member wanted to avoid paying they would have to Ragequit the entirety of their shares, completely removing them from the guild. They would then have to reapply as a member, and it is expected that existing members would be hesitant to readmit the defecting applicant. From existing game theoretic research perspective this will be a strong incentive for members to not abuse the ragequit mechanism.

****Hypercompetition and Forked Evolution****

The Ragequit mechanism can push Moloch to fragment into sub-entities when contentious disagreements are reached. Also, Moloch is upgraded by having all members ragequit and start over. This is a feature, not a flaw. Moloch is wanted to be forked, upgraded and iterated on rapidly, both with new onchain and offchain mechanisms. A major driver for this will be guild size - members are incentivized towards increasing the pool value since it would mean a lower per-person cost per proposal, but are also incentivized to keep guild small enough to retain voting power and keep guild philosophy aligned on a specific goal. Once this balance is exceeded, strong incentives are there for new applicants to fork the core guild and build their own. Since the code is open source, and since they could easily add rewards for early participants in their own guild, leading eventually create a hypercompetitive market for MolochDAOs

****Free Riders****

Any solution to the Tragedy of the Commons would be remiss without a discussion of the free rider problem. Simply put, how to ensure that other entities do not also share in the benefit of an ecosystem when the cost is paid only by a single or small group of projects?

Solving this problem is not possible when the Guild Bank is collateralized only with wETH as all ETH holders would always share in some of the benefit of Ethereum’s upgrade and the increased price/utility of ETH. However, there are enough stakeholders who care enough about coordinating around Eth 2.0 that the molochDAO is able to validate the technology and core game theory.

****Learn from the old to build the new****

In building the MolochDAO, the first concern was to ensure the security of deposited funds at all times, where the founders looked to past major security breaches on Ethereum, such as the 2016 DAO hack and both Parity multisig hacks, to put together a set of design principles for secure development.

First and foremost, a goal of putting only the absolute minimum set of functionality on-chain is set. In the vast majority of edge cases, social coordination mechanisms (offline coordination) can be used as roundabout solutions to problems. By minimizing on-chain coordination, the potential attack surface is reduced to account for.

Second, the founders decided to follow iterative development methodology by choosing to only increase complexity upon validation of core game theory and technology assumptions. For instance, in the DAO MVP, only wETH is allowed as a tribute. While doing it this way does not let us validate the entirety of the game theory proposed above, building the MVP this way allows the MolochDAO to be immediately useful to the ecosystem.

Lastly, complexity tradeoffs to building in upgradeability in contracts are observed. Thus, an experimentation with a library-based architecture is done, but the additional friction of use and increased attack surface were not valuable enough to focus on over validating the core use case. As such, upgrading from the simplest standpoint: participants can coordinate offchain when an upgrade needs to happen by deploying a new DAO smart contract and exit Moloch if they choose to participate in the upgrade.

****Moloch Shares****

The MolochDAO uses Shares to satisfy game theoretic conditions. Shares are requested on a per-proposal basis and are expected to be issued proportional to the applicant’s tribute amount as compared to the total pooled funds. Shares confer the right to vote on proposals for how the resources in the Guild Bank should be allocated. They can also be irreversably redeemed via Ragequit for a portion of the Guild Bank’s held funds at any time proportional to ownership.

![](file:///C:/Users/user/AppData/Local/Temp/ksohtml23196/wps2.jpg)For example, if the Guild Bank holds 100 wETH with Shares distributed among 10 members and each member has 10 Shares, then the value of each share is 1 wETH and each member owns 10% of the GB. If a single member leaves and liquidates their 10 Shares, the Guild Bank total value drops to 90 wETH. However, each member still holds 10 Shares and so still owns 10 wETH. Their relative ownership of the GB (and thus their voting power) changes from 10% → 11.11%.

Shares are not transferable. This means they are incompatible with the ERC20 standard, and that is to ensure that votes cannot be bought and sold on the open market, and so that if members are bribed to submit proposal or votes it can still be more easily attributed to them.

****Joining Moloch****

Joining the guild requires submitting a membership proposal along with a tribute in wETH. A membership proposal requests a certain number of Shares in return for the tribute. Existing members of the guild vote on the proposal, including whether to grant the requested Shares. If the membership proposal is accepted, the tribute tokens are deposited into the Guild Bank and new Shares are minted and issued to the applicant. If the membership proposal is rejected, the tribute tokens are returned. In order to reduce spam, membership proposals may only be submitted by existing guild members. This means that applicants must convince an existing member to champion their proposal when they apply. Additionally, membership proposals require a 10 ETH deposit, 9.9 ETH of which is returned after the proposal is processed, regardless of outcome. The remaining 0.1 ETH is reserved to incentivize processing the proposal once it is ready

****Aborting a Membership Proposal****

A vulnerability discussed in this construction is the possibility of a member submitting a proposal with an applicant’s tribute and maliciously requesting fewer Shares than what the applicant was expecting. If the proposal passed, this would mean that the guild purchased the applicant’s wETH at a steep discount.

To counteract this, new applicants are able to abort their membership proposal during an Abort Period that starts immediately when the proposal is submitted. Aborting during this time will prevent submitting any future votes on the proposal and will cause the vote to fail regardless of the votes already cast. Aborting will automatically return all tribute to the applicant just as if their proposal had been rejected. The 10 wETH proposal deposit, however, will still only be returned to the member who submitted the proposal once it is processed. Since it was their fault for submitting the proposal with the incorrect number of shares requested, they should not stand to benefit (by having their deposit returned early) from the applicant aborting the proposal.

Note that, by default, the MolochDAO will have an Abort Period that lasts for 1 day into the Voting Period. This stops potential griefing vectors where applicants maliciously create proposals that they intend to abort in order to waste members’ time. Members can vote with confidence on proposals that have been in the Voting Period for at least 1 day knowing they can no longer be aborted.

****Submitting Grant Proposals****

Submitting a grant funding proposal utilizes the same underlying contract mechanisms as those used by membership proposals. As above, the proposal may only be submitted by a member of the guild. In this case, the proposal would contain some work to be delivered in exchange for a requested number of Shares. For recordkeeping, the proposal details can be hashed and stored on IPFS.

Members then vote on the proposal. If accepted, the Guild Bank mints new Shares and issues them to the grant funding applicant.

****Voting on Proposals****

Proposals are voted on in the order that they are submitted and can be parallelized subject to certain limitations. For the MVP, the voting period of each proposal is 7 days. Up to 5 proposals may be submitted per day and so there are a maximum of 35 proposals being voted on at any given time (each staggered by 4.8 hours). Futhermore, votes are won by simple majority with no quorum requirement. Unlike other voting systems where members are immediately locked into the outcome of a vote, because Moloch provides a grace period during which members who voted No can exit.

From the other hand, members are only able to vote once on proposals. Votes are counted and finalized at the end of the voting period but BEFORE the start of the grace period or the subsequent issuance of new Shares. This means that an application for new Shares issued will not be added to Yes or No votes on active proposals. Additionally, members who Ragequit on one proposal will not be removing their votes from the vote on a different active proposal. Because Ragequitting members who voted No do not have their votes deducted and members who voted Yes can’t ragequit, the vote tally for a proposal is final as soon as its Voting Period is complete.

****Grace Period****

After votes are finalized, the Grace Period begins. As mentioned in “Ragequitting”, the Grace Period lasts 7 days and allows members to exit the guild should they strongly disagree with the outcome of a vote. Members can only freely exit if they vote No on a proposal. Members who vote Yes on a proposal that passes will be forced to bear the cost of dilution from that proposal.  At the end of the Grace Period, the proposal is processed by calling the processProposal function. A reward of 0.1 ETH is deducted from the 10 ETH proposal deposit and sent to the member that called the function to incentivize timely processing.

Because proposals are parallelized, there are some edge cases around Ragequitting and the Grace Period. First, Ragequitting a proposal will mean that all active (i.e. being voted on) proposals and all other proposals currently in the Grace Period will not affect the member. This could result in a bad outcome for the member if they were simultaneously issued Shares in another proposal being processed at the same time (thus disincentivizing them from Ragequitting). It could also be the case that a new applicant, after joining and being issued shares, immediately suffers dilution because of a malicious proposal queued directly after theirs. These types of cases are handled by the staggered queue. In the absolute worst case, a member will always have a maximum of 4.8 hours where all previous proposals have completed being processed and they can still ragequit

****Dilution Bound****

As a safety mechanism, a dilution bound is built to stop a large set of colluding actors from forcing a minority of guild members to experience massive dilution in a single hit by all Ragequitting at the same time. ADilution Bound field is specified in the contract (default = 3) which bounds the maximum dilution that a member can suffer.

For instance, if 80% of the voting power of the guild were to Ragequit all at once, the remaining members would suffer a 5x dilution. When the proposal is being processed, the Dilution Bound would be triggered and the proposal would fail, i.e. no new Shares would be issued. Since Ragequitters would have taken their proportional holdings of ether, the total Guild Bank balance would be reduced but the remaining members would have exactly the same ether as before the proposal was processed. If the remaining members, then wanted to, they could re-submit the proposal.

****Initializing the Guild****

Since the process of adding new members to the guild and minting new Voting Shares requires a vote of all guild participants, adding the initial set of participants to the guild will require a different process.

For the MVP, the MolochDAO contracts will be deployed with one “summoner” member address in the constructor. Then, this member, utilizing their one vote, will manually add a set of initial founders to the guild by issuing Shares for a fixed entry tribute

**IV. **Moloch v2****

Moloch v2 is an upgraded version of MolochDAO that allows the DAO to acquire and spend multiple different tokens, instead of just one. It introduces the Guild Kick proposal type which allows members to forcibly remove another member (their assets are refunded in full). It also also allows for issuing non-voting shares in the form of Loot. Finally, v2 fixes the "unsafe approval" issue raised in the original [Nomic Labs audit](https://medium.com/nomic-labs-blog/moloch-dao-audit-report-f31505e85c70).

****Design Principles****

In developing Moloch v2, molochDAO stuck with its ruthless minimalism, deviating as little as possible from the original while dramatically improving utility. Thus, many features are skipped again and the design represents a Minimally Viable For-Profit DAO, yet one flexible enough to support a variety of use decentralized cases, including venture funds, hedge funds, investment banks, and incubators.

****Overview****

Moloch v2 is designed to extend MolochDAO's operations from purely single-token public goods grants-making to acquiring and spending (or investing in) an unlimited portfolio of assets. Proposals in Moloch v2 now specify a tribute token and a payment token, which can be any whitelisted ERC20. Membership proposals which offer tribute tokens in exchange for shares can now offer any token, possibly helping balance the DAO portfolio. Grant proposals can now be in both shares and a stablecoin payment token to smooth out volatility risk, or even skip shares entirely to pay external contractors without awarding membership. Members can also propose trades to swap tokens OTC with the guild bank, which could be used for making investments, active portfolio management, selloffs, or just to top off a stablecoin reserve used to pay for planned expenses. In addition to standard proposals above, there are two special proposals. The first is for whitelisting new tokens to be eligible as tribute, and the second is for removing DAO members via Guild Kick. Both follow the same voting mechanics as standard proposals (no quorum, simple majority rules).

****MolochLAO****

In order to limit legal liability on members of a for-profit deployment of Moloch v2, the members may opt to form a [LAO](https://www.thelao.io/). LAOs are DAOs wrapped in a legally compliant entity, such as an LLC or C-Corp. The LAO can enter legal contracts, custody offchain assets (e.g. SAFTs), and distribute dividends. Investors in a LAO must be accredited, but service providers compensated in LAO shares can earn their shares of the LAO portfolio. The current Moloch v2 contract standard was designed through a [collaborative effort](https://medium.com/@thelaoofficial/the-lao-joins-forces-with-moloch-dao-and-metacartel-to-begin-to-standardize-dao-related-smart-b6ee4b0db071) between MetaCartel, ConsenSys’s The LAO, and Moloch. The MetaCartel [Venture DAO](https://twitter.com/venture_dao) is the first deployment of Moloch v2 and blaze the trail for other for-profit DAOs to follow.

Security Tokens

To interface with offchain securities like SAFTs, the MolochLAO will issue security tokens that follow the Claims Token Standard [ERC-1843](https://github.com/ethereum/EIPs/issues/1843) and the Simple Restricted Token Standard [ERC-1404](https://github.com/ethereum/EIPs/issues/1404). Upon distribution of the SAFT tokens, the LAO custodian would send them to the claims token contract to be distributed to the claims token holders.

For equity, debt, or other revenue yielding securities the LAO custodian would receive the proceeds, liquidate to a token suitable for dividends (e.g. DAI) and then send the dividend tokens to the claims token contract to be distributed to the claims token holders.

Members that ragequit and receive their fraction of all LAO-held security claims tokens will still be able to use their various claims token to withdraw their dividends from each claims token contract.

Transfer restrictions will be enforced such that the security claims tokens can only be transferred to other DAO members, or other addresses whitelisted by the LAO admins.

**V. **Moloch v3****

Even though Moloch is very useful and powerful, it has a lot of unnecessary features. Also, there are a few features that are missing and are hard to change. This is why a more modular approach has been introduced to Moloch architecture, which will provide:

- Simpler code, each part would do something more specific, this means easier to understand.

- Adaptable, each part is adaptable of the DAO to the needs of the ones using it without the need to audit the entire code bade every time.

- Upgradable, it should be easier to upgrade parts once the need evolves. The best example is voting, maybe the way of voting evolve with time and it is good to be able to upgrade that economic, such as some modules being used by multiple DAOs without the need to be redeployed

Moloch v3 was inspired by the hexagonal architecture pattern that can provide additional layers of security in addition to breaking the main contract into smaller contracts. With this loosely coupled modules/contracts has been created, which are easier to audit, and can be easily connected to the DAO.

V3 architecture is mainly composed of 3 main types of components:

- Core Modules:

- Core modules keep track of the state changes of the DAO.

- Each ore Module is defined via Interface, implemented, and registered into the DAO registry module when the DAO is created.

- The core module name Registry keeps track of all registered core modules, so they can be verified during call executions.

- Only Adapters or other Core Modules are allowed to call a Core Module function.

- Core modules do not communicate with External World directly, they need to go through an Adapter.

- Each core module is a Smart Contract with the “onlyAdapter” and/or “onlyModule” modifiers applied to its functions, it shal not expose its functions in a public way (external or public modifier should not be added to core module functions, except for the read-only functions).

- Adapters:

- Public/External accessible functions called from External World.

- Adapters do not keep track of the state of the DAO, they might use storage but the ideal is that any DAO relevant state change is propagated to the Core Modules.

- Adapters just execute Smart Contract logic that changes the state of the DAO by calling the Core Modules, they also can compose complex calls that interact with External World to pull/push additional data.

- Each Adapter is a very specialized Smart Contract designed to do one thing very well.

- Adapters can have public access or access limited to members of the DAO (onlyMembers modifier).

- External World:

-RPC clients responsible for calling the Adapters public/external functions to interact with the DAO Core Modules

![](http://daorayaki.org/content/images/2021/06/640-10.png)The main idea is to limit access to the contracts according to each layer. External World (e.g: RPC clients) can access core modules only via Adapters, never directly. Every adapter will contain all the necessary logic and data to provide to the Core modules during the calls, and Core Modules will keep track of the state changes in the DAO. An initial draft of this idea was implemented in the Financing Adapter which allows an individual to submit a request for financing/grant. The information always flows from External World to the Core Modules, never the other way around. If a Core Module needs external info, that should be provided via an Output Adapter instead of calling External World directly.

**VI. **Contracts****

All MolochDAO contracts are available under the following Github repository: <https://github.com/Moloch-Mystics>

**VII. **References****

To those whom are interested in the way MolochDAO was inspired and started you can visit the following links listed below:

[Moloch Wikipedia Page](https://en.wikipedia.org/wiki/Moloch)

[Meditations on Moloch - Scott Alexander](https://slatestarcodex.com/2014/07/30/meditations-on-moloch/)

[Howl - Allen Ginsberg](https://www.poetryfoundation.org/poems/49303/howl)

[Logic of Collective Action - Mancur Olson](https://www.hup.harvard.edu/catalog.php?isbn=9780674537514)

[The State of Ethereum 2.0 - Kyokan](https://docs.google.com/document/d/1PS0k9MaKPdPwEw3Uh9rq7USjq7LcSpT6ICQUXRij4YE/edit)

[Funding the Evolution of Blockchains - Fred Ehrsam](https://medium.com/@FEhrsam/funding-the-evolution-of-blockchains-87d160988481)

[The Tragedy of the Commons - Garrett Hardin](https://science.sciencemag.org/content/162/3859/1243.full)

[The Prisoner’s Dilemma](http://pespmc1.vub.ac.be/PRISDIL.html)

[Governing the Commons - Elinor Ostrom](https://www.amazon.com/Governing-Commons-Evolution-Institutions-Collective/dp/1107569788)

[Iterated Prisoner’s DIlemma Strategies - Juriˇsi ́c et al.](https://bib.irb.hr/datoteka/583494.1818-A-Review-of-Iterated-Prisoner-s-Dilemma-Strategies-v1_2.pdf)

[Accelerating Evolution Through Forking - Fred Ehrsam](https://medium.com/@FEhrsam/accelerating-evolution-through-forking-6b0bba85a2ba)

**VIII. **Contact informations:****

****Official Website:**** [****https://www.molochdao.com/****](https://www.molochdao.com/)

****Twitter:**** [****https://twitter.com/molochdao****](https://twitter.com/molochdao)

****Discord:**** [****https://discord.gg/M3AkgBxs****](https://discord.gg/M3AkgBxs)

****Github:**** [****https://github.com/Moloch-Mystics****](https://github.com/Moloch-Mystics)



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





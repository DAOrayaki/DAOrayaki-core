


[Synthetix](/tag/synthetix/)

Synthetix：去中心化治理结构
==================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



26 May 2021
• 12 min read






![Synthetix：去中心化治理结构](/content/images/size/w2000/2021/05/1-18.png)



### DAOrayaki DAO研究奖金池：

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 4/7 通过

赏金总量：150 USDC

研究种类：DAO, Synthetix , Organization Framework, Governance Mechanisms

原文作者:  Kain Warwick

贡献者：Demo, DAOctor @DAOrayaki

原文: Synthetix Foundation Decommissioned

![](http://daorayaki.org/content/images/2021/05/----_20210426113809-11.png)        Synthetix 是一个建立在以太坊上的、去中心化的合成资产发行协议。在 Synthetix 协议中，用户可以铸造、持有并交易多种多样的合成资产，包括法币、大宗商品、股票，还有像比特币、MKR 和 LINK 这样的密码学货币的合成资产。用户可通过在平台上合成资产来获得相关资产的做多和做空风险收益。协议所发行的合成资产（也叫 “Synths”）背后都是有 Synthetix Network Token（SNX）背书的，使合成资产具备价值及得以清算。Synthetix 在 DeFi 生态系统中占据了关键位置，因为它为 DeFi 利用传统金融资产及更多样、更复杂的交易策略提供了通道。

        作为DeFi领域的小天王，Synthetix 自2020年7月起基金会治理转为DAO治理。Kain Warwick指出依靠非营利性基金会来管理一个项目可能使得净收益为负，而这种治理框架最终会被广泛适用于多项目的DAO模式所取代。因此，在该领域的一些项目和社区的帮助下，Synthetix转化为代币持有者治理（token holder governance）的去中心化自治平台。

        Synthetix协议由三个去中心化自治组织（DAO）控制：

        ·protocolDAO，负责控制协议的升级和变量配置；

        ·grantsDAO，为Synthetix生态系统中的公共产品提供资金；     

        ·synthetixDAO，负责管理和部署资金给捐助者和其他项目需要。

        这篇文章将提供每个DAO的最新情况以及Synthetix治理的未来计划。

### 1. protocolDAO

        **protocolDAO**是所有Synthetix合约的所有者，并使用4/8多义词来修改和升级协议。这意味着protocolDAO负责实施由社区通过有大多数人的共识（rough consensus process）程序批准的SIPS和SCCPs。它还负责协议的运行安全，这意味着对主网合约以及Oracles的所有监测和监督。主要的变化将有引入合约升级的时间锁、代币持有人的否决权、系统暂停功能和分散的断路器。

        备注：大多数人的共识（rough consensus process）即找到大体上的一致意见，而不是简单的多数决原则。rough consensus 首次由互联网工程任务组IETF使用，用以形容在做决定时使用工作组里的主流意见，而无须所有参与者的同意。

        Synthetix协议严重依赖外部Oracles来提供现实世界的价格信息，但它也是一个复杂的智能合约套件，尽管经过无数轮的审计，仍然可能包含软件缺陷。这就需要在检测到异常情况时，能够自动或手动暂停协议，以保护Synthetix协议以及Uniswap和Aave等连接协议中的资金。合约暂停功能的问题是，这为审查协议引入了一个危险的攻击载体。我们实施的系统旨在减少这种协议捕获或审查的风险，同时保持资金的最大安全性，并减少用户中断的可能性。

        由于契约可以在系统级和单个synth级自动暂停或手动暂停，实现这一功能显著改善了资金的安全性，同时也极大地降低了审查的阻力。解决这个问题的办法是引入代币持有人对这些状态的控制。下面来看几个例子。

        现在我们来看一个案例，所有protocolDAO成员合谋以扰乱系统。protocolDAO有能力通过不断地提交暂停交易来无限期地暂停合约。如果protocolDAO成员都投票决定无限期暂停系统，而这一行动是恶意的，代币持有人可以投票重新启用系统，推翻protocolDAO。这确保了权力最终由代币持有者而不是protocolDAO掌握。在未来的迭代中，我们将使代币持有者能够移除协议DAO的个别成员，以确保代币持有者的意愿得到维护。这个机制还有一个额外的组成部分，即代币持有人否决权的门槛。

        最初，我们希望门槛很低，但如果一个有争议的变化尽管得到了社区的共识支持，依然一再被少数代币持有者拒绝，那么可以启动一个升级程序来解决争端。在最坏的情况下，社区的根本性分裂可能会导致协议分叉。虽然这在短期内不太可能，但从长远来看，必须确保提供一个公平、公正和合法的治理形式，以确保社区不发生分裂。

        去中心化的断路器功能确保了当合约检测到Oracles中的异常时系统自动关闭。同样，代币持有者的控制权也是这样的存在，即使protocolDAO成员不能或不愿意重新启用系统，代币持有者可以直接投票重新启用系统，确保他们对系统保持最终控制。

        **时间锁定功能（timelock functionality）确保代币持有者对协议升级有最终的监督权。**任何代币持有者都可以通过protocolDAO拥有的委托迁移者合约提出升级。委托迁移者（delegated migrator）是一个自动系统，用于在链上发布和执行协议变更。这意味着对协议的修改不能在没有代币持有者的监督下进行，因为每个建议必须在确认和实施之前至少等待48小时。如果一个代币持有者或protocolDAO成员提交了一个没有社区共识的合约修改建议，它可以在执行前通过代币持有者的投票被否决。这对于抵制审查制度至关重要，本质上是一种例外治理（governance by exception）。只要protocolDAO执行社区共识，每个提议的升级都应该通过，但如果protocolDAO或社区成员试图执行违反代币持有人利益的合约变更，就会被阻止，迫使社区对提议的变更进行探讨并努力达成共识。

### 2. grantsDAO

        grantsDAO负责公益资金，这包括通过奖励SIP冠军来激励社区参与SIP进程，以及资助snx.tools和SNX Link等举措，这些举措为向利益相关者展示关键信息提供了一个可选借口。synthetixDAO已经承诺在未来三年内，每年为grantsDAO提供100万SNX，以确保对公共产品和倡议的持续资助。

        grantsDAO是由社区成员管理的。这是为了确保它是生态系统中的一支独立力量，并为符合社区利益的补助提供资金。重要的是，它还在确保有可选接口与网络互动方面发挥作用，因此，即使核心贡献者未能提供dApp升级和其他增强功能，社区仍将有与合约交互的稳健接口。

        这种接口的去中心化是确保网络不受审查的关键组成部分。未来几个月的一个重点将是资助部署接口和分叉的前端到IPFS和其他永久托管解决方案。这也需要dapps访问链上数据的免许可机制。

### 3. synthetixDAO

        synthetixDAO最初是在代币销售期间作为一个简单的多义词合约创建的，以确保所筹集的资金是安全的，并通过社区共识以最符合网络利益的方式部署。synthetixDAO为澳大利亚的基金会以及世界上许多其他实体提供了运营资金，这些实体为网络的发展做出了贡献。synthetixDAO将继续为网络的发展提供资金，但以前基金会是资金的主要接受者，现在大量的小型实体将直接向synthetixDAO申请捐助资金。

        重要的是，这是一个开放的过程，任何实体都可以向synthetixDAO申请资金，这通常是通过grantsDAO审查进行的，如果提案的范围不在grantsDAO的授权范围内，就会转到synthetixDAO进行审查。随着基金会的退役，synthetixDAO必须不断发展，以确保网络中的所有利益相关者都被代表，并确保任何能做出贡献的实体都能获得资金。目前synthetixDAO有三名成员代表网络中的关键利益相关者，包括核心贡献者和大型代币持有者。我们预计在未来三到六个月内，能够在synthetixDAO的控制下将整个迁移整个链上的资金。在这之前，现有的托管人将代表synthetixDAO管理链外资金。

        未来，成员资格将向代币持有人开放，他们可以登记加入synthetixDAO的兴趣。只要有足够数量的代币持有者支持其成员提案，他们就会被加入到synthetixDAO。最终，我们转型到一个所有的融资建议都是公开的机制，并由synthetixDAO的成员进行投票，他么有权否决为代币持有者保留的否决权。但在过渡时期，目前的操作程序将继续进行。根据目前流动的加密货币、现金和SNX的财库价值，未来多年仍将以目前的烧钱速度运行。

        最初的代币销售筹集了大约3万个ETH。这笔钱在销售结束后被分成三份，1/3被清算，并一直在为网络的运营和发展以及发行前的成本提供资金。1/3被分配给做市商，其中大部分用于在2018年的熊市期间稳定SNX的价格，迄今为止的做市活动已经带来了约10万ETH的未实现收益。鉴于我们长期与以太坊保持一致，并且对以太坊网络的前景充满信心，最后的1/3被保留在ETH中。目前的财库价值是~1.5亿美元或~45万ETH，在这篇文章的时候。虽然我们在对冲2018年ETH价格下跌方面当然可以更加保守，但鉴于我们在过去两年中成功地增加了以美元和ETH为基础的财库价值，同时也为网络的运营提供了资金，我们相信资金管理得到了良好的执行。我们还通过财库销售筹集了少量的额外资金，约600万美元，这对财库绩效也有好处。我们尽可能精简运营成本，在过去的3年中维持了一个小而精的团队。

        上述变化标志着Syntheti治理的阶段性转型，虽然我们已经用“**有大多数人的共识（rough consensus）**”进行了一段时间的治理，但这种转变将更多的权力直接交到了代币持有人手中，而且提供了一个机制来保护代币持有人免受共谋和审查，后者更加关键。转型后，协议变得更加健全，并减少了核心贡献者所需的信任。Synthetix的目标一直是为交换合成资产提供一个不受审查的协议，这些变化则是实现这一目标的重要一步。一如既往，Synthetix社区将继续迭代和测试这些变化，以确保其与我们的长期目标相一致。



---

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）

详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](#wechat_redirect)

历史文章：

[万字解读| Upshot One 对等预测协议](#wechat_redirect)

[Synthetix：去中心化治理结构](#wechat_redirect)

[DAO 联盟|Open DeFi DAO 治理结构](#wechat_redirect)

[策展市场|一种构建联合关注网络的机制](#wechat_redirect)

[Farming机制是否代表着代币分配的进步？](#wechat_redirect)

[全方位解读PANVALA：去中心化的以太坊资助平台](#wechat_redirect)

[Social token与DAO思潮下微观经济体的崛起](#wechat_redirect)

[什么是社区贡献机会（CCO）？](#wechat_redirect)

[如何DAO化|基于社区贡献机会（CCO）机制的去中心化治理](#wechat_redirect)

[罗宾·汉森经典论文（四）|Futarchy：工程设计25个问题](#wechat_redirect)

[罗宾·汉森经典论文（三）|Futarchy：工程设计25个问题](#wechat_redirect)

[罗宾·汉森经典论文（二）|Futarchy：我们应该价值投票、对赌信仰吗？](#wechat_redirect)

[罗宾·汉森经典论文（一）|Futarchy：我们应该价值投票、对赌信仰吗？](#wechat_redirect)





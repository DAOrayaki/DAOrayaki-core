

DAOrayaki｜算法治理实验：DAO治理动态、韧性及崩溃
==============================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



13 Sep 2021
• 27 min read







**DAOrayaki DAO研究奖金池：**

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 3/7 通过

赏金总量：130 USDC

研究种类：DAO, DAO governance

原文作者：Kelsie Nabben

贡献者：Demo, DAOctor @DAOrayaki

原文：Experiments in algorithmic governance continue

![](http://daorayaki.org/content/images/2021/09/image-51.png)“去中心化自治组织”（DAO）是一种承诺“自治”的政治去中心化组织的新形式。2017年，2017 年，奎因·杜邦（Quinn DuPont）撰写了一个书籍章节《算法治理实验：“DAO”——一个失败的去中心化自治组织的历史和民族志》。这些实验仍在继续。本博客系列探讨的问题是：去中心化的自治组织是否有韧性，如果有，它们何时以及如何崩溃（break）？

本博客分为两部分。第1部分探讨了当今区块链社区中现代DAO（modern-day DAOs）概念出现的历史背景。我强调了起源于赛博朋克运动的DAO中政治去中心化的动态，以及在“自治”组织概念中人类角色和算法治理之间的紧张关系，这植根于长期存在的“链上”和“链下”治理辩论。我着重DAO作为社会技术结构，并探讨了一些建立DAO的常见方法，包括 DAOFirst 和“退出到DAO（exit to DAO）”。然后，我通过列出常见的漏洞以供进一步的以太坊民族志（ETHnographic）调查，进一步完善DAO的韧性的方法。

第二部分将观察DAO的运行情况，以探索DAO是否具有韧性（意味着参与者继续参与实现所述目标），如果是这样，是什么赋予了DAO的人类和自动化组件之间的韧性，或什么阻碍了它。

这篇博客是在我为2021年8月5日至7日举行的“智能合约研究峰会”上主持的“DAO的实施”对话之前写的。它也有助于我对“去中心化技术中的韧性”的博士论文的早期分析。我们非常欢迎建设性的参与。

引用格式建议：Nabben, K. “Experiments in algorithmic governance continue: Trying not to fail at Decentralised Autonomous Organisations (DAOs)”. Substack. 29 July, 2021. Available online: https://kelsienabben.substack.com/p/experiments-in-algorithmic-governance.

**1. 引言**

“去中心化自治组织”（Decentralized Autonomous Organizations, DAO）是一种革命性的自我组织方式，在赛博朋克的主流自由主义想象的传统中梦想着，治理由人际网络中的软件代码来管理。基于区块链的工具正处于成熟阶段，足以支持有关这一概念的快速实验。DAO通常被承诺为参与性的、高度民主的系统，提供运营效率。DAO是社会技术的混合体，在 “链上”和“链下”世界中运作。这些系统的性质仍然是新兴的，而这些系统的人类结果仍然没有得到充分的研究。这篇文章探讨了“DAO是否有弹性”的问题。

在我对去中心化技术社区韧性的研究中，我认为所谓韧性（resilience）就是社会-科技系统应对威胁和危机的适应和转换能力。对于DAO，韧性就是DAO在应对社会和技术的攻击以及冲击下的持续力。在社会-技术系统的研究中，我把脆弱性视为与韧性相关的概念。

我将治理视为协调和控制复杂系统的行动领域。DAO需要建立行动领域（初始设置），以及可能的技术、社会和加密经济行动。

**2. 什么是DAO？**

缩写“DAO”代表“去中心化的自治组织”。DAO最初的基本目的是作为一个虚拟实体，成员有权花费资金和修改代码。虽然没有关于DAO的正式定义，因为这些机构形式仍在不断发展，但DAO是一种在没有中央中介的情况下在同行之间进行协调的模式，以实现一个既定目标。

2013年，Bitshares、Steem和EOS区块链的联合创始人Dan Larimer将比特币描述为一种DAO，将加密货币比喻为“去中心化自治公司”（DAC）的股份，目标是通过在自由市场上提供服务为股东赚取利润。五天后，当时在比特币杂志的作者Vitalik Buterin（现在是以太坊区块链的创始人）指出，公司“无非是人和合同的全部”。

此后，DAO的概念被区块链社区普及，特别是在以太坊生态系统中。以太坊协议的软件语言允许自动化、智能合约颁布可组合的治理过程和机制，DAO作为自动化、治理和自治的一个开放的实验领域正在激增。为进一步进行民族志调查，DAO被称为算法治理的场所。

**3. “去中心化”、“自治”和“组织”的历史和目标**

去中心化的自治组织使事物能够以政治上去中心化的方式组织起来。“去中心化”指的是物理计算硬件或对等网络中的“节点”在架构上的去中心化，以及不受可能拥有影响系统的权力的强制当局或中介机构的影响。

“自主”是指独立，或个人和组织本身的自我管理。这不能与自动化相混淆，尽管规则的自动执行会导致自主性。根据Buterin的说法，自治系统的想法早于区块链社区（见Robin Hanson的futarchy，“通过预测市场的组织治理机制”，“自动机”自操作机器，以及小说系列Daemon）。

DAO是赛博朋克的网络和物理自治理想的延续（逻辑上的延伸）。在20世纪90年代，在比特币发明之前，赛博朋克们深入探讨了自动化、数字市场和物理世界结果的想法。一些人甚至主张废除产权，建立“临时自治区”，即“避开正式控制结构”的非等级社会系统的特设、自治领土。DAO在数字空间运作，但延伸到影响物理世界。

2014年，Buterin描述说：“一个去中心化的组织不是由一组人类亲自互动管理的等级结构，并通过法律系统控制财产，而是涉及一组人类根据代码中指定的协议互相互动，并在区块链上执行”。虽然这些想法在今天的开源区块链社区之前就存在于商业、经济学、控制论和政治中，但去中心化的公共区块链使它们成为可能。

分析DAO的一种方法是，什么正在被组织，什么正在被去中心化，以及谁或什么正在被自主化？这不仅包括个人自治，也包括集体自治，以及需要怎样的权衡来优化每一种自治。

**4. 人类在自治组织中的作用**

DAO既适用于公司，也适用于社区。DAO有内部资本（或财产）。DAO的主要利益相关者是投资者、雇员和客户。

Buterin强调的去中心化治理的张力是，在算法可编程的组织中，我们到底有多需要人？虽然一些人的行动对于高阶的专门任务是必要的（而不是相反），但在后工业时代，人在组织的日常运作中越来越不重要。

“在自主代理中，完全没有必要的具体的人类参与；也就是说，虽然某种程度的人类努力可能是必要的，以建立代理运行的硬件，但不需要任何人类存在，意识到代理的存在。” - Vitalik Buterin，2014年。

科幻小说的梦想是，“自主代理”将成为这些组织的参与者，或利益相关者。一个完全自主的代理也就是完全人工通用智能（Artificial General Intelligence, AGI）。这囊括了韧性的本质，即代理可以适应环境，转变和生存，以实现其目标，直到永远。观察“去中心化自治组织”的尝试揭示了社会结果、利益和关注的早期动态，以假设自治系统的作用以及自治代理作为协调基础设施的可能性。

DAO为自己“思考”，以自动化为中心，人类为边缘。

![](http://daorayaki.org/content/images/2021/09/image-52.png)来源：DAO、DAC、DA 等：不完整的术语指南 —— Vitalik Buterin，2014 年。

Voshmgir、Zargham和Emmett在“DAO2DAO关系的概念模型”中说：“这一愿景与国家和企业赞助的监视超级结构形成鲜明对比，后者是由中央机构资助和部署的人工智能进步的主要应用”，2021。

公共去中心化区块链、智能合约和 DAO 的概念提供了探索组织章程中有多少可以转化为软件代码并由智能合约执行的可能性，以从人类的方向自主运行。

区块链机构（如DAO）中被自动化的是对系统的某种程度的信任，以实现数字社会机构的可扩展性和社会的进步。在题为“货币、区块链和社会可扩展性”的著名文章中，Nick Szabo指出，区块链减少了人类“对我们的同伴、中介和外人的脆弱性”，这提高了资源的效率，从而提高了社会可扩展性。“信任最小化是减少参与者对彼此以及对外人和中介的潜在有害行为的脆弱性"—Nick Szabo。DAO打算通过区块链启用的加密信任最小化和自动化效率，减少人类的脆弱性，以产生可扩展的、独立的、自我指导的社会机构和社会。

这些新的、网络物理的制度形式是否确实实现了个人和集体自治还有待观察。下一节将探讨 DAO 的类型、创建 DAO 所采用的常用方法以及 DAO 中弹性的定义，以进行进一步的案例研究分析。

**5. DAO 治理: 链上技术和链下社交**

学者们将两种主要类型的 DAO称为参与式和算法式。参与式DAO（Participatory DAOs）通过智能合约通过分布式共识进行管理，以表明成员的偏好。算法DAO（Algorithmic DAOs）旨在完全由算法控制，底层智能合约决定DAO的全部功能。

参与式DAO的一个例子可能是GitcoinDAO，它有一个理事会，可以将治理代币分配给管理员，在论坛上审议提案，对“快照”（一种“链外”投票工具）进行投票，然后执行投票提案，例如分配资金。算法 DAO 的一个例子是 DxDAO，它在没有预定义成员的情况下启动，并且完全由社区运行，无需任何项目或团队的干预，它控制着去中心化的交易协议和其他 DeFi 工具。DxDAO以及其他可能将自己定义为“算法”的 DAO 的目标是“从一开始就尽可能广泛地分布”。

然而，所有DAO都具有参与性和算法性。这就是DAO的独特之处。DAO需要参与，这是一个政治过程，参与决策过程的参与者通过“链下”发生的权力关系相互定位，以及算法治理，这是决策被反映和执行的点“链上”通过使用智能合约。DAO结构和治理的技术（包括密码和算法）组件和社会（包括规范决策，或符合可接受文化价值观的决策）都具有必要性和价值。

这两个组件之间的这种思维差异所表明的，是关于社会组件的价值和风险与区块链社区中技术组件的价值的更深层次的文化动态。这种二元张力在整个区块链历史中反复出现，并植根于区块链治理的历史。

**6. 作为“链上”和“链下”的区块链治理简史**

从历史上看，区块链治理是指区块链协议的软件代码如何变化的区块链规则。围绕区块链治理的想法深深植根于文化中，例如比特币的不变性理想和人与人之间的最小信任，这导致了“代码即法律”的意识形态。关于人们干预算法的作用的争论也被称为“链上”与“链下”治理。

“链上”治理是在软件代码中明确治理规则，区块链节点自动执行协议中的代码升级以响应链上代币持有者的投票过程。相比之下，“链下”治理是指规则不那么正式，在正式、记录、透明的决策之外如何共享、讨论和评估想法的非基于代码的过程最终反映在节点决策升级中 他们的软件传递对协议的更改。因此，点对点网络中的节点是治理过程的积极参与者。

在黑客攻击和关于治理的持续辩论之后，Buterin表示：“那些认为区块链的目的是完全消除人类软弱的直觉和感觉而支持完全算法治理（强调“完全”）的人绝对是疯了”。

今天，以太坊社区通常采用其“链下”、以人为本的流程。例如，以太坊基金会在协议的开发中保持着重要的协调作用，例如聘请研发人员和主持定期的“以太坊改进提案”（EIP）会议。当社区需要协调一个粗略的社会共识挖矿者、交易所和节点运营商来升级他们的软件以在“DAO”黑客之后“分叉”协议时，这种方法的优势是显而易见的。偏向“链下”治理的一个缺点仅仅是效率和可扩展性，以太坊的创始人Vitalik Buterin表示Ethereum2.0协议升级的过程比最初预期的要慢得多。

相比之下，Polka Dot和Tezos等其他区块链社区采用链上治理，其中协议升级通过公投类型投票决定，软件代码是不可变的，这意味着一旦部署就无法更改。这样做的一个优点是代表性和透明度。这种方法的一个缺点是将治理简化为投票，而实际上它是在系统的协调和控制中相互作用的多层社会和技术组件和流程，这是无法提前预测的，因此不可能预先编码到协议规则中。

区块链社区以政治权力下放的价值为导向。链上治理流程建立了明确的治理规则并提供透明度。相比之下，链下治理流程不透明、混乱且具有内在的政治性，但在一定程度上不可避免，并且可能有助于在项目中领导、教育和建立明确且可信的方向。DAO中治理的社会和技术方面的可供性不仅是一种系统设计选择，而且是一种意识形态选择。区块链社区和治理的参与者制定了影响信息和激励的文化规范。

对“链下”或“链上”治理过程产生什么结果和强调，以及在某些情况下哪个更具弹性，还有待分析。

**7. “DAO主义”——现代DAO**

可以肯定地说，DAO 已成为“准网络宗教（quasi-cyber-religion）”。

现代DAO通常是部署在第1层协议区块链之上的“去中心化应用程序”。公共区块链为DAO实验提供的能力得到了当今区块链社区中出现的大量“DAO”方法的证明。

要获得注册公司实体的法律地位（在美国），DAO 必须：

· 部署在公共区块链上，

· 提供唯一的公共地址（已），以便任何人都可以查看他们的操作，

· 软件代码必须开源，软件代码必须经过审计，外行能够读取智能合约变量和代币限制，

· 治理必须在 DAO 的技术架构中去中心化，

· 至少有一名 DAO 成员，

· 一个联络点，

· 对参与者具有约束力的争议解决机制，以及，

· 与 DAO 之外的第三方互动的争议解决机制。

在作为社会技术系统的区块链基础设施中，同时存在两种治理类型：由基础设施治理和治理基础设施。这种双重性在现有 DAO 的角色和功能中都很明显。

DAO 存在用于风险资本分配 (FlamingoDAO)、资助公共产品 (GitcoinDAO)、管理“去中心化金融”(DeFi) 协议，例如自动做市商 (UniswapDAO)、资助寿命延长研究 (VitaDAO) 和构建自身(1Hive)。

这些可以进一步分类，尽管定义仍然很宽泛。 DAO 参与者管理协议的规则，并在 DAO 内提供受协议管理的劳动力。

**8. 通过可组合性实现自治**

通过区块链基础设施的可组合性，DAO正在朝着自治的理想发展。一个DAO，比如1Hive，可以运行在以以太坊为例的一个协议上。唯一身份可以通过去中心化应用程序（如 BrightID）进行验证。它可以通过联合曲线、公平发布或追溯空投获得公共资金。劳动贡献可以用“信用”来确认和衡量。争议可以通过（例如 Aragon 或 Kleros）在分散的法院进行仲裁。并且可以在代码中的黑客或错误导致损失的情况下提供保险。这些提供了模块化、可组合、多层次的机制，用于执行在物理空间和网络空间之间转换的特定治理过程。

下一节概述了通过“DAOFirst”或“退出到 DAO”方法“创建”或“成为”DAO 的常见方法。

**9. Just DAO it （出生，birth）**

来源：“如何启动DAO”，来自 Gitcoin（现为 GitcoinDAO）联合创始人兼首席执行官 Kevin Owocki的推文。

![](http://daorayaki.org/content/images/2021/09/image-53.png)“DAO优先（DAO First）”v.s. “退出到DAO（exit to DAO）”

“通常 DAO就像生物，有自己的主观意识，可以感知、感知、思考、理解和做出决定。” ——马坦场，DAOStack。

DAO正在采取两条主要路线来成为DAO。一个是“DAO优先”方法。另一种是通过渐进式路线过渡到去中心化，我称之为“退出到 DAO”。

**“DAO优先”方法**

Synthetix DeFi 协议的创始人Kain Warwick率先提出了“DAO 优先”方法。DAO优先是指从设计DAO开始就确定代币分配和资本形成的初始规则，而不是建立并从传统公司过渡到DAO的替代方案。

**“退出到DAO”（渐进式去中心化）**

DAO优先方法的替代方案是渐进式去中心化。这种方法在许多项目中都可以看到，其开始时只是一个产品或想法，鉴于DAO工具的成熟度不高，现在希望将决策权“下放（decentralise）”给社区。渐进式去中心化是在项目拥有社区后确定代币分配和资本形成规则。这样做的复杂性在于，需要与社区共同做出决定才能被视为合法地分散项目，但可能会卷入歧义、协议政治和官僚主义（或“fucking yourself”，根据Kain的说法）。

我将“渐进式去中心化”称为“退出到DAO”（这被SCRF的Rich Brown亲切地称为“DExit”）。在Nathan Schneider和Morshed Mannan的“退出到社区（exit to community）”中，有三种工具可以让企业将控制权移交给他们的社区。即：i.信托模型（the trust model），所有权集中在受托人管理的信托中；ii.联邦模型（the federation model），企业由多个独立的企业实体组成，以及，iii．代币化模型（the tokenization model），使用区块链技术。在DAO中，我们看到所有三种工具都在发挥作用：从作为“受托人”的多重签名钱包持有者，确保系统稳定性的代币鲸鱼，以及促进更广泛社区参与的代币化。我指出的风险是，项目创始人迅速退出以“去中心化”到DAO，使这些机构基础设施设计工具的多个底层面临风险。

尽管人们非常重视开启一个DAO，但它们的常见攻击向量以及它们提取价值的方式却很少受到关注。

本文的其余部分旨在探索创建和解决DAO中漏洞的DAO动态，以此作为手段来了解，DAO结构或治理（作为决策规则和流程）的哪些社会和技术方面正在被社会技术算法组合稳定或破坏这些方面的韧性。

**10. 定义DAO的韧性（resilience in DAOs）**

DAO因参与而生，因参与而死。一个有韧性的DAO是一个维持一定数量的参与者以继续追求其既定目的和目标的DAO。DAOStack的联合创始人 Matan Field 表示：“如果去中心化决策系统中的行为确保DAO中做出的所有决定都与其大致意见一致，那么它就具有韧性。” 如果没有一个明确的目的和参与的参与者，对韧性和“成功”的衡量就不明确。因此，韧性是一种按照其自身的使命和治理目的行事的行为。

DAO社区的紧张局势在于如何建立可扩展的、去中心化的、自治的组织，以有效平衡社会和技术动态以实现其既定目标。因此，定义治理面（governance surface）和实施治理（enacting governance）是韧性的关键杠杆。

**DAO的脆弱性（DAO vulnerabilities）**

DAO容易受到社会和技术攻击。

社会攻击包括共谋攻击和女巫攻击。共谋攻击（collusion attacks）是指相当大比例的某种类型的成员串通一气，专门指导DAO的活动。女巫攻击（Sybil attacks）是人们创建多个身份以破坏声誉规则并利用系统的地方。贿赂和中心化也被视为对DAO的威胁，这可能是机制设计（信息和激励）的结果。有一个专门描述治理漏洞的新术语，称为“治理可提取价值（governance extractible value）”，用于描述资本的结构性剥削和短期主义。

技术攻击可以是造成安全错误的软件代码错误，如“The DAO”黑客所示。

这种对一般DAO漏洞的初步分析浮现了文化对参与的重要性，因此也是DAO的韧性的一部分。

**11. DAO生命的基本构成**

![](http://daorayaki.org/content/images/2021/09/image-54.png)《当一家公司成为DAO时》，来自Gitcoin（现为GitcoinDAO）联合创始人兼首席执行官Kevin Owocki的推文

**一种参与的文化**

Blockscience创始人Michael Zargham表示，DAO是“人、工具和流程”的集合。这包括编码为技术参数和信息的文化、规则和激励措施，以实现明确的目标或目的。然后，这些元素在进化的、适应性的过程中相互共同构建，有时会加强DAO的生命（参与上述目标），有时会阻碍它。DAO必须激励参与才能生存。

利润和文化是参与DAO的两个主要激励因素。参与是DAO的重要组成部分。由于DAO 既是社会性的又是技术性的，因此激励参与DAO的一些方面是文化和利润。DAO通常需要两者兼而有之。

当价格上涨时，每个人都听说过加密货币。DAO使用数字代币激励来为参与者建立所需的行为并惩罚不良行为（例如权益证明中的“削减（slashing）”）。DAO部分由堕落者组成，“一种与去中心化金融臭名昭著的角落相关的亚文化，以拉高出货计划而闻名”，被称为“DeFi Degens”。

另一个要素是文化。文化被理解为人类社会的社会行为和规范，表现为个人和群体的知识、信仰和习俗。例如，FlamingoDAO“旨在支持、购买、存档、收集和潜在地标记这个生态系统的重要部分”，特别是NFT。它正在投资于识别和保护有价值的文化艺术品。然而，它由注册投资者组成，并认识到其对这些文化资产的投资的盈利能力。相比之下，1Hive等其他DAO使用数字代币来激励DAO内的劳动力，以促进其自身的发展、增长和可持续性。

**设计文化**

在“数字龙卷风之后”中，Kevin Werbach 认为区块链系统中的治理必须是“按设计”的，不能事后才想到。或许，文化也必须是设计出来的，因为它是通过适应来引导社区并在整个系统的冲击和转变过程中让参与者参与进来的东西。

**12. 总结**

本博客的第1部分概述了DAO的关键历史和文化动态，尤其是DAO治理中人为影响和算法影响之间的紧张关系。我概述了DAO的现代区块链社区概念的历史，DAO 治理中人与算法组件之间的紧张关系，如沉浸在“链上”和“链外”治理辩论中的紧张关系，并概述了建立DAO的一些常见方法，这是以后案例研究的有用描述。

这已经建立了一个基本的DAO词典，通过它可以观察DAO的元素和类别以对抗某些漏洞，以观察和理解DAO中的弹性，作为通过算法治理尝试政治权力下放的例子。

第2部分将通过民族志案例研究观察DAO中常见的社会和技术漏洞。这包括寻找DAO死亡和复活的案例。分析不同类型的DAO（链上和链下治理）如何应对这些将有助于更好地了解通过政治去中心化的自治组织是否可以实现韧性，以及这一现象中参与者和DAO的动态、风险和权衡。  




---

了解去中心化自治组织（DAO），探讨最新治理话题，关注DAO的发展趋势，欢迎加入群聊！

![](http://daorayaki.org/content/images/2021/09/image-55.png)欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）

详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)

历史文章：

[买单投票：一种新型的混合代币投票/Futarchy](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485291&idx=1&sn=ff0ca088955037fa294720f2c1e6e61b&chksm=c1d806bef6af8fa80e64a7f2ae74b596139f40d0cad45a396a4c3979337ba2aa6af4b4089605&scene=21#wechat_redirect)

[DAOrayaki｜Venture DAO生态系统概述](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485290&idx=1&sn=64cd97ea158f34c32869f3dbd9bdd856&chksm=c1d806bff6af8fa943297b2df599d7d8c74b8b2b830d84ecc012de0bac0140c981592618598d&scene=21#wechat_redirect)

[DAOrayaki｜PoolHAUS与去中心化流动性供应](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485283&idx=1&sn=076f4eeb3bcaeca66eb6e7dbaf69f483&chksm=c1d806b6f6af8fa0a9e585e5279f81e5fc067973d213a2f22589488dda74830c768739e4a405&scene=21#wechat_redirect)

[DAOrayaki｜GitcoinDAO 群体思维正在崛起](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485278&idx=1&sn=63416f19a34b866ddf0da9bd736a4d5d&chksm=c1d8068bf6af8f9dced37dacd6cc45d96044ad3cd724b3f083d728fda6b0f06b2f81cf6128e9&scene=21#wechat_redirect)

[DAOrayaki｜连续性公共物品资助](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485274&idx=1&sn=98578d145471283151b61ca337ccf9ac&chksm=c1d8068ff6af8f99ebef0e626da72f758719a81853604d5891f779600fe42b394eea62fa44cb&scene=21#wechat_redirect)

[DAOrayaki｜如何利用社交代币实现长期增长](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485235&idx=1&sn=65643c070b9ed7baf55ed25809d8af68&chksm=c1d806e6f6af8ff00e90178feedbd3a97bdf6e9d764ddb5190f5eaa0de9b30fce6879abf8e69&scene=21#wechat_redirect)

[DAOrayaki｜连续性公共物品资助](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485278&idx=2&sn=0973c0c45206bdccf6832c112f551119&chksm=c1d8068bf6af8f9dd3c2d1dc5e76eac9dc69094928416eb533d31e5f782453127515595db6f0&scene=21#wechat_redirect)

[DAOrayaki｜GitcoinDAO 群体思维正在崛起](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485278&idx=1&sn=63416f19a34b866ddf0da9bd736a4d5d&chksm=c1d8068bf6af8f9dced37dacd6cc45d96044ad3cd724b3f083d728fda6b0f06b2f81cf6128e9&scene=21#wechat_redirect)

[DAOrayaki｜“可追溯公共物品融资”进展分析](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485234&idx=1&sn=4666b41f9501e9b997e5306f7fc54bf0&chksm=c1d806e7f6af8ff17f9c55dee14fca29056f0f15058a08da7702faad81c2ce5d50f3c3fed5c3&scene=21#wechat_redirect)

[DAOrayaki｜Vitalik Buterin：超越代币投票的治理](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485212&idx=1&sn=c3565e9fef0400442ac0aa9ea8282271&chksm=c1d806c9f6af8fdfce9b19c8ad352ca480ebe044735d758539ba26cfbb74adfb29a967e3195f&scene=21#wechat_redirect)

[DAOrayaki｜“可追溯公共物品融资”进展分析](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485234&idx=1&sn=4666b41f9501e9b997e5306f7fc54bf0&chksm=c1d806e7f6af8ff17f9c55dee14fca29056f0f15058a08da7702faad81c2ce5d50f3c3fed5c3&scene=21#wechat_redirect)

[通证工程共享（Token Engineering Commons）：分析权益持有者、通证和治理过程](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485199&idx=1&sn=85752e9d476dfcf1c54ae60e41eedc91&chksm=c1d806daf6af8fcc58d8fc289b93196ac238fe8c5dbd03fc332db08033a5f991540cbf829f89&scene=21#wechat_redirect)

[DAOrayaki｜关于改善配对协调补贴的一个方法探讨](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485197&idx=1&sn=b28b0f7450999d040fdc322ba9148bda&chksm=c1d806d8f6af8fce8e56b1206d431fcf3f18799dbe1afd08bfbac2dc456530bc759440bc40de&scene=21#wechat_redirect)

[DAOrayaki｜针对高度不可能事件押注的预测市场设计](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485192&idx=1&sn=fc0f043a055e70c7a69592d6d0d4aea0&chksm=c1d806ddf6af8fcb9326e37ac8e55b7fdc285b3023406ce44ad1854697698849cf4fa844cd44&scene=21#wechat_redirect)

[DAOrayaki｜DAO 国库多元化的范围代币](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485191&idx=1&sn=25c47e7c527cb48d4ce97bf2785bd4d0&chksm=c1d806d2f6af8fc4f84e53e06cd301cc35a24518c66c91246e3937ed6b0ef7483c8a1b9ea231&scene=21#wechat_redirect)

[DAOrayaki｜二次方投票：机制设计如何使民主激进化](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485100&idx=1&sn=c9da137fd19efa8d342b69dab3de524c&chksm=c1d80779f6af8e6ffc76352b779653d9283f9b00057a122f6b3e6ac61ec9cbdcf7f204c7777a&scene=21#wechat_redirect)

[DAOrayaki｜元数据、数据堆栈、数据目录3.0](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485099&idx=2&sn=2d3f8933133b1231c5b6d57cccbb738b&chksm=c1d8077ef6af8e68634421946416f3d1c3508c28bd8fed63fed844d1777d4f02f747ee44c8bc&scene=21#wechat_redirect)

[DAOrayaki｜二次方投票和区块链治理](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485046&idx=1&sn=21c5550753bb5405ba838eeb7857f2d6&chksm=c1d807a3f6af8eb57ebb1ad7a1b1ba8079ed40e4f60ef36d11930d472d233c8ee3d7b6b88ac3&scene=21#wechat_redirect)[DAOrayaki｜可追溯公共物品融资](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485099&idx=1&sn=59c46a5a5b44dbf3c74c902a2d7c33bd&chksm=c1d8077ef6af8e68247e4557d52e8c7435563ebc25aef988f9986f8881eb244a12a360c82303&scene=21#wechat_redirect)

[DAOrayaki｜二次方投票与公共物品](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485045&idx=1&sn=aff37e0951631c79f7e660f7adf888d0&chksm=c1d807a0f6af8eb656250e092d56aa93dac7f6df9358ec6cf7a9848fac3ee3d3c12d10c47a8e&scene=21#wechat_redirect)

[二次方资助V2协议: 抗女巫攻击、公平和规模化的链上二次方投票](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485044&idx=1&sn=1c0ea021684fc2c8e00cee3c3be83659&chksm=c1d807a1f6af8eb772b7892f23c525ac912ee6a448c8362ca44b2ffb6ae1eeeb42747c0f9e74&scene=21#wechat_redirect)

[DAOrayaki｜全面综述：女巫攻击和防御方法](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484986&idx=1&sn=2e9df8b7db1ccd488eb161428354e146&chksm=c1d807eff6af8ef938a76d7ec10dc91b81414339173b8931aec08a7616f5eae94d95d06c9d3c&scene=21#wechat_redirect)

[DAOrayaki ｜代币经济学导论](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484979&idx=1&sn=ba636f6be333c3a74bf9c9dd49dbd16b&chksm=c1d807e6f6af8ef024ee28871129a35879e2f742f20e902c492e27610313f0cbc1035c87f890&scene=21#wechat_redirect)

[DAOrayaki｜价格与预言机](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484807&idx=1&sn=273c664de6afa9c263f4be0c595d080a&chksm=c1d80452f6af8d44c5c12a9b33313cc3d5df3128d06921ae61c90fd6f494817a91beb29d5508&scene=21#wechat_redirect)

[DAOrayaki｜去中心化自治组织（DAO）行业发展月报（2021.6）](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484806&idx=1&sn=28088c05ecf1c26dcd94ccdc8347be23&chksm=c1d80453f6af8d45040b58692b61c2e2d9bdaf1894d51382ea9042e66fe134f7173c2c5687cd&scene=21#wechat_redirect)

[DAOrayaki｜DAO 通过财政多元化为下一个加密冬天做准备](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484808&idx=1&sn=f089e891fe0c8d0ba6a0c5cf208b9c9b&chksm=c1d8045df6af8d4b37cd79d4efb40d2e0c71d4e2aeb5f322615eecbc06664f452c927a75ae90&scene=21#wechat_redirect)

[加密技术的全面论述—开放金融系统](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484742&idx=1&sn=711607523b7112e1f6dd5dcd855894cf&chksm=c1d80493f6af8d8558574439a91347b54e0a9410cf6a711ed9e75bf2e68543f2d1df8970e640&scene=21#wechat_redirect)

[D2D：面向去中心化的谈判协议](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484740&idx=1&sn=ab336ebc7b925d01e547c14f18f5a8df&chksm=c1d80491f6af8d874266b2b365b0e5847fa5ed12f064b9ac0eb5c8c8a72628afb1b0ccf822df&scene=21#wechat_redirect)

[DAOrayaki解读｜价格敞口和投票权](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484712&idx=1&sn=674e8305b9899f73343eae5d68be6a99&chksm=c1d804fdf6af8deb14b0fb4ae8debb6abef6e96ec0a638768f06da475e097a97cf3f00ea5c8f&scene=21#wechat_redirect)

[Muse Museum率先加入DAOrayaki Funders MolochDAO并开展联合研究](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484739&idx=1&sn=7a15f813ff8ca419221bcba9b14cf2f8&chksm=c1d80496f6af8d8038bc222f8ce4eecf9a4ddf47477fdc12233797e48495884334a23322cce5&scene=21#wechat_redirect)

[D2D：面向去中心化的谈判协议](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484740&idx=1&sn=ab336ebc7b925d01e547c14f18f5a8df&chksm=c1d80491f6af8d874266b2b365b0e5847fa5ed12f064b9ac0eb5c8c8a72628afb1b0ccf822df&scene=21#wechat_redirect)

[DAOrayaki | 去中心化仲裁：Kleros、Aragon、Jur](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484741&idx=1&sn=6dd674ebc05296fa3fe21acada6c1d5f&chksm=c1d80490f6af8d86f57987537135f059d8b95be2267c7f5fb0a1f4af297eea6cdf95daacfe16&scene=21#wechat_redirect)

[DAOrayaki解读｜8步实现去中心化](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484713&idx=1&sn=3b76441db3d940c4ea33fcc7e440e276&chksm=c1d804fcf6af8dea80f1e3bec50b06915e603a5927dac9e255ba3e61f4002c4df27191efb835&scene=21#wechat_redirect)





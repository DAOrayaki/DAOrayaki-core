


[Vocdoni](/tag/vocdoni/)

详解Vocdoni: 去中心化的投票系统
====================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



8 Jun 2021
• 47 min read






![详解Vocdoni: 去中心化的投票系统](/content/images/size/w2000/2021/06/----_20210608161043-1.png)



![](http://daorayaki.org/content/images/2021/06/home.jpg)DAOrayaki DAO研究奖金池：

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 4/7 

通过赏金总量：200 USDC

研究种类：Vocdoni, Aragon, Ethereum, Election, Decentralized Voting (Vochain), Ballot, InterPlanetary File System(IPFS), zero-knowledge Proof (zk-Snark), Tendermint, Gateways)

贡献者：Jones, 朱莉,  DAOctor @Daorayaki

![](http://daorayaki.org/content/images/2021/06/----_20210426113809-8.png)Vocdoni是一个用户友好、高度安全、以隐私为中心的治理平台。目前Aragon已经收购了Vocdoni协议背后的公司DvoteLabsOü，该公司旨在使用去中心化技术构建最安全，匿名的投票系统。Vocdoni提供基于普遍可验证，私有和可扩展投票的治理解决方案，该解决方案是为来自公共和私人市场的组织（包括市政当局，公共管理机构，公司和会员协会）量身定制的。Vocdoni的技术利用zkSnarks来启用完全匿名投票，IPFS和libp2p来实现反审查数据可用性和协议通信，以及第二层特定的投票目的区块链Vochain来透明地进行投票。Vocdoni的平台以前托管了有史以来最大的投票程序，完全在formnium Cultural的公共区块链上进行，,mniumCultural是欧洲最大的文化协会，拥有超过18万名人口普查。

I.背景

Devote Labs诞生于2017年加泰罗尼亚独立运动，Vocdoni项目官方人员主要由加泰罗尼亚人组成，他们曾亲身经历过压制民主投票。当时，加泰罗尼亚试图脱离西班牙被认为是非法的。在警察镇压，骚乱和高调逮捕之后，投票最终以平局告终。简而言之，Vocdoni将分散式基础架构（例如星际文件系统（IPFS））与最新的零知识证明（zk-SNKARKs）相结合，旨在将民主带入21世纪。该项目虽然不是crypt-first，但使用了Cosmos区块链也采用的Tendermint共识机制。后来，2021年12月 Aragon宣布收购其位于爱沙尼亚的实验室Dvote LabsOü的投票项目Vocdoni。

Vocdoni首席财务官JOANArús在接受CoinDesk的电话采访中表示，此次收购以私募价格完成，Vocdoni的团队成员在此次收购中收到了一笔私募ANT，这是收购的一部分，是Aragon网络的代币。

II.团队，附属机构与合作伙伴：

2021年1月11日，Aragon协会宣布收购Dvote LabsOÜ，该公司旨在使用Vocdoni等去中心化技术构建最安全，匿名的投票系统，其团队由9名开发人员以及支持人员组成。

**II.1.高管团队**

-Xavier Vives - 联合创始人，产品负责人：

在大多数情况下，Xavier的工作涉及确保Vocdoni的平稳运行。随着项目的发展，他的重点集中在Vocdoni平台的产品管理上，产品设计及创建可行的产品推出策略。在他的整个职业生涯中，他追求各种整合方法，使他可以胜任北美，亚洲和欧洲地区初创企业中产品开发的各个级别的工作。

-Pau Escrich – 联合创始人兼CTO：

Pau是Vocdoni的首席工程师，主要是mesh网络，分布式系统，安全性和区块链集成方面的专家。在此之前，他是qmp.cat，libremesh.org等各种项目的共同创立者，欧盟FP7研究项目CONFINE和Community的开发人员。

-Joan Arùs –COO和CFO：

Joan担任COO和CFO的主要职责是帮助Vocdoni从概念发展为可扩展的业务，确保获得实现此目标所需的资源并领导战略规划，具有扎实的科学和商业背景。在互联网和食品行业创立了几家公司。除此之外，他还是巴塞罗那数字商会的联合创始人，加泰罗尼亚中心区块链顾问。

**II.2.技术团队:**

-Jordi Moraleda – 开发人员：

Jordi是全栈开发人员，负责集成整个平台上的集成组件工作。他以新项目的基架开发，研究新框架，测试原型的可行性以及文件协议而出名。乔迪（Jordi）也是三家公司的联合创始人，作为一名加密货币开发者，他以单一竞争对手的身份赢得了有史以来的他的第一次黑客松比赛。

-Abel Boldy –开发人员：

Abel是一名DevOps工程师，在分布式基础架构，Linux，网络，安全性，监视以及与系统相关方面具有很强的专业知识。在DAppNode工作2年。

-Jordi Pinyana Paga – 开发人员：

Jordi Pinyana是区块链后端开发人员，在以太坊和Tendermint方面拥有丰富的经验。他主要致力于使用Golang开发Vochain（第一个用于投票处理和会计的区块链）。此外，他还是加泰罗尼亚理工大学的区块链教授。

-Emmanouil Dimogerontakis – 开发人员：

Emmanouil是一位分布式网络工程师。工作包括设计和实施中间层及后台系统。在专业领域，他分析了分布式网络，在博士期间主要研究底层mesh网络。在过去的几年中，Emmanouil专注于区块链技术与去中心化网络的应用。

-Òscar Casajuana – 开发人员：

高级全栈开发人员，主要专注于Vocdoni的前端客户端应用程序，例如管理器和区块链浏览器。在过去的十年中，他为多家公司创建了应用程序，并构建了多种类型的基础架构，并掌握了从上到下的所有有关Web开发的重要知识。

-Nathaniel Williams – 开发人员：

一个初级的全栈开发人员，专注于为Vocdoni的投票区块链以及Vocdoni移动应用程序构建区块链浏览器。他是Vocdoni的全职雇员，于2019年夏季作为实习生首次加入该团队。

**II.3.商务团队**

-Ferran Reyes – 商务主管：

Ferran管理Vocdoni的商务，重点是伙伴关系，社交媒体和促进基层的交流。在Vocdoni之外，他是西班牙最大的电信合作社SomConnexiò的董事会成员。

**III.Vocdoni 初衷**

Vocdoni核心协议是Aragon协议栈的一部分，其创新之处，是实施第一个去中心化，抗审查和匿名的在线投票协议。但是，除了这些技术抱负之外，该议定还支持与广泛的民主进程进行兼容。Vocdoni完成了通用的投票规范有关部分。III.1.投票流程

在Vocdoni的体系结构中，每个组织都会在数据库或公共分类帐中维护潜在选民的公钥列表。下面是使用Vocdoni进行投票的步骤：

1. 创建投票程序：

组织者整理了属于符合投票条件的选民的密钥清单，以进行选民普查（例如，年龄超过16岁的成员）。他们使用ZK-Snark友好的哈希函数（Poseidon）对它们进行哈希处理，并创建了Merkle tree。通过分布式文件系统（IPFS）分发数据结构，即选民普查，并将过程元数据（包括普查的Merkle根和用于投票加密的过程公钥）发布在以太坊区块链上。

2. 投票：

一旦过程开始，用户即可投票。为此，他们需要提供有效的“特许证明”以证明其资格。

3. 不具有匿名性：

每个用户将计算其Merkle证明，可以使用它来计算投票过程的Merkle根，从而验证它们是否是普查的一部分。

4. 具有匿名性：

为了满足唯一性和匿名性要求，每个用户都使用零知识证明（ZK-Snark）将选票附在信封中.ZK-Snark证明（特许证明）是一种易于验证的手段在不透露选民身份的情况下证明选民的资格。就是说，该方法允许用户说服第三方验证者参与普查，并且他们只能投一次，且不透露有关选民或投票本身的任何信息。

5. 选票验证：

一个基于Tendermint的自定义区块链负责验证投票信封和特许经营证明，以存储和计算有效选票。这被称为投票链（Vochain）。投票主要由三部分组成：-选举/进程ID。-加密或未加密的投票内容。-特许经营证明（Franchise Proof）

![](http://daorayaki.org/content/images/2021/06/640-8.png)**III.2.数据可用性：**

通常，数据可用性是由所谓的云提供的，实际上，这意味着由少数几家非常强大的公司收集我们的数据并进行集中化管理。Vocdoni的目标是成为一个自治生态系统，因此我们尝试对所有非敏感数据进行去中心化和分布式。

目前，Vodconi依靠“星际文件系统”（IPFS）来存储信息。在投票过程中，将引用文本（问题，描述和选项），补充图像和普查（可以由公共密钥或用户声明形成）。这些数据不必永久保存，并且保存起来很昂贵，因此可以将其上传到IPFS，直到作废为止。由于Vocdoni设计是模块化的，因此将来需要更多地集成数据层，例如Etherphere Swarm，DAT或STORj。

**III.3.数据同步**

IPFS可以完成这项工作，但是如果没有人在上传数据时将其“选中”，则只能从原始位置获得。为了确保数据的可用性和弹性，创建固定相同内容的IPFS节点群集。为此，创建者开始使用“ ipfs-cluster”，但是发现现有体系结构存在一些不兼容问题。因此，他们开发了一个名为“ ipfs-sync”的新组件。遵循KISS方法，“ IPFS同步”使创建IPFS群集的方式更加快捷，简便。创建自己的集群所需的唯一条件是共享密钥，它将用作对称密钥来加密，认证和查找其他集群节点。当前可以与libp2p / rendezvous，swarm / pss一起用p2p传递层实现传输消息。

每个ipfs-sync节点都会在确定性的Merkle树中聚合本地固定文件列表。根通过DHT网络向共享相同秘密的节点进行广播。找到新的根后，节点会向消息的发起者询问其 pins列表。因此，所有节点都将具有相同的文件列表和相同的Merkle树。除了数据同步外，节点还通过DHT宣布其Multiadress地址，因此其他集群节点可以通过IPFS连接。

**III.4.数据完整性和主要协作**

人们可能将这个组件称为“圣经”，但实际上是“以太坊”。以太坊是所有主要和重要信息的存储地。出于可扩展性的原因，创建者尝试尽可能少地使用它。目前，Vocdoni使用的是Goerli tesnet，但开发人员计划在Vocdoni整合后将基础架构转移至主网（Mainnet）。

Vocdoni部署了两个智能合约： 

1- Entity resolver智能合约，其中包含使用Vocdoni各实体的元数据。用于履行该合约的以太坊服务名称（ENS）为“ entity-resolver.vocdoni.eth”。

解析合约程序对实体元数据的信息，以及其他信息的源或URI进行索引。此外，“ entity-id”下记录的“ vnd.vocdoni.eth”将以JSON格式返回可找到描述实体的URI（通常为IPFS）。此外，还允许其他记录信息，例如“ vnd.vocdoni.boot-nodes”，该记录指示使用哪些指引节点访问其他组件。如果实体未指定，则将使用Vocdoni的默认启动节点。

2-流程管理智能合约，用于发布和管理选举流程。实体（以太坊地址标识）想要创建一个新流程。实体可以向该合约发送包含创建合约所需交易的基本信息，例如：

-选举类型（民意测验，snarks等）。

-开始和结束区组数。-带有选举数据信息的URI元数据（存储在IPFS上的JSON文件）。

-选民普查哈希根和URI。该合约受一个或多个Oracle监视，Oracle是以太坊和Vochain组件的桥梁。

**III.5.身份**

除非密钥确实属于目标用户，否则无法保证投票的准确性。在我们的身份识别模型中，用户在其设备上生成密钥。因此，当涉及识别时，应选择自治权身份。用户通过辅助渠道向社区证明他们有投票权以及密钥的所有权。Vocdoni的设计与选民的验证方式无关，社区可以按要求选择。在当前阶段，Vodconi使用著名的简单ECDSA公钥/私钥对。目前，暂时通过公共密钥来识别用户或实体。

**III.6.普查**实体有责任更新公共用户密钥列表。为此，Vodconi提供了一项普查服务，该服务使“ REST API后端”可以方便地管理普查。API的主要思想是允许实体拥有和管理其私人基础设施。通常，数据库存储真实的用户数据，例如姓名，电子邮件地址和电话号码。但是Vocdoni还提供了一个非常简单的基于Web的统一解决方案，任何实体都可以免费使用。在Vocdoni设计中，人口普查是由合格选民的ECDSA公钥列表，基于“ iden3实施”，使用Poseidon哈希（对ZK-Snarks友好）在Merkle树上汇总而成。

![](http://daorayaki.org/content/images/2021/06/640--1--4.png)为什么要使用Merkle树作为普查数据结构？

1-整个数据结构可以总结为一个散列

2-用户可以提供Merkle证明来证明符合普查身份的工作。例如，在上面的示例中，左侧Pubkey的所有者只需要发送其Pubkey + Hash4 + Hash2（命名为兄弟）即可允许第三方重构哈希根。证明者不需要访问整个数据结构，只需访问根（32字节）即可。

**III.7.投票**

Vocdoni的目标是扩展和支持各种规模的投票程序，甚至在未来举行数百万合格选民的大选。为此，Vocdoni的创建者实现了自己的名为Vochain的投票区块链项目。该设计意味着范式转移。Vocdoni系统无需依赖集中式计数系统，且任何人都可以审核投票过程，同时创建可视化工具。Vocdoni为此发布名为“检查程序（scrutinizer）”的基本系统，任何人都可以运行该系统来验证结果的正确性。

Vochain没有代币，也没有虚拟机。它唯一的目的是利用一种非常有效的方式来验证和计数选票。基于“ Tendermint”，因此是加权的权威证明。节点（矿工或验证者）允许在Vochain上创建新区块通过以太坊智能合约来管理和协调。Vocdoni合并后，下一步就是启用混合的权威性证明/权益证明，以分散者的权限，实现去中心化验证。

oracle是能够创建一组特殊交易的特殊Vochain身份，充当以太坊和Vochain之间的桥梁。因此，一旦在以太坊中创建新的投票流程，oracles 就会向“ Vochain”发送一个“ addProcess”交易。尽管oracles是受信任的组件，任何人都可以验证他们没有操纵或采用任何形式的审查制度。

当前，Vochain允许进行以下交易：

-addProcess：创建新的选举（仅适用于oracle）。

-cancelProcess：取消当前的选举（仅适用于Oracle）。

-addVote：为现有的进程ID（投票）发送新的投票。

-addOracle：添加由公钥标识的新oracle（仅适用于矿工）。

-removeOracle：删除现有的oracle（仅限矿工）。

-addValidator：添加由公钥标识的新矿工（仅矿工）。

-removeValidator：删除现有的矿工（仅限矿工）。

-addProcessKey：添加用于加密投票有效负载的加密公共密钥（仅限矿工）。

-revelProcessKey：添加用于解密投票有效负载的加密私钥（仅限矿工）。

![](http://daorayaki.org/content/images/2021/06/640--2--3.png)区块链的状态由三个嵌套的在单个根哈希中（称为状态哈希）的Merkle树代表。所有知名矿工必须在本地计算相同的哈希值。这种机制确保所有区块链字节都是正确的并且具有有效共识。例如，如果矿工在区块123开始新的投票，则新的根哈希将在p2p网络上进行广播。然后，区块链的所有节点将验证相同的投票，包括检查计算出的状态是否匹配（如果不匹配，它们将分叉）。

当前实施和允许的投票类型为：

-民意调查：

对于非匿名投票，选民必须提供有效的Merkle证明以证明其资格。

-Snarks：

对于匿名投票，投票者必须提供有效的ZK-Snark证明（处于POC状态）。

Vocdoni如何实现去中心化的？

Vocdoni的大多数组件都基于去中心化技术：IPFS，以太坊，Tendermint等。但是，所有这些技术在CPU /内存和网络上都非常消耗资源。因此，在智能手机或Web环境中运行它们并不现实。要解决该问题，需要创建一个名为Gateway的新组件。

网关为P2P网络提供了一个入口。它们允许客户端通过WebSocket HTTP（s）API接口访问权力分散服务。网关密码存储在go-dvote repository中。当前，可以根据网关业主的意愿启用/禁用五个可用的API，它们是：

-File api：

提供对IPFS或其他支持的文件系统的访问。

-Census api：提供普查的访问权限，例如创建和发布新的普查或为符合条件的选民生成Merkle证明。

-Vote api：提供Vochain的访问，例如进行新的投票。

-Results api：如果启用，Vochain审查程序将计算选举结果汇总给客户端。

-Web3 API：为以太坊区块链提供访问权限。

![](http://daorayaki.org/content/images/2021/06/640--3--2.png)Gateways 为愿意为Vocdoni生态系统做出贡献的人添加网关，但也可以由不信任其他网关并希望完全自控交流的用户添加网关。目前，Vodconi团队正在研究网关激励机制，以确保网关网络具有良好运行状况。新的网关启动后，它将通过P2P / DHT网络（当前为libp2p）公开。Bootnodes将检查网关是否正常工作，并将正常的网关添加到列表中。当APP客户端需要访问网关时，它将与Bootnodes联系以获取此列表并选择一个（或多个）网关。另一方面，Bootnode基于 entity-resolver 智能合约进行管理。

![](http://daorayaki.org/content/images/2021/06/640--4--2.png)网关可能会受到攻击，但任何人都可以设置新网关，因此，网络可以像现有的区块链一样横向扩展。计划与DappNode整合使网关可以一键部署，最后，在持续的DDOS攻击中，可以私下和静默添加网关。因此，组织或社区可以共享自己的私有网关基础架构，以确保他们可以访问Vocdoni平台。

**如何在Vocdoni中实现匿名？**

匿名投票是通过零知识技术Zk-Snarks来实现的。Zk-Snark证明是一种向第三方验证者证明选民处于普查范围内并且在不透露其身份的情况下进行不超过两次投票的简单方法。每个Zk-Snark用例都需要其自己的流程，由证明者和验证者共享。流程主要由密码运算符组成，并以严格和确定的方式确定输入值是否有效。Vocdoni团队使用非标准叉（non-standard fork）（进行了一些细微的修改）来设计和实现他们的流程。Circm是由“ iden3”开发和维护的项目。

![](http://daorayaki.org/content/images/2021/06/640--5--2.png)专用输入端是生成ZK-Snark证明时专用的输入端。它们主要是Merkle证明（表明用户是普查的一部分）和私钥（用户的身份）组成。一旦用户为特定的普查根和ElectionID生成了有效的证明，便需要将Nullifier与Vote软件包一起公开。该无效符是独特的数字，它将标识投票（但不能标识其所有权），因此，如果相同身份投票两次，将被显示。另一方面，需要公共输入端来验证Zk-Snark证明，因此任何证明者都能访问这些输入端。

-普查默克尔根。

-投票包（可能被加密）。

-选举ID（ElectionID）。

-取消者（Nullifier）。

-提交密钥。

提交和显示密钥启用减少购买投票的机制。所有公开密钥公开后，任何人都可以为特定选举生成有效的Zk-Snark证明。因此，一旦选举结束，用户就无法公示自己支持特定选项的选票。除此之外，一旦新的选举开始，Vochain的矿工将自动生成提交密钥，而公开密钥将在完成后立即发布。这是匿名投票架构的弱点之一，但出现的前提是所有矿工都同意篡改选举结果。

关于透明度，可以强制执行吗？

透明度是确保普选可靠性的关键。如果任何人都可以在系统内验证正确性，则该过程是端到端可验证性。Vocdoni团队使用区块链技术实现了端到端验证，因为当投票过程完成时，任何人都可以下载并验证相应的Vochain，从而评估发布的结果正确性。

尽管Vocdoni力求最大程度地提高其组件的透明度，使整体上去信任化，但并不可能完全透明。从本质上需要一些信任，例如实体的私有普查。但是，即使实体尝试操纵普查，也有一些属性可以缓解这些问题：

-任何人都可以检查选举结果，所有选民信息（目前通常很容易混淆）都存储在公共场所并开放Vochain区块链。区块链中不会更新任何个人或敏感数据。

-任何人都可以检查普查的规模，因此，如果实体试图添加相关数量的虚假身份来操纵选举，则观察员都可能会找出（即，如果市议会有1000名居民，则1200个身份的普查将显示示警红旗）。

-如果实体在普查中替换了身份，则替换的用户将注意到该身份（不发送投票），因此，如果在一定数量的用户中发生此情况，则很可能会发现这种操作。

III.8.Vocdoni

投票协议Vocdoni投票协议旨在成为一个非常简单而有力的说明，用于表现投票和投票过程的结果，后者由一个或多个字段组成，每个字段代表一个问题或一个选项，具体取决于流程类型。投票时，符合条件的选民将从每个字段的选项中进行选择。允许的答案数量、答案类型还取决于特定的流程类型。合格的选民通过投票来表达自己的选择。

![](http://daorayaki.org/content/images/2021/06/640--6--2.png)选票显示为自然数的数组（或列表）。数组的每个位置都应对流程字段答案。之后，将结果累积在二维自然数数组（矩阵）中，此矩阵的每个箭头对应一个选票字段，每列对应于该字段的一个可能值。结果矩阵中的任何数字都只是该索引所表示值的票数。

为了深入研究如何配置流程，下面给出了一个通用示例。假设我们有一个包含三个字段A，B和C的过程，每个字段都启用0、1和2作为可能的值。我们不知道这些值或字段代表什么，这暂时不重要。

在此示例中，已投了两票。第一个投票者为A字段选择了值2，B字段选择了0，C字段选择了1.第二个投票的值分别为0、0和2.可以在上图中看到投票与结果矩阵的关系。选票值的索引确定该值所属的字段-即选票1的第一个索引的值为2，因此选票1将值2分配给字段A.在结果矩阵的每个字段中，该值投票数由其索引表示。我们在字段A的索引2处放置1以代表对值2的一票表决。

III.9.协议本身：

![](http://daorayaki.org/content/images/2021/06/640--1-.jpg)投票协议由数字和布尔（真/假）变量组成，这些变量限制有效投票的格式。

1.如何用协议表示所提出的示例？

首先，我们知道有三个字段，因此：

3.maxCout = 3。

我们用0、1和2作为有效值，因此我们可以设置：

4.minValue = 0。

5.maxValue = 2。

第二张选票包含多个字段的值0。因此，为了使这次投票有效，我们必须设置：

6.uniqueValues = 0（此处的0表示“ false”，而1表示“ true”）。

接下来的三个变量没有一组具有明显赋值，因此让我们在示例过程中添加更多内容。例如，说这个过程只是单一问题，要求选民将代币委派给不同的组织。每个字段代表一个组织，分配给该字段的值是选民要分配给该组织的代币数量。

我们已经根据minValue和maxValue变量进行设置； 我们知道每个用户可以向任何一个组织分配0到2个代币。但是我们添加一条合理的规则，使选民总共只能分配3个代币。我们还可以假设选民必须分配至少1个代币。这使上图的流程图更有意义； 第一次投票总共分配了3个代币（也许他们支持组织A和C，但他们更喜欢A）。第二次投票仅分配其3个可能的代币中的2个（它们仅支持组织C，宁愿浪费他们的第三个代币而不是将其分配给A或B）。因此，为了使两个选票均有效，我们可以设置：

7.minTotalCost = 1。

8.maxTotalCost = 3。

我们需要设置的最后一个变量是cost Exponent，它与二次方投票有关。我们暂时不会进行这种类型的投票，所以我们设置默认值：

9.costExponent = 1。

同样，花点时间思考一下这些变量，看看是否能理解更改其中任一变量会如何影响示例投票过程。

III.10.结果解析

上面的变量代表了Vocdoni投票协议的整体，其中涵盖了处理核心基础架构的选票验证和结果列表。但显然，在试验中仍然缺少很多信息。协议的集成商需要决定如何将过程中发生的事情传达给投票者，以及如何解析和表示结果矩阵。结果解析不在选票协议的范围内，但与了解如何使用该协议有关。在当前迭代版本中中，Vodconi定义了两种结果解析格式：“索引加权（Index-weighted）”和“离散值（Discrete values）”。

1.索引加权

在示例过程中，我们将使用索引加权结果解释公式。该模式适用于单一问题过程，例如排名选择，

多选或参与预算。结果矩阵字段中的每个索引代表一个加权值，在这种情况下，权重代表分配给组织的代币数量。投票总和乘以其指数加权值即为该字段的总价值。

![](http://daorayaki.org/content/images/2021/06/640--7--2.png)我们的示例过程汇总了解释。机构A收到2个代币，机构C收到3个代币。

2.离散值离

散值解释用于每个字段有其自身问题的流程。在这里，每个值代表一个单独的离散选项（即“候选2”），而不是乘数（即“ 2指向该选项”）。这样，该方法通过简单汇报每个字段获得最多投票的值（如果有）来解释结果。

0用于选项之间的联系。

这两种格式并非穷尽的。如上所述，投票协议本身与结果的汇总方式无关，任何在协议上构建自己的应用层的人都可以定义自己的结果解释。

![](http://daorayaki.org/content/images/2021/06/640-1.jpg)IV.联系方式：  
Official Website: https://aragon.org/vocdoni

Blog: https://blog.aragon.org/vocdoni/

Twitter: https://twitter.com/vocdoniDiscord: discord.gg/x7GYRB8dpp

Telegram: https://t.me/vocdoni

Github: https://github.com/vocdoni?page=1

**Vocdoni: A decentralized self-sovereign governance system**

DAOrayaki DAO Research Grant：

Fund Address: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

Voting Result：DAO Committee /7 Yes

Grant Amount：200 USDC

Category: (Vocdoni, Aragon, Ethereum, Election, Decentralized Voting (Vochain), Ballot, InterPlanetary File System(IPFS), zero-knowledge Proof (zk-Snark), Tendermint, Gateways)

Contributor：Jones @Daorayaki，Julie @Daorayaki

Launch date: According to the aragon project which is currently the official owner of Vocdoni, the release date presumed to be on May,2021.

**Brief Overview about Vocdoni**

Vocdoni is a universally verifiable, censorship-resistant and anonymous governance system, designed to be scalable and easy to use on modest devices. The goal is to provide the foundation to run national elections, general shareholders meetings, assemblies, etc. It mainly concentrates on providing a trust-less voting system, where people can speak their voice and everything can be audited.

**I.Background**

Born out of the 2017 Catalan independence movement, Devote Labs’ the official staff of Vocdoni project mostly consists of Catalans who experienced the suppression of a democratic vote firsthand. At the time, Catalonia tried to secede from Spain, which was deemed illegal. The vote ultimately fell flat after police suppression, riots and high-profile arrests.

Simply put, Vocdoni combines decentralized infrastructure such as the InterPlanetary File System (IPFS) with bleeding-edge zero-knowledge proofs (zk-SNKARKs) in an effort to bring democracy into the 21st century. The project, while not crypt-first, uses the Tendermint consensus mechanism also employed by the Cosmos blockchain. Later on, in December, 2020, Aragon Association, the stewards of a protocol that makes for the easy creation of decentralized autonomous organizations (DAOs) has announced its acquisition of voting project Vocdoni from Estonia-based Dvote Labs Oü. The purchase was completed for an undisclosed price, where Vocdoni team members received an undisclosed amount of ANT, the native token of the Aragon network, as part of the acquisition, according to Vocdoni CFO JOAN Arús in a phone interview with CoinDesk.

**II.Team, Affiliates & Partners:**

On December, 2020, The Aragon Association announced its acquisition of Dvote Labs O[Ü](https://vocdoni.io/), which aims to build the most secure and anonymous voting system using decentralized technologies such as Vocdoni, their team comprises nine developers, in addition to supporting personnel.

**II.1.****Executive Team:**

-       **Xavier Vives - Co-founder, Product Lead:** For the most part, Xavier work involves making sure that the gears of Vocdoni are woking smoothly. As the project has grown. His focus centered on the role of product lead for the Vocdoni Platform designing it and creating an achievable go-to-market strategy. Throughout his career, he sought various holistic approaches, making him working at all levels of product development in startups across North America, Asia, and Europe.

-       **Pau Escrich – Co-Founder & CTO:** Pau is the Lead Engineer of Vocdoni, mainly expert on mesh networking, distributed systems, security and blockchain integrations. Previously, he co-founded and worked for several years on various projects such as qmp.cat, libremesh.org, and was one the architects and developers behind the EU FP7 research projects CONFINE and Community.

-       **Joan Arùs – COO & CFO:** Joan main role as a COO and CFO is to help Vocdoni grow from a concept and idea into a scalable business, securing the resources to achieve that and leading the strategic planning, with a solid background in science and business, he founded several companies in the internet and food industries. Besides that, he is also the co-founder of the Digital Chamber of Commerce of Barcelona and advisor to the Center Blockchain Catalunya.

**II.2.****Tech Team:**

-       **Jordi Moraleda – Developer:** Jordi is a full stack developer, used to integrating components all across the platform. He is known for his scaffolding for new projects, research new frameworks, test the viability of prototypes and document the protocol. Jordi also co-founded three companies, and as a crypto developer he stated off by winning his first ever hackathon as a single competitor.

-       **Abel Boldy – Developer:** Abel is a DevOps engineer, with expertise in decentralized infrastructure, Linux, networking, security, monitoring, and all things related to systems. He worked with DAppNode for 2 years.

-       **Jordi Pinyana Paga – Developer:** Jordi Pinyana is a blockchain backend developer with a lot of experience in Ethereum and Tendermint. He mainly focuses in the development of Vochain (the first blockchain for ballot processing and accounting) using Golang. Also, he is a blockchain professor at the Polytechnic Unviersity of Catalonia.

-       **Emmanouil Dimogerontakis – Developer:** Emmanouil is a decentralized networks engineer. His role consists of designing and implementing middleware and backend systems. As an area of expertise, he analyzes decentralized netowrks, which mainly was focus on grassroots mesh network during his phd. Over the last couple of years, Emmanouil focuses on the application of blockchain technologies together with decentralized networks.

-       **Òscar Casajuana – Developer:** A senior full-stack developer who mainly focused on Vocdoni’s frontend client apps, like the manager and the blockchain explorer. He has created apps and built infrastructures of many kinds over the last 10 years for multiple companies, armed with all the important insights about web-development from top to bottom.

-       **Nathaniel Williams – Developer:** A junior full-stack developer, focusing on building a Block Explorer for Vocdoni’s voting Blockchain as well as the Vocdoni mobile application. He is Vocdoni’s latest full-time hire and a recent university graduate who joined the team first as an intern in the summer of 2019.

**II.3.****Communication Team:**

-       **Ferran Reyes – Communication Lead:** Ferran manages communications for Vocdoni, with an emphasis on partnerships, social media communication, and promotin grassroots movements. Outside of Vocdoni, he is a board member of Som Connexiò, the largest telecommunications cooperative in Spain.

**III.The ideas behind Vocdoni:**

The core innovation of the Vocdoni core protocol, part of the Aragon stack, is in implementing the first ever decentralized, censorship-resistant, and anonymous online voting protocol. But on top of these technical aspirations, the Protocol enables compatibility with a wide range of democratic processes. Vocdoni achieves this partly with our versatile specification for vote ballots.

**III.1.****Voting Process:**

In Vocdoni’s architecture, each organisation maintains a list of public keys from their potential voters, either in a database or in a public ledger. Down below are the steps in which a voting process using Vocdoni is divided:

1.    Creation of the Voting process: The organiser collates a list of those keys belonging to eligible voters to create a census (for example, members over 16 years old). They hash them using a ZK-Snark friendly hash function (Poseidon) and create a [Merkle tree](https://en.wikipedia.org/wiki/Merkle_tree). This data structure, so-called Census, is distributed through a decentralized file-system (IPFS) and the process metadata (including the Merkle root of the census and a process public key for vote encryption) is published on the Ethereum blockchain.

2.    Casting of votes: Once the process has begun, users can vote. To this aim they will need to provide a valid ‘franchise proof’ in order to demonstrate their eligibility.

1.    **Without anonymity:** Each user will compute its Merkle proof which can be used by the prover to compute the Merkle root of the voting process and thus verify they are part of the census.‌‌

2.    **With anonymity:** To satisfy uniqueness and anonymity requirements, each user wraps her ballot in an envelope using a zero-knowledge proof (ZK-Snark).‌‌The ZK-Snark proof (franchise proof) is an easy-to-verify method for proving the eligibility of a voter without revealing their identity. That is to say, the method allows a user to convince a third party verifier that it is part of the census and they have not voted twice, without revealing any information about the voter or the vote itself.

3.    Validation of votes: A custom Tendermint based blockchain is responsible for validating the voting envelope and the franchise proof, to store and account valid ballots. This is referred to as the Voting Chain (Vochain). A ballot is mainly composed of three parts:

-       Election/process ID.

-       Encrypted or unencrypted vote content.

-       Franchise Proff.

![](http://daorayaki.org/content/images/2021/06/--1-8.png)**III.2.****Data availability:**

Usually data availability is provided by the so-called cloud, which in reality means a centralization of our digital information, gathered by a small set of very powerful companies. Vocdoni aims to be a self-sovereign ecosystem, so we try to enforce the decentralization and distribution of all the non-sensitive data.

![](http://daorayaki.org/content/images/2021/06/--2-3.png)Currently, Vocdoni relies on the ‘InterPlanetary File System’ (IPFS) for storing information. In a voting process a reference to the text (question, description and options), complementary images, and the census (that can be formed by public keys or user claims). This data doesn’t have to be permanent and its expensive to keep it around, so it’s uploaded to IPFS until it can be discarded, and since Vocdoni design is modular, more incorporation for data layers in the future such as Etherphere Swarm, DAT or STORj is required.

**III.3.****Data Synchronization:**

IPFS does the job, but if no one “pins” it when data is uploaded, it will only be available from the origin. To ensure the availability and resilience of the data, a cluster of IPFS nodes pinning the same content should be created. For that, creators start using “ipfs-cluster”, but some incompatibilities were found with our architecture. For that reason, they developed a new component named “ipfs-sync”. Following a KISS approach, “IPFS-sync” enables the creation of IPFS clusters in a very quick and easy way. The only required input to create your own cluster is a shared secret, which will be used as a symmetric key to encrypt, authenticate and find other cluster nodes. The current implementation can work either with libp2p/rendezvous and swarm/pss for the p2p transport messaging layer.

Every ipfs-sync node aggregates the list of locally pinned files in a deterministic Merkle tree. The root is broadcaster via the DHT network to those nodes which share the same secret. When a new root is found, the node asks the originator of the message for its list of pins. Thus, all nodes will end up with the same list of files and with the same Merkle tree. In addition to the data synchronisation, the nodes also announce their Multiadress via the DHT, so other cluster nodes can directly connect via IPFS.

**III.4.****Data integrity and main coordination:**

One might call this component “the Bible” but its name is actually “Ethereum”. Ethereum is where all main and most important information is stored, though the creators try to use it as little as possible for scalability reasons. At the moment, Vocdoni is using the Goerli tesnet, but developers plan to move the infrastructure to Mainnet once Vocdoni consolidates.

![](http://daorayaki.org/content/images/2021/06/--3-3.png)Vocdoni has deployed two **smart contracts:**

**1-****Entity resolver smart contract,** which contains the meta data of the Entities using Vocdoni. The Ethereum Name Service (ENS) used to address this contract is “entity-resolver.vocdoni.eth”.

The resolver contract indexes the origin or URI of the entity metadata, among other information. Furthermore, the record “vnd.vocdoni.eth” under the key “entity-id” will return the URI (usually IPFS) where the entity description can be found, in JSON format. In addition, some other records are allowed, such as “vnd.vocdoni.boot-nodes” that indicated which boot nodes should be used to reach the rest of the components. If none are specified by the entity, Vocdoni’s default boot nodes will be used.

**2-****Process management smart contract,** used by the entities to publish and manage election process. One an entity (identified by an Ethereum address) wants to create a new process, the entity can send a transaction to this contract containing the basic information required to create it, such as:

-       **Election type (poll, snarks, etc).**

-       **Start and end block number.**

-       **URI metadata with the election data information (a JSON file stored on IPFS).**

-       **Census Root hash and URI.**

This contract is monitored by one or many **Oracles,** the component which makes the bridge between Ethereum and the Vochain.

**III.5.****Identity:**

Voting correctness cannot be guaranteed unless keys really belong to the targeted user. In our identity model the user generates the keys on their device. For this reason, when it comes to identity, **self-sovereign identity** is chosen. Through side channels, the users prove to the organization their eligibility for voting and the ownership of the generated keys. Vocdoni’s design is agnostic to how voters are validated, and organizations can choose their own requirements. At the current stage of, Vocdoni uses the well-known plain ECDSA public/private key pairs. As a result, for the time being a user or an entity is globally identified by a public key.

**III.6.****Census:**

The entity has the responsibility of keeping a list of public user keys up-to-date. To this end, Vocdoni provides a **Census service,** which enables a “REST API backend” to manage the census in a convient manner. The main idea behind the API is allowing the entities to own and manage their private infrastructure. Usually, a database would be storing the real user data such as names, email addresses, and phone numbers. But Vocdoni also provides a very simple, unified web-based solution that can be freely used by any entity. In Vocdoni design, the census is a list of ECDSA public keys from eligible voters, aggregated on a Merkle tree using Poseidon hashes (which are ZK-Snarks friendly) based on the “iden3 implementation”.

![](http://daorayaki.org/content/images/2021/06/--4-3.png)**1.****Why using a Merkle Tree as a census date structure?**

1-   The whole data structure can be summarized as a single hash.

2-   A user can provide a Merkle proof to demonstrate that its identity is part of the census. For instance, in the example above, the owner of the left-side Pubkey only needs to send its Pubkey + Hash4 + Hash2 (named siblings) to allow a third party to reconstruct the root hash. The prover does not need to have access to the whole data structure, just to the root (32 bytes).

**III.7.****Voting:**

Vocdoni aims to scale and support all sized of voting processes and, in the future even national elections with millions of eligible voters. To this end Vocdoni creators implemented their own voting blockchain named **Vochain.** The design implies a paradigm shift. Instead of relying on centralized counting systems, Vocdoni system allows anyone to audit any voting process and at the same time, visualisation tools could be created. Vocdoni has a basic system for this purpose named **“scrutinizer”** that anyone can run to verify the correctness of the results.

There are no tokens nor virtual machines on the **Vochain**; its only purpose is to validate and count votes in a very efficient way. It’s based on “Tendermint”, so currently it’s a weighted Proof-of-Authority. The nodes (miners or validators) allowed to create new blocks on the Vochain are managed and coordinated in an Ethereum smart contract. Once Vocdoni consolidates the next step is to enable a mixed Proof-of-Authority/Proof-of-Stake in order to decentralize the validators.

The oracles are special Vochain identities able to create a set of special transactions. They act as bridge between Ethereum and the Vochain. So for instance, once a new voting process is created in Ethereum the oracles will send an “addProcess” transaction to the Vochain. Although the oracles are trusted components, anyone can verify they are not manipulated or applying any kind of censorship.

![](http://daorayaki.org/content/images/2021/06/--5-3.png)Currently, the Vochain allows the following transactions:

-       **addProcess:** Creates a new election process (oracle only).

-       **cancelProcess:** Cancels a current election process (oracle only).

-       **addVote:** sends a new vote for an existing process id (votes).

-       **addOracle:** adds a new oracle identified by a pubKey (miners only).

-       **removeOracle:** removes an existing oracle (miners only).

-       **addValidator:** adds a new miner identified by a pubKey (miners only).

-       **removeValidator:** removes an exsiting miner (miners only).

-       **addProcessKey:** adds an encryption public key for encrypting the votes payload (miners only).

-       **revelProcessKey:** adds an encryption private key for decrypting the votes payload (miners only).

The state of the blockchain represented by three nested Merkle trees summarised in a single root hash (named State hash). All noted and miners must calculate the same hash locally. This mechanism ensures that all blockchain bytes are correct and the consensus works. For example, if a new vote is included on block 123 by the miners, the new root hash will be broadcasted on the p2p network. Then, all nodes of the blockchain will validate the same vote, include it, and check that the calculated state matches (if not they will fork).

![](http://daorayaki.org/content/images/2021/06/--6-2.png)The vote types currently implemented and allowed are:

-       **poll:** for non-anonymous voting, the voter must provide a valid Merkle proof to demonstrate its eligibility.

-       **Snarks:** for anonymous voting, the voter must provide a valid ZK-Snark proof (in POC state).

**1.****How decentralization is achieved in Vocdoni?**

Most of Vocdoni’s components are based on decentralized technologies: IPFS, Ethereum, Tendermint, etc. However, all these technologies are very resource-demanding on CPU/Memory and Network. Consequently, running them on a smartphone or in a web environment is not very realistic. To fix this problem a new component named **Gateway** is created.

**Gateways** provide an entry point to the P2P networks. They allow clients to reach decentralized services through a WebSocket HTTP(s) API interface. The Gateway code can on the [go-dvote repository](https://gitlab.com/vocdoni/go-dvote). Currently, there are five available APIs that can be enabled/disabled at the Gateway owner’s will, they are:

-       **File api:** provides access to IPFS or any other supported filesystem.

-       **Census api:** provides access to the census methods, such as create and publish a new census or generate Merkle proof for an eligible voter.

-       **Vote api:** provides access to the Vochain, for instance to cast a new vote.

-       **Results api:** if enabled, the Vochain scrutinizer will computer the election results and summarize it for the clients.

-       **Web3 api:** provides acess to the Ethreum blockchain.

![](http://daorayaki.org/content/images/2021/06/--7-3.png)The Gateways could be added by anyone willing to contribute to the Vocdoni ecosystem but it can also be added by a user who does not trust other Gateways and want to have complete control over its communications. Currently, Vocdoni team is working on a Gateway incentivization mechanism to ensure a good health of the Gateways network. One a new Gateway is started it becomes public via a P2P/DHT network (currently libp2p). Bootnodes will check that the Gateway is actually working and will add it to a list. When an APP client needs to reach a Gateway, it will contact the Bootnodes to get this list and choose one (or several). From the other hand, Bootnodes are managed on the entity-resolver smart contract.

![](http://daorayaki.org/content/images/2021/06/--8-1.png)Gateways can be attacked, but anyone can set up new ones, so the network scales horizontally, just as any existing blockchain. The integration with DappNode is planned to make Gateways one-click deployable, and as a last resort, on a continued DDOS attack, a Gateway can be added privately and silently. So, groups or communities can share their own private Gateway infrastructure to ensure they can access the Vocdoni platform.

**2.****How user anonymity is ensured in Vocdoni?**

Voting anonymity is achieved by the usage of the Zero-knoledge technology **Zk-Snarks.** Zk-Snark proofs are a convient methods to prove to third-party verifiers that a voter is within a census and has not voted twice without revealing its identity.

Each Zk-Snark use case requires its own circuit which is shared among provers and verifiers. A circuit is composed mainly by cryptographic operators and indicates, in a strict and deterministic way, if a set of input values is valid or not. Vocdoni team uses a non-standard fork of circom (with some minor modification) to design and implement their circuit. Circm is a project developed and maintained by “iden3”.

![](http://daorayaki.org/content/images/2021/06/--9-2.png)Private inputs are those required exclusively when generating a ZK-Snark proof. They are mainly the Merkle proof (that demonstrates a user is part of a census) and the private key (identity of a user). Once the user generates a valid proof for a specific Census Root and ElectionID, it needs to make the Nullifier public together with the Vote package. That nullifier is a unique number that will identify the vote (but not its ownership) thus it will make visible if the same identity is voting twice. On the other side, public inputs are required for validating the Zk-Snark proof, so any prover must have access to these inputs.

-       Census Merkle Root.

-       Vote package (might be encrypted).

-       ElectionID.

-       Nullifier.

-       Commit Key.

The Commit and Reveal Keys enable a mechanism to mitigate the vote purchase. Once all reveal keys are public anyone can generate a valid Zk-Snark proof for that specific election. So, it makes it impossible for a user to demonstrate he voted for a specific option once the election is over. In addition to that, the commit keys will be generated automatically by the Vochain’s miners once a new election starts and the reveal keys will be published once it finishes. This is one of the weak points of the anonymous voting architecture, but only if all miners agree on tampering with the election results.

**3.****What about transparency is it possible to enforce it?**

Transparency is a key point in order to enable universal election reliability. A process is end-to-end verifiable if anyone can validate the correctness within the system by its own. The way Vocdoni team uses blockchain technology enables the end-to-end verification as, when the voting process are finished, anyone can download and validate the corresponding Vochain, thus, evaluate if the published results are correct or not.

Although Vocdoni aims to maximise transparency in all its components in order to become trust-less as whole, complete transparency is not always totally possible. There are still some private components which, by nature require some trust such as the private census of an entity. However, even if the entity tries to manipulate the census, there are some properties that will mitigate these issues:

-       Anyone can scrutinise the results of an election, all the voters information (currently often conveniently obfuscated) are stored in the public and open Vochain blockhain. No personal or sensitive data is updated in the blockhain.

-       Anyone can check the size of a census, so if the entity tries to add a relevant amount of fake identities to manipulate an election it might be caught by any observer (i.e if a city council has 1000 inhabitants, a census of 1200 identities would show a red flag).

-       If an entity replaces an identity on the census, the replaced user will notice it (the vote annot be sent), so if this happens for a relevant amount of users, the manipulation will be probably discovered.

**III.8.****Vocdoni Ballot Protocol:**

The **Vocdoni Ballot Protocol** aims to be a very simple yet powerful specification for the representation of ballots and results for a voting process, this latter is made out of one or more **fields**, each of which represents a single question or an option for a question, depending on the **type of process.** When voting, eligible voters choose from a set of predefined **answers** for each field. The allowed number of answers, type of answer also depends on the specific type of process. An eligible voter expresses their choices by casting a **ballot.**

A **ballot** is represented as an array (or list) of natural numbers. Each position of the array contains an answer to one of the process’ fields. After that, the results are accumulated in a two-dimension array of natural numbers (a matrix), each arrow of this matrix corresponds to a ballot field, and each column corresponds to one of the possible values for that fields. Any number in the results matrix is simply a count of the votes for the value represented at that index.

In order under to go through the weeds of how a process might be configured, a generic example is represented below. Say we have a process with three fields, A, B, and C, each of which enables 0, 1, and 2 as possible values. We don’t know what these values or fields represent, but that doesn’t matter for now.

![](http://daorayaki.org/content/images/2021/06/--10.png)In this example, two votes have been cast. The first voter chose the value 2 for field A, 0 for field B, and 1 for field C. The second ballot has the values 0, 0, and 2. You can see in the diagram above how the ballots relate to the results matrix. The index of a value of a ballot determines the field that value belongs to- i.e. the first index of ballot 1 has the value 2, so ballot 1 is assigning the value 2 to field A. Within each field of the results matrix, the value of the vote is represented by its index. We place a 1 at index 2 of field A to represent the one vote for the value 2.

**III.9.****The Protocol Itself:**

The **ballot protocol** is composed of a set of numeric and Boolean (true/false) variables that restrict the format of a valid ballot.

![](http://daorayaki.org/content/images/2021/06/--11.png)**1.****How might the presented example be represented with this protocol?**

To start, we know we have three fields, so:

3.    maxCout = 3.

We have 0, 1 and 2 as our valid values, so we can set:

4.    minValue = 0.

5.    maxValue = 2.

The second ballot contains the value 0 for multiple fields. So, in order for this ballot to be valid, we must set:

6.    uniqueValues = 0 (0 here represents ‘false’ and 1 represent ‘true’).

There’s no one obvious set of assignments for the next three variables, so let’s add a little more context to our example process. For example, say this process is a single question asking voters to delegate gold coins to different organizations. Each field represents a single organization, and the value assigned to that field is the number of gold coins that voter wants to allocate to that organization.

Based on the minValue and maxValue variables we’ve already set; we know that each user can allocate between 0 and 2 coins to any one organization. But a plausible rule we could add is that voters can only allocate 3 coins in total. And let’s also imagine voters have to allocate at least 1 coin. This adds meaning to the process diagram above; the first ballot allocates 3 total coins (maybe they support organizations A and C, but they like A a little more). The second ballot only allocates 2 of its 3 possible coins (they only support organization C and would rather waste their third coin than give it to A or B). So, to make both ballots valid we can safely set:

7.    minTotalCost = 1.

8.    maxTotalCost = 3.

The final variable we need to set is costExponent, which pertains to quadratic voting. We won’t dive into this type of voting for now, so let’s just set the default:

9.    costExponent = 1.

Again, take a moment to reflect on each of these variables, and see if you can understand how changing any one of them might affect our example voting process.

**III.10.****Results parsing:**

The variables above represent the entirety of the Vocdoni Ballot Protocol, which covers ballot validation and results tabulation as handled by the core infrastructure. But there's obviously still a lot of missing information when it comes to the human experience. Integrators of the protocol need to decide how to communicate the actual content of a process to voters, as well as how to parse and represent the results matrix. Results parsing is outside the scope of the Ballot Protocol but is relevant to understanding how the Protocol might be used. In its current iteration, Vocdoni defines two results parsing formats: “Index-weighted” and “Discrete values”.

**1.****Index-weighted**

We would use the Index-weighted results interpretation formula for our example process. This schema is suited for single-question processes such as ranked-choice, multiple choice, or participatory budgeting. Each index in a field of the results matrix represents a weighted value, where in this case the weight represents the number of coins allocated to an organization. The sum of the votes, multiplied by their index-weighted values, is the total value for that field.

![](http://daorayaki.org/content/images/2021/06/--12.png)This interpretation aggregates our example process. Organization A receives 2 coins, organization C receives 3.

**2.****Discrete Values**

Discrete values interpretation is used for processes in which each field is its own question. Here each value represents a single discrete option (i.e. 'Candidate 2'), rather than a multiplier (i.e. '2 points to this option'). As such, this method interprets results by simply reporting which value, if any, received the most votes for each field.

0 is reserved for a tie between options.

![](http://daorayaki.org/content/images/2021/06/--13.png)These two formats are not intended to be exhaustive. As stated above, the Ballot Protocol itself is agnostic to how results are aggregated, and anyone building their own application layer on top of the protocol can define their own results interpretation.

**IV.Contact Information**

**Official Website:** <https://aragon.org/vocdoni>

**Blog:** <https://blog.aragon.org/vocdoni/>

**Twitter**: <https://twitter.com/vocdoni>

**Discord:** [discord.gg/x7GYRB8dpp](https://t.co/jDwGp8n0UD?amp=1)

**Telegram:** <https://t.me/vocdoni>

**Github:** <https://github.com/vocdoni?page=1>



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





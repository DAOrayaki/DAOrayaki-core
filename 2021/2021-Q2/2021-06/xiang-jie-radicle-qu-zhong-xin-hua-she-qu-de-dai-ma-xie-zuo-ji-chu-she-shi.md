

详解Radicle：去中心化社区的代码协作基础设施
=========================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



7 Jun 2021
• 66 min read






![详解Radicle：去中心化社区的代码协作基础设施](/content/images/size/w2000/2021/06/project-source-laptop.png)



**DAOrayaki DAO**研究奖金池：

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 4/7 

通过赏金总量：200 USDC

研究种类：P2P Decentralized Github, Decentralized Code Collaboration, Open-source Work, GIT, Bazaar-style

贡献者： 黑白QB, DAOctor@Daorayaki

上线时间：2018年项目启动，2021年2月以太坊主网上线

Token（代币）：RAD （2021-02-26 首次流动性发行） ERC-20

Token Value（币值）：$6.09（2021-05-31）

Market Value（市值）：$35,281,520.00 （2021-05-31）

![](http://daorayaki.org/content/images/2021/06/----_20210426113809-7.png)Radicle是一个建立在开放协议radicle上的去中心化的代码协作网络。它使开发人员能够在不依赖可信中介机构的情况下进行代码协作。Radicle旨在提供类似于集中式代码协作平台或功能，同时保留Git的点对点性质，旨在做到强分布式版本控制。Radicle还利用以太坊（opt-in）获得独特的全局名称、DAO代码库和一些融资相关的协议，帮助维护者维持其开源工作。

**如何运转？**

该网络由一个建立在Git基础上的点对点复制协议驱动，称为Radicle Link。Radicle Link通过一个叫做 "gossip"的过程来传播数据，用点对点的发现来扩展Git。也就是说，网络中的参与者通过在本地保留冗余副本，并与选定的同伴分享（也称为 "复制"）他们的本地数据，从而分享和传播他们 "感兴趣 "的数据。通过利用Git的智能传输协议，Radicle Link保持了Git在数据复制方面的效率，同时通过点对点网络层提供全球分散的存储库。

由于网络上的所有数据都是由网络上对等的点在本地存储的，所以开发者可以分享和协作Git仓库，而不需要依赖托管服务器等中介机构。

**与GitHub的区别？**

在Radicle上的协作与在GitHub和GitLab等集中式代码协作平台上的协作略有不同。

1）Radicle协作从上到下都是开源的。没有 "封闭 "的组件。Radicle协作的每个组件都是可审计、可修改和可扩展的。

2）Radicle是完全建立在开放协议上的。没有 "特殊服务器"、特权用户或公司来控制你的协作。

3）Radicle是基于点对点的架构，而不是客户端-服务器模式。

4）Radicle默认不是全局性的。相反，你跟踪的同行和项目的社交图决定了你看到的、互动的和复制的内容。

5）Radicle是为集市式开发（bazaar-style development）设计的。这意味着在项目中，没有一个单一的主分支供贡献者合并使用。相反，同行维护他们自己的项目视图，其他同行可以通过补丁获取和合并。

6）Radicle用以太坊上的去中心化组织取代了中心化机构的机关功能及其等级管理模式。

7）Radicle是一个自我维持和社区拥有所有权的网络，而不是一个公司。它的管理依靠一种名为RAD的代币，主要在以太坊上使用。

**如何使用？**

使用Radicle最简单的方法是使用Upstream，这是一个由Radicle项目创始团队开发的桌面客户端。通过Upstream，你可以创建一个身份，托管你的代码，并与Radicle网络上的其他人进行协作。

**创始团队**

·Cory Levinson 联合创始人

Cory Levinson 是 Clovers Network 独立分析师、软件开发者、数据科学家。他是区块链与分布式点技术领域各种项目的积极贡献者，曾分别与 Oscoin、Secure Scuttlebutt 以及最近的 Clovers Network 有合作。

此前，他曾担任数据分析师，后来加入 SoundCloud 数据基础架构团队，工作约 5 年时间。2017 年，他在莫斯科的 Strelka 研究所，开始积极研究区块链领域，在那里领导了能源项目 Phi 的开发。

·Eleftherios Diakomichalis 联合创始人

Eleftherios Diakomichalis 是 Oscoin 联合创始人，由 OSS 合作与激励的去中心化网络与密码货币。另外，他是 SoundCloud 早期员工，此前担任其副总裁，领导数据科学团队。他的兴趣在于网络科学和统计学，侧重于在线社区。

·Abbey Titcomb 联合创始人

Abbey Titcomb 现任 Onward Labs 策略主管。此前，她在 UnderscoreVC 工作过，研究基于协作的加密经济模型和系统设计。

详情介绍：

**1. 为何使用Radicle?**

在过去的十年中，开源已经成为软件开发的一个标准。自由和公开地分享代码，使软件的开发成本大大降低，也更容易，科技创新因此激增。

像GitHub和GitLab这样的代码托管和协作平台通过将开源代入主流受众，为开源的发展做出了巨大的贡献。他们定义了标准的词汇和行为，使更多的人能够接触到git，增强了社会编码的能力，并创造了全球性的开发者社区。一个不可否认的事实是，他们已经完全改变了人们写代码的方式。

这些平台还托管着最大的开源开发存储库，不仅包括代码，还包括问题、拉取请求、评论。 甚至社交关系—明星、点赞、关注—也存在于这些平台中。

然而，这些平台是由公司拥有的。它们受公司法的约束，有权定义其服务条款。他们可以实施用户禁令，比如目前针对伊朗、叙利亚和克里米亚的GitHub账户的禁令，以应对美国政府的压力。它们很容易受到审查制度以及企业和国家目的的影响，这些目的往往与自由和开源社区的目标不一致。

在一个几乎所有的软件都依赖开放源代码的世界里，维护自由和开放源代码生态系统的弹性和健康比以往任何时候都更重要。这就是为什么我们认为，依赖集中托管的平台和公司来分发关键的开源基础设施是不可持续的。对这种集中式服务的依赖与自由和开放源码生态系统的价值相矛盾。

Radicle被认为是一种替代物。其目标是消除中介，建立一个健壮、功能强大和安全的P2P生态系统。必须有一种有意识的改变，优先采用符合自由和开源软件原则的去中心化代码协作替代方案。

**替代方案**

存在GitHub的替代品，从SourceForge和GitLab这样的平台，到更成熟的协作方式，如邮件列表。像Gitea或Gogs这样的平台为代码协作提供了自我托管的开源解决方案，具有较低的平台风险，但使开发者处于孤立的环境中，无法进入全球的开发者网络。一种可行的替代方案是联盟。诸如ForgeFed联合GitLab的提议是朝着正确方向迈出的一步，但实施起来还不够完善。此外，联盟依赖于域名，而域名可能经常被政府扣押。

其他成熟的开源项目，如Linux内核，采用了更多不局限于单一平台的市场化和可访问的开发环境，如邮件列表。这些都是可行的，但当它们被要求达到像GitHub这样的平台所建立的可用性标准时，就会出现问题。

像Scuttlebutt这样的点对点协议为我们提供了分享和托管信息的替代解决方案。这些协议能够在不依赖服务器的情况下离线工作，但建立在它们之上的应用程序缺乏让用户在全球范围内轻松协调的能力。这对博客或社交网络的使用案例来说不是太大问题，但当涉及到软件协作时，为了满足当今集中式平台的可用性和可发现性标准，一个规范的全球注册表是必要的。任何人无论身在何处都能为任何开源项目做出贡献，这对于培养一个真正的自由和开放的网络是必要的。

**设计的原则**

当我们着手构建替代方案时，自由和开源代码协作是不可或缺的价值。 我们制定了以下指导原则列表：

**1.它必须优先考虑用户自由。**

**2.它必须是可访问和抗审查的**任何人都应该有使用该软件与他人协作的自由。任何一方都不能禁止用户访问系统，也不能禁止内容的分享。它必须是可审计和透明的。此外，用户应该有自由控制他们的互动和他们在个人基础上看到的内容。

**3.它必须是用户友好的**该软件必须易于使用，并且不期望用户的行为发生巨大的变化。响应性和功能必须符合当前平台所建立的标准。

**4.它必须是离线优先的**它必须不需要互联网连接、DNS或在线门户才能来运行。必须没有单点故障，而且必须始终可用。

**5.它必须在安全上不妥协**

使用时必须不需要信任第三方或中介机构。该系统的每一个人工制品都必须用加密签名来证明，并进行验证。

让我们在这个框架下看看GitHub或GitLab这样的托管平台：它们的成功在于用户友好和可访问性，但由于它们是集中控制的，所以它们是可审查的，并不优先考虑用户自由。如果我们看看Gitea、Phabricator或Gogs等自我托管的解决方案，它们是免费的、抗审查的、用户友好的，然而，由于把关（gate-keeping）和隔离的环境，它们不容易被访问：跨Phabricator部署的用户不能相互交流。我们所看到的所有目前可用的自我托管解决方案都是这种情况。他们还存在单点故障，并且需要互联网连接来与系统进行大部分互动。

假设一个联合的GitLab可以满足所有的要求，但是，联合的服务不能是离线优先的，也不能提供对用户身份的主权。用户被捆绑在特定的实例上，因此也存在与集中式服务相同的缺点。

像Linux内核邮件列表这样的集市式解决方案几乎在所有概述的原则方面都很成功，但在用户友好性方面却很有限。很难将电子邮件线程的可用性与GitHub和GitLab等平台上可能出现的复杂工作流程进行比较。

**Radicle：一个用于代码协作的点对点堆栈**

Radicle采用了Scuttlebutt社会覆盖范式，在分布式版本控制系统之上建立了一个点对点复制层，首先是git。用户账户和登录被公钥加密技术所取代，托管问题跟踪器被本地对等复制所取代，单一规范上游的想法被基于补丁的点对点或 "集市 “模型所取代。

为了补充复制层，我们引入了一个建立在以太坊上的选择注册表，它持有规范的项目元数据。这使得项目能够锚定重要的信息-如项目状态和存储库负责人-并保证其全球可用性和不可更改性。

需要强调的三个主要主题是：专注于点对点的代码协作模式，建立在底层的分布式版本控制系统上进行复制，以及采用协议优先的方法。

重新审视 “集市“

大教堂和集市 "描述了两种自由软件的开发方式。大教堂模式，以Emacs等项目为例，公开发布版本，但让所谓的 "个人巫师 "独家开发。另一方面，集市模式-由Linus Torvalds推广，并由Linux的巨大成功所验证，要求完全开放的开发，频繁和早期发布，在整个社区内授权，并尽可能多的 "眼球 “关注代码。只要有足够的眼睛，所有的错误都是浅显的。

点对点网络使开发者和维护者更容易开发出不仅是共享的，而且是以实际源代码和安全的对等身份为基础的项目。通过对等复制，补丁变得更加全面，因为它们与开发过程中的本地问题、评论和审查联系在一起。有了更全面的补丁，集市式开发可以保持其灵活性，同时支持更复杂的工作流程。这就是为什么Radicle用90年代和21世纪初开源黑客们所熟悉的点对点模式取代了单一的模式的想法。它使集市式的开发更容易、更好。

这种潜力导致 Radicle 选择了基于gossip的“社交覆盖”，该系统建立在分布式版本控制系统上，该系统免费且始终可用，无需自托管或信任拥有用户数据的公司。

Git gossips优点

下一个设计决定来自于我们对分散存储的实验结果。在IPFS上建立第一个版本的Radicle后，我们遇到了性能和功能问题。主要的认识是，在存储层上点对点地复制git repos，使我们别无选择，只能失去packfile协议，这是git能够快速的原因之一。这种方法会使源代码成为二等公民--这使得存储历史大数据变得不切实际。

在思考上述问题时，一个几乎显而易见的想法出现了：为什么不使用git本身来分发数据？在git中存储合作成果（问题、拉动请求、评论......）以前已经做过了，而且git中的数据结构可以满足我们所有的需求。与gossip层搭配，git就成为了存储、复制和分发代码和协作工件的必要条件。

通过在git之上建立一个点对点的覆盖层，我们不仅找到了一个高性能的解决方案，而且是一个更适合代码协作的解决方案。问题、评论和评论成为本地工件，被加密签名并进行离线交互。

协议，不是平台

大型代码托管平台的故事与互联网从开放协议到私有平台的普遍转变相吻合。今天，大多数社会编码平台实际上利用了开放协议（git、mercurial、ssh），但已经建立了封闭的花园。

Radicle 的方法旨在通过专注于协议优先的理念，并拒绝中介机构的数据收集和孤立。 这反映在构建和扩展git的决策中。 将其作为复制的纽带建立在其优势和去中心化性质之上。 在本地提供问题、拉取请求、评论为开发人员提供了管理和设计工作流程的工具，而无需将他们锁定在新的“体验”中。 尽管将构建任何前端接口，Radicle 最重要的是作为一个开放协议存在—而不是一个平台。

**2、Radicle设计**

Radicle Link是一个带有通用分布式版本控制后端的点对点gossip协议。它的目标是足够通用，可以用在pijul或mercurial等系统之上，尽管它最初的实现主要是支持Git。

该协议通过基于gossip的复制来传播Git存储库，使存储库的托管和共享不依赖于中央服务器。Radicle网络上的存储库被称为 "项目"，由 "同伴 "进行gossip。

在Radicle中。

1）同行跟踪其他同行

2）同伴跟踪他们感兴趣的项目

3）点对点对项目进行闲谈。这意味着复制来自他们所追踪的同伴和他们感兴趣的项目的更新。

4）这些互动创造了一个 "可信的 "同伴和项目的社交图，成为Radicle内部合作的基础。Radicle Link支持集市式的合作模式，其中没有单一的 "主 "分支供贡献者合并，而是由众多的上游通过远程交换补丁。

**身份概述**

Radicle Link区分了两种类型的身份：个人和项目。前者描述了系统中的行为者（同行），而后者描述了一个或多个行为者协作的软件项目（仓库）。

Radicle Link中的 "身份 "概念仅仅意味着在Git存储库中的常规位置存在一个身份文件，该文件要遵守某些验证规则。初始文件的哈希值被认为是其稳定的标识符，并被编码为统一资源名称（URN），其形式为rad:git:$HASH（针对Git仓库）。该URN应该可以在网络上解析为同名的顶级Git仓库（$HASH.git），如果该仓库包含所述身份文件，并且该文件通过了验证规则，则该仓库是有效的。

**数据模型**

我们维护资源库数据一致性的模型，是基于更新框架（TUF），它被设想为安全分发软件包的一种手段。我们的方法是建立一个所有权证明，与一个对等体的网络身份，或一组对等体的网络身份相联系，这样，项目的观点可以根据对等体之间的信任关系进行复制（"跟踪"）。

Revision是一个文件内容的加密哈希值，这样，这个文件在存储系统内可以通过这个哈希值进行内容寻址。

replaces指的是文件的前一个修订版，如果是第一个修订版，则指的是没有。

payload是一个可扩展的、向前和向后兼容的数据类型，包含应用程序定义的关于存储库的元数据。协议解释了其中的一些属性，如Doc Payload中所述。

delegation包含被授权发布和批准文件新修订的密钥所有者的公钥。授权格式取决于正在建立的身份类型。

**Git 实现概述**

Radicle基本上把Git当作一个数据库。这意味着一切都存储在一个单一的Git monorepo中，并通过Upstream客户端进行读取和写入。我们的Git实现是为了激励播种者提供所有必要的数据来解决和验证一个仓库，同时通过尽可能地消除gossip查询和git获取来减少延迟。

**对等发现和复制概述**

Radicle Link 通过一个叫做 gossip 的过程，通过点对点网络发现来扩展 Git。 这意味着网络中的对等点通过在本地保留（复制）冗余副本并与点对点共享增量来共享和传播他们“感兴趣”的数据。使用Radicle，我们根据节点和项目的“社交图”在连接的存储库中复制数据，从而根据用途和价值传播源代码和变更集：对某个项目感兴趣的节点越多，该项目就越可用 项目制作到网络。

**复制模型**

存储库是 Radicle 中复制的基本单元。要将存储库发布到网络，必须首先将其初始化为项目。项目将源代码、问题和提议的更改组合在一个保护伞下，并带有唯一的、可共享的点对点标识符。整个项目数据和元数据，包括评论等社会人工制品，都存储在存储库中。要创建项目，存储库的所有者定义项目身份。在后台，按照惯例 rad/id，在存储库的预定不相交分支中创建项目身份文档。该文件包含重要的元数据，例如项目名称、维护者列表以及任何相关链接。

复制单元是一个存储库，由项目文档上下文中的 PeerID 标识（请参阅数据模型）。相应 DeviceKey 的持有者称为存储库的维护者。属于同一项目的存储库在本地表示为单个存储库，由 Radicle URN（或上游客户端中的 Radicle ID）标识。在项目的上下文中，存储库的维护者可以选择跟踪其他对等点的存储库（这在 git 术语中称为远程：对远程存储库的命名引用）。如果发现远程存储库跟踪其他远程存储库，则跟踪存储库还将传递跟踪这些远程存储库，最多 n 度。

因此，Radicle 上的项目保留了其远程节点的传递信息（即通过哪个跟踪的 PeerID 跟踪另一个 PeerID）。

**追踪**

追踪是协作的基础，因为它推动了项目及其工件的交换。 在 Radicle 中，peer 跟踪他们感兴趣的其他 peer 和项目。当一个 peer 克隆另一个 peer 的项目或通过 Upstream 将它们作为远程添加到他们的项目来直接跟踪一个 peer 时，就会发生这种情况。

由于对等点代表网络中的独立设备，因此他们每个人都有自己的网络视图。 每个对等点都在其自己的 monorepo 中跟踪来自连接对等点的项目、身份和数据的视图。

当一个节点在一个项目的上下文中跟踪另一个节点时——比如说，如果它克隆了另一个节点的项目——它设置了获取和gossip另一个节点对该项目的看法的意图。 这意味着包括项目元数据、所有工作分支和提交，并且变更集将被复制并存储在跟踪peer的 monorepo 中，以便可以获取和协作。

**直接追踪**

一个点可以跟踪另一点的方法是，明确告诉其Monorepo跟踪特定的PEER\_ID。使用带有感兴趣的 PEER\_ID 的 track 函数，monorepo 在 git 配置中创建一个新条目。来自被跟踪peer的任何更新都可以类似地获取并应用到跟踪peer的 monorepo。

Upstream 中的 Manage Remotes 功能使用 track 功能将作为远程的对等点直接添加到项目中。

**社交图（The Social Graph）**

在多个 peer 复制的情况下，任何跟踪项目的 peer 也会隐式跟踪它的维护者。这意味着当网络上的任何 peer 克隆一个项目时，所有该项目的维护者都将最终出现在该 peer 的远程列表中。由于项目的维护者是在项目的规范视图上进行工作的，因此这种自动跟踪功能可以确保在整个网络中散布项目时，其运行状况和一致性。

这也意味着对于单个 PEER\_ID，我们有一个包含更多 PEER\_ID 的子图——无论他们是项目的维护者还是其他被跟踪的同行。任何时候复制一个对等点，他们的子图的一部分也会被复制，最多 2 度。

![](http://daorayaki.org/content/images/2021/06/640-6.png)  
这意味着每次跟踪对等点时，您不仅将它们添加为遥控器，而且还添加了它们的遥控器，以及它们遥控器的遥控器。这确保了项目在整个网络中始终可用，而无需完全依赖项目的维护者或原始跟踪peer。

**验证**

为了确保数据的完整性和真实性，当创建一个项目的工作副本时，根据远程对等体的证明历史在所有其他版本库内容之前被获取，并对其运行验证程序。如果这没有产生一个验证的状态，克隆就会被中止。由此产生的仓库状态必须包括根据远程对等人对身份文件的看法，至少有四分之一的代表的证明历史。在Git中，在获取仓库内容之前，可以通过检查公布的远程参考文献来确定是否会出现这种情况的说法。如果这些前提条件没有得到满足，克隆就会被中止，已经获取的数据也会被剪除

**播种（seeding）**

为了提高数据可用性，网络中的参与者可以选择充当种子。这在概念上类似于 Secure Scuttlebutt 中的酒吧。种子节点是在公共 IP 地址上运行的“永远在线”节点，为任何连接的对等点提供数据。通过加入种子节点，它会自动跟踪您并在其他连接用户的网络中共享您的数据。这提高了您的数据在整个网络中的可用性，同时也更容易找到其他人的数据。

种子可能会跟踪给定项目的大量存储库，因此从种子进行克隆将大大增加跟踪图的连通性。另请注意，通过跟踪种子，上游维护者可以增加返回它们的路径数量，这样即使贡献来自不在维护者的跟踪存储库集中的参与者，也可以回流。

上游预先配置了官方 Radicle 种子节点，以引导您的连接。如果您删除了默认种子节点，您可以随时按照添加种子节点中的步骤重新添加它。

**协作模式**

我们从 git commit 构建的 Identity 允许多个 id 来描述文档的相同修订版（因此同样有效）。这意味着各个代表的历史记录可能会在其提交历史记录中有所不同，但仍会就已证明的文档修订的有效性达成一致。

这意味着上游中没有单一的规范分支（或主），因为同行都在维护自己的同一个项目的上游。但是，由于 Radicle 身份的数据模型，与维护者相关联的项目始终存在“规范”视图。维护者可以遵循基于领导者的工作流程，在该工作流程中，他们将贡献节点的历史融合到他们的主要分支中。由于他们的视图是可验证的，并且在同行关注项目时隐式跟踪，因此，同行可以确保他们正在复制项目的规范和更新视图。

除此之外，Radicle Link 的工作方式对最终用户的协作体验有一定的影响：

您的社交图决定了您看到、互动和复制的内容类型。

假设您已经在 Radicle 网络中发现了一个感兴趣的项目（稍后将详细介绍可发现性），那么为了与其交互，您必须做的第一件事就是跟踪它。跟踪项目表示兴趣，并且设计意味着跟踪项目的维护者，因此在他们的社交图中复制数据。

在项目的上下文中，存储库的维护者可以选择跟踪其他所有者的视图（这在 Git 术语中称为远程：对远程存储库的命名引用）。如果发现远程存储库跟踪其他远程存储库，则跟踪存储库还应传递跟踪这些远程存储库，最多可配置 N 度（目前正在开发中）。

垃圾邮件和内容审核自然由peer的社交图处理

虽然这起初可能看起来令人困惑，但实际上它更自然（它实际上模仿了现实生活中的交流），并且通过设计解决了垃圾邮件和内容审核等问题，这些问题自然由同行的社交图处理。

垃圾邮件发送者的补丁或问题永远不会被实际维护者跟踪，因此网络的其余部分不会看到它们（除非明确跟踪）。同样，如果您对同行的观点或对项目的贡献不感兴趣，您可以简单地取消关注他们，停止复制、查看他们的数据并与之交互。

在同一个项目中，两个同行可能有不同的看法。

上述设计也意味着，即使在同一个项目中，同行也有主观（并且经常有分歧）的观点。

至少，您对项目的看法将成为您所关注人员的看法加上项目维护者的看法的总和。此外，您可以通过配置复制设置来扩展您的视角，以便还可以从您关注的peer（即，peer的peer/远程方的远程方）传递跟踪 N 度以外的其他远程方。

这种设计也解决了完全依赖分布式账本技术的去中心化系统的一个重要问题，即 "区块链中毒 "的问题。这是指有人故意将非法内容添加到仅有的append source中，希望使复制项目的唯一行为产生法律上的问题，正如Linux基金会的Konstantin Ryabitsev正确指出的关于依赖IPFS的Radicle的前一个版本。

**3、代币**

Radicle项目的建立有两个主要目标。

1）开发有弹性的合作基础设施，尊重用户的自由，不依赖可信的守门人，也不依赖企业或国家。

2）利用新开发的主权金融基础设施（比特币、以太坊、DeFi），以便为开发者创造新的价值流并发展数字公域。

为了实现这两个目标，一直有一个先决条件：让Radicle能够自我维持。

Radicle项目已经在网络上发布了1000多个项目，并且在其公开测试版中每周平均增长8%，Radicle项目已经准备好在其社区中分散网络，并开始寻求自我可持续发展。

**为什么选择代币？**

虽然主权和审查抵制的论点继续加强，但去中心化的理由超越了技术。在当前的闭源网络时代，用户已经放弃了对其隐私和软件自由的控制权，以自由方便地进入开放互联网。现在，他们正在寻找替代方案，因为我们的全球社交平台由于社会压力、缺乏创新以及满足利益相关者所需的无情开采而恶化。

在这种现实中，在传统范式中构建 Radicle，例如 SaaS 或开放核心公司，将迫使用户保持客户/公司关系，使他们容易受到最终提取（extraction）的影响。此外，如果Radicle要成为真正尊重用户自由的弹性协作基础架构，则需要在考虑信任最小化的情况下进行开发，让世界上任何人都可以访问它，同时在资金雄厚的大型市场中保持适应性和竞争力- 公司。摆脱这种模式的唯一方法是构建自给自足和社区所有的免费和开源网络。

在这些限制条件下，Radicle 将基于代币的可持续性模型视为最有希望的前进道路。更具体地说，正是加密网络中治理原语的出现，为工程社区拥有的开源协议和网络提供了一个新的设计空间。这些原语为真正“开放”的开源世界提供了基础，而不受任意墙的束缚。

出于这些原因，Radicle 项目将作为一个开源、社区主导和自我维持的软件协作网络向前发展。 Radicle的Ethereum集成将实现这一愿景，这是一套补充Radicle对等网络的开放协议。它的智能合约系统支持独特的全球名称、分散的组织和经验，帮助维护者维持他们的开源工作。集成的智能合约系统将使用 Radicle 代币去中心化——这是一种治理代币，可实现 Radicle 网络的集体治理和长期可持续性。

**如何运转？**

Radicle 代币 (RAD) 被设计为一种治理代币，它支持许多基于以太坊的功能以及 Radicle 网络的公共所有权、集体治理和长期可持续性。

简而言之，Radicle 代币的经济模型会在用户与某些基于以太坊的协议交互时向用户收取费用，除非他们是成员（代币持有者）。通过购买（或获得奖励）并持有一定数量的代币，用户可以避免（或打折）费用并参与网络治理。成员保持对所有基于以太坊的智能合约的管理控制权，最重要的是，拥有超过 50% 的代币总供应量的Radicle金库。

任何人都可以通过购买和持有一定数量的 Radicle 代币成为会员，以换取以下好处：

1）与 Radicle 基于以太坊的协议交互时可享受折扣或不收费。

2）参与Radicle智能合约系统治理（通过投票和提案）的权利。

通过为 Radicle 用户提供持有代币的功能性理由，他们可以体验治理带来的好处，并开始为数字开源基础设施的公共所有权建立新的范式。如果出于任何原因，他们对网络不满意，他们可以通过参与治理来“表达”担忧，或者可以通过向市场出售代币来“退出”。

**治理**Radicle

治理模块是一个复合分叉，赋予所有者参与 Radicle 智能合约系统治理的权利。明确地说，这意味着会员可以控制和参数化其会员体验-无论是通过更改费用，升级合同还是引入新的体验。

选择 Compound 治理模块是因为它经过了实战测试、审计，并通过其流动授权方案平衡了执行权与社区参与。

与 Compound 类似，每个 RAD 代币等于一票，并且通过将投票权委托给代币持有者选择的地址（或多个地址）来启用投票：

1）业主自己的钱包，如果他们想自己投票。

2）另一个用户的钱包，如果他们希望另一个用户代表他们投票。

3）没有钱包，如果他们不想投票。

任何将1%的RAD委托给其地址的人都可以提出治理动作。建议是可执行代码，而不是团队或基金会实施的建议。所有提案都有3天的投票期，任何有投票权的地址都可以对提案投赞成票或反对票。

**金库**

与其他去中心化协议类似，选择加入Radicle的一些Ethereum功能会产生网络费用。这些费用累积在Radicle财库中，这是一个智能合约，占整个代币供应量的50%。

财政部完全由Radicle代币持有人通过Radicle DAO控制。成员将通过社区计划和倡议协调库房的供应分配，从而支持网络的长期可持续性。这些社区项目（例如，开发者挖矿，贡献者奖励，赠款等……）将通过Radicle社区有机地出现，因为Radicle成员使用国库来不断支持网络的增长和恢复力。

网络的代码和资产库是公开管理的，允许任何开发者为项目做出贡献并影响项目的发展方向，使Radicle成为集体治理的实验。

代币分配和发布时间表1 亿个 Radicle 代币（固定）已在创世时铸造，并将在 4 年内授予。

1）50% 社区资金（归属超过 4 年）

2）19% 团队（从加入之日起 4 年归属，从创世起 1 年锁定）

3）20% 早期支持者（1 年锁定期）

4）5% 基金会（1 年锁定期）

5）2% 种子计划（1 年锁定期）

6）~4% 流动性引导池

![](http://daorayaki.org/content/images/2021/06/640--1--2.png)**4、问答**

在 Radicle 上进行协作与在 GitHub 上协作有何不同？

与集中式代码协作平台相比，Radicle专为集市式协作而设计。 在Radicle网络上，内容通过称为gossip的过程进行点对点分发。 这意味着同级可以控制他们的社交互动，因为他们自托管自己的内容以及他们感兴趣的任何同级的内容。这也意味着在项目中，没有贡献者合并到一个单一的主分支。 每个peer都使用其变更集和分支维护项目的视图。 这些观点会被其他对这些变化感兴趣的同行gossip。

Radicle 如何比中心化平台更安全？

Radicle 网络是点对点的，建立在公钥密码学基础上。 首先，这意味着无需依赖第三方来访问或使用 Radicle 网络。 由于没有失败的中心点，并且可以抵抗公司和国家的捕获和审查，因此更难取缔。 此外，Radicle 网络上的所有数据都经过加密签名和验证，因为它在peer之间进行gossip。 虽然中心化平台依赖用户界面组件和关键预言机来表示用户与用户之间的信任，但 Radicle 已将信任设计为协议的核心。

Radicle 如何与 Git 交互？

Radicle Link-为 Radicle 网络提供动力的协议建立在 Git 上。 所有 Radicle 数据都存储在您机器上的单个 Git monorepo 中，通过上游客户端读取和写入。 

Radicle如何获得许可？

Radicle 是完全免费和开源的。 它在 GNU 通用公共许可证 (GPLv3) 的第 3 版下使用 Radicle Linking Exception 获得许可。

问题和 PR 将如何运作？

社交协作功能（即错误报告、补丁、讨论等）都在 Radicle 路线图上。 它们的工作方式与我们现在的体验非常相似，但将是本地优先和加密签名的。 这意味着问题、PR 和讨论将更加安全，可离线使用，并作为 git 对象存储在您的机器上-而不是在中央服务器上！

我可以在 Radicle 上备份 GitHub 项目吗？

是的！将代码库发布到 Radicle 是创建存储库点对点备份的好方法。在 Radicle 上维护一个项目的镜像就像推送到另一个遥控器一样简单。阅读有关创建项目的更多信息。

我可以用 Radicle 替换 GitHub 吗？

如果你想！虽然我们的 Beta 版本将只有基本的协作功能（即代码托管、共享、签出和推送/拉取），但我们计划引入可以支持与 GitHub 类似的日常代码协作体验的功能。它们将包括错误报告，补丁，代码审查和讨论。

话虽如此，虽然我们认为减少对中央托管平台的依赖通常是一个好主意，但我们也相信代码协作解决方案为不同的人服务于不同的目的。 Radicle Upstream将支持社交协作，但其首要任务是提供安全的，本地优先的，对等代码协作-而不是确切的GitHub副本。

我的数据存储在哪里？

在Radicle网络上，内容通过称为gossip的过程进行点对点分发。 这意味着对等点在他们的机器上本地的 Git monorepo 中自行托管他们自己的内容——以及他们感兴趣的任何对等点的内容。 这也意味着无论何时您的数据发布到网络，它都可以被复制并存储在另一台对等机器上。

我可以在 Radicle 上创建私有存储库吗？

不，还没有-但是将来！ 具有端到端加密的私人项目在我们的路线图上。 同时，请务必注意，放置在Radicle上的所有内容都可以公开获得。

什么是remote？

远程是指你的项目由另一个人维护的项目版本。要在 Radicle 上与其他人合作，你必须添加并关注其他人的remote才能从他们那里获取更改。 你可以在项目页面上管理remote。

什么是 Radicle ID？

Radicle ID 是在 Radicle 网络中识别项目的独特方式。 您可以在项目页面或种子节点仪表板上找到它。 

什么是设备 ID？

设备 ID 是绑定到特定设备的peer公钥的编码。 未来人们将能够管理多个设备 ID，但目前每个身份只能有一个设备 ID。

我可以在多个设备上使用 Radicle 吗？

可以，但是目前没有。 尽管还没有多设备支持，但是您仍然可以在不同的设备上创建帐户，但是它们不会被链接到一个上游用户帐户下。

我如何确保没有其他人知道我的显示名称？

你还不能…… 我们将很快引入独特的名称。

我可以删除项目吗？

目前，此功能不受支持，但已在路线图中，并将包含在即将发布的版本中。在此之前，您只能从本地机器上删除您的项目，从而限制了可以找到和复制您的项目的对等点数量。您不能从其他peer的本地机器上删除项目，因为他们保留对其本地数据的控制权。

为什么我只连接到一个对等点？

默认情况下，上游客户端连接到Radicle操作的种子节点。虽然我们支持流行病广播来寻找并连接到其他对等点，但我们目前不支持打孔，这将阻止两台计算机之间的稳定连接。

**5、合约Radicle Token:**

 Radicle Token: 0x31c8eacbffdd875c74b94b077895bd78cf1e64a3

Governance: 0x690e775361AD66D1c4A25d89da9fCd639F5198eD

Timelock: 0x8dA8f82d2BbDd896822de723F55D6EdF416130ba

Genesis: 0x6838f63899728816f602B3e9bF73952e2bD6dc35

Registrar: 0x37723287Ae6F34866d82EE623401f92Ec9013154

**6、联系方式**

Twitter：https://twitter.com/radicle\_xyz?ref=block123

Blog：https://radicle.xyz/blog/

Community：https://radicle.xyz/community.html

Code：https://github.com/radicle-dev

官网：https://radicle.xyz/

**Radicle：Code collaboration infrastructure for decentralized communities--P2P decentralized Github**

DAOrayaki DAO Research Grant：

Fund Address: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

Voting Result：DAO Committee 4/7 

Grant Amount：200 USDC

Category: (P2P decentralized Github, DECENTRALIZED CODE COLLABORATION, open-source work, GIT, bazaar-style )

Contributor：黑白QB, DAOctor@Daorayaki

Launch time：The project started in 2018 and launched on the mainnet of Ethereum in February 2021

Token：RAD （2021-02-26 LBP）ERC-20

Token Value：$6.09（2021-05-31）

Market Value：$35,281,520.00 （2021-05-31）

**What is Radicle?**

Radicle is a decentralized code collaboration network built on open protocols 🌱. It enables developers to collaborate on code without relying on trusted intermediaries. Radicle was designed to provide similar functionality to centralized code collaboration platforms — or "forges" — while retaining Git’s peer-to-peer nature, building on what made distributed version control so powerful in the first place.

Radicle also leverages Ethereum (opt-in) for unique global names, decentralized organizations, and protocols that help maintainers sustain their open-source work.

**How it works**

The network is powered by a peer-to-peer replication protocol built on Git, called Radicle Link. Radicle Link extends Git with peer-to-peer discovery by disseminating data via a process called gossip. That is, participants in the network share and spread data they are "interested" in by keeping redundant copies locally and sharing, otherwise known as "replicating", their local data with selected peers. By leveraging Git's smart transfer protocol, Radicle Link keeps Git's efficiency when it comes to data replication while offering global decentralized repository storage through the peer-to-peer networking layer.

Since all data on the network is stored locally by peers on the network, developers can share and collaborate on Git repositories without relying on intermediaries such as hosted servers.

**How is Radicle different from GitHub?**

Collaborating on Radicle is slightly different than collaborating on centralized code collaboration platforms like GitHub and GitLab.

* The Radicle stack is open-source from top to bottom. There are no "closed" components. Every component of the Radicle stack is auditable, modifiable, and extendable.
* Radicle is built entirely on open protocols. There are no "special servers", privileged users or companies in control of your collaboration.
* Radicle is based on a peer-to-peer architecture instead of a client-server model.
* Radicle is not global by default. Instead, the social graph of peers and projects you track determines what content you see, interact with, and replicate.
* Radicle is designed for bazaar-style development. This means that within projects, there isn't a single master branch that contributors merge into. Instead, peers maintain their own views of projects that can be fetched and merged by other peers via patches.
* Radicle replaces the Org functionality of centralized forges and their hierarchical admin models with decentralized organizations on Ethereum
* Radicle is a self-sustained and community-owned network — not a corporation. It's governance is organized by a token called RAD that lives on Ethereum.

**How do I use Radicle?**

The easiest way to use Radicle is with Upstream, a desktop client developed by the founding team of the Radicle project. With Upstream, you can create an identity, host your code, and collaborate with others on the Radicle network.

**Founding Team**

**Cory Levinson Co-Founder**

Cory Levinson is an independent analyst, software developer, and data scientist at Clovers Network. He is an active contributor to various projects in the blockchain and distributed point technology space, having worked with Oscoin, Secure Scuttlebutt, and most recently Clovers Network, respectively.

Previously, he worked as a data analyst and later joined the SoundCloud data infrastructure team for about five years. in 2017, he started active research in the blockchain space at the Strelka Institute in Moscow, where he led the development of the energy project Phi.

**Eleftherios Diakomichalis Co-founder**

Eleftherios Diakomichalis is the co-founder of Oscoin, a decentralized network, and cryptocurrency inspired by the OSS partnership. In addition, he was an early employee of SoundCloud and previously served as its VP, leading the data science team. His interests lie in network science and statistics, with a focus on online communities.

**Abbey Titcomb Co-Founder**

Abbey Titcomb is currently the Head of Strategy at Onward Labs. Previously, she worked at UnderscoreVC on collaboration-based crypto-economic models and system design.

**Details Introduction**

**1 Why Radicle?**

Throughout the last decade, open source has become a standard for software development. Sharing code freely and publicly has made it drastically cheaper and easier to build software—and tech innovation is surging as a result.

Code hosting and collaboration platforms like GitHub and GitLab have contributed heavily to the growth of open source by bringing it to a mainstream audience. They defined standard vocabulary and behaviors, made git accessible to a greater audience, empowered social coding, and created global communities of developers. It is an undeniable fact that they have completely changed the way people write code.

As the status quo for code collaboration, these platforms also host the largest repositories of open source development made up of not just code, but issues, pull requests, reviews, and comments. Even the social relationships—stars, likes, follows—exist solely within these platforms.

These platforms, however, are owned by corporations. They are subject to corporate law and have the right to define their terms of services. They can implement user bans—like those currently in place against Iranian, Syrian, and Crimean GitHub accounts in response to pressure from the U.S. government. They are vulnerable to censorship as well as corporate and state ends, which are often misaligned with the goals of free and open source communities.

In a world where nearly all software relies on open source code, maintaining the resilience and health of the free and open source ecosystem is more important than ever. That's why we believe that dependence on centrally hosted platforms and corporations for the distribution of critical open source infrastructure is unsustainable. Reliance on such centralized services contradicts the values of the free and open source ecosystem and threatens its well-being.

Radicle was conceived as an alternative. Its goal is to eliminate intermediaries and create a peer-to-peer ecosystem that is robust, functional, and secure. There must be an intentional shift in narrative to prioritize the adoption of decentralized alternatives for code collaboration that abide by the principles of free and open source software.

**Exploring alternatives**

Alternatives to GitHub exist ranging from platforms like SourceForge and GitLab, to more established methods of collaboration such as mailing lists. Platforms like Gitea or Gogs offer self-hosted and open source solutions for code collaboration that have low platform risk but leave developers in isolated environments with no access to the global network of developers. One proposed alternative is federation. Proposals such as ForgeFed and federated GitLab are a step in the right direction, but implementations are underdeveloped or lacking. In addition, federation is dependent on domain names which can and are regularly seized by governments.

Other well-established open-source projects such as the Linux kernel adopt more bazaar and accessible development environments that aren't confined to single platforms, such as mailing lists. These work, but they falter when held to the usability standard that platforms like GitHub have established.

Peer-to-peer protocols like Scuttlebutt have provided us with alternative solutions to share and host information. These protocols are able to work offline without reliance on servers, but applications built on them lack the ability for users to easily coordinate on a global scale. This isn't too much of an issue for a blogging or social networking use case, but when it comes to software collaboration, a canonical global registry is necessary to meet the usability and discoverability standards of centralized platforms today. The ability for anybody to contribute to any open source project no matter where they are is necessary to cultivate a truly free and open network.

**Designing by principles**

As we set out to build an alternative, we started by thinking about the values that we recognize as integral to free and open source code collaboration. With that said, we developed the following list of guiding principles:

1. It must prioritize user freedom In the words of the free software movement:
2. It must be accessible and uncensorable

Anyone should have the freedom to use the software to collaborate with others. No single party should be able to ban users from accessing the system, or content from being shared. It must be auditable and transparent. In addition, users should have the freedom to control their interactions and the content they see on an individual basis.

1. It must be user-friendly

The software must be easy to use and not expect tremendous change in behavior from the user. Responsiveness and functionality must meet the standards established by current platforms.

1. It must be offline-first

It must not require internet connectivity, DNS or online portals to function. There must be no single point of failure and it must be always available.

1. It must not compromise on security

Trust in a third party or intermediary must not be required for use. Every artefact of the system must be attested with cryptographic signatures, and verified.

Let’s look at hosting platforms like GitHub or GitLab in the context of this framework: they succeed by being user-friendly and accessible, but since they are centrally controlled, they are censorable, and do not prioritize user freedoms. If we look at self-hosted solutions like Gitea, Phabricator or Gogs, they are free, uncensorable, and user-friendly, however, they are not easily accessible due to gate-keeping and isolated environments: users across Phabricator deployments cannot interact with each other. This is the case for all currently available self-hosted solutions we've looked at. They also present single points of failure and require internet connectivity for most interactions with the system.

Hypothetically, a federated GitLab could fill all the requirements, however, federated services cannot be offline-first and don’t offer sovereignty over user's identity. Users are tied to specific instances and thus subject to some of the same drawbacks as centralized services.

Bazaar-style solutions like the Linux Kernel mailing list succeed at almost all outlined principles, but are limited in terms of user friendliness. It's hard to compare the usability of email threads to the sophisticated workflows possible on platforms like GitHub and GitLab.

**Radicle: A peer-to-peer stack for code collaboration**

Radicle adopts the Scuttlebutt social overlay paradigm by establishing a peer-to-peer replication layer on top of distributed version control systems, starting with git. User accounts and login is replaced by public key cryptography, hosted issue trackers are replaced by local peer replication, and the idea of a single canonical upstream is replaced by a patch-based peer-to-peer or "bazaar" model.

To complement the replication layer we introduce an opt-in registry built on Ethereum which holds canonical project metadata. This allows projects to anchor important information-such as project state and repository heads-with the guarantee of global availability and immutability.

The three major themes to highlight are the decisions to focus on a peer-to-peer code collaboration model, to build on the underlying distributed version control system for replication, and to adopt a protocol-first approach.

**Revisiting the Bazaar**

The Cathedral and the Bazaar describes two approaches to free software development. The cathedral model, exemplified by projects like Emacs, makes releases open and available but keeps development exclusive to so called "individual wizards". On the other hand, the bazaar model—popularized by Linus Torvalds and validated by the massive success of Linux, calls for completely open development with frequent and early releases, delegation throughout communities, and as many "eyeballs" on the code as possible. Given enough eyeballs, all bugs are shallow.

Peer-to-peer networking makes it far easier for developers and maintainers to develop not just a shared, but a trusted representation of project state grounded in actual source code and secure peer identities. With peer replication, patches become more comprehensive because they are tied to local issues, comments, and reviews connected to the development process. With more comprehensive patches, bazaar-style development can retain its flexibility while supporting more sophisticated workflows. This is why Radicle replaces the idea of a single canonical upstream with a peer-to-peer model familiar to the open source hackers of the 90s and early 2000s. It makes bazaar-style development easier and better.

This potential is what caused Radicle to settle on a gossip-based "social overlay" built on distributed version control systems that is free and always available without the hassle of self-hosting or trusting companies with user data.

**Git gossips well**

The next design decision came as a result of our experimentation with decentralized storage. After building the first version of Radicle on IPFS, we ran into performance and functionality issues. The major realization was that replicating git repos peer-to-peer on the storage layer left us no choice but losing the packfile protocol, one of the things that makes git fast. This approach would make source code a second-class citizen—making it impractical to store repositories with large histories.

When reflecting on the above, the almost obvious thought returned: why not use git itself to distribute data? Storing collaboration artifacts (issues, pull requests, comments, ...) in git has been done before and the data structures available in git satisfy all our needs. Paired with a gossip layer, git becomes exactly what's necessary to store, replicate and distribute code and collaboration artifacts.

By building a peer-to-peer overlay on top of git, we find not only a performant solution, but one that is better adapted for code collaboration. Issues, comments and reviews become local artifacts that are cryptographically signed and interacted with offline.

**Protocols, not platforms**

The story of the big code hosting platforms coincides with the general shift of the internet from open protocols to privately-owned platforms. Most social coding platforms today actually leverage open protocols (git, mercurial, ssh) but have built up closed gardens.

Radicle's approach is meant to return to the protocol-first philosophy by focusing on building code collaboration primitives instead of user experiences, and to reject data collection and siloing by intermediaries. This is reflected in the decision to build on and extend git. Having it as the nexus of replication builds on its strengths and decentralized nature. Having issues, pull requests, comments, and reviews locally gives developers the tools to manage and design their workflows without locking them into a new "experience". Despite any front-end interface that will be built, Radicle exists foremost as an open protocol — not a platform.

**2 How it Works**

**Overview**

Radicle Link is a peer-to-peer gossip protocol with a generic distributed version control backend. It aims to be general enough to be used on top of systems such as pijul or mercurial, though it's initial implementation is focused on supporting Git.

The protocol disseminates Git repositories via gossip-based replication, enabling the hosting and sharing of repositories without reliance on central servers. Repositories on the Radicle network are called 'projects', which are gossiped by 'peers'.

In Radicle:

* Peers track other peers
* Peers track projects they are interested in
* Peers gossip about projects. This means replicating updates from the peers they track and the projects they are interested in

These interactions create a "trusted" social graph of peers and projects that become the foundation for collaboration within Radicle.

Radicle Link supports a bazaar-style collaboration model in which there is no single canonical 'master' branch that contributors merge into, but a multitude of upstreams exchanging patches via remotes.

**Identities**

**Overview**

Radicle Link distinguishes two types of identities: personal and project. The first describes an actor (a peer) in the system, while the second describes a software project (repository) on which one or more actors collaborate.

The notion of "identity" in Radicle Link simply means the presence of an identity document at a conventional location within a Git repository, where the document is subject to certain verification rules. The hash of the initial document is considered its stable identifier and encoded as a uniform resource name (URN) of the form rad:git:$HASH (for Git repositories). The URN is supposed to be resolvable on the network into a top-level Git repository of the same name ($HASH.git), which is valid if it contains said identity document, and the document passes the verification rules.

**Data Model**

Our model for maintaining consistency on repository data, is based on The Update Framework (TUF), which was conceived as a means of securely distributing software packages. Our approach is to establish an ownership proof, tied to the network identity of a peer, or a set of peers, such that the views of a project can be replicated according to the trust relationships between peers ("tracking").

Revision is a cryptographic hash of a document's contents, such that this document is content-addressable by this hash within the storage system.

replaces refers to the previous revision of the document, or none if it is the first revision.

payload is an extensible, forwards- and backwards-compatible datatype containing application-defined metadata about the repository. The protocol interprets some of the properties, as described in Doc Payload.

delegations contains the public keys of key owners who are authorised to issue and approve new revisions of the document. The delegation format depends on the type of identity being established.

**Git Implementation**

**Overview**

Radicle basically uses Git as a database. This means everything is stored in a single Git monorepo that is read and written from via the Upstream client. Our Git implementation was devised to create an incentive for the seeder to provide all data necessary to resolve and verify a repository, while reducing latency by eliminating gossip queries and git fetches as much as possible.

**Peer Discovery & Replication**

**Overview**

Radicle Link extends Git with peer-to-peer network discovery via a process called gossip. This means that peers in the network share and spread data they are "interested" in by keeping (replicating) redundant copies locally and sharing deltas with peers. With Radicle, we replicate data across connected repositories according to a “social graph” of peers and projects, enabling source code and changesets to be disseminated according to use and value: the more peers who are interested in a certain project, the more available this project is made to the network.

**Replication Model**

Repositories are the base unit of replication in Radicle. To publish a repository to the network, it must first be initialized as a project. Project combine source code, issues and proposed changes under a single umbrella, and carry a unique, shareable peer-to-peer identifier. The entirety of the project data and metadata, including social artefacts such as comments, are stored within the repository. To create a project, the owner of a repository defines a project identity. In the background, a project identity document is created in a predetermined disjoint branch of the repository, by convention rad/id. This file contains important metadata such as the project name, list of maintainers, as well as any related links.

The unit of replication is a repository, identified by a PeerID in the context of a project document (See Data Model). The holder of the corresponding DeviceKey is referred to as the maintainer of the repository. Repositories belonging to the same project are represented locally as a single repository, identified by a Radicle URN (or Radicle ID in the Upstream client). In the context of a project, the maintainer of a repository may choose to track the repositories of other peers (this is called a remote in git terminology: a named reference to a remote repository). If the remote repository is found to track other remotes, the tracking repository will also transitively track those, up to n-degrees out.

Therefore, a project on Radicle preserves the transitivity information of its remotes (i.e. via which tracked PeerID another PeerID is tracked).

**Tracking**

Tracking is the backbone of collaboration as it drives the exchange of projects and their artifacts. In Radicle, peers track other peers and projects that they are interested in. This happens when a peer clones another peer's project or tracks a peer directly by adding them as a remote to their project via Upstream.

Since peers represent seperate devices in the network, they each have their own view of the network. Each peer tracks this view of projects, identities, and data from connected peers in its own monorepo.

When a peer tracks another peer in the context of a project — say, if it clones another peer's project — it sets the intention to fetch and gossip the other peer's view of that project. This means includes the project metadata, all working branches and commits, and changesets will be replicated and stored in the tracking peer's monorepo, so that it can be fetched and collaborated on.

**Direct Tracking**

The other way a peer can track another peer is by explicity telling their monorepo to track a specific PEER\_ID. Using the track function with PEER\_ID of interest, the monorepo creates a new entry in the git config. Any updates from the tracked peer can be similarly fetched and applied the tracking peer's monorepo.

The Manage Remotes feature in Upstream uses the track function to add peers as remotes directly to the project.

**The Social Graph**

In the case of multiple peer replications, any peer that tracks a project will implicitly track it's maintainers as well. This means that when any peer on the network clones a project, all of said project's maintainers will end up in that peer's remote list. Since maintainers of the project work on the canonical view of the project, this automatic tracking ensures the health and consistency of a project as it's gossiped across the network.

This also means that for a single PEER\_ID, we have a sub-graph that consists of more PEER\_IDs — whether they be the maintainers of the project or other tracked peers. Any time a peer is replicated, a portion of their sub-graph is replicated as well, up to 2 degrees out.

This means that everytime you track a peer, you are not only adding them as a remote, but also their remotes, and the remotes of their remotes. This ensures that a project is consistently available across the network without a total reliance on the maintainers of the project or the original tracked peer.

![](http://daorayaki.org/content/images/2021/06/640-7.png)**Validation**

To ensure data integrity and authenticity, when creating a working copy of a project, the attestation history according to the remote peer is fetched before all other repository contents, and the verification procedure is run on it. If this does not yield a verified status, the clone is aborted. The resulting repository state must include the attestation histories of at least a quorum of the delegates as per the remote peer's view of the identity document. In Git, the claim that this will be the case can be determined before fetching the repository contents by examining the advertised remote refs. If these preconditions are not met, the clone is aborted, and already fetched data is pruned.

**Seeding**

To improve data availability, participants in the network can choose to act as seeds. This is similar in concept to a pub in Secure Scuttlebutt. Seed nodes are "always-on" nodes running on public IP addresses that serve data to any connected peers. By joining a seed node, it automatically tracks you and shares your data across its network of other connected users. This increases the availability of your data throughout the network, while making it easier to find other's data as well.

A seed may track a large number of repositories for a given project, so cloning from a seed will greatly increase the connectedness of a tracking graph. Also note that, by tracking a seed, upstream maintainers can increase the number of paths leading back to them, such that contributions can flow back up even if they come from participants not within the set of tracked repositories of a maintainer.

Upstream is preconfigured with an official Radicle seed node to bootstrap your connectivity. If you have removed the default seed node, you can always re-add it later by following the steps in Adding a seed node.

**Collaboration Model**

Our construction of the Identity from a git commit allows for multiple ids to describe the same revision of the document (and thus be equally valid). This means that the respective delegates' histories may diverge in their commit histories, but still converge to an agreement on the validity of the attested document revision.

This means that there isn't a single canonical branch (or master) in Upstream, as peers are all maintaining their own upstreams of the same project. However, due to the data model of Radicle idenities, there will always be a 'canonical' view of a project associated with its maintainers. Maintainers can follow a leader-based workflow in which they are converging histories of contributing peers into their main branch. Since their view is verifiable and implicitly tracked whenever a peer follows a project, peers can ensure they are replicating a canonical and updated view of a project.

In addition to this, the way Radicle Link works introduces certain implications for end-user collaboration experience:

Your social graph determines what type of content you see, interact with and replicate.

Assuming you have discovered a project of interest within the Radicle network (more on discoverability later), then the first thing you have to do in order to interact with it is to track it. Tracking a project signals interest, and by design implies tracking the project's maintainers, therefore replicating the data within their social graphs.

In the context of a project, maintainers of a repository may choose to track the views of other owners (this is called a remote in Git terminology: a named reference to a remote repository). If the remote repository is found to track other remotes, the tracking repository shall also transitively track those, up to a configurable N-degrees out (currently in the works).

Spam and content moderation is naturally handled by the peer's social graph

While this might appear confusing at first, in fact its far more natural (it actually mimics real life communication) and by design addresses issues like spam and content moderation, which are naturally handled by the peer's social graph.

A spammer's patches or issues will never be tracked by the actual maintainers and as a result they wont be seen by the rest of the network (unless explicitly tracked). Similarly, if you are not interested in a peer's views or contributions to a project, you can simply un-follow them, stopping to replicate, view and interact with their data.

Within the same project, two peers might have diverging views.

The above design also means that even within the same project, peers have subjective (and often diverging) views.

At minimum, your view of a project becomes the sum of the views of the people you follow, plus the views of the maintainers of the project. In addition, you can expand your perspective by configuring your replication settings to also transitively track other remotes N-degrees out from the peers you follow (i.e. peers of your peers / remotes of your remotes).

This design also addresses a significant problem with decentralized systems relying exclusively on distributed ledger technology, the problem of "blockchain poisoning". This is when someone deliberately adds illegal content to an append only source in hopes to make the sole act of replicating the project legally problematic, as correctly pointed out by Konstantin Ryabitsev of the Linux foundation with regards to a previous version of Radicle that was relying on IPFS.

**3 TOKEN**

The Radicle project was established with two main objectives:

* Develop resilient collaboration infrastructure that respects users freedoms, without a reliance on trusted gatekeepers nor on corporate or state overlords.
* Use the newly developed sovereign financial infrastructure (Bitcoin, Ethereum, DeFi) in order to create new value flows for developers and grow the digital commons.

To accomplish both objectives there has always been one prerequisite: make Radicle self-sustainable.

With over 1000 projects already published to the network and an average growth of 8% week-to-week in its public beta, the Radicle project is ready to decentralize the network among its community and begin the quest towards self-sustainability.

**Why a token?**

While the arguments for sovereignty and censorship-resistance continue to strengthen, the case for decentralization goes beyond the tech. In the current era of the closed-source web, users have relinquished control of their privacy and software freedoms for a free and convenient gateway into the open Internet. Now, they are looking for alternatives as our global social platforms deteriorate due to societal pressure, lack of innovation, and the relentless extraction necessary to satisfy stakeholders.

In this reality, building Radicle within the traditional paradigm, as for example a SaaS or open-core company, would force users to remain in a customer/corporation relationship, leaving them vulnerable to eventual extraction. Additionally, if Radicle is to be resilient collaboration infrastructure that truly respects user freedoms, it needs to be developed with trust-minimization in mind, be accessible to anyone in the world, all while remaining adaptive and competitive in a market with well-funded mega-corporations. The only way out of this pattern is to build free and open source networks that are self-sustaining and community owned.

Operating by these constraints, Radicle recognizes token-based sustainability models as the most promising path forward. More specifically, it’s the emergence of governance primitives within crypto-networks that present a new design space for engineering community-owned open-source protocols & networks. These primitives provide a foundation for a truly "open" open-source world, not one bound by arbitrary walls.

For these reasons, the Radicle project will be moving forward as an open-source, community-led, and self-sustaining network for software collaboration. This vision will be realized by Radicle’s Ethereum integration — a set of open protocols that complement the Radicle peer-to-peer network. Its smart contract system enables unique global names, decentralized organizations, and experiences that help maintainers sustain their open-source work. The integration’s smart contract system will be decentralized with the Radicle token — a governance token that will enable the collective governance and long-term sustainability of the Radicle network.

**How it works**

The Radicle token (RAD) is designed as a governance token that enables a number of Ethereum-based features as well as the communal ownership, collective governance, and long-term sustainability of the Radicle network.

In short, the economic model of the Radicle token subjects users to fees when they interact with certain Ethereum-based protocols, unless they are members (token-holders). By buying (or being rewarded) and holding an amount of tokens, users can avoid (or have discounted) fees and participate in the governance of the network. Members maintain governing control over all Ethereum-based smart contracts and most importantly, the Radicle Treasury which holds more than > 50% of the total token supply.

Anyone can become a member by buying and holding an amount of Radicle tokens, in exchange for the following benefits:

Discounted or no fees when interacting with Radicle's [Ethereum-based protocols](http://radicle.xyz/blog/integrating-with-ethereum.html).

The right to participate in the governance (through voting and proposals) of the Radicle smart contract system.

By giving Radicle users a functional reason to hold the token, they can experience the benefits of governance and start establishing a new paradigm for the communal ownership of digital open-source infrastructure. If, for any reason, they are unhappy with the network, they can “voice” concerns by participating in governance or they can “exit” by selling their tokens to the market.

**Governance**

The Radicle governance module is a [Compound](https://compound.finance/) fork and gives owners the right to participate in the governance of the Radicle smart contract system. Explicitly, this means members can control and parameterize their membership experiences — whether it's by changing fees, upgrading contracts, or introducing new experiences.

The Compound governance module was chosen because it's battle tested, audited, and balances executive power with community participation through its liquid delegation scheme.

Similar to Compound, each RAD token is equal to one vote and voting is enabled by delegating voting rights to the address (or addresses) of the token holder's choice:

* The owner’s own wallet, if they would like to vote on their own.
* Another user's wallet, if they would like the other user to vote on their behalf.
* No wallet, if they don't want to vote.

Anybody with 1% of RAD delegated to their address can propose a governance action. Proposals are executable code, not suggestions for a team or foundation to implement. All proposals are subject to a 3-day voting period, and any address with voting power can vote for or against the proposal.

**Radicle Treasury**

Similar to other decentralized protocols, opting-in to some of Radicle’s Ethereum features incurs network fees. These fees accrue in the Radicle Treasury, a smart contract where 50% of the overall token supply exists.

The Treasury is entirely controlled by Radicle token holders via the Radicle DAO. Members will support the long-term sustainability of the network by coordinating the distribution of the Treasury’s supply via community programs and initiatives. These community programs (e.g. developer mining, contributor rewards, grants etc…) will emerge organically through the Radicle community as Radicle members use the Treasury to continuously support the growth and resilience of the network.

The network’s code and treasury of assets are publicly managed, allowing any developer to contribute to and influence the direction of the project, making Radicle an experiment in collective governance.

**Token Allocation and Release Schedule**

100M Radicle tokens (fixed) have been minted at genesis and will be vested over the course of 4 years.

* 50% Community Treasury (vesting over 4 years)
* 19% Team (4 year vesting from join date, 1 year lock-up from genesis)
* 20% Early Supporters (1 year lock-up*)
* 5% Foundation (1 year lock-up)
* 2% Seeders Program (1 year lock-up*)
* ~4% Liquidity Bootstrapping Pool**

![](http://daorayaki.org/content/images/2021/06/640--1--3.png)**4 FAQ**

**How is collaborating on Radicle different than GitHub?**

In contrast to centralized code collaboration platforms, Radicle is designed for bazaar-style collaboration. On the Radicle network, content is distributed peer-to-peer via a process called gossip. This means that peers are in control of their social interactions as they self-host their own content and the content of any peers they are interested in. This also means that within projects, there isn't a single master branch that contributors merge into. Each peer maintains a view of a project with their changesets and branches. These views are gossiped around to other peers that are interested in those changes.

**How is Radicle more secure than centralized platforms?**

The Radicle network is peer-to-peer and built on public key cryptography. To start, this means that there is no need to rely on third parties to access or use the Radicle network. It is harder to take down because there is no central point of failure, and is resistant to corporate and state capture and censorship. In addition, all data on the Radicle network is cryptographically signed & verified as it's gossiped between peers. While centralized platforms rely on user interface components and key oracles to signal trust from user to user, Radicle has designed trust into the core of the protocol.

**How does Radicle interact with Git?**

Radicle Link-the protocol that powers the Radicle network is built on Git. All Radicle data is stored in a single Git monorepo on your machine that is read from and written to via the Upstream client.

**How is Radicle licensed?**

Radicle is completely free and open-source. It's licensed under version 3 of the GNU General Public License (GPLv3) with the Radicle Linking Exception.

**How will issues and PRs work?**

Social collaboration features (i.e. bug reports, patches, discussions etc...) are all on the Radicle roadmap. They will work very similarly to the experiences we have now, but will be local-first and cryptographically signed. This means issues, PRs, and discussions will be more secure, available offline, and stored on your machine as git objects -not on a central server!

**Can I backup a GitHub project on Radicle?**

Yes! Publishing a codebase to Radicle is a great way to create a peer-to-peer backup of your repositories. Maintaining a mirror of a project on Radicle is as simple as pushing to another remote. Read more about creating projects.

**Can I replace GitHub with Radicle?**

If you want! While our Beta release will have only the basic collaboration features (i.e. code hosting, sharing, checking out, and pushing/pulling), we plan to introduce features that could support a similar day-to-day code collaboration experience to GitHub. They will include bug reporting, patches, code review, and discussions.

That being said, while we believe that reducing one's reliance on centrally-hosted platforms is generally a good idea, we also believe that code collaboration solutions serve different purposes for different people. Radicle Upstream will support social collaboration, but it's priority will be delivering secure, local-first, peer-to-peer code collaboration — not an exact GitHub replica.

**Where is my data stored?**

On the Radicle network, content is distributed peer-to-peer via a process called gossip. This means that peers self-host their own content — and the content of any peers they are interested in — locally on their machine in a Git monorepo. It also means that whenever your data is published to the network, it can be replicated and stored on another peer's machine.

**Can I create private repositories on Radicle?**

No, not yet - but in the future! Private projects with end-to-end encryption are on our roadmap. In the meantime, be sure to note that everything you put on Radicle will be publicly available.

**What is a remote?**

A remote refers to a version of your project that is maintained by another person. To collaborate with others on Radicle, you have to add and follow other their remotes to be able to fetch changes from them. You can manage remotes on your project page.

**What's a Radicle ID?**

A Radicle ID is a unique way of identifying projects in the Radicle Network. You can find it on a project's page or on the seed node dashboard.

**What's a Device ID?**

A Device ID is the encoding of a peer's public key that is tied to a specific device. People will be able to manage multiple Device IDs in the future, but for now you can only have one Device ID per identity.

**Can I use Radicle with multiple devices?**

Yes and no. While there isn't multi-device support yet, you can still create accounts on different devices, they just won't be linked under one Upstream user account.

**How do I make sure nobody else has my display name?**

You can't.... yet. We will be introducing unique names soon.

**Can I delete a project?**

Currently, this feature is not supported but it is on the roadmap and will be included in an upcoming release. Until then, you can only remove your project from your local machine, thus limiting the number of peers who can find and replicate your project. You can not delete a project from another peer's local machine, as they retain control over their local data.

**Why am I only connected to one peer?**

By default, the Upstream client is conecting to a seed node operated by Radicle. While we support epidemic broadcast to find and connect to other peers, we don't have support for hole punching just yet, which will prevent a stable conenction between two computers.

**Contracts**

Radicle Token: [0x31c8eacbffdd875c74b94b077895bd78cf1e64a3](https://etherscan.io/token/0x31c8eacbffdd875c74b94b077895bd78cf1e64a3)

Governance: [0x690e775361AD66D1c4A25d89da9fCd639F5198eD](https://etherscan.io/address/0x690e775361AD66D1c4A25d89da9fCd639F5198eD)

Timelock: [0x8dA8f82d2BbDd896822de723F55D6EdF416130ba](https://etherscan.io/address/0x8dA8f82d2BbDd896822de723F55D6EdF416130ba)

Genesis: [0x6838f63899728816f602B3e9bF73952e2bD6dc35](https://etherscan.io/address/0x6838f63899728816f602B3e9bF73952e2bD6dc35)

Registrar: [0x37723287Ae6F34866d82EE623401f92Ec9013154](https://etherscan.io/address/0x37723287Ae6F34866d82EE623401f92Ec9013154)

**5 Contact Information**

Twitter：<https://twitter.com/radicle_xyz?ref=block123>

Blog：<https://radicle.xyz/blog/>

Community：<https://radicle.xyz/community.html>

Code：<https://github.com/radicle-dev>

Official website：https://radicle.xyz/



---

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）

  
详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)

历史文章：

[Synthetix：去中心化治理结构](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484318&idx=1&sn=ebea1216fb8bdaa17de340aec02274a5&chksm=c1d8024bf6af8b5dcc504cefe8129bd910cc6234a2bd6828f6d9e375a97048209149d1b19e8a&scene=21#wechat_redirect)

[DAOMaker: 代币化的创业孵化器和募资平台](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484380&idx=1&sn=c6b092df9c03839de357626b9a167209&chksm=c1d80209f6af8b1fe100bda68669993ede2058b3495df82b0463f5bf50ea567c344137212dbe&scene=21#wechat_redirect)

[详解Gnosis Safe: 灵活、安全的数字资产管理工具](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484494&idx=1&sn=e2f89b473594c066e30c81e8c737a674&chksm=c1d8059bf6af8c8d2bfaef9a398bad203d4ca95844bd69c55d0703394cadd0cac24aa77c5716&scene=21#wechat_redirect)

[DAO治理中的同构性](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484493&idx=1&sn=4169ed86c19a17a063dc97c9f6b9b87e&chksm=c1d80598f6af8c8e6cac5807f59a01c8e7d062ee3b9806c18b9a5cb139377a7b3c5b55d0dd1d&scene=21#wechat_redirect)

[自动化奥斯特罗姆（Ostrom）以实现有效的DAO管理](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484492&idx=1&sn=a664c1791f6c5c15dbf7a70bff95f1fa&chksm=c1d80599f6af8c8fbb7de3a133867adc4416db070eafe730fce5ff8510aa8c0b10332ae3c75a&scene=21#wechat_redirect)

[Alchemy：预算、协作和DAO管理的去中心化应用程序](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484491&idx=2&sn=d5349b33e7a787156151376914ac22a6&chksm=c1d8059ef6af8c88ba86b617f15373254a62712fb7f1ba2b3bb5d476aac339e2b429426c0ad7&scene=21#wechat_redirect)

[全面解读｜Colony v2：有效降低市场交易成本的DAO基础设施](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484386&idx=1&sn=9e321dfea0e1a7755464f7b844708a05&chksm=c1d80237f6af8b21ab290d3318c1816dd85a21d91057c3c5abe6a600c7c67aa23a2467481ef1&scene=21#wechat_redirect)

[SourceCred：基于贡献的计算信用工具](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484383&idx=1&sn=67f820312396793b6aa143159d38c04c&chksm=c1d8020af6af8b1ceb21fb35bc49aa9e289ab7b38bc733283dd7945e2c5df55b729e61847ce5&scene=21#wechat_redirect)

[二次方融资（Quadratic Funding）的攻击与防守](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484342&idx=1&sn=d5af12dec12244cdc70b1835961dca9b&chksm=c1d80263f6af8b757cb940f4c984fb1309dd8c67f047fd29c0483a040b08e2ddfaa44b4343c9&scene=21#wechat_redirect)

[道德作为通证工程共享（Token Engineering Commons）的使命与动机](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484343&idx=1&sn=aa1f6bb3142b78723c0c48733d343352&chksm=c1d80262f6af8b74bc2f81913487360bf2f5f6dfce48e08b7d6847b841759aa57e879e4e1b54&scene=21#wechat_redirect)

[DAO 联盟|Open DeFi DAO 治理结构](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484317&idx=1&sn=1ac6d1189e6aee909cec138d4d7de226&chksm=c1d80248f6af8b5e09abfb1efdd93ff3e66961d177a0e1f24bfe3a4ecce07ce6fb7362d04611&scene=21#wechat_redirect)

[策展市场|一种构建联合关注网络的机制](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484316&idx=1&sn=90adbf5eccb96834789773506442e5fa&chksm=c1d80249f6af8b5f8e4993c27f2f84019bce612d1bd069cb09fb2b47585922789c2ca061dce5&scene=21#wechat_redirect)

[Farming机制是否代表着代币分配的进步？](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484314&idx=1&sn=38f8fadf609317df6416be9f36cc7063&chksm=c1d8024ff6af8b598f427a174a11a37f97a210b1e7c9da02c4ef36efdce3da84838e6339269d&scene=21#wechat_redirect)

[全方位解读PANVALA：去中心化的以太坊资助平台](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484312&idx=1&sn=4d5174d7c98f9d605634827213fb8887&chksm=c1d8024df6af8b5b7d8ffd4b97279c256381cc991207675c91eccaac86b672640a526d5a1b5d&scene=21#wechat_redirect)

[Social token与DAO思潮下微观经济体的崛起](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484264&idx=1&sn=b87c1c5dc66ad4291f8b2f4743d7276d&chksm=c1d802bdf6af8bab24cfd6897a11fb616047d3101c1eed4dde2f4974400979da81dc549c9bec&scene=21#wechat_redirect)

[什么是社区贡献机会（CCO）？](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484198&idx=1&sn=54dffa59966036ef1e1f6575ba49e3c5&chksm=c1d802f3f6af8be555072f23221f911a3d14c44ef93ccd777a71088ea86f59449054b928e1c1&scene=21#wechat_redirect)

[万字解读| Upshot One 对等预测协议](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484241&idx=1&sn=0e5e335c501f5bca41ed47157cad2b88&chksm=c1d80284f6af8b92c360917fd05ae7db737da4170bf91b49c6f3607b87b4e4bc997e35770578&scene=21#wechat_redirect)

[如何DAO化|基于社区贡献机会（CCO）机制的去中心化治理](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484199&idx=1&sn=d57ee97b1a5c22f9b790ead21fbce7ac&chksm=c1d802f2f6af8be4fd0de26075ad746ae8d5d4f50d9daf3f3a293f3d5dd117ecc142ee498198&scene=21#wechat_redirect)

[罗宾·汉森经典论文（四）|Futarchy：工程设计25个问题](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484198&idx=2&sn=811eb205869e6cd11ed2d21bbc10512f&chksm=c1d802f3f6af8be57cf39a226588f43f4cdcd19f3a28e49776da42d33be0bbf3cc6e9b27bcd7&scene=21#wechat_redirect)

[罗宾·汉森经典论文（三）|Futarchy：工程设计25个问题](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484178&idx=2&sn=a5e207bfea688f4fcbe08c0367e9de99&chksm=c1d802c7f6af8bd1795ceeae71f09585418522c9860c320f2d6ef5bc2d5e1cb6a06f58bc2e17&scene=21#wechat_redirect)

[罗宾·汉森经典论文（二）|Futarchy：我们应该价值投票、对赌信仰吗？](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484168&idx=2&sn=88d850212afe61773c0aa2e8c19e2734&chksm=c1d802ddf6af8bcb3210df536511892dc3ebff4b788e43a8dde348cdb6c132de1705533a2bdf&scene=21#wechat_redirect)

[罗宾·汉森经典论文（一）|Futarchy：我们应该价值投票、对赌信仰吗？](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484154&idx=2&sn=5562e8b04ffd450720a7b9a49b8dbcd3&chksm=c1d8032ff6af8a39d7a4bb58d97833829ee97ee8969703ea41c31231818997e6e79a1cba0d7f&scene=21#wechat_redirect)

[DAOs的设计再思考：信任与决策权、风险、剩余索取权的分配](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484100&idx=1&sn=336bdc7b92314aeea4f24fcddaf2d165&chksm=c1d80311f6af8a07a18fd5e9aa0226d011283575c6707d2bd241afc93258a72c13e38d84ba27&scene=21#wechat_redirect)

[基于 Futarchy治理的案例：Amoveo、Tezos、Gnosis](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484178&idx=1&sn=286ca0a3bb98b585e3b41cf41de348b8&chksm=c1d802c7f6af8bd135b1ab5fbf1e639f0a8ccb210a1311b967018770f303a89da8b1ada7b306&scene=21#wechat_redirect)[联合曲线设计脑洞大全及参数大典](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484168&idx=1&sn=939737a69feb60a822ebd86b8d94cce1&chksm=c1d802ddf6af8bcba3944b673af03cf03404cde39285c6e2a605ea99e14e606631f4a6cd4523&scene=21#wechat_redirect)

[DAOrayaki首发| SEC.gov代币安全港提案2.0](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484100&idx=2&sn=34ecbf7ecfa2e32646d69026c550c555&chksm=c1d80311f6af8a0726e84cf990c874002fead7a5f6f3cedd45a216064a4f7ae80185a1356172&scene=21#wechat_redirect)

[深度回顾币安智能链BSC Grant HackerLink第一期](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484046&idx=1&sn=72f298e4d41833d6f39340deed5bf424&chksm=c1d8035bf6af8a4de7934291b2f6cff23bd0f808b57d65ccc177266bdf7649516e103cf35cbe&scene=21#wechat_redirect)

[Futarchy | 价值投票，对赌信仰，用钱说话，口说无凭](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484004&idx=1&sn=433b36bc5b077011f5abdd8b83c802b2&chksm=c1d803b1f6af8aa74094f3c2d14ca2b9d22d807a5fdc4374cbe6f5f55b8e33d585d61604f07e&scene=21#wechat_redirect)

[平行世界｜DeFi无缝集成全球最性感资产—BTC，特斯拉和茅台](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483954&idx=1&sn=d0a5a470a969e9aa9d9f6a6b2bb89232&chksm=c1d803e7f6af8af1574df947cb8be6710937f0a5f30978c255acf81ec02b989b86d184a2e205&scene=21#wechat_redirect)

[「激进市场」和二次方投票 | 用市场本身去监管市场](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483861&idx=1&sn=4e8b5b58a53a942df10fd7e38147ae61&chksm=c1d80000f6af8916f92328a4dc051a92c6836fe6b35bdd762dcb002e944d7663a94b63254e59&scene=21#wechat_redirect)





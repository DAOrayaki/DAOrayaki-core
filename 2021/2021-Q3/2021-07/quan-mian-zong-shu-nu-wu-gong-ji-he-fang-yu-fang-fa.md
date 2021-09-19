

全面综述：女巫攻击和防御方法
==============




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



21 Jul 2021
• 39 min read






![全面综述：女巫攻击和防御方法](/content/images/size/w2000/2021/07/1.jpg)



**DAOrayaki DAO研究奖金池：**

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee /7 通过

赏金总量：170 USDC

研究种类：DAO, Social networks, Sybil defenses, Survey

原文作者:  Aziz Mohaisen, Joongheon Kim

贡献者： Natalie, DAOctor @DAOrayaki

原文: The Sybil Attacks and Defenses: A Survey

![](http://daorayaki.org/content/images/2021/07/----_20210426113809-10.png)### 摘要

本文，主要梳理了女巫攻击及其防御进展。从现有的方法中，我们确定了三种主要抵御攻击的方式：可信认证、资源测试和社交网络。通过可信认证防御攻击，这是使用可以代替中心化认证实体的密码原语的中心化认证或分布式认证来完成的。 通过资源测试来防御攻击，即可以通过 IP 测试、网络协调、经常性成本以及要求客户回答问题的形式。使用社交网络则是通过结合用作引导安全的社交网络和来自随机游走理论的工具来减轻攻击，这些工具已证明在某些假设下可有效防御攻击。我们分别对三种主要抵御攻击的方法进行梳理和分析，总结优缺点，其中这些缺点提供了几个值得研究的有趣方向和研究问题。

### 引言

点对点（p2p）计算范式比其他传统范式有很多优势。例如，带宽、内存和数据等资源可供其他所有参与用户使用 [1]。从广义上讲，这种范式包括结构化和非结构化系统。结构化叠加（例如 Kademlia [2] 和 Chord [3]）为数据和对等点发现提供确定性机制，而非结构化叠加（例如 Gnutella [4]）在随机图中组织对等点并使用泛洪算法进行对等点和数据发现。大多数流行的点对点系统都缺乏“中央权威”，这使得这种范式能够抵御故障攻击。另一方面，缺乏这种中心化授权会导致许多具有挑战性的安全问题：保护网络系统所需的大多数安全服务都需要一种或另一种中心化授权，使得对等系统无法使用这些服务[5] ]。更糟糕的是，其中许多系统完全去中心化和开放的特性在其他分布式系统中导致了大范围的未知安全威胁，包括女巫攻击 [6]。

女巫攻击在点对点、有线和无线网络环境中是众所周知的。 在其基本形式中，代表攻击者的对等点生成尽可能多的身份，并且表现得好像她是系统中的多个对等点 [6]，旨在干扰系统的正常行为。 攻击者可以生成的身份数量仅取决于攻击者的能力，该能力受限于响应系统中其他对等点并发请求所需的带宽、存储与每个生成的女巫身份相对应的节点的路由信息所需的内存，以及在没有明显延迟的情况下处理并发请求所需的计算资源。 随着硬件的急剧增长（例如，在存储容量和处理方面）以及具有高带宽速率的宽带互联网的广泛传播，即使是在通用硬件上运行的攻击者也可能对大型系统造成重大损害。

女巫攻击出现在很多情况下，同样的，在点对点系统以及其他通用分布式系统和范式中必不可少的我的服务上也是常见的。此类环境包括投票系统、信誉系统、路由、分布式存储等。为了说明这种攻击在现实的系统中是如何工作的，请想象一个建立在点对点覆盖 [7] 上的推荐系统。在这样的系统中，系统的目标是根据其他人的推荐过滤出用户可能感兴趣的信息。在这种情况下，可以通过伪造多个身份 (女巫) 充当多个用户的攻击者可以轻松地在合法用户投票的合法对象上投票。

在任何现实的推荐系统中，通常对对象进行投票的合法用户的数量始终不超过系统总用户的 1%，这几乎是可以保证的 [7]。鉴于此，这种攻击对攻击者很有吸引力，他们是系统中的潜在用户，试图攻击提供高度激励的系统。例如，线上市场eBay，使用客户的推荐来确定其卖家、使用其平台销售商品的人的声誉，因此对于此类卖家进行不当行为以获得更高声誉的行为很有诱惑力。在许多其他情况中也会出现相同的情况，例如内容由用户评级的点对点文件共享行为，以声誉为依据分配带宽的行为，在这一行为中，甚至该声誉用于确定用户分发的内容的好坏。在所有此类示例中，都存在用户行为不端的诱因，而且女巫攻击被证明是此类攻击者实现其目标的强大工具。

为了防御攻击，已经有人尝试了几种防御或缓解的形式来防御或限制攻击的影响。这种攻击可以大致分为两种思想流派：中心化和去中心式（即分布式）防御。在中心化防御 [6, 8, 9, 10] 中，中央权威负责验证系统中每个用户的身份。虽然这种防御在防御攻击方面有些有效，但它对系统做出了某些假设，其中一些假设在点对点的去中心化系统中不容易实现。首先，正如名称和操作描述所表明的那样，此类系统需要中心化权限，出于安全性和功能性原因，许多此类系统可能无法负担得起。此外，即使存在这样的中心化权威，也需要一些与系统中用户相关的凭据，以便将用户的这些凭据与其数字身份相匹配：在许多情况下，获取此类凭据是非常有挑战性的工作。

另一方面，去中心化防御包括但不限于 [11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 7, 21, 22, 23] 中的工作，它们不需要系统中有中心化的权威，并为分散的点对点系统精心设计而成。在其操作的核心，此类防御会权衡系统中用户之间的协作，以接纳或拒绝可能是攻击者的用户。用户的接纳或拒绝基于与用户关联的凭据，如加密分布式防御的情况，或合法诚实用户的网络属性，如使用社交图的女巫防御的情况。 在任何一种解决方案中，防御的最终目标都是以分散的方式模拟中央权威的力量，并使用这种力量来检测女巫和诚实的节点。

防御的另一种分类可能是根据这种防御的运作方式。 因此，以往的工作中，女巫防御可以分为使用可信认证的防御——其中证书通常是为诚实用户生成的，并根据受信任机构的公钥进行验证，产生成本——其中用户受到一些成本的惩罚，从而限制他们的可用资源数量，减少他们的不当行为，以及基于社交网络的女巫防御。

这种防御在它们的假设、所应用的网络类型、提供的保证以及产生的成本方面有很大不同。 为此，本文主要回顾、总结、比较和展示现有的方法中，女巫防御的不足之处。

### 2. 女巫攻击模型和目标

在本节中，详细说明了大多数女巫攻击研究和防御中通常假设的攻击者模型，进一步探讨了攻击者的目标和防御目标。

**2.1 问题陈述和模型**

该问题被表述为系统中的单个用户在系统中具有一种能力，此能力让她像是具有多个分身一般行动。 这对于如此多的应用程序来说是有问题的，因为此类应用程序的正确性取决于同行的行为、他们的数量以及在系统中诚实地参与协作的意愿。 然而，试图偏向系统整体行为的单个攻击者的女巫身份不能满足这样的系统目标。

攻击者的正式特征是她可以在系统中注入的虚假身份的数量。 攻击者的动机是最大化虚假身份的数量。 攻击者生成并注入系统的身份数量的价值和意义取决于应用程序本身，并因应用程序而异。 例如，要攻击一个推荐系统，将系统中 1% 的诚实用户的匹配总和作为假身份就足够了。 因为通常观察到，即使对于该系统中非常受欢迎的对象，也只有 1% 的诚实节点投票支持它，所以这尤其是一个足以使系统的行为产生偏差并超过系统中的诚实节点。也就是说，通过拥有比系统中某个对象投票的诚实节点的确切数量更多的单一身份，女巫攻击者将能够超过诚实节点的投票。

另一方面，在其他系统中，例如用于通信匿名化的混合网络（如 Tor 网络），即使是少量的女巫身份可能会严重破坏系统中的承诺。 从理论上讲，电路上两个节点的妥协足以识别这种混合网络上通信的发送方和接收方[24]。 另一方面，网络中足够多的身份的妥协将使攻击者能够监控任意数量的电路。身份数量本身很重要的其他应用程序包括对文件共享系统的攻击 [25] ，这样的例子有很多。

![](http://daorayaki.org/content/images/2021/07/image-218.png)图一 在P2P叠加环境中几种不同的女巫防御的方式

C/CA 代表中心化的认证机构

D/C 代表去中心化的加密原语

T/D  代表可信设备认证

IP/T  代表IP检测

R/C 代表基于成本循环的检测

S/G 代表基于社交图谱的防御方式

**2·2 女巫防御的目标和成功的标准**

女巫防御的最终目标是通过在覆盖网络中侦查并且孤立女巫身份，或者那些对等地能够产生这些女巫身份的节点，来消除女巫攻击。但是，这一终极目标并不总是能够实现，因为大多数防御，除了基于中心化可信认证的方案之外，大多数防御在其检测机制中都有误报和漏报的可能性，可能会容忍某些女巫节点，同时错误地报告其他诚实的节点，就像我们在假阳性和假阴性报错中看到的那样。假阳性报告指女巫节点被报告为诚实节点。另一方面，假阴性诚实节点被报告为女巫节点。防御机制的现实和实际可实现的目标是尽可能地减少假阴性率。

**2.3 女巫防御的深度**

除了第 1 节所示将女巫防御分为中心化和去中心化防御的广泛分类之外，本文调查的女巫防御方式还包括两大类技术：可信认证和资源测试类别，如图 1 所示。在可信认证的列表中，我们梳理了使用中心化认证机构、去中心化加密原语或可信设备的相关工作。

### 3. 使用可信认证

可信认证方法可以说是当下最流行的方法之一，因为 Douceur [6] 已经证明它具有消除 Sybil 攻击的潜力 [26]。 在这种方法的传统形式中，中心化授权 (CA) 用于通过将这些身份与预先分配的凭据进行匹配来确保分配给每个对等方的身份是唯一且合法的。这些凭证可能包括加密密钥、通常由一次性密码生成器 (OTP) 生成的同步随机字符串或由中心化认证颁发的数字证书。

虽然上述传统形式的中心化证书颁发机构在文献中有明确定义，但已经通过应用适用于分布式多方模型的加密原语来定义分布式证书方案，这些模型使假定诚实的对等方之间能够协作以证明加入覆盖的其他对等方.

**3.1 中心化认证机构**

中心化可信认证可能是唯一可以消除女巫攻击的方法 [6]。 在 P2P 覆盖的环境中，已经有一些关于使用中心化证书颁发机构进行凭证生成、分配和验证的工作。 例如，使用第 5 节中解释的社交图并利用公钥密码学作为构建块的研究，假定用户公钥的真实性通过在离线阶段通过中心化授权分配给用户的证书 [19]。 利用基于 CCA 的方法的其他方案示例包括 [8]、[9]、[6] 和 [10] 中的工作。

**3.2 加密原语**

最近，已经涌现了一些关于加密原语的工作 [11, 12, 13, 14, 15]。这些原语旨在提供用于验证对等点的基础设施，以便通过仅让合法对等点参与覆盖来使女巫攻击更难发生。通常，这些工作试图以去中心化方式利用公钥基础设施 (PKI) 并使用阈值加密成分（例如，秘密共享和阈值签名），以确保所谓的诚实用户之间的协作，以验证加入覆盖其上的对等方的操作时间。有趣的是，明确陈述的动机超出了其中一些原语（例如，[11, 12, 13, 14]），这是因为文献中的许多非加密协议都假设存在用于覆盖合法用户的认证系统（例如 SybilGuard 和 SybilLimit）。因此，加密方法旨在确保此类协议的成功运行。

**3.3 可信设备**

与可信认证的想法类似，一些研究与实践，建议使用可信设备或可信模块来存储先前由中心化机构分配给用户的证书、密钥或身份验证字符串。 这种设备由于其潜在的高价而基本上很难获得，因此可用于限制女巫攻击者的机会。 在[27]和[28]中提出了这种机制的例子，尽管后来的工作是在无线传感器网络上。 理论上，当攻击者意图获取尽可能多的女巫身份时，这些防御措施可能会奏效。 然而，在匿名（例如 Tor）和推荐系统等情况下，考虑到较少的女巫身份就可能会造成很大的危害，所以这些防御措施已经过时了。

### 4. 资源测试

除了用于防御女巫攻击的资源测试方法之外，基本思想是检查与假定不同用户相关联的一组身份是否拥有与身份数量匹配的足够资源。这些资源可能包括计算能力、带宽、内存、IP 地址，甚至信任凭证。尽管 Douceur 证明了资源测试的想法是无效的 [6]，但一些研究人员认为它是一种最低限度的防御。也就是说，该方法不能完全消除攻击，但是会使其女巫攻击更难发生。

理论上，此类防御中的大多数方案将女巫身份的数量限制为比没有防御的情况下的数量少。然而，在实践中，即使是更少数量的女巫身份也足以威胁许多系统的可用性和安全性。例如，如前所述，匿名系统（如 Tor）中的匿名性取决于每个电路的两个节点。此外，在线声誉系统中有 1% 的虚假身份就足以投票给合法节点。

**4.1 IP 测试**

通用测试方案包括测试对等方的 IP 地址，试图确定他们的位置并将其与他们的活动相匹配。特别是，如果从同一特定地理区域产生大量活动，则其中一些活动很可能是由于女巫身份。此外，此类作品中的假设是获取不同地理区域的 IP 地址，但这并不便宜。例如，弗里德曼等人 [29] 介绍了 Tarzan，其中根据节点在特定自治系统中的地理位置测试其 IP 地址。Cornelli 等人在 [30] 和 [30] 中介绍了类似的结果。

这些工作的主要假设是 IP 地址很难在广泛的地理区域中获得。然而，最近有迹象表明存在巨大的僵尸网络 [31]，受感染的主机由单个管理实体控制并驻留在不同的自治系统中，可以肯定的是，这种防御机制是无用的。

**4.2 成本循环**

一些研究及实践，建议将经常性成本作为防御女巫攻击的一种方法。 特别是，计算难题 [16, 32] 和图灵测试（例如 CAPTCHA [33]）被建议作为解决方案。 然而，出于同样的原因，IP 测试对控制僵尸网络的攻击者不起作用，这些基于成本的方案也不会起作用。 此外，对于类似 CAPTCHA 的解决方案，已经表明 Sybil 攻击者可能会在控制的站点上发布 CAPTCHA 测试，供用户测试以访问攻击者提供的服务。

此外，某些版本的 CAPTCHA 容易受到某些图像处理攻击 [34]。

### 5. 基于社交图谱的防御

虽然之前针对分布式系统中女巫攻击问题提出的大多数解决方案都有局限性和缺点，但基于社交网络的女巫防御尝试以优雅的方式克服这些问题。首先，基于社交网络的女巫防御大多是解决女巫攻击问题的去中心化解决方案，这意味着这些设计在没有任何中心授权的情况下运行——这是大多数分布式系统中的重要特性。由于随机游走理论，这种去中心化的操作模型更加容易，随机游走理论是这些防御中最常用的成分。其次，这些防御利用社交节点之间社交链接的信任，使诚实节点之间的协作变得可能且容易。第三也是最后一点，这些防御在几项研究中得到了证明，它们能以低成本实用且有效地防御女巫攻击，而且它们现在进一步开发为许多服务的组件，包括分布式哈希表 (DHT)、抗女巫攻击投票，并用于移动网络路由。

尽管它们在设计细节和操作上有很大不同，但所有基于社交网络的女巫防御都有两个共同的假设：算法属性即快速混合属性以及信任。 首先，这些防御基于社交图的“快速混合”属性。 非正式地，社交图的快速混合属性意味着此类图中的“诚实”节点很好地啮合，并且诚实区域不包含稀疏切割——一种将两个大型诚实节点子集与一些社交网络连接起来的切割。为简单起见，社交图的快速混合特性意味着来自社交图中任意节点的随机游走将非常接近在几步后该图上定义的马尔可夫链 (MC) 的平稳分布。 在百万节点的网络中，建议这样的步数为 10 到 15 步。

这种防御脉络的第二个共同假设是信任。 特别是，所有这些防御都假定在底层社交图中具有良好的信任值，例如，通过节点之间的面对面交互所表明的。 为了推断任意多个攻击者的社交链接渗透社交网络的难度，这个特定的假设是必要的。 虽然用于正确识别社交图中“诚实”节点的女巫防御的操作是由快速混合假设保证的，并且使用这种算法属性的相应方案的构建，识别 女巫节点的能力仅在假设以下条件下得到保证攻击者，或攻击者的集体，控制着自己与社交图中其他诚实节点之间的一些链接（这种链接称为攻击边）。

下面我们梳理了一些被广泛引用和关注的基于社交网络的女巫防御的方法。

**5.1 Sybil Guard**

SybilGuard 的设计，归功于 Yu 等人[19, 20]，它使用信任拥有社交网络的快速混合特性来检测女巫节点。从技术上讲，SybilGuard 包括两个阶段：初始化阶段和在线检测阶段。在初始化阶段，每个节点构建它的路由表，作为其相邻节点的随机排列，用于输入和输出边对。接下来，每个节点启动一个长度为 w = O (根号n log n) 的随机游走，并按照使用随机排列构建的路由表将其传播到其相邻节点。随机游走路径上的每个节点都会注册随机游走发起者的见证人，然后当该节点成为嫌疑节点时充当该节点的见证者。此外，利用随机游走的回溯性，随机游走的每个发起者都会收到“见证人”列表（即注册发起者公钥并位于发起者随机游走构建的路径上的节点） .

在线上阶段，验证者确定嫌疑人是否诚实，如下所示。 首先，嫌疑人将其随机路由上的“证人”的地址发送给验证者。 因此，验证者将见证人列表与其验证者路由列表进行比较。 如果两个集合之间没有交集（一个非常有可能发生的事件），验证者将中止并拒绝嫌疑人。否则，验证者将继续，要求比较两个集合之间的交集上的节点来验证嫌疑人是否有用它们注册的公钥。如果嫌疑人被交叉节点验证，则验证者接受嫌疑人或将其标记为女巫节点。

**5.2 Sybil Limit**

与使用单个长随机游走的 SybilGuard 不同，SybilLimit 建议使用多个较短的随机游走。此外，与 SybilGuard（验证者和嫌疑人的公钥注册在社交图中的节点上不同，SybilLimit [18] 建议在社交图中的边上注册此类密钥。 SybilLimit 由初始化阶段和在线验证阶段组成。在初始化阶段，每个节点使用 SybilGuard 中描述的相同方法构建其路由表，并执行 r = O (根号 n) 的随机游走，每次长度为 w = O (log n) 其中 O (log n) 是混合时间社交图的 10 到 15 个社交图 ，理论上假设足以从非常接近统计分布的分布中采样节点。与 SybilGuard 不同，随机路由路径上的所有节点都用于注册随机游走发起者的公钥，r 次随机游走中每次游走的最后一条边用于注册该发起者节点的公钥（每个这样的边称为尾部）。特别地，游走发起者的公钥注册在随机游走到达的最后一条边下的最后一个节点上。同样利用随机路由的回溯性，注册发起者节点（可以是嫌疑人或验证者）公钥的见证人将他们的身份返回给该节点。社交图中的每个节点都执行相同的过程，并且每个发起注册随机游走的节点都收集一组见证人（或验证节点）。

在线上阶段，SybilLimit也与 SybilGuard 相同，嫌疑人将证人的标识符和地址发送到验证者节点，该节点将比较嫌疑人列表中的证人，试图找到冲突。 如果在验证者端的两个集合中发生冲突，验证者会要求两个集合中具有共同身份的见证人验证嫌疑人的身份，并根据此过程的结果决定是接受还是拒绝嫌疑人。如果两者之间没有交集（这样的事发生的可能性很小）验证者通过将嫌疑人标记为攻击者来中止并拒绝嫌疑人。

用于推理 SybilLimit 的可证明保证的主要成分与 Sybil Guard 中的相同。特别地，假设随机游走长度 w 是社交图的混合时间，那么在这种随机游走中选择的最后一个节点是根据平稳分布的。

此外，随机游走中的最后一条边是从社交图中的边中“几乎”均匀随机选择的。此外，假设 r = O（根号 n），如果正确选择了隐藏常量 r0（其中 r = r0 ×根号 n），则验证者和嫌疑人的采样边缘之间的交集将以压倒性的概率存在。作者将这种条件称为“交集”条件，用于保证诚实区域中节点随机游走的高概率交集。与 SybilGuard 一样，假设有 g 个攻击者边缘，则允许攻击者在最多 gwr = O (g ×根号 n× log n) 尾（称为污染尾）上注册其女巫身份的公钥。在这种情况下，每个附加边都会引入额外的 O (log n) 女巫身份（假设攻击者通过在每个可能的受污染尾部注册不同 Sybil 身份的不同公钥来使用最佳攻击策略）。

SybilLimit 的安全性也很大程度上依赖于 w。 由于没有估计参数的确切值的机制，因此低估或高估这些参数都是有问题的，如上所示。 SybilLimit 还提供了一种用于估计该参数的“基准测试技术”，该技术也不对参数估计的质量提供任何可证明的保证。 最后，只要 g = o (n / log n)，Sybil Limit 就可以保证每个攻击边缘引入的女巫身份的数量。 请注意，SybilGuard 和 SybilLimit 都不需要对其运营的社交网络有任何全局了解，并且可以以完全去中心化的方式实施。

**5.3 Sybil Infer**

SybilInfer 使用在随机游走（称为轨迹）上定义的概率模型来推断生成此类轨迹的一组节点 X 的真实程度。 SybilInfer 中的基本假设是每个节点都拥有社交网络的全局视图和知识，网络是快速混合的，发起 SybilInfer 的节点是一个诚实节点。从技术上讲，SybilInfer 试图最终将图中的不同节点标记为诚实节点或女巫节点。在 SybilInfer 中，n 个节点的网络中的每个节点执行 s 次行走，因此通用迹中的行走总数为 s × n。这些迹中的每个痕迹由第一个节点（随机游走的发起者）和随机游走中的最后一个节点（即尾部）构成。与 SybilGuard 和 SybilLimit 中使用的统一（超过节点度）转移概率不同，SybilInfer 定义了节点上统一的转移矩阵，从而惩罚具有更高度的节点。 SybilInfer 操作的最终目标是计算概率 P (X = Honest | T)；也就是说，计算给定轨迹 T 的一组节点 X 是诚实的概率。这个概率是使用贝叶斯定理计算的。

SybilInfer 通过技术手段对诚实配置进行采样，该配置最初用于从跟踪中确定一组节点的诚实性。 这个采样是使用 Metropolis-Hasting 算法进行的，它首先考虑一个集合 X0 并通过删除或添加节点到集合中一次修改该集合：在每次，并且有概率从 X¯0 中填充一个新节点 x被添加到 X0 使 X ′ = X0 [x 或 X0 中的节点以概率 premove 被删除。 该过程执行 n× log n 轮以获得独立于 X0 的良好样本。

**5.4 Sum Up**

不像 SybilGuard 和 SybilLimit 是通用的节点准入问题，并且在不需要单个节点携带有关社交图的全局信息的意义上去中心化，以及用于推断节点诚实度的 Sybil-Infer，SumUp [35] 试图在投票聚合的背景下解决女巫攻击问题。在这种情况下，一个称为投票收集器的节点希望以抗女巫的方式从网络中的其他节点收集投票。这就是，在给定数量的对象投票中，投票收集者希望增加诚实节点接受的投票比例，减少攻击者通过其攻击边缘投出的接受投票，并在攻击者多次反复行为不当时识别攻击者。在 SumUp 的核心是，链接容量分配机制用于自适应地为信任拥有社交图中的链接分配容量，并限制从投票者一侧传播到选票收集器的选票数量。 SumUp 的自适应投票流机制使用了传统在线投票系统的两个观察结果：系统中的少数用户对单个对象进行投票，并且——如果这种投票系统是在社交图之上实现的——拥堵仅出现在靠近选票收集器的链上。因此，SumUp 建议根据它们与投票收集器的距离（根据使用广度优先搜索算法计算的某些级别）在社交图中的不同链接上分发大量票证。

该技术的一个明显吸引力在于其高计算要求：典型算法（例如 Ford-fulkerson 算法）的运行时间将需要一个操作边数的顺序，以收集单个选民的投票。它的作者进一步提出了一种启发式方法，它仅使用图直径步数的顺序，其中每个节点贪婪地选择更高级别的节点，通过该节点使用非零容量连接并传播投票，直到达到投票收集器。 在任何时间，考虑到贪婪步骤可能不会导致非零容量，每个节点都被允许探索其他节点以寻找相同或更低级别的路径。

**5.5 GateKeeper**

GateKeeper [21] 借用了 SumUp 和 SybilLimit 的工具来实现高效操作。尤其是它试图通过合并 SumUp 的票证分发组件来提高 SybilLimit 的性能。不像在 SumUp 中，节点通过从投票者到收集者的非零路径被接纳，如前所述，GateKeeper 只考虑 SumUp 的“票证分配”阶段，其中票证被准入控制器用于接纳节点。此类票证以与 SumUp 中相同的方式从控制器传播到所有节点。但是，为了限制攻击者获得更多门票的机会并降低其整体优势，GateKeeper 中的控制器随机选择 m 个不同的随机节点；这些节点被称为“有利节点”，当且仅当可疑节点从不同的有利位置收到 fadmitm 票证（其中 fadmit 是随机选择的有利位置的分数；在 GateKeeper 中使用 0.2）时，它才会被允许。因此，一旦一个节点被这个有利位置的一小部分允许，它就会被允许。为了防止双花攻击，Gate Keeper 建议使用门票的路径的加密签名链（传播到控制器）。

**5.6 其他基于社交网络的 DHT**

SPROUT [36] 是另一种 DHT 路由协议，它使用具有信任的社交图的社交链接将信息路由到在社交网络上操作的用户。 SPROUT 实际上建立在 Chord [3] 之上，并在 Chord 中向任何给定节点的社交网络中的其他用户添加了额外的链接（路由表条目），这些用户随时在线。 通过这样做，SPROUT 声称可以提高 Chord 本身的可靠性和负载分布。

Whanau 最初在 [23] 中提出，其中 [22] 中的工作包括对性能和安全性的进一步分析和证明以及端到端保证的实施和演示。

在 [1] 中，作者使用引导图——显示了DHT 中引入关系的树，以防御 女巫攻击。通过修改感兴趣的 DHT Chord 的操作，使每个节点返回它知道的所有节点的地址（包括引入点），作者设计了几种用于减少女巫攻击影响的策略。与使用 Chord 上的接近度作为路由（查询）度量的原始 Chord 不同，该解决方案考虑了多种路由策略，包括多样性、混合和 zig-zag。作者通过实验表明，当此类策略在女巫攻击下运行时，它可用于更有效地执行抗女巫的DHT 查找，而且它的查询次数将少于普通 Chord 设计所需的查询数量。

MobID [37] 的设计是一种基于社交网络的女巫防御，声称可以为移动环境提供强大的防御，而现有的防御主要是为点对点网络设计的，并且基于随机游走理论。此外，MobID 使用介数（社交图中的一种图论度量）来确定节点的优度，以防御女巫攻击。然而，这项工作似乎没有提供任何可证明的保证。各种方案与文献中的其他方案之间的比较见表 1 和表 2。

### 6. 结论

P2P 覆盖网络极易受到女巫攻击，并且由于 P2P 覆盖的性质，解决女巫攻击这一问题比以往都难：它不鼓励安全实施所需的中心化认证机构，而且甚至有时中心化认证机构在 P2P 覆盖设计中不存在。 本文，主要梳理了用于防御 P2P 覆盖中的女巫攻击的不同方法。 并对不同防御的假设、特征和缺点进行比较。

### 参考文献：

[1] George Danezis, Chris Lesniewski-laas, M. Frans Kaashoek, and Ross Anderson. Sybil-resistant dht

routing. In In ESORICS, Lecture Notes in Computer Science, pages 305–318, Berlin, Heidelberg, 2005. Springer.

[2] Petar Maymounkov and David Mazi`eres. Kademlia: A peer-to-peer information system based on the xor metric. In Peter Druschel, M. Frans Kaashoek, and Antony I. T. Rowstron, editors, IPTPS, Lecture Notes in Computer Science, pages 53–65, Berlin, Heidelberg, 2002. Springer.

[3] Ion Stoica, Robert Morris, David R. Karger, M. Frans Kaashoek, and Hari Balakrishnan. Chord: A scalable peer-to-peer lookup service for internet applications. In SIGCOMM, pages 149–160, New York, NY, USA, 2001. ACM.

[4] Yong Wang, Xiao chun Yun, and Yifei Li. Analyzing the characteristics of gnutella overlays. In ITNG, pages 1095–1100, Washington, DC, USA, 2007. IEEE Computer Society.

[5] Vivek Pathak and Liviu Iftode. Byzantine fault tolerant public key authentication in peer-to-peer

systems. Computer Networks, 50(4):579–596, 2006.

[6] John Douceur and Judith S. Donath. The sybil attack. In IPDPS, pages 251–260, Washington, DC, USA, 2002. IEEE.

[7] Haifeng Yu, Chenwei Shi, Michael Kaminsky, Phillip B. Gibbons, and Feng Xiao. Dsybil: Optimal sybil-resistance for recommendation systems. In IEEE Symposium on Security and Privacy, pages 283–298, Washington, DC, USA, May 2009. IEEE Computer Society.

[8] Miguel Castro, Peter Druschel, Ayalvadi J. Ganesh, Antony I. T. Rowstron, and Dan S. Wallach. Secure routing for structured peer-to-peer overlay networks. In OSDI, Berkeley, CA, USA, 2002. USENIX Association.

[9] Atul Adya, William J. Bolosky, Miguel Castro, Gerald Cermak, Ronnie Chaiken, John R. Douceur, Jon Howell, Jacob R. Lorch, Marvin Theimer, and Roger Wattenhofer. Farsite: Federated, available, and reliable storage for an incompletely trusted environment. In OSDI, New York, NY, USA, 2002. USENIX Association.

[10] Jonathan Ledlie and Margo I. Seltzer. Distributed, secure load balancing with skew, heterogeneity and churn. In INFOCOM, pages 1419–1430, Washington, DC, USA, 2005. IEEE.

[11] Fran¸cois Lesueur, Ludovic M´e, and Val´erie Viet Triem Tong. An efficient distributed pki for structured p2p networks. In Proceeding of P2P, pages 1–10, Washington, DC, USA, 2009. IEEE

Computer Society.

[12] Fran¸cois Lesueur, Ludovic M´e, and Val´erie Viet Triem Tong. A distributed certification system for structured p2p networks. In David Hausheer and J¨urgen Sch¨onw¨alder, editors, AIMS, volume 5127 of Lecture Notes in Computer Science, pages 40–52, Berlin, Heidelberg, 2008. Springer.

[13] Fran¸cois Lesueur, Ludovic M´e, and Val´erie Viet Triem Tong. A sybil-resistant admission control coupling sybilguard with distributed certification. In WETICE, pages 105–110, Washington, DC, USA, 2008. IEEE Computer Society.

[14] Fran¸cois Lesueur, Ludovic M´e, and Val´erie Viet Triem Tong. A sybilproof distributed identity

management for p2p networks. In ISCC, pages 246–253, Washington, DC, USA, 2008. IEEE.

[15] Agapios Avramidis, Panayiotis Kotzanikolaou, and Christos Douligeris. Chord-pki: Embedding a

public key infrastructure into the chord overlay network. In Javier Lopez, Pierangela Samarati,

and Josep L. Ferrer, editors, EuroPKI, volume 4582 of Lecture Notes in Computer Science, pages 354–361, Berlin, Heidelberg, 2007. Springer.

[16] Nikita Borisov. Computational puzzles as sybil defenses. In Alberto Montresor, Adam Wierzbicki,

and Nahid Shahmehri, editors, Peer-to-Peer Computing, pages 171–176, Washington, DC,

USA, 2006. IEEE Computer Society.

[17] Haifeng Yu, Phillip B. Gibbons, and Michael Kaminsky. Toward an optimal social network

defense against sybil attacks. In Indranil Gupta and Roger Wattenhofer, editors, PODC, pages

376–377. ACM, 2007.

[18] Haifeng Yu, Phillip B. Gibbons, Michael Kaminsky, and Feng Xiao. Sybillimit: A near-optimal social network defense against sybil attacks. In IEEE Symposium on Security and Privacy, pages 3–17, Washington, DC, USA, 2008. IEEE Computer Society.

[19] Haifeng Yu, Michael Kaminsky, Phillip B. Gibbons, and Abraham Flaxman. SybilGuard: defending against sybil attacks via social networks. In Luigi Rizzo, Thomas E. Anderson, and Nick McKeown, editors, SIGCOMM, pages 267–278, New York, NY, USA, 2006. ACM.

[20] Haifeng Yu, Michael Kaminsky, Phillip B. Gibbons, and Abraham D. Flaxman. Sybilguard: defending against sybil attacks via social networks. IEEE/ACM Trans. Netw., 16(3):576–589, 2008.

[21] Nguyen Tran, Jinyang Li, Lakshminarayanan Subramanian, and Sherman S.M. Chow. Optimal sybil-resilient node admission control. In The 30th IEEE International Conference on Computer Communications (INFOCOM 2011), Shanghai, P.R. China, 2011. IEEE.

[22] Chris Lesniewski-Lass and M. Frans Kaashoek. Wh¯anau: A sybil-proof distributed hash table. In

7th USENIX Symposium on Network Design andImplementation, pages 3–17, Berkeley, CA, USA,

2010. USENIX Association.

[23] C. Lesniewski-Laas. A Sybil-proof one-hop DHT. In Proceedings of the 1st workshop on Social network systems, pages 19–24, New York, NY, USA, 2008. ACM.

[24] Paul F. Syverson, David M. Goldschlag, and Michael G. Reed. Anonymous connections and

onion routing. In IEEE Symposium on Security and Privacy, pages 44–54, Washington, DC, USA,

1997. IEEE Computer Society.

[25] Peng Wang, James Tyra, Eric Chan-tin, Tyson Malchow, Denis Foo Kune, and Yongdae Kim.

Attacking the kad network, 2009.

[26] B.N. Levine, C. Shields, and N.B. Margolin. A survey of solutions to the sybil attack. Technical

report, University of Massachusetts Amherst, Amherst, MA, 2006.

[27] Rodrigo Rodrigues, Barbara Liskov, and Liuba Shrira. The design of a robust peer-to-peer system. In 10th ACM SIGOPS European Workshop, pages 1–10, New York, NY, USA, 2002. ACM.

[28] James Newsome, Elaine Shi, Dawn Song, and Adrian Perrig. The sybil attack in sensor networks: analysis & defenses. In IPSN ’04: Proceedings of the 3rd international symposium on Information processing in sensor networks, pages 259–268, New York, NY, USA, 2004. ACM.

[29] Michael J. Freedman and Robert Morris. Tarzan: a peer-to-peer anonymizing network layer. In

Vijayalakshmi Atluri, editor, ACM Conference on Computer and Communications Security, pages 193–206, Washington, DC, USA, 2002. ACM.

[30] Fabrizio Cornelli, Ernesto Damiani, Sabrina De Capitani di Vimercati, Stefano Paraboschi, and Pierangela Samarati. Choosing reputable servents in a p2p network. In WWW, pages 376–386, New York, NY, USA, 2002. ACM.

[31] Brent ByungHoon Kang, Eric Chan-Tin, Christopher P. Lee, James Tyra, Hun Jeong Kang, Chris Nunnery, Zachariah Wadler, Greg Sinclair, Nicholas Hopper, David Dagon, and Yongdae Kim. Towards complete node enumeration in a peer-to-peer botnet. In Wanqing Li, Willy Susilo, Udaya Kiran Tupakula, Reihaneh Safavi-Naini, and Vijay Varadharajan, editors, ASIACCS, pages 23–34, New York, NY, USA, 2009. ACM.

[32] Frank Li, Prateek Mittal, Matthew Caesar, and Nikita Borisov. Sybilcontrol: practical sybil

defense with computational puzzles. In Proceedings of the seventh ACM workshop on Scalable trusted computing, pages 67–78. ACM, 2012.

[33] Luis von Ahn, Manuel Blum, Nicholas J. Hopper and John Langford. Captcha: Using hard ai problems for security. In Eli Biham, editor, EUROCRYPT, volume 2656 of Lecture Notes in Computer Science, pages 294–311, Berlin, Heidelberg, 2003. Springer.

[34] Jeff Yan and Ahmad Salah El Ahmad. Breaking visual captchas with naive pattern recognition algorithms. In ACSAC, pages 279–291, Washington, DC, USA, 2007. IEEE Computer Society.

[35] N. Tran, B. Min, J. Li, and L. Subramanian. Sybil-resilient online content voting. In NSDI, Berkeley, CA, USA, 2009. USENIX.

[36] Sergio Marti, Prasanna Ganesan, and Hector Garcia-Molina. Dht routing using social links. In IPTPS, pages 100–111, Washington, DC, USA, 2004. IEEE.

[37] Daniele Quercia and Stephen Hailes. Sybil attacks against mobile users: friends and foes to the

rescue. In INFOCOM’10: Proceedings of the 29th conference on Information communications, pages

336–340, Piscataway, NJ, USA, 2010. IEEE Press.

[38] Abedelaziz Mohaisen, Aaram Yun, and Yongdae Kim. Measuring the mixing time of social graphs. In Proceedings of the 10th annual conference on Internet measurement, IMC ’10, pages 383–389,

New York, NY, USA, 2010. ACM.

[39] Bimal Viswanath, Ansley Post, Krishna P. Gummadi, and Alan Mislove. An analysis of social network-based sybil defenses. In SIGCOMM, New York, NY, USA, August 2010. ACM.

[40] George Danezis and Prateek Mittal. SybilInfer: Detecting sybil nodes using social networks. In

The 16th Annual Network & Distributed System Security Conference, Lecture Notes in Computer Science, Berlin, Heidelberg, 2009. Springer-Verlag.

[41] Abedelaziz Mohaisen, Huy Tran, Nicholas Hopper, and Yongdae Kim. Understanding social networks properties for trustworthy computing. In ICDCS Workshops, pages 154–159. IEEE, 2011.

[42] Abedelaziz Mohaisen and Scott Hollenbeck. Improving social network-based sybil defenses by augmenting social graphs. In WISA, 2013.

[43] Abedelaziz Mohaisen, Nicholas Hopper, and Yongdae Kim. Keep your friends close: Incorporating trust into social network-based sybil defenses. In INFOCOM, pages 1943–1951. IEEE, 2011.

[44] Haifeng Yu. Sybil defenses via social networks: a tutorial and survey. ACM SIGACT News, 42(3):80–101, 2011.



---

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）  
  
详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)

历史文章：

[DAOrayaki｜DAO 通过财政多元化为下一个加密冬天做准备](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484808&idx=1&sn=f089e891fe0c8d0ba6a0c5cf208b9c9b&chksm=c1d8045df6af8d4b37cd79d4efb40d2e0c71d4e2aeb5f322615eecbc06664f452c927a75ae90&scene=21#wechat_redirect)

[DAOrayaki ｜依靠钱包追踪鲸鱼活动](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484965&idx=1&sn=a1b3b144d0df863e8b1e68a4eaf86f0b&chksm=c1d807f0f6af8ee6c0c5992cd3317714cbff02554e790181233d627bdc8d58ea493bc86988cb&scene=21#wechat_redirect)

[DAOrayaki ｜加密货币里的吸血鬼攻击](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484939&idx=1&sn=3c76bbaef8b1c1637530e1a16f8272a2&chksm=c1d807def6af8ec85bdaf2d7c3cbc2e11e475906d933f4da9f484b713521994366db32383183&scene=21#wechat_redirect)

[DAOrayaki｜价格与预言机](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484807&idx=1&sn=273c664de6afa9c263f4be0c595d080a&chksm=c1d80452f6af8d44c5c12a9b33313cc3d5df3128d06921ae61c90fd6f494817a91beb29d5508&scene=21#wechat_redirect)

[DAOrayaki｜去中心化自治组织（DAO）行业发展月报（2021.6）](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484806&idx=1&sn=28088c05ecf1c26dcd94ccdc8347be23&chksm=c1d80453f6af8d45040b58692b61c2e2d9bdaf1894d51382ea9042e66fe134f7173c2c5687cd&scene=21#wechat_redirect)

[加密技术的全面论述—开放金融系统](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484742&idx=1&sn=711607523b7112e1f6dd5dcd855894cf&chksm=c1d80493f6af8d8558574439a91347b54e0a9410cf6a711ed9e75bf2e68543f2d1df8970e640&scene=21#wechat_redirect)

[DAOrayaki | 去中心化仲裁：Kleros、Aragon、Jur](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484741&idx=1&sn=6dd674ebc05296fa3fe21acada6c1d5f&chksm=c1d80490f6af8d86f57987537135f059d8b95be2267c7f5fb0a1f4af297eea6cdf95daacfe16&scene=21#wechat_redirect)

[D2D：面向去中心化的谈判协议](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484740&idx=1&sn=ab336ebc7b925d01e547c14f18f5a8df&chksm=c1d80491f6af8d874266b2b365b0e5847fa5ed12f064b9ac0eb5c8c8a72628afb1b0ccf822df&scene=21#wechat_redirect)

[DAOrayaki解读｜价格敞口和投票权](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484712&idx=1&sn=674e8305b9899f73343eae5d68be6a99&chksm=c1d804fdf6af8deb14b0fb4ae8debb6abef6e96ec0a638768f06da475e097a97cf3f00ea5c8f&scene=21#wechat_redirect)

[Muse Museum率先加入DAOrayaki Funders MolochDAO并开展联合研究](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484739&idx=1&sn=7a15f813ff8ca419221bcba9b14cf2f8&chksm=c1d80496f6af8d8038bc222f8ce4eecf9a4ddf47477fdc12233797e48495884334a23322cce5&scene=21#wechat_redirect)

[D2D：面向去中心化的谈判协议](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484740&idx=1&sn=ab336ebc7b925d01e547c14f18f5a8df&chksm=c1d80491f6af8d874266b2b365b0e5847fa5ed12f064b9ac0eb5c8c8a72628afb1b0ccf822df&scene=21#wechat_redirect)

[DAOrayaki | 去中心化仲裁：Kleros、Aragon、Jur](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484741&idx=1&sn=6dd674ebc05296fa3fe21acada6c1d5f&chksm=c1d80490f6af8d86f57987537135f059d8b95be2267c7f5fb0a1f4af297eea6cdf95daacfe16&scene=21#wechat_redirect)

[DAOrayaki解读｜8步实现去中心化](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484713&idx=1&sn=3b76441db3d940c4ea33fcc7e440e276&chksm=c1d804fcf6af8dea80f1e3bec50b06915e603a5927dac9e255ba3e61f4002c4df27191efb835&scene=21#wechat_redirect)[$WORK 奖励、利益相关者经济学和就业共享的代币化](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484579&idx=1&sn=e52f69e1e926eed1f2d895ad3c23df47&chksm=c1d80576f6af8c60a9f3f0e21d713a61e55ffbad904f0701634aba2f28b9ae746bc2ddd5f046&scene=21#wechat_redirect)

[DAOrayaki解读｜价格敞口和投票权](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484712&idx=1&sn=674e8305b9899f73343eae5d68be6a99&chksm=c1d804fdf6af8deb14b0fb4ae8debb6abef6e96ec0a638768f06da475e097a97cf3f00ea5c8f&scene=21#wechat_redirect)

[DAOrayaki解读｜DAO与全球经济秩序-新自由主义的黄昏（一）](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484684&idx=1&sn=f38e7f8f884f4c6b997506c3c49ca688&chksm=c1d804d9f6af8dcf7e2b8aa629846b60b783d410057e50797ee9b697434f7183d40f04b5f461&scene=21#wechat_redirect)

[DAOrayaki 解读|奥斯特罗姆：公共事务的治理之道](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484580&idx=1&sn=1d1c5412ab24b34242912813041c138a&chksm=c1d80571f6af8c67fbfac08c52c900562a4328f65c7b7a05d09ba3473704ff22aa7153bbefe0&scene=21#wechat_redirect)[DAO治理中的同构性](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484493&idx=1&sn=4169ed86c19a17a063dc97c9f6b9b87e&chksm=c1d80598f6af8c8e6cac5807f59a01c8e7d062ee3b9806c18b9a5cb139377a7b3c5b55d0dd1d&scene=21#wechat_redirect)





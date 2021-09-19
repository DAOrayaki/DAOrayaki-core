


[DAOs](/tag/daos/)

可选用的DAOs投票机制汇总
==============




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



2 Jun 2021
• 20 min read






![可选用的DAOs投票机制汇总](/content/images/size/w2000/2021/06/640.png)



**DAOrayaki DAO**研究奖金池：

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 4/7 通过

赏金总量：150 USDC

研究种类：DAO, Voting Mechanisms, Quorum Voting, Holographic Consensus, Conviction Voting, Multisig, Lazy Consensus

原文作者:  Eric Arsenault

贡献者：Demo, DAOctor @DAOrayaki

原文: Voting Options in DAOs

![](http://daorayaki.org/content/images/2021/06/----_20210426113809-2.png)本文通过与DAO创建者和构建者的对话，探讨DAO使用的不同投票机制。

一、基于代币的法定人数投票

法定人数投票要求有一定的投票者门槛（投票阈值），以使提案获得通过（例如：60%的法定人数，这意味着需要60%的投票权来投票）。一旦达到这个门槛，拥有更多的票数的决策就会获胜。没有达到法定人数门槛，提案就会失败。

门槛通常基于总票数，尽管有些协议（如复合治理（compound governance））只对赞成提案通过的票数设置了法定门槛（在这种情况下，20%的法定门槛意味着20%的投票权对提案投了赞成票，以使提案被考虑通过）。

使用过这种方法的项目包括Compound、Curve和Kleros（以及其他许多项目）。

这种治理机制已久经沙场，在我们的政治体系中有着悠久的历史，用户体验也比较简洁。

另一方面，纯粹基于代币的投票也存在一些问题。财阀政治并不好，选择“正确的”法定人数要求也很困难。较低的法定人数使得提案能够轻易通过，系统也很容易受到攻击。但太高的法定人数使提案很难通过。若涉及到鲸鱼（掌握巨额代币的持有者），挑战就更大了。基于代币的投票对某些类型的攻击很敏感（比如我们在Maker中看到的flash治理攻击）。基于法定人数的投票还需要成员的大量参与才能通过提案，而这既昂贵又耗时。

以下为来自Curve的Michael的Q&A环节：

1）如何看待基于法定人数的投票在你的DAO中的应用？

基于法定人数的投票对我们来说是有意义的。不过，投票率通常非常低。我们在通过提案时并没有遇到太多挑战（只有1个没有达到30人的法定人数）。让人恼火的是，投票确实会变成一种与鲸鱼博弈的游戏。gas的数量在一定程度上是一个障碍，但我们希望在未来通过元交易（meta transactions）补贴gas。

2）你是否担心与基于法定人数的投票有关的一些风险？(注意：Curve不使用直接的代币投票。他们要求代币持有者锁定代币，而给予的投票权与锁定的代币数量以及锁定的时间成正比，其可以减少攻击向量。）

不担心。因为投票权是基于锁定代币的时间给予代币锁定者的，其他风险我也不太担心，比如无法达到法定人数。

3）如果你能轻易改变这个DAO的投票机制，你会这样做吗？

我真正想拥有的是流民主（liquid democracy），即投票权的委托。

以下为来自Kleros的Clement的Q&A环节：

1）如何看待基于法定人数的投票在你的DAO中的应用？

我讨厌它。我建议项目使用的唯一法定人数百分比是0（即，没有法定人数）。

2）你最不喜欢哪些方面？

它会引致战术性投票（tactical voting）。战术性投票之所以不理想，并不能做出最佳决策，原因有很多。（战术性投票意味着人们可能会被激励隐藏自己的真实偏好，以获得最好的结果。例如，在美国选举中经常有这种例子，即使他们支持一个独立的政党，他们也会投票给民主党或共和党，因为他们的“选票不会算数”）。在法定人数投票中，反对提案的人通常会弃权，而不是投反对票，因为这样更有可能阻止提案通过。

当无法达到法定人数时，基于法定人数的投票还会导致治理锁（governance locks）。它还产生了被迫保守主义（forced conservatism），因为只有极受欢迎的提案才能通过，而简单的提案很难让人们投票。

3）你是否担心与基于法定人数的投票有关的一些风险？

是的，我很担心。治理锁的风险是重大的，可能导致项目终止或不能及时地应对新的环境条件。

4）如果你能轻易改变这个DAO的投票机制，你会这样做吗？

信念投票（conviction voting）很有意思，Moloch许可式可以适合一些DAO。我也很喜欢孔多塞方法（Condorcet method）的投票系统。

以下为来自Compound的匿名者的Q&A环节：

1）如何看待基于法定人数的投票在你的DAO中的应用？

至少在Compound，它似乎起作用了，社区也在不断对其升级。达到法定人数并不是问题，可能是因为有活跃的巨鲸。

2）关于法定人数投票，你最不喜欢的是什么?

作为一种投票机制，代币有一个主要围绕投机形成的市场价格。把投票权从财政方面分离出来会比较好。

复合治理的挑战似乎与社会和激励问题更相关。例如:许多人参与社区是因为他们在意，而不是因为有长期利益。让更多的人与协议的长期方向一致是好的，但让更多的人去关心总体上是很难的。此外，即使Compound是去中心化的，许多人仍然只是接触团队，而不是在社区内工作。这一问题的部分原因可能是缺乏围绕提案和投票的基础设施，以及被人们认为的中心化。

3）如果你能轻易改变这个DAO的投票机制，你会这样做吗？

二次方投票（Quadratic voting）的思路似乎很有趣。可能需要锁定代币以增加投票权。可能还会向“农民”发放归属补偿，以调整长期激励措施。

其他我可以想到的是投票权与代币被押注的时间长短有关。

二、全息共识

全息共识（Holographic Consensus，HC）是由DAOstack带头提出的一个概念。这种投票机制将一个预测市场与每个提案联系起来。预测者可以用资金支持或反对他们认为会通过或失败的提案。如果预测正确，他们会获得经济收益。被预测为会通过的提案会被“提升”，投票从50%的法定人数转换为相对多数（只看赞成票和反对票，不需要法定人数），使得通过提案的障碍比没有资金押注的提案低得多。

使用过这种投票机制的项目包括DXdao、NecDAO和Prime DAO。

这种投票机制天然会保护项目不受恶意提案的攻击，因为需要付费才能攻击（通过在提案上押注资金）。它对有许多提案的项目非常有效，因为成员只需要真正关注有押注的提案。它还允许DAO能够快速通过提案。

另一方面，其用户体验比较混乱，而且它引入了一个新的代币机制（在提案上押注），这并不总是人们所希望的。

与来自DXdao的Sky的Q&A环节：

1）你如何看待基于HC的投票在你的DAO中的应用？

DXdao正在使用的基于全息共识的投票一直运作良好。参与一个使用不可转让的REP进行投票，并使用GEN-staking代币对提案进行预测的系统是非常有趣的，因为这与其他大多数单一的代币治理系统相比很独特。

我的理解是，全息共识的设计是一个可以扩展到数万或数十万成员的系统。显然，目前还没有这种大规模的实践经验，所以DXdao正在实践我们所说的更轻版本的设计。当队列中的提案达到一定程度时锁定机制就成为了过滤的一个重要方面，这种情况并不常见。

总的来说，它运行得很好。DXdao并没有很多有争议的投票。部分原因可能是提出建议的人经常在提出建议之前通过论坛发帖/聊天和社区讨论获得社会共识。这近似于为治理组合添加了第三层。

2）你最不喜欢HC型投票的哪些地方？

全息共识为增加了治理过程的复杂性。最大的缺点可能是很难理解系统工作的确切细节，特别是如果一个人是DAO和系统的新手。

正因为如此，人们需要大量时间和精力来熟悉治理过程以及如何最有效地利用它进行治理。另外，我想说的是，一个有很多成员和移动部件活跃的全息共识治理系统将变得相当昂贵，特别是在以太坊的gas价格上涨的情况下。

3）如果你能轻易改变这个DAO的投票机制，你会这样做吗？

对我来说，目前的治理系统最有趣的补充是将信念投票纳入治理过程的某种方式，以用于目前系统之上的特定类型的提案。我在Gitcoin资助期间，看到Commons Stack的Panvala信念投票系统在运行，感觉非常酷。我认为这种流动的投票方式在某些情况下意义重大。

我也非常喜欢Moloch DAO的简单性——对于新人来说，它们相当容易迅速理解，而且其高效并安全（假如你有必要的社区在监督它们）。

在这一点上，我不认为完全切换到任何其他投票机制是有意义的，因为HC已经很好地满足了DXdao的需求，但我们也是永远在实验！

与来自Prime DAO的Luuk的Q&A环节：

1）你如何看待基于HC的投票在你的DAO中的应用？

我认为HC对一个DAO过滤提案很有用。但我不确定其是否能够为一个DAO做出最好的决策，毕竟对某个事物有专业知识的人并不一定有投票权。Colony的初创想法（即人们在特定领域拥有声誉）看起来很有趣。事实上，在我正在研究的另一个DAO (CuraDAO)中，有些人甚至发现对他们不了解的某些提案进行投票是不道德的!我并不一定相信这些巨型DAO的愿景。

虽然与投票机制没有什么关系，但我确实非常喜欢DAOstack DAO中的提案信息和流程。

2）你最不喜欢HC型投票的哪些地方？

使用GEN非常具有挑战性。

3）如果你能轻易改变这个DAO的投票机制，你会这样做吗？

我会对不同的决策采用多重投票机制。HC用于基础层决策，然后信念投票用于预算决策。一代币一票（1 Token 1 Vote）用于其他情况。对我来说，用合适的工具做正确的事情是最有意义的。HC对高层有意义，但不一定适用于低层。

三、授权的相对多数（**Moloch DAO**）

相对多数（即，你只是对赞成和反对票的总数进行比较）对于DAO来说不是一个可行的治理方案，因为它们很容易被攻击（一个人可以在其他人不注意的时候轻易地耗尽DAO的资金！）。然而，Moloch DAO有一个很好的小功能来防止这种情况：提案需要由DAO成员赞助才能被投票，这提供了一个很好的安全缓冲区。

使用过这种方式的项目包括MetaCartel Ventures、Raid Guild和DAOhaus。

这种投票机制的一些优点包括简单的用户体验、成员需要的行动较少，这意味着较低的关注度需求和gas成本。另一方面，因为提案很容易通过，如果没有人关注，就会带来风险。这种机制被设计得比较慢。

与来自LexDAO的Adam的Q&A环节：

1）如何看待“授权的相对多数”在你的DAO中的应用？

LexDAO以前使用基于法定人数的投票，这是一个噩梦。我们必须不去鞭策每一票，以获得足够的人加入。对gas的抱怨是无休止的，即使是在投票是0.50美元的时候。即使投票很少，人们也仍然被gas困扰。另一方面，Moloch倾向于有效地调整激励机制以促进社区发展。它将负担从“让足够多的人说是”作为完成任何事情的门槛，转为“如果你在意你就要说‘不’”。

2）你对这种投票机制有讨厌之处吗？

它实在比较慢。很多内置的保护措施都是围绕着提案过程的时间来进行的。

3）你会换成别的投票体系或者对它做出一些改变吗？

授权可能是一个很好的补充。

与来自Raid Guild的Dekan的Q&A环节：

（Dekan是运行Moloch DAOS的平台DAOhaus的建设者）

1）如何看待“授权的相对多数”在你的DAO中的应用？

我喜欢简单多数的规则，也喜欢Moloch投票时没有法定人数。只需要一票就能通过一个提案，这样可以节省gas，但也需要成员对监督提案保持警惕。这需要一个参与式的社区。

2）你对这种投票机制有讨厌之处吗？

虽然“少数服从多数”有其积极意义，但在某种意义上也是一种消极因素。一张选票可以决定很多事情，所以如果社区没有参与，一个提案就可以偷偷通过。如果一个提案真的通过了，成员仍然可以愤怒地退出，但这也可能被错过。因此，对你的DAO中发生的投票要有高度的责任感。

3）你会换成别的投票体系或者对它做出一些改变吗？

我希望有一个提前投票的机制，这样一个特别提案可以在达到一定的法定人数后立即通过。

四、信念投票

信念投票（Conviction Voting）是一个高水平的投票机制，用于预测在分布式工作提议系统的实时集体偏好。投票者不断表达他们的偏好，把代币投在他们希望通过批准的提案上。随着投票时间的推移，他们对自己投票的信念（即，权重）也在增长。集体信念累积，直到它达到一个提案所需的基金比例的算法型设置的门阀。当信念累积超过阈值，提案就会通过，基金就会被发放，项目可以开始了。Aragon最近开始了这种新型投票机制的试点，目前仍处于非常试验性的阶段。

正在使用这种方式的项目包括1Hive、Panvala和Commons Stack。

这种投票机制在理论上可以防止拥有大量押注和强势意见的人压制少数选民。不需要大多数人对每个提案达成共识，相反，代币持有者可以简单地关注他们支持的提案。

另一方面，这种投票机制还没有经过实战检验，它的用户体验比较混乱，很可能需要与其他投票机制一起使用，这些机制更适合于“Yes or No”或时间敏感的决策。

来自1Hive的Luke的Q&A环节：

（Luke是1Hive和Aragon的成员，这两个组织资助建立了信念投票系统）

1）如何看待您迄今为止对信念投票进行的试验？

信念投票真的很有趣，现在还为时尚早，但我认为从去中心化治理的角度来看，它是一个游戏规则的改变者。由于其工作方式非常不同，很难将它与其他投票机制进行比较。至少在我们使用的背景下，其更多的是关于预算和资源分配，而不是达成一个具体的共识/决定。

2）你认为它可以有效地用于特定的共识/决策吗？或者有什么原因使它不那么好用？

这不是真正正确的工具，尽管在某些情况下它可以被应用。例如，我们把它用于募资，所需的支持量取决于一个提案从财政库/池子的可用资金中申请的资金量。另一个用例是更新一个线性参数（如通货膨胀率），这可以通过定期平均信号来移动参数值来完成。但如果做出“升级这个智能合约”这样的任意决定，就没有什么意义了。

3）你会换成别的投票体系或者对它做出一些改变吗？

我希望有一个提前投票的机制，这样一个特别提案可以在达到一定的法定人数后立即通过。

五、多签

许多项目和社区都选择走多签（Multisig）路线（通常使用Snapshot进行链下信号传递）。在这种投票机制中，代币持有者对提案发出信号，然后由一个更集中的委员会执行，该委员会通常控制一个Gnosis Safe。对这一选项的更深入分析以及问答将在以后公布。

六、**Colony**的**“**懒惰共识**”**投票机制

在这个由Colony开发的系统中，社区中的任何人都可以提出动议，让事情发生。如果在一定时间内没有人反对，就会发生。如果有人反对，则由信誉加权的投票决定是否应该发生。这种投票机制仍在开发中，所以我们还没有第一手资料或实例项目。

七、结语

目前，绝大多数项目都在使用基于法定人数的投票，部分原因是它是最经得起考验的，而且对现有的项目来说也是最简单的整合。但是，我们仍然处于产品/协议治理的超级早期阶段。项目所使用的投票机制影响着从成员参与到安全和社区文化的一切。“正确的”投票机制可以在项目的长期成功中发挥关键作用，因为它允许团体以正确的速度和最小的风险做出最佳决定。

在一个绝对的赢家出现之前，项目应该尽量减少将自己锁定在一个特定的协议或投票机制中，并随着空间的不断发展而开放实验。



---

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）

详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)

历史文章：

[Synthetix：去中心化治理结构](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484318&idx=1&sn=ebea1216fb8bdaa17de340aec02274a5&chksm=c1d8024bf6af8b5dcc504cefe8129bd910cc6234a2bd6828f6d9e375a97048209149d1b19e8a&scene=21#wechat_redirect)

[DAOMaker: 代币化的创业孵化器和募资平台](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484380&idx=1&sn=c6b092df9c03839de357626b9a167209&chksm=c1d80209f6af8b1fe100bda68669993ede2058b3495df82b0463f5bf50ea567c344137212dbe&scene=21#wechat_redirect)

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

[基于 Futarchy治理的案例：Amoveo、Tezos、Gnosis](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484178&idx=1&sn=286ca0a3bb98b585e3b41cf41de348b8&chksm=c1d802c7f6af8bd135b1ab5fbf1e639f0a8ccb210a1311b967018770f303a89da8b1ada7b306&scene=21#wechat_redirect)

[联合曲线设计脑洞大全及参数大典](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484168&idx=1&sn=939737a69feb60a822ebd86b8d94cce1&chksm=c1d802ddf6af8bcba3944b673af03cf03404cde39285c6e2a605ea99e14e606631f4a6cd4523&scene=21#wechat_redirect)

[DAOrayaki首发| SEC.gov代币安全港提案2.0](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484100&idx=2&sn=34ecbf7ecfa2e32646d69026c550c555&chksm=c1d80311f6af8a0726e84cf990c874002fead7a5f6f3cedd45a216064a4f7ae80185a1356172&scene=21#wechat_redirect)

[深度回顾币安智能链BSC Grant HackerLink第一期](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484046&idx=1&sn=72f298e4d41833d6f39340deed5bf424&chksm=c1d8035bf6af8a4de7934291b2f6cff23bd0f808b57d65ccc177266bdf7649516e103cf35cbe&scene=21#wechat_redirect)

[Futarchy | 价值投票，对赌信仰，用钱说话，口说无凭](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484004&idx=1&sn=433b36bc5b077011f5abdd8b83c802b2&chksm=c1d803b1f6af8aa74094f3c2d14ca2b9d22d807a5fdc4374cbe6f5f55b8e33d585d61604f07e&scene=21#wechat_redirect)

[平行世界｜DeFi无缝集成全球最性感资产—BTC，特斯拉和茅台](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483954&idx=1&sn=d0a5a470a969e9aa9d9f6a6b2bb89232&chksm=c1d803e7f6af8af1574df947cb8be6710937f0a5f30978c255acf81ec02b989b86d184a2e205&scene=21#wechat_redirect)

[「激进市场」和二次方投票 | 用市场本身去监管市场](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483861&idx=1&sn=4e8b5b58a53a942df10fd7e38147ae61&chksm=c1d80000f6af8916f92328a4dc051a92c6836fe6b35bdd762dcb002e944d7663a94b63254e59&scene=21#wechat_redirect)





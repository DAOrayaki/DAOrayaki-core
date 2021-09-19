

元数据、数据堆栈、数据目录3.0
================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



3 Aug 2021
• 16 min read






![元数据、数据堆栈、数据目录3.0](/content/images/size/w2000/2021/07/1.png)



### DAOrayaki DAO研究奖金池：

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 3/7 通过

赏金总量：120 USDC

研究种类：DAO, Metadata, Data Stacks, Data Catalog 3.0

原文作者:  Prukalpa

贡献者： Dewei, DAOctor @DAOrayaki

原文: Data Catalog 3.0: Modern Metadata for the Modern Data Stack

![](http://daorayaki.org/content/images/2021/07/----_20210426113809-19-3.png)2020年给我们的日常词汇带来了很多新词汇——想想冠状病毒、封锁、大流行、退款。但在数据世界中，另一个短语一直在流传……现代数据堆栈

数据世界最近汇集了处理海量数据的最佳工具集，即“现代数据堆栈”。这包括在同类最佳工具上设置数据基础架构，例如用于数据仓库的 Snowflake、用于数据湖的 Databricks 和用于数据摄取的 Fivetran。

现代数据堆栈的优点：现代数据堆栈非常快，很容易在几秒钟内扩展，而且需要很少的开销。缺点：在数据治理、信任和上下文方面，它仍然是个新手

****数据堆栈-元数据的来源****

那么，现代元数据在今天的现代数据堆栈中应该是什么样子呢？基本数据目录如何发展成为数据民主化和治理的强大工具？为什么要进行元数据管理需要一个范式的转变来满足今天的需求？

****为什么现代数据堆栈比以往任何时候都更需要“现代”元数据管理？****

几年前，数据主要由组织中的 IT 团队使用。 然而，今天的数据团队比以往任何时候都更加多样化——数据工程师、分析师、分析工程师、数据科学家、产品经理、业务分析师、公民数据科学家等等。 这些人中的每一个都有自己喜欢的、同样多样化的数据工具，从 SQL、Looker 和 Jupyter 到 Python、Tableau、dbt 和 R。

这种多样性既是一种力量，也是一种斗争。 这些人都有不同的解决问题的方式、工具、技能组合、技术堆栈、工作方式……本质上，他们每个人都有独特的“数据 DNA”。

结果往往是协作中的混乱。 令人沮丧的问题，例如“此列名称实际上是什么意思？” 和“为什么仪表板上的销售数字又错了？” 在需要使用数据时让快速团队陷入困境。

这些问题并不新鲜。毕竟，Gartner 发布元数据管理解决方案魔力象限已经超过 5 年了。

但是仍然没有很好的解决办法。 大多数数据目录只不过是 Hadoop 时代的创可贴解决方案，而不是跟上当今现代数据堆栈背后的创新和进步。

****元数据管理的过去和未来****

就像数据一样，我们思考和使用元数据的方式在过去三年中一直在稳步发展。 它可以大致分为三个演进阶段：数据目录 1.0、数据目录 2.0 和数据目录 3.0。

****数据目录1.0：IT团队的元数据管理****

时间：1990 年代和 2000 年代初

产品：Informatica、Talend

![](http://daorayaki.org/content/images/2021/07/image-224.png)元数据在技术上自古以来就存在——例如 附在亚历山大图书馆每卷卷轴上的描述性标签。 然而，元数据的现代概念可以追溯到 1900 年代后期。在 1990 年代，我们庆幸将软盘放在一边，并拥抱了这种称为互联网的新奇工具。很快，大数据和数据科学风靡一时，组织正试图弄清楚如何组织他们的新数据集合。

随着数据类型和格式以及数据本身的爆炸式增长，IT 团队负责创建“数据清单”。 像 Informatica 这样的公司在元数据管理方面处于领先地位，但是对于 IT 人员来说，建立和保持新的数据目录一直是一项艰巨的任务。

数据仓库团队经常花费大量时间谈论、担心元数据，并为元数据感到内疚。 由于大多数开发人员天生厌恶文档的开发和有序归档，因此尽管每个人都承认元数据很重要，但元数据通常会从项目计划中删除。”

– 拉尔夫·金博尔，2002

****数据目录2.0：由数据管理员提供动力的数据库存****

时间：2008-2020

产品：collibra，Alation

![](http://daorayaki.org/content/images/2021/07/image-225.png)随着数据变得越来越主流并扩展到 IT 团队之外，数据管理的想法开始生根发芽。 这指的是一组专门负责管理组织数据的人员。他们将处理元数据、维护治理实践、手动记录数据等。

与此同时，元数据的想法发生了变化。 随着公司开始建立大规模的 Hadoop 实施，他们意识到简单的 IT 数据清单已经不够了。 相反，新的数据目录需要将数据清单与新的业务环境相融合。

就像这个时代超级复杂的 Hadoop 系统一样，Data Catalog 2.0 很难设置和维护。 它们涉及严格的数据治理委员会、正式的数据管理员、复杂的技术设置和冗长的实施周期。 总而言之，这个过程可能需要长达 18 个月的时间。

这个时代的工具基本上是建立在整体架构上并部署在本地的。 每个数据系统都有自己的安装程序，公司无法通过推送简单的云更新来推出软件更改。

技术债务不断增长，元数据管理开始稳步落后于其他现代数据栈

****元数据中范式的转变****

尽管其他数据基础架构堆栈在过去几年中得到了发展，而且 Fivetran 和 Snowflake 等工具让用户可以在不到 30 分钟的时间内建立一个数据仓库，但数据目录却跟不上。 即使尝试使用 Data Catalog 2.0 时代的元数据工具也需要花费大量的工程时间进行设置，更不用说至少与销售代表进行 5 次通话以获得演示

由于缺乏可行的替代方案，现代数据堆栈的最早采用者和大多数大型科技公司都诉诸于构建自己的内部解决方案。 一些著名的例子包括 Airbnb 的 Dataportal、Facebook 的 Nemo、LinkedIn 的 DataHub、Lyft 的 Amundsen、Netflix 的 Metacat 和 Uber 的 Databook。

然而，并不是所有的公司都有这样的工程资源，而且构建几十个类似的元数据工具并不是特别有效。

数据目录3.0：面向不同数据用户的协作工作区

今天，我们正处于元数据管理的转折点——从缓慢的内部部署数据目录 2.0 转变为新时代数据目录 3.0 的开始。 就像从 1.0 到 2.0 的跳跃一样，这将是我们对元数据的看法的根本转变

Data Catalog 3.0 的外观和感觉与 Data Catalog 2.0 代的前辈不同。 相反，数据目录 3.0 将建立在嵌入式协作的前提下，这是当今现代工作场所的关键，借鉴了 Github、Figma、Slack、Notion、Superhuman 和其他当今司空见惯的现代工具的原则

![](http://daorayaki.org/content/images/2021/07/image-226.png)****数据目录3.0的4个特征****

****1.数据资产 》表格****

Data Catalog 2.0 生成的前提是“表格”是唯一需要管理的资产。 但现在完全不一样了。

如今，BI 仪表板、代码片段、SQL 查询、模型、功能和 Jupyter 笔记本都是数据资产

3.0代元数据管理将需要足够灵活，以便智能地存储和将所有这些不同类型的数据资产链接在一个地方。

**2.端到端数据可见性，而不是零碎碎的解决方案**

数据目录 2.0 时代的工具在改进数据发现方面取得了重大进展。 然而，他们并没有为组织提供数据的“单一事实来源”。 有关数据资产的信息通常分布在不同的地方——数据沿袭工具、数据质量工具、数据准备工具等等。数据目录 3.0 将帮助团队最终实现圣杯，即组织中每个数据资产的单一事实来源。

**3.元数据为“大数据”的世界而构建**

我们正在快速接近元数据本身就是大数据的世界。 能够处理和理解元数据将有助于团队更好地理解和信任他们的数据。

这就是为什么新的数据目录3.0应该不仅仅是一个元数据存储的原因。

它应该从根本上利用元数据作为一种数据形式，可以以与所有其他类型的数据相同的方式进行搜索、分析和维护

今天，云的可扩展性使这成为可能，这是前所未有的。 例如，查询日志只是当今可用的一种元数据。 通过解析 Snowflake 中查询日志中的 SQL 代码，可以自动创建列级沿袭，为每个数据资产分配流行度分数，甚至可以推断每个资产的潜在所有者和专家。

**4. 嵌入式协作已经成熟**

Airbnb 在分享他们在推动采用内部数据门户方面的经验时说了一些深刻的话：“设计数据工具的界面和用户体验不应该是事后的想法。”

由于数据团队的基本多样性，需要设计数据工具以与团队的日常工作流程无缝集成。

这就是嵌入式协作理念真正活跃的地方。 嵌入式协作是指在您所在的位置进行工作，摩擦最少。

如果可以在获得链接时请求访问数据资产，就像使用 Google Docs 一样，并且所有者可以在 Slack 上获得请求并立即批准或拒绝它，该怎么办？ 或者，当您检查数据资产并需要报告问题时，您可以立即触发与工程团队的 JIRA 工作流程完美集成的支持请求，该怎么办？

嵌入式协作可以统一数十个这样的微型工作流程，这些工作流程会浪费时间、造成挫折并导致数据团队的工具疲劳，反而让这些任务变得有趣！

****数据保护与连接元数据****

**为什么保护元数据如此重要？**

连接元数据是您在线进行操作时生成的数据，例如访问网站、使用应用程序或发送消息。此元数据记录信息，例如谁发送了数据（以 IP 地址的形式）、他们将数据发送到何处（另一个 IP）、何时以及发送了多少数据。简而言之，它是关于数据的数据。

就其本身而言，这似乎并不多，但每次在线互动都会生成数十个元数据，几乎都是公开的或易于查找的。如果有人收集了足够多的元数据，他们很快就会清楚地了解你的在线活动，并了解你的线下生活。即使连接是端到端加密的，这也是可能的。

**为什么存在连接元数据？**

因此，如果存在这样的问题，为什么不停止创建所有这些元数据，或者至少将其设为私有？不幸的是，事情并没有那么简单：公共元数据对于互联网目前的运作方式至关重要，这是一个没有人能够想象互联网会发展到多大的时代的遗物，或者恶意行为者可能会如何滥用它。

基本上，可以把它想象成邮寄一封信。内容可以密封在信封中，但要到达目的地，信封需要清楚地注明地址。任何人都可以读取此地址信息。如果他们愿意，他们可以记下信封的去向、信封有多大以及何时寄出。随着时间的推移，他们可以建立这些信息的数据库并开始寻找模式。所有这些都无需打开信封。

如果我可以看到您在哪些商店购物、您正在使用哪些应用程序以及您向谁发送消息，我实际上不需要知道您的消息内容或您购买的完整详细信息来推断很多关于你的信息。

但是谁真正看到了这个元数据？每次上网时，数十家不同的公司和服务都会看到并可能记录此元数据。有互联网服务提供商 (ISP)、电信公司、使互联网正常工作的 DNS 服务器和内容交付网络 (CDN)，例如 Cloudflare，它们实际上为大部分 Web 内容提供服务。大多数情况下，这些服务都在未经您同意的情况下收集和存储有关您的信息。

现代网络服务相互关联的方式意味着这个列表只会增加。例如，如果访问一个嵌入了 YouTube 视频的网站，那么即使不点击视频，Google 也会收到访问通知。这些信息可以通过IP 地址轻松链接到用户的姓名，谷歌通过用户的谷歌帐户知道用户的姓名，并添加到谷歌维护的关于用户的详细档案中。不仅仅是谷歌。同样的事情也发生在 Facebook，或者像 Medium 这样的博客托管网站，或者即时消息平台。这一切都不需要 cookie 或任何额外的代码，更改您的隐私设置也不会阻止它。这就是当今互联网的运作方式。

那时我们甚至还没有遇到黑客、政府过度干预等问题，以及如果用户是在线企业，如何安全地处理和保护元数据的巨大问题，现在监管机构已经开始注意到这一点。但这些是未来剧集的主题。

公共连接元数据在 Internet 的工作方式中根深蒂固，因此没有简单的解决方案。解决它的唯一方法是采用全新的数据传输方法。

目前，区块链项目开始关注这一领域。即使得用户、公司和设备在完全隐私的情况下，进行在线交换信息。通信和交易的人可以确保没有人能够知道正在共享哪些数据、谁正在发送或接收数据，甚至有多少数据被发送。

最重要的是，具备去中心化的、完全透明且无需信任的特点，意味着永远不必依赖第三方，也永远不会被锁定在服务中或不得不放弃对数据的控制。



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







Keep3r : 去中心化协作服务网络
===================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



28 Jun 2021
• 23 min read






![Keep3r : 去中心化协作服务网络](/content/images/size/w2000/2021/06/--1-17.png)



DAOrayaki DAO 研究奖金池：

资助地址:0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee Yes

赏金总量：200 USD

研究种类：DAO, Blockchain, Keeper, jobs, Yearn Finance, Decentralized Collaborative

贡献者：Jones ，黑白BQ，Daoctor @Daorayaki

![](http://daorayaki.org/content/images/2021/06/----_20210426113809-30.png)上线时间: 2020年10月20日

代币: KP3R (ERC20 $111.8091 2021-06-21)

Keep3r网络是一个去中心化的keeper网络，为需要外部开发的项目和外部团队寻找keeper工作。

Keep3r Network 为任务协议，包含任务发行方和任务执行方。发布任务的 DeFi 协议方，需要支付费用。支付可以通过为 KP3R 提供流动性。例如用户在 Uniswap 或 Sushiswap，通过为 KP3R/ETH 提供流动性，然后可以获得 JobCredit，现机制为通过销毁 Credits 产生 KP3R 支付给执行任务的 Keeper。

yearn.finance 创始人 Andre Cronje 转推由 DeFi Wonderland 发起关于 Keep3r Network v2 新经济模型的提议，针对在 Keep3r Network 中开发人员提供工作获得的代币奖励（KP3R）缺乏流动性这一问题提供了以下解决方案，一、Keep3r Network 将引入稳定币，创建 KP3R 的稳定币锚定机制，并且稳定币可以作为 Job 的支付方式。二、将销毁 JobCredit 获得 KP3R 的机制改为销毁 JobCredit 获得稳定币。该提案通过后将于 Keep3r Network v2 版本进行更新。

创始人：Andre Cronje是Yearn.finance的建造师，Crypto Briefing的首席加密代码审查员。前Fantom基金会技术委员会主席，Lemniscap的技术分析师。

**I 介绍**

Keep3r 是去中心化的 Keeper 任务网络，一方面有的智能合约项目需要外部实体帮忙解决 devops 方面的任务，一方面有些外部实体（个人或团队）可以通过完成相应任务获得报酬。Keep3r 为这部分人群构建去中心化的任务服务网络。

Keeper 是指执行工作的外部人员或团队。这些任务可以是简单的（如调用交易），也可以是复杂的（要求链下的逻辑）。Keep3r 不是严格意义上的任务服务平台，Keep3r 本身并不管理这些任务，它允许项目方（合约）注册任务，而 keeper 也需要注册，这样双方都可以选择彼此。在这个过程中，keeper 设置其 devops 以及基础设施，并可以创建规则（基于有利可图的交易）。

根据 Andre Cronje 的说法，当前的 Keep3r 核心要解决智能合约需要外部触发的问题。一些合约需要由外部实体（机器人、脚本、EOA）提交交易从而触发响应。Keep3r 试图解决这个问题，它通过去中心化的方式，构建出一个协作系统，试图帮助这些项目找到 keeper 来进行合约的外部触发从而保持运行。从这个角度，Keep3r 不是面向普通用户的项目，它主要为 dApp 的开发者们服务。

那么，作为项目方和外部实体的协作网络，keep3r 是如何通过去中心化的方式将两者组织起来的？项目方需要将其合约提交到 Keep3r 网络，合约会由绑定 KP3R 保证金的 Keeper 进行审查和批准，之后，keeper 可以执行市场上的任务。

![](http://daorayaki.org/content/images/2021/06/--1-15.png)****Keep3r 中的任务****

在 keep3r 中，当前的任务，主要是指智能合约希望外部人员执行某个操作。同时，项目方希望 keeper 的执行是善意的，而不是恶意的，尤其是智能合约可能会涉及到财务的风险。

在 Keep3r 中，需要外部执行的系统都可以成为任务。Keep3r 不会定义或限制执行任务的范围，它主要为 keeper 和合约之间提供激励机制。

当前的任务主要是一些合约需要外部实体提交交易从而触发响应。例如在预言机上调用 update() 以更新其基础值；在聚合挖矿协议上调用 Harvest() 以实现资金调换策略；在治理合约上代表用户使用许可 / 批准机制调用 vote()；去中心化交易中价格匹配时触发限价订单；在基于债务的系统中触发清算；在 layer2 中外部系统代表用户批量提交交易等。当前，每个项目为了解决这些问题，都是独立进行的。如 **Aave** 的清算、**Synthetix** 的缓存更新、YFI 的挖矿等。这也是 Andrew Cronje 在构建 Keep3r 时主要构想的任务。

Keep3r 中的任务是需要注册的，目前创建任务可以通过两种方式：

**通过治理注册任务**

通过治理提交提案来注册任务，如果治理获得通过，则无须进一步措施。

**通过合约界面注册任务**

用户通过调用 keep3r 合约上的 addLiquidityToJob （address,uint）来注册任务。调用 addLiquidityToJob （address,uint）将创建等待中的治理投票。用户通过该地址可在每 14 天提交新的任务申请。

![](http://daorayaki.org/content/images/2021/06/--2-8.png)此外任务也有安全级别，项目方根据自己的安全需要选择 Keeper，例如要求 keeper 的保证金数量、完成任务情况、成为 Keeper 的时间长短以及 keeper 质押相关代币的量等。同时，对于没有风险只需执行的合约，可以使用默认的 isKeeper （address）调用。

![](http://daorayaki.org/content/images/2021/06/--3-7.png)****Keep3r 中的 Keeper****

智能合约会提供任务，keeper 可以执行合约任务。为了成为 keeper，可以在 Keep3r 合约上调用 bond （unit），如果用户没有 KP3R 代币，可以使用 bond （0）加入。bonding 有三天时间延迟，三天后即可调用 Activate （）。

![](http://daorayaki.org/content/images/2021/06/--4-6.png)****Keep3r 的代币经济机制****

KP3R 是 Keep3r 网络的代币，不过它不作为交易的硬性支付媒介。因为在 Keep3r 中，项目方可以使用 ETH 或项目代币支付给 keeper。为了激励 Keeper 完成任务，项目方需要给 Keeper 奖励。目前项目方可以选择三种方式奖励 keeper：

l 直接支付 ETH

l 直接支付代币

l 通过提供流动性间接支付给 Keeper

当然，这些任务也可以用 KP3R 代币进行奖励。通过成为流动性提供者，可有获得 Credit，这些信用额度可用来获得对应数量的 KP3R 代币。每次任务执行时都会为 Keeper 提供（最多） gasUsed * fastGasPrice + premium%，这些会从项目方的信用额度中扣除（不会从流动性中扣除）。项目方可以随时增加和移除全部流动性。

如果 KP3R 不作为支付代币，那么，它有什么用处？

**保证金**

因为有些合约的外部触发工作跟财务风险有关，执行触发任务的外部 keeper 需要最小的保证金才能有资格执行相关任务。而这个保证金使用的是 KP3R 代币。也就是说，要想执行这些任务的 Keeper 必须存入相应的最低数量的 KP3R 保证金。

**治理**

Keep3r 网络治理是由绑定了 KP3R 保证金的 Keeper 来管理的。

**捕获交易费用**

交易虽然不一定通过 KP3R 支付，但所有交易依然会产生费用，对于任何非 KP3R 交易（ETH 或代币支付的交易），存储库获得 0.3% 的费用。

总结来说，KP3R 可以用来治理，可以作为获得高风险任务的保证金，可以捕获交易费用。此外，流动性提供者可以给 Keeper 支付 KP3R 信用。

****治理****

按照 Andre Cronje 的设计，Keep3r 治理主要任务有：

l 添加接受任务信用的流动性池

l 批准 / 撤销任务

l 关于争议 / 消减 / 解决 / 撤销 Keeper

l KP3R 奖励金设置

****当前进展****

l 存储库价值 980 万美元，会由治理投票决定存储库资金的使用和分配

UniswapV2Oraclefeeds 已有足够数据点可用于 Keep3rV1 Helper feeds

l 目前正在审查的任务：Hegic Pool 维护；Aave 的清算；Synthetix （多个任务）；**Yearn** （多个任务）；Cream Finance 的清算。

****II 任务市场****

****协议会发布哪些任务请求？****

在理解任务请求之前，需要先理解我们经常看到「智能合约」。「智能合约」在其逻辑执行完成之后停止，需要再次触发才能执行，也就是说，所谓的「智能合约」其实并不「智能」，很多时候是无法自动执行的。

比如人们参加流动性挖矿，产生奖励之后，这些奖励不会自动进入用户的钱包地址，而是需要「claim」；在 **Yearn** 的聚合挖矿中，获得挖矿代币奖励之后，需要卖出换成稳定币，然后再存入继续挖矿，在挖矿过程中，它有策略，有大量工作需要触发，需要跟智能合约交互；在 Sushiswap 进行限价订单的交易，也需要在符合价格要求时候进行触发；在 Hegic 上期权到期后也需要触发才能解锁其锁定资金等等。

该系统与Keepers和Jobs一起工作。

Jobs是需要外部行动的智能合约，而Keepers是完成工作的个人或团队。

Jobs的创造者可以设置Keepers必须满足的条件，以获得资格，包括完成的工作，代币持有量，年龄，或赚取的资金。

Jobs可以通过治理程序获得批准，也可以通过向已批准的货币对（如KP3R/ETH）增加流动性直接纳入。

Jobs可以用ETH、代币或通过KP3R的流动性支付给Keeper。

安德烈最近宣布，Keeper将与ChainLink一起扩大规模，利用该协议的安全性和可靠性。

目前的智能合约上有大量的任务需要触发来执行（触发清算、调用预言机、解锁质押品等）。这就是为什么有很多任务（jobs）的原因。

这些 jobs 的规模多少，直接决定了 KP3R 未来的上限。KP3R 能达到多高的高度，核心还是取决于 jobs 市场规模有多大。随着 DeFi 协议的发展，KP3R 的任务会越来越多，其市场规模也会越来越大。但具体有多大，目前还不明确。

**什么是Keep3rV1 (KP3R)代币？**

Keep3rV1 (KP3R)代币是Keep3r Network项目的原生加密货币。Keep3rV1 (KP3R)以DeFi币形式生产，最大供应量和流通量为 200,991 个KP3R币。

**保留KP3R的优点和缺点**

保留KP3R的优点包括：

较高的担保增加了 Jobs Keepers 有资格从事的类型；

只有质押KP3R 才能在治理中授予投票权；

不能利用质押的 KP3R。这是为了防止 Job 漏洞。

然而，保持质押 KP3R 的缺点是你不能立即为 Keeper 交易收回 ETH。这意味着 Keepers 必须保留未质押天数的 ETH 作为浮动。对此的解决方案是 MetaKeep3r.

任务执行人 Keeper

KP3R 的任务市场有很多需要触发的工作，不过这些触发的工作是不是 DeFi 协议自己也可以通过自动化的机器人来完成？为什么还需要 keeper？这也跟 DeFi 协议的追求有关。DeFi 最终来说，它要实现其去中心化的目标，它需要的不仅仅是自动化，更是去中心化的自动化。

Keeper 可以帮助 Yearn vault 用户触发 claim，可以帮助货币市场触发清算，而这个市场上的 keeper 不只有一个，有很多个，这样可以保证在一个 keeper 不接任务的时候，其他 keeper 可以接任务。

为了成为 Keeper，他们需要质押保证金，可以防止 keeper 作恶，有些任务可能会要求有最低的质押数额。质押保证金使用 KP3R，这也形成了对 KP3R 的需求。如果 Keeper 作恶，其质押的 KP3R 会遭受罚没。

****KP3R 成为 DeFi 的基础层****

在 DeFi 中有不少基础层，例如预言机领域算一个，而 KP3R 也是一个基础层，它不是服务于某个特定的 DeFi 协议，而是服务于整个 DeFi 领域。

当然，如果从更底层的角度，KP3R 可以有预言机的服务，可以帮助协议解决喂价问题。这个时候预言机的节点就成为了执行任务的 Keeper。

****对 KP3R 的需求****

****KP3R 作为质押保证金****

随着需要触发服务的 DeFi 协议越来越多，对 KP3R 的需求越来越多，因为要想成为 Keeper，要想赚取 job 市场上的费用，首先需要质押 KP3R。

质押的 KP3R 保证金有 14 天的退出期，以保证 Keeper 不会做恶。

****为 KP3R 提供流动性****

发布任务的 DeFi 协议方，需要支付费用。支付费用的方式可以是代币，也可以是 ETH，也可以通过为 KP3R 提供流动性。例如用户在 **Uniswap** 或 Sushiswap，通过为 KP3R/ETH 提供流动性，然后可以获得 credits，通过这些 Credits 产生 KP3R 支付给执行任务的 Keeper。

目前 Uniswap 上为 KP3R 提供流动性的代币为 4802 个，大约占据 KP3R 总量的 2.39%。

****协议费用****

当任务使用 ETH 或代币支付时，KP3R 会收取 0.03% 的费用。

**III 联系方式：**

官网: <https://www.coingecko.com/en/coins/keep3rv1/>

Github:  <https://github.com/keep3r-network>

Twitter：<https://twitter.com/AndreCronjeTech>

coinmarketcap: <https://coinmarketcap.com/currencies/keep3rv1/>

Coingecko:  <https://www.coingecko.com/en/coins/keep3rv1/>

****Keep3r : Decentralized Collaborative Services Network****

DAOrayaki DAO Research Grant：

Fund Address: **0xCd7da526f5C943126fa9E6f63b7774fA89E88d71**

Voting Result：**DAO Committee Yes**

Grant Amount：**200 USDC**

Category: Blockchain, Keeper, jobs, Yearn Finance

Contributor：黑白QB, **DAOctor** @Daorayaki

Launch TIme: 2020年10月20日

Token: KP3R (ERC20 $111.8091  2021-06-21)

Keep3r Network is a decentralized keeper network for projects that need external devops and for external teams to find keeper jobs.

**Founder：Andre Cronje** is Architect at Yearn.finance, Chief Crypto Code Reviewer at Crypto Briefing. Former Chair, Technology Council at Fantom Foundation, Technology Analyst at Lemniscap.

**I Introduction**

Keep3r has had some performances these days, which has attracted the attention of the encryption community. What is Keep3r? It is a new work by Andre Cronje. It is a decentralized Keeper task network. On the one hand, some smart contract projects require external entities to help solve devops tasks. On the other hand, some external entities (individuals or teams) can get paid by completing the corresponding tasks. Keep3r builds a decentralized task service network for this group of people.

Keeper refers to an external person or team that performs work. These tasks can be simple (such as invoking transactions) or complex (requiring off-chain logic). Keep3r is not a task service platform in the strict sense. Keep3r itself does not manage these tasks. It allows the project party (contract) to register tasks, and the keeper also needs to register, so that both parties can choose each other. In this process, the keeper sets up its devops and infrastructure, and can create rules (based on profitable transactions).

According to Andre Cronje, the current Keep3r core has to solve the problem of external triggering of smart contracts. Some contracts require external entities (robots, scripts, EOA) to submit transactions to trigger responses. Keep3r tries to solve this problem. It uses a decentralized way to build a collaborative system, trying to help these projects find keeper to trigger the contract externally and keep it running. From this perspective, Keep3r is not a project for ordinary users. It mainly serves dApp developers.

So, as a collaborative network between project parties and external entities, how does keep3r organize the two in a decentralized way? The project party needs to submit its contract to the Keep3r network. The contract will be reviewed and approved by the Keeper bound to the KP3R deposit. After that, the keeper can perform tasks on the market.

![](http://daorayaki.org/content/images/2021/06/--1-16.png)**Tasks in Keep3r**

In keep3r, the current task mainly refers to the smart contract expecting an external person to perform an operation. At the same time, the project party hopes that the execution of the keeper is well-intentioned, not malicious, especially the smart contract may involve financial risks.

In Keep3r, all systems that need external execution can become tasks. Keep3r does not define or limit the scope of tasks performed. It mainly provides an incentive mechanism between the keeper and the contract.

The current task is mainly that some contracts require external entities to submit transactions to trigger responses. For example, call update() on the oracle machine to update its basic value; call Harvest() on the aggregate mining protocol to implement the fund exchange strategy; call vote() on behalf of the user using the permission/approval mechanism on the governance contract; decentralized transactions Trigger limit orders when the medium price matches; trigger liquidation in the debt-based system; in layer2, the external system submits transactions in batches on behalf of users. Currently, each project is carried out independently in order to solve these problems. Such as Aave's liquidation, Synthetix's cache update, YFI's mining, etc. This is also the main task that Andrew Cronje conceived when building Keep3r.

The tasks in Keep3r need to be registered. Currently, there are two ways to create tasks:

l Registration tasks through governance

Submit proposals through governance to register tasks. If governance is passed, no further measures are required.

l Register tasks through the contract interface

The user registers the task by calling addLiquidityToJob(address, uint) on the keep3r contract. Calling addLiquidityToJob(address, uint) will create a waiting governance vote. Through this address, users can submit new task applications every 14 days.

![](http://daorayaki.org/content/images/2021/06/--2-9.png)In addition, the task also has a security level. The project party chooses the Keeper according to its own security needs, such as the amount of the keeper's deposit required, the completion of the task, the length of time to become the Keeper, and the amount of related tokens the keeper pledges. At the same time, for contracts that only need to be executed without risk, the default isKeeper(address) call can be used.

![](http://daorayaki.org/content/images/2021/06/--3-8.png)**Keeper in Keep3r**

Smart contracts will provide tasks, and the keeper can perform contract tasks. In order to become a keeper, you can call bond(unit) on the Keep3r contract. If the user does not have KP3R tokens, you can use bond(0) to join. There is a three-day delay for bonding, and Activate() can be called after three days.

![](http://daorayaki.org/content/images/2021/06/--4-7.png)**Keep3r's token economic mechanism**

KP3R is the token of the Keep3r network, but it is not used as a rigid payment medium for transactions. Because in Keep3r, the project party can use ETH or project tokens to pay to the keeper. In order to motivate Keeper to complete tasks, the project party needs to reward Keeper. Currently, the project party can choose three ways to reward the keeper:

l Pay ETH directly

l Direct payment tokens

l Indirect payment to Keeper by providing liquidity

Of course, these tasks can also be rewarded with KP3R tokens. By becoming a liquidity provider, you can obtain Credit, and these credit lines can be used to obtain the corresponding amount of KP3R tokens. Keeper will be provided with (at most) gasUsed * fastGasPrice + premium% each time the task is executed, which will be deducted from the credit line of the project party (not deducted from liquidity). The project party can add and remove all liquidity at any time.

If KP3R is not used as a payment token, what use is it for?

l Margin

Because the external triggering work of some contracts is related to financial risks, the external keeper performing the triggering task needs a minimum margin to be qualified to perform the related tasks. And this deposit uses KP3R tokens. In other words, Keeper who wants to perform these tasks must deposit the corresponding minimum amount of KP3R deposit.

l Governance

Keep3r network governance is managed by Keeper bound with KP3R deposit.

l Capture transaction fees

Although transactions may not be paid through KP3R, all transactions still incur fees. For any non-KP3R transactions (transactions paid in ETH or tokens), the repository receives a 0.3% fee.

In summary, KP3R can be used for governance, can be used as a margin for obtaining high-risk tasks, and can capture transaction costs. In addition, liquidity providers can pay Keeper KP3R credits.

**Governance**

According to the design of Andre Cronje, the main tasks of Keep3r governance are:

l Add a liquidity pool that accepts task credit

l Approve/revoke tasks

l About dispute/reduction/resolution/withdrawal of Keeper

l KP3R bonus setting

**Current Progress**

The value of the repository is 9.8 million U.S. dollars, and the use and distribution of repository funds will be determined by governance.

l UniswapV2Oraclefeeds has enough data points available for Keep3rV1 Helper feeds

l Tasks currently under review: maintenance of Hegic Pool; liquidation of Aave; Synthetix (multiple tasks); Year (multiple tasks); liquidation of Cream Finance.

****II Task market****

****What task requests will the agreement issue?****

Before understanding the task request, we need to understand that we often see "smart contracts". The "smart contract" stops after its logic execution is completed and needs to be triggered again to execute. That is to say, the so-called "smart contract" is not actually "smart" and cannot be executed automatically in many cases.

For example, after people participate in liquidity mining, after rewards are generated, these rewards will not automatically enter the user's wallet address, but need to "claim"; in Year's aggregate mining, after receiving mining token rewards, they need to be sold for exchange. In the process of mining, it has a strategy and a large amount of work needs to be triggered, and it needs to interact with smart contracts; the transaction of limit orders in Sushiswap also needs to meet the price requirements Trigger; after the option expires on hegic, it also needs to be triggered to unlock its locked funds and so on.

**The system works with Keepers and Jobs.**

Jobs are smart contracts needing an external action, and Keepers are individuals or teams that complete jobs.

Job creators can set conditions Keepers must meet in order to be eligible, including jobs completed, token holdings, age, or earned funds.

Jobs can either go through the governance process to be approved, or be included directly via adding liquidity to an approved pair, e.g. KP3R/ETH.

Jobs can pay Keepers in ETH, tokens, or via KP3R liquidity.

Andre recently announced that Keeper would be scaling with ChainLink, taking advantage of the protocol’s security and reliability.

There are a large number of tasks on the current smart contracts that need to be triggered to execute (triggering liquidation, calling oracles, unlocking pledges, etc.). This is why there are so many tasks (jobs).

The size of these jobs directly determines the upper limit of KP3R in the future. The core of how high KP3R can reach depends on the size of the jobs market. With the development of the DeFi protocol, KP3R will have more and more tasks, and its market size will also increase. However, it is still unclear how big it is.

**What is Keep3rV1 (KP3R) Token?**

Keep3rV1 (KP3R) Token is the native Crypto currency of the project called Keep3r Network. Keep3rV1 (KP3R) is produced as DeFi coin, the maximum supply and circulation supply is 200,991KP3R Coins.

Advantages and disadvantages of keeping bonded KP3R

Advantages of keeping bonded KP3R include:

l Higher bonds increase the types of Jobs Keepers can qualify to do;

l only bonded KP3R grants voting rights in governance;

l bonded KP3R cannot be exploited. This is in case a Job introduces an exploit.

Yet the disadvantage of keeping bonded KP3R is that you cannot immediately recoup ETH for Keeper transactions. Meaning that Keepers had to keep an unbond days amount of ETH as a float. A solution to this is MetaKeep3r.

****Keeper****

There are many tasks that need to be triggered in the task market of KP3R, but can these triggered tasks be completed by the DeFi protocol itself through automated robots? Why do we need keeper? This is also related to the pursuit of the DeFi protocol. Ultimately, DeFi wants to achieve its goal of decentralization. It needs not only automation, but also decentralized automation.

Keeper can help Yearn vault users trigger claims and trigger liquidation in the currency market. There are not only one keeper in this market, but there are many. This ensures that when one keeper does not pick up the task, other keeper can accept the task.

In order to become a Keeper, they need a pledge deposit to prevent the keeper from doing evil. Some tasks may require a minimum pledge amount. The pledge deposit uses KP3R, which also creates a demand for KP3R. If the Keeper commits evil, the KP3R pledged by it will be fined.

**KP3R becomes the basic layer of DeFi**

There are many basic layers in DeFi, such as the oracle field, and KP3R is also a basic layer. It does not serve a specific DeFi protocol, but serves the entire DeFi field.

Of course, from a lower-level perspective, KP3R can have the service of an oracle, which can help the agreement solve the problem of price feeding. At this time, the node of the oracle becomes the Keeper that performs the task.

KP3R data

****KP3R as a pledge deposit****

With more and more DeFi protocols that need to trigger services, there is more and more demand for KP3R, because if you want to become a Keeper, if you want to earn fees in the job market, you first need to pledge KP3R.

The pledged KP3R deposit has a 14-day withdrawal period to ensure that Keeper will not do evil.

****Provide liquidity for KP3R****

The DeFi agreement party that publishes the task needs to pay a fee. The payment method can be tokens, ETH, or by providing liquidity for KP3R. For example, in Uniswap or Sushiswap, users can obtain credits by providing liquidity for KP3R/ETH, and use these credits to generate KP3R payment to the Keeper who performs the task.

Currently, there are 4802 tokens on Uniswap that provide liquidity for KP3R, accounting for approximately 2.39% of the total KP3R.

****Agreement fee****

When the task is paid in ETH or tokens, KP3R will charge a fee of 0.03%.

****III Contact Information****

Offical Website: <https://www.coingecko.com/en/coins/keep3rv1/>

Github:  <https://github.com/keep3r-network>

Twitter：<https://twitter.com/AndreCronjeTech>

coinmarketcap: <https://coinmarketcap.com/currencies/keep3rv1/>

Coingecko:  <https://www.coingecko.com/en/coins/keep3rv1/>



---

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）  
  
详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)

历史文章：

[DAOrayaki解读｜价格敞口和投票权](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484712&idx=1&sn=674e8305b9899f73343eae5d68be6a99&chksm=c1d804fdf6af8deb14b0fb4ae8debb6abef6e96ec0a638768f06da475e097a97cf3f00ea5c8f&scene=21#wechat_redirect)

[DAOrayaki解读｜8步实现去中心化](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484713&idx=1&sn=3b76441db3d940c4ea33fcc7e440e276&chksm=c1d804fcf6af8dea80f1e3bec50b06915e603a5927dac9e255ba3e61f4002c4df27191efb835&scene=21#wechat_redirect)[$WORK 奖励、利益相关者经济学和就业共享的代币化](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484579&idx=1&sn=e52f69e1e926eed1f2d895ad3c23df47&chksm=c1d80576f6af8c60a9f3f0e21d713a61e55ffbad904f0701634aba2f28b9ae746bc2ddd5f046&scene=21#wechat_redirect)

[DAOrayaki解读｜价格敞口和投票权](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484712&idx=1&sn=674e8305b9899f73343eae5d68be6a99&chksm=c1d804fdf6af8deb14b0fb4ae8debb6abef6e96ec0a638768f06da475e097a97cf3f00ea5c8f&scene=21#wechat_redirect)

[DAOrayaki解读｜DAO与全球经济秩序-新自由主义的黄昏（一）](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484684&idx=1&sn=f38e7f8f884f4c6b997506c3c49ca688&chksm=c1d804d9f6af8dcf7e2b8aa629846b60b783d410057e50797ee9b697434f7183d40f04b5f461&scene=21#wechat_redirect)

[DAOrayaki 解读|奥斯特罗姆：公共事务的治理之道](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484580&idx=1&sn=1d1c5412ab24b34242912813041c138a&chksm=c1d80571f6af8c67fbfac08c52c900562a4328f65c7b7a05d09ba3473704ff22aa7153bbefe0&scene=21#wechat_redirect)[DAO治理中的同构性](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484493&idx=1&sn=4169ed86c19a17a063dc97c9f6b9b87e&chksm=c1d80598f6af8c8e6cac5807f59a01c8e7d062ee3b9806c18b9a5cb139377a7b3c5b55d0dd1d&scene=21#wechat_redirect)

[DAOrayaki 研究｜Badger: 加速比特币在DeFi中的发展](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484583&idx=1&sn=ce3513d785537c63563a2a6f4b0f255c&chksm=c1d80572f6af8c64dc90942ec0094915267df5b768dbdc3566eb01a03861a05d85f6bd2d1fec&scene=21#wechat_redirect)

[DAOrayaki 研究｜OpenLaw：自动化法律协议](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484582&idx=1&sn=399fb6eb57009a841d42b686202b6c8c&chksm=c1d80573f6af8c652254e94b62f8b0caa85a5ae22f8ffa745c2fd093e3028e3b0c45768f4674&scene=21#wechat_redirect)

[DAOrayaki 研究｜Orca Protocol：轻量级的社区铸造和管理平台](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484580&idx=1&sn=1d1c5412ab24b34242912813041c138a&chksm=c1d80571f6af8c67fbfac08c52c900562a4328f65c7b7a05d09ba3473704ff22aa7153bbefe0&scene=21#wechat_redirect)

[DAOrayaki 研究｜Badger: 加速比特币在DeFi中的发展](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484583&idx=1&sn=ce3513d785537c63563a2a6f4b0f255c&chksm=c1d80572f6af8c64dc90942ec0094915267df5b768dbdc3566eb01a03861a05d85f6bd2d1fec&scene=21#wechat_redirect)

[Synthetix：去中心化治理结构](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484318&idx=1&sn=ebea1216fb8bdaa17de340aec02274a5&chksm=c1d8024bf6af8b5dcc504cefe8129bd910cc6234a2bd6828f6d9e375a97048209149d1b19e8a&scene=21#wechat_redirect)

[DAOrayaki 研究｜Orca Protocol：轻量级的社区铸造和管理平台](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484581&idx=1&sn=89d7600ed7b2ce945b85f8a3fe73bd73&chksm=c1d80570f6af8c6679920e7e0ea5e42ac253ffa028367881f5d542edb690d613e21b30ab5a88&scene=21#wechat_redirect)

[详解Radicle：去中心化社区的代码协作基础设施](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484495&idx=1&sn=eb91cfc99d2de5fd8a2e4b069abad13c&chksm=c1d8059af6af8c8c9d3a6559505eb8e7dad087b93255f1eaac78222f3497ceff7b0c400a9684&scene=21#wechat_redirect)

[详解Vocdoni: 去中心化的投票系统](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484529&idx=1&sn=1b5c7043115435a09d4241e5d4962230&chksm=c1d805a4f6af8cb2f1570b3cb9bc5e9bd9d396304a247e8447a6bcbc99f26c51dca3161efa6d&scene=21#wechat_redirect)[$WORK 奖励、利益相关者经济学和就业共享的代币化](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484579&idx=1&sn=e52f69e1e926eed1f2d895ad3c23df47&chksm=c1d80576f6af8c60a9f3f0e21d713a61e55ffbad904f0701634aba2f28b9ae746bc2ddd5f046&scene=21#wechat_redirect)

[DAOrayaki 解读|奥斯特罗姆：公共事务的治理之道](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484580&idx=1&sn=1d1c5412ab24b34242912813041c138a&chksm=c1d80571f6af8c67fbfac08c52c900562a4328f65c7b7a05d09ba3473704ff22aa7153bbefe0&scene=21#wechat_redirect)





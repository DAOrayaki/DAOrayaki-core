


[DAO Media](/tag/dao-media/)

Dora Factory支持去中心化DAO研究组织DAOrayaki
==================================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



2 Mar 2021
• 6 min read






![Dora Factory支持去中心化DAO研究组织DAOrayaki](/content/images/size/w2000/2021/03/DAO-Landscape-1.png)



![](http://daorayaki.org/content/images/2021/03/Dora-Factory-logo-4.png)Eric, Architect @DoraHacks @DoraFactory  
義理の姉, Lover of #Dorayaki  
DAOctor, DAO Researcher

现在我们尝试使用一种去中心化自治的形式构建媒体。将DAO作为媒体的组织形态及运用其治理模式运营生态: 读者可以直接通过资助DAO，参与治理，选举执行团队，制定规则和内容标准，DAO根据规则激励整个媒体生态。

设计一个去中心化内容贡献DAO
---------------

首先，传统媒体的运行方式是这样的：

![https://ssimg.frontenduse.top/article/2021/02/17/08c677e1078ba6310a760b9cd9924eae.png?x-oss-process=image/format,webp](https://ssimg.frontenduse.top/article/2021/02/17/08c677e1078ba6310a760b9cd9924eae.png?x-oss-process=image/format,webp)这个传统模型有明显的特点：

* 资本方和金主和媒体受众不是一群人
* 媒体由受董事会控制的公司运营
* 内容创作者被雇佣进行内容编辑
* 公司通过以媒体受众为中心的流量获取利润

传统模型的问题可不再赘述。

也许我们可以重构上面的模型:

* 将媒体公司替换为一个可在链上被选举的执行委员会（DAO Committee），负责运营工作和内容审核
* 媒体DAO的资助者和订阅者/用户这两个群体重合起来（至少部分重合），使资助者从风险承担者，订阅者/用户从旁观者，共同转变为受益者和治理者
* 贡献者（供稿人、作者，等）的激励方式由公司雇佣变为积极自主的DAO激励。

![https://ssimg.frontenduse.top/article/2021/02/17/c3456a15bcc50551ccad68599d3f2b22.png?x-oss-process=image/format,webp](https://ssimg.frontenduse.top/article/2021/02/17/c3456a15bcc50551ccad68599d3f2b22.png?x-oss-process=image/format,webp)相对于传统媒体模型，新的模型有以下几个特点:

* 媒体与内容贡献者的关系发生改变，从合同关系转变为合约关系
* 媒体与资本、金主的关系发生改变，从风险承担者转变为共同治理者
* 内容贡献者与用户关系发生改变，从单向输入，转变为“粉丝”模式
* 媒体的盈利模式发生改变，从以用户为基础的流量模式，转变为以用户、贡献者、资本方为核心的社区活跃度
* 媒体的治理模式发生改变，从反映董事会的思想意志，转变为由直接反映读者意志（需求）且可通过选举替换的DAO Committee治理

这个去中心化内容贡献的DAO具有以下一些功能模块:

* 接受资助并注册成员
* 通过投票选举执行委员会成员
* 提案（对某一项动议发起提案，例如资助特定的内容，或在内容平台增加特定的功能，等）
* 激励规则

### DAO资助者和读者 (Backers & Viewers)

根据不同兴趣群体关注的内容，由订阅者组成的DAO由订阅者直接资助。这样，资助者（很大一部分订阅者）也就自然成为了DAO的成员。DAO的成员有以下三种权力：

* 提案: 激励某个特定的内容，或提案修改DAO的规则
* 投票: 对提案进行投票
* 选举: 选举执行委员会的成员

### 执行委员会 (DAO Committee)

DAO Committee是执行委员会，有以下几个职能：

* 审核内容
* 发布内容
* 根据规则激励贡献者
* 其他管理工作

这里，执行委员会替代了媒体公司，并且由DAO的资助者直接选举产生。另外，执行委员会根据DAO预先设定的公开规则审核内容，执行和激励的过程保持链上可见。

### 贡献者网络 (Contributor Network)

贡献者是内容的生产者。贡献者可以通过提交DAO指定的内容获取激励（前提是内容通过被发布），或通过完成Bounty赏金获取激励。

### 主动激励 vs. 被动激励

在激励规则中，有主动激励和被动激励两种形式。主动激励可以通过独立的提案，或Bounty赏金完成。被动激励可以通过DAO设置的激励规则完成。例如，一个媒体/内容贡献网络的默认激励是“如果A提交了内容，且执行委员会决定发布此内容，那么A获得X奖励。”

DAOrayaki: 一个研究DAO的去中心化媒体
-------------------------

我们现在用上面的模型来设计一个研究DAO和链上治理机制的媒体DAOrayaki。

![https://ssimg.frontenduse.top/article/2021/02/17/b75a3e4db75a37a05635b17bdb71f1e8.png?x-oss-process=image/format,webp](https://ssimg.frontenduse.top/article/2021/02/17/b75a3e4db75a37a05635b17bdb71f1e8.png?x-oss-process=image/format,webp)在第一阶段，实现去中心化贡献和激励机制。DAOrayaki Committee由 7名DAO深度玩家组成。

### DAOrayaki的内容类别

* DAO项目分析
* DAO工具
* 链上治理机制研究

### DAOrayaki的内容投票规则和激励规则

DAO Committee需要对任何提交的文章进行投票。简单多数通过(>50%)文章即可发布。

**被发布的原创文章贡献者将获得100 USDC的奖励。被发布的翻译文章将获得<=100 USDC的奖励。**

另一种激励方式是通过HackerLink Bounty发布，悬赏金额由Bounty确定。https://hackerlink.io/bounty

参与贡献请加入TG https://t.me/daorayaki

### 项目分析类文章内容覆盖范围

1. 项目介绍
2. 内容分类  
DeFi DAO（去中心化金融DAO）  
VC DAO （去中心化DAO基金）  
Public Chain Community （公链社区DAO）  
Developer DAO （开发者DAO）  
Off-chain DAO（链下治理DAO）  
DAO Tools（DAO工具）  
Others（其他）
3. 当前项目概况：  
成立时间，团队介绍，主要业务，发展状况
4. 数据指标：  
-Token市值  
-用户数量  
-TVL  
-用户参与度  
-Proposal数量/通过率  
-融资情况  
-等
5. DAO生成平台：  
-DAO生成工具（from Aragon，Colony，Moloch，DAOstack，DAOHaus，etc）  
-自行研发
6. 技术／公链：  
公链（Ethereum，Polkadot，BSC, Solana，etc）
7. 社区：  
-社交媒体: 关注量，活跃度  
-论坛：发帖量，用户数  
-KOL推荐
8. 机制：  
-参与门槛  
-投票机制  
-激励机制  
-仲裁机制

### 附录1 – DAO全景图 Landscape

![](http://daorayaki.org/content/images/2021/03/DAO-Landscape.png)参与贡献请加入TG https://t.me/daorayaki

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！

  






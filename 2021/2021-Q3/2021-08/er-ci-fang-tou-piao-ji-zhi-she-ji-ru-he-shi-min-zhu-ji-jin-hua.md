

二次方投票：机制设计如何使民主激进化
==================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



5 Aug 2021
• 17 min read







**DAOrayaki DAO研究奖金池：**

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee /7 通过

赏金总量：170 USDC

研究种类：DAO, Quadratic Voting, radicalize democracy

原文作者:  ****Steven P. Lalley,E. Glen Weyl****

贡献者： Yofu, DAOctor @DAOrayaki

原文: Quadratic voting: How mechanism design can radicalize democracy

![](http://daorayaki.org/content/images/2021/08/----_20210426113809-2.png)Vickrey（1961）以一个项目启动了机制设计，以实现Lerner（1944）的“社会主义”福利最优梦想并且没有一个仁慈和全知的计划者。当Vickrey成为诺贝尔奖得主时，他宣布他计划利用诺贝尔奖给他的“天坛讲坛”将这一愿景带给更广泛的公众，但他不幸在几天后去世了。此外，尽管Vickrey的野心获得了一些早期追随者（Tideman and Tullock 1976）和经验（Ausubel and Milgrom 2005;Rothkopf 2007），但维克瑞自己的警告表明，他的确切计划通常是不切实际的。

因此，虽然机制设计改变了经济理论，但它提出的新机制在很大程度上被视为一系列见解深刻的理论好奇心，几乎没有实际意义，或应用在相当狭窄的环境中，例如频谱和互联网广告拍卖（Milgrom 2004;Edelman, Ostrovsky, and Schwarz 2007）。在即将出版的一本书中（Posner和Weyl即将出版），我们中的一个人旨在复兴机制设计的更激进的雄心，并提出它们可能为我们这个时代的经济、政治和社会危机提供一个解决方案。

这场危机中最引人注目的因素，或许是民主国家为解决多数与少数的冲突而进行的斗争，以及由此导致的多数或多数人主导的“民粹主义”暴政的统治。这一最古老、最持久的民主问题似乎特别适合Vickrey的方法，一方面是因为其广泛的范围，另一方面是因为其根本问题似乎恰恰是缺乏市场。

一人一票（1p1v）限制了每个选民对任何集体决定的影响力，从而阻碍了潜在的Pareto-improving贸易。当我们抱怨标准民主未能考虑到偏好或知识的强度时（Hirschman 1982），我们的意思是，它阻碍了一些公民愿意放弃他们在某些问题上的影响力，以获得对其他问题的更多影响力的交易。此外，考虑到标准的市场交换体系可能衍生为大社会中Vickrey程序的限制（Tideman and Plassmann 2017），将类似逻辑应用于公共产品似乎可以得到一个解决方案。

然而，据我们所知，在我们就这一主题开展工作之前，还没有提出一个简单而灵活的集体决策定价制度，可以适用于二元决策等常见情况。1 Groves and Ledyard（1977）和Hylland and Zeckhauser（1980）提出了选择连续公共产品的密切相关的市场体系，但选民群体很少直接选择连续公共产品。在这里，我们提出了Hylland和Zeckhauser方案的一个简单版本，用于社区重复做出二元集体决策的常见情况。与私人物品的市场体系一样，Vickrey方案的人口上限（这次是公共物品），我们将证明这是在市场达到最优的条件下，类似“价格接受”模型中实现最优性的独特的投票定价方式。

****一、价格理论模型****

考虑一个有N个选民的社会，在这个社会

![](http://daorayaki.org/content/images/2021/08/image-16.png)中出现了许多二元集体决策（例如，公民投票或领导人的选择）。为了创造市场交易的机会，每个选民都被赋予了大量的“声音积分”，他们可以用来影响这些决定的结果。正如在对私人商品市场的分析中常见的那样（Willig 1976），我们假设存在足够多的问题，并且每一个问题都足够无关紧要，以至于每个选民都有准线性的“延续价值”，为未来的投票保留声音积分。正如在公平资源分配理论（Varian 1974）中，我们假设语音信用已以相关社会认为公平的方式分配（如平等分配），即以语音信用单位最大化总等价延续价值定义了社会最优性。

考虑一些特殊的决定。把选民看到备选方案A优于备选方案B所获得的价值（以语音积分为单位）称为

![](http://daorayaki.org/content/images/2021/08/image-17.png)，负值表示偏爱B而不是A。社区投票决定哪一种选择被执行，每个选民选择一个连续的数字

![](http://daorayaki.org/content/images/2021/08/image-18.png)是积极的还是消极的取决于她喜欢哪种选择。当

![](http://daorayaki.org/content/images/2021/08/image-20.png)。每个选民支付

![](http://daorayaki.org/content/images/2021/08/image-21.png)当C是可微的、凸的、偶数的，并且在

![](http://daorayaki.org/content/images/2021/08/image-22.png)中严格增加到一个中央票据交换所时，她的声音将为她的投票加分。我们将描述C为投票定价规则。

博弈论分析将指定每个选民对价值分布的信念，并得出一个均衡策略。我们在其他地方进行这样的分析，其中涉及对信念、行为和细微统计的狭隘假设（Lalley和Weyl 2017）。我们在这里关注的是一个价格接受近似（Weyl即将发表），它似乎在更广泛的范围内是有效的（Weyl 2017），并简单地展示了核心逻辑。

因此，我们假设每个选民在决定购买多少选票时，会将额外选票的边际成本与这张选票对选举产生关键影响的可能性进行权衡。我们采用的定价假设最初由 Mueller （1973） 和 Laine （1977） 提出，是所有选民都同意这个问题的选票的边际关键性（尽管当然他们可能因问题而异）。在这种假设下，理性的选民会选择

![](http://daorayaki.org/content/images/2021/08/image-23.png)最大化

![](http://daorayaki.org/content/images/2021/08/image-24.png)。通过我们假设投票积分是公平分配的，社会希望在

![](http://daorayaki.org/content/images/2021/08/image-25.png)时准确地实施 A。我们说投票定价规则是鲁棒最优的，如果，对于每一个

![](http://daorayaki.org/content/images/2021/08/image-26.png)，

![](file:///C:/Users/user/AppData/Local/Temp/ksohtml/wpsC068.tmp.jpg)N和向量U，每个接受价格的投票者i选择投票

![](http://daorayaki.org/content/images/2021/08/image-27.png)，所以

![](http://daorayaki.org/content/images/2021/08/image-28.png)与

![](http://daorayaki.org/content/images/2021/08/image-29.png)有相同的符号。

****二、独特性****

我们的主要结果是，鲁棒最优投票定价规则集恰好是二次方规则集。

定理1：当且仅当投票定价规则为二次型时，它是鲁棒最优的。

证明：

请参阅我们的在线附录。

省略形式证明的中心思想是，二次函数是唯一具有线性导数的函数，因此，选民购买选票的唯一函数等于她的边际效益和成本，其票数与她的价值成比例。考虑一类投票定价规则

![](http://daorayaki.org/content/images/2021/08/image-30.png)对于

![](http://daorayaki.org/content/images/2021/08/image-31.png)。选民优化的一阶条件是，通过微分，

![](http://daorayaki.org/content/images/2021/08/image-32.png)如果a=2，这导致

![](http://daorayaki.org/content/images/2021/08/image-33.png)与u成正比i也就是稳健最优性。对于其他的a

![](http://daorayaki.org/content/images/2021/08/image-34.png)和

![](http://daorayaki.org/content/images/2021/08/image-35.png)不成比例，因此，对于某些值和p的安排，代价高昂的投票规则将是次优的。

相反，考虑

![](http://daorayaki.org/content/images/2021/08/image-36.png)（当投票成本趋于线性时）和

![](http://daorayaki.org/content/images/2021/08/image-37.png)（当投票成本变得非常凸时）的两个极端。在前一种情况下，对

![](http://daorayaki.org/content/images/2021/08/image-38.png)确定

![](http://daorayaki.org/content/images/2021/08/image-39.png)变成了无穷大，因此只有稍微大一点的值的选民将投票无穷大。线性投票因此导致最激烈的选民独裁，如Casella, Llorente- Saguer和Palfrey（2012）。这反映了反对投票交易的普遍直觉：允许它将导致最强烈的特殊利益集团抓住它。

在

![](http://daorayaki.org/content/images/2021/08/image-40.png)的情况下，

![](http://daorayaki.org/content/images/2021/08/image-41.png)的幂接近于0，所以所有的选民只购买他们偏好的方向的一票，如1p1v。从这个意义上说，QV是介于极端的独裁统治和多数统治之间的最优中间点。这是一票定价规则，在这一规则下，那些只想获得自己利益的选民仿佛被一只看不见的手牵着走，以促进社会的利益。我们将基于二次定价规则的投票称为二次方投票（QV），原因很明显。

****三、实际承诺****

虽然价格接受是一个有用的启发式，但它不太可能真的适用于选民行为的博弈论模型。在其他工作中，我们考虑了各种各样的模型。在Lalley和Weyl（2017）中，我们分析了博弈论文献中最典型的情况，在这种情况下，选民的价值独立而相同地从一个已知的值分布中得出，并作为理性的、风险中性的预期效用最大化者。我们证明，在适当的条件下，在所有对称贝叶斯-纳什均衡中，价格接受假设对于几乎所有的选民都是成立的，因此，随着人口增长，QV带来的福利损失一般以

![](http://daorayaki.org/content/images/2021/08/image-42.png)的速率衰减。另一个与市场平行的是，随着竞争的增长，私人商品市场向效率趋同的速度是相同的。

博弈论均衡的结构是相当微妙的，因此我们对这一结果的严格数学证明是冗长和技术性的。然而，采用我们在这种情况下严格证明的近似，适当调整，在其他情况下，并使用数值方法允许对其他环境的QV进行分析。在Chandar和 Weyl （2017） 中，我们中的一个与另一位合著者在数值上考虑了较小人群中的基线模型，并发现 QV 相对于最优值损失的福利非常小（很少超过几个百分比）点），而在 1p1v 下的损失可能很容易接近 100%。

在Weyl（2017）中，我们中的一个人使用这些近似来考虑共谋、价值分布的不确定性，以及选民不是完全理性和结果主义的可能性。在其中一些设置中，QV 的性能比我们的基线要好，而且与 1p1v 相比，它的福利损失很少超过非常小的福利损失。此外，QV的实验室实验（Goeree and Zhang 2017;Cárdenas, Mantilla，和Zárate 2014）在很大程度上与这些稳健性结论一致。虽然参与者并不像博弈论均衡所预测的那样进行精确的博弈，但投票通常与带有一些噪声的值成线性比例，导致结果比1p1v更接近最优。

这些结果都有其自身的重要局限性;有些是程式化的，或特定的实验设置，而另一些是近似的或数值的。然而，我们认为，它们具有重要的前景，因为它们说明了这个简单但（近似）最优的投票规则的稳健性。这与其他投票规则形成了对比，这些规则要么是最优的，但被广泛认为过于脆弱，无法在实践中应用，要么不是以最优为目标。

在第一类中，最著名的建议是由Clarke（1971）和Groves（1973）精炼的Vickrey的原始方案，即第一种完全最优机制。然而，这种方法对极小群体的勾结非常敏感（Ausubel和Milgrom, 2005）。它还需要大量和高度不确定的资金支出，这使得它严重依赖于使用真实货币而不是声音信贷（格林伯格，Mackay，和Tideman 1977），考虑到大多数社会的财富不平等，这种可能性可能是不公平的（劳伦斯和Sher 2017;欧博2017）。正如我们在引言中提到的，为了解决这些问题，Groves and Ledyard（1977）和Hylland and Zeckhauser（1980）提出了一种与QV密切相关的机制，但只适用于在实际应用中很少出现的持续性公共物品问题。文献中提出的其他最优机制甚至更不可靠（Weyl 2017）。鉴于此，实际的注意力主要集中在那些甚至不追求近似最优性的机制上，比如那些不允许表达偏好强度的机制（Brams and Fishburn 1978），或者类似QV但具有线性代价高昂的投票函数的机制（Casella 2005;hortala - valve 2012），从而导致最激烈的选民独裁。

QV旨在将后一组设计的简单性和实用性与第一组设计的近似最优化结合起来。这允许应用程序进行投票和调查

研究（Quarfoot et al. 2017;荷兰，2017），初步研究的证据表明，与现有的偏好诱导方法相比，该方法有了显著的改进。更高风险的政治应用（Posner and Weyl 2015）或公司治理应用（Posner and Weyl 2014）仍然具有更大的投机性，如果不在更小的范围进行进一步试验，就不可取。

****四、激进的民主，激进的市场****

然而，考虑到QV在某些意义上创造一个真正激进的民主的潜力，谨慎但越来越雄心勃勃的实验似乎是有必要的。首先，从机制上来说，QV也可以被视为个人获得的票数等于他们所花费的声音积分的平方根或根号。其次，QV触及了现代民主制度的制定者，如亚历山大·汉密尔顿（Alexander Hamilton）、孔多塞侯爵（Marquis de Condorcet）和杰里米·边沁（Jeremy Bentham）所认为的民主目标的根源：确保国家最大限度地为人民的普遍幸福服务。第三，QV从根本上扩大了公民充分、自由表达政治观点的权利，使公民从1p1v影响力配给的束缚中解放出来。从这个意义上说，它表明了机制设计如何建议社会制度的基本而又实际的改革。

然而，维克瑞的观点对私人产品和公共产品市场的贡献几乎一样多。作为亨利·乔治（Henry George）的追随者，维克瑞对私有财产持怀疑态度，他1961年出版的经典著作的核心论点是，拍卖资产可以确保资产的有效配置。另一方面，Myerson和Satterthwaite（1983）指出，从私有制开始就不可能实现配置效率。根据Vickrey最喜欢的英式拍卖方式，你可以想象很多资产（除了个人财产）被持续拍卖出租，就像互联网广告时段一样。然而，正如乔治所设想的那样，这些收入可以作为社会红利，以平等的份额返还给公众，而不是被网络平台占用。这样一个Vickrey Commons一方面将自由市场的逻辑发挥到极致，另一方面废除私有财产和大多数不平等。这是私人商品市场的本质，类似于QV的激进市场逻辑。

与直接将Vickrey的方案应用于集体决策一样，Vickrey Commons将面临许多实际挑战，而Weyl和Zhang（2017）提出的变体具有更大的实际意义。然而，作为一种思想实验，它和QV一起表明了打破困扰我们社会的左派和右派意识形态僵局的潜力。机制设计者要实现这一潜力，就必须拓宽视野，超越狭隘的应用和不切实际的理论，学会既理想又务实，灵活运用严谨，并考虑社会学、心理、法律以及由于分析的难易性，他们历来回避的其他因素。在这里，我们试图简要说明这种方法的挑战和前景。



---

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）  
  
详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)  


历史文章：

[DAOrayaki｜二次方投票和区块链治理](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485046&idx=1&sn=21c5550753bb5405ba838eeb7857f2d6&chksm=c1d807a3f6af8eb57ebb1ad7a1b1ba8079ed40e4f60ef36d11930d472d233c8ee3d7b6b88ac3&scene=21#wechat_redirect)

[DAOrayaki｜可追溯公共物品融资](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485099&idx=1&sn=59c46a5a5b44dbf3c74c902a2d7c33bd&chksm=c1d8077ef6af8e68247e4557d52e8c7435563ebc25aef988f9986f8881eb244a12a360c82303&scene=21#wechat_redirect)

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





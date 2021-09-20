

DAOrayaki | Gas成本和选民参与
======================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



18 Sep 2021
• 9 min read







**DAOrayaki DAO研究奖金池：**

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 4/7 通过

赏金总量：70  USDC

研究种类：DAO, Costs and Participation,Gas costs，

原文作者：Tally

贡献者：Dewei, DAOctor @DAOrayaki

原文： Gas Costs and Voter Participation

![](http://daorayaki.org/content/images/2021/09/image-65.png)协议治理机制的选择对协议的成功和未来的发展路径有很大的影响。在诸如 Compound 的 Governor Bravo 之类的链式治理框架上，允许对提案结果进行无信任执行，这提供了更大的去中心化，但需要用户支付交易费用才能参与。另一方面，像 Snapshot 这样的链下投票机制支持自由投票，但不能自动执行，并且涉及额外的信任假设（例如，信任多重签名以正确跟踪投票结果）。

协议必须权衡更多参与的好处与中心化风险。但在他们开始考虑这种权衡之前，他们需要更好地了解交易成本和Gas如何影响参与链上协议。客座贡献者 Raphael 提供了一个数据驱动的分析，其中有一些关于去中心化协议的惊人发现。

![](http://daorayaki.org/content/images/2021/09/image-66.png)**投票成本会影响治理参与吗？**

我们试图通过数据优先的方法来回答这个问题。下面我们将分享我们的发现并量化交易成本与投票之间的相关性。

如果您对方法论不太感兴趣，可以跳到下面的结果部分。

**总结**

交易成本会影响治理参与，但只有超过 10 美元才会显著影响。

在我们包含 110 个提案和 5000 多张选票的整个数据集中，投票成本仅占差异的 2%。换句话说，没有相关性。

然而，过滤掉平均成本低于 10 美元的提案会使相关性增加到 7%。进一步过滤掉低于 20 美元的提案，相关性进一步提高至 18.5%。

总之，成本确实会影响参与度，随着成本的增加，参与度的影响会越来越大。然而，18.5%仍然客观上较低，表明其他因素的影响更大。

**了解更多分析过程，请看此部分。**

实验设计：弄清楚如何量化交易成本和治理参与之间的关系。

我们的研究涵盖了五个 DAO 的提案。他们分别是：

lCompound

lIdle

lIndexed

lInverse

lPool Together

我们在每个DAO中收集个人投票数据，并按提案对其进行分组。

为了量化投票参与和交易成本之间的相关性，我们首先需要定义这两个变量。

**定义提案参与**

我们将给定提案的治理参与定义为：

投出的选票数量 / 对同一 DAO 中的单个提案投出的最大选票数量

这种简单的方法有助于控制 DAO 在规模和参与度方面的自然差异。结果是一个简单的百分比，用于捕获给定提案的参与。

**定义交易成本**

我们的下一步是定义交易成本。研究的所有 DAO 都在以太坊上，我们可以用 Gwei 计价交易成本。然而，考虑到以太坊的波动性和标准化指标的愿望，我们选择以美元计价交易成本。

一个怪癖是我们无法收集交易中使用的确切Gas（我们只能收集Gas限制）。

这使得我们声明的交易成本高于选民实际花费的金额。然而，鉴于选民设定了限额，我们认为这代表了选民愿意支付的金额。

**结果**

有了我们的数据集，我们就可以进行分析了。我们首先查看所有数据点。

![](http://daorayaki.org/content/images/2021/09/image-67.png)正如您所料，趋势线显示，随着投票成本的增加，参与度下降。然而，当我们查看实际的相关性时，它揭示了一个不同的故事。

皮尔逊系数只有 2%，这基本上意味着没有相关性。

一种想法是，当名义投票成本很小时，变化不应该对参与产生影响。例如，我们是否应该期望 5 美分的差异会影响参与度？

包括这些低投票价格会给数据集带来很多噪音，降低整体相关性。

在这里，我们删除了平均投票成本低于 10 美元的所有提案。而且，我们实际上看到 皮尔逊系数增加了三倍以上，达到 7%。

![](http://daorayaki.org/content/images/2021/09/image-68.png)按照同样的思路，我们可以假设从 10 美元到 10.50 美元的变化不应该影响参与率。

下面，我们删除了平均投票成本低于 20 美元的所有数据点。再次，我们看到 Pearson 系数，这次一直到 18.5%。

![](http://daorayaki.org/content/images/2021/09/image-69.png)**那么，我们如何解释这些不同的观点呢？**

无论我们是否按投票成本过滤参与数据，我们都会看到两个一致的结果：

1.所有图表都显示负趋势线，并且

2.所有图表都显示了相当低的 R2 值。

直觉上，低于某个阈值，交易成本的变化不会影响参与。因此，过滤掉低于某个数量的提案是合适的，指出对参与度下降的贡献介于 11% 到 18.5% 之间。

尽管如此，这是一个相当低的皮尔逊平方值，并强调了存在许多混杂变量的现实。

可能的例子包括提案的重要性、协议的当前流行度、协议的大小和日期等。

**自己探索数据**

我们创建了一个交互式仪表板，您可以在其中自己处理数据。

您可以按 DAO 进行过滤，以查看协议的参与如何单独关联。具有讽刺意味的是，Inverse 的参与实际上是负相关的（随着交易价格的上涨，参与也随之增加）。

此外，您可以通过平均投票成本来限制数据集中包含哪些提案。

**下一步**

为了加深我们对参与成本影响的理解，我们应该丰富我们的数据集。

一些想法包括：

1.按通过的票数分割地址

2.在无Gas/无成本环境中引入控件，例如 Snapshot

3/引入措施来控制活动代表随时间推移的漂移

**构建数据库，添加更多 DAO、提案和价格点**

最终，如果 DAO 想要最大限度地参与，他们应该承认交易成本的影响，并考虑在高交易成本环境中减轻影响的方法。但与此同时，重要的是不要夸大Gas成本的影响，因为可能有更重要的选民参与驱动因素。某些缓解措施，例如使用无Gas fee链下投票和用于提案执行的多重签名，会损害安全性和去中心化。因此，对于 DAO 来说，重要的是要考虑收益是否大于风险。



---

DAOrayaki 是一个去中心化的研究者组织和去中心化媒体，通过 DAO的形式去中心化地资助世界各地的研究者进行研究、翻译、分析等工作。DAOrayaki 由早期的 DAO 组织 DAOONE 核心成员发起，得到了Dora Factory基础设施的支持。

  
了解去中心化自治组织（DAO），探讨最新治理话题，关注DAO的发展趋势，欢迎加入群聊！

![](http://daorayaki.org/content/images/2021/09/image-70.png)欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！

欢迎访问DAOrayaki官网（daorayaki.org）

详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)

历史文章：

[DAOrayaki｜算法治理实验：DAO治理动态、韧性及崩溃](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485358&idx=1&sn=88d00171a6eccee2fdc8281a8365b73c&chksm=c1d8067bf6af8f6dc6d10bcfc145df75b304b2b719781484864d65a55a625b09e12d77e9dffd&scene=21#wechat_redirect)

[DAOrayaki｜打破媒体第四面墙：观众和创作者的融合](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485358&idx=2&sn=ac525be0573245c5bf63dca3ea62185d&chksm=c1d8067bf6af8f6d4349154c2d4b7ea9b80c4c2657c2eb86dc6ab90652538241d4e367afda7e&scene=21#wechat_redirect)

[DAOrayaki｜新媒体结构：所有权经济](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485357&idx=2&sn=d780f8d94fca85530842876fa190b3a9&chksm=c1d80678f6af8f6eae4fa9e31709693211b8623cd169a636012ed4fc1d6ef1c9b5338f01740d&scene=21#wechat_redirect)

[DAOrayaki｜Loot: 从文本文件到完全去中心化的社区](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485357&idx=1&sn=6f646a93d909d6d1187dd7a80fb350a4&chksm=c1d80678f6af8f6e5fcb224e6fdecf9b0c38f59a7dacbf2559eefb588c3536929bae503c16d0&scene=21#wechat_redirect)

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





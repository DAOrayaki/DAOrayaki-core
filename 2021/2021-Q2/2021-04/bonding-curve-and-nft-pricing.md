


[DAOrayaki](/tag/daorayaki/)

价格发现的艺术，嵌套的策展市场，当联合曲线遇到NFT
==========================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



11 Apr 2021
• 13 min read






![价格发现的艺术，嵌套的策展市场，当联合曲线遇到NFT](/content/images/size/w2000/2021/04/-----2021-04-11---6.25.55.png)



**DAOrayaki DAO研究奖金池：**

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee 6/7 通过

赏金总量：100 USDC

研究种类：Bonding curve token／Liquidity token／NFT pricing/Auction

贡献者：義理の姉@DAOrayaki

Reference: Billy Rennekamp,Jade and Sanchez@BES, Simon de la Rouviere等

**前言：**

  
在传统的框架中，有三种力量主导着资源分配，市场，政府和第三部门（道德、宗教、非营利组织）。在一个市场经济社会里，几乎所有的东西都可以被定价和交易，一个常见的理论是均衡价格处在供需曲线的交点，在二级市场上，价格的发现变得稍微复杂，至少要考虑时间因素、多空双方的势力、流通盘和交易深度等。**而联合曲线模型是通过【买卖函数】发行通证的合约，****联合曲线模型可以理解为描述“买卖价格”与“发行总量”间的函数关系，形成的“价格-发行量”曲线。**也可以理解为是一种以智能合约的方式自动执行的一种自动做市商。  


**联合曲线（Bonding Curve）本质上是什么？**它的本质是在链上环境中建立一个去中心化的协作机制，融合了时间、交易对手、盘面、深度、价格等多重要素，由算法来负责整个协作机制内的资源的分配。目前，在理论层面还需要大量的有关市场经济，公共物品分配等经济问题的研究，来解决包括sybil attack（女巫攻击），front running（提前下单），fork（分叉）等问题。但毋庸质疑，联合曲线为我们提供了一个全新的视角。

最近被Dorafactory收购的PentaLaunch就是一个联合曲线拍卖市场（bonding curve auction platform），目前它的主要用途是为了开源项目筹资。DAOrayaki去中心化研究组织认为，**对于NFT的定价来说，策展市场(curation market）将是这种联合曲线模型的最重要的应用领域之一****，**不过可能不是连续曲线，而是离散曲线。

![](http://daorayaki.org/content/images/2021/04/penta1.jpeg)**今天，我们将介绍一个新的概念，Re-Fungible Token（可重新同质化的通证）。**当艺术品、收藏品这些链下资产都已经被数字化变成了NFT（非同质化通证），可以在DeFi世界被重新拼接、组合时，对于它们的定价机制，我们绝不该再拘泥于传统的策展和拍卖的思维窠臼。

**当Re-Fungible Token遇上联合曲线**

**Core Author：Billy Rennekamp**

**Reference：每个应用类Dapp的经济系统必修课——联合曲线（Token Bonding Curve），联合曲线：通证发行方式的创新型探索 | ONE.TOP评级，Curation Market等**

本文的重点是探索**使用ERC20联合曲线通证（Simon de la Rouviere，Bonding Curve Token)或流动性通证（Bancor，Liquidity Token)作为ERC721标准的NFT的所有者地址。**和过往一个特定的人拥有一个特定的NFT不同，人们可以持有一定数量的同质化通证，而这代表了他们拥有一个原始的NFT。我觉得这对艺术品、知识产权和数字付费的策展市场会很有帮助。

**联合曲线和流动性通证（Bonded Curves & Liquid Tokens）**

有一种特殊类型的ERC20通证，允许用户直接买卖在智能合约上进行买卖，Simon de la Rouviere称之为bonded curve tokens，Bancor称之为liquid tokens，两者都是指一个智能合约，它接受用ETH或另一个EC20 token，换取铸造成某种新通证的面额。

Simon de la Rouviere的版本是根据曲线命名的，图中的曲线表示每个通证的价格（y轴）与流通中的通证数量（x轴）通过预定义的斜率公式结合在一起。**斜率可以是线性的、指数的、对数的或完全任意的**，这取决于用例，但最常见的情况是价格随着流通中通证的数量而增加。

这里普及一下联合曲线的数学内涵（引用自《[每个应用类Dapp的经济系统必修课——联合曲线（Token Bonding Curve](https://mp.weixin.qq.com/s?__biz=MzUzOTc0MzE2Nw==&mid=2247483815&idx=1&sn=2cf2f4bd05ebe208b8a056f9a58dabc3&scene=21#wechat_redirect)），首发区块律动》：

关于联合曲线的函数形态，其种类和设计唯一受限的只有人类的想象力了。Bancor协议是第一套从价格函数到交易定价整体数学推演完备的一种设计思路。

**买入和卖出函数不相同的线性函数**

以这种机制为例，对于每次卖出收取手续费的 30%。假设买入曲线是简单的线性函数 y = x。则卖出函数 y = (1-30%)*x = 0.7x。两条曲线的简单形态就如下图所示：

![](http://daorayaki.org/content/images/2021/04/-----2021-04-11---7.30.23.png)![图片](data:image/gif;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVQImWNgYGBgAAAABQABh6FO1AAAAABJRU5ErkJggg==)**买入卖出函数相同的类线性函数**

凸函数曲线类型（包括指数类型）

![](http://daorayaki.org/content/images/2021/04/-----2021-04-11---7.30.45.png)凹函数曲线类型（Logarithmic类型，反函数类型，类多项式类型）

![](http://daorayaki.org/content/images/2021/04/-----2021-04-11---7.46.55.png)**内涵：**其中a与c代表在通证数量每翻c倍时，通证价格增长a%。m和b作为线性函数参数调节截距和斜率。以上面的公式为例，这条特定的函数曲线代表了通证数量每次翻倍时，价格增长25%。

**联合曲线通证和策展市场（Bonded Curve Tokens & Curation Markets）**

这些联合曲线通证主要是描述在策展市场中使用，其中通证的价格可以代表一个主题的流行程度。一个例子是趋势预测（Trend Forecasting），可以通过买卖代表不同趋势的不同通证来进行。预测某一风格成功的人可能会购买通证，期望随着该风格声名鹊起，更多人追随。随着新铸造的通证为早期采用者创造利润，价格将随之上涨。与预测市场类似，它通过经济激励措施，汲取“大众智慧”。

**流动通证和做市商（Liqui****d Tokens & Market Makers）**

Bancor将这项技术称为流动通证，强调通证始终可以以任何数量被购买或出售。它们将买入面额（buying denomination）和卖出面额（selling denomination）之间的关系确定为存款准备金率。低于1/2的比率呈指数增长，高于1/2的比率呈对数增长，1/2的比率呈线性增长。购买的价格是根据通证的总供应量、基础准备金的数额和预先确定的存款准备金率来计算的。

**Bancor的目标是支持那些在传统交易所没有足够数量的买卖订单（缺乏交易深度和流动性）的长尾通证。**通过鼓励使用自己的Bancor网络通证（Bancor Network Token）作为普通买入面额，他们可以提供不同通证之间的交换。  


**可以重新同质化的通证（Re-Fungible Token，RFT）**

最后，我们可以开始思考我最初提出的实验：**如果一个ERC721 NFT被一个ERC20 Bonded Curve Token/Liquid Token的地址所拥有，会发生什么**？

从本质上讲，非同质化资产将再次成为同质化资产。这些同质化通证的铸造和非铸造（unminting）将绑定到预先定义好的的价格曲线上。

**最终有可能证明NFT的部分所有权，就像通过标准ERC20接口证明通证所有权一样。**如果我是一个钱包，我可以查看NFT的数字资产注册表（Digital Asset Registry，DAR），看看谁拥有它。然后，我可以检查所有者的地址，看看它是否真的是一个RFT合同。如果是这样，我可以使用balanceOf函数检查某个地址是否拥有一定数量的RFT令牌，并验证原始NFT的部分所有权。  


根据具体情况，可以通过代表资产的每个通证的价格来收集一些信号。**一个价格非常高的RFT必须代表一些预期的高质量，比如一副名画，一个知名IP，才能有这么多的用户愿意购买它。**这些用户可能是理性的参与者，他们期望从通证的进一步增长中获取利润，也有可能他们是这个IP的铁粉（感性支持者），而不管他们的投资效果如何。从每个通证的价格中获得的信号可能会有所不同，这取决于它所代表的NFT的类型。  


**策展市场中的艺术**

毫无疑问，信息不对称在艺术品市场上非常猖獗。这种情况在很大程度上有利于经销商和拍卖行，他们通常能够通过锁定价格，故意制造稀缺来利用更大的卖价来销售作品。  


将NFT艺术品与联合曲线的Re-Fungible通证挂钩将创建一个新的交易系统，在这个系统中，艺术品的价值会随着联合曲线上的策展市场不断更新价格。这种系统可以创建出一个有利于艺术家的机制，而有敏锐品味的投资者会通过精明的收购获得收益。**艺术家们也可以类似地投机或预先造币（****pre-mint****），或利用****RFT****上的通货膨胀来获得可持续的收入来源。**在通货膨胀的情况下，买卖曲线上可能有一个价差，两者之间的差额将不断地支付给作品的作者，或者在每次交易中有一个简单的固定费用。这样基本上，艺术家每次卖出作品都会赚钱。

![](http://daorayaki.org/content/images/2021/04/Penta2.jpeg)当然，这种情况可能会产生更多的问题，而不是答案。**艺术品特定通证的价格在多大程度上反映了该作品的质量？如果一件艺术品只能由一个集体所有，那么它在概念上意味着什么？这会导致或多或少的艺术道德消费吗？价格多少波动？**

  
**嵌套的投资市场（Nested Investment Market****）**  


在这种背景下的策展市场是嵌套（nested）的，每个Bonding Curve Token在铸造时接受一些基本面额（base denomination）。这种基本面额可以是ETH，类似于DAI的稳定币或任何其他ERC20通证，包括另一种Bonding Curve Token。

一个艺术品NFT，在我们的市场下将反映多个不同层面的定价要素。在一个层面上，可能是一种通用投资通证（GIT，general investment token），与ETH或稳定币绑定。这个GIT可以用来购买不同的数字资产池（DARTs，Digital Asset Registry），这些通证可以代表整个NFT类型；

![](http://daorayaki.org/content/images/2021/04/-----2021-04-11---8.42.27.png)想象一下一个CryptoKitty DART、一个名人DART和一个CryptoPunk DART。最后一级将是RFT（Re-Fungible Token），与DART一起购买，代表单个NFT的部分所有权。

![](http://daorayaki.org/content/images/2021/04/-----2021-04-11---8.47.40.png)NFT绑定的价格——RFT——应该标志着单个艺术品的成功，DART——标志着整个某种类型的NFT池的成功，GIT——标志着整个系统的成功。

**以上的嵌套模型详情可以参考文章：Continuous Token-Curated Registries：The Infinity of Lists，****Solving Price Discovery Of Non-Rivalrous Goods (with Curved Bonding)，******解决非竞争性商品的价格发现问题**（感兴趣的可以翻译并给DAOrayaki投稿）**

**下一步是什么？**

所有这些场景都需要大量的实验，因为有很多问题没有答案。创建一个高效的系统需要哪些参数？支付需要多少通证？这个数字会随着时间的推移而改变吗？价格曲线应该如何设定？什么程度的通货膨胀为通证创始人提供了足够的报酬，同时提供了有吸引力的投资机会？这些通证可能涉及的合规问题？

当艺术品、收藏品这些链下资产都已经被数字化变成了NFT（非同质化通证），可以在DeFi世界被重新拼接、组合时，对于它们的定价机制，我们绝不该再拘泥于传统的策展和拍卖的思维窠臼。希望这篇文章对你有所启发。

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！

详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)  


历史文章：

[深度回顾币安智能链BSC Grant HackerLink第一期](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484046&idx=1&sn=72f298e4d41833d6f39340deed5bf424&chksm=c1d8035bf6af8a4de7934291b2f6cff23bd0f808b57d65ccc177266bdf7649516e103cf35cbe&scene=21#wechat_redirect)

[Futarchy | 价值投票，对赌信仰，用钱说话，口说无凭](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247484004&idx=1&sn=433b36bc5b077011f5abdd8b83c802b2&chksm=c1d803b1f6af8aa74094f3c2d14ca2b9d22d807a5fdc4374cbe6f5f55b8e33d585d61604f07e&scene=21#wechat_redirect)

[平行世界｜DeFi无缝集成全球最性感资产—BTC，特斯拉和茅台](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483954&idx=1&sn=d0a5a470a969e9aa9d9f6a6b2bb89232&chksm=c1d803e7f6af8af1574df947cb8be6710937f0a5f30978c255acf81ec02b989b86d184a2e205&scene=21#wechat_redirect)

[「激进市场」和二次方投票 | 用市场本身去监管市场](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483861&idx=1&sn=4e8b5b58a53a942df10fd7e38147ae61&chksm=c1d80000f6af8916f92328a4dc051a92c6836fe6b35bdd762dcb002e944d7663a94b63254e59&scene=21#wechat_redirect)

[Dora Factory：重建22世纪松芝工厂](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=4&sn=58246e8d0028edc9dab7a65f6505dc7f&chksm=c1d80075f6af89631c8b83eba862b458f7f115ce9f4377efa6777a6d601704db14aff68371fe&scene=21#wechat_redirect)





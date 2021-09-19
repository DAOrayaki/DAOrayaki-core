

DAOrayaki｜关于改善配对协调补贴的一个方法探讨
===========================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



16 Aug 2021
• 18 min read







### DAOrayaki DAO研究奖金池：

资助地址: 0xCd7da526f5C943126fa9E6f63b7774fA89E88d71

投票进展：DAO Committee /7 通过

赏金总量：150 USDC

研究种类：DAO, Pairwise Coordination Subsidies

原文作者:  Zoudavid 讨论者：Vitalik、Vbuterin、Peter Watts

贡献者： Demo, DAOctor @DAOrayaki

原文: A Proposal to Improve Pairwise Coordination Subsidies

![](http://daorayaki.org/content/images/2021/08/----_20210426113809-7.png)****1. 背景介绍****
---------------

自2018年以来，Vitalik一直主张二次方融资（QF）作为一种在去中心化的、自组织的生态系统中生成最优公共产品供应的方法（Buterin、Hitzig和Weyl, 2018）。QF面临的最具挑战性的问题之一是共谋。例如，一个参与者或一组协调的参与者可能控制多个地址或共谋“游戏系统”，并在QF中提取不合理的补贴。

自2019年以来，Gitcoin Grants已经运行了多轮的QF。Gitcoin Grants使用了一种创新的方法：****双界协调补贴（pairwise-bounded coordination subsidies）****（Buterin，2019）。然而，Zoudavid认为Buterin（2019）中的不协调系数（discoordination coefficient）的说明不是很直观，也不太令人信服。此外，Buterin（2019）中的可调整参数（tweakable parameter）主要用于约束任何一对投资者的可提取价值，但在调整他们之间的共谋方面做得不够。在《关于改善配对协调补贴的提议》（**A Proposal to Improve Pairwise Coordination Subsidies**）一文中，Zoudavid提出了一种新的方法来改进具有丰富经济意义的配对协调补贴（pairwise coordination subsidies）。

****2. 不协调系数的一种新规范****
----------------------

采用Buterin(2019)的符号，Zoudavid提出了一种新的不协调系数的规范：

![](http://daorayaki.org/content/images/2021/08/image-71.png)其中

![](http://daorayaki.org/content/images/2021/08/image-72.png)是向量i和j的不协调系数，

![](http://daorayaki.org/content/images/2021/08/image-73.png)以及

![](http://daorayaki.org/content/images/2021/08/image-74.png)表示投资者i和j对项目p的投资，

![](http://daorayaki.org/content/images/2021/08/image-75.png)是所有项目的总和。不协调系数衡量的是衡量的是一对投资者在作出投资决策时的独立性。有两种视角来理解等式（1）的经济含义。

一种视角是，考虑两个向量

![](http://daorayaki.org/content/images/2021/08/image-76.png)以及

![](http://daorayaki.org/content/images/2021/08/image-77.png)，其中p表示项目的总数。

令

![](http://daorayaki.org/content/images/2021/08/image-78.png)表示向量的模：

![](http://daorayaki.org/content/images/2021/08/image-79.png)令

![](http://daorayaki.org/content/images/2021/08/image-80.png)表示两个向量的内积，

![](http://daorayaki.org/content/images/2021/08/image-81.png)令

![](http://daorayaki.org/content/images/2021/08/image-82.png)表示两个向量之间的角度，则有，

![](http://daorayaki.org/content/images/2021/08/image-83.png)如果这两个向量是正交的（如，

![](http://daorayaki.org/content/images/2021/08/image-84.png)），那么

![](http://daorayaki.org/content/images/2021/08/image-85.png)并且

![](http://daorayaki.org/content/images/2021/08/image-86.png)从(1)-(4)，很容易可以看出，

![](http://daorayaki.org/content/images/2021/08/image-87.png)对于(5)来说，先考虑两种比较极端的案例。

****案例#1：****对于每一个p

![](http://daorayaki.org/content/images/2021/08/image-88.png)，这意味着和没有共有的投资，这就符合

![](http://daorayaki.org/content/images/2021/08/image-89.png)![](http://daorayaki.org/content/images/2021/08/image-90.png)（如，正交的向量）。在这个例子中，

![](http://daorayaki.org/content/images/2021/08/image-91.png)，意味着i和j有最大的不协调性。

****案例#2：****如果存在一个

![](http://daorayaki.org/content/images/2021/08/image-92.png)使得对于每一个p，有

![](http://daorayaki.org/content/images/2021/08/image-93.png)，这意味着i和j做了同样的投资决策。尽管他们可能有不同的投资金额，但有相同的资产配置决策的百分比。这符合

![](http://daorayaki.org/content/images/2021/08/image-94.png)![](file:///C:/Users/user/AppData/Local/Temp/ksohtml/wps6C20.tmp.jpg)的情况（如，同一方向的向量）。在这种情况下，

![](http://daorayaki.org/content/images/2021/08/image-95.png)，也就是和有最大的协调性。

其他的例子都落在案例#1和#2之间：

![](http://daorayaki.org/content/images/2021/08/image-96.png)在0和

![](http://daorayaki.org/content/images/2021/08/image-97.png)![](file:///C:/Users/user/AppData/Local/Temp/ksohtml/wps6C45.tmp.jpg)之间，即

![](http://daorayaki.org/content/images/2021/08/image-97.png)因此，

![](http://daorayaki.org/content/images/2021/08/image-98.png)******在0到1之间。******

![](http://daorayaki.org/content/images/2021/08/image-99.png)******越大，不协调性越大****。**

另外一种视角是从概率论的角度理解

![](http://daorayaki.org/content/images/2021/08/image-100.png)的含义。在事前，每个投资者的投资决定都是一个随机变量。因此，向量

![](http://daorayaki.org/content/images/2021/08/image-101.png)分别是i和j的事后现实的投资决策。在等式(1)中，

![](http://daorayaki.org/content/images/2021/08/image-102.png)只是对他们的投资决策之间的相关系数进行了抽样估计。****协调系数越大，不协调系数就越小。****

****3. 不协调系数调整后的补贴****
----------------------

对于项目p来说，在协调调整过i和j的补贴是

![](http://daorayaki.org/content/images/2021/08/image-103.png)当

![](http://daorayaki.org/content/images/2021/08/image-104.png)或者说i和j是完美协调（perfect correlated）时，这个补贴为0。

从等式(6)，Zoudavid定义了i和j从所有项目中提取的不协调系数调整后的补贴（discoordination adjusted subsidy，DAS）为

![](http://daorayaki.org/content/images/2021/08/image-105.png)值得指出的是，要用(1)估计

![](http://daorayaki.org/content/images/2021/08/image-106.png)，可以使用前几轮二次方融资的样本数据，而不仅仅是本轮。这样，可以使不协调系数的估计更稳健，并减少对当前样本量的限制。

****4. 对配对边界的调整****
-------------------

假设对于任何一对投资者从所有项目中提取的总补贴引入一个上限。设B是普遍适用的上限。类似于Buterin（2019）中的可调整参数。

给

![](http://daorayaki.org/content/images/2021/08/image-107.png)加上上限B：与Buterin（2019b）相似，Zoudavid使用了下面的公式：

![](http://daorayaki.org/content/images/2021/08/image-108.png)显然，

![](http://daorayaki.org/content/images/2021/08/image-109.png)同样与Buterin（2019）类似，如果存在总补贴的特定水平，需要在满足下列约束的情况下求解出B（是投资者总数）：

![](http://daorayaki.org/content/images/2021/08/image-111.png)用数值方法不难求出等式(9)的解。

****5. 与现有方法相比****
------------------

考虑一种情况：i和j做出了同样的投资决策（如，存在一个

![](http://daorayaki.org/content/images/2021/08/image-112.png)使得对于每一个p

，有

![](http://daorayaki.org/content/images/2021/08/image-113.png)）。用Zoudavid的方法，他们将不会得到任何补贴。但用目前的方法，他们可以获得大量的补贴，只是被可调整的参数所缩减。

用Buterin（2019）中描述的景象举例。假设K个经过协调的代理人都向一个项目贡献了一笔很大数额的资金w。由于他们是完美协调的，用Zoudavid的方法他们可以提取的资金是0。然而，用现存的方法他们可以提取的资金是

![](http://daorayaki.org/content/images/2021/08/image-114.png)，其中M是可调整的参数。

Vitalik建议了这样一种情况：假设有两个赠款者A和B和三个项目A，B和C，其中有相同字母的捐赠者和项目对是相互串通的。现在假设A捐赠了X 0 X，以及B捐赠了0 X X。

在这个例子中，

![](http://daorayaki.org/content/images/2021/08/image-115.png)。如果使用过去几轮二次方融资的数据，

![](http://daorayaki.org/content/images/2021/08/image-116.png)可能会有不同的估计，而且可能会更准确。

不协调系数调整后的补贴是

![](http://daorayaki.org/content/images/2021/08/image-117.png)，这正好是当前方法的一半水平。在把上界纳入考虑之后，总的补贴是B*X/B+X。用当前方法，总的补贴是

![](http://daorayaki.org/content/images/2021/08/image-119.png)****从上面的例子中可以清楚地看到，在当前的方法中，没有对不协调的调整，只有对边界的调整。****

****6. 针对该方法的多方观点****
---------------------

****（1）优势****

Vbuterin认为该提议是非常有趣的洞见，其有趣之处在于用点积（dot product）来直接估计多个协调者之间的不相关关系。

****（2）存在的不足****

一方面，Vbuterin认为，本质上来说，任何一个代理人A总是可以通过简单地创建一个项目并对他自己和代理人B进行一笔大金额的捐赠来提高他和B的不协调系数。如果每一个A都创建一个项目

![](http://daorayaki.org/content/images/2021/08/image-120.png)，那么其点积就不会受到任何影响。因为不会有其他的人向

![](http://daorayaki.org/content/images/2021/08/image-121.png)捐赠，但这会增加他们的

![](http://daorayaki.org/content/images/2021/08/image-122.png)价值到无限大，使得分式为0并且对于所有的j来说

![](http://daorayaki.org/content/images/2021/08/image-123.png)Vbuterin提出了约束的相关系数（bound-based correlation coefficient），其属性是，两个参与者向同一个项目捐赠会增加他们的相关分数（correlation score），但两个参与者向不同的项目捐赠不会减少他们的相关分数。他认为如果Zoudavid想有一个系统，其中两个参与者捐赠给不同的项目将减少他们的相关分数，那么需要以某种方式击败发送至自身的攻击（send-to-self attack）。

而Zoudavid有针对性地提出，发送至自身的攻击（send-to-self attack）并不会带来很大的问题。并给出了三点理由。

首先，自发送攻击代价高昂，因为攻击者需要在他的“假”项目中锁定大量资金。而与此同时，其回报将是有限的。假设攻击者创建了一个只有他投资而没有其他投资者投资的项目。的确，通过增加对这个项目的投资，他可以增加对他和其他投资者之间相关性的估计。然而，他可以从他的“假”项目中提取的补贴仍然是0。对于其他项目，由于攻击而增加的补贴应该是非常有限的，而且这种增加不能被攻击者独享。

其次，在计算不协调系数时，可以简单地排除任何只有一个投资者的项目。例如可以认为这些项目融资失败，没有资格获得QF补贴。在法币众筹中，通常有一个门槛机制：任何一个项目在一定时间内无法获得足够的支持或资金承诺将被认为是失败的，之后任何资金承诺将被返还。Zoudavid认为QF可以纳入类似的机制。

最后，可以利用前几轮QF的数据来估计不协调系数，使其估计受单个数据点的影响更小。

另一方面，Peter Watts察觉到协调惩罚（Coordination penalties）似乎依赖于一个假设：诚实的用户会将资金分散到多个项目中，完美地反映出他们的偏好（即按比例为每个他们将获得价值的项目提供资金）。而实际上，他怀疑许多用户会因为方便或强烈的偏好而只投资一小部分。因此，真正的公共产品将会有很多高度相关的资助者，而得不到足够的补贴。

****（3）进一步探讨****

Vbuterin提出了一个方法，就是将重点再移开一步，不关注项目本身，而是关注向同一项目捐赠的一对捐赠者，并提出用3条规则来判断：

1. 如果代理人i和j都向项目p捐赠那么他们是更加相关的；

2. 如果代理人i和j都向项目p捐赠，而存在某个代理人k也是都捐赠了p和q，那么i和j是更加相关的；

3. 如果代理人i和j都向项目p捐赠，而存在某个代理人k只捐赠了p或者q中的一个，那么i和j的相关性变弱。

规则（3）将在所有代理中进行汇总，因此，捐赠给你自己的项目比捐赠给其他100人也捐赠的项目所带来的不相关要少得多。

Vbuterin提出用更复杂的矩阵乘法的使用来描述这个问题。如果M是一个（非正方形）矩阵，将个人贡献的平方值映射到项目上，那么

![](http://daorayaki.org/content/images/2021/08/image-124.png)会给出个人之间的原始相关性，然后可以做一些其他的事情来计算出高阶测量，但是这个方法需要进一步考虑。

针对Vbuterin“高阶相关测度（higher-order measures of correlation）”的建议，Zoudavid做了一些初步的研究。基本上，除了不同投资者之间的相关性，还应该考虑不同项目之间的相关性。就像协调的投资者倾向于做出相似的投资决策一样，相关的项目也倾向于吸引相似的投资者群体。在利用投资数据估计投资者之间的相关性时，应该意识到项目之间的相互依赖性。对于此，Zoudavid提出奇异值分解（Singular Value Decomposition，SVD）是研究这一问题的合适工具。然而，该解决方案可能过于复杂，难以与投资者社区沟通。此外，解决方案可能容易过拟合。

Peter Watts认为当试图减少欺诈时，最重要的是不要失去CLR的核心租户。在完全基于协调惩罚的局部最大值确定之前，可能还有更多的机制可以探索，要么补充协调惩罚，要么取代它们。衡量成功的标准不应仅仅是减少欺诈的程度，还应是资金分配到真正的公共产品的程度。针对这个问题，他提出了几个想法：

****1. 负的偏好（Negative preferences）****

对于每个用户来说，项目实际上可以分为三类：

A)我愿意资助的项目（高价值感知）

B)我没有资助的项目，但不介意他们是否得到补贴（小价值感知）

C)我不想要补贴的项目（没有/负价值）

目前，还没有办法区分B和C。也许UI可以允许用户对某些项目投反对票（downvote），这些信息会影响补贴。其反对票只会影响没有资助的项目之间的补贴分配。因此，否决所有其他项目就相当于否决零。而这源于这样一个现实，即用户不会为每一个能让他们受益的项目提供资金。公共产品的本质是，它们中的许多人都喜欢给予小的、间接的好处，因此更容易识别那些明显是欺诈性的或不可能以任何方式使之受益的项目。

****2. 给一些独特贡献者更高的权重****

大多数攻击通过贡献大量的资源来利用执行超额影响的能力。这是因为在一个抗女巫攻击的系统中，它比捐助者更容易积累资金。因此，降低“假”项目有效性的一个简单方法是，为有更多贡献者的项目提供更高的补贴。这限制了强烈偏好的影响，但值得权衡。

一个极端是，有CLR，它允许强烈的偏好，但很容易被共谋。另一个极端是，可以根据一个项目收到的独特贡献者的数量来划分补贴。Peter Watts的想法是用一个系数来选择这个光谱上的最佳点。

****7. 结论****
-------------

为解决在去中心化自治组织中最优公共产品供应的方法中存在的共谋问题，在Buterin（2019）提出了配对协调补贴的基础上，Zoudavid提出了一种新的方法对这一具有丰富经济意义的配对协调补贴进行了调整和改进，他提出了一种新的不协调系数的规范，并对配对边界进行了调整，使得估计结果更加稳健。其与当前现有的方法相比，在对不协调进行调整之外，还对边界进行了调整，使得补贴更为严格。该方法用用点积来直接估计多个协调者之间的不相关关系，是一个突出亮点，但也同时存在潜在的应对发送至自身的供给的问题，以及真正的利益相关者得不到足够补贴的问题。针对这一方法，还有很多值得探讨和进一步深入挖掘的方向，包括“高阶相关测度”和惩罚协调的机制等。

****参考文献****
------------

[1] Buterin, Vitalik, Zoë Hitzig, and E. Glen Weyl, 2018, “Liberal Radicalism: A Flexible Design for Philanthropic Matching Funds”. URL:https://papers.ssrn.com/sol3/papers.cfm?abstract\_id=32436561

[2] Buterin, Vitalik, 2019b, “Pairwise Coordination Subsidies: A New Quadratic Funding Design”. URL: Pairwise coordination subsidies: a new quadratic funding design



---

欢迎提交你的DAO研究到邮箱：daorayaki@dorafactory.org，瓜分10000USDC赏金池！欢迎访问DAOrayaki官网（daorayaki.org）  
  
详情请参考：

[Dora Factory支持去中心化DAO研究组织DAOrayaki](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247483808&idx=1&sn=df951c963f866525ac1a63395be0d28d&chksm=c1d80075f6af8963e9eece49f88b2455402395dd36020293af9bfa9a40a7ed9c227f669dea1c&scene=21#wechat_redirect)

历史文章：

[DAOrayaki｜二次方投票：机制设计如何使民主激进化](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485100&idx=1&sn=c9da137fd19efa8d342b69dab3de524c&chksm=c1d80779f6af8e6ffc76352b779653d9283f9b00057a122f6b3e6ac61ec9cbdcf7f204c7777a&scene=21#wechat_redirect)

[DAOrayaki｜元数据、数据堆栈、数据目录3.0](http://mp.weixin.qq.com/s?__biz=MzkyNDIxMTM4Ng==&mid=2247485099&idx=2&sn=2d3f8933133b1231c5b6d57cccbb738b&chksm=c1d8077ef6af8e68634421946416f3d1c3508c28bd8fed63fed844d1777d4f02f747ee44c8bc&scene=21#wechat_redirect)

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





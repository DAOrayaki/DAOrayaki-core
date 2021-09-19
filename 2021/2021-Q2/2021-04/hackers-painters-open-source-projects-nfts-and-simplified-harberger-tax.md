


[DAO Media](/tag/dao-media/)

Hackers & Painters, Open Source Projects, NFTs, and Simplified Harberger Tax
============================================================================




* Daorayaki
---------


Read [more posts](/author/daorayaki/) by this author.



#### [Daorayaki](/author/daorayaki/)



17 Apr 2021
• 4 min read






![Hackers & Painters, Open Source Projects, NFTs, and Simplified Harberger Tax](/content/images/size/w2000/2021/04/-----2021-04-17---9.25.47.png)



![](http://daorayaki.org/content/images/2021/04/DAOrayaki-Guidelines-08-3.png)Author：Architecht @ Dora factory

In this article I discuss an alternative funding and price discovery mechanism for open source projects with NFTs and a simplified Harberger Tax.

As open source developer groups are becoming venture units, incentivizing open source projects are important tasks. Hackathon and bounty have always been direct methods to do it — developers can build something to win prize at a hackathon, or solve some problem and get rewards from a bounty.

There have been new mechanisms to fund developers. For example, quadratic funding grants have been developed by GitCoin, clr.fund and DoraHacks’ developer platform HackerLink. Most of the major blockchain ecosystems are accepting quadratic funding as a way to co-fund open source developer projects with the community. So far, GitCoin grants have supported many projects from the Ethereum ecosystem, whereas HackerLink grants are supporting projects from BSC, Flow, Filecoin, Solana, HECO, and more.

On the other hand, all these schemes are ways to rank projects within a certain scope, therefore serving as a way for people to identify promising projects from the crowd. Hackathons are normally generating ranks based on judge opinions (judges are mostly experts or investors in related domains), whereas quadratic funding grants generate ranks based on community popularity. For example, at DoraHacks, venture capitals look at the hackathon ranks and grant leaderboards to source top-ranked projects to invest.

Hackathon ranks and grant leaderboards work well. However, they all rely on organizers, therefore having limited capacities, i.e. hackathons have to be organized, grants must be hosted in rounds. Fundings and rankings are generated within each event, so the value / price discovery is not intrinsic.

So how can we design a mechanism for open source project funding and price discovery without dependency on external events? Here I propose a method to achieve this by using NFTs and Harberger Tax combined.

NFTs are intuitive — they are non-fungible tokens to represent unique assets.

Harberger Tax is a property tax with two features:

1. People assess value of their asset and pay tax based on their own assessment
2. Anyone can buy a property at the assessed price from its owner, forcing a sale

There are some Harberger tax based Dapps that have received great attentions and interesting feedbacks. The earliest one is [ThisArtworkIsAlwaysOnSale](https://thisartworkisalwaysonsale.com/), created by Simon de la Rouviere. In the NGO space, [Wildcards](https://wildcards.world/) is using Harberger tax to raise fund for conservation. These experiments are pioneering and inspiring.

With the help of blockchain and smart contracts, Harberger tax is finally found feasible and useful in certain domains.

However, it is important to recognize that the background of Harberger tax is different from now. It’s under the assumption that real properties have two features: 1) operation costs are significant, e.g. government needs a great amount of resource to operate and manage public space so real property tax is a must, 2) scarcity is common in real properties.

In the virtual space, these assumptions are not important. Creating and holding a digital art NFT does not incur any operational cost, and there are infinite NFTs we can create in the virtual space.

Because of that, it’s more reasonable to tax on capital gains rather than charging a patronage. For example, an art collector does not want to be taxed all the time just because owning a painting, and there is no need to do so, because an art — in the end — is not a real property. However, the artist can be well funded with an initial sale plus a certain percentage of tax on capital gains from each future resale. The same logic applies to digital artists, and in our case, open source artists (developers).

One feature from Harberger tax that is very useful is forcing a sale. With a smart contract, we can do two things: (1) register all NFTs, (2) anyone can force a sale without permission from the previous owner.

We can use some features of Harberger tax and what we have discussed to design an alternative mechanism for fund open source project funding and price discovery. The mechanism works as follows:

1. Every project can issue a unique non-fungible token, with an initial price. The address that minted the token becomes the first owner of the token.
2. Anyone can buy the token from a previous owner based on his/her own assessment of the asset, as long as the price is set higher than the previous price.
3. A tax will be imposed on the capital gains of the sale. For example, if an OSS / BUIDL NFT is sold at 20 $DORA and the previous sale was at 10 $DORA, then a 20% of tax means 2 $DORA will be distributed to the project owner, and 18 $DORA will be distributed to the previous owner.

The Dora team is currently deploying a feature to HackerLink and experiment this mechanism. It will show up next week on [HackerLink BUIDL](https://hackerlink.io/en/Buidl). In practice, there can be a few additional rules that we can add to the mechanism.

1. Any currency can be used to price the token.
2. Add a fee to each sale to avoid small-amount attack to the system (e.g. add 0.000001 $DORA and the ownership is transferred).
3. Add a message to each NFT and refer to its HackerLink BUIDL ID and GitHub repo link.

In additional to OSS BUIDLs, this mechanism can be applied to funding and price discovery in other fields. For example, it can be an alternative way to issue NFTs for crypto arts and help the arts with price discovery while continuing to reward the artists. It can also help environment conservation organizations to price wildlife cards and collect funding from the transaction of the cards. For example, [Project Ark](https://hackerlink.io/en/Grant/GHS/Round/1/buidl/325) recently applied for DoraHacks Singapore Hackathon’s grant, and they are generating NFT cards for wildlife conservation.

Think of it like a factory that allows any OSS project to issue its own “Uniswap sock token” that is freely tradable with NFTs and simplified Harberger Tax.





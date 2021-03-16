---
title: "Keeper DAO (ROOK)"
categories:
  - Whitepaper Wednesday
tags:
  - Post Formats
  - readability
  - standard
---
Years ago we read [Flash Boys 2.0](https://arxiv.org/pdf/1904.05234.pdf), a [paper](https://twitter.com/phildaian/status/1116155253890613249?lang=en) that illuminated the issue with PGA (Priority Gas Auctions).  With the rise of DEX's arbitrage has becoming a growing part of the blockspace.  Because all transactions must first sit in the mempool before being mined, they live for a small time in [Ethereum's Dark Forest](https://medium.com/@danrobinson/ethereum-is-a-dark-forest-ecc5f0505dff) visible to all.  Arbitrage itself is not a problem, but as DeFi exploded this summer, blockspace became scarce and gas fees exploded.  When blockspace is abundant, we tend to [use these networks inefficiently](https://satoshidice.com/).  As gas fees go up, we collectively must figure out how to use blockspace more efficiently.  [Gas Auctions create MEV](https://anchor.fm/uncommoncore/episodes/9-Gas-Wars-Understanding-Ethereums-Mempool--Miner-Extractable-Value-ejtp3j) (Miner Extractable Value) by creating a competition between independent arbitrageurs competiting to be the first transaction mined and capturing an arbitrage opportunity.  As parties compete by raising their gas bids, only one can be accepted causing each player to bid fees up to the value of the arb.  Any economic system which allows pure competition drives economic profit of firms to zero and the blockchain is the fairest playing field ever created.  The mempool is available to all.  As gas prices rise and the profit of arbitrageurs goes to 0 they transfer the profit from themselves into the miners pockets.  Miners capture all excess value in the ETH ecosystem.

[Keeper DAO](https://github.com/keeperdao/whitepaper/blob/main/whitepaper.pdf) created the coordination game to incentivize arbitrageurs and liquidators, named Keepers to work together rather than competition.  Using the principles of Bitcoin, they created an economic model that restructures the profit incentive to behave in a manner that is optimal/efficient for the network rather than wasteful.  

- For liquidations, they ask you to allow their Keepers to liquidate you slightly before Maker/AAVE would. By giving their network priority there is no competition to liquidate.
- For arbitrage they share the rewards between Keepers and have some kind of round robin arb opportunity allocation mechanism.

**Problems raised with Keeper Dao**

On the initial read of the paper it wasn't clear how Keeper Dao would hide the transactions from the mempool.  After chatting with folks in their discord it appears they do NOT do any specialized routing or hiding of Keeper transactions.  They solve the problem purely by incentivizing all Keepers to join the collective/cartel rather than competing with it.  The issue that was raised during our conversation was that their are [other Keeper networks being created](https://docs.keep3r.network/).  If the microstructure of the market incentivizes multiple cartels to form and compete all economic profits will still accrue to miners.  Will all Keeper networks eventually merge into one giant conglomerate?  Is this decentralized or desirable?

Lastly, this still does not solve the problem of miners eventually bringing Keepers in house.  Given that they have control over the ordering of transactions, there is nothing the Keepers can do to prevent miners from re-ordering their own transactions, keeping the fee AND "stealing" the arbitrage.

Check out [@kirstenrpomales excellent tweet thread](https://twitter.com/kirstenrpomales/status/1367219619304505354) on this topic

If you'd like to join discussions like this, [DM me on twitter](https://twitter.com/blake41).  We try and keep the group small and by reference only to maintain a high quality conversation.

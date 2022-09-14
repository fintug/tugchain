What is TugChain?
-------------

TugChain is a decentralized blockchain project built on optimized proof of stake consensus. 
The major features of the TugChain network include:

1. Compatibility with the Ethereum Virtual Machine, which allows for compatibility with most existing Solidity based smart contracts. No special solidity compiler is required to deploy your smart contract to TugChain. 
2. A Proof of Stake consensus system which is optimized for TugChain's contract model. Any user can stake and help to secure the network. There is no voting, master nodes, or minimum amount required. There have been transactions as small as 2 Tugs that have created blocks in the past. Staking from smart contracts is under development.
3. The Decentralized Governance Protocol is completely implemented and functional, which allows certain network parameters to be modified without a fork or other network disruption.

TODO - Trasnaction model decision.
TODO - TugChain Documentation and Usage Resources

Basic usage resources:
Development resources:

General Info about TugChain:

Developer's Tools
-----------------

What is TugChain Core?
------------------

### TugChain Web Wallet

A browser wallet that supports the Ledger hardware wallet, offline cold wallet, restoration from mobile wallets, creation of QRC20 tokens and QRC1155 NFTs.


### iOS and Android Wallets

These wallets run on mobile devices and synchronize quickly. 

# Building TugChain Core



# Proof of Stake \(PoS\)

The proof-of-stake \(PoS\) mechanism works using an algorithm that selects participants with the highest stakes as validators, assuming that the highest stakeholders are incentivized to ensure a transaction is processed. The idea is that those with the most coins in circulation have the most to lose so they are positioned to work in the interest of the network. The amount of coins that a network may require changes just like the difficulty in PoW.

In PoS, the blocks aren’t created by miners doing work, but by minters staking their tokens to “bet” on which blocks are valid. In the case of a fork, minters spend their tokens voting on which fork to support. Assuming most people vote on the correct fork, validators who voted on the wrong fork would “lose their stake” in the correct one.  
The common argument against proof-of-stake is the Nothing at Stake problem. The concern is that since it costs validators almost no computational power to support a fork unlike PoW, validators could vote for both sides of every fork that happens. Forks in PoS could then be much more common than in PoW, which some people worry could harm the credibility of the currency.  


## Coin age

To distinguish between users who have just obtained their coins and users who have been holding their coins for a period of time, proof-of-stake algorithms use the idea of coin age.

Coin age is used in the calculation for both stake weight AND the staking reward. Staking reward is set by the coin's APR. The effect is a stable, consistent interest for all staking wallets, regardless of input size or reasonable downtime.

The longer a user holds the coins, the higher the changes of winning the right to create a block of the network blockchain and get a reward.

## Incentivizing to stay connected

In order to keep most user active, the reward for the creation of a block increase if there is too many users offline, so there is more benefits to go online.

## Penalizing offline users

Most if not all PoS algorithm penalize Holders which can stay offline for long periods of time. Otherwise they could get control by connecting back to it and having over 50% of voting power because of the size of their holdings.

## Pseudo anonymous users

Validators within the PoS network are anonymous users who are identified only by their wallet address. This pro-vides no additional accountability over PoW for bad actors who can amass significant wealth on the network.

## Security

The security model is an economic one, based on the “game-theory” assumption that the cost of acquiring the tokens necessary to become a block producer is more than an attacker is willing to bear, that couples the network’s security to the value of its token, ie: the higher the value of the token, the more secure the network becomes.

## nothing-at-stake attack

Without economic penalties for attackers, the chain can suffer nothing-at-stake attacks where stakers are incentivised to validate all proposed forks to maximise their returns. ![pos-nothing-stake](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/pos-nothing-stake.png)

## Algorithm

![Cosmos.network.pos](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/pos-cosmos.network.png)

1. The validators will have to lock up some of their coins as stake.
2. After that, they will start validating the blocks. Meaning, when they discover a block which they think can be added to the chain, they will validate it by placing a bet on it.
3. If the block gets appended, then the validators will get a reward proportional to their bets.

## **Pros**

* Cost efficient: speed, energy, hardware
* The more people use the network and have coins, the more secure the network.
* More decentralized

## Cons

* Economic inequality, rich get richer.
* Attackers can calculate the probability of winning the reward to create a block of the blockchain based on who has how many coins.
* Initial targets for Ethereum’s Casper implementation are only 100 TPS
* **Nothing at Stake** attacks

## Read more

* [Wikipedia](https://en.wikipedia.org/wiki/Proof-of-stake)



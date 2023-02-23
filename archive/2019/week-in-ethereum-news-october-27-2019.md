---
title: "Week in Ethereum News <BR> October 27, 2019"
date: "2019-10-28"
---

## **Eth News and Links**

**Eth1**

- Latest [core devs call](https://youtu.be/zT4TzlXQ6wA?t=153). [Notes from the call](https://twitter.com/TimBeiko/status/1187731839370301444).
- Istanbul tentatively scheduled for December 4th with January 8th as a backup.
- Train station model: how to get a [regular release cadence for Eth1](https://medium.com/@timbeiko/train-planes-network-upgrades-6edfc9f6b7dd). Hard forks happen on a schedule, EIPs go in when they’re ready and agreed to.
- Did raising the [gas limit affect the state growth](https://medium.com/@akhounov/ethereum-block-gas-limit-increase-and-state-growth-b95353153179)? So far it is inconclusive.

**Eth2**

- [What’s New in Eth2](https://notes.ethereum.org/@ChihChengLiang/Sk8Zs--CQ/Sk8Zs--CQ?type=book), featuring Ben's thoughts on Eth2 and composability.
- Danny Ryan’s quick [update on Eth2 plans](https://blog.ethereum.org/2019/10/23/eth2-quick-update/). The deposit contract is ready, but waiting on BLS standardization. Testnets are coming soon, but phase 0 is getting simplified given how phase 1 sharding has evolved.
- Latest [implementer call](https://www.youtube.com/watch?v=DXGeC7cg71Y). [Notes from the call](https://docs.google.com/document/d/1UN16SgDzG9mMVCKTrpw9QKANM-TBc_Jz6rhkGke7hAM/edit)
- Updated spec [v0.8.4](https://github.com/ethereum/eth2.0-specs/releases/tag/v0.8.4), minor changes
- [Muskoka](https://twitter.com/protolambda/status/1187320137092714496) eth2 client test harness
- [Responding to “a 51% attack](https://ethresear.ch/t/responding-to-51-attacks-in-casper-ffg/6363) would be a moment of joy for the community, as at the cost of a day or perhaps a week’s disruption, an amount of the attacker’s ETH would get burned that counteracts _years_ of protocol-level issuance, increasing the value of ETH and hence making future attacks more expensive”
- RuntimeVerification’s [formal model in K of the beacon chain](https://medium.com/coinmonks/a-formal-model-in-k-of-the-beacon-chain-ethereum-2-0s-primary-proof-of-stake-blockchain-429883e316b9)

**Layer 2**

- [Fuel](https://medium.com/@fuellabs/fuel-scaling-stablecoin-payments-10x-today-50x-in-the-near-future-961e3113b39b): optimistic rollup for stablecoin from Nick Dodson and John Adler
- [Optimistic rollup Q&A](https://docs.google.com/document/d/17f9JeeSW_M3PrMmvMsmArTDEqOkSKEZQySNKfpewIP4/edit) with Plasma Group
- An [overview of rollup](https://medium.com/@kimiwu/zk-rollup-optimistic-rollup-70c01295231b), both zk and optimistic
- Celer’s [state channels specification walkthrough](https://medium.com/celer-network/celer-state-channel-full-specification-and-design-principles-walkthrough-64db4659ee93)

**Stuff for developers**

- [web3js v1.2.2](https://github.com/ethereum/web3.js/releases/tag/v1.2.2) - TypeScript support, transaction signing and confirmation changes, new JSON RPC method, and bloom filters
- [OpenZeppelin Test Helpers v0.5](https://forum.openzeppelin.com/t/openzeppelin-test-helpers-0-5/1600)
- Guide to [using Dai in your code](https://github.com/makerdao/developerguides/blob/master/dai/dai-in-smart-contracts/README.md)
- Istanbul’s [SLOAD reprice to 800 gas](https://medium.com/authereum/istanbul-gas-reprice-breaks-contract-interactions-4236fdddb5e0) breaks contract interactions
- [Eth.Build](https://eth.build/) - Austin Griffith’s new series of tutorials with a dev sandbox

**Ecosystem**

- All [Devcon5 main stage videos](https://slideslive.com/ethereum/devcon5)
- [Everything you can do with your ENS name right now](https://medium.com/the-ethereum-name-service/everything-you-can-do-with-your-ens-name-right-now-9a66763e970a)
- You can now [search for people on 3Box](https://medium.com/3box/3box-hub-search-6ba9ec0e672)
- Kevin Kim’s [DeFi UX research study](https://medium.com/usegossamer/the-next-wave-of-defi-users-a-ux-research-study-f20f180c23a1)
- Results from [q3 Gitcoin Grants](https://gitcoin.co/blog/gitcoins-q3-match/)

**Enterprise**

- Hyperledger Besu [v1.3.2](https://pegasys.tech/solutions/hyperledger-besu/)
- A Besu addon: [PegaSysPlus](https://pegasys.tech/pegasys-plus-commercially-licenced-enterprise-ethereum-client-by-pegasys-protocol-engineering/) which adds RocksDB encryption, event streaming and monitoring
- 11 requirements for [choosing a permissioned chain](https://media.consensys.net/taking-a-regulated-permissioned-blockchain-network-to-production-9f33709d3af0) in production
- [Trustology for business](https://trustology.io/wp-content/uploads/2019/10/Press-release_Trustology-Business-Account_Sept-2019-1-1.pdf): a custodial wallet of HSMs

**Application layer**

- Maker [roadmap to Multi-collateral Dai launch](https://blog.makerdao.com/mcd-security-roadmap-update-october-2019/) on Nov 18
- All [Compound admin functions are now on a 2 day time delay](https://medium.com/compound-finance/upgrading-compound-governance-c56b55a2996c)
- [Gitcoin Quests](https://gitcoin.co/quests/) - gamified web3 learning
- [Set Protocol as asset management platform](https://medium.com/set-protocol/set-protocol-enabling-programmable-assets-1fb9857811e9)
- KyberSwap [limit order v2](https://medium.com/kyberswap/kyberswap-limit-order-2-0-63b79633daee)
- A bunch of great [Alethio stablecoin data viz](https://medium.com/alethio/statistics-around-dai-stablecoin-fb359d6881aa)
- [STLD Exchange will do instant payouts to winners](https://medium.com/@stldexchange/introducing-stld-exchange-1e6a15f8221d) on Augur v2
- Numerai [achieves “Meta Model supremacy.”](https://medium.com/numerai/achieving-meta-model-supremacy-at-numerai-9ca3abeef98a) And the tourney now [running on Erasure](https://twitter.com/richardcraib/status/1188115587311910912)
- [TruSat](https://www.geekwire.com/2019/morphing-planetary-resources-consensys-space-unveils-trusat-satellite-tracker/) - a satellite tracking platform for amateur stargazers

**Tokens / Business / Regulation / Global Realpolitik**

- Chris Burniske on the plethora of [mechanics working against 2017’s overfunded eth killers](https://www.placeholder.vc/blog/2019/10/22/fire-before-growth-the-likely-fate-of-ethereum-killers)
- Mark Zuckerberg appeared before a US House committee and promoted [Libra as an instrument of American power](https://www.washingtonpost.com/business/technology/zuckerberg-appears-in-congress-as-facebook-faces-scrutiny/2019/10/23/3aaf442a-f5bc-11e9-b2d2-1f37c9d82dbb_story.html)
- A couple days later, Chinese President Xi says they will [increase investment and focus on “blockchain.”](https://medium.com/@mablejiang/xi-jinpings-speech-at-the-18th-collective-study-of-the-chinese-political-bureau-of-the-central-1219730677b2) Cryptoassets shot up ~30%
- On Bank of England Governor [Mark Carney’s globalcoin](https://medium.com/@C1aranMurray/on-mark-carneys-globalcoin-5896ba44a59d)
- ESPN article [how it would work to buy Spencer Dinwiddie tokens](https://www.espn.com/nba/story/_/id/27853850/how-investing-150k-spencer-dinwiddie-actually-work)
- [Graph Network indexing protocol](https://thegraph.com/blog/the-graph-network-in-depth-part-1). Interesting token model
- Ryan Sean Adams: [ETH’s monetary policy is underrated](https://bankless.substack.com/p/eths-monetary-policy-is-underrated)

**General**

- [Transparent SNARKs from DARK compilers](https://eprint.iacr.org/2019/1229.pdf)
- [ETH now live on Bitpay](https://twitter.com/BitPay/status/1186664834793914368?)
- Ex-CFTC Chair Giancarlo says they approved [bitcoin futures to pop the BTC bubble](https://finance.yahoo.com/amphtml/news/trump-administration-popped-2017-bitcoin-191510223.html)
- How to calculate [Brave’s ad blocker time savings](https://brave.com/accurately-predicting-ad-blocker-savings/)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Oct 28-Nov 11 - [Web3 World virtual hackathon](https://hackathons.gitcoin.co/web3-world/)
- Oct 28-Nov 1 - [SF Blockchain Week](https://sfblockchainweek.io/)
- Nov 1 - [Ledger EU](https://ledgerproject.eu/) apply for 200k euro startup funding
- Nov 5-6 - [Decentralized insurance D1Conf](https://blog.etherisc.com/d1conf-2019-to-focus-on-blockchain-adoption-november-5-6th-in-malta-3b8b582ac7b4) (Malta)
- **Nov 7 - [web3 UX unconference](http://ux.conflux.network/#/) (Toronto)**
- Nov 8-10 - [ETHWaterloo](https://ethwaterloo.com/)
- Jan 1 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff-update/)
- Feb 9-15 - [EthLagos](https://ethlagos.io/)
- Feb 14-16 - [ETHDenver](https://www.ethdenver.com/)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

It’s amazing to me how many people email me when every issue has a link at the bottom saying not to email me to get in the newsletter.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **This headline stays as long as so many people continue to link to old URL and not the right one: [weekinethereumnews.com](https://weekinethereumnews.com/)**

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/week-in-ethereum-news-october-27-2019/](https://weekinethereumnews.com/week-in-ethereum-news-october-27-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

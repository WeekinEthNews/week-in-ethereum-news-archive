---
title: "June 7, 2018"
date: "2018-06-07"
---

## **News and Links**

**Protocol**

- [Core devs call](https://www.youtube.com/watch?v=7FNRWEQ_H7w).  Lane’s [notes](https://github.com/ethereum/pm/blob/master/All%20Core%20Devs%20Meetings/Meeting%2039.md).
- Latest [Casper standup](https://www.youtube.com/watch?v=AhEy1f17QLs)
- Fichter: [Simple Fast Plasma Withdrawals](https://ethresear.ch/t/simple-fast-withdrawals/2128)
- Two implementations I didn’t have time to read but seemed interesting: 1) Lucidity’s [yellow paper for Plasma chain](https://lucidity.tech/wp-content/uploads/2018/06/Lucidity-Yellowpaper-v0.5.10-060618.pdf) for programmatic ads and 2) Levj’s [Plasma Gluon](https://blog.leverj.io/a-faster-dex-using-plasma-5d0b326567ab) which says it is on testnet
- [PlasmaBits](https://gist.github.com/eordano/ec3bd1e0bdcbc090e65320a8eed1e2c6): Esteban Ordano’s proposal aimed more at generalized state
- Pysmatic’s [sharding implementation call](https://t.co/7csRDZItWs)
- Buterin: [A proposal for structuring committees, cross-links, etc](https://ethresear.ch/t/a-proposal-for-structuring-committees-cross-links-etc/2118)
- Drake: [Registrations, shard count and shuffling](https://ethresear.ch/t/registrations-shard-count-and-shuffling/2129)
- [Charging rent for testnet storage](https://ethereum-magicians.org/t/allcoredevs-discussion-about-storage-rent-in-the-testnets/495) discussion

**Stuff for developers**

- [gnarly](https://github.com/XLNT/gnarly) optimistic UI library is in alpha.
- [Drizzle v1.2](https://github.com/trufflesuite/drizzle/releases/tag/1.2.0) 
- [Connext v0.3](https://medium.com/connext/connext-v0-3-developer-update-4d6914d02b76) - virtual channels live on Rinkeby
- [OpenZeppelin v1.10](https://github.com/OpenZeppelin/openzeppelin-solidity/releases/tag/v1.10.0) release
- [Solidity graphical debugger](https://www.reddit.com/r/ethereum/comments/8oqalq/i_created_a_solidity_graphical_debugger_still_at/), somewhat similar to [Mythril](https://github.com/ConsenSys/mythril-trace-explorer/)
- [Mocha reporter for Truffle](https://github.com/cgewecke/eth-gas-reporter).  Not new, but [Andy Tudhope says](https://twitter.com/cryptowanderer/status/1003557515425181696) most devs don’t know it exists in the [Ethprize developer interviews](https://medium.com/@cryptowanderer/ethprize-an-introduction-8fb60c7a0b7)
- Turning [smart contracts into gastoken factories](https://blog.polymath.network/turning-smart-contracts-into-gastoken-factories-3e947f664e8b) 
- [EthereumJS](https://www.reddit.com/r/ethereum/comments/8nmelx/ethereumjs_monthly_recap_may_2018/) May recap
- Options for fixing the [missing return value bug](https://medium.com/coinmonks/missing-return-value-bug-at-least-130-tokens-affected-d67bf08521ca)  affecting ~100 tokens
- Loom releases [SDK for dappchains](https://github.com/loomnetwork/cocos-sdk) for Cocos gaming platform (supposedly one of the largest in Asia?)
- Gas golfing fun: [converting quicksort in Java to Solidity](https://blog.cotten.io/thinking-in-solidity-6670c06390a9) 
- Malicious [backdoors in Ethereum proxies](https://medium.com/nomic-labs-blog/malicious-backdoors-in-ethereum-proxies-62629adf3357)

**Ecosystem**

- Josh Stark: [making sense of web3](https://medium.com/l4-media/making-sense-of-web-3-c1a9e74dcae)
- Loom: [Ethereum Will Be the Backbone of the New Internet](https://medium.com/loom-network/ethereum-will-be-the-backbone-of-the-new-internet-88718e08124f)
- Zeppelin: [Introducing the Transaction Permission Layer](https://blog.zeppelin.solutions/introducing-the-transaction-permission-layer-tpl-protocol-358f28cfff40)
- A [primer on light clients](https://medium.com/zkcapital/a-primer-on-ethereum-blockchain-light-clients-f3cadde49137)
- EthBerlin is aiming for [500-700 hackers](https://medium.com/ethberlin/back-to-basics-introducing-ethberlin-62ae3a922f53)
- [6 principles for UX dapp design](https://hackernoon.com/6-principles-for-designing-dapps-for-regular-people-from-a-consensus-18-hackathon-winner-134cdb881cc1) 
- [Raw responses](https://docs.google.com/spreadsheets/d/1nmWZKJq-ndF0uZGnHgQZq7Lm2_0xJbYWxmQTOrgIFfg/edit#gid=840981558) from the EIP0 values survey

**Live on mainnet**

- [Aragon launches its survey app](https://blog.aragon.one/aragon-launches-survey-app-on-mainnet-ed5eefeb66f5) on mainnet
- [Status latest release](https://blog.status.im/status-alpha-0-9-19-release-notes-a841affc3983) enables mainnet as a _**test**_ option.  After writing that, they had a [hotfix release](https://blog.status.im/0-9-19-hotfix-9addbea512ba).

**Client Release**

- Parity [1.11.3 (beta)](https://github.com/paritytech/parity/releases/tag/v1.11.3) or [1.10.6 (stable)](https://github.com/paritytech/parity/releases/tag/v1.10.6). Upgrade ASAP because of an issue with unsigned transactions when EIP86 disabled

**Governance and Standards**

- [ERC1132](https://github.com/ethereum/EIPs/issues/1132): Extending ERC20 with token locking capability
- Dicussion on [ERC1081](https://github.com/ethereum/EIPs/pull/1081) bounties standard
- Discussion on [ERC1098](https://github.com/ethereum/EIPs/pull/1098) cross-client encrypt/decrypt
- [ERC1138](https://github.com/ethereum/EIPs/issues/1138): URI Format for Calling Functions
- [ERC1133](https://github.com/ethereum/EIPs/issues/1133): Nesting token standard

**Project Updates**

- A profile of [Althea’s NW Oregon meshnet in operation.](https://inthemesh.com/archive/althea-deploys-rural-oregon/)  Also, [Althea governance model](https://medium.com/althea-mesh/the-althea-governance-model-232dbe20a71e): subnet DAOs with TCRs for subnet discovery.  
- Margin trading protocol [dYdX launches](https://medium.com/dydxderivatives/dydx-launches-on-testnet-38b2812c56e?source=linkShare-b3d17ffd3219-1528225715) on Kovan testnet
- [Golem beta v0.16](https://blog.golemproject.net/brass-golem-beta-0-16-0-7ed7ee2341b0): requesters can set minimums for provider machines. Non-backward compatible.
- Creating easy [onboarding for Raiden with Plasma payment hubs](https://medium.com/@raiden_network/creating-an-easy-onboarding-user-experience-for-the-raiden-network-4dcdc9e2eeed)
- New 2 minute [Streamr promo vid](https://www.youtube.com/watch?v=nbWIPVE8zFE)
- Funfair [update on their closed beta](https://funfair.io/funfair-closed-beta-weekly-update/)
- [TheGraph](https://thegraph.com/) decentralized query protocol:  use GraphQL to build Eth/IPFS dapps
- [Fig acquires Ownage](https://venturebeat.com/2018/05/31/fig-acquires-ownage-to-publish-blockchain-games/) to publish blockchain games
- Very interesting [future of online video stack](https://twitter.com/Felipether/status/1002279236445589504) Twitter thread from Paratii

**Interviews, Podcasts, Videos, Talks** 

- Amrit Kumar and Ilya Sergey talk [Zilliqa’s formally verified Scilla language](https://epicenter.tv/episode/238/) on Epicenter
- Colony’s [Alex Rea](https://itunes.apple.com/us/podcast/the-smartest-contract/id1377520772?mt=2) on Smartest Contract
- [EthBuenosAires episode](http://www.zeroknowledge.fm/28) of Zero Knowledge
- Gavin Wood’s recent talk on [Substrate and Energy Web Foundation](https://www.youtube.com/watch?v=iUMZyL5kTwc)
- More [talks and short interviews](https://www.youtube.com/channel/UCSFiCr8d3ej_pC57E75pPew/videos) from EthBuenosAires
- [DAOstack](https://epicenter.tv/episode/237/) on Epicenter
- [Christian Reitwiessner](https://itunes.apple.com/us/podcast/the-smartest-contract/id1377520772?mt=2#) on Smartest Contract
- [Nadav Hollander talks Dharma Protocol](https://itunes.apple.com/us/podcast/token-talks-interviews-with-the-best-projects-in-crypto/id1362129613?mt=2) on Token Talks
- [Raul Jordan and Preston Van Loon](https://softwareengineeringdaily.com/2018/06/01/scaling-ethereum-with-raul-jordan-and-preston-van-loon/) on Software Engineering Daily

**Tokens** 

- NYT: “[In the World of Cryptocurrency, Even Good Projects Can Go Bad](https://mobile.nytimes.com/2018/05/31/technology/envion-initial-coin-offering.html).”  This was not particularly close to being a “good project” and I barely remember it.  But good on NYT for calling them out on exaggerating the amount raised. That’s normally the case unless you can verify on-chain the amount raised.
- Interesting ideas for [extensible and composable NFTs](https://medium.com/@brianubiquik/crafting-new-value-with-existing-tokens-de95fe838fea)
- [Copyright in a time of Cryptokitty abundance](https://medium.com/@dennisonbertram_32974/copyright-in-a-time-of-abundance-4c48073edb8a)
- Enigma proposes [encrypted secret voting for TCRs](https://blog.enigma.co/private-voting-for-tcrs-with-enigma-b441b5d4fa7b)
- EthBuenosAires winner [Crypto against Humanity](https://medium.com/crypto-against-humanity/crypto-against-humanity-3aca70e7f001) will be an interesting experiment of TCRs and bonding curves

**General**

- [South African Reserve Bank demos Quorum with IBFT consensus](https://www.resbank.co.za/Lists/News%20and%20Publications/Attachments/8491/SARB_ProjectKhokha%2020180605.pdf) that can process all daily SA payments in 2 hours with privacy
- NYT on [SIG’s crypto desk](https://www.nytimes.com/2018/06/05/technology/bitcoin-susquehanna.html). Interesting bit: they built their own custody
- Coinbase: we’re going to do a [regulated security token](https://blog.coinbase.com/our-path-to-listing-sec-regulated-crypto-securities-a1724e13bb5a) exchange; acquires broker-dealer, ATS and RIA licenses
- Sequoia’s [Matt Huang to start crypto fund with Fred Ehrsam](http://archive.is/E2bZ4)
- Binance [announces $1 billion fund](https://techcrunch.com/2018/06/01/binance-1-billion-investment-fund/)
- Guide to [joining the Cosmos testnet](https://medium.com/forbole/a-step-by-step-guide-to-join-cosmos-hub-testnet-e591a3d2cb41)
- Zooko’s [notes from a call with Jihan Wu](https://forum.z.cash/t/so-i-had-a-videochat-with-jihan-wu/29379)
- 5 ways the [Catholic church should use blockchain](http://catholicblockchain.org/2018/06/03/5-ways-the-catholic-church-can-use-blockchain-technology-to-better-carry-out-her-mission/)
- Lots of NYT this week: “[When Crypto Meets Conceptual Art, Things Get Weird](https://www.nytimes.com/2018/06/05/arts/design/cryptocurrency-blockchain-art-kevin-abosch.html)”
- SEC names [Valerie Szczepanik its crypto czar](https://www.sec.gov/news/press-release/2018-102).  She comes from enforcement, but she’s also known for understanding the tech
- IMF: [Monetary policy in the digital age](https://www.imf.org/external/pubs/ft/fandd/2018/06/central-bank-monetary-policy-and-cryptocurrencies/he.pdf).  They’re taking this seriously.

## **Dates of Note**

**Upcoming dates of note:**

- June 14 -- [CryptoCup](https://t.co/WNf9jPuPCN) deadline to enter.  Link contains referral code, price goes up June 11
- June 24 -- [Colony](https://blog.colony.io/announcing-the-colony-global-hackathon-1d9bf9004407) online hackathon finishes
- June 25 -- [Etherisc](https://blog.etherisc.com/dip-token-generating-event-will-start-on-25-june-2018-db8c5aa832ac) token sale starts
- June 28 -- [BuildEth](http://www.buildeth.io/) (San Francisco)
- June 30 -- [Solidity Gas Golfing](https://g.solidity.cc/) challenge deadline
- June 30-July1 -- [Off the chain](https://binarydistrict.com/courses/master-workshop-off-the-chain/) state channel workshop (Berlin)
- July 6-7 -- TechCrunch [blockchain and Ethereum events](https://techcrunch.com/2018/06/03/announcing-the-techcrunch-ethereum-meetup-alongside-our-blockchain-event-in-zug/) (Zug) 
- July 9 -- [Augur](https://medium.com/@AugurProject/augur-weekly-development-update-may-23rd-4d78befe7bf8) scheduled to launch
- July 12-18 -- [IC3 Eth Bootcamp](http://www.initc3.org/events/2018-07-12-IC3-Ethereum-Crypto-Boot-Camp.html) (Ithaca, NY)
- July 14-15 -- [FEM governance meetings](https://ethereum-magicians.org/t/proposed-agenda-for-the-council-of-berlin-set-for-july-14-15/377) in Berlin
- July 19-20 -- [DappCon](https://www.dappcon.io/) (Berlin)
- August 3-4 -- [Discon](https://discon.io/) (Boulder, CO)
- August 10-12 -- EthIndia hackathon (Bangalore)
- September 6 -- [Security unconference](https://ethereum-magicians.org/t/wiki-gathering-of-security-community/433) (Berlin)
- September 7-9 -- [EthBerlin](http://ethberlin.com/) hackathon
- September 7-9 -- WyoHackathon (Wyoming)
- Oct 5-7 -- [TruffleCon](http://truffleframework.com/trufflecon2018) in Portland
- Oct 5-7 -- EthSanFrancisco hackathon
- Oct 22-24 -- [Web3Summit](http://web3summit.com/) (Berlin)
- Oct 30 - Nov 2 -- [Devcon4](https://devcon.ethereum.org/) (Prague)
- December -- EthSingapore hackathon

## **If you appreciate this newsletter, thank ConsenSys**

I'm thankful that [ConsenSys](http://consensys.net/) has brought me on and given me time to do this newsletter.  

![](https://steemitimages.com/640x0/https://78.media.tumblr.com/9114e5ec047c95b2ef505fd878651dc4/tumblr_inline_p9lxt7kwVA1rxca3y_250.jpg)

Editorial control is 100% me.  If you're unhappy with editorial decisions, blame me.

## **Shameless self-promotion**

Note: this post was on steemit. I figured I’d try putting on issue on Steemit as an experiment.  

Most of what I link to I tweet first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

This newsletter is supported by [ConsenSys](https://consensys.net/)

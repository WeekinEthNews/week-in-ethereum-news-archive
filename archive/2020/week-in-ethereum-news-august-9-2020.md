---
title: "Week in Ethereum News <BR> August 9, 2020"
date: "2020-08-09"
---

## **Eth News and Links**

**Eth1**

- [Regenesis plan](https://ledgerwatch.github.io/regenesis_plan.html) proposal
- Latest [core devs call](https://youtu.be/Riu-PqrJVH4?t=174) video. Beiko [notes](https://twitter.com/TimBeiko/status/1291725797506482177)
- Turbogeth [improved stability](https://github.com/ledgerwatch/turbo-geth/releases/tag/2020.08.01-alpha) release
- Turbogeth’s [staged sync](https://github.com/ledgerwatch/turbo-geth/tree/master/eth/stagedsync) explainer - how it does a full sync to an archive node in under 700gb and just a few days

**Eth2**

- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200808): the Medalla multi-client testnet launched
- Danny Ryan’s latest [quick eth2 update](https://blog.ethereum.org/2020/08/03/eth2-quick-update-no-14/), attacknet bounties now tripled
- Jonny Rhea’s attacks [found a bug in Go-lang](https://github.com/ethereum/public-attacknets/issues/12) with the help of protolambda, Raúl Kripalani, and Preston Van Loon (Go already released a bugfix)
- Latest [eth2 call](https://youtu.be/DVePZUQOyFk?t=147). Notes from [Ben](https://hackmd.io/@benjaminion/B1PSWKFbv) and [Mamy](https://gist.github.com/mratsim/1985e83a37419fb6d33e2ba8a5fcf004).
- Latest [Prysmatic client](https://medium.com/prysmatic-labs/eth-2-0-dev-update-55-medalla-testnet-7d03d828aaa8) update
- Eth2 annotated specs from [Vitalik Buterin](https://github.com/ethereum/annotated-spec) and [Ben Edgington](https://benjaminion.xyz/eth2-annotated-spec/)
- Ethereum Foundation is looking to [expand its security team for eth2](https://twitter.com/drakefjustin/status/1289656431927611398)
- Stats from [crawling Medalla nodes](https://txrx-research.github.io/prkl/medalla-analysis.html). A serious problem: [client diversity](https://eth2.ethernodes.org/network/Medalla)
- Some guides to staking: [Larrypc](https://gist.github.com/Larrypcdotcom/fcd4e79c2cf02ce37ec6ed9797beca2c), [Somer Esat](https://medium.com/@SomerEsat), [CoinCashew](https://www.reddit.com/r/ethstaker/comments/i3ee37/ultimate_ubuntu_eth2_staking_guide_with_lodestar/). Make sure you collect your [POAP medals for each different client](https://beaconcha.in/poap)
- [Defining attestation effectiveness](https://www.attestant.io/posts/defining-attestation-effectiveness/): Attestant’s work to create the stat on validator quality that you now see on [beaconcha.in](https://beaconcha.in/)

**EIPs/Standards**

- [ERC2771](https://eips.ethereum.org/EIPS/eip-2771): Secure Protocol for Native Meta Transactions
- [ERC2848](https://github.com/InternetOfPeers/EIPs/blob/73fbef9a7bbe1ff95a222b9ef31d97fbbd1ddfcc/EIPS/eip-2848.md): My Own Messages

**Crypto**

- StarkWare’s [IACR paper on EthSTARK](https://eprint.iacr.org/2020/948.pdf)
- [BLS sigs explainer series](https://medium.com/@alonmuroch_65570/bls-signatures-part-2-key-concepts-of-pairings-27a8a9533d0c)

**Layer2**

- iden3’s [hermez zk-rollup](https://blog.hermez.io/welcome-to-the-light-hermez/), expected to launch with 2000 tps on mainnet this year.
- [Optimize for minting tokens](https://ethresear.ch/t/lazy-launch-deploy-early-with-scaleability-then-add-smart-contract-interoperability-later/7805): a different l2 flavor inspired by Reddit bakeoff

* * *

### **This newsletter is made possible thanks to [Trail of Bits](https://www.trailofbits.com/)!**

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F4ad922bc-c1e9-41bb-a9bf-c4f4f2c09961_1876x1128.png)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F4ad922bc-c1e9-41bb-a9bf-c4f4f2c09961_1876x1128.png)

DeFi composability is hard, and it’s easy to accidentally expose your new protocol to unexpected risk.

Stay current: learn about the latest composability risk [Sam Sun found in yEarn](https://blog.trailofbits.com/2020/08/05/accidentally-stepping-on-a-defi-lego/), and follow Trail of Bits' checklist for [integrating with tokens](https://github.com/crytic/building-secure-contracts/blob/master/development-guidelines/token_integration.md).

* * *

**Stuff for developers**

- ZoKrates [v0.6](https://github.com/Zokrates/ZoKrates/releases/tag/0.6.0) - unsigned integer types, zokrates.js works with browser/nodeJS, native SHA256 implementation at 28k constraints
- TypeChain’s [stable ethers v5 release](https://github.com/ethereum-ts/TypeChain/releases/tag/ethers-v5)
- [Opyn got hacked](https://medium.com/opyn/opyn-eth-put-exploit-c5565c528ad2) for 370k USDC, and then Sam Sun helped them rescue another 570k. They [reimbursed all victims](https://twitter.com/opyn_/status/1292506131533672449). Here’s [Peckshield’s explainer](https://blog.peckshield.com/2020/08/05/opyn/). If you prefer to watch, here’s an [Epheph video](https://www.youtube.com/watch?v=sMANc7K4lHk&feature=share) explainer
- Sam Sun found a bug in the initial [release of yEarn’s yVault](https://blog.trailofbits.com/2020/08/05/accidentally-stepping-on-a-defi-lego/) where an attacker could “man in the middle” the swaps.
- Martinet Lee and Jun-You Liu also found some [exploits in the yCurve yVault](https://hackmd.io/@martinetlee/rkQImCQbP)
- [Gas Saver](https://github.com/emilianobonassi/gas-saver): wrap methods to use gas tokens
- Deploy your [first contract with Chainlink](https://docs.chain.link/docs/example-walkthrough)
- [Clean contracts](https://www.wslyvh.com/clean-contracts/) - Solidity best practices
- [eth-permit](https://www.npmjs.com/package/eth-permit): easy token permit signing npm
- OpenZeppelin [Contracts special release to support Solidity v0.7](https://forum.openzeppelin.com/t/openzeppelin-contracts-and-solidity-0-7/3476)
- Trail of Bits [token integration checklist](https://github.com/crytic/building-secure-contracts/blob/master/development-guidelines/token_integration.md)

**Ecosystem**

- ethereum.org [development update](https://blog.ethereum.org/2020/08/05/ethereum-dot-org-development-update-4/): a new look!
- [Save on paying gas](https://medium.com/dextf/ethereum-how-to-save-even-more-on-gas-price-with-a-weekly-plan-c6689ac09fe6) with a weekly plan. In other words: what time of day gas prices are low
- Related to when gas prices are low: [DeFi is taking off in China](https://medium.com/imtoken/defi-is-taking-off-in-china-9837d9756bd)

**Enterprise**

- A [Coca-Cola bottling group to use Baseline Protocol on Eth mainnet](https://provide.services/baselining-the-north-america-coca-cola-bottling-supply-chain/) for their supply chain vendors
- Goldman Sachs [exploring creation of its own cryptodollar](https://www.cnbc.com/2020/08/06/goldman-names-new-head-of-digital-assets-in-bet-that-blockchain-is-the-future-of-financial-markets.html) stablecoin

**Application layer**

- [DarkForest goes live](https://blog.zkga.me/announcing-darkforest) with Ropsten testnet beta: a decentralized, real time strategy game using SNARKs
- [Deversifi draws an unsecured credit line](https://medium.com/aave/first-credit-delegation-on-aave-protocol-to-deversifi-is-here-c6c0aedb70d4) using Aave and OpenLaw contract
- [Chem@Golem](https://blog.golemproject.net/announcing-chem-golem/), a Seti@Home inspired scientific modelling project
- How yDai offers [fully collateralized, fixed-interest borrowing](https://medium.com/yield-protocol/introducing-ydai-43a727b96fc7) using zero-coupon bonds
- [Set Protocol v2](https://medium.com/set-protocol/introducing-set-v2-afc577050bc0): many more assets, yield farming support, much more gas efficient

**Tokens/Business/Regulation**

- dYdX launches their [10x perpetual ETHUSD](https://twitter.com/dydxprotocol/status/1290696535634841600)
- Decentralized governance: [innovation or limitation](https://medium.com/dragonfly-research/decentralized-governance-innovation-or-imitation-ad872f37b1ea)?
- Grayscale’s [Ethereum Trust will be SEC reporting company](https://medium.com/grayscale-investments/a-milestone-for-ethe-8a92f899f343) due to “record quarterly inflows” and weekly inflows over 10 million USD
- Putin allows [crypto ownership but requires rubles](https://www.forbes.com/sites/kenrapoza/2020/08/06/putin-outlines-new-russian-crypto-rules-and-banks-prepare-for-new-exchanges/#5872007e66ed) as the medium of exchange

**General**

- [Andreas Antonopoulos](https://www.youtube.com/watch?v=MYOvvOyStvg&list=PLPQwGV1aLnTtLvDWXU80BJY-DTIJzcF1d&index=48&t=0s&utm_source=aantonop.io&utm_medium=urlshortener&utm_campaign&utm_term&utm_content) video answering basic Ethereum questions
- This week, BTC maxis spun themselves their usual tall tales about how hard it was to figure out the exact ETH supply. It’s not that hard. Here’s [Nethermind.](https://twitter.com/nethermindeth/status/1292075479835586560) [Geth](https://twitter.com/mhswende/status/1292368771802435584). Or this [Marc-André Dumas script](https://twitter.com/marcandu/status/1292099399980593154)
- ETC [51% attacked for second time](https://blog.bitquery.io/ethereum-classic-attack-8-august-catch-me-if-you-can) in a week
- [Filecoin plans to implement EIP1559](https://twitter.com/Whyrusleeping/status/1291916219470159872) on its next testnet

* * *

## **Job Listings**

- mStable is looking for developers: [see 3 open roles](https://cryptocurrencyjobs.co/startups/mstable/)
- OpenZeppelin: [Security Services Lead](https://openzeppelin.com/jobs/security-services-lead/), [Security Platform Dev](https://openzeppelin.com/jobs/security-platform-developer/) & [Open Source Dev](https://openzeppelin.com/jobs/open-source-developer/)
- [15+ open roles](https://careers.smartcontract.com/) at Chainlink: [Senior Software Eng](https://careers.smartcontract.com/o/senior-software-engineer-chainlink), [Product Marketing](https://careers.smartcontract.com/o/head-of-product-marketing), [Test Eng](https://careers.smartcontract.com/o/senior-software-engineer-test-chainlink)
- Trail of Bits is looking for: [blockchain security engineer](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & [senior software eng](https://jobs.lever.co/trailofbits/4fec3724-6ecb-4517-a092-5f9c12a60fc6)
- Celer Network: [Android developer](https://www.celer.network/career.html)
- 0x is looking for all kinds of devs: [full-stack, back-end, and front-end](https://0x.org/about/jobs)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH/DAI/USDC to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **Week in Eth News available sponsor slots tokenized as $EVAN**

This week, I [tokenized a few available sponsorship slots for this newsletter](https://www.evanvanness.com/post/625827671656595456/24-hours-of-evan-token) as $EVAN. I also added a few more redemption options. Without me doing anything it got listed on CoinGecko and CoinMarketCap, as well as a semi-accurate CoinTelegraph article. Check it out if you’re interested in my experiment in tokenizing indie media sponsorship space.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-9-2020/](https://weekinethereumnews.com/week-in-ethereum-news-august-9-2020/)

Did you get **forwarded** this newsletter? **[Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Aug 9-11 - [EDCON](https://edcon.io/)
- **Aug 13 - [Randomness Summit](https://randomness2020.com/?ref=weekinethereumnews)**
- Aug 28-29 - Chainlink’s [Smart Contract Virtual Summit](https://www.smartcontractsummit.io/)
- Oct 2-30 - [EthOnline hackathon](https://www.ethonline.org/)
- Nov 6-7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)

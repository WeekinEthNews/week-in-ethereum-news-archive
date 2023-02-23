---
title: "Week in Ethereum News<BR> March 21, 2020"
date: "2020-03-21"
---

## **Eth News and Links**

**Eth1**

- Latest [core devs call](https://youtu.be/vDGj660uZE0). [Tim Beiko’s notes](https://twitter.com/TimBeiko/status/1241001075739701248).
    - Discussions (non-exhaustive list) about EIP inclusions in next hard fork: eip2537 (BLS12-381 curve precompile) final, so we can have eth2 light clients on eth1. eip2456 timestamp for scheduling instead of block number, eip2542 vs ungas, eip2046 reducing gas cost for static calls, and eip1962 generalized precompile
- Geth [v1.9.12](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.12) - eth\_call no longer defaults to first account
- [Merry Go Round](https://ethresear.ch/t/merry-go-round-sync/7158) - an idea for syncing state, a la Bittorrent

**Eth2**

- Danny Ryan’s [Eth2 update](https://blog.ethereum.org/2020/03/17/eth2-quick-update-no-9/)
- Latest [what’s new in Eth2](https://notes.ethereum.org/@ChihChengLiang/Sk8Zs--CQ/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200320?type=book)
- [Prysmatic client](https://medium.com/prysmatic-labs/eth-2-0-dev-update-46-slasher-running-integrated-fuzz-testing-6d3647833afc) update - stable testnet for a month (but to be rebooted to current spec), surround vote slashing
- Tutorial to [run your own Lighthouse testnet](https://dev.to/q9/how-to-run-your-own-beacon-chain-e70)
- Vitalik’s personal [long-term ETH roadmap](https://twitter.com/VitalikButerin/status/1240365047421054976), beyond eth2
- Mikhail Kalinin’s writeup of his [eth1<>eth2 bridge idea](https://ethresear.ch/t/miners-vote-back/7129)
- [Sensor fusion for BFT clock sync](https://ethresear.ch/t/sensor-fusion-for-bft-clock-sync/7142). Alex Vlasov’s research on hardening timestamps
- [State transition in Eth2](https://sgryphon.wordpress.com/2020/03/17/eth-2-0-state-transition/) explainer from Nethermind’s Sly Gryphon
- How [Eth2 improves on Eth1’s weaknesses](https://medium.com/@0xKiwi/what-eth2-has-learned-from-eth1-d1f7e0830a98) from Prysmatic’s Ivan Martinez
- Gitcoin playlist of [short eth2 explainer videos](https://www.youtube.com/watch?v=td750o3xf8k&list=PLvTrX8LNPbPkOOTmVqjljLs2vk5-YZwLG)

**Layer2**

- Why iden3 is using [zk-rollup for universal identities](https://blog.iden3.io/zkrollup-to-universal-identities.html)

**Stuff for developers**

- Solidity [v0.5.17](https://github.com/ethereum/solidity/releases/tag/v0.5.17) (last?) release of 0.5.x (since 0.6 is out) disallowing overriding of private functions
- [TenderlyPro](https://blog.tenderly.dev/announcing-tenderly-pro/) released - simulate txs, advanced analytics, debugging
- [Debugging transactions with Buidler and Truffle](https://dev.to/fvictorio/debugging-transactions-in-ethereum-part-2-truffle-and-buidler-36pp)
- [Subspace v2](https://blog.embarklabs.io/news/2020/03/18/subspace-2.0/), much easier to track events in React.
- A [demo on observing Defi](https://our.status.im/subspace-observing-defi/) with Subspace
- [svm](https://blog.web3labs.com/a-solidity-version-manager-using-sokt): Solidity version manager
- Choose how many [IPFS replications you want pinned in each region](https://medium.com/pinata/ipfs-regions-and-replications-a1e52d60dfdb) with Pinata
- Austin Griffith video on [gas limits and gas prices](https://t.co/OLH595GiKm?amp=1)
- [Intro to Eth for Python devs](https://consensys.net/blog/blockchain-development/how-to-send-money-using-python-a-web3-py-tutorial/) using web3py
- Compare [Eth API performance with the Versus](https://blog.infura.io/compare-ethereum-api-performance-with-versus) tool
- Tutorial on [Ethereum RPCs, methods and calls in Infura](https://blog.infura.io/ethereum-rpcs-methods/)
- Mahesh Murthy updated his famous “[Full Stack Hello World Voting Ethereum Dapp Tutorial](https://medium.com/@mvmurthy/full-stack-hello-world-voting-ethereum-dapp-tutorial-part-1-40d2d0d807c2)” to use current libraries
- Guide to [building a margin trading platform](https://0x.org/docs/guides/develop-a-margin-trading-smart-contract-with-0x-api) on 0x
- A quick start guide for devs to [borrowing assets from Compound](https://medium.com/compound-finance/borrowing-assets-from-compound-quick-start-guide-f5e69af4b8f4)

**Ecosystem**

- A taxonomy of the advantages/disadvantages of [different types of Eth wallets](https://blog.gnosis.pm/breaking-down-ethereum-wallets-options-2162b41477d7)
- How do we better [onboard newcomers to Ethereum](https://medium.com/ethereum-cat-herders/how-can-we-onboard-newcomers-to-ethereum-better-6794a3314337)?
- [Custom text records](https://medium.com/the-ethereum-name-service/new-custom-text-records-means-every-project-can-have-its-own-ens-record-a68022bb8f86) on ENS

**Enterprise**

- [Baseline Protocol is now open source](https://github.com/ethereum-oasis/baseline), a common system of record between enterprises
- “blockchain will do, for networks of companies and business ecosystems, what ERP did for the single enterprise” - [Paul Brody, Cornell Blockchain interview](https://medium.com/@cornellblockchain/a-steady-march-of-adoption-7ffdc8fd560d)
- Resolving key considerations for [blockchain connectivity with PegaSys Orchestrate](https://pegasys.tech/resolving-key-considerations-for-blockchain-connectivity-with-pegasys-orchestrate/)
- Hyperledger Besu [v1.4.1](https://github.com/hyperledger/besu/releases/tag/1.4.1)
- First [public meeting of EEA’s mainnet working group](https://medium.com/@tasd/first-public-meeting-of-enterprise-ethereum-alliance-mainnet-working-group-scheduled-9ec6c6afc98e) scheduled for April 3

**Governance, DAOs, and standards**

- Technical overview of [Vocdoni’s anonymous voting system](https://blog.vocdoni.io/vocdoni-technical-overview-v1/)
- The [two token structure of SingularDTV’s SnglsDAO](https://medium.com/singulardtv/two-token-ecosystem-38650a79ce51)

**Application layer**

- [USDC added as collateral](https://blog.makerdao.com/usdc-approved-by-maker-governance-as-the-third-collateral-type-of-the-maker-protocol/) for Maker to help restore DAI to 1:1 parity with USDC and more Dai liquidity in liquidation auctions and MKR auctions. In Maker parlance, liquidation auctions are _flips_, and MKR auctions to cover system deficit are _flops_
- [flops.live](http://flops.live/) to track the MKR auctions
- [Backstop syndicate](https://backstopsyndicate.com/) is live. Pool your DAI to buy MKR at a favorable price, if an auction should drop that low
- NexusMutual [declined claims from Maker liquidated auctions](https://medium.com/nexus-mutual/black-thursday-claims-3d9e74356992) since smart contract cover doesn’t include the risk that only one bot bids on the auction
- [DeFiSaver and liquidated auctions](https://medium.com/defi-saver/black-thursday-at-defi-saver-3c35ea6cd0d0), the oracle delay was a problem but did [12500 ETH worth of Aave flash loan volume](https://medium.com/aave/crypto-black-thursday-the-good-the-bad-and-the-ugly-7f2acebf2b83) over 4000 transactions
- Also check out Covalent if you need [advanced notification as a user](https://www.covalenthq.com/blog/makerdao-liquidation-notifications/)
- Balancer’s [80/20 liquidity pools](https://medium.com/balancer-protocol/80-20-balancer-pools-ad7fed816c8d)
- [Making requests on ErasureBay](https://medium.com/numerai/making-requests-on-erasure-bay-a9e2f9b02ff2)
- OpenLaw: [smart clauses for digital legal agreements](https://medium.com/@OpenLawOfficial/smart-clauses-for-digital-legal-agreements-cc10339684a6)

**Tokens/Business/Regulation**

- Microsponsors: [mint and auction your time as NFTs](https://twitter.com/microsponsors/status/1239965603483418625) on a 0x market
- [Making sense of synthetic assets](https://medium.com/imtoken/defi-explained-synthetic-assets-1733e1072f14) on Ethereum
- Ryan Sean Adams on [Covid-19 and crypto](https://bankless.substack.com/p/bankless-covid-19-prep-plan)
- [Capital markets meltdown signals the birth of DeFi](https://medium.com/@jonathanjoseph/meltdown-in-the-capital-markets-signals-the-birth-of-the-defi-era-5066be3224c2)

**General**

- AZTEC’s [Plookup tables for faster SNARK verification](https://eprint.iacr.org/2020/315.pdf) of digital signatures
- Using [machine learning classifiers and SNARKs to detect improper video transcoding](https://medium.com/livepeer-blog/livepeer-research-photoproof-paper-review-f82788d8e13a) in Livepeer
- Benchmarking [performance of Rescue and Poseidon hash functions](https://ethresear.ch/t/performance-of-rescue-and-poseidon-hash-functions/7161) vs MiMC
- ICL paper says [bZx flash loan attackers left money on the table](https://arxiv.org/abs/2003.03810)
- NYT’s Nathaniel Popper reports on how the [lead dev of Venezuela’s Petro scam got screwed](https://www.nytimes.com/2020/03/20/technology/venezuela-petro-cryptocurrency.html)

* * *

## **Dates of Note**

Upcoming dates of note _(_new in **bold**_)_**:**

_**EthLagos [postponed](https://twitter.com/EthLagos/status/1240282238236884992)**_

- Mar 23 - [Gitcoin Grants CLR, round 5](https://gitcoin.co/grants/) starts
- **Apr 3 - [EEA Mainnet Working Group](https://medium.com/@tasd/first-public-meeting-of-enterprise-ethereum-alliance-mainnet-working-group-scheduled-9ec6c6afc98e) public meeting**
- Apr 3-6 - [NonCon](https://noncon.org/) (Vienna) - [now virtual](https://twitter.com/ParallelePolis/status/1237450754761293830)
- Apr 13 - Deadline to apply for [50k euro for blockchain startup](https://blockchers.eu/open-calls/)s in Europe
- Apr 24-26 - [EthTurin](https://ethturin.com/) - now virtual
- Apr 29-30 - [SoliditySummit](https://solidity-summit.ethereum.org/) (Berlin) - [now virtual](https://twitter.com/ethchris/status/1237833026257764359)
- May 8-9 - [Ethereal Summit](https://www.etherealsummit.com/) (NYC) - [now virtual](https://www.etherealsummit.com/news/join-us-for-the-ethereal-virtual-summit-2020)
- **May 22-31 - [Ethereum Madrid](https://ethereummadrid.com/hackathon-2020-update/) public health virtual hackathon**
- June 17 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

* * *

## **Thank you, ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum News. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

* * *

## **I really want you to link to [weekinethereumnews.com](https://weekinethereumnews.com/)**

Issue permalink: [https://weekinethereumnews.com/week-in-ethereum-news-march-21-2020/](https://weekinethereumnews.com/week-in-ethereum-news-march-21-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

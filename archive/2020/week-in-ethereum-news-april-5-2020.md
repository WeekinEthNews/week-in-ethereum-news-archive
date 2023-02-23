---
title: "Week in Ethereum News<BR> April 5, 2020"
date: "2020-04-05"
---

## **Eth News and Links**

**Eth1**

- Latest [core devs call](https://youtu.be/JqxVvJBhTxo). [Notes](https://twitter.com/TimBeiko/status/1246069932179238912). Discussion of the curve used in eth2 (EIP2537), EVM subroutines (EIP2315), and reducing gas to call precompiles (EIP2046)
- Alex Stokes explains [how eth2 benefits from EIP2537](https://medium.com/@ralexstokes/what-eth2-needs-from-eth1-over-the-next-six-months-86b01863746)
- OpenEthereum has an [initial alpha](https://github.com/openethereum/openethereum/releases/tag/v3.0.0-alpha.1) release
- Updated [tech tree on Stateless Ethereum](https://blog.ethereum.org/2020/04/02/eth1x-stateless-tech-tree/) - what’s needed for improved sync, witnesses, EVM changes, and binary trees

**Eth2**

- Ben Edgington’s latest [what’s new in eth2](https://notes.ethereum.org/@ChihChengLiang/Sk8Zs--CQ/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200403?type=book)
- Danny Ryan’s [quick eth2 update](https://blog.ethereum.org/2020/03/31/eth2-quick-update-no-10/)
- [Bug bounty for the first phase of eth2](https://notes.ethereum.org/@djrtwo/phase0-bounty) is live. Run ‘pip install eth2spec’
- A [Casper FFG explainer](https://www.adiasg.me/2020/03/31/casper-ffg-explainer.html) with proofs of its guaranty of liveness and safety
- Latest [Prysmatic client](https://medium.com/prysmatic-labs/eth-2-0-dev-update-47-multiclient-target-testnet-restart-security-audit-rfp-9c6cf095802c) update - restarting the testnet to run latest spec, RFP for security audits
- Latest [Lighthouse client](https://lighthouse.sigmaprime.io/update-23.html) update - 3x sync speedup, catching a spec bug, prepping for multi-client testnet
- A [report on eth2 staking UX](https://medium.com/empireventures/eth2uxreport-858c73ca1f53)
- [Staking calculator update](https://twitter.com/StakeETH/status/1244992592137326593)

**Layer2**

- [What is Zeropool](https://medium.com/what-is-zeropool/what-is-zeropool-eb94e1540561)? A privacy-first optimistic rollup that functions like a mixer. Next step: rewrite in Rust
- [Burner Wallet on Fuel’s rollup](https://medium.com/@fuellabs/burner-wallet-fuel-7b8ce8e54aff). Check it out on burner.fuel.sh
- Dharma is doing a [rollup chain with interstate](https://blog.dharma.io/dharma-heart-layer-two/?utm_source=weekinethereumnews), using the spec published on ethresearch

**Stuff for developers**

- Analyzing [try/catch in Solidity v0.6](https://forum.openzeppelin.com/t/a-brief-analysis-of-the-new-try-catch-functionality-in-solidity-0-6/2564)
- Calculating [exponents in Solidity](https://medium.com/coinmonks/math-in-solidity-part-5-exponent-and-logarithm-9aef8515136e)
- [Decoding the memory of an Eth contract](https://inuka.dev/decoding-the-memory-of-an-ethereum-contract/)
- [How to use call value](https://medium.com/@luizhamilton29/how-to-use-call-value-7b275ec7f568) and not transfer
- [Best practices when using an oracle](https://medium.com/tellor/best-practices-for-oracle-users-on-ethereum-1ad9e2a43c3b) by Tellor
- Implementing a classifieds [ERC721 market](https://medium.com/coinmonks/how-to-implement-an-erc721-market-f805959ddcf) tutorial
- Constructing a [FootballManager-type simulation for tennis](https://medium.com/coinmonks/lets-make-an-ethereum-simulation-game-part-3-604064fab5da)
- An [iExec quick start guide](https://docs.iex.ec/for-developers/quick-start-for-developers)
- [Using static lookahead analysis to guide fuzzers](https://blog.mythx.io/misc/targeted-fuzzing-using-static-lookahead-analysis-how-to-guide-fuzzers-using-online-static-analysis/) in MythX
- Using [MythX with Embark](https://blog.embarklabs.io/news/2020/04/02/2020-smart-contract-security-analysis-with-mythx/)
- A user [comparison of running and benchmarking MythX, Slither, and Security](https://medium.com/@msolomon44/ethereum-security-analysis-tools-an-introduction-and-comparison-1096194e64d5)
- Samczsun finds an [Aragon bug](https://blog.aragon.one/aragon-court-v1-upgrades/)
- [Easily support hardware wallets](https://blog.blocknative.com/blog/custom-derivation-paths) with Blocknative’s onboard.js
- Fortmatic’s [magic.link](https://magic.link/?ref=weekinethereumnews) for web2 logins without a password (input email -> click link in email -> logged in, even if clicked from different browser/device)
- RicMoo’s [Rooted](https://blog.ricmoo.com/contract-upgrade-wizardry-rooted-cd5c6726132b): deploy a contract and be able to arbitrarily update it. Screens of [Austin Griffith playing with it](https://twitter.com/austingriffith/status/1246096630547243012) on eth.build

**Ecosystem**

- [Ethereum.org is now available on IPFS at ethereum.eth](https://twitter.com/ensdomains/status/1244699514373431296) on Metamask, Status, Opera, or Brave. You may have to type in https://ethereum.eth
- Chart of [Ethereum.org non-English traffic](https://twitter.com/samonchain/status/1245536485597569024)
- [Ethereum Foundation 2019 grant list](https://blog.ethereum.org/2020/04/01/ecosystem-support-program-allocation-update/)
- [Devcon archive](https://archive.devcon.org/) - a permanent site for devcon footage
- [xDai is now a dPOS chain](https://forum.poa.network/t/posdao-activation/3310). Related: [Apple killing local storage frustrates Burner Wallet](https://www.reddit.com/r/ethereum/comments/ft1315/apple_just_killed_local_storage_what_that_means/)

**Enterprise**

- EEA Mainnet Working Group’s [first public call](https://www.youtube.com/watch?v=XAAGGlDGyNY) video
- [One pager on Baseline Protocol](https://docs.google.com/presentation/d/1gMlpY8jPeJRgyB_pzd_HGsmIg5GmJcVCfibhyFwKVGs/edit#slide=id.g7292e0462e_0_0)
- [FundsDLT](https://www.credit-suisse.com/about-us-news/en/articles/media-releases/financial-institutions-team-up-to-develop-fundsdlt--a-groundbrea-202003.html) private chain for investment funds from Credit Suisse Asset Management and Luxembourg Stock Exchange
- [Hitachi to partner with ConsenSys for enterprise adoption](https://consensys.net/blog/press-release/hitachi-solutions-partners-with-consensys-to-bring-enterprise-ethereum-to-the-japanese-market-with-pegasys-plus/) in Japan

**Governance, DAOs, and standards**

- [MakerDAO planning for imminent complete decentralization](https://blog.makerdao.com/what-will-maker-governance-look-like-after-complete-decentralization/)
- The [design philosophy of KyberDAO](https://blog.kyber.network/kyberdao-staking-and-voting-overview-70be71ee58f0)
- [ERC2579](https://github.com/ethereum/EIPs/blob/2fdaf08915accc95aa5babe124a42163f43d65bc/EIPS/eip-2579.md): Merkle Tree Generalized Index
- [ERC2571](https://github.com/ethereum/EIPs/issues/2571): Royalty token standard
- [EIP2584](https://github.com/ethereum/EIPs/pull/2584/files): Trie format transition with overlay trees
- [EIP2583](https://github.com/ethereum/EIPs/pull/2583/files): Penalty for account trie misses

**Application layer**

- [Balancer is live on mainnet](https://medium.com/balancer-protocol/balancer-is-live-4ba2f474131b)
- [Clay Golem](https://blog.golemproject.net/clay-golem-rises/): Task API on mainnet to deploy your own dockerized app 
- [Augur v2 details](https://www.augur.net/blog/augur-v2-deployment-details/): v2 scheduled for June, v1 cutoff now May 15
- Could [prediction markets have prevented the Corona virus pandemic](https://medium.com/sunrise-over-the-merkle-trees/the-potential-of-pandemic-prediction-markets-ac6b6ec2ac98)?
- [Aave interest rate swaps](https://medium.com/opium-network/interest-rate-swaps-now-for-aave-hedge-yourself-or-trade-with-10x-leverage-1fd068c833f5) with Opium Network
- Status’s [web3 browser](https://our.status.im/exploring-the-status-web3-browser/)
- RealT has sold [1m USD of tokenized Detroit real estate](https://medium.com/@TrustlessState/1m-of-real-estate-on-ethereum-9fcebd549280)
- Brave launches a [swag store on Origin Protocol](https://brave.com/brave-launches-new-swag-store-powered-by-origin/)
- Coingecko’s [DeFi book](https://landing.coingecko.com/how-to-defi/) is free this month
- Graph of [DeFi Score vs interest rate](https://twitter.com/JordanLyall/status/1245483054455353345)
- [Livepeer’s opportunity in a socially distanced world](https://medium.com/livepeer-blog/the-rise-of-live-streaming-and-how-livepeer-can-help-a-socially-distanced-world-9ceeb3ef59e1)

**Tokens/Business/Regulation**

- Fat Brands bonds live on mainnet show how [Ethereum will eat Wall Street's settlement layer](https://bankless.substack.com/p/ethereum-will-eat-wall-streets-settlement)
- [USDC grows 50%](https://twitter.com/jerallaire/status/1246249782055763970) in a month

**General**

- Bitmain extends [E3 ASIC through October](https://blog.bitmain.com/en/bitmains-antminer-e3-firmware-update/) with firmware update
- [Binance acquires CoinMarketCap](https://www.coindesk.com/binances-coinmarketcap-acquisition-is-a-bet-that-crypto-really-is-for-the-masses)
- Ligero’s IACR paper: [Lightweight Scalable RSA Modulus Generation with a Dishonest Majority](https://eprint.iacr.org/2020/374)
- [Demystifying Supersonic Snarks](https://research.cryptium.ch/demystifying-supersonic-part-1/)
- [Bilinear accumulators as merkle tree alternative](https://decentralizedthoughts.github.io/2020-04-02-bilinear-accumulators-for-cryptocurrency/), a particular type of polynomial commitments
- [Simple guide to multiexponentiations](https://ethresear.ch/t/simple-guide-to-fast-linear-combinations-aka-multiexponentiations/7238)
- [Open VDF](https://medium.com/supranational/open-vdf-asic-introduction-7d7ad72f200), an architecture of the current hardware design

* * *

## **Dates of Note**

Upcoming dates of note _(_new in **bold**_)_**:**

- Apr 3-6 - [NonCon](https://noncon.org/) - [now virtual](https://twitter.com/ParallelePolis/status/1237450754761293830)
- Apr 7 - [Gitcoin Grants CLR, round 5](https://gitcoin.co/grants/) ends (shameless plug: [my grant](https://gitcoin.co/grants/237/week-in-ethereum-news))
- Apr 13 - Deadline to apply for [50k euro for blockchain startup](https://blockchers.eu/open-calls/)s in Europe
- **Apr 21-23 - [EY Global Blockchain Virtual Summit](https://pub.ey.com/public/2019/1911/1911-3312324/global-blockchain-summit/home.html)**
- Apr 24-26 - [EthTurin](https://ethturin.com/) - now virtual
- Apr 29-30 - [SoliditySummit](https://solidity-summit.ethereum.org/) (Berlin) - [now virtual](https://twitter.com/ethchris/status/1237833026257764359)
- May 8-9 - [Ethereal Summit](https://www.etherealsummit.com/) (NYC) - [now virtual](https://www.etherealsummit.com/news/join-us-for-the-ethereal-virtual-summit-2020)
- May 22-31 - [Ethereum Madrid](https://ethereummadrid.com/hackathon-2020-update/) public health virtual hackathon
- June 17 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

* * *

## **Thank you, ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum News. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

* * *

## **I really want you to link to [weekinethereumnews.com](https://weekinethereumnews.com/)**

Issue permalink: [https://weekinethereumnews.com/week-in-ethereum-news-april-5-2020/](https://weekinethereumnews.com/week-in-ethereum-news-april-5-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

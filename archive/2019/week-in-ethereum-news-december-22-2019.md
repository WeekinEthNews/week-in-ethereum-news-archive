---
title: "Week in Ethereum News <BR> December 22, 2019"
date: "2019-12-23"
---

## **Eth News and Links**

**Eth1**

- [Update your clients for the Muir Glacier hard fork](https://blog.ethereum.org/2019/12/23/ethereum-muir-glacier-upgrade-announcement/) in early January
- Nethermind [v1.3.8](https://github.com/NethermindEth/nethermind/releases/tag/1.3.8) significantly better peer connections stability, can now sync a full node in a few hours. They also have a [Beam Sync prototype](https://twitter.com/nethermindeth/status/1207813525739114506)
- Parity [v2.6.7beta](https://github.com/paritytech/parity-ethereum/releases/tag/v2.6.7) and [v2.5.12stable](https://github.com/paritytech/parity-ethereum/releases/tag/v2.5.12). ready for Muir Glacier
- [EthereumJS VM v4.1.2](https://www.reddit.com/r/ethereum/comments/ed9io6/ethereumjs_vm_v412_with_muirglacier_support/) supports Muir Glacier
- Notes from the [latest eth1 very long-term sustainability call](https://blog.ethereum.org/2019/12/20/eth1x-files-digest-no-1/) on the path forward to stateless Ethereum
- How to [sync an Ethereum node over TOR](https://medium.com/@oaeee/how-to-sync-an-ethereum-node-via-tor-755534775ae1)
- New version of BlockchainsLLC/Slockit’s [Incubed light client now also supports TOR](https://github.com/slockit/in3-server/issues/5)
- Is [state growing faster with block gaslimit of 10m](https://medium.com/@akhounov/is-ethereum-state-growing-faster-now-and-ethereum-state-analytics-project-97777ab47af)? Seems like it, but inconclusive.
- [Ethereum on ARM update](https://www.reddit.com/r/ethereum/comments/eehdjq/ethereum_on_arm_raspberry_pi_4_out_of_memory/): run a full node on Raspberry Pi 4, NanoPC-T4, and RockPro64 boards

**Eth2**

- Latest [what’s new in Eth2](https://notes.ethereum.org/@ChihChengLiang/Sk8Zs--CQ/Sk8Zs--CQ?type=book)
- Danny Ryan’s [quick Eth2 update](https://blog.ethereum.org/2019/12/19/eth2-quick-update-no-6/) - Least Authority spec audit, native nim libp2p, v0.10 spec coming in Jan with standardized BLS
- Latest [implementers call](https://www.youtube.com/watch?v=LYLiqpj-wiE). Notes from [Ben](https://hackmd.io/@benjaminion/rJOaJZFRH) and [Mamy](https://gist.github.com/mratsim/4a07ca7e1ec48188bbb78c8f397a506b).
- Sigma Prime’s [lessons learned from the Lighthouse public testnet](https://lighthouse.sigmaprime.io/update-20.html). Bitfly/Etherchain put up a [block explorer for Lighthouse](https://lighthouse.beaconcha.in/).
- Prysmatic [client update](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-41-prysmatic-labs-856851a1bd28). Better peering, faster syncing, fuzzing the caches. New testnet early Jan
- Ben’s [notes from latest networking call](https://hackmd.io/@benjaminion/SJ3W0qwAH)
- Dankrad’s [primer on data availability checks](https://dankradfeist.de/ethereum/2019/12/20/data-availability-checks.html). Several options on this: [FRI as erasure code fraud proof](https://ethresear.ch/t/fri-as-erasure-code-fraud-proof/6610) and [using polynomial commitment schemes](https://ethresear.ch/t/an-alternative-low-degreeness-proof-using-polynomial-commitment-schemes/6649)
- [cross-shard Eth transfers](https://ethresear.ch/t/a-meta-execution-environment-for-cross-shard-eth-transfers/6656) through a meta execution environment
- Exploring the [2 keys used in Eth2 staking](https://www.attestant.io/posts/exploring-staking-keys/)
- How [eth2 staking is designed to promote decentralization](https://twitter.com/VitalikButerin/status/1207779041970917377)

**Layer2**

- Loopring [launches the first rollup chain](https://twitter.com/loopringorg/status/1208494620214284292), capacity 1400 transactions per second (not yet 2000-3000 because of operator bottleneck)
- [Account-Based anonymous rollup](https://ethresear.ch/t/account-based-anonymous-rollup/6657)
- Perun’s [state channel framework](https://github.com/perun-network/go-perun) in Go

**Stuff for developers**

- Solidity [v0.6](https://github.com/ethereum/solidity/releases/tag/v0.6.0) - “Changes include explicit virtual and override keywords in inheritance, support for try/catch, splitting the fallback function into a receive Ether function and an actual fallback function and limitations on how the length of an array can be changed.” ABIEncoderV2 no longer experimental. Yul optimizer automatically activated.
- Truffle [v5.1.5](https://github.com/trufflesuite/truffle/releases/tag/v5.1.5) compatible with Solidity v0.6
- [Easier deployment with Truffle Teams](https://www.trufflesuite.com/blog/take-control-of-your-deployments-with-truffle-teams) with Metamask and hardware wallets
- AirAssembly [v0.2](https://ethresear.ch/t/airassembly-a-low-level-language-for-zk-starks/6419/4), language for STARKs
- [Base Circom library](https://www.reddit.com/r/ethereum/comments/ecibip/base_circom_library_by_abdk_consulting/)
- MythX: the [journey from slow Python tool to EVM code analysis platfom](https://blog.mythx.io/features/mythx-tech-behind-the-scenes-of-smart-contract-analysis/)
- [decentralized source verification repository](https://chriseth.github.io/notes/articles/closing_the_trust_gap/part3) for better wallet confirmations
- Loredana [released an early version of Pipeline](https://twitter.com/lorecirstea/status/1208380509216288768), visual IDE
- Austin Griffith’s latest eth.build on [transactions and gas prices](https://twitter.com/austingriffith/status/1208083607010467840)
- [3 approaches to permissioning](https://medium.com/coinmonks/guide-to-ownership-and-access-control-in-solidity-f2d99f63c6d4) in Solidity
- [Atomic proxy contract](https://medium.com/@andreafspeziale/atomic-ethereum-blockchain-operations-88043eff5f7b)
- [Test your code from Java using web3j-unit](https://medium.com/web3labs/how-to-test-ethereum-smart-contracts-from-java-using-web3j-unit-2edfb8b877f1)
- EY’s [ERC20 token testing service](https://review-tool.blockchain.ey.com/) is in public beta
- [how EY reduced Nightfall’s gas costs so drastically](https://medium.com/@iAmMichaelConnor/timber-7db8a5130849) by using logs

**Ecosystem**

- Privacy is here: [Tornado.cash v2](https://medium.com/@tornado.cash/tornado-cash-version-2-has-been-released-8c739d3706df). 10 ETH and 1 ETH now supported. Also now supports DAI, with USDC and USDT coming. Plus withdrawals 60% cheaper due to EIP1108 in Istanbul. 1000+ anonymity set and anyone can run a relayer.
- [Private voting and whistleblowing using Semaphore](https://medium.com/@weijiek/private-voting-and-whistleblowing-in-ethereum-using-semaphore-449b376808e)
- Parity announces plans to [assign IP for its Rust client to a DAO](https://www.parity.io/parity-ethereum-openethereum-dao/). Drama ensued, to put it mildly.
- The [Gnosis Safe Multisig launch](https://blog.gnosis.pm/announcing-the-gnosis-safe-multisig-launch-a5d4ab17bd01).
- [Social recovery with Argent](https://medium.com/argenthq/introducing-your-new-argent-security-centre-bf54c1c69380) gets even easier. Plus, Argent’s [Ethereum ecosystem 2020 hype video](https://twitter.com/argentHQ/status/1207316549297754112) is great

**Enterprise**

- Tradeshift Frontiers and Monerium [first cross-border euro transaction](https://monerium.com/monerium/2019/12/18/worlds-first-cross-border-transaction-using-euro-on-blockchain.html). “Invoices and purchase orders were issued through Tradeshift smart-contracts and settled using Monerium e-money on-chain.”
- Seberino: [private blockchains are not pointless](https://medium.com/@cseberino/why-private-blockchains-are-not-pointless-cee91df12489) because of decentralized administration and complete security histories.
- Hyperledger Besu [v1.3.8](https://github.com/hyperledger/besu/releases/tag/1.3.8) better loq query performance

**Governance and standards**

- Control of the [MKR token handed over to MakerDAO](https://blog.makerdao.com/transfer-of-mkr-token-control-a-giant-leap-toward-system-decentralization/)
- Synthetix planning to [decentralize its governance in 2020](https://blog.synthetix.io/transition-to-decentralised-governance/)
- [Deversifi launches its necDAO](https://medium.com/necdao/necdao-launches-on-mainnet-claim-reputation-c11b991560e7) on DAOstack with 17k ETH in the DAO. Reputation received for locking NEC.
- [MetaCartel Ventures](https://github.com/metacartel/MCV/blob/master/Whitepaper.pdf): a Moloch extension for-profit dapp investment fund
- [EIP2442](https://github.com/ethereum/EIPs/blob/5768b03a38a5814121ba2fd4b5f7f85612351168/EIPS/eip-2442.md): LOGQUERY(x) opcode

**Application layer**

- [Buy ads-free Forbes](https://unlock-protocol.com/blog/forbes-ads-free/) for a week or month using Unlock Protocol
- Affogato is doing a [Unisocks-style sale of specialty coffee](https://medium.com/affogato-network/cafe-dynamically-priced-coffee-fc1d0a5ec98d) from Honduras.
- [Roll](https://tryroll.com/social-money-exchange/): a “social money exchange” on Uniswap, aimed at online content creators
- Synthetix is now [using Chainlink oracles](https://blog.synthetix.io/chainlink-decentralizes-first-wave-of-synthetix-price-feeds/)
- Neon District: [Every blockchain game is an MMO](https://medium.com/blockadegames/the-neon-district-token-model-8a0d5896a8e9)
- [Burner Machine](https://burnermachine.com/): spin up 3 hours of an anonymous cloud desktop for $1 in crypto
- ETH being down in the market meant [every set on Set Protocol is up in Eth terms](https://twitter.com/sassal0x/status/1207052673674989568)

**Tokens / Business / Regulation**

- TheGraph: [web3 is going to be the next big platform](https://thegraph.com/blog/the-path-to-web3), and it will start in 2020
- SEC still charging [random ICOs with unregistered security offerings](https://www.sec.gov/news/press-release/2019-267)
- SEC proposes [adding financial sophistication](https://www.sec.gov/news/press-release/2019-265) as criteria for accredited investor status
- [Proof of use](https://codefi.consensys.net/blog/proof-of-use-activating-networks-through-encoded-participation) as standard in token launches
- [ZimDai](https://www.reddit.com/r/ethereum/comments/edmol8/the_people_of_zimbabwe_are_trapped_in_an_abusive/): a plan for Dai adoption in Zimbabwe to offer its citizens a hyperinflation alternative
- 1:1 collateralized [stablecoin for the Nigerian Naira](https://ngnt.org/)

**General**

- [PLONK benchmarks vs Groth16](https://medium.com/aztec-protocol/plonk-benchmarks-2-5x-faster-than-groth16-on-mimc-9e1009f96dfe) on MiMC and SHA-256
- [Byte serialization in blockchains](https://medium.com/whiteblock/byte-serialization-in-blockchain-e147347ab578)
- [Redundancy in Swarm](https://arxiv.org/abs/1912.04269) (arxiv paper)
- [DeFi explained](https://yos.io/2019/12/08/decentralized-finance-explained/). A nice primer
- [Ethereum for dummies](https://simpleaswater.com/ethereum-for-dummies/)
- Surveillance capitalism: [location tracking from your smartphone apps](https://www.nytimes.com/interactive/2019/12/19/opinion/location-tracking-cell-phone.html) (NYTimes)
- Who should own the internet naming system of the future? [ENS as public good](https://medium.com/the-ethereum-name-service/who-should-own-the-naming-system-of-the-future-ens-as-a-public-good-10e4a0ab71d8)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Jan 1 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff-update/)
- Jan 1-30 - [EthIndia online hackathon](https://online.ethindia.co/)
- Jan ~2 - [Muir Glacier upgrade](https://ethernodes.org/muir_glacier) to delay difficulty increase
- Jan 6-20 - Gitcoin [take back the web online hackathon](https://gitcoin.co/hackathon/take-back-the-web/?)
- **Jan 6-21 - [Gitcoin grants](https://gitcoin.co/blog/gitcoin-grants-2020/) quadratic matching**
- Jan 31 - deadline for [EU ledger 200k euro grants](https://fundingbox.com/spaces/ledger-ledger-news-and-updates/5dbfcb7d52317832f85906c8) for blockchain startups
- Feb 14-16 - [ETHDenver](https://www.ethdenver.com/)
- Mar 3-5 - [EthCC](https://ethcc.io/) (Paris)
- Mar 29-Apr4 - [EthLagos](https://ethlagos.io/)
- Apr 3-7 - [Edcon](https://www.edcon.io/) (Vienna)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum News. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

It’s amazing to me how many people email me when every issue has a link at the bottom saying not to email me to get in the newsletter.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **I want your links, because Google needs help: [weekinethereumnews.com](https://weekinethereumnews.com/)**

Archive on the web if you’re linking to it:  [https://weekinethereumnews.com/week-in-eth-news-december-22-2019/](https://weekinethereumnews.com/week-in-eth-news-december-22-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

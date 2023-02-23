---
title: "Week in Ethereum News<BR> April 13, 2020"
date: "2020-04-13"
---

## **Eth News and Links**

**Eth1**

- [EIP1559 fee market change simulations](https://github.com/ethereum/rig/blob/master/eip1559/eip1559.ipynb), assuming demand is exogenous
- [EVM Bytecode Merklization](https://medium.com/ewasm/evm-bytecode-merklization-2a8366ab0c90) - merklize code chunks for block witnesses, estimates 40-60% reduction
- Some more [estimates on code merklization](https://ethresear.ch/t/some-quick-numbers-on-code-merkelization/7260) based on recent blocks

**Eth2**

- Bitfly’s [explanations of eth2 block explorer charts](https://kb.beaconcha.in/charts)
- PegaSys’s [Teku client fully syncs with the Lighthouse testnet](https://twitter.com/benjaminion_xyz/status/1247631816498053120)
- Latest [Nimbus client](https://our.status.im/nimbus-update-april-10/) update. Getting up to the multi-client testnet spec, networking improvements, interop ready with Lighthouse
- SigmaPrime’s update [fuzzing the eth2 clients](https://blog.sigmaprime.io/beacon-fuzz-03.html). Catching bugs, new fuzzing engine
- Work on [formally verifying the eth2 spec using Dafny](https://github.com/PegaSysEng/eth2.0-dafny)
- A look at the GUI for [Rocketpool’s decentralized staking pool](https://medium.com/rocket-pool/development-update-10th-april-72db7824c8e0)
- Aditya’s [how FFG is implemented in Eth2](https://www.adiasg.me/2020/04/09/casper-ffg-in-eth2-0.html) explainer

**Eth2, post-BeaconChain launch**

- A design for [merging eth1 and eth2 clients](https://ethresear.ch/t/eth1-eth2-client-relationship/7248) to turn off PoW
- Better [attestation aggregation algos](https://ethresear.ch/t/attestation-aggregation-heuristics/7265)
- [Verifiable precompiled contracts](https://ethresear.ch/t/verifiable-precompiled-contracts/7242)
- An approach for [cross-shard transfers at EE level](https://ethresear.ch/t/asynchronous-user-level-eth-transfers-over-netted-balance-approach-for-ee-level-eth-transfers/7246)

**Stuff for developers**

- Solidity [v0.6.6](https://github.com/ethereum/solidity/releases/tag/v0.6.6) and [v0.6.5](https://github.com/ethereum/solidity/releases/tag/v0.6.5) - ‘immutable’ new major feature, tuple assignment bugfix, and memory array creation overflow bugfix
- Truffle [v5.1.21](https://github.com/trufflesuite/truffle/releases/tag/v5.1.21) adds Solidity’s immutable
- wighawag’s [Buidler Deployment Plugin](https://github.com/wighawag/buidler-deploy)
- Not new, but a [comparison of ethers.js and web3js](https://github.com/adrianmcli/web3-vs-ethers)
- Example of using [web3modal (former web3connect) with vanilla Javascript](https://www.reddit.com/r/ethdev/comments/fz55ln/web3modal_wallet_connecting_with_vanilla_js/)
- [MelonJS v1](https://medium.com/melonprotocol/melonjs-release-of-version-1-d627d691372c) to interact with Melon’s deployed code
- Tool for [decoding Ethereum storage](https://inuka.dev/an-ethereum-storage-decode-tool/)
- [Arrays and maps in Solidity](https://medium.com/coinmonks/array-and-map-in-solidity-a579b311d74b)
- [Yul+ Remix plugin](https://www.reddit.com/r/ethereum/comments/fxp1mv/easily_write_test_debug_yul_smart_contracts_with/)
- [Chainlink redeployed ETHUSD contract](https://twitter.com/chainlink/status/1248279409183899650); 2 weeks to migrate from old code
- [Maintaining offchain NFT data](https://medium.com/pinata/who-is-responsible-for-nft-data-99fb4e8147e4) using IPFS
- [SQL queries on DuneAnalytics](https://ethereumdev.io/explore-ethereum-data-with-sql-queries-on-dune-analytics/) tutorial
- [Django with web3py](https://medium.com/coinmonks/how-i-integrated-django-with-blockchain-and-built-a-decentralized-application-dapp-f104ae551e12) tutorial

**Ecosystem**

- [discv5](https://vac.dev/kademlia-to-discv5): an explainer of Eth networking’s peer discovery protocol
- [Eth brand survey](https://twitter.com/qnou/status/1245935118616756224)

**Enterprise**

- from the founder of Simple, [Sila](https://techcrunch.com/2020/04/08/programmable-fintech-payments-startup-sila-raises-7-7m-seed-to-wipe-out-ach/): payments API to take on ACH
- [EEA mainnet survey](https://medium.com/@tasd/eea-mainnet-survey-92a4ca7bebdb)
- Hyperledger Besu [v1.4.3](https://github.com/hyperledger/besu/releases/tag/1.4.3) - adds eth/65 for better networking, issue found for private transactions created with v1.3.4 and before

**Governance, DAOs, and standards**

- MakerDAO’s [13 improvement proposals to decentralize](https://blog.makerdao.com/the-first-13-maker-improvement-proposals-to-further-decentralization-of-makerdao) governance
- [TheLAO launches April 28](https://medium.com/@thelaoofficial/building-a-permissionless-silicon-valley-the-lao-launches-on-april-28-25f7837e92c5)
- how to [create a bankless DAO](https://bankless.substack.com/p/how-to-create-a-bankless-dao)
- [EIP2593](https://github.com/ethereum/EIPs/blob/ddb7a6afc477705ffdd8ba8b57774954a7955871/EIPS/eip-x.md): Escalator algo fee market change

**Application layer**

- Reddit is rolling out the [tokenization of it its karma for more than just r/EthTrader](https://medium.com/@MagoTsan/what-are-reddits-blockchain-based-community-points-363117e53733)?
- Status [v1.2](https://our.status.im/status-launches-private-peer-to-peer-messaging-protocol/), adds Waku to replace Whisper for better messaging
- [SmokeSignal.eth](https://www.reddit.com/r/ethereum/comments/fx87gk/in_response_to_the_current_panic_some_governments/), post by burning Dai interface prioritizes higher burn
- Autumated [dollar cost averaging of your stablecoins on Uniswap](https://www.reddit.com/r/ethereum/comments/fx8bso/i_built_a_dapp_to_automate_dollar_cost_averaging/)
- [Suggestions and programs](https://blog.colony.io/suggestions-and-programs/) in Colony
- Overview of DxDAO’s [Omen prediction markets](https://daotalk.org/t/omen-mvp-overview/1229)
- [Inspect](https://inspect.codefi.network/), DeFi transparency registry
- Fairmint’s [continuous securities offering is live on mainnet](https://blog.fairmint.co/fairmint-is-open-for-business/)

**Tokens/Business/Regulation**

- PieDAO’s [BTC++ is live on mainnet](https://www.reddit.com/r/ethereum/comments/fx5cpg/btc_by_piedaoorg_live_on_mainnet/), a token of comprised of multiple versions of locked/synthetic BTC
- Is [tokenized BTC on Ethereum good for ETH](https://bankless.substack.com/p/is-tokenized-btc-bullish-for-eth)?
- [Top 10 use cases of Dai](https://blog.makerdao.com/top-10-use-cases-and-benefits-of-the-dai-stablecoin/)
- [NFTScribe](https://conlan.github.io/nft-scribe/) - attach a message onchain to an NFT while you own it
- a16zcrypto: [crypto’s biz model isn’t that different but who benefits is](https://a16z.com/2020/04/08/crypto-network-effects/)

**General**

- [Chicago DeFi Alliance](https://chicagodefi.org/) formed to connect market makers and DeFi startups
- [CryptoHack](https://cryptohack.org/): online puzzles to learn cryptography
- UTokyo [paper on digital courts](https://www.carf.e.u-tokyo.ac.jp/admin/wp-content/uploads/2020/03/F474.pdf)
- You can join the [trusted setup ceremony for Semaphore](https://twitter.com/weijie_eth/status/1247115346554707969), a zk privacy layer for apps

* * *

## **Dates of Note**

Upcoming dates of note _(_new in **bold**_)_**:**

- **Apr 19 - deadline to apply to EthGlobal’s [HackMoney](https://medium.com/ethglobal/hackmoney-ethglobals-first-online-defi-hackathon-aa6e97815db0) virtual hackathon**
- Apr 21-23 - [EY Global Blockchain Virtual Summit](https://pub.ey.com/public/2019/1911/1911-3312324/global-blockchain-summit/home.html)
- Apr 24-26 - [EthTurin](https://ethturin.com/)
- Apr 29-30 - [SoliditySummit](https://solidity-summit.ethereum.org/) (Berlin)
- May 8-9 - [Ethereal Summit](https://www.etherealsummit.com/) (NYC)
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

Issue permalink: [https://weekinethereumnews.com/week-in-ethereum-news-april-13-2020/](https://weekinethereumnews.com/week-in-ethereum-news-april-13-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

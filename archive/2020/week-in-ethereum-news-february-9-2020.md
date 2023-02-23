---
title: "Week in Ethereum News<BR> February 9, 2020"
date: "2020-02-10"
---

## **Eth News and Links**

**Eth1**

- Latest [core devs call](https://youtu.be/535tJTI0c58). Beiko’s [notes](https://twitter.com/TimBeiko/status/1225780379107368961)
- [EIP1962](https://github.com/saitima/eip1962) generalized elliptic curve and pairing engine implementation in Go
- Nethermind [v1.6.1](https://github.com/NethermindEth/nethermind/releases/tag/1.6.1) - better tip of the chain tracking and reorg handling, JSON RPC bugfixes
- Parity [v2.7.2](https://github.com/paritytech/parity-ethereum/releases/tag/v2.7.2) and the [next steps for Parity client maintenance](https://www.parity.io/contributors-join-openethereum/) under GPL3 (though [reportedly most participants preferred](https://twitter.com/realLedgerwatch/status/1225305288414318594) a more permissive license)
- Slockit’s [Incubed ultralight client server setup](https://in3-setup.slock.it/) wizard

**Eth2**

- Danny Ryan’s [quick eth2 update](https://blog.ethereum.org/2020/02/04/eth2-quick-update-no-8/) - it’s optimization time
- [What’s New in Eth2](https://notes.ethereum.org/@ChihChengLiang/Sk8Zs--CQ/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200207?type=book)
- Latest [eth2 call](https://www.reddit.com/r/ethereum/comments/ezpqyy/live_ethereum_20_call_33_202026_1400_gmt/). Notes from [Mamy](https://gist.github.com/mratsim/1e9feaafd81a2dfa5e7106d08fc2848d) and [Ben](https://hackmd.io/@benjaminion/SyDfdcFGL).
- Jim McDonald: [defining eth2 network metrics](https://www.attestant.io/posts/defining-ethereum-2-network-metrics/)
- A look at [Rocketpool’s GUI](https://medium.com/rocket-pool/development-update-4th-feb-2020-55c1cb7a2ca1)
- Nimbus’ [first mobile testnet](https://twitter.com/m_ratsim/status/1224769743892230151) on Android. Plus part 2 of [building Nimbus on Android](https://our.status.im/building-nimbus-on-android-2/).
- [Eth2 research team ask me anything](https://www.reddit.com/r/ethereum/comments/ez972u/ama_we_are_the_eth_20_research_team_pt_3/) on Reddit

**Layer2**

- [Batch Deposits for \[op/zk\] rollup / mixers / MACI](https://ethresear.ch/t/batch-deposits-for-op-zk-rollup-mixers-maci/6883)
- Matic explains [advantages and limitations of Plasma and rollup](https://blog.matic.network/explaining-plasma-and-rollups-advantages-and-limitations-matic-network/)s

**Stuff for developers**

- Kendrick Tan’s [practical guide to building zk dapps](https://kndrck.co/posts/practical_guide_build_zk_dapps/)
- Kimi Wu’s [hands on your first zk dapp](https://medium.com/coinmonks/hands-on-your-first-zk-application-70fe3a0c0d82)
- OpenZeppelin contracts [v2.5](https://forum.openzeppelin.com/t/openzeppelin-contracts-v2-5/2155) - with CREATE2, enumerableset and big NFT gas savings
- Remix [v0.9.3](https://medium.com/remix-ide/low-level-interactions-on-remix-ide-5f79b05ac86) - you can now test the functionality of receive & fallback functions
- ABDK adds a [number converter to its online toolkit](https://www.reddit.com/r/ethereum/comments/exvahe/ultimate_number_converter_for_ethereum_developers/)
- [ethers.js and Google’s Bigquery](https://github.com/blockchain-etl/ethers.js-bigquery)
- Alethio adds [API endpoints for Rinkeby, Kovan and Ropsten](https://medium.com/alethio/completing-the-web3-development-cycle-with-alethio-3a0b63150ac2) testnets, as well as webhooks
- MythX, Quantstamp, Runtime Verification, Sooho, SmartDec and ConsenSys Diligence starting [Ethereum Trust Alliance, a security rating system](http://ethtrust.org/) for deployed Eth code
- [Time travel queries using a subgraph](https://blocklytics.org/blog/ethereum-blocks-subgraph-made-for-time-travel/) from The Graph
- Brownie now [supports Vyper](https://medium.com/coinmonks/brownie-s-vyper-6cb348cd614f)
- Microsoft’s [Azure Eth development kit](https://azure.microsoft.com/en-us/updates/azure-blockchain-development-kit-for-ethereum-is-now-generally-available/) is now generally available
- A write up of the bug that Sam Sun found in three of [Kyber’s bridge reserves](https://blog.kyber.network/anatomy-of-a-bridge-reserve-smart-contract-vulnerability-and-how-we-fixed-it-fc5c50d13238)
- EthVigil’s [interactive tutorials for devs](https://tutorials.ethvigil.com/) new to Ethereum concepts
- 3Box [Comments and Chatbox plugins now have emojis, likes, and votes](https://medium.com/3box/3box-messaging-plugins-get-more-social-354e2afe88cb)

**Ecosystem**

- [Why ENS uses Ethereum and not a new basechain](https://medium.com/the-ethereum-name-service/why-ens-uses-ethereum-and-eth-not-a-bespoke-blockchain-and-token-36f86727e71f). (Also: ENS’ [registry migration is complete](https://twitter.com/ensdomains/status/1226950669904400384))
- How Whisper-fork [Waku does DNS based discovery](https://vac.dev/dns-based-discovery)
- [ConsenSys lays off 14%](https://consensys.net/blog/press-release/consensys-outlines-strategic-transformation/) as part of strategic transformation
- Matt Leising says he [knows who the DAO hacker is](https://twitter.com/mattleising/status/1224370482822205440)
- [SHPLONK](https://hackmd.io/@tompocock/shplonk), an explainer of last week’s paper from Boneh, Drake, Fisch, and Gabizon

**Enterprise**

- [ConsenSys acquires Heritage Financial Systems](https://www.bloomberg.com/news/articles/2020-02-04/tough-to-disrupt-municipal-market-attracts-blockchain-developer), a municipal bond broker-dealer, to tokenize them on Codefi

**Governance and standards**

- Two articles on DigixDAO dissolution: as an example of [DAOs working](https://www.finder.com.au/what-we-learnt-from-the-rise-and-fall-of-the-digixdao-autonomous-organisation) (though just 58 addresses voted out of 11,000+) and [Coinfund looks at the Digix voting power](https://blog.coinfund.io/digixdao-divorce-story-6ed74b00e2bd)
- Why [ragequit is game changing](https://buymagic.substack.com/p/why-ragequit-is-game-changing)

**Live on mainnet**

- [Colony is in public beta](https://blog.colony.io/the-colony-public-beta-is-live/) live on mainnet
- First [10,000 zkDai is on Aztec](https://medium.com/aztec-protocol/the-first-10-000-zkdai-d499a133b8a0)
- [Mattereum’s asset passports](https://mattereum.com/about/) are live on mainnet
- District0x’s [District Registry](https://blog.district0x.io/presenting-the-district-registry-60a542bc8da7) is live on mainnet, a TCR for its community
- [Coronavirus whistleblower Dr. Li Wenliang is memorialized](https://etherscan.io/address/0x6e46d3ab7335fffb0d14927e0b418cc08fe60505#code) on mainnet
- [AirSwap Delegates](https://medium.com/fluidity/introducing-airswap-delegates-1c3db83be1db) is live on mainnet. Configure automated trading rules, onchain limit orders, liquidity integration with Kyber, and ability to add new tokens

**Application layer**

- DeFi hit [$1 billion USD equivalent locked up](https://defipulse.com/blog/1-billion-tvl-in-defi/)
- Maker [Dai Stability Fee 8%; DSR 7.5%](https://twitter.com/MakerDaiBot/status/1226313689814519808)
- Data viz on [Maker’s Sai to Dai migration success](https://medium.com/alethio/maker-mcd-a-success-in-protocol-upgrade-on-chain-governance-7021874ae4a1)
- A [spreadsheet of admin keys in DeFi](https://www.reddit.com/r/ethfinance/comments/ez8djp/overview_the_admin_keys_still_present_in_most/)
- [Etherisc’s flight insurance app returns](https://blog.etherisc.com/etherisc-to-leverage-chainlink-oracles-for-decentralized-flight-insurance-product-9559b64d79c7) on Rinkeby testnet using Chainlink
- [Idle Finance v2](https://medium.com/@idlefinance/announcing-idle-finance-v2-1c4fb4060a34) (an autobalancer similar to Staked’s [RAY](https://staked.us/v/robo-advisor-yield))
- [Collateral Swap](https://twitter.com/daveytea/status/1224760425272745991) - swap between Maker collateral (eg, ETH<>BAT) with Aave + Uniswap
- [List of DeFiZaps](https://defizap.com/zaps) - one click to do a bunch of DeFi actions
- [Gelato](https://blog.gnosis.pm/bots-on-ethereum-if-you-cant-beat-them-join-them-meet-gelato-774f01bec9d7), a no code bot to automate your Ethereum tasks. [Tutorial](https://medium.com/@gelatofinance/how-to-start-using-your-own-ethereum-bot-no-code-edition-a42752670a00)
- Gauntlet’s analysis of [why Uniswap is a good oracle](https://medium.com/gauntlet-networks/why-is-uniswap-a-good-oracle-22d84e5b0b6c)
- [Credentify](https://credentify.eu/), an API to issue standard European education credentials stacked into ECTS
- [Circles’s universal basic income](https://twitter.com/CirclesUBI/status/1226152510693552130) is live on Kovan testnet
- [Maple Loans](https://medium.com/maple-finance/introducing-maple-loans-200d8245340d) undercollateralized loans through communities with the option to slice up the risk CDO-style
- [Zero Collateral](https://twitter.com/Zer0Collateral/status/1225818856700051456) loans with cDai, live on mainnet (but unaudited alpha software)
- [Dharma’s dtokens](https://blog.dharma.io/introducing-the-dtoken/) - wrappers around Compound tokens, a la rDai, but for services to take profits. In this case, 10% of interest to Dharma

**Tokens/Business/Regulation**

- Hester Peirce [speech proposing an SEC safe harbor for tokens](https://www.sec.gov/news/speech/peirce-remarks-blockress-2020-02-06)
- Op-ed: [America falling behind the world in blockchain](https://www.nationalreview.com/2020/02/blockchain-technology-america-falling-behind-world/)
- [Viewing GDPR](https://media.consensys.net/interpreting-gdpr-through-the-blockchain-lens-f1a1d8ce6fa9) from a blockchain lens
- 6 [central banks to talk digital currency](https://uk.reuters.com/article/us-cenbank-digital/six-central-banks-to-hold-digital-currency-meeting-in-april-nikkei-idUKKBN1ZZ348) in April
- [Ethereum needs more entrepreneurs and product people](https://medium.com/horizin/ethereums-growth-problem-5cab86734917) just as much as more devs
- Are [stablecoins parasites on ETH](https://bankless.substack.com/p/are-stablecoins-parasites-market-ba6)?
- Why [ETH will sustain a monetary premium](https://bankless.substack.com/p/why-eth-will-sustain-a-monetary-premium)

**General**

- Dispelling [Bitcoin maximalist myths about Ethereum](https://medium.com/swlh/ethereum-isnt-decentralized-and-other-myths-ef2d132ee1fe)
- a [visual introduction to Merkle trees](https://blog.iden3.io/merkle-trees-visual-introduction.html)
- [Accelerating powers-of-tau ceremonies with optimistic pipelining](https://ethresear.ch/t/accelerating-powers-of-tau-ceremonies-with-optimistic-pipelining/6870)
- [How does cryptocurrency have value](https://blog.makerdao.com/how-does-cryptocurrency-have-value-and-why-should-i-care/), part 2 of Maker’s intro series

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Feb 8 - [Augur v1 cutoff](https://twitter.com/AugurProject/status/1214545983205494784)
- Feb 14-16 - [ETHDenver](https://www.ethdenver.com/)
- **Feb 18-Mar 31 - [Social Impact hackathon/incubator](https://blockchainforsocialimpact.com/incubator/)**
- **Feb 20 - [NFT.NYC](https://www.nft.nyc/)**
- Feb 20 - [Decentraland launch](https://decentraland.org/blog/announcements/decentraland-announces-publich-launch/)
- blockchain social impact hackathon
- Feb 28-Mar 1 - [ETHLondon UK](https://ethlondon.com/)
- Mar 3-5 - [EthCC](https://ethcc.io/) (Paris)
- Mar 6-8 - [EthParis2020](https://www.hackparis.io/)
- Mar 29-Apr4 - [EthLagos](https://ethlagos.io/)
- Apr 3-7 - [Edcon](https://www.edcon.io/) (Vienna)
- Apr 13 - Deadline to apply for [50k euro for blockchain startup](https://blockchers.eu/open-calls/)s in Europe
- April 24-26 - [EthTurin](https://ethturin.com/)
- May 8-9 - [Ethereal Summit](https://www.etherealsummit.com/) (NYC)
- **May 15-17 - [ETHNYC](https://nyc.ethglobal.co/)**
- May 15 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

* * *

## **Thank you, ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum News. Editorial control has always been me.

* * *

## **I really want you to link to [weekinethereumnews.com](https://weekinethereumnews.com/)**

Issue permalink:  [https://weekinethereumnews.com/week-in-ethereum-news-february-9-2020/](https://weekinethereumnews.com/week-in-ethereum-news-february-9-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness).

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

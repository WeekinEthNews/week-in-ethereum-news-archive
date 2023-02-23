---
title: "Week in Ethereum News <BR> August 17, 2019"
date: "2019-08-18"
---

## **Eth News and Links**

**Layer 1**

- Latest [What’s New in Eth2](https://notes.ethereum.org/c/Sk8Zs--CQ/https%3A%2F%2Fbenjaminion.xyz%2Fnewineth2%2F20190816.html)
- [Demystifying Eth2 terms](https://medium.com/alethio/ethereum-2-0-terms-demystified-8398357429d7) - a solid eth2 explainer in the form of glossary
- Data viz of [Prysmatic’s merged PRs](https://twitter.com/preston_vanloon/status/1162500817850703874)
- [Mothra](https://twitter.com/JonnyRhea/status/1161989070593110017): wrappers for libp2p in rust
- Latest [Eth2 implementer call](https://youtu.be/Av74vZRXeKo?t=428). Notes from [Ben](https://docs.google.com/document/d/197ZK_cyxcwAF3V5yQ7DIPKFJ0zz2VMt7gGiSWbutygg/edit#) and [Mamy](https://gist.github.com/mratsim/5e3f38d04c4c33ae714b30819eacf1c9)

**Stuff for developers**

- Solidity [v0.5.11](https://github.com/ethereum/solidity/releases/tag/v0.5.11). calldata structs bugfix in ABIEncoderV2. Some SMT checker bugs fixed. Internal types added to ABI outputs. Yul/wasm improvements
- Embark [v4.1](https://embark.status.im/news/2019/07/22/whats-new-in-embark-4.1/). better deployment, as well as enabling services from console.
- Integrate [Gas Station Network into your app](https://blog.openzeppelin.com/build-your-app-with-the-gas-station-network/)
- [Onboarding crypto noobs with a link or QR code](https://medium.com/linkdrophq/https-medium-com-linkdrophq-dashboard-launch-d8b3a2c8eec9) that gives them the asset after they download a wallet
- Austin Griffith vid on [Burner Wallet collectibles](https://www.youtube.com/watch?v=-jZIDQcldnY)
- [Benchmarking IPFS gateways](https://aadhi.rocks/benchmarking-ipfs-gateways/)
- [Managing storage with IPFS](https://kauri.io/article/3e8494f4f56f48c4bb77f1f925c6d926) in a Java app
- How to build a [decentralized chat app using Swarm and fds.js](https://blog.datafund.net/chattie-or-how-to-build-a-decentralised-chat-app-in-10-minutes-72ba816b88) in 10 minutes. Here’s a [Swarm progress report](https://medium.com/ethereum-swarm/ethereum-swarm-team-newsletter-july-2019-4f93a7c81f5b)
- Loredana [demo of Pipeline](https://twitter.com/lorecirstea/status/1162745148326973440): drag & drop to create apps. More Loredana demos: [dType 101](https://www.reddit.com/r/ethereum/comments/cpe5of/dtype_101_a_developer_guide_the_anatomy_of_a/) and [web2 MVC architecture emulated on Web3, with dType & Alias](https://youtu.be/4IHDQXuNarA)
- Playing with [dynamic arrays in assembl](https://forum.openzeppelin.com/t/playing-with-dynamic-arrays-in-assembly/1170)y
- How CoinbaseCommerce [uses CREATE2](https://blog.coinbase.com/usdc-payment-processing-in-coinbase-commerce-b1af1c82fb0) to keep costs down
- [Attacking timelocks](https://blog.openzeppelin.com/bypassing-smart-contract-timelocks/) by selling future ownership

**Clients**

- Geth [v1.9.2](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.2)
- Parity [v2.6.1-beta](https://github.com/paritytech/parity-ethereum/releases/tag/v2.6.1) and [v2.5.6-stable](https://github.com/paritytech/parity-ethereum/releases/tag/v2.5.6)
- Pantheon [v1.2.1](https://pegasys.tech/solutions/)
- EVMC [v6.3](https://github.com/ethereum/evmc/releases/tag/v6.3.0)
- [Minimal](https://medium.com/@umbracle/announcing-minimal-f1174616c0be), a modular client written in Go, licensed with Apache or MPL, from Umbracle.

**Ecosystem**

- TrustToken is using GasToken-like technique so end users have [reduced token transfer cost](https://blog.trusttoken.com/gasboost-how-tusd-uses-15-less-gas-than-every-other-stablecoin-929b6a110b27)
- Oracles: DirtProtocol releases [pricefeed oracle protocol](https://twitter.com/yinyinwu/status/1162089347866222593) and UMA on the [economic assurances of their price feeds](https://medium.com/uma-project/umas-data-verification-mechanism-3c5342759eb8)
- Pelle Brændgaard’s [Wardley map of Ethereum](https://chainstrat.substack.com/p/building-a-working-map-of-ethereum)
- [ENS supports TOR’s .onion addresses](https://medium.com/the-ethereum-name-service/ens-now-supports-tor-onion-address-resolution-9bb3bdff6217). Originally an ETHNewYork hack
- [ETHIndia submissions](https://ethindia.devfolio.co/submissions). List of [winners](https://twitter.com/KushalSeth14/status/1158087205597794305).

**Enterprise**

- EEA’s [Mainnet Initiative bridging public and private chains](https://media.consensys.net/enterprise-ethereum-alliances-new-mainnet-initiative-bridges-permissioned-and-public-blockchains-bab7424e4d53)
- PegaSys’ [EthSigner](https://pegasys.tech/protecting-your-ethereum-private-key-with-ethsigner/) - keep your private key separate from dapps/node

**Governance and Standards**

- Latest [core devs call](https://youtu.be/08eaI8JjSbw?t=329). Istanbul split into two forks.
- [EIP tracker](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-1679.md) for what goes in which fork.
- Compound’s vote on next asset to add will use [lifetime interest earned/paid as a weighting mechanism](https://medium.com/compound-finance/select-the-next-compound-asset-9e5e98f26822)
- [Melon Council launches on an Aragon DAO](https://medium.com/melonprotocol/launching-the-melon-council-dao-on-aragonos-42147c86582)
- [EIP2242](https://github.com/ethereum/EIPs/blob/42093a21c0f69781ba6d6bcda0262caa69f5f56c/EIPS/eip-draft_postdata.md): transacton postdata

**Application layer**

- Understanding [emergency shutdown in multi-collateral Dai](https://blog.makerdao.com/introduction-to-emergency-shutdown-in-multi-collateral-dai/)
- Alethio’s [growth of DeFi data viz](https://twitter.com/AlethioEthstats/status/1162426236636938240) is stunning
- [tBTC](https://twitter.com/mhluongo/status/1162481737525583873) - spec for a trustless Eth to Btc bridge from Keep and Summa
- [rDAI](https://www.decentral.ee/2019/08/13/rdai/) - tokenized interest earned by Compound’s cDAI
- Spec for a [multi-token private trading](https://ethresear.ch/t/opaque-mandrake-multi-token-private-pool-inside-ethereum/5965) using snarks.
- [Crypto wallets in the Brave nightly](https://twitter.com/lukemulks/status/1162431747918663680) release, which means they’re a couple months away from the regular release.
- Loopring deployed [beta version of its v3](https://medium.com/loopring-protocol/release-of-loopring-3-0-beta3-and-start-of-security-audit-3e3cdb8d0ad4), which does 350 transactions a second with data availability on chain, and goes up to 1400 txs per second after Istanbul.
- You can now [limit your slippage on Uniswap](https://twitter.com/UniswapExchange/status/1161348478900981761) to prevent frontrunning

**Interviews, Podcasts, Videos, Talks** 

- This section was going to be all podcasts, but it would’ve been mostly the usual suspects. I created a Twitter poll to find out [whether I should keep podcasts in this section](https://twitter.com/evan_van_ness/status/1162959862864764935).

**Tokens / Business / Regulation**

- SEC gets [asset freeze on Veritaseum/Reggie Middleton](https://www.sec.gov/news/press-release/2019-150), which was discussed for years as the most blatant scam
- [Revisiting the fat protocol thesis](https://medium.com/@jonathanjoseph/revisiting-the-fat-protocol-thesis-7ab50718ac56)
- [PIP](https://ethresear.ch/t/public-interest-projects-a-fully-onchain-risk-minimized-seed-funding-mechanism/5977) - Use interest for compound to fund projects in exchange for tokens
- [Discovery of apps](https://our.status.im/this-is-not-a-launch-post/) in Status is live as a bonding curve

**General**

- Electric Capital’s [crypto developer report](https://medium.com/@ElectricCapital/electric-capital-developer-report-h1-2019-7d836d68fecb). Ethereum has 4x the developers of Bitcoin at the protocol level, not even counting Ethereum’s magnitudes of lead at the app level.
- [Coinbase buys Xapo’s institutional](https://blog.coinbase.com/coinbase-custody-acquires-xapos-institutional-business-becoming-the-world-s-largest-crypto-2c1b46fc94c4) business, says it has $7b under management
- ErisX [spot market is live](https://twitter.com/ErisX_Digital/status/1161346433448075264). Bakkt announces [September 23 launch](https://medium.com/bakkt-blog/cleared-to-launch-8dfc3e6f9ed0) date
- MyCrypto on [trust trading Twitter scams](https://medium.com/mycrypto/research-into-trust-trading-scams-on-twitter-ba6309d87a18)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Aug 21-23 - [Dappcon](https://dappcon.io/) (Berlin)
- Aug 23 - [Last day for IDEX withdrawals](https://medium.com/idex/idex-kyc-transition-period-and-updated-asset-availability-for-us-markets-set-to-begin-d45e945f842d) without KYC
- **Aug 24-25 - [EthPlanet Shenzhen](https://twitter.com/Linktimetech/status/1160833156557070336) hackathon**
- Aug 23-25 - [ETHBerlin](https://ethberlinzwei.com/)
- **Aug 28-Sep11 - [Ethereal Blocks](https://hackathons.gitcoin.co/ethereal-blocks/) virtual hackathon**
- Aug 29-30 - [ERC1400 security token hackathon](https://medium.com/@ramvi/invitation-to-hackathon-in-oslo-29-30-august-1d8ec54a26ad) (Oslo)
- Sep 2-16 - [Decentraland SDK virtual hackathon](https://hack.decentraland.org/?with=weekinethereum) (250k USD in prizes. There’s a referral code on that link that gets both you and me something extra)
- Sep 3 - Deadline to [apply for EU Horizon Prize](https://ec.europa.eu/info/funding-tenders/opportunities/portal/screen/opportunities/topic-details/blockchain-eicprize-2019). 1m € each to 5 "Blockchains for Social Good" projects
- Sep 6-8 - [ETHBoston](https://eth.boston/)
- **Sep 10-11 - [DeFi Summit](https://defisumm.it/) (London)**
- Sep 15 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff/)
- Sep 15 - [Ethereal Tel Aviv](https://etherealsummit.com/events/ethereal-tel-aviv/)
- Sep 16 - [Tachyon accelerator application](https://labs.consensys.net/tachyon/) deadline
- Sep 15-16- [StarkWare sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- Sep 22 - [IDEO virtual hackathon](https://coinlist.co/build/ideo) ends
- Oct 7 - [ENS workshop](https://medium.com/the-ethereum-name-service/ens-workshop-applications-are-now-open-f46db6c63384) (Osaka)
- Oct 8-11 - [DeVcon](https://devcon.org/) (Osaka) and [Devcon social events calendar](http://osaka.kickback.events/events/)
- Nov 8-10 - [ETHWaterloo](https://ethwaterloo.com/)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I own 100% Week In Ethereum. Editorial control has always been me.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **I changed the URL to rank for Ethereum News, but people keep linking to the old URL not to  [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/week-in-ethereum-news-august-17-2019/](https://weekinethereumnews.com/week-in-ethereum-news-august-17-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

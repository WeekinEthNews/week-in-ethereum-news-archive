---
title: "Week in Ethereum News <br> May 6, 2023"
date: "2023-05-06"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest consensus layer devs [call video](https://www.youtube.com/watch?v=RZnf3K1i3NM&t=176s). Notes from [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-consensus-call-108/):
    - Discussions on CL max blobs per block and EL using SSZ or RLP to encode blob transactions

- EIP4844:
    - EIP4844 [readiness checklist](https://github.com/ethereum/pm/blob/master/Breakout-Room/4844-readiness-checklist.md)
    
    - Latest EIP4844 implementer [call video](https://www.youtube.com/watch?v=M2pYYEtM3Gw&t=2s). Notes from [Terence](https://twitter.com/terencechain/status/1653105610572075008)
    
    - [Blob transaction encoding options](https://hackmd.io/nz-IqXLPQ-yahFPFlPl62A): EIP6493, EL specific SSZ or RLP based

- [KZG ceremony has over 95,000 contributions](https://ceremony.ethereum.org/), you can contribute with GitHub and/or an account that has made 32 mainnet transactions, the lobby is regularly empty

- Tim Beiko’s [Core Devs update](https://tim.mirror.xyz/8hWUEmXWt-ZYNh4UlU4dMhsV9aNo26oNigCuy-z1k38): summary of included & candidate EIPs for Dencun

**Layer 1**

- EF bug bounty program: [execution layer](https://github.com/ethereum/public-disclosures/blob/master/disclosures/EL-2023-05-03.md) & [consensus layer](https://github.com/ethereum/public-disclosures/blob/master/disclosures/CL-2023-05-03.md) disclosed vulnerabilities

- Verkle implementers [call notes](https://docs.google.com/document/d/1D2GtzI3q9btZd1ZOzCsWPsvzCaA-fCLZdXDtawoPUyM/edit#heading=h.mat4jp8l6adl): [Beverly Hills testnet](https://twitter.com/gballet/status/1654560525362114567) shuts down May 12

- [Proposal for warm/cold account balances](https://ethereum-magicians.org/t/value-bearing-calls-are-priced-unfairly-warm-cold-account-balances-proposal/14100), CALL with value has 6700 gas stipend

- Ben Edgington’s Upgrading Ethereum book [Capella update](https://eth2book.info/capella/)

**Client releases**

- Consensus layer:
    - Lodestar [v1.8.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.8.0): Obol distributed validator support and gossip queue enhancements

- Execution layer:
    - Besu [v23.4.0](https://github.com/hyperledger/besu/releases/tag/23.4.0): improvements to database performance, logging, metrics, EVM performance and gas estimation; deprecates GoQuorum-compatible privacy modes & IBFT1.0
    
    - Nethermind [v1.18.0](https://github.com/NethermindEth/nethermind/releases/tag/1.18.0): reduced memory usage, experimental reduced full pruning time, improved sync time & block processing

**Research**

- [MEV-Boost bid cancellations](https://ethresear.ch/t/bid-cancellations-considered-harmful/15500) considered harmful

**Layer 2**

- Aztec [hybrid zkRollup roadmap](https://medium.com/aztec-protocol/aztec-the-hybrid-zkrollup-a90a197bf22e): public & private state, not EVM compatible, UTXOs represent data, contracts written in Noir, local testnet Q3, public testnet 2024

- James Prestwich: [shared sequencing for optimistic rollups](https://prestwich.substack.com/p/the-definitive-guide-to-sequencing)

**EIPs/Standards**

- Discussion on [EIP/ERC numbering](https://github.com/ethereum/EIPs/issues/6990)

- EIPs:
    - [EIP6963](https://github.com/ethereum/EIPs/pull/6963/files): Multi-injected provider interface (MIPI)
    
    - [EIP6968](https://github.com/ethereum/EIPs/pull/6969/files): Contract secured revenue on an EVM based L2
    
    - [EIP6988](https://github.com/ethereum/EIPs/pull/6988/files): Slashed validator cannot be elected as a block proposer

- ERCs:
    - [ERC6956](https://github.com/ethereum/EIPs/pull/6956/files): Asset-bound NFTs
    
    - [ERC6960](https://github.com/ethereum/EIPs/pull/6960/files): Dual-layer token
    
    - [ERC6981](https://github.com/ethereum/EIPs/pull/6981/files): Reserved ownership accounts
    
    - [ERC6982](https://github.com/ethereum/EIPs/pull/6982/files): Minimalistic efficient lockable tokens

**Stuff for developers**

- Foundry:
    - [Symbolic testing of Foundry projects](https://hackmd.io/@SaferMaker/EVM-Sym-Test) using Halmos, hevm, KEVM & EthBMC/Foundry
    
    - [Forge-exec](https://github.com/wighawag/forge-exec#readme): interact using languages such as JavaScript & Rust via IPC, requires ffi
    
    - [Add Foundry](https://twitter.com/jtriley_eth/status/1653885929592090625) to existing project without forge init
    
    - Tip: [use makeAddr & makeAddrAndKey cheats](https://twitter.com/PaulRBerg/status/1654573378152349697) to create accounts from a string

- RareSkills [Solidity tutorial](https://www.rareskills.io/learn-solidity) for web2 devs, using Remix & Foundry

- [Multi-contract reentrancy locks](https://medium.com/@elliotfriedman3/multi-contract-reentrancy-locks-8c12934e30ab) using a global contract with multiple lock levels, unaudited

- Secureum RACE #17: [8 question Solidity quiz & answers](https://ventral.digital/posts/2023/5/1/race-17-of-the-secureum-bootcamp-epoch-infinity)

- OpenZeppelin Ethernaut: [Switch](https://twitter.com/openzeppelin/status/1653412591572746240) level [solution](https://blog.softbinator.com/solving-ethernaut-level-29-switch/)

- [Artemis](https://github.com/paradigmxyz/artemis#readme): MEV bot framework in Rust, includes strategy for Seaport & Sudoswap NFT arbitrage

- Guide to [searching on Flashbots MEV-Share](https://writings.flashbots.net/searching-on-mev-share)

**Security**

- DEI stablecoin on Arbitrum [exploit](https://twitter.com/adamb83024264/status/1654558408803250176), simple implementation error

- yAcademy: [common DeFi forked protocol bugs](https://github.com/YAcademy-Residents/defi-fork-bugs#readme)

**Ecosystem**

- [Median gas returned to May 2022 level](https://twitter.com/hildobby_/status/1654103974516015104) driven by meme coins

- [Ethereum.org writers cohort](https://ethereumwriterscohort.carrd.co/) starts May 11  
    

**Enterprise**

- [Stripe onramp](https://stripe.com/en-au/newsroom/news/fiat-to-crypto-onramp) via embeddable widget or no code link for ETH & USDC on mainnet, US only

- [Sotheby’s Metaverse secondary NFT marketplace](https://twitter.com/Sothebysverse/status/1653049950786265094) on mainnet, supports creator royalties

**Notable at app layer**

- [Curve USD stablecoin deployed](https://github.com/curvefi/curve-stablecoin/blob/master/deployment-logs/mainnet.log); redeployed after [missing fees](https://twitter.com/curvefinance/status/1654060060090179585) & [high gas usage](https://twitter.com/CurveFinance/status/1654214766104027138)

- [Dump Services](https://dump.services/): sell multiple tokens in a single transaction using CoW protocol

- [Blend](https://www.paradigm.xyz/2023/05/blend): Blur NFT perpetual lending with no oracles & no expiries, borrow or buy now pay later

- Zapper [onchain activity feed](https://twitter.com/zapper_fi/status/1654165559137665039)

- Umbra adds [LUSD and RAI for stealth payments](https://twitter.com/UmbraCash/status/1653440435514114077)

* * *

### Job Listings

- Mimic seek a [blockchain engineer](https://mimic-fi.notion.site/Blockchain-engineer-f70df67acbba4dd1a39e974767f9c709)

- Solidity team need a highly skilled [Developer Advocate](https://jobs.lever.co/ethereumfoundation/b9e33c9e-48ee-464f-a672-d51eece2b99d)

- [Snr React Native UI Dev](https://grnh.se/2fada6031us) at Status: [All jobs](https://grnh.se/9fc6e6fc1us)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Biden [proposal for crypto mining tax](https://www.whitehouse.gov/cea/written-materials/2023/05/02/cost-of-cryptomining-dame-tax/) equal to 30% of electricity costs

- [Poloniex $7.6 million settlement](https://ofac.treasury.gov/recent-actions/20230501_33) with OFAC

- [Coinbase International Exchange](https://www.coinbase.com/blog/introducing-coinbase-international-exchange): perpetual futures exchange launched in Bermuda for non-US institutional users

**General/crypto**

- [AT&T email accounts hacked](https://techcrunch.com/2023/04/26/hackers-are-breaking-into-att-email-accounts-to-steal-cryptocurrency/) to steal users crypto

- [ZKML](https://mirror.xyz/privacy-scaling-explorations.eth/K88lOS4XegJGzMoav9K5bLuT9Zhn3Hz2KkhB3ITq-m8): convert TensorFlow Keras models into zk-compatible versions, proof of concept

- [Plonk](https://www.notamonadtutorial.com/all-you-wanted-to-know-about-plonk/) explainer

- Make sure to update to [latest iOS and MacOS updates](https://www.macrumors.com/2023/05/01/rapid-security-response-16-4-1/) 

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-may-6-2023](https://weekinethereumnews.com/week-in-ethereum-news-may-6-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- **May 7 – Zuzalu** [**CryptoXai.wtf**](https://zuzalu.city/event/94/session/633) **(livestream)**

- May 9 – [Gitcoin Grants Beta Round](https://grants.gitcoin.co/) ends (support [Week in Eth News](https://explorer.gitcoin.co/#/round/1/0xaa40e2e5c8df03d792a52b5458959c320f86ca18/0xaa40e2e5c8df03d792a52b5458959c320f86ca18-53))

- May 9-12 – [EY blockchain summit](https://web.cvent.com/event/c066d44d-4e50-4d7e-b6fb-3cc0abdae7ff/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7)

- May 11-14 – [Pragma Lisbon](https://ethglobal.com/events/pragma-lisbon) & [ETHGlobal Lisbon](https://ethglobal.com/events/lisbon) hackathon

- May 19-23 – [EDCON](https://edcon.io/) Montenegro (changed from Vienna)

- May 20-21 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 24-26 – [Spaghett ETH](https://naples.spaghett-eth.com/) (Naples) conference

- May 26-28 – [ETHDublin](https://www.ethdublin.io/) hackathon

- Jun 2-4 – [ETH Seoul](https://2023.ethseoul.org/)

- Jun 2-7 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 9-11 – [ETHPrague](https://ethprague.com/) conference & hackathon

- Jun 23–25 – [ETHGlobal Waterloo](https://ethglobal.com/events/waterloo2023) (changed from Toronto)

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Aug 13-16 – [ETHToronto](https://www.ethtoronto.ca/) & [ETHWomen](https://www.ethwomen.com/)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org/) (Buenos Aires)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 30 – Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 18-21 – [ETH Montréal](https://ethmontreal.xyz/) hackathon & conference

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6–27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 27–29 – [ETH Miami](https://ethmiami.net/) festival + hackathon

- Oct 28–30 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- **Nov 3-5 –** [**ETHBrno**](https://twitter.com/ethbrno/status/1652198745902137344)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 17-19 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

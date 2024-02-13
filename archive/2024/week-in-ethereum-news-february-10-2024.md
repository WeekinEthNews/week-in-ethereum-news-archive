---
title: "Week in Ethereum News <br> February 10, 2024"
date: "2024-02-09"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=FLB61CpMB70&t=235s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-127/):
    - **Mainnet Dencun upgrade set for March 13 epoch 269568**, client releases in 2 weeks
    
    - **Goerli testnet**: tested blob expiry with nodes using checkpoint sync
    
    - **Invalid blocks**: triggering MEV-Boost circuit breaker to local building discussion
    
    - **Electra upgrade scope** (small cross layer fork targeting late 2024):
        - Priorities & complexities of potential features: SSZification EIPs, ePBS, inclusion lists (EIP7547) and increase max EB (EIP7251); breakout calls planned
        
        - peerDAS (EIP7594) can be developed in parallel to Electra

- Holešky testnet [uneventfully upgraded](https://twitter.com/ethpandaops/status/1755197602931327379) to Dencun

- Dencun interop testing [call video](https://www.youtube.com/watch?v=RoQ6Gy-KbUs&t=5s): testing churn limit on Holešky testnet & shadowfork planned with mainnet releases

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.59%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: **Geth 72% supermajority**, could cause a chain split
        - [**Supermajority dashboard**](https://supermajority.info/)**: simulate node operators changing to minority clients**
    
    - Consensus layer: Prysm 39%, any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Toni Wahrstätter & Vitalik: [options to increase block gas limit](https://ethresear.ch/t/on-increasing-the-block-gas-limit/18567) via increasing calldata cost; incentivize L2s to use blobs for data availability

- [bloXroute relay in optimistic mode broadcast invalid blocks](https://gist.github.com/benhenryhunter/5f63ad6b5d68452192e9965925b9878e#file-postmortem-md) built by rsync builder on Feb 6 resulting in 9 missed slots

- Reth [roadmap](https://docs.google.com/presentation/d/1K4Hejbp3Q6aPLw5CWuSboMvN8g3nCflJ_gN_kzz-0ww) (EL client in Rust): targeting v0.2 beta late Feb & v1 production by end of April

**Research**

- Overview of [spec changes for inclusion lists](https://notes.ethereum.org/@mikeneuder/il-spec-overview)

**Client releases**

- Consensus layer:
    - Lodestar [v1.15.1](https://github.com/ChainSafe/lodestar/releases/tag/v1.15.1): hotfixes for Besu users, blindedLocal & lock file issues

- Execution layer:
    - Geth [v1.13.12](https://github.com/ethereum/go-ethereum/releases/tag/v1.13.12): mainnet Dencun upgrade
        - [Era1 initial implementation](https://github.com/ethereum/go-ethereum/pull/26621), provides Execution Layer data history pre-merge; post-merge Execution Layer data is encapsulated within Beacon chain Era files
    
    - Reth [v0.1.0-alpha.17](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.17): critical fixes for Dencun, sidechain root validation & networking improvements

**For stakers**

- Remy Roy: [guide to migrating a validator to a larger disk](https://github.com/eth-educators/ethstaker-guides/blob/main/migrating-to-a-larger-disk.md)

**Layer 2**

- Polygon [Type 1 Prover](https://polygon.technology/blog/upgrade-every-evm-chain-to-zk-introducing-the-type-1-prover) open sourced

- RollCall (L2 standards) precompiles [breakout call](https://www.youtube.com/watch?v=tg01COfxi_M) and [notes](https://ethereum-magicians.org/t/rollcall-breakout-3-precompiles-and-the-rip-process/18508/3): secp256r1 precompile (RIP7212) live on Polygon testnet and rollup precompile registry in progress

**EIPs/Standards**

- EIPs:
    - [EIP7612](https://github.com/ethereum/EIPs/pull/8162/files): State storage transition using an overlay tree
    
    - [EIP7619](https://github.com/ethereum/EIPs/pull/8190/files): Precompile Falcon512 generic verifier

- RIPs (Rollup Improvement Proposals):
    - [RIP7614](https://github.com/ethereum/RIPs/pull/10/files): Expose call stack to contracts

- ERCs (application layer):
    - [ERC7613](https://github.com/ethereum/ERCs/pull/236/files): Puppet proxy contract
    
    - [ERC7615](https://github.com/ethereum/ERCs/pull/235/files): Atomic push-based data feed among contracts
    
    - [ERC7616](https://github.com/ethereum/ERCs/pull/244/files): Hybrid fungible token
    
    - [ERC7617](https://github.com/ethereum/ERCs/pull/245/files): Chunk support for ERC5219 mode in web3 URL
    
    - [ERC7618](https://github.com/ethereum/ERCs/pull/246/files): Content encoding in ERC5219 mode web3 URL

**Stuff for developers**

- [EthereumJS releases](https://twitter.com/efjavascript/status/1755920124605759824): Dencun upgrade support, WASM used by default for crypto primitives, RPCStateManager, expanded EIP1186 proof functionality and Tx addSignature API

- Gaslite Merkle Drop base contracts: [GasliteMerkleDN](https://github.com/PopPunkLLC/gaslite-core/blob/main/src/GasliteMerkleDN.sol) (native tokens) & [GasliteMerkleDT](https://github.com/PopPunkLLC/gaslite-core/blob/main/src/GasliteMerkleDT.sol) (ERC20)

- Ethers js [v6.11.0](https://github.com/ethers-io/ethers.js/releases/tag/v6.11.0): adds EIP4844 blob transactions

- [Ethers-kt](https://github.com/Kr1ptal/ethers-kt#readme) (Kotlin): async library for EVM interaction, targets JVM & Android platforms

**Ecosystem**

- [Ethereum Protocol Fellowship study group](https://blog.ethereum.org/2024/02/07/epf-study-group), 10 week series starts Feb 19, research & development tracks, precursor to fifth cohort

- Ethereum Foundation [academic grants round](https://esp.ethereum.foundation/academic-grants), $1M available

* * *

### Job Listings

- Status is hiring: Technical Chief Operating Officer - [Apply here](https://grnh.se/0ecdaa981us)

- Nethermind: [Distributed System Engineer](https://grnh.se/893258d2teu) (DSE) and [Cryptography Researcher](https://grnh.se/51fa8652teu)

- EF seek an [Executive Assistant](https://jobs.lever.co/ethereumfoundation/444bc50a-236e-4a4e-8385-c0454b0044e9) to support senior decision makers

- Sourcify seek a [TypeScript Developer](https://jobs.lever.co/ethereumfoundation/fbcb2cf8-cd58-4140-ab3a-47a402616d50)

- Solidity: [C++ Software Engineer](https://jobs.lever.co/ethereumfoundation/a6e4598e-6c12-493e-8426-438cb0a5eeca) and [Programming Language Researcher](https://jobs.lever.co/ethereumfoundation/d510dfd7-d5dd-435c-9111-1c50112715c1)

- MetaMask Staking: [Staff Software Engineer](https://grnh.se/533bf5521us) and [Software Engineer](https://grnh.se/7efeff9b1us)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 9.4 to 367 gwei, with 35.2 gwei average
    - Zero net issuance currently at 22.2 gwei 
    
    - 10.1k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,279 - $2,522, currently $2,495

- [ETHBTC](https://ratiogang.com/): currently 0.053 (Flippening at ~0.16)

**Notable at app layer**

- [GoDaddy](https://aboutus.godaddy.net/newsroom/company-news/news-details/2024/GoDaddy-and-Ethereum-Name-Service-Bridge-the-Gap-Between-Domain-Names-and-Crypto-Wallets/default.aspx) integrated with ENS, users can associate an address with their domain name

- POAP [Collections](https://blog.poap.xyz/collections/): curate groups of POAPs

- Kain Warwick: [Synthetix 2024 roadmap](https://mirror.xyz/kain.eth/kuLEnkUhJBPdJCs9gSIQ2_umGprJq3ZZCExmtc69zn8)

- Brice [reflects on app governance](http://tokenbrice.xyz/farewell-glc/) upon leaving GHO liquidity committee

- Gitcoin Grants [proposed updates](https://gov.gitcoin.co/t/gitcoin-grants-proposed-updates/17649): refocus on open source software & ETH infrastructure with rounds every 6 months & $1M matching pool, communities can run their own web3 community & education rounds

**Regulation/business/tokens**

- [SEC “dealer” rule finalized](https://www.sec.gov/news/press-release/2024-14), excludes those with/controlling less than $50M in assets

- Jake Chervinsky: [state of crypto vs SEC](https://twitter.com/jchervinsky/status/1755241769514705126)

- Kain Warwick: [SEC response to ICOs](https://twitter.com/kaiynne/status/1754360250491445612) created worse outcomes than if they had done nothing

**General**

- Josh Stark: [Trust Experience](https://stark.mirror.xyz/rkLEVz9p4r3ouusD-WCkWP_iVZYkZ0K7TFkzeRfiXCU) shape expectations of future blockchain behavior

- Vitalik: [authenticate people by asking security questions](https://vitalik.eth.limo/general/2024/02/09/securityquestions.html) to mitigate deep fakes

- [Constant-size zk-SNARKs in ROM](https://eprint.iacr.org/2024/173) from Falsifiable Assumptions

* * *

Publisher & Founder: [@evan van ness](https://twitter.com/evan_van_ness); Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-february-10-2024](https://weekinethereumnews.com/week-in-ethereum-news-february-10-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- **Feb 19 –** [**Ethereum Protocol Fellowship study group**](https://blog.ethereum.org/2024/02/07/epf-study-group) **10 week series starts**

- Feb 23-Mar 3 – [ETHDenver](https://www.ethdenver.com/) BUIDLWeek & hackathon

- **Mar 5 –** [**EF academic grants round**](https://esp.ethereum.foundation/academic-grants) **application deadline**

- **Mar 13 –** [**mainnet Dencun upgrade**](https://eips.ethereum.org/EIPS/eip-7569#activation) **epoch** [**269568**](https://beaconcha.in/epoch/269568)

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024) hackathon

- Mar 19-21 – [ETH Canal](http://ethcanal.xyz) (Panama City, Panamá) conference & hackathon

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- Mar 22-24 – [ETHSamba](https://ethsamba.org/) (Rio)

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) conference & hackathon

- Mar 29-31 – [ETH Seoul](https://www.ethseoul.org/) hackathon

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) virtual hackathon

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Apr 12-14 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- **Apr 16-18 –** [**EY Global blockchain summit**](https://web.cvent.com/event/e0ad2c12-3e65-41a9-bafb-a436754cf4ae/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7) **(London)**

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/) hackathon

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- Jun 3-5 – [ETH Belgrade](https://ethbelgrade.rs/) conference

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 26-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

---
title: "Week in Ethereum News <br> December 14, 2024"
date: "2024-12-14"
---

## Eth News and Links

Stakers can increase gas limit to 36M

**Eth R&D protocol call (All Core Devs)**

- [Consensus layer focused protocol call](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-147-december-12-2024/22161) (ACDC #147):
    - **Pectra upgrade:**
        - [**Mekong testnet**](https://mekong.ethpandaops.io/): stable, gas limit increased to 36M
        
        - **Gas limit increase**: restricted by gossip limit, consensus layer teams to check spec conformity & consider how best to handle gas/gossip limits, gossip limit won’t be increased for now
        
        - [**Pectra-devnet-5 spec**](https://notes.ethereum.org/@ethpandaops/pectra-devnet-5):
            - Aim to launch over the holidays
            
            - **EIP7742 uncouple blob count between CL/EL**: replaced by EIP7840 execution layer config to set max & target blob count
            
            - **EIP7251 max effective balance**: minor changes
            
            - **EIP7762 increase min base fee**: not included, L2s work around
            
            - **EIP2537 BLS precompile:** gas repricing proposed, final MSM benchmarks required before ACDE next week
    
    - **Fusaka upgrade:**
        - PeerDAS rebasing on top of Pectra
    
    - **CFI/SFI statuses**: considered for inclusion (CFI) EIPs should be in a future upgrade devnet & scheduled for inclusion (SFI) EIPs will be in the next upgrade devnet

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- [Client testing call #16](https://ethereum-magicians.org/t/client-testing-call-16-december-9-2024/22137): Mekong testnet 98% participation, minor changes in pectra-devnet-5 spec and consensus layer client teams discussed gossip limit

[**Fusaka**](https://eips.ethereum.org/EIPS/eip-7607) **(Osaka + Fulu) upgrade**

- [EOF implementers call #63](https://ethereum-magicians.org/t/eof-implementers-call-62-november-27-2024/21543): Solidity working on EOF as experimental feature and discussed metadata section

**Layer 1**

- Toni Wahrstätter: [increase gas limit to 36M](https://x.com/nero_eth/status/1867158840715993549), beyond 40M currently unsafe due to gossip limit, review again after Pectra upgrade
    - [Prysm cannot set gas limit](https://github.com/prysmaticlabs/prysm/issues/14721) through validator client currently

- [FOCIL breakout #1](https://ethereum-magicians.org/t/focil-breakout-1-december-13-2024/22160): consensus layer spec relatively stable, aim for devnet at end of January

- [L1 R&D workshops](https://github.com/ethereum/pm/tree/master/Breakout-Room-Meetings/DevconSEA/R%26D-workshop): notes from pre-Devcon workshops

**Research**

- [Execution Tickets evaluated using agent-based simulation](https://ethresear.ch/t/agent-based-simulation-of-execution-tickets/21254): validator decentralization & MEV capture is promising but questions remain for builder centralization, off-chain agreements & multi-block MEV

- [EF academic grants round](https://blog.ethereum.org/2024/12/10/academic-grants-22): summary of 39 completed & in progress results from 2022 grants

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.4%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~43% & Nethermind ~36% (estimate based on 74% self reported data)
    
    - Consensus layer: Prysm 35%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Client Releases**

- Consensus layer:
    - Nimbus [v24.12.0](https://github.com/status-im/nimbus-eth2/releases/tag/v24.12.0): adds reading bootstrap nodes yaml
    
    - Teku [v24.12.0](https://github.com/Consensys/teku/releases/tag/24.12.0): block publishing performance improved

- Execution layer:
    - Besu [v24.12.0](https://github.com/hyperledger/besu/releases/tag/24.12.0): breaking changes including metric name updates
    
    - Erigon [v3.0.0-alpha6](https://erigon.tech/announcing-erigon-v3-alpha-6-focus-on-staking-and-full-node-performance/): default mode changed from archive to full node, adds minimal prune mode for low disk space users and performance improvements
    
    - Nethermind [v1.30.0](https://github.com/NethermindEth/nethermind/releases/tag/1.30.0): default gas limit increased to 36M and adds Taiko & Linea L2 support; [v1.30.1](https://github.com/NethermindEth/nethermind/releases/tag/1.30.1): startup fix
    
    - Reth [v1.1.3](https://github.com/paradigmxyz/reth/releases/tag/v1.1.3): breaking API changes, adds NodePrimitives (primitive trait abstraction) to several components; [v1.1.4](https://github.com/paradigmxyz/reth/releases/tag/v1.1.4): op-reth fix

**Layer 2**

- [RollCall #9](https://ethereum-magicians.org/t/rollcall-9-december-11-2024/21322) (L2 standards):
    - Pectra upgrade: L2s don’t use or can work around fee history being removed and are ok with not including EIP7762 as they work around min blob base fee
    
    - Overview of L2 execution common core project

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7839](https://github.com/ethereum/EIPs/pull/9128/files): Unified network configuration (EL to fetch config from CL at startup)
    
    - [EIP7840](https://github.com/ethereum/EIPs/pull/9129/files): Add blob schedule to EL config files

- ERCs (application layer):
    - [ERC7837](https://github.com/ethereum/ERCs/pull/759/files): Diffusive tokens
    
    - [ERC7838](https://github.com/ethereum/ERCs/pull/762/files): Instruction specific address
    
    - [ERC7841](https://github.com/ethereum/ERCs/pull/766/files): Cross-chain message format and mailbox

**Stuff for developers**

- Ape [v0.8.22](https://x.com/apeframework/status/1866941701866373552) (Python contract framework): 2x faster checksumming, updated isolation and adds support for web3.py v7 & python v3.13

- Heimdall-rs [v0.8.5](https://x.com/BeckerrJon/status/1866936001026986030): adds LLM postprocessing to decompiler

- CTFs:
    - [Secureum RACE #35](https://ventral.digital/posts/2024/12/10/race-35-of-the-secureum-bootcamp-epoch-infinity/): answers to 8 question Solidity quiz

- [Safe multisig transaction hashes](https://github.com/pcaversaccio/safe-tx-hashes-util/pull/10) (Bash script): adds support for offchain message hashes

**Security**

- Clober (DEX) [$500k exploit](https://rekt.news/cloberdex-rekt/) on Base via reentrancy

- 1inch [resolver contract exploit](https://blog.1inch.io/1inch-promptly-responds-to-an-unauthorized-access-incident/) via private key compromise

- Radiant Capital [October $50M exploit update](https://medium.com/@RadiantCapital/radiant-capital-incident-update-e56d8c23829e), developer shared zipped PDF containing macOS malware received from impersonator of former contractor

* * *

### Job Listings

- Mimic: [Tech Lead Engineer](https://mimic-fi.notion.site/Tech-Lead-Engineer-14b9958dbf4d80d88dadf252126e6375)

- Vyper (Pythonic EVM language) seek a [DevRel](https://e63fu2j2ew4.typeform.com/to/Rt6A2juT)

**Job listings: $600 for 4 issues** (75 char limit). [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.** Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 6.1 to 226.6 gwei, 18.7 gwei average; zero net issuance at 24.1 gwei
    
    - 4.4k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,538 - $4,021, currently $3,921 all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.039 (Flippening at ~0.164)

**Ecosystem**

- [ETHIndia](https://twitter.com/ETHIndiaco/status/1866098806758252987) top ten hackathon projects

**Notable at app layer**

- [Sablier Flow](https://blog.sablier.com/introducing-sablier-flow/): open-ended streams with top ups for recurring payments

**General**

- [Columbia cryptoeconomics workshop](https://www.youtube.com/playlist?list=PLpktWkixc1gXuGS_C31RlPQMiHFgFBrcA) videos

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-december-14-2024](https://weekinethereumnews.com/week-in-ethereum-news-december-14-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Dec 20 – [ETH Rangers](https://blog.ethereum.org/2024/12/02/ethrangers-public-goods) application deadline

- Jan 20 – [Ethereum protocol attackathon](https://blog.ethereum.org/2024/11/25/ethereum-protocol-attackathon) ends

- Jan 30-31 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Feb 23 - Mar 2 – [ETHDenver](https://www.ethdenver.com/)

- Apr 4-6 – [ETHGlobal Taipei](https://ethglobal.com/events/taipei) hackathon

- May 9-11 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 27-29 – [ETHPrague](https://ethprague.com/) conference

- May 30 - Jun 1 – [ETHGlobal Prague](https://ethglobal.com/events/prague) hackathon

- Jun 3-8 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 12-13 – [Protocol Berg](https://protocol.berlin/) (Berlin) conference

- Jun 16-18 – [DappCon](https://dappcon.io/) (Berlin)

- Jun 26-28 – [ETHCluj](https://www.ethcluj.org/) (Romania) conference

- Jun 30 - Jul 3 – [EthCC](https://ethcc.io/) (Cannes) conference

- Jul 4-6 – [ETHGlobal Cannes](https://ethglobal.com/events/cannes) hackathon

- Aug 15-17 – [ETHGlobal New York](https://ethglobal.com/events/newyork2025) hackathon

- Sep 26-28 – [ETHGlobal New Delhi](https://ethglobal.com/events/newdelhi) hackathon

- Nov – [ETHGlobal Devconnect](https://ethglobal.com/events/ethglobal-devconnect) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

---
title: "Week in Ethereum News <br> March 2, 2024"
date: "2024-03-02"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- Mainnet upgrades to Dencun March 13, epoch 269568, update your nodes
    - MEV-Boost [v1.7](https://github.com/flashbots/mev-boost/releases/tag/v1.7): Dencun support
    
    - EF [mainnet Dencun upgrade announcement](https://blog.ethereum.org/2024/02/27/dencun-mainnet-announcement)
    
    - Devnet 12 will be deprecated after mainnet upgrades
    
    - Reminder: [Goerli testnet deprecated](https://blog.ethereum.org/2023/11/30/goerli-lts-update), client & EF testing teams will start exiting validators April 17 (3 months after Goerli was upgraded)

- Blobs:
    - [EF EIP4844 data challenge](https://esp.ethereum.foundation/data-challenge-4844): write a blob data analysis/viz post by June 14, up to $30k in prizes
    
    - [Blob usage estimates](https://twitter.com/MSilb7/status/1762841908341080079): 4x growth before blob gas price is greater than 1 gwei

**Pectra (Prague + Electra) upgrade (meta** [**EIP7600**](https://eips.ethereum.org/EIPS/eip-7600)**)**

- Future EOA &Account Abstraction breakout [call video](https://www.youtube.com/watch?v=FfEZdTFAz4E&t=46s).  Recap by [Tim Beiko](https://twitter.com/abcoathup/status/1763024493738704975) and notes by [Dom](https://notes.ethereum.org/QT9e9r6NRdSOjWRBzA3JLA):
    - Align short term EOA improvements with an agreed account abstraction end game 

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=4ioJwNPe6RU&t=333s). [Recap](https://twitter.com/christine_dkim/status/1763294754014388614) & [notes](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-182/) from Christine Kim:
    - **Retroactive EIP proposals**: EIP7610 (revert contract creation for non-empty storage) no expected issues with Verkle
    
    - **Pectra upgrade** (small fork targeting late 2024)
        - Continued discussion from future EOA breakout on possible improvements in Pectra
        
        - Potential EIP discussions (but no decisions on what to include):
            - EIP7623 (increase calldata cost)
            
            - EIP5920 (PAY opcode)
            
            - EIP7609 (transient storage pricing)
            
            - EIP7639 (stop serving pre-merge history)
            
            - EIP7642 (drop pre-merge fields)
        
        - Block confirmation rule engine API & JSON RPC changes

**Osaka upgrade (meta** [**EIP7607**](https://eips.ethereum.org/EIPS/eip-7607)**)**

- Verkle implementers [call video](https://www.youtube.com/watch?v=ekxELDRsv4Y&t=3s) & [notes](https://twitter.com/rudolf6_/status/1763469139778167244)

**Client Releases**

- Consensus layer:
    - Nimbus [v24.2.2](https://github.com/status-im/nimbus-eth2/releases/tag/v24.2.2): hotfix for consensus violation issue on Deneb upgraded networks

- Execution layer:
    - Geth [v1.13.14](https://github.com/ethereum/go-ethereum/releases/tag/v1.13.14): blob pool improvements & blob pool capacity reduced from 10GB to 2.5GB
    
    - Reth [v0.1.0-alpha.21](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.21): fixes live sync critical bug

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.26%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: **Geth 72%** supermajority, could cause a chain split
        - [**Updated assumptions**](https://old.reddit.com/r/ethfinance/comments/1b14ls9/daily_general_discussion_february_27_2024/ksekapv/)**: unknown validators 100% Geth & unaccounted validators 80% Geth**
        
        - [**Kiln**](https://twitter.com/kiln_finance/status/1762841341254373598) **migrated to 50.1% Nethermind**
        
        - [**Coinbase**](https://www.coinbase.com/cloud/discover/insights-analysis/execution-client-diversity) **migrating to 50% Nethermind & plans Erigon support**
    
    - Consensus layer: **Prysm 37%**, any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Marius Van Der Wijden: [optional inclusion lists](https://mariusvanderwijden.github.io/blog/2024/01/11/InclusionLists/)

**ePBS (enshrined Proposer-Builder Separation)**

- [Side benefits of ePBS](https://hackmd.io/@potuz/ry9NirU2p): improved pipelining, enhanced incentives for blob inclusion, market & mechanism flexibility and inclusion list flexibility

- Barnabe: [allocate proposing rights](https://mirror.xyz/barnabe.eth/LJUb_TpANS0VWi3TOwGx_fgomBvqPaQ39anVj3mnCOg) rather than building rights

**MEV**

- [MEV research chatbot](https://www.mev.fyi/), requires GitHub or Google login

**Research**

- [Committee-enforced inclusion sets](https://ethresear.ch/t/the-more-the-less-censored-introducing-committee-enforced-inclusion-sets-comis-on-ethereum/18835) (COMIS) for censorship resistance

**Layer 2**

- [Blast](https://twitter.com/blast_l2/status/1763316176263008551) (optimistic rollup) live

- Based sequencing:
    - Sequencing & pre confirmations [call video](https://www.youtube.com/watch?v=mAGGdPRmhsc&t=3s) and [notes](https://docs.google.com/document/d/1hWJU20EwQT3K3uB3GiwDsFlsK3uKuJX20noAN7ZqreA/edit#heading=h.c8nbkk9qxkx6): presentations on risks & concerns
    
    - RollCall (L2 standards) based sequencing breakout [call video](https://www.youtube.com/watch?v=eycLQCaqDsk)
    
    - Specification for a [minimal key store rollup](https://hackmd.io/@mdehoog/mksr)

**EIPs/Standards**

- EIPs:
    - [EIP7636](https://github.com/ethereum/EIPs/pull/8260/files): Extension of EIP778 for "client" ENR entry
    
    - [EIP7637](https://github.com/ethereum/EIPs/pull/8261/files): EXTCODEHASH optimize
    
    - [EIP7639](https://github.com/ethereum/EIPs/pull/8266/files): Cease serving history before PoS
    
    - [EIP7640](https://github.com/ethereum/EIPs/pull/8267/files): Transaction revert protection
    
    - [EIP7642](https://github.com/ethereum/EIPs/pull/8271/files): eth/69 - Drop pre-merge fields
    
    - [EIP7643](https://github.com/ethereum/EIPs/pull/8277/files): History accumulator for pre-PoS data

- ERCs (application layer):
    - [ERC7638](https://github.com/ethereum/ERCs/pull/282/files): Optimized calls encoding (for contract wallets)
    
    - [ERC7641](https://github.com/ethereum/ERCs/pull/284/files): Intrinsic rev share token (ERC20 extension)
    
    - [ERC7644](https://github.com/ethereum/ERCs/pull/292/files): ERC721 name registry extension

**Stuff for developers**

- Remix [v0.44](https://medium.com/remix-ide/remix-release-v0-44-0-eede8a3b1402): save deployed contracts and adds Sindri integration (compute zk proofs remotely)

- Foundry:
    - [Isolated mode](https://twitter.com/gakonst/status/1762624475676454957) for gas measurement

- Base64 library (Solidity):
    - OpenZeppelin Contracts [v5.0.2](https://twitter.com/OpenZeppelin/status/1763272841145794677): fixes Base64 encoding potentially dirty bytes since v4.50
    
    - Solady [Base64](https://twitter.com/optimizoor/status/1763278265479774605): updated to be agnostic to dirty trailing memory bits

- Vyper:
    - Vyper [v0.4.0b1](https://github.com/vyperlang/vyper/releases/tag/0.4.0b1): import system overhauled, reusable Vyper modules and experimental venom IR
    
    - Guide to [get started with Vyper modules](https://gist.github.com/pcaversaccio/cebfca2e26646bb619a52b1ff9ab2c07)

- [BALLS](https://twitter.com/real_philogy/status/1763701628048179476): DSL/Huff-preprocessor in Rust to generate optimized assembly

- [EVM from scratch](https://evm-from-scratch.xyz/): guide to create a mini EVM, work in progress

- Slither [v0.10.1](https://github.com/crytic/slither/releases/tag/0.10.1): Solidity v0.8.24 & top level event support, new detector: [Arbitrum out of order retryable tickets](https://blog.trailofbits.com/2024/03/01/when-try-try-try-again-leads-to-out-of-order-execution-bugs/) and limit results with include-paths option

- Guide to [using Napalm to manage custom detection modules](https://github.com/ConsenSysDiligence/napalm/blob/main/docs/module-hacker.md)

- OpenZeppelin [Defender v2](https://blog.openzeppelin.com/announcing-the-general-availability-of-openzeppelin-defender) general availability

- [EIP4844 blob dev usage](https://github.com/colinlyguo/EIP-4844-dev-usage#readme) guide, how to send blob transactions and query blobs

- [Mopro-cli](https://github.com/oskarth/mopro/tree/main/mopro-cli): build & test Circom circuits from Rust, MVP

- MACI [v1.2](https://maci.pse.dev/blog/maci-v1-2-0-release/): supports non-quadratic voting polls and adds EAS gatekeeper
    - Contribute to MACI v1.2 [trusted setup ceremony](https://ceremony.pse.dev/projects/MACI%20V1.2.0%20Trusted%20Setup%20Ceremony) by March 5

**Security**

- [Tornado Cash deposits using IPFS gateways](https://twitter.com/ameensol/status/1761536032057495633) likely have notes exposed & deposit is at risk, warning blog post may also be a trap

- Seneca [$6.4M exploit](https://rekt.news/seneca-protocol-rekt/) on mainnet & Arbitrum via arbitrary call, revoke any approvals, 80% of funds returned

- SoK: [security vulnerabilities in SNARKs](https://arxiv.org/abs/2402.15293), analysis of 141 implementation vulnerabilities

**Ecosystem**

- Blocknative [Ethernow](https://www.ethernow.xyz/): adds live dashboard of transactions & base fee

**Enterprise**

- [HackMD](https://twitter.com/hackmdio/status/1762132448454885667) adds Sign-in with Ethereum

* * *

### Job Listings

- [TechOps](https://techops.services) are looking for [DevOps](https://apply.workable.com/techops-services/j/5AD8CF90E0/). Work on projects such as MakerDAO.

- ChainSafe seek a [Head of Protocol Engineering](https://grnh.se/c6e27e794us)

- Nethermind: [Distributed Systems Dev Lead](https://grnh.se/c3fd6842teu) & [Cryptography Researcher](https://grnh.se/51fa8652teu)

- [Sr. Developer Relations Manager](https://wellfound.com/jobs/2933743-sr-developer-relations-manager-at-powerloom-protocol) & [Technical Writer](https://wellfound.com/jobs/2931135-technical-writer-at-powerloom-protocol) at [Powerloom](https://powerloom.io/)

- Solidity: [C++ Software Engineer](https://jobs.lever.co/ethereumfoundation/a6e4598e-6c12-493e-8426-438cb0a5eeca) and [Programming Language Researcher](https://jobs.lever.co/ethereumfoundation/d510dfd7-d5dd-435c-9111-1c50112715c1)

- Devcon: [Community Supporter](https://jobs.lever.co/ethereumfoundation/6ad3d8e7-17cb-4d5c-820d-c279e8002551), [Production Assistant](https://jobs.lever.co/ethereumfoundation/aa4c69f8-f564-4036-9c5e-3e09f0eb27df) & [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/e93dae67-65a6-495c-8638-46e3db28cb64)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 16.5 to 305.8 gwei, with 46.2 gwei average
    - Zero net issuance currently at 22.8 gwei 
    
    - 17.8k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,908 - $3,512, currently $3,453

- [ETHBTC](https://ratiogang.com/): currently 0.055 (Flippening at ~0.16)

**Notable at app layer**

- Ondo [global markets](https://blog.ondo.finance/introducing-ondo-global-markets/): tokens represent rights to securities held by broker-dealers

- [Astaria Intents](https://twitter.com/astariaxyz/status/1762612905390834173) (intent-based lending) live on Base

- [Arbitrum Arcade](https://arbitrumfoundation.medium.com/introducing-arbitrum-arcade-8681ce85f20d): 8 week promotion to try games on Arbitrum, starts March 11

**Regulation/business/tokens**

- Gemini plan to [return Earn users assets](https://twitter.com/geminitrustco/status/1762954631150207226) subject to bankruptcy approval & [$37M fine](https://www.dfs.ny.gov/reports_and_publications/press_releases/pr202402282) to NY DFS

- [Fidelity All-in-One ETFs](https://www.fidelity.ca/en/investments/solutions-portfolios/all-in-one/) include 1-3% crypto allocation

- [Optimism RetroPGF3](https://optimism.mirror.xyz/Bbu5M1mTNV2Z637QxOiF7Qt7R9hy6nxghbZiFbtZOBA) learnings & reflections

**General**

- US Whitehouse: [use memory safe programming languages](https://www.whitehouse.gov/wp-content/uploads/2024/02/Final-ONCD-Technical-Report.pdf)

* * *

**End of service:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-march-2-2024](https://weekinethereumnews.com/week-in-ethereum-news-march-2-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Mar 4 – [EF academic grants round](https://esp.ethereum.foundation/academic-grants) application deadline

- Mar 9 – [ETH Salvador](https://ethsalvador.org/)

- Mar 13 – [mainnet Dencun upgrade](https://eips.ethereum.org/EIPS/eip-7569#activation) epoch [269568](https://beaconcha.in/epoch/269568)**, (**[**watch party**](https://www.youtube.com/watch?v=iL0cZRkyrV0)**)**

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024) hackathon

- Mar 18 – [ZK grants round](https://esp.ethereum.foundation/zk-grants) application deadline

- Mar 19-21 – [ETH Canal](http://ethcanal.xyz) (Panama City, Panamá) conference & hackathon

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- Mar 22-24 – [ETHSamba](https://ethsamba.org/) (Rio)

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) conference & hackathon

- Mar 29-31 – [ETH Seoul](https://www.ethseoul.org/) hackathon

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) virtual hackathon

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Apr 12-14 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- Apr 16-18 – [EY Global blockchain summit](https://web.cvent.com/event/e0ad2c12-3e65-41a9-bafb-a436754cf4ae/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7) (London)

- Apr 26-28 – [ETHBoston](https://ethboston.xyz/) conference & hackathon

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/) hackathon

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- Jun 3-5 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- **Jun 14 –** [**EF EIP4844 data challenge**](https://esp.ethereum.foundation/data-challenge-4844) **deadline**

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 26-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Oct 6-8 – [ETHRome](https://ethrome.org/)

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

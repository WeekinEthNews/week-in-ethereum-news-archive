---
title: "Week in Ethereum News <br> February 24, 2024"
date: "2024-02-24"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- [Mainnet shadow fork](https://twitter.com/ethpandaops/status/1761053965834162314) successfully upgraded to Dencun, tested blobs with each EL/CL pair and MEV relayers

- **Client releases for mainnet Dencun upgrade**, update your nodes
    - Consensus layer:
        - Lighthouse [v5.0.0](https://github.com/sigp/lighthouse/releases/tag/v5.0.0)
        
        - Lodestar [v1.16.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.16.0)
        
        - Nimbus [v24.2.1](https://github.com/status-im/nimbus-eth2/releases/tag/v24.2.1)
        
        - Prysm [v5.0.0](https://github.com/prysmaticlabs/prysm/releases/tag/v5.0.0)
        
        - Teku [v24.2.0](https://github.com/Consensys/teku/releases/tag/24.2.0)
    
    - Execution layer:
        - Besu [v24.1.2](https://github.com/hyperledger/besu/releases/tag/24.1.2)
        
        - Erigon [v2.58.1](https://github.com/ledgerwatch/erigon/releases/tag/v2.58.1)
            - Otterscan [v2.4.0 alpha](https://github.com/otterscan/otterscan/releases/tag/v2.4.0): adds blob info
        
        - Geth [v1.13.13](https://github.com/ethereum/go-ethereum/releases/tag/v1.13.13)
        
        - Nethermind [v1.25.4](https://github.com/NethermindEth/nethermind/releases/tag/1.25.4)
        
        - Reth [v0.1.0-alpha.19](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.19)

- Dencun interop testing [call video](https://www.youtube.com/watch?v=SRW-NdnzcSc)

**Pectra (Prague + Electra) upgrade (meta** [**EIP7600**](https://eips.ethereum.org/EIPS/eip-7600)**)**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=FgOuUEgguN0&t=249s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-128/):
    - Electra upgrade scope (small cross layer fork targeting late 2024):
        - **peerDAS (EIP7594)**: develop in parallel to Electra
        
        - **Inclusion lists (EIP7547)**: speed run proof of concept to check complexity for Electra
        
        - **ePBS and increase max EB (EIP7251)**: unlikely for Electra
        
        - **Proposed** [**issuance curve adjustment**](https://ethereum-magicians.org/t/electra-issuance-curve-adjustment-proposal/18825) (30% reduction) and [case for targeting](https://ethresear.ch/t/endgame-staking-economics-a-case-for-targeting/18751) staking ratio of 1/4
        
        - [**Light client roadmap**](https://hackmd.io/@etan-status/electra-lc): proposes backfill protocol & SSZification for Electra

**Osaka upgrade (meta** [**EIP7607**](https://eips.ethereum.org/EIPS/eip-7607)**)**

- Shadow fork [converted Holešky testnet state to Verkle](https://twitter.com/gballet/status/1760657579766669346)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.54%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: **Geth 68%** supermajority, could cause a chain split
    
    - Consensus layer: Prysm 38%, any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Péter Szilágyi: [transaction propagation](https://twitter.com/peter_szilagyi/status/1759957808328392965) proposal to produce less nonce gaps

- Erigon: [Caplin Archival format](https://erigon.tech/releasing-caplins-archival-format/) for storing Beacon Chain history

- [Missed slot penalties](https://ethresear.ch/t/missed-slot-penalties-temperature-check/18713) discussion

**ePBS (enshrined Proposer-Builder Separation)**

- Terence: [why you should care about ePBS](https://terencechain.substack.com/p/why-you-should-care-about-epbs?r=2t6yfg)

- Potuz: [ePBS design constraints](https://ethresear.ch/t/epbs-design-constraints/18728)

**MEV**

- MEV-Boost community [call video](https://www.youtube.com/watch?v=WZ-ON7yAm1Q&t=4s) and [notes](https://twitter.com/terencechain/status/1760344174598266904)

- [Flashbots Protect & MEV-Share](https://collective.flashbots.net/t/publishing-flashbots-protect-and-mev-share-data/3087) data published

- Data Always: [Latency is money](https://hackmd.io/@dataalways/latency-is-money)

**Research**

- Analysis of [increasing the number of proposers in a single slot](https://ethresear.ch/t/concurrent-block-proposers-in-ethereum/18777)

**Layer 2**

- OP chains [Delta upgrade](https://twitter.com/Optimism/status/1760711365168353442) live, adds span batches which reduces fixed costs by over 90%

- [ZK grants round](https://esp.ethereum.foundation/zk-grants) to improve ZK Layer 2 ecosystem, $900k in funds from EF, Aztec, Polygon, Scroll, Taiko & zkSync, applications close March 18

**EIPs/Standards**

- ERCs (application layer):
    - [ERC7625](https://github.com/ethereum/ERCs/pull/265/files): Contract IDs and metadata extension
    
    - [ERC7627](https://eips.ethereum.org/EIPS/eip-7627): Secure messaging protocol
    
    - [ERC7628](https://github.com/ethereum/ERCs/pull/266/files): ERC721 balance extension
    
    - [ERC7629](https://github.com/ethereum/ERCs/pull/269/files): Unified token
    
    - [ERC7631](https://github.com/ethereum/ERCs/pull/271/files): Dual nature token pair (DN404 hybrid ERC721 & ERC20)
    
    - [ERC7632](https://github.com/ethereum/ERCs/pull/275/files): Interfaces for named token
    
    - [ERC7634](https://github.com/ethereum/ERCs/pull/274/files): Limited Transferrable NFT (ERC721 extension)
    
    - [ERC7635](https://github.com/ethereum/ERCs/pull/277/files): Multi-Fungible Token

**Stuff for developers**

- [Fuzz-utils](https://github.com/crytic/fuzz-utils#readme): generate Foundry unit tests from Echidna & Medusa failed properties

- Hardhat-viem [v2](https://github.com/NomicFoundation/hardhat/releases/tag/%40nomicfoundation/hardhat-viem%402.0.0): adds Viem v2

- [Ether Deck Mk2](https://github.com/jtriley-eth/ether-deck-mk2/#readme) (Solidity): optimized contract account

- [createXcrunch](https://github.com/HrikB/createXcrunch#readme): find zero-leading/containing/pattern-matching addresses for CreateX factory

- Protolambda: [Ethereum libs/tools in Go](https://twitter.com/protolambda/status/1759818412048388363) updated for Dencun & Go v1.21

- [King of the Frame strategy](https://twitter.com/0xjustadev/status/1758973668011434062), gas optimizations to lower cost of stealing

- [Circom-plus](https://marketplace.visualstudio.com/items?itemName=vuvoth.circom-plus) (language server): supports go to definition & Circom 2

- [Cyfrin Updraft courses](https://twitter.com/CyfrinUpdraft/status/1760671527996199023) now public: development, testing, contract security & auditing

**Security**

- Blueberry (lending) [exploit](https://twitter.com/blueberryFDN/status/1760872935982879030) front run by c0ffeebabe, 367 ETH returned

**Ecosystem**

- Ethereum Protocol Fellowship [study group](https://epf.wiki/#/eps/week1) started, open to everyone

- [EF Q4 grantees](https://blog.ethereum.org/2024/02/20/esp-allocation-q423) share $30M in funding

**Enterprise**

- [Reddit](https://www.sec.gov/Archives/edgar/data/1713445/000162828024006294/reddits-1q423.htm) holds ETH in treasury

- City of Buenos Aires releases [code for self-sovereign digital identity](https://twitter.com/fernandezdiego/status/1760776277068337619) \[Spanish\]

* * *

### Job Listings

- [Sr. Developer Relations Manager](https://wellfound.com/jobs/2933743-sr-developer-relations-manager-at-powerloom-protocol) & [Technical Writer](https://wellfound.com/jobs/2931135-technical-writer-at-powerloom-protocol) at [Powerloom](https://powerloom.io/)

- Nethermind: [Distributed Systems Dev Lead](https://grnh.se/c3fd6842teu) & [Cryptography Researcher](https://grnh.se/51fa8652teu)

- Sourcify seek a [TypeScript Developer](https://jobs.lever.co/ethereumfoundation/fbcb2cf8-cd58-4140-ab3a-47a402616d50)

- [Executive Assistant](https://jobs.lever.co/ethereumfoundation/444bc50a-236e-4a4e-8385-c0454b0044e9) wanted by EF to support senior decision makers

- Solidity: [C++ Software Engineer](https://jobs.lever.co/ethereumfoundation/a6e4598e-6c12-493e-8426-438cb0a5eeca) and [Programming Language Researcher](https://jobs.lever.co/ethereumfoundation/d510dfd7-d5dd-435c-9111-1c50112715c1)

- MetaMask Staking: [Staff Software Engineer](https://grnh.se/533bf5521us) and [Software Engineer](https://grnh.se/7efeff9b1us)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 11.8 to 198.7 gwei, with 34 gwei average
    - Zero net issuance currently at 22.5 gwei 
    
    - 8.6k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,739 - $3,025, currently $2,921

- [ETHBTC](https://ratiogang.com/): currently 0.058 (Flippening at ~0.16)

**Notable at app layer**

- Uniswap:
    - Proposal for [fees to reward UNI holders that delegate & stake](https://gov.uniswap.org/t/rfc-activate-uniswap-protocol-governance/22936)
    
    - [Uniswap v2](https://blog.uniswap.org/uniswap-v2-now-live-across-more-major-chains) live on Arbitrum, OP mainnet & Base

- [Yuga Labs acquired PROOF](https://news.yuga.com/yuga-labs-acquires-proof), including Moonbirds

- Optimism [airdrop 4](https://community.optimism.io/docs/governance/airdrop-4): NFT deployers on mainnet & OP chains can claim share of 10M OP

**Regulation/business/tokens**

- [Kraken](https://blog.kraken.com/news/sec-kraken-dismiss) filed to dismiss SEC lawsuit 

- [Roman Storm & Alex Pertsev legal defense fundraiser](https://twitter.com/freealexeyroman/status/1760393791620428010) extended until Mar 15 with new NFTs

**General**

- [Extractable witness encryption scheme for KZG commitments](https://eprint.iacr.org/2024/264) and efficient Laconic OT

- [Circle STARKs](https://eprint.iacr.org/2024/278): use efficient M31 field for STARKs, StarkWare & Polygon collaboration

- [LatticeFold](https://eprint.iacr.org/2024/257): leads to post-quantum secure IVC/PCD/SNARKs, performance competitive with pre-quantum folding schemes

- [Minimize foreign arithmetic](https://eprint.iacr.org/2024/265) in ZKP Circuits

- [DoS vulnerability in Pedersen DKG implementations](https://blog.trailofbits.com/2024/02/20/breaking-the-shared-key-in-threshold-signature-schemes/) used in threshold signature schemes

- Apple [iMessage end-to-end encryption upgrading to PQ3](https://security.apple.com/blog/imessage-pq3/) (post-quantum cryptography)

* * *

**End of service:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-february-24-2024](https://weekinethereumnews.com/week-in-ethereum-news-february-24-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Mar 4 – [EF academic grants round](https://esp.ethereum.foundation/academic-grants) application deadline

- **Mar 9 –** [**ETH Salvador**](https://ethsalvador.org/)

- Mar 13 – [mainnet Dencun upgrade](https://eips.ethereum.org/EIPS/eip-7569#activation) epoch [269568](https://beaconcha.in/epoch/269568)

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024) hackathon

- **Mar 18 –** [**ZK grants round**](https://esp.ethereum.foundation/zk-grants) **application deadline**

- Mar 19-21 – [ETH Canal](http://ethcanal.xyz) (Panama City, Panamá) conference & hackathon

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- Mar 22-24 – [ETHSamba](https://ethsamba.org/) (Rio)

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) conference & hackathon

- Mar 29-31 – [ETH Seoul](https://www.ethseoul.org/) hackathon

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) virtual hackathon

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Apr 12-14 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- Apr 16-18 – [EY Global blockchain summit](https://web.cvent.com/event/e0ad2c12-3e65-41a9-bafb-a436754cf4ae/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7) (London)

- **Apr 26-28 –** [**ETHBoston**](https://ethboston.xyz/) **conference & hackathon**

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/) hackathon

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- Jun 3-5 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 26-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- **Sep 12-14 –** [**NapulETH**](https://napul.eth.limo/) **(Napoli)**

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- **Oct 6-8 –** [**ETHRome**](https://ethrome.org/)

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

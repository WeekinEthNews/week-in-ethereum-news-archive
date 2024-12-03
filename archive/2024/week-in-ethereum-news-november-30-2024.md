---
title: "Week in Ethereum News <br> November 30, 2024"
date: "2024-11-29"
---

## Eth News and Links

Tornado Cash contracts can’t be sanctioned under current law, blob increase included in Pectra upgrade and Ethereum protocol attackathon

**Eth R&D protocol call (All Core Devs)**

- [Consensus layer focused protocol call](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-146-november-28-2024/21793) (ACDC #146):
    - **Pectra upgrade:**
        - [**Mekong testnet**](https://mekong.ethpandaops.io/): consensus layer client teams fixing deposit processing bug
        
        - **Blobs:**
            - Agreed to increase blobs per block target to 6 & max of 9 and change update fraction via EIP7691
                - [Long range syncing](https://ethpandaops.io/posts/network-limit-devnets/), clients not purely bottlenecked by bandwidth
                
                - [Block arrival & home staker analysis](https://ethresear.ch/t/block-arrivals-home-stakers-bumping-the-blob-count/21096) supports increase to 4/8 or 6/9 (target/max)
            
            - Blob fee market discussion
            
            - EIP7623 (increase calldata cost): inclusion in Pectra to be decided at execution layer call (ACDE) next week
        
        - [**Pectra-devnet-5 spec**](https://notes.ethereum.org/@ethpandaops/pectra-devnet-5): agreed to exclude empty requests in Engine API to mirror EIP7685 & consolidation processing fix in EIP7251
    
    - [EIP7805 Fork-choice enforced Inclusion Lists](https://docs.google.com/presentation/d/1BYZQOmNkv-nLe25NmPOowhBLPVa76kDDibR_nR0-RGU/edit) (FOCIL) presentation
    
    - [All Core Devs process improvements](https://ethereum-magicians.org/t/allcoredevs-network-upgrade-ethmagicians-process-improvements/20157/51)

[**Fusaka**](https://eips.ethereum.org/EIPS/eip-7607) **(Osaka + Fulu) upgrade**

- [PeerDAS breakout #12](https://ethereum-magicians.org/t/peerdas-breakout-12-november-26-2024/21542): spec discussions on decoupling subnets and validator custody

- [EOF implementers call #62](https://ethereum-magicians.org/t/eof-implementers-call-62-november-27-2024/21543): discussions on compiler metadata and EOFCREATE hash

**Layer 1**

- [QUIC support](https://ethresear.ch/t/quic-support-among-ethereum-consensus-layer-clients/21102): ~42% of nodes, majority running Lighthouse & mostly over IPv4

- [BuilderNet](https://x.com/SheaKetsdever/status/1861480598000304148): block building network running on TEEs, shares MEV with users, early version live operated by Flashbots, Beaverbuild & Nethermind

- Terence: [same slot vs next slot](https://hackmd.io/@ttsao/same-vs-next-slot-il) for inclusion list design, spec & prototype will use same slot

**For stakers**

- [Deposit tools vulnerability](https://www.reddit.com/r/ethstaker/comments/1h0hn4j/insecure_keystore_files_generated_from_the/): multiple keystore files generated in a single run should be considered as unencrypted

**Research**

- [In-protocol transaction ordering](https://ethresear.ch/t/in-protocol-transaction-ordering/21084), extension to Fork-Choice enforced Inclusion Lists (FOCIL)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.1%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~43% & Nethermind ~36% (estimate based on 74% self reported data)
    
    - Consensus layer: Prysm 35%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Client Releases**

- Consensus layer:
    - Lodestar [v1.23.1](https://github.com/ChainSafe/lodestar/releases/tag/v1.23.1): fixes for issues in recent devnets

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7825](https://github.com/ethereum/EIPs/pull/9049/files): Transaction gas limit cap

- ERCs (application layer):
    - [ERC7826](https://github.com/ethereum/ERCs/pull/731/files): Quantum supremacy bounty
    
    - [ERC7827](https://github.com/ethereum/ERCs/pull/734/files): JSON contract with value version control
    
    - [ERC7828](https://github.com/ethereum/ERCs/pull/735/files): Chain-specific addresses using ENS
    
    - [ERC7829](https://github.com/ethereum/ERCs/pull/744/files): Data asset NFT

**Stuff for developers**

- [Foundry compiler profiles](https://x.com/gretzke/status/1861175176005570977): compile contracts needing optimization with IR & tests without IR; 10x compile time reduction for Uniswap v4 contracts

- [Echidna trace parser](https://github.com/Enigma-Dark/echidna-trace-parser#readme): convert Echidna call traces into Foundry tests

- Uniswap [Compact](https://github.com/Uniswap/the-compact#readme) (Solidity): ownerless ERC6909 contract, facilitates formation/dissolution of reusable resource locks

- [MicroStable](https://github.com/shafu0x/MicroStable-World#readme): simple stablecoin design in Solidity & Vyper

- Cyfrin Upgrade [beginner](https://updraft.cyfrin.io/courses/intro-python-vyper-smart-contract-development) & [intermediate](https://updraft.cyfrin.io/courses/intermediate-python-vyper-smart-contract-development) Python & Vyper courses

- CTFs:
    - [OSAKA](https://github.com/minaminao/my-ctf-challenges/tree/main/ctfs/seccon-ctf-13-quals/osaka#readme): EVM Object Format (EOF) challenge

- [Drift](https://github.com/delvtech/drift#readme): write cached contract calls for web3 libraries (viem, web3.js & ethers)

**Security**

- [Ethereum protocol attackathon](https://blog.ethereum.org/2024/11/25/ethereum-protocol-attackathon): $1.5M reward pool, January 20 deadline

* * *

### Job Listings

- Nethermind: [AI Agent](https://job-boards.eu.greenhouse.io/nethermind/jobs/4465865101), [Infra](https://job-boards.eu.greenhouse.io/nethermind/jobs/4467282101), [Blockchain](https://job-boards.eu.greenhouse.io/nethermind/jobs/4467974101), [Full Stack](https://job-boards.eu.greenhouse.io/nethermind/jobs/4467217101), [BizDev](https://job-boards.eu.greenhouse.io/nethermind/jobs/4471319101) & [Researcher](https://job-boards.eu.greenhouse.io/nethermind/jobs/4466531101)

**Job listings: $600 for 4 issues** (75 char limit). [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.** Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 4.0 to 46.4 gwei, 11.2 gwei average; zero net issuance at 24.2 gwei
    
    - 9.5k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,288 - $3,666, currently $3,598, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.037 (Flippening at ~0.164)

**Notable at app layer**

- Dan Finlay: [meme token experiment](https://blog.danfinlay.com/meme-tokens-and-consent), tools & incentives not currently sufficient for fundraising or having fun

- [Kraken NFT marketplace closing](https://support.kraken.com/hc/en-us/articles/nft-marketplace-closure-faq), users have 3 months to withdraw NFTs

- [Freysa](https://x.com/jarrodwattsdev/status/1862299845710757980): player successfully convinced AI agent to transfer prize pool

**Regulation/business/tokens**

- US Fifth Circuit rules [Tornado Cash immutable contracts can’t be sanctioned](https://assets.ctfassets.net/c5bd0wqjc7v0/70EasapqSxH1kLInf3IQrd/1a1ce21cdc6bc903921f45018cce3821/Tornado_Cash.pdf) under current law, OFAC overstepped

- [Coinbase USDC Rewards](https://www.reddit.com/r/CoinBase/comments/1h1zf4u/no_more_interest_on_usdc_to_europeans/) sunset in Europe due to MiCA regulation

**General**

- EF [Poseidon cryptanalysis initiative](https://www.poseidon-initiative.info/): attack bounties & research grants

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-november-30-2024](https://weekinethereumnews.com/week-in-ethereum-news-november-30-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Dec 4-5 – [Columbia CryptoEconomics workshop](http://columbiacryptoeconomics.org/) (New York)

- Dec 6-8 – [ETHIndia](https://ethindia.co/) hackathon

- Dec 9 – [EF internships 2025](https://blog.ethereum.org/2024/11/16/announcing-ef-internship-program) application deadline

- **Jan 20 –** [**Ethereum protocol attackathon**](https://blog.ethereum.org/2024/11/25/ethereum-protocol-attackathon) **ends**

- Jan 30-31 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Feb 23 - Mar 2 – [ETHDenver](https://www.ethdenver.com/)

- Apr 4-6 – [ETHGlobal Taipei](https://ethglobal.com/events/taipei) hackathon

- May 9-11 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 27-29 – [ETHPrague](https://ethprague.com/) conference

- May 30 - Jun 1 – [ETHGlobal Prague](https://ethglobal.com/events/prague) hackathon

- **Jun 3-8 –** [**ETH Belgrade**](https://ethbelgrade.rs/) **conference & hackathon**

- Jun 12-13 – [Protocol Berg](https://protocol.berlin/) (Berlin) conference

- Jun 16-18 – [DappCon](https://dappcon.io/) (Berlin)

- Jun 26-28 – [ETHCluj](https://www.ethcluj.org/) (Romania) conference

- Jun 30 - Jul 3 – [EthCC](https://ethcc.io/) (Cannes) conference

- Jul 4-6 – [ETHGlobal Cannes](https://ethglobal.com/events/cannes) hackathon

- Aug 15-17 – [ETHGlobal New York](https://ethglobal.com/events/newyork2025) hackathon

- Sep 26-28 – [ETHGlobal New Delhi](https://ethglobal.com/events/newdelhi) hackathon

- Nov – [ETHGlobal Devconnect](https://ethglobal.com/events/ethglobal-devconnect) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

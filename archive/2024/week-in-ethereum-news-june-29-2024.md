---
title: "Week in Ethereum News <br> June 29, 2024"
date: "2024-06-29"
---

## Eth News and Links

SEC charges Consensys, US Supreme Court overrules Chevron deference and Reth (Paradigm’s Rust execution layer client) is production ready

**All core devs**

- [**All core devs – consensus (ACDC) #136**](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-call-136-june-27-2024/20397):
    - Presentation on [private sharing of client info by validators](https://ethresear.ch/t/research-report-allowing-validators-to-share-client-information-privately-a-project-by-nethermind-research/19506) research
    
    - Péter Szilágyi: proposal to [cross validate](https://gist.github.com/karalabe/47c906f0ab4fdc5b8b791b74f084e5f9) with other execution layer clients statelessly (before Verkle) and change engine API encoding from JSON to SSZ
    
    - **Pectra (Prague + Electra) upgrade**:
        - **pectra-devnet-1**: waiting on execution layer clients
        
        - **EIP6110 validator deposits onchain**: proposal to rate limit deposit processing
        
        - **EIP7594 PeerDAS**: [peerdas-devnet-1](https://peerdas-devnet-1.ethpandaops.io/) launched with 3 consensus layer clients, discussion on decoupling layers for blob count
        
        - **EIP7688 SSZ StableContainer**: devnet running but not all clients have implemented, no decision yet on including in Electra 

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade, likely targeting Q1 2025**

- [Future of EOA/AA breakout #5](https://ethereum-magicians.org/t/future-of-eoa-aa-breakout-5-june-26-2024/20398): EIP7702 delegation designation proposal to be merged next week

- [PeerDAS breakout #2](https://ethereum-magicians.org/t/peerdas-breakout-2-june-25-2024/20399): passing max blobs per block is preferred solution for decoupling layers, value should be configurable and fetching from execution layer pool experiment

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 29.2%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~55% majority 
    
    - [**Lighthouse client info in graffiti**](https://x.com/EthDreamer/status/1806384165413146821) **(7.4% of blocks): Geth 62%**
    
    - Consensus layer: Prysm 38%
    
    - Any client bug over 33.3% could mean loss of finality

- [**Geographic distribution of validators**](https://ethresear.ch/t/estimating-validator-decentralization-using-p2p-data/19920#results-15)**, estimated using p2p data**

**Layer 1**

- [Gossipsub performance](https://ethresear.ch/t/number-duplicate-messages-in-ethereums-gossipsub-network/19921), recommends reducing concurrent IWANT messages sent & lowering heartbeat frequency

- EF [Protocol Security Research](https://github.com/ethereum/protocol-security#readme) team explainer of what they do

**Research**

- [Orbit SSF](https://ethresear.ch/t/orbit-ssf-solo-staking-friendly-validator-set-management-for-ssf/19928): solo-staking-friendly validator set management for single slot finality

- [Execution Auctions superior to Execution Tickets](https://ethresear.ch/t/execution-auctions-as-an-alternative-to-execution-tickets/19894), simpler to implement but have centralization concerns (which may be curbed by Inclusion Lists)

**Client Releases**

- Consensus layer:
    - Lighthouse [v5.2.1](https://github.com/sigp/lighthouse/releases/tag/v5.2.1): small fixes for sync & backfill
    
    - Nimbus [v24.6.0](https://github.com/status-im/nimbus-eth2/releases/tag/v24.6.0): SHA256 hashing 30% faster, avoid slashing when validator key sharing improperly configured, adds block scoring and enables block monitoring by default

- Execution layer:
    - Erigon [v2.60.2](https://github.com/ledgerwatch/erigon/releases/tag/v2.60.2): fixes
    
    - Reth (Paradigm) [v1](https://www.paradigm.xyz/2024/06/reth-prod): **production ready**; sync from genesis in ~50 hours, 2.3TB archive node

**Layer 2**

- Arbitrum [Timeboost](https://forum.arbitrum.foundation/t/constitutional-aip-proposal-to-adopt-timeboost-a-new-transaction-ordering-policy/25167) proposed, auction for express transaction submission (non-express transactions have a short delay), proceeds will either be in ARB (burnt) or ETH (collected)

- Flashbots: [MEV on L2s](https://collective.flashbots.net/t/it-s-time-to-talk-about-l2-mev/3593)

- Offchain Labs [BlobWatcher](https://github.com/OffchainLabs/Blobwatcher#readme): monitor transaction pool for blob transactions

- [Blast](https://x.com/blast_l2/status/1805964805414830506) phase 1 airdrop, goes in at $2B FDV

- L2Beat [ZK Catalog](https://medium.com/l2beat/introducing-the-zk-catalog-7ac6f22889c0): code verification of onchain ZK verifiers

**For Stakers**

- Stakesaurus: [DVT home staking guide](https://dvt-homestaker.stakesaurus.com/) (Diva), aimed at novices

- [Ethereum on ARM](https://x.com/ethereumonarm/status/1805899645899383056): full node (Geth + Nimbus) on Rock 5B 16 GB RAM with 2 physical cores

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7727](https://github.com/ethereum/EIPs/pull/8684/files): EVM transaction bundles

- RIPs (Rollup improvement proposals):
    - [RIP7728](https://github.com/ethereum/RIPs/pull/27/files): Precompile for L1SLOAD

- ERCs (application layer standards):
    - [ERC7729](https://github.com/ethereum/ERCs/pull/506/files): Token with metadata (ERC20 extension)
    
    - [ERC7730](https://github.com/ethereum/ERCs/pull/509/files): Structured data clear signing format

**Stuff for developers**

- Snekmate [v0.1](https://github.com/pcaversaccio/snekmate/releases/tag/v0.1.0) (Vyper contracts): contracts made module friendly, targets Vyper v0.4.0

- Remix [v0.51](https://medium.com/remix-ide/remix-release-v0-51-0-ffe0260a9ad5): adds SolidityScan to analyze code for vulnerabilities and supports EIP712 eth\_signTypedData in Remix VM

- Patrick Collins: [guide to where EVM can read/write data](https://www.cyfrin.io/blog/fixing-data-location-must-be-memory-or-calldata)

- [Gas playground](https://x.com/WilsonCusack/status/1804990999954899017): browser playground for Solidity contracts, uses live state (currently Base only)

- Guide to [mine an efficient address](https://x.com/z0r0zzz/status/1804476268852998221) using create2crunch

- EVMole [v0.3.5](https://x.com/cdump/status/1805590325433409984) (function selector extractor): adds Vyper support

- Viem [experimental](https://viem.sh/experimental) adds Solady ERC1271 Actions

- Paradigm fellowship [technical questions](https://x.com/transmissions11/status/1805630729885565197)

- RareSkills [Uniswap v2 puzzles](https://github.com/RareSkills/uniswap-v2-puzzles/#readme)

- [Cyfrin updraft](https://x.com/cyfrinupdraft/status/1806676546758783470): updated Solidity & Foundry courses

**Ecosystem**

- EF Next Billion [cohort 4 fellows](https://blog.ethereum.org/2024/06/24/next-billion-cohort4)

- ETHKyiv [hackathon projects](https://taikai.network/ethkyiv/hackathons/ethkyiv/projects)

**Enterprise**

- [Stripe adding Base support](https://www.coinbase.com/en-au/blog/coinbase-stripe-team-up-to-increase-global-adoption-of-crypto) to their crypto payouts & onramp

* * *

### Job Listings

- Gnosis is hiring: [Discord Moderator](https://gnosis.jobs.personio.com/job/1166297?_pc=1517287)

- IMC: [Quant Developer](https://imczug.recruitee.com/o/quant-developer-defi) for DeFi and MEV focused team

- Privacy and Scaling Explorations: [ZK Circuits Engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4)

- Nethermind: [Preconfirmations Senior Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4344191101), [Protocol Researcher](https://boards.eu.greenhouse.io/nethermind/jobs/4347537101), [Senior Content Marketing](https://boards.eu.greenhouse.io/nethermind/jobs/4351446101) & [Senior Marketing Manager](https://boards.eu.greenhouse.io/nethermind/jobs/4346942101)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 1.2 to 31.4 gwei, 4.5 gwei average; zero net issuance at 23.5 gwei 
    
    - 13k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,259 - $3,516, currently $3,385, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.056 (Flippening at ~0.16)

**Regulation/business/tokens**

- [SEC charges Consensys](https://storage.courtlistener.com/recap/gov.uscourts.nyed.517222/gov.uscourts.nyed.517222.1.0.pdf) as an unregistered broker for MetaMask Swaps and claims MetaMask Staking sells securities (stETH & rETH)

- US Supreme Court:
    - holds [SEC violated right to trial by jury;](https://x.com/jchervinsky/status/1806335052038488531) no more SEC kangaroo courts 
    
    - [overrules Chevron](https://twitter.com/JBSDC/status/1806799823107997893), courts no longer must defer to federal agency power grabs 

- [Coinbase](https://twitter.com/iampaulgrewal/status/1806299309836746909) filed FOIA lawsuits against SEC & FDIC over Biden’s Operation Chokepoint 2.0 

- [US Treasury finalized broker rule](https://x.com/millercwl/status/1806785545202475511), but punts on DeFi

**General**

- [Iranians vote](https://x.com/ameensol/status/1806643812715897138): scan passport NFC to prove eligibility, generate ZK proof & vote on Gnosis chain

- [Polyfill](https://www.bleepingcomputer.com/news/security/polyfillio-javascript-supply-chain-attack-impacts-over-100k-sites/) (JavaScript) supply chain attack, [Cloudflare](https://blog.cloudflare.com/automatically-replacing-polyfill-io-links-with-cloudflares-mirror-for-a-safer-internet) automatically replacing links

- Wired: [home invader convicted of burglarizing & torture](https://www.wired.com/story/crypto-home-invasion-crime-ring/) to steal crypto 

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-june-29-2024](https://weekinethereumnews.com/week-in-ethereum-news-june-29-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jul 7 – [Devcon scholars program](https://blog.ethereum.org/2024/06/07/devcon7-scholars) deadline

- Jul 9– [Devcon ticket raffle & auction](https://raffle.devcon.org/) deadline

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 29-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 2-4 – [Ethereum Argentina](https://ethereumargentina.org/) conference & hackathon

- Aug 7-9 – [Science of Blockchain Conference](https://www.sbc-conference.com/) (New York)

- Aug 15-17 – [Ethereum Uruguay](https://www.ethereumuruguay.org/) hackathon & conference

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 23-26 – [ETHTokyo](https://www.ethtokyo.com/) hackathon & conference

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- Sep 5-8 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 9-15 – [ETHSafari](https://ethsafari.xyz/) (Kenya)

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 13-14 – [Ethereum México](https://ethmexico.org/)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Sep 26-27 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 4-6 – [Ethereum Kuala Lumpur](https://www.2024.ethkl.org/) conference & hackathon

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

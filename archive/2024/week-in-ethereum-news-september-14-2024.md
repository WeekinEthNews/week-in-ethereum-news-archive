---
title: "Week in Ethereum News <br> September 14, 2024"
date: "2024-09-14"
---

## Eth News and Links

Danny Ryan taking indefinite break, Pectra upgrade split proposed & cbBTC live

**All core devs**

- [All Core Devs - Execution (ACDE) #196](https://ethereum-magicians.org/t/all-core-devs-execution-acde-196-september-12-2024/20922):
    - **Pectra (Prague + Electra) upgrade:**
        - [**Pectra split proposed**](https://hackmd.io/@ralexstokes/rJVuKtlpR): overall scope to remain the same, cap Pectra at devnet-3 spec to target Q1 2025, second upgrade with PeerDAS & EOF to target H2 2025, agree split at ACDC 
        
        - [**Pectra-devnet-3**](https://pectra-devnet-3.ethpandaops.io/): live, validator consolidations & EIP7702 work as expected and wallet devs can use to test EIP7702
        
        - **EIP7685 execution layer requests**: explicit ordering & handling of invalid requests to be specified
        
        - **EIP7702**: minimal validity checks, inline with existing transaction types
        
        - **EIP2537 BLS precompile:** MSM precompiles need benchmarking with concurrency disabled to see if gas cost should be doubled

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- [Pectra testing call #4](https://ethereum-magicians.org/t/pectra-testing-call-4-9-september-2024/21045): PeerDAS local devnet debugging ongoing

[**Fusaka**](https://eips.ethereum.org/EIPS/eip-7607) **(Osaka + Fulu) upgrade**

- [Verkle implementers call #24](https://ethereum-magicians.org/t/verkle-implementers-call-24-september-9-2024/21063): plan to evaluate binary tries & lean into tree-agnostic development (in case ZK solution ready in similar timeframe to Verkle), discussed deletions, EOF/EIP7702 impact and sync

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.2%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~52% majority
    
    - Consensus layer: **Prysm 37%**
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Layer 1**

- [ePBS breakout #9](https://ethereum-magicians.org/t/epbs-breakout-9-september-13-2024/21062): slot auctions give out-of-protocol trusted advantage, new Engine API method to request payloads by range and discussed moving withdrawals processing to execution phase

**Research**

- [AUCIL](https://ethresear.ch/t/aucil-an-auction-based-inclusion-list-design-for-enhanced-censorship-resistance-on-ethereum/20422): auction-based inclusion list, aggregator role auctioned off with winner proposing largest inclusion list

**Client Releases**

- Execution layer:
    - Erigon [v2.60.7](https://github.com/erigontech/erigon/releases/tag/2.60.7): release process changes & Windows users need to build locally

**Layer 2**

- Optimism [Granite upgrade](https://x.com/optimism/status/1833903320945041685) reenabled permissionless fault proofs on OP Mainnet

- [OP Succinct](https://blog.succinct.xyz/op-succinct/): convert OP Stack chain to a zkEVM using SP1, 1 hour finality & ~1 cent per transaction proving costs

- [ZKsync governance](https://blog.zknation.io/zksync-governance-system/) live, consists of token assembly, security council & guardians

- [L2 safety](https://l2safety.info/): simplified view of L2Beat

- [RollCall #7](https://ethereum-magicians.org/t/rollcall-7-september-11-2024/20707) (L2 standards): L2s should shout blobspace needs as PeerDAS may ship after Pectra, Oasis L2 transaction fee API & status specs and EIP7762 blob minimum price

**EIPs/Standards**

- RIPs (rollup improvement proposals):
    - [RIP7767](https://github.com/ethereum/RIPs/pull/37/files): Gas to Ether precompile (GASBACK)

- ERCs (application layer):
    - [ERC7765](https://github.com/ethereum/ERCs/pull/624/files): Privileged NFTs tied to RWA (ERC721 extension)
    
    - [ERC7766](https://github.com/ethereum/ERCs/pull/626/files): Signature aggregation for account abstraction (ERC4337)

**Stuff for developers**

- [EVM Object Format (EOF) explainer](https://x.com/jtriley_eth/status/1833548628314767681): less stack-too-deep errors, lower cost execution, smaller bytecode and can lead to better tooling

- [Allegedly](https://github.com/kyscott18/allegedly#readme): Solidity compiler in TypeScript for EVM simulations

- [Moccasin](https://github.com/Cyfrin/moccasin#readme): Vyper contract development framework, uses Python for scripts & tests, alpha

- CTFs:
    - Secureum RACE #32: [answers to 8 question Solidity quiz](https://ventral.digital/posts/2024/9/8/race-32-of-the-secureum-bootcamp-epoch-infinity/)

- [MEV searcher](https://x.com/bertcmiller/status/1834218771432587623) mines vanity transaction hash prefixes, function selector & call data
    - Unsuccessful [attempt to reverse engineer](https://x.com/jtriley_eth/status/1834692924204105915) the contract

**Security**

- Security notes on [ERC4337 account abstraction](https://blog.yacademy.dev/2024-09-09-security-notes-erc4337/)

**Ecosystem**

- [EF EIP4844 data challenge](https://blog.ethereum.org/2024/09/13/4844-data-challenge) winners

- Hackathon projects: ETHGlobal [ETHOnline](https://x.com/ethglobal/status/1834627552914375038) finalists and [ETHWarsaw](https://ethwarsaw-hackathon-2024.devfolio.co/projects)

**Enterprise**

- Visa: [stablecoin usage in emerging markets](https://castleisland.vc/wp-content/uploads/2024/09/stablecoins_the_emerging_market_story_091224.pdf) & updated [stablecoin dashboard](https://visaonchainanalytics.com/)

- [EVE Frontier](https://x.com/latticexyz/status/1834233880880316654) (space survival game) playtest planned on Redstone testnet

* * *

### Job Listings

- Gnosis seek [CoreDevs](https://gnosis.jobs.personio.com/job/893408?_pc=1517287), [Sr Algorithm Engineer](https://gnosis.jobs.personio.com/job/1698369?_pc=1517287), [Sr Smart Contract Engineer](https://gnosis.jobs.personio.com/job/1698390?_pc=1517287)

- Join [Witnet](https://witnet.io/) as a [Community Builder](https://wellfound.com/l/2Akjg4)! Full-time, remote opportunity.

- [Status](https://status.app/) [free.technology](https://free.technology/) is hiring a [Business Developer](https://grnh.se/63f67b381us). More [jobs](https://free.technology/jobs) at IFT!

- [Nomos](https://free.technology/nomos) is hiring [Ecosystem Developer](https://grnh.se/6a2297081us), [Rust Engineer](https://grnh.se/bd96340e1us) & [Applied Researcher](https://grnh.se/03fe75801us)!

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 0.6 to 28.1 gwei, 3.2 gwei average; zero net issuance at 24.1 gwei 
    
    - 16k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,225 - $2,458, currently $2,437, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.04 (Flippening at ~0.164)

**Notable at app layer**

- Coinbase [cbBTC](https://www.coinbase.com/en-au/blog/coinbase-wrapped-btc-cbbtc-is-now-live) live on mainnet & Base; upgradeable, pausable & blacklistable

- [PayPal & Venmo](https://blog.ens.domains/post/bringing-crypto-transfers-to-millions-with-paypal-and-venmo) add ENS support, use ENS names in search when sending crypto

- ZeroDev [magic account](https://magicaccount.io/): chain abstracted USDC on mainnet, Arbitrum, Optimism & Base

- [Snapshot X](https://snapshot.mirror.xyz/F0wSmh8LROHhLYGQ7VG6VEG1_L8_IQk8eC9U7gFwep0): onchain voting using Starknet and storage proofs of mainnet holdings

- [Friend Tech](https://x.com/friendtech/status/1832581118165709140) sent contract admin/ownership to zero address

- [Fractionalized CryptoPunk](https://x.com/0xQuit/status/1833981559910850603) bought out for 10 ETH on Niftex (decommissioned platform)

**Regulation/business/tokens**

- US Financial Services subcommittee hearing: [decoding DeFi](https://financialservices.house.gov/calendar/eventsingle.aspx?EventID=409331)

- [eToro $1.5M settlement](https://www.sec.gov/newsroom/press-releases/2024-125) with SEC, US users restricted to trading ETH & Bitcoin
    - [SEC used "crypto asset securities" term](https://x.com/jchervinsky/status/1834459757295398993) despite telling a federal court they would stop

- [Robinhood $3.9M settlement](https://oag.ca.gov/news/press-releases/attorney-general-bonta-secures-39-million-settlement-cryptocurrency-company) with California DoJ for failing to allow crypto withdrawal

- Binance employee [Tigran Gambaryan](https://rekt.news/bring-tigran-home/) still held in Nigeria

**General**

- [Danny Ryan](https://github.com/djrtwo/writing/blob/main/docs/2024-09-13_goodbye-for-now.md) taking an indefinite break from Ethereum L1 R&D

- [Indodax](https://rekt.news/indodax-rekt/) (Indonesian centralized exchange) $25M stolen from hot wallets

- [PIXHELL](https://arxiv.org/abs/2409.04930): malicious code can leak info from air gap computers via noise generated by pixels

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-september-14-2024](https://weekinethereumnews.com/week-in-ethereum-news-september-14-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Sep 20-22 – [ETHCapeTown](https://www.ethcapetown.com/) hackathon

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Sep 26-27 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 4-6 – [Ethereum Kuala Lumpur](https://www.2024.ethkl.org/) conference & hackathon

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 17-20 – [ETHLisbon](https://ethlisbon.org/) hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

- Dec 6-8 – [ETHIndia](https://ethindia.co/) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

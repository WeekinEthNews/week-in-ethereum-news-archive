---
title: "Week in Ethereum News <br> November 9, 2024"
date: "2024-11-08"
---

## Eth News and Links

EF 2024 report & conflict of interest policy and Mekong testnet (Pectra public testnet) live

**Eth R&D protocol call (All Core Devs)**

- [Execution layer focused protocol call](https://ethereum-magicians.org/t/all-core-devs-execution-acde-200-november-7-2024/21463) (ACDE #200):
    - **Pectra upgrade:**
        - [**Pectra-devnet-4**](https://pectra-devnet-4.ethpandaops.io/): testing planned during Devcon & will then be deprecated
        
        - **Pectra-devnet-5 spec**:
            - EIP7702: EXTCODE\* delegation behavior removed
            
            - Proposal to return fee from getter for EIP7002 & EIP7251 system contracts, review async, audits started
    
    - **Fusaka upgrade**:
        - **Activate EOF/PeerDAS separately for testing**: agreed to enable as separate consensus layer & execution layer upgrades
    
    - **EIP7801 eth/70 - sharded blocks protocol:** proposal for short term alternative to integrating Portal Network to serve historical data
    
    - **EIP7610 revert creation for non-empty storage**: EIP was previously retroactively included but some client teams have issues implementing, alternative to be proposed

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- [Mekong testnet](https://blog.ethereum.org/2024/11/07/introducing-mekong-testnet): Pectra public testnet with devnet-4 spec

- [Weekly testing call #12](https://ethereum-magicians.org/t/pectra-testing-call-12-november-4-2024/21592): peerdas-devnet-4 & EOF devnet to be based on pectra-devnet-5 spec, ideally by the end of November

[**Fusaka**](https://eips.ethereum.org/EIPS/eip-7607) **(Osaka + Fulu) upgrade**

- [EVM Object Format (EOF) benefits for ZK proofs](https://blog.succinct.xyz/eofbenefits/): benchmarks show 2.9x more efficient for total & interpreter cycles, runs 2.7x faster and proof size 2x smaller

[**Amsterdam**](https://eips.ethereum.org/EIPS/eip-7773) **upgrade**

- [Stateless implementers call #27](https://ethereum-magicians.org/t/stateless-implementers-call-27-november-4-2024/21599)

**Layer 1**

- Flashbots:
    - [rbuilder running in-process](https://collective.flashbots.net/t/announcing-in-process-rbuilder/4036) with Reth
    
    - [Parallel block building](https://writings.flashbots.net/parallel-builder): backtesting shows better blocks 50% of the time in high MEV

**Research**

- [3-slot finality](https://ethresear.ch/t/3-slot-finality-ssf-is-not-about-single-slot/20927) (3SF): finalize blocks within 3 slots using only one voting phase per slot, compared with single slot finality which uses three voting phases per slot

- [Orbit single-slot finality design](https://ethresear.ch/t/orbit-ssf-in-practice/20943): proposal simplifies committee formation

- [Random execution auctions](https://ethresear.ch/t/proposers-do-play-dice-introducing-random-execution-auctions-randeas/20938) (randEAs): mitigate multi-block MEV by auctioning proposing rights for a slot window but exact slot only assigned & revealed one slot in advance

- [Full DAS analysis](https://ethresear.ch/t/full-das-sampling-analysis/20912): fast sampling can be performed at scale, network can absorb large correlated failures but malicious majority attacks remain a challenge

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 27.8%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~52% majority
    
    - Consensus layer: Prysm 37% & Lighthouse 33.3%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Client Releases**

- Execution layer:
    - Erigon [v2.60.10](https://github.com/erigontech/erigon/releases/tag/v2.60.10): bug fixes
    
    - Reth [v1.1.1](https://github.com/paradigmxyz/reth/releases/tag/v1.1.1): performance improvements & bug fixes and Engine 2.0 enabled by default for op-reth

**For stakers**

- Beaconcha.in [v2 beta](https://x.com/beaconcha_in/status/1853453247559680433) (explorer): real-time monitoring, custom validator groups and adds validator efficiency metric

- [BuidlGuidl client](https://client.buidlguidl.com/): one line command to run Reth + Lighthouse

**Layer 2**

- Marius Van Der Wijden: [EVM-semi compatible rollup design](https://mariusvanderwijden.github.io/blog/2024/07/12/L2s/), higher throughput but higher trust assumptions

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7807](https://github.com/ethereum/EIPs/pull/9017/files): SSZ execution blocks
    
    - Meta [EIP7808](https://github.com/ethereum/EIPs/pull/9020/files): Reserve tx-type range for RIPs
    
    - [EIP7809](https://github.com/ethereum/EIPs/pull/9026/files): Native tokens

- RIPs (rollup improvement proposals):
    - Meta [RIP7810](https://github.com/ethereum/RIPs/pull/41/files): RIP Purpose and Guidelines 

- ERCs (application layer):
    - [ERC7806](https://github.com/ethereum/ERCs/pull/696/files): Minimal intent-centric EOA smart account
    
    - [ERC7811](https://github.com/ethereum/ERCs/pull/709/files): Wallet asset discovery
    
    - [ERC7812](https://github.com/ethereum/ERCs/pull/710/files): ZK identity registry
    
    - [ERC7813](https://github.com/ethereum/ERCs/pull/711/files): Store, table-based introspectable storage

**Stuff for developers**

- [Solar](https://www.paradigm.xyz/2024/11/solar): Solidity compiler frontend in Rust; Apache/MIT license

- [Devcon faucet](https://devcon-mekong-faucet.pk910.de/): claim 100 testnet ETH for Mekong, Sepolia & Holešky using ticket on Zupass

- Etherscan [EIP2535 Diamond proxy support](https://x.com/etherscan/status/1853414623581753801), beta

- Wevm [Ox v0.1](https://github.com/wevm/ox#readme) (TypeScript): unopinionated low-level utilities & types

- [Convert Bank challenge CTF](https://x.com/fucory/status/1852804233156084078) from Foundry to Tevm

- Coinbase OnchainKit [NFTMintCard](https://onchainkit.xyz/mint/nft-mint-card) (React component): mint NFTs

- Micro-eth-signer [v0.12.1](https://github.com/paulmillr/micro-eth-signer/releases/tag/0.12.1): adds Verkle JavaScript implementation

**Security**

- [Cross-chain token recovery](https://github.com/codeislight1/Cross-Chain-Token-Recovery-Registry#readme): script to recover funds sent to a contract address on a chain where the contract didn’t exist and a list of projects that may be able to recover funds

**Ecosystem**

- [EF 2024 report](https://ethereum.foundation/report-2024.pdf):
    - **Core values**: long term thinking, subtraction & stewardship of values
    
    - **Spending**:
        - $105.4M in 2022: $38.2M internal & $67.2M external
        
        - $134.9M in 2023: $50.2M internal & $84.7M external
        
        - 22 EF teams
    
    - **Treasury**:
        - $970.2M (at Oct 31), $788.7M crypto (99.45% ETH) & $181.5M non-crypto; includes remaining 26,701 ETH for client incentive program
    
    - **EF conflict of interest policy v1**: internal disclosures; discussion group to review prior to starting outside work above cap, angel investing, investing & co-founding; outside work paid in illiquid assets with unknown market value generally prohibited

- [Justin Drake](https://x.com/drakefjustin/status/1852734263541874824) & [Dankrad Feist](https://x.com/dankrad/status/1852734273461080320) drop EigenLayer advisorships

- Josh Stark: [Ethereum's distinctive property is hardness](https://stark.mirror.xyz/A9csRsDaAJHJCCWa2Vv16bmxl0BgDqiLdupASxBT2r4)

- Evan’s dumbing down of Vitalik’s roadmap explainers: [the Scourge](https://x.com/evan_van_ness/status/1853558885417922775)

**Enterprise**

- [Detroit to accept crypto](https://detroitmi.gov/news/detroit-become-largest-city-us-accept-cryptocurrency-payments-taxes-other-fees) for fees & taxes using PayPal in mid 2025

* * *

### Job Listings

- [Executive Director](https://docs.google.com/document/d/16qSjXRk2r9v6EnRRVSCoQjrPyJB6icoWgBkCxAme8Nc/edit) for Enterprise Ethereum Alliance

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 1.9 to 84.4 gwei, 10.3 gwei average; zero net issuance at 24.3 gwei 
    
    - 10.5k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,374 - $2,976, currently $2,959, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.039 (Flippening at ~0.164)

**Notable at app layer**

- [Synthetix](https://blog.synthetix.io/synthetix-acquires-ecosystem-leading-perps-platform-kwenta/) acquires Kwenta after spinning it out in 2020

- MakerDAO votes for [Sky brand to stay](https://vote.makerdao.com/polling/QmZzSVJE)

- Safe [proposers](https://help.safe.global/en/articles/235770-proposers): authorized addresses can prepare transactions for owners to review

**Regulation/business/tokens**

- [Michigan pension fund](https://x.com/matthew_sigel/status/1853463874772643926) buys more ETH than BTC via ETFs

**General**

- [Okta vulnerability](https://trust.okta.com/security-advisories/okta-ad-ldap-delegated-authentication-username/) for usernames above 52 characters

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-november-9-2024](https://weekinethereumnews.com/week-in-ethereum-news-november-9-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

- Dec 4-5 – [Columbia CryptoEconomics workshop](http://columbiacryptoeconomics.org/) (New York)

- Dec 6-8 – [ETHIndia](https://ethindia.co/) hackathon

- **Jan 30-31 –** [**EthereumZuri.ch**](https://ethereumzuri.ch/) **conference**

- **Feb 23 - Mar 2 –** [**ETHDenver**](https://www.ethdenver.com/)

- **May 9-11 –** [**ETHDam**](https://www.ethdam.com/) **(Amsterdam)**

- **May 30 - Jun 4 –** [**ETH Belgrade**](https://ethbelgrade.rs/) **hackathon & conference**

- **Jun 12-13 –** [**Protocol Berg**](https://protocol.berlin/) **(Berlin)**

- **Jun 16-18 –** [**DappCon**](https://dappcon.io/) **(Berlin)**

- **Jun 26-28 –** [**ETHCluj**](https://www.ethcluj.org/) **(Romania) conference**

- **Jun 30 - Jul 3 –** [**EthCC**](https://ethcc.io/) **(Cannes) conference**

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

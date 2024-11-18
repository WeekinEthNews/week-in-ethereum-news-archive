---
title: "Week in Ethereum News <br> November 16, 2024"
date: "2024-11-16"
---

## Eth News and Links

Devconnect in 2025 & Devcon in 2026, Justin Drake’s beam chain proposal and Virgil Griffith coming home in April

**Layer 1**

- [FastEthereumCrawler](https://ethresear.ch/t/crawling-the-ethereum-discv5-network-fast/20962): node discovery v5 (discv5) crawler based on Nim implementation

**Research**

- Justin Drake: [beam chain proposal](https://www.youtube.com/watch?v=Plvy7fgFCm4) \[video\], upgrade consensus layer with a batch of features in ~2029 for faster slots, faster finality, SNARKs & quantum security

- Anders Elowsson: [consolidation incentives in Orbit single slot finality](https://notes.ethereum.org/@anderselowsson/Incentives_SSF)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 27.9%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~52% majority
    
    - Consensus layer: Prysm 37% & Lighthouse 33.3%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Client Releases**

- Consensus layer:
    - Lodestar [v1.23.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.23.0): Mekong testnet support & fix for CPU illegal instruction compatibility issue

**Layer 2**

- [Lisk](https://lisk.com/blog/posts/lisk-user-mainnet-is-live/) (former alt-L1) migrated to OP Stack

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7814](https://github.com/ethereum/EIPs/pull/9028/files): Introspection precompiles

- ERCs (application layer):
    - [ERC7815](https://github.com/ethereum/ERCs/pull/712/files): Swap order routing interface
    
    - [ERC7816](https://github.com/ethereum/ERCs/pull/713/files): Schnorr signature scheme for EVM Applications
    
    - [ERC7817](https://github.com/ethereum/ERCs/pull/715/files): Dapp security policy
    
    - [ERC7818](https://github.com/ethereum/ERCs/pull/718/files): Expirable ERC20 

**Stuff for developers**

- OpenZeppelin [community contracts](https://github.com/OpenZeppelin/openzeppelin-community-contracts#readme) (Solidity): experimental contracts, co-developed libraries & newer ERC implementations; unaudited

- Coinbase smart wallet [spend permissions](https://www.smartwallet.dev/guides/spend-permissions/overview): request to spend native & ERC20 tokens for 1-click/no-click user experience

- [DuneScan](https://dune.com/1inch/dunescan): block explorer in Dune

- CTFs:
    - OpenZeppelin [Ethernaut](https://ethernaut.openzeppelin.com/) new levels: impersonator & magic animal carousel
    
    - [Secureum RACE #34](https://ventral.digital/posts/2024/11/10/race-34-of-the-secureum-bootcamp-epoch-infinity/): answers to 8 question Solidity quiz

- 0xPARC [Provable Object Datatype](https://pod.org/) (POD): used in Zupass, FrogCrypto & Meerkat

**Security**

- DeltaPrime [$4.8M exploit](https://rekt.news/deltaprime-rekt2/) on Arbitrum & alt L1, attacker then staked stolen funds

- Red Guild: [Phishing Dojo](https://phishing.therektgames.com/), interactive quiz on identifying phishing attacks

**Ecosystem**

- Devcon [videos](https://www.youtube.com/@EthereumFoundation/videos)

- Devconnect next up in 2025 & Devcon in 2026, [suggest a location](https://forum.devcon.org/c/ethereum-events-location-suggestions/14)

- Evan’s dumbing down of Vitalik’s roadmap explainers: [the Verge](https://x.com/evan_van_ness/status/1856067071945388374), [the Purge](https://twitter.com/evan_van_ness/status/1856381066900033905) & [the Splurge](https://x.com/evan_van_ness/status/1856745233850978425)

* * *

### Job Listings

- Nethermind: [Auditor](https://job-boards.eu.greenhouse.io/nethermind/jobs/4411504101), [Agent Engineer](https://job-boards.eu.greenhouse.io/nethermind/jobs/4465865101), [Content Marketing Manager](https://job-boards.eu.greenhouse.io/nethermind/jobs/4427133101) & [Researcher](https://job-boards.eu.greenhouse.io/nethermind/jobs/4466531101)

- [Executive Director](https://docs.google.com/document/d/16qSjXRk2r9v6EnRRVSCoQjrPyJB6icoWgBkCxAme8Nc/edit) for Enterprise Ethereum Alliance

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 4.4 to 131.5 gwei, 24.5 gwei average; zero net issuance at 24.3 gwei 
    
    - 0.3k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,967 - $3,396, currently $3,096, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.034 (Flippening at ~0.164)

**Notable at app layer**

- ERC4337 [shared user operations pool](https://mirror.xyz/0x836F73BE367a8215FCab4C15E5012DaF574b9Ce4/F3CTe3nmBbm_X_Ee9hD2RyezBDueKnBZts1ZmUY8138) live on mainnet, Arbitrum & OP mainnet

- Vitalik: [info finance category](https://vitalik.eth.limo/general/2024/11/09/infofinance.html), includes prediction & decision markets

**Regulation/business/tokens**

- [Polymarket CEO raided](https://nypost.com/2024/11/13/business/fbi-seizes-polymarket-ceos-phone-electronics-after-betting-platform-predicts-trump-win-source/) by FBI

- [SEC sued by 18 states](https://x.com/fund_defi/status/1857164872011645014) for regulatory overreach in crypto

- [US Attorney's Office SDNY](https://www.reuters.com/legal/manhattan-us-attorney-scale-back-crypto-cases-prosecutor-says-2024-11-15/) devoting fewer resources to harass crypto

- [ETH ETF](https://farside.co.uk/eth/) net positive lifetime inflows

- Rekt: [CryptoPunks & NFT influencers](https://rekt.news/under-the-influence/)

**General**

- [Virgil Griffith coming home](https://x.com/aurbelis/status/1856921347538260324) in April

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-november-16-2024](https://weekinethereumnews.com/week-in-ethereum-news-november-16-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Dec 4-5 – [Columbia CryptoEconomics workshop](http://columbiacryptoeconomics.org/) (New York)

- Dec 6-8 – [ETHIndia](https://ethindia.co/) hackathon

- Jan 30-31 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Feb 23 - Mar 2 – [ETHDenver](https://www.ethdenver.com/)

- May 9-11 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon 

- May 30 - Jun 4 – [ETH Belgrade](https://ethbelgrade.rs/) hackathon & conference

- Jun 12-13 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Jun 16-18 – [DappCon](https://dappcon.io/) (Berlin)

- Jun 26-28 – [ETHCluj](https://www.ethcluj.org/) (Romania) conference

- Jun 30 - Jul 3 – [EthCC](https://ethcc.io/) (Cannes) conference

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

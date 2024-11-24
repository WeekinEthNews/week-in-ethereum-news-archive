---
title: "Week in Ethereum News <br> November 23, 2024"
date: "2024-11-22"
---

## Eth News and Links

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- [Client testing call #13](https://ethereum-magicians.org/t/client-testing-call-13-november-21-2024/21782): pectra-devnet-4 not finalizing, plan to deprecate next week and pectra-devnet-5 spec discussion, PeerDAS & EOF will rebase once spec released
    - Reminder: [Mekong testnet](https://blog.ethereum.org/2024/11/07/introducing-mekong-testnet) live, app/wallet devs & stakers can test Pectra upgrade

- Consensus-specs [v1.5.0-alpha.9](https://github.com/ethereum/consensus-specs/releases/tag/v1.5.0-alpha.9)

- Toni Wahrstätter: [blob fee market](https://ethresear.ch/t/on-blob-markets-base-fee-adjustments-and-optimizations/21024), proposal to increase blob count & reduce execution layer payload size via EIP7623 (increase calldata cost) and analysis of other potential changes

[**Fusaka**](https://eips.ethereum.org/EIPS/eip-7607) **(Osaka + Fulu) upgrade**

- [PeerDAS from scratch](https://hackmd.io/@manunalepa/peerDAS) explainer

**Layer 1**

- [EIP4444 (history expiry) implementation plan](https://hackmd.io/Dobc38YVQ1qmbbyI6LcFqA?view): pre-merge data expiry planned for May 1 using Portal network, EIP7801, ERA & Erigon torrents

- Anders Elowsson: [issuance reward curve](https://x.com/weboftrees/status/1859845411118383570), could reduce to a new curve over 1-2 years

- EIP7732 ePBS:
    - [ePBS breakout #13](https://ethereum-magicians.org/t/epbs-breakout-13-november-22-2024/21786): discussed withdrawals when building on empty blocks and how staking pool operators can become builders
    
    - Potuz: [case for ePBS in Fusaka upgrade](https://hackmd.io/@potuz/Bkcwd5hG1x)

- [Péter Szilágyi](https://x.com/peter_szilagyi/status/1857703746236788974) (Geth) taking a sabbatical

**Research**

- [Metaclear](https://ethresear.ch/t/transport-privacy-exploration-of-the-validator-relayer-builder-api/21050): transport-level privacy leaks at validator-relay interfaces

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: **Geth ~43% & Nethermind ~36%** (estimate based on 74% self reported data)
    
    - Consensus layer: **Prysm 35%**
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Client Releases**

- Execution layer:
    - Geth: [v1.14.12](https://github.com/ethereum/go-ethereum/releases/tag/v1.14.12): changes in tracing & signing, database optimizations, RISC-V docker images and removes personal RPC namespace & unlock flag
    
    - Reth [v1.1.2](https://github.com/paradigmxyz/reth/releases/tag/v1.1.2): payload fetching improvements, bug fixes and OP Stack Holocene upgrade support

**Layer 2**

- L2Beat [user operations per second](https://x.com/l2beat/status/1859554770005938551) (UOPS) added to activity dashboard

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7819](https://eips.ethereum.org/EIPS/eip-7819): Create delegate
    
    - [EIP7822](https://github.com/ethereum/EIPs/pull/9041/files): EVM modular arithmetic extensions
    
    - [EIP7823](https://github.com/ethereum/EIPs/pull/9046/files): Set upper bounds for MODEXP

- ERCs (application layer):
    - [ERC7820](https://github.com/ethereum/ERCs/pull/723/files): Access control registry
    
    - [ERC7821](https://github.com/ethereum/ERCs/pull/726/files): Minimal batch executor interface
    
    - [ERC7824](https://github.com/ethereum/ERCs/pull/728/files): State channels with account abstraction

**Stuff for developers**

- Reminder: [Devcon faucet](https://devcon-mekong-faucet.pk910.de/), claim testnet ETH for Mekong, Sepolia & Holešky using Zupass

- Trail of Bits: [AI Solidity code completion evaluated](https://blog.trailofbits.com/2024/11/19/evaluating-solidity-support-in-ai-coding-assistants/), best commercial: Claude 3 Opus & best local: DeepSeek Coder

- [Prolog on Ethereum](https://github.com/r55-eth/r55/blob/prolog/r55/erc20.pl): prototype integrated with revm alongside R55

- [Solchip8](https://www.piapark.me/chip-8-emulation-on-evm/): CHIP-8 (interpreted language from 70’s 8-bit microcomputers) emulator contract

- Devcon CTFs:
    - Immunefi [ETH Escape](https://escape.ctf.mt/): challenges open to all for 2 weeks
    
    - [BuidlGuidl CTF game](https://ctf.buidlguidl.com/): 12 Solidity challenges

**Ecosystem**

- [EF internships 2025](https://blog.ethereum.org/2024/11/16/announcing-ef-internship-program): 12 weeks, research or software engineering, apply by December 9

- [ETHGlobal Bangkok](https://x.com/ethglobal/status/1858086013576585678) hackathon finalists

**Enterprise**

- McDonald’s [McCafé Doodles holiday cups](https://mcdonalds.doodles.app/) in US

* * *

### Job Listings

- Nethermind: [Auditor](https://job-boards.eu.greenhouse.io/nethermind/jobs/4411504101), [Agent Engineer](https://job-boards.eu.greenhouse.io/nethermind/jobs/4465865101), [Content Marketing Manager](https://job-boards.eu.greenhouse.io/nethermind/jobs/4427133101) & [Researcher](https://job-boards.eu.greenhouse.io/nethermind/jobs/4466531101)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 5.9 to 48.0 gwei, 13.0 gwei average; zero net issuance at 24.3 gwei 
    
    - 8.4k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,053 - $3,419, currently $3,320, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.034 (Flippening at ~0.164)

**Regulation/business/tokens**

- [Alex Pertsev](https://x.com/alex_pertsev/status/1859701374814126484) remains in pre-trial detention

- [SEC’s dealer rule struck down](https://theblockchainassociation.org/blockchainassociation-and-cfat-prevail-against-sec-dealer-rule-struck-down/) by District court as SEC exceeded statutory authority

- [SEC Chair Gary Gensler](https://www.sec.gov/newsroom/press-releases/2024-182) stepping down January 20

- [”Dutch” sentenced to 5 years & “Razzlekhan” to 18 months](https://www.coindesk.com/policy/2024/11/18/bitfinex-hack-launderer-heather-razzlekhan-morgan-sentenced-to-18-months-in-prison/) for laundering BTC from Bitfinex 2016 hack

- [21Shares adds ETH staking ETP](https://www.21shares.com/en-eu/product/ethc) in EU

**General**

- [NIST deprecating ECDSA](https://nvlpubs.nist.gov/nistpubs/ir/2024/NIST.IR.8547.ipd.pdf) after 2030 & disallowing use after 2035

- Justin Thaler: [Jolt roadmap](https://a16zcrypto.com/posts/article/getting-bugs-out-of-snarks/) to formally verified implementation

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-november-23-2024](https://weekinethereumnews.com/week-in-ethereum-news-november-23-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Dec 4-5 – [Columbia CryptoEconomics workshop](http://columbiacryptoeconomics.org/) (New York)

- Dec 6-8 – [ETHIndia](https://ethindia.co/) hackathon

- **Dec 9 –** [**EF internships 2025**](https://blog.ethereum.org/2024/11/16/announcing-ef-internship-program) **application deadline**

- Jan 30-31 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Feb 23 - Mar 2 – [ETHDenver](https://www.ethdenver.com/)

- **Apr 4-6 –** [**ETHGlobal Taipei**](https://ethglobal.com/events/taipei) **hackathon**

- May 9-11 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon 

- **May 27-29 –** [**ETHPrague**](https://ethprague.com/) **conference**

- **May 30 - Jun 1 –** [**ETHGlobal Prague**](https://ethglobal.com/events/prague) **hackathon**

- May 30 - Jun 4 – [ETH Belgrade](https://ethbelgrade.rs/) hackathon & conference

- Jun 12-13 – [Protocol Berg](https://protocol.berlin/) (Berlin) conference

- Jun 16-18 – [DappCon](https://dappcon.io/) (Berlin)

- Jun 26-28 – [ETHCluj](https://www.ethcluj.org/) (Romania) conference

- Jun 30 - Jul 3 – [EthCC](https://ethcc.io/) (Cannes) conference

- **Jul 4-6 –** [**ETHGlobal Cannes**](https://ethglobal.com/events/cannes) **hackathon**

- **Aug 15-17 –** [**ETHGlobal New York**](https://ethglobal.com/events/newyork2025) **hackathon**

- **Sep 26-28 –** [**ETHGlobal New Delhi**](https://ethglobal.com/events/newdelhi) **hackathon**

- **Nov –** [**ETHGlobal Devconnect**](https://ethglobal.com/events/ethglobal-devconnect) **hackathon**

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

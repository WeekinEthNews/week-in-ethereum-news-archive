---
title: "Week in Ethereum News <br> September 7, 2024"
date: "2024-09-07"
---

## Eth News and Links

CFTC regulation by enforcement & EF Research AMA

**All core devs**

- [All Core Devs – Consensus (ACDC) #141](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-141-september-5-2024/20890):
    - **Pectra (Prague + Electra) upgrade**:
        - **Pectra-devnet-2**: Prysm fixed finality bug, deprecated
        
        - **Pectra-devnet-3**: testing locally with ready clients, launch next week
        
        - **EIP7685 execution layer requests**: proposed change to return requests as opaque hex bytes, review at ACDE
        
        - **EIP6110 validator deposits onchain**: proposed change to queue deposit requests to avoid consensus layer DoS
        
        - **PeerDAS**:
            - **PeerDAS-devnet-2**: testing locally with subset of clients, launch soon
            
            - **Blob proof generation timing:** discussed options for local builders with lower spec hardware, proposal to pre-prepare blobs on consensus layer
        
        - **Remove SSZ unions** from consensus spec proposal (not used in production)

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- [Pectra testing call #3](https://ethereum-magicians.org/t/pectra-testing-call-3-2-september-2024/20946)

- [EOF implementers call #57](https://ethereum-magicians.org/t/eof-implementers-call-57-sep-4-2024/20956): discussed EIP7761 ISCONTRACT & alternatives to support ERC721/1155 safe transfer

- [PeerDAS breakout #7](https://ethereum-magicians.org/t/peerdas-breakout-7-september-3-2024/20891): blob proofs could take up to 1 second to compute

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.4%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~52% majority
    
    - Consensus layer: Prysm 36%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Research**

- [EF Research AMA](https://www.reddit.com/r/ethereum/comments/1f81ntr/ama_we_are_ef_research_pt_12_05_september_2024/) on r/Ethereum:
    - [ETH value accrual](https://www.reddit.com/r/ethereum/comments/1f81ntr/comment/llbzkm1), [L1 scaling](https://www.reddit.com/r/ethereum/comments/1f81ntr/comment/llbyqky), [blob price discovery](https://www.reddit.com/r/ethereum/comments/1f81ntr/comment/llbwkc1), [L2 sequencer decentralization](https://www.reddit.com/r/ethereum/comments/1f81ntr/comment/llhq1rj), [zk research](https://www.reddit.com/r/ethereum/comments/1f81ntr/comment/llbyj2r), [credible neutrality](https://www.reddit.com/r/ethereum/comments/1f81ntr/comment/llc8h7g/), [issuance](https://www.reddit.com/r/ethereum/comments/1f81ntr/comment/llco6kk), [EF runway](https://www.reddit.com/r/ethereum/comments/1f81ntr/comment/lldvwme), [pivot Fusaka upgrade from Verkle](https://www.reddit.com/r/ethereum/comments/1f81ntr/comment/llft9ii) and more

- [ERC4337 embedded fee markets](https://ethresear.ch/t/embedded-fee-markets-and-erc-4337-part-2/20384), solutions to prevent users from overpaying

**Client Releases**

- Execution layer:
    - Erigon [v3.0.0-alpha3](https://github.com/erigontech/erigon/releases/tag/3.0.0-alpha3): 30% reduction of latest state, 2x reduction in chaindata, 2x less RAM & prune doesn't impact chain-tip performance; resync required

**Layer 2**

- Arbitrum [Stylus](https://blog.arbitrum.io/arbitrum-stylus-mainnet/) live on Arbitrum One & Nova, adds Web Assembly VM, write contracts in languages that compile into WASM such as Rust, composable with EVM contracts

- [Base plan to increase gas target](https://base.mirror.xyz/6NDvVKw8x5obo3h1OgQx582hF73m81CnJabgbRneW2Q) by 1 Mgas/s weekly towards goal of 1 Ggas/s
    - [Blobspace saturation](https://x.com/ryanberckmans/status/1831726177397940648) projected for February

- [Matter Labs](https://x.com/gluk64/status/1830968752210375030) (ZKsync) laid off ~16% of team

**For Stakers**

- Geth node on [Banana Pi BPI-F3 RISCV board](https://x.com/EthereumOnARM/status/1831620151344525459), consensus clients struggle to run currently

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7762](https://github.com/ethereum/EIPs/pull/8849/files): Increase MIN\_BASE\_FEE\_PER\_BLOB\_GAS (to speed up price discovery)

- ERCs (application layer):
    - [ERC7763](https://github.com/ethereum/ERCs/pull/615/files): App keys for fully embedded accounts
    
    - [ERC7764](https://github.com/ethereum/ERCs/pull/618/files): Buyer-seller negotiable pricing

**Stuff for developers**

- Solidity [v0.8.27](https://soliditylang.org/blog/2024/09/04/solidity-0.8.27-release-announcement): require with custom errors, caching of optimized IR for faster compilation and parser support for transient storage variables

- [Scaffold-ETH 2 extensions](https://x.com/buidlguidl/status/1832071356604654004) hackathon finalists

- EVMole [v0.4](https://x.com/cdump/status/1829816548837494914) (function selector extractor): improved accuracy of function state mutability extraction and improved speed for Python & JavaScript

- [Supersim](https://github.com/ethereum-optimism/supersim/#readme): simulate interoperable OP Stack Superchain locally

- [CTF Challenges](https://github.com/BlockChomper/ctf-challenges#readme): Uniswap V2 ERC4626 vulnerable vault

**Security**

- Penpie [$27M exploit](https://blog.penpiexyz.io/penpie-post-mortem-report-1ac9863b663a) on mainnet & Arbitrum via reentrancy 

- [L2 DAI deployer compromised](https://x.com/godsflaw/status/1830986263098466561) allowing attacker to deploy contracts on other L2s with same address as DAI on Optimism & Arbitrum

- [Vyper compiler](https://x.com/pcaversaccio/status/1831968493580804387) added to EF bounty program

**Ecosystem**

- [Devcon community hub](https://forum.devcon.org/c/community-hubs/15) proposals

- [ETHAccra](https://taikai.network/en/ethaccra/hackathons/hackathon2024/projects) hackathon projects

* * *

### Job Listings

- [Status](https://status.app/) [free.technology](https://free.technology/) is hiring a [Business Developer](https://grnh.se/63f67b381us). More [jobs](https://free.technology/jobs) at IFT!

- [Nomos](https://free.technology/nomos) is hiring [Business Developer](https://grnh.se/6a2297081us), [Rust Engineer](https://grnh.se/bd96340e1us) & [Applied Researcher](https://grnh.se/03fe75801us)!

- Join [Witnet](https://witnet.io/) as a [Community Builder](https://wellfound.com/l/2Akjg4)! Full-time, remote opportunity.

- Gnosis seek [CoreDevs](https://gnosis.jobs.personio.com/job/893408?_pc=1517287), [Sr Algorithm Engineer](https://gnosis.jobs.personio.com/job/1698369?_pc=1517287), [Sr Smart Contract Engineer](https://gnosis.jobs.personio.com/job/1698390?_pc=1517287)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 0.4 to 53.4 gwei, 3.2 gwei average; zero net issuance at 24.0 gwei 
    
    - 16k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,165 - $2,548, currently $2,233, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.041 (Flippening at ~0.164)

**Notable at app layer**

- Euler [v2](https://euler.finance/blog/euler-v2-is-live) live, modular lending, use vaults as collateral in other vaults

- [Lextek](https://x.com/z0r0zzz/status/1831388124326588759) v0: onchain legal forms live on Base, starting with SAFE & DEAL (escrow & invoicing)

- Snapshot [v2](https://snapshot.mirror.xyz/0qnfjmE0SFeUykArdi664oO4qFcZUoZTTOd8m7es_Eo): discussions view, delegate dashboard and improved voting/proposal UX, beta

- [Atomic](https://wirehaired-calf-089.notion.site/Hi-This-is-Atomic-0c850bf5197846e5973a1bd9eb07e23c): exercise challenges live on Base, stake USDC, log Strava workouts & claim stake

**Regulation/business/tokens**

- CFTC regulation by enforcement:
    - Dissent by [Commissioner Mersinger](https://www.cftc.gov/PressRoom/SpeechesTestimony/mersingerstatement090424) & [Commissioner Pham](https://www.cftc.gov/PressRoom/SpeechesTestimony/phamstatement090424) of [Uniswap enforcement](https://www.cftc.gov/PressRoom/PressReleases/8961-24) for not blocking leverage tokens

- [Kalshi won against CFTC](https://www.coindesk.com/policy/2024/09/06/kalshi-cleared-to-offer-congressional-prediction-markets-in-victory-against-cftc) to list prediction market for control of US congress

- [Galois Capital settled with SEC](https://x.com/Galois_Capital/status/1831015164688093539) for using a disclosed non-qualified custodian when the SEC won’t approve custodians

- [FBI](https://www.ic3.gov/Media/Y2024/PSA240903): North Korea targeting crypto projects via social engineering

**General**

- Vitalik: [glue & coprocessor architecture](https://vitalik.eth.limo/general/2024/09/02/gluecp.html), central glue (high generality but low efficiency) shuttles data between coprocessors (low generality buy high efficiency) e.g. EVM & precompiles

- [EUCLEAK](https://ninjalab.io/eucleak/): Infineon ECDSA side-channel vulnerability, requires physical access, impacts some [YubiKeys](https://www.yubico.com/support/security-advisories/ysa-2024-03/)

- [Notes on extractable witness encryption](https://www.leku.blog/kzg-we/) for KZG commitments and efficient Laconic OT

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-september-7-2024](https://weekinethereumnews.com/week-in-ethereum-news-september-7-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Sep 9-15 – [ETHSafari](https://ethsafari.xyz/) (Kenya)

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 13-14 – [Ethereum México](https://ethmexico.org/)

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

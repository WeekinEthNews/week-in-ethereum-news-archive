---
title: "Week in Ethereum News <br> January 6, 2024"
date: "2024-01-05"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=6xgxmKfVjtA&t=316s). Recap by [lightclient](https://mirror.xyz/abcoathup.eth/fxJUSVwy6fWzzL-du9AFUhybfz9znKlb16JVw6qTqg0).  Notes from [lightclient](https://twitter.com/lightclients/status/1742963481618289061) & [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-178/):
    - **Testnet upgrade dates confirmed** (assumes no issues): Goerli Jan 17, Sepolia Jan 30 & Holešky Feb 7
    
    - **Pectra (Prague + Electra)**: discussed small feature upgrade first vs focusing on [Verkle](https://verkle.info/) (~18 months) and reviewed [proposed EIPs](https://ethereum-magicians.org/t/prague-electra-network-upgrade-meta-thread/16809)
    
    - **Precompile address ranges**: proposed EIP7587 (reserves 0x100-0x1ff for RIPs)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.71%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~84% supermajority, could possibly cause a chain split, [estimated to cost billions of dollars](https://www.reddit.com/r/ethstaker/comments/18xv282/quantifying_the_damage_a_supermajority_client_can/)
    
    - Consensus layer: Prysm 41%, any client bug over 33.3% could mean [loss of finality](https://eth2book.info/capella/part2/incentives/diversity/#2-client-x-has-more-than-one-third-of-the-stake)

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- [libp2p TCP vs QUIC](https://twitter.com/mempirate/status/1742564119776018717): TCP ~2x speed of QUIC

**Client releases**

- Consensus layer:
    - Nimbus [v24.1.0](https://github.com/status-im/nimbus-eth2/releases/tag/v24.1.0): Goerli testnet Dencun upgrade and adds v3 blocks/{slot} Beacon API end-point

- Execution layer:
    - Erigon [v2.56.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.56.0): Goerli testnet Dencun upgrade
    
    - Nethermind [v1.25.0-rc](https://github.com/NethermindEth/nethermind/releases/tag/1.25.0-rc): Goerli testnet Dencun upgrade and OP Stack Canyon support

**Research**

- [Proposer selection with EIP7251](https://ethresear.ch/t/proposer-selection-with-increased-maxeb-eip-7251/18144) (increase max effective balance): probability remains the same for consolidated validators

**MEV**

- Terence: [timing games with blobs](https://ethresear.ch/t/validator-timing-game-post-eip4844/18129) (post Dencun upgrade), may be more unpredictable

- [Timing.pics](https://timing.pics/) (dashboard of timing games): missed slots & bids selected by entity

**Layer 2**

- [Arbitrum Orbit](https://twitter.com/arbitrum/status/1742954565341700135) supports using an ERC20 token for gas

- [L2s TVL](https://twitter.com/0xstark/status/1742906255662837797) flips other L1s

**EIPs/Standards**

- EIPs
    - Informational [EIP7587](https://github.com/ethereum/EIPs/pull/8074/files): Reserve precompile address range for RIPs

- ERCs (application layer):
    - [ERC7586](https://github.com/ethereum/ERCs/pull/178/files): Interest rate swaps
    
    - [ERC7588](https://github.com/ethereum/ERCs/pull/185/files): Blob transactions metadata JSON schema

**Stuff for developers**

- Reminder: [Solidity developer survey 2023](https://soliditylang.org/blog/2023/12/08/solidity-developer-survey-2023-announcement/) closes January 7

- [Foundry multibuild](https://github.com/PaulRBerg/foundry-multibuild): GitHub Action to test building project with range of Solidity versions

- Overview of [proxy contracts](https://noxx.substack.com/p/smart-contract-patterns-the-proxy)

- Wagmi [v2](https://twitter.com/wevm_dev/status/1742991699842916629): TanStack Query support, connect multiple connectors, switch chains while disconnected and EIP6963 (multi injected provider discovery) support

- Viem [v2](https://twitter.com/wevm_dev/status/1742646513367687280): low-level OP Stack actions & utilities and enhanced types

- Secureum RACE #25: [8 question Solidity quiz & answers](https://ventral.digital/posts/2024/1/1/race-25-of-the-secureum-bootcamp-epoch-infinity/)

**Security**

- Gamma (liquidity management) [$4.5M exploit](https://rekt.news/gamma-strategies-rekt/) on Arbitrum via price manipulation

- Radiant (Aave v2 fork) [$4.5M exploit](https://twitter.com/peckshield/status/1742334242120466580) of new USDC market on Arbitrum via known rounding issue

**Ecosystem**

- Vitalik’s [updated roadmap diagram](https://twitter.com/vitalikbuterin/status/1741190491578810445)
    - single slot finality (SSF) to resolve PoS design weaknesses, significant progress on rollups & Verkle trees, scourge redesigned, state expiry a low priority and VDFs dead for now

- [Devcon Southeast Asia](https://blog.ethereum.org/2024/01/03/devcon-sea-announcement) in Bangkok, November 12-15

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 7.9 to 329.4 gwei, with 19.8 gwei average
    - Zero net issuance currently at 22.0 gwei 
    
    - 1.7k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,187 - $2,434, currently $2,246

- [ETHBTC](https://ratiogang.com/): currently 0.051 (Flippening at ~0.16)

**Notable at app layer**

- Vitalik calls for [L2 CCIP resolvers](https://twitter.com/vitalikbuterin/status/1742540651797823948) for low cost ENS subdomains

- Daimo [bundle compression](https://daimo.com/blog/bulk) reduces cost of ERC4337 transactions on L2

- State of [private voting](https://odyslam.com/blog/state-of-private-voting/)

- [Regen Learnings](https://gov.gitcoin.co/t/regenlearnings-xyz-research-group/17361): research group for public goods funding

* * *

### Job Listings

- Status is hiring: Technical Chief Operating Officer - [Apply here](https://grnh.se/0ecdaa981us)

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US tax code: [receipt of $10k+ in crypto](https://twitter.com/jerrybrito/status/1742246479593382207) (for trade/business) to be reported to IRS within 15 days

- [SBF second trial dropped by DoJ](https://twitter.com/watcherguru/status/1740941426236752039), including charges for unlawful campaign contributions

- Logan Paul’s [CryptoZoo buy back](https://twitter.com/LoganPaul/status/1742965334645276708) after game not delivered, in exchange for waiving claims

- [UK users of centralized exchanges](https://www.cnbc.com/2024/01/05/coinbase-gemini-plan-user-risk-assessments-in-uk-ahead-of-new-rules.html) required to complete investor declaration

**General**

- Orbit bridge [$81M hack](https://rekt.news/orbit-bridge-rekt/)

- [Orange Spain internet outage](https://www.bleepingcomputer.com/news/security/hacker-hijacks-orange-spain-ripe-account-to-cause-bgp-havoc/), RIPE account hacked to misconfigure BGP routing & RPKI config

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-january-6-2024](https://weekinethereumnews.com/week-in-ethereum-news-january-6-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jan 15 – EF’s [Next Billion fellowship cohort 4](https://fellowship.ethereum.foundation/) deadline

- Jan 17 – [Goerli testnet](https://github.com/ethereum/EIPs/pull/8051) Dencun upgrade epoch 231680

- Jan 30 – [Sepolia testnet](https://github.com/ethereum/EIPs/pull/8051) Dencun upgrade epoch 132608 (assuming no issues)

- Feb 2-4 – [ETH Cinco de Mayo](https://ethcincodemayo.com/) hackathon (Cholula, Puebla)

- Feb 3 – [Ethereum Lima Day](https://ethlimaday.org/)

- Feb 7 – [Holešky testnet](https://github.com/ethereum/EIPs/pull/8051) Dencun upgrade epoch 29696 (assuming no issues)

- Feb 23-Mar 3 – [ETHDenver](https://www.ethdenver.com/) BUIDLWeek & hackathon

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024) hackathon

- Mar 19-21 – [ETH Canal](http://ethcanal.xyz) (Panama City, Panamá) conference & hackathon

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) hackathon & conference 

- Mar 29-31 – [ETH Seoul](https://www.ethseoul.org/) conference

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) virtual hackathon

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Apr 12-14 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/)

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- Jun 3-5 – [ETH Belgrade](https://ethbelgrade.rs/) conference

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 26-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- **Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)**

- **Nov 15-17 –** [**ETHGlobal Bangkok**](https://ethglobal.com/events/bangkok) **hackathon**

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

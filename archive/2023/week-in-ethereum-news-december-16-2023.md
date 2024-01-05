---
title: "Week in Ethereum News <br> December 16, 2023"
date: "2023-12-16"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=1mLDIRmGtNk&t=334s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-124/):
    - **Devnet-12**: Prysm joined, MEV-Boost being tested
    
    - **Goerli shadow fork 1**: syncing started
    
    - Discussions on SSE block event for block propagation times, slashable message propagation and GossipSub IDONTWANT control message

- Dencun interop testing [call video](https://www.youtube.com/watch?v=B88GLgKvxuI&t=76s)

- Tim Beiko’s [core devs update](https://tim.mirror.xyz/HzH5MpK1dnw7qhBSmzCfdCIxpwpD6DpwlfxtaAwEFro): Dencun upgrade EIPs, EIP process changes and Prague/Electra planning

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.98%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~84% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm 41% & Lighthouse 34%, any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Yoav: [ERC4337 (account abstraction) vs EIP3074 (execution abstraction)](https://notes.ethereum.org/@yoav/erc-4337-vs-eip-3074-false-dichotomy)

- Vitalik: [enshrined zkEVMs at Layer 1](https://notes.ethereum.org/@vbuterin/enshrined_zk_evm), tradeoffs and design challenges

- [Ethernets.io](https://hackmd.io/@angaz/BJ-kJ3bIT) (node crawler): ~17k nodes found, 60% not accepting connections

- [Monitoreth.io](https://twitter.com/miga_labs/status/1735344631112466626) (consensus layer dashboard) updated with ISP & staking entities distribution

**For Stakers**

- EthStaker: [DVT home staker program](https://paragraph.xyz/@ethstaker/dvtprogram), pilot reimbursing hardware costs of new stakers

**Client releases**

- Consensus layer:
    - Lodestar [v1.12.1](https://github.com/ChainSafe/lodestar/releases/tag/v1.12.1): patch for v1.12 block root errors ([post-mortem](https://twitter.com/lodestar_eth/status/1734628608595878309))
    
    - Teku [v23.12.0](https://github.com/Consensys/teku/releases/tag/23.12.0): adds checkpoint-sync-url option and performance improvements

- Execution layer
    - Nethermind [v1.24.0](https://github.com/NethermindEth/nethermind/releases/tag/1.24.0): not downgradable, improvements to headers database

**Research**

- Timing games: [cost of artificial latency in PBS](https://ethresear.ch/t/the-cost-of-artificial-latency-in-the-pbs-context/17847)

**Layer 2**

- [Arbitrum One sequencer & feed stalled](https://status.arbitrum.io/clq6te1l142387b8n5bmllk9es) during surge in traffic
    - [90% of transactions](https://twitter.com/hildobby_/status/1735710373192335637) were inscriptions

- RollCall (L2 standards) [call video](https://www.youtube.com/watch?v=omgzqe72e0I): discussed RIP7212 (secp256r1 precompile), RIP7560 (native account abstraction) and EIP3074 (AUTH & AUTHCALL)

**EIPs/Standards**

- EIPs:
    - Meta [EIP7577](https://github.com/ethereum/EIPs/pull/8034/files): Versioning scheme for EIPs

- RIPs (Rollup Improvement Proposals):
    - [RIP7212](https://github.com/ethereum/RIPs/pull/5/files): Precompile for secp256r1 Curve Support (moved from EIPs)

- ERCs (application layer):
    - [ERC7573](https://github.com/ethereum/ERCs/pull/153/files): Conditional-upon-Transfer-Decryption for Delivery-versus-Payment
    
    - [ERC7574](https://github.com/ethereum/ERCs/pull/155/files): Authentication SBT using credential
    
    - [ERC7575](https://github.com/ethereum/ERCs/pull/157/files): Partial and extended ERC4626 vaults
    
    - [ERC7578](https://github.com/ethereum/ERCs/pull/160/files): Physical asset redemption
    
    - [ERC7579](https://github.com/ethereum/ERCs/pull/163/files): Minimal modular smart accounts
    
    - [ERC7580](https://github.com/ethereum/ERCs/pull/165/files): Inter dapp tracking interface

**Stuff for developers**

- Foundry:
    - Forge-std [v1.7.4](https://github.com/foundry-rs/forge-std/releases/tag/v1.7.4): adds Balance, Extcodesize, Extcodehash, Extcodecopy as account access kinds and new cheat codes to delete snapshots
    
    - [Polygon deployment & upgrade libraries](https://twitter.com/gretzke/status/1734210579294814691) (JavaScript), Forge Chronicles (creates JSON & markdown deployment log), Storage Delta (compares storage layouts) & Deployer Kit (generate deployer contracts for upgradeable contracts), beta

- [Create an AMM in Vyper](https://dev.to/rabuawad/create-your-own-uniswap-defi-application-from-scratch-using-vyper-python-3i9h) using Ape (Python contract dev framework)

- [Code MASTER](https://github.com/hananbeer/master): create AST mutators

- EVMole [v0.2.0](https://twitter.com/cdump/status/1734930002997592159) (function selector extractor): adds extracting function arguments

- [Ponder](https://ponder.sh/blog/introducing-ponder) (dapp backend framework): index events, generate GraphQL API, local dev server with hot reloading, implemented in TypeScript

- [FUZD](https://twitter.com/etherplay/status/1734875536608882799): commit/reveal system, executes delayed transactions decrypted at execution time, alpha

- OpenZeppelin [Defender v2](https://twitter.com/openzeppelin/status/1734619213711515921), public beta, new modules: Code (analysis of PRs), Audit (track issues & resolutions), Deploy, Monitor, Incident Response, Actions  & Access Control

**Security**

- [Ledger Connect Kit library supply chain attack](https://www.ledger.com/blog/a-letter-from-ledger-chairman-ceo-pascal-gauthier-regarding-ledger-connect-kit-exploit), drainer injected into dapps

- OKX DEX [$370k exploit](https://twitter.com/okxweb3/status/1734794114657657004), deprecated contract compromised

- Hypr bridge [exploit](https://www.hypr.network/articles/incident-postmortem-bridge-exploit), contract reinitialized, built on fork of OP Stack develop branch

- Cyfrin Updraft [security & auditing course](https://updraft.cyfrin.io/courses/security) (22 hours)

**Ecosystem**

- ETH supply [below Vitalik’s proposed EIP960 ETH supply cap](https://evanvanness.com/post/736817590099410945/eth-supply-breaks-below-vitaliks-rejected-eip960)

- ETHIndia [hackathon finalists](https://twitter.com/ethglobal/status/1733819070208688275)

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 16.9 to 346.6 gwei, with 41.7 gwei average
    - Zero net issuance currently at 21.9 gwei 
    
    - 15k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,161 - $2,385, currently $2,223

- [ETHBTC](https://ratiogang.com/): currently 0.053 (Flippening at ~0.16)

**Notable at app layer**

- [ENS root being transferred](https://twitter.com/nicksdjohnson/status/1735667398051557640) to the ENS DAO

- Coinbase wallet [buy/send USDC for free](https://twitter.com/coinbasewallet/status/1735016950596554783) on Layer 2

- [Synthetix](https://blog.synthetix.io/the-end-of-synthetix-token-inflation/) ends SNX inflation

* * *

### Job Listings

- [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db) wanted by EF

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

**Job listings: $600 for four issues** (75 character limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [SEC denied Coinbase’s petition](https://twitter.com/iampaulgrewal/status/1735716481541996640) for crypto rules; [SEC Republican members disagree](https://www.sec.gov/news/statement/peirce-uyeda-petition-121523)

- [Tether](https://tether.to/en/tether-introduces-new-policy-to-strengthen-ecosystem-security/) freezing wallets on OFACs list

- [KuCoin](https://ag.ny.gov/press-release/2023/attorney-general-james-secures-more-22-million-cryptocurrency-platform-operating) settlement with New York: cease operations in the state, refund users & $5.3M penalty

- [Four people charged](https://www.justice.gov/opa/pr/four-individuals-charged-laundering-millions-cryptocurrency-investment-scams) for laundering proceeds from “pig butchering” crypto investment scams

- [Coinbase International Exchange](https://www.coinbase.com/blog/coinbase-international-exchange-to-launch-spot-markets) spot ETH-USDC for non-US institutional clients

**General**

- S&P Global Ratings [stablecoin stability assessment](https://www.prnewswire.com/news-releases/sp-global-ratings-launches-stablecoin-stability-assessment-302012532.html)

- [BIS tighten stablecoin criteria](https://www.bis.org/press/p231214.htm) in 2022 proposal that banks can hold up to 2% in crypto

- [Twitter XSS vulnerability](https://twitter.com/shoucccc/status/1734802168723734764): attackers could have taken over accounts

- [Arecibo](https://blog.lurk-lang.org/posts/arecibo-supernova/): implementation of SuperNova

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-16-2023](https://weekinethereumnews.com/week-in-ethereum-news-december-16-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jan 15 – EF’s [Next Billion fellowship cohort 4](https://fellowship.ethereum.foundation/) deadline

- Feb 2-4 – [ETH Cinco de Mayo](https://ethcincodemayo.com/) hackathon (Cholula, Puebla)

- **Feb 3 –** [**Ethereum Lima Day**](https://ethlimaday.org/)

- Feb 23-Mar 3 – [ETHDenver](https://www.ethdenver.com/) BUIDLWeek & hackathon

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024)

- Mar 19-21 – [ETH Canal](http://ethcanal.xyz) (Panama City, Panamá) conference & hackathon

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) hackathon & conference

- **Mar 29-31 –** [**ETH Seoul**](https://www.ethseoul.org/)

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) (virtual)

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference & hackathon

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney)

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/)

- **May 31-Jun 2 –** [**ETHPrague**](https://ethprague.com) **conference & hackathon**

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels)

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels)

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) (virtual)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024)

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024)

- Nov – [ETHGlobal DevCon](https://ethglobal.com/events/devcon2024)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

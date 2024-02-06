---
title: "Week in Ethereum News <br> February 3, 2024"
date: "2024-02-03"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=KE4VH-lSfHg&t=154s). Recap by [Tim Beiko](https://mirror.xyz/abcoathup.eth/qWo4915gMtK2r2jgNRrtf4rOpeoBUK9SeYxv5tOGEFc).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1753125753020137890) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-180/):
    - **Mainnet**: Dencun upgrade date to be set on ACDC next week; assumes no issues with Holešky testnet upgrade, Goerli blob expiry & churn limit testing and Devnet 12 blob spamming
    
    - **Sepolia testnet**: [uneventfully upgraded](https://twitter.com/parithosh_j/status/1752468658868126030) to Dencun, blobs are flowing
    
    - **Prague upgrade**: Discussions on including EOF or EIP4444 (bound historical data) and how [Portal network](https://notes.ethereum.org/@Kolby-ML/HJ-9D5aYp) could distribute historical data; scope to be finalized on ACDE in two weeks
    
    - **Osaka upgrade:** Verkle agreed as core feature; [Verkle overview & current status](https://docs.google.com/presentation/d/1R_UkS0WyGN1FK3qYxSBK5zZxBbN8Cx2mFHQj6rQ0jRA): ~2 weeks to build Verkle tree prior to upgrade & execution 10% slower

**Osaka upgrade (meta** [**EIP7607**](https://github.com/ethereum/EIPs/pull/8159/files)**)**

- [Kaustinen testnet](https://twitter.com/gballet/status/1753390094567047643) (Verkle) rebooted with new features & fixes

- Verkle implementers [call video](https://www.youtube.com/watch?v=YTwUc38GiUI&t=7s) & [notes](https://twitter.com/rudolf6_/status/1752966751254618547)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.82%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth 78% supermajority, could cause a chain split
    
    - Consensus layer: Prysm 39%, any client bug over 33.3% could mean loss of finality
    
    - **Research starting for** [**validators to provide client info privately**](https://ethresear.ch/t/allowing-validators-to-provide-client-information-privately-a-project-by-nethermind-research-and-nethermind-core/18527)

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Research**

- [Unconditional inclusion lists](https://ethresear.ch/t/unconditional-inclusion-lists/18500) (for censorship resistance): transactions are included in a first or second slot, otherwise they are unconditionally added in order to the bottom of the second slot

**Client releases**

- Consensus layer:
    - Lodestar [v1.15.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.15.0): fixes for Deneb upgrade, js-libp2p updated to v1 and minor fixes for UX & performance improvements
    
    - Nimbus [v24.2.0](https://github.com/status-im/nimbus-eth2/releases/tag/v24.2.0): stability improvements for Deneb
    
    - Prysm [v4.2.1](https://github.com/prysmaticlabs/prysm/releases/tag/v4.2.1): older CPUs without AVX support will have failures on testnets

- Execution layer:
    - Erigon [v2.57.2](https://github.com/ledgerwatch/erigon/releases/tag/v2.57.2): fix for RpcDaemon seeing recently retired blocks

* * *

### **Support the** [**Roman Storm & Alex Pertsev legal defense fund**](https://juicebox.money/@free-pertsev-and-storm)

![Open source is not a crime](https://weekinethereumnews.com/wp-content/uploads/2024/01/open-source-is-not-a-crime-1024x341.jpg)

The Biden administration is attempting to criminalize open source software development as part of its war on crypto.

Donate to [defend our innocent Ethereum heroes](https://juicebox.money/@free-pertsev-and-storm).  Retweet to [spread awareness](https://twitter.com/rstormsf/status/1749490246000238942).

* * *

**Layer 2**

- Arbitrum One [ArbOS v11](https://forum.arbitrum.foundation/t/aip-arbos-version-11/19696) live, adds Shanghai support (including PUSH0)

- Optimism [bicameral governance for upgrades](https://twitter.com/optimismgov/status/1752847061400334398), citizens house can veto \[Andrew is a badgeholder\]

- RollCall (L2 standards) [fee markets breakout call](https://www.youtube.com/watch?v=URa8Jn-0aU4&t=2s) and [notes](https://twitter.com/abcoathup/status/1753319621439156441); repricing EVM operations, L1 passthrough fees & potential multi-dimensional pricing

**EIPs/Standards**

- EIPs:
    - [EIP7605](https://github.com/ethereum/EIPs/pull/8149/files): Homogeneous validator penalty
    
    - Meta [EIP7607](https://github.com/ethereum/EIPs/pull/8159/files): Hardfork Meta - Osaka
    
    - [EIP7609](https://github.com/ethereum/EIPs/pull/8158/files): Decrease TLOAD/TSTORE pricing
    
    - [EIP7610](https://github.com/ethereum/EIPs/pull/8161/files): Revert creation in case of non-empty storage

- ERCs (application layer):
    - [ERC7604](https://github.com/ethereum/ERCs/pull/223/files): ERC1155 permit approvals
    
    - [ERC7606](https://github.com/ethereum/ERCs/pull/229/files): Transaction risk monitoring
    
    - [ERC7611](https://github.com/ethereum/ERCs/pull/231/files): Sovereign bridged NFTs

**Stuff for developers**

- Remix [v0.42](https://medium.com/remix-ide/remix-release-v0-42-0-56ec48a49ae0): Solidity v0.8.24 now default and GPT help for Circom compiler errors

- [GasliteVest](https://github.com/PopPunkLLC/gaslite-core/blob/main/src/GasliteVest.sol): continuous linear token vesting base contract

- [Soledge](https://github.com/Vectorized/soledge#readme) (Solidity): convert numbers to strings, transient storage helper & reentrancy guard

- [ERC4626 Vault exchange rate manipulation](https://www.euler.finance/blog/exchange-rate-manipulation-in-erc4626-vaults) & mitigations

- [Natspec smells](https://github.com/defi-wonderland/natspec-smells#readme): identify missing or incomplete natspec

- Brownie [v1.20.0](https://github.com/eth-brownie/brownie/pull/1736) (Python): no longer actively maintained

- [Napalm](https://github.com/ConsensysDiligence/napalm#readme): productivity framework for custom Solidity vulnerability detectors

- Farcaster [Frames](https://warpcast.notion.site/Farcaster-Frames-4bd47fe97dc74a42a48d3a234636d8c5): mini apps in posts using an image & buttons to trigger callbacks
    - [Frame verifier](https://github.com/wilsoncusack/frame-verifier#readme) (Solidity): encode/verify MessageData structs containing Frame actions
    
    - OnchainKit [FrameKit](https://github.com/coinbase/onchainkit?tab=readme-ov-file#framekit-%EF%B8%8F) (TypeScript): get Frame HTML, message and metadata

- mesc [v0.2](https://twitter.com/notnotstorm/status/1752027269156245650): configure & manage RPC endpoints

- Secureum RACE #26: [8 question Solidity quiz & solutions](https://ventral.digital/posts/2024/1/30/race-26-of-the-secureum-bootcamp-epoch-infinity/)

**Security**

- ERC1271 (signature validation for contracts) [replay disclosure](https://mirror.xyz/curiousapple.eth/pFqAdW2LiJ-6S4sg_u1z08k4vK6BCJ33LcyXpnNb8yU), possible when the signed digest doesn't include the smart account address

- Abracadabra’s Magic Internet Money [$6.5M exploit](https://rekt.news/abra-rekt/) via rounding error

**Enterprise**

- Karen Scarbrough is the new [interim Executive Director of Enterprise Ethereum Alliance](https://twitter.com/thekscar/status/1751999184910049551)

* * *

### Job Listings

- MetaMask Staking: [Staff Software Engineer](https://consensys.io/open-roles/5444306) and [Software Engineer](https://consensys.io/open-roles/5577174)

- Sourcify seek a [TypeScript Developer](https://jobs.lever.co/ethereumfoundation/fbcb2cf8-cd58-4140-ab3a-47a402616d50)

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

- EF seek an [Executive Assistant](https://jobs.lever.co/ethereumfoundation/444bc50a-236e-4a4e-8385-c0454b0044e9) to support senior decision makers

- Nethermind: [Distributed System Engineer](https://grnh.se/893258d2teu), [Lead Engineer](https://grnh.se/e2d52f72teu), [Protocol Researcher](https://grnh.se/53b888b2teu)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 6.4 to 152.8 gwei, with 19.7 gwei average
    - Zero net issuance currently at 22.0 gwei 
    
    - 1.8k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,243 - $2,380, currently $2,307

- [ETHBTC](https://ratiogang.com/): currently 0.053 (Flippening at ~0.16)

**Notable at app layer**

- ENS [gasless DNSSEC](https://blog.ens.domains/post/gasless-dnssec) live, configure DNS names that support DNSSEC to work with ENS

- [Chipped](https://twitter.com/winnyeth/status/1753431562022945005): NFC press-on nails, create offchain friends list using Disco secured by your private key, pre-order

- Superstate [short duration US government securities fund](https://superstate.co/blog/introducing-superstate-short-duration-us-government-securities-fund-ustb) (USTB), US qualified purchasers only

- [Horswap](https://1.horswap.eth.limo/): Uniswap frontend without censorship or interface fees

**Regulation/business/tokens**

- Proposal for [combating illicit finance in DeFi](https://twitter.com/rebeccarettig1/status/1751967709359665569)

- US SEC Commissioner Peirce [gag rule dissent](https://www.sec.gov/news/statement/peirce-nand-013024)

- [US DoJ](https://www.justice.gov/opa/pr/three-individuals-charged-roles-189b-cryptocurrency-fraud-scheme) & [SEC](https://www.sec.gov/news/press-release/2024-11) charges for HyperFund $1.9B fraud scheme

**General**

- Vitalik: [crypto + AI](https://vitalik.eth.limo/general/2024/01/30/cryptoai.html) and [turning 30](https://vitalik.eth.limo/general/2024/01/31/end.html)

- [ETH recovered from Ledger Nano S](https://www.reddit.com/r/ledgerwallet/comments/1af8ei9/nano_s_with_firmware_12_539_eth_recovered/) (Firmware v1.2) with no seed phrase

- Cloudflare [November security incident](https://blog.cloudflare.com/thanksgiving-2023-security-incident), via a token & credentials from Okta compromise that hadn’t been rotated

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links.  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-february-3-2024](https://weekinethereumnews.com/week-in-ethereum-news-february-3-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Feb 7 – [Holešky testnet](https://eips.ethereum.org/EIPS/eip-7569#activation) Dencun upgrade [epoch 29696](https://holesky.beaconcha.in/epoch/29696)

- Feb 23-Mar 3 – [ETHDenver](https://www.ethdenver.com/) BUIDLWeek & hackathon

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024) hackathon

- Mar 19-21 – [ETH Canal](http://ethcanal.xyz) (Panama City, Panamá) conference & hackathon

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- **Mar 22-24 –** [**ETHSamba**](https://ethsamba.org/) **(Rio)**

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) conference & hackathon

- Mar 29-31 – [ETH Seoul](https://www.ethseoul.org/) hackathon

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) virtual hackathon

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Apr 12-14 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/) hackathon

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- Jun 3-5 – [ETH Belgrade](https://ethbelgrade.rs/) conference

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 26-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

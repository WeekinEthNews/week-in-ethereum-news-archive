---
title: "Week in Ethereum News <br> January 20, 2024"
date: "2024-01-19"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=FhMBatolkOM&t=67s). Recap by [Tim Beiko](https://mirror.xyz/abcoathup.eth/VSzilRKCWz88j5a7z5Jl2aBr5dQ2J0UhavXMxa6drEU).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1748064586023239900) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-179/):
    - **Goerli testnet:** [successfully upgraded to Dencun](https://notes.ethereum.org/@ethpandaops/goerli-dencun-analysis), Prysm bug [patched](https://twitter.com/terencechain/status/1747528980725719156), blob spamming started & blob expiry can be tested from Feb 5 
    
    - **Testnet upgrade dates unchanged**: Sepolia Jan 30 & Holešky Feb 7
    
    - **Mainnet upgrade**: Tim Beiko expects minimum 1 month after Holešky upgrade
    
    - **Pectra (Prague + Electra)**:
        - Small fork late 2024; Verkle likely in following upgrade (Osaka)
        
        - Candidates for inclusion: EIP2537 (BLS precompile), EIP6110 (validator deposits onchain) & EIP7002 (EL triggerable exits)
        
        - Diagram of all [proposed EIPs](https://ethereum-magicians.org/t/prague-electra-network-upgrade-meta-thread/16809/45) & viz of [where each EIP fits in roadmap](https://twitter.com/jimmyragosa/status/1747628330604523568)
        
        - Presentations on [batch txs for EOAs](https://docs.google.com/presentation/d/1XPrY8fwhhQlVKfzkpz65Npa4GCvSgpnJYybSgYNDALE) (EIP3074), [SETCODE](https://docs.google.com/presentation/d/1fUsgZmfTwH59rr8Ca7MK2xSaDLgkHXhjBQk-AnP31_g/edit#slide=id.p), EIP7251 (increase max effective balance) & EIP7547 (inclusion lists)
    
    - next ACDE to discuss potential big feature: Verkle, EOF & EIP4444 (bound historical data)

- [Ephemery testnet](https://twitter.com/TMIYChao/status/1748071205171564729) successfully upgraded to Dencun

- Consensus-specs [v1.4.0-beta.6](https://github.com/ethereum/consensus-specs/releases/tag/v1.4.0-beta.6): fork choice filter change

**Verkle**

- Verkle implementers call [video](https://www.youtube.com/watch?v=r7CA6L6yOWI&t=42s) & [notes](https://twitter.com/rudolf6_/status/1747671196144112074): all client teams working on Verkle, testnet to be relaunched and challenges with BLOCKHASH opcode

- [Verkle proofs & stateless clients](https://ihagopian.com/posts/anatomy-of-a-verkle-proof) explainer

**Client releases**

- Consensus layer:
    - Lodestar [v1.14.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.14.0): option for local block publishing signed by the validator
    
    - Prysm [v4.2.1-rc.0](https://github.com/prysmaticlabs/prysm/releases/tag/v4.2.1-rc.0): fix historical roots for Goerli Dencun upgrade

- Execution layer:
    - Erigon [v2.57.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.57.0): Sepolia & Holešky testnets Dencun upgrade
    
    - Nethermind [v1.25.1](https://github.com/NethermindEth/nethermind/releases/tag/1.25.1): fix eth\_syncing behavior and extra bodies & receipts downloaded after upgrading long-living node
    
    - Reth [v0.1.0-alpha.15](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.15): consensus fix for Dencun and enables default on-disk blob store

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 32.10%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth 84% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm 40%, any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Pari: [testing path to raise gas limit](https://ethresear.ch/t/testing-path-for-a-gas-limit-increase/18399), local then shadowforks to ensure within burst (worst case) & long term constraints

- Potuz: [heuristics for detecting censorship](https://hackmd.io/@potuz/BkpzmOgK6) so execution layer clients can signal for local building

**For stakers**

- [Besu](https://wiki.hyperledger.org/display/BESU/2024+-+Besu+Performance+Improvements+since+the+Merge) (execution layer client) performance improvements (95% of blocks processed within ~250ms) and optimal config

**MEV**

- Flashbots [order flow visualization](https://writings.flashbots.net/illuminate-the-order-flow) using Sankey diagrams

**Layer 2**

- [Arbitrum Orbit permissionless L2 & L3 creation](https://forum.arbitrum.foundation/t/the-arbitrum-expansion-program-and-developer-guild/20722), requires revenue sharing

- [Public Goods Network](https://gov.gitcoin.co/t/announcing-the-spin-down-of-pgn-eol-june-2024/17430) (PGN) shutting down in June

**EIPs/Standards**

- EIPs
    - Meta [EIP7600](https://github.com/ethereum/EIPs/pull/8121/files): Hardfork Meta - Pectra (Prague + Electra)

- ERCs (application layer):
    - [ERC7595](https://github.com/ethereum/ERCs/pull/202/files): Collateralized NFT (ERC721 extension)
    
    - [ERC7596](https://github.com/ethereum/ERCs/pull/205/files): Equity shares book-entry system
    
    - [ERC7597](https://github.com/ethereum/ERCs/pull/206/files): Signature validation extension for Permit (ERC2612)
    
    - [ERC7598](https://github.com/ethereum/ERCs/pull/207/files): Use contract signature for signed transfer
    
    - [ERC7599](https://github.com/ethereum/ERCs/pull/210/files): Onchain autonomous AI agent NFT

**Stuff for developers**

- Foundry:
    - Forge-std [v1.7.6](https://github.com/foundry-rs/forge-std/releases/tag/v1.7.6): new cheat codes dumpState (write state to disk in JSON), signP256 (generate secp256r1 signatures) and toBase64 & toBase64URL

- Remix challenge: [4 questions on zk proofs with Circom](https://hackmd.io/fVMlqo3zQz6-Va0qZt-2pQ), mint NFT on Optimism

- [GasliteToken](https://github.com/PopPunkLLC/gaslite-core/blob/main/src/GasliteToken.sol) (ERC20 base smart contract): gas optimized ERC20 with fees 

- [Contract obfuscation](https://degatchi.com/articles/mev-smart-contract-obfuscation) to avoid generalized front running

- [The Rippler](https://github.com/jtriley-eth/the-rippler): fast multicaller, reverse packed encoding 

- [Vyper Jupyter plugin](https://medium.com/@daniel.schiavini/connecting-vyper-to-your-wallet-in-jupyter-colab-d23581cd9655) to deploy from Jupyter notebooks & Google Colab using titanoboa

- Curta CTF [ZSafe solution](https://philogy.github.io/posts/curta-zsafe-writeup)

- [ABI parsers vulnerable to zero-sized types](https://github.com/paulmillr/micro-eth-signer/discussions/20) (ZSTs) DoS attack

**Security**

- Socket/Bungee [$3.3M exploit](https://sockettech.notion.site/Socket-Incident-Report-16-Jan-9aba3bbf08814fc49e4f2ffb58284912) on mainnet, token approvals drained via unverified user input

**Enterprise**

- Enterprise Ethereum Alliance: [DeFi risk assessment guidelines](https://entethalliance.org/the-eeas-drama-wg-has-released-a-review-draft-of-its-defi-risk-guidelines-discussion-paper-for-public-feedback/), feedback by April 15

- [GameStop NFT marketplace](https://nft.gamestop.com/) shutting February 2, due to regulatory uncertainty

* * *

### Job Listings

- Nethermind: [Distributed System Engineer](https://grnh.se/893258d2teu), [Lead Engineer](https://grnh.se/e2d52f72teu), [Protocol Researcher](https://grnh.se/53b888b2teu)

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

- Status is hiring: Technical Chief Operating Officer - [Apply here](https://grnh.se/0ecdaa981us)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 11.3 to 74.6 gwei, with 28.7 gwei average
    - Zero net issuance currently at 22.0 gwei 
    
    - 6.9k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,419 - $2,605, currently $2,485

- [ETHBTC](https://ratiogang.com/): currently 0.06 (Flippening at ~0.16)

**Notable at app layer**

- Sablier [monthly unlocks](https://twitter.com/sablier/status/1745219417703850100) streaming curve, can use like traditional payroll

- [Dagon](https://twitter.com/z0r0zzz/status/1747496774342955459) (DAO singleton) live on mainnet & Optimism, add weighted token voting to any account

- [Zuzalu QF grants](https://www.gitcoin.co/blog/zuzalu-qf-grants-program-on-grants-stack): spinoff events (Zu-villages) & digital public goods rounds

**Regulation/business/tokens**

- US IRS: [$10k+ crypto transaction reporting not currently enforced](https://twitter.com/jerrybrito/status/1747383019592188153)

- [EU provisional agreement on AML](https://www.consilium.europa.eu/en/press/press-releases/2024/01/18/anti-money-laundering-council-and-parliament-strike-deal-on-stricter-rules/), customer due diligence required for €1k+ crypto transactions

**General**

- [$32M in rugpulls](https://blockfence.io/security/32m-stolen-over-1300-fake-tokens-rugged/) from 1,300 automatically created meme tokens

- [Dark DAO lite demo](https://initc3org.medium.com/daos-must-confront-dark-daos-or-fall-under-their-shadow-b4c47cb6a1be) for vote buying

- Trail of Bits: [LeftoverLocals](https://blog.trailofbits.com/2024/01/16/leftoverlocals-listening-to-llm-responses-through-leaked-gpu-local-memory/), recovery of data from GPU local memory 

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-january-20-2024](https://weekinethereumnews.com/week-in-ethereum-news-january-20-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- **Jan 22 – EF’s** [**Next Billion fellowship cohort 4**](https://fellowship.ethereum.foundation/) **deadline extended**

- Jan 30 – [Sepolia testnet](https://eips.ethereum.org/EIPS/eip-7569#activation) Dencun upgrade epoch 132608 (assuming no issues)

- Feb 2-4 – [ETH Cinco de Mayo](https://ethcincodemayo.com/) hackathon (Cholula, Puebla)

- Feb 3 – [Ethereum Lima Day](https://ethlimaday.org/)

- Feb 7 – [Holešky testnet](https://eips.ethereum.org/EIPS/eip-7569#activation) Dencun upgrade epoch 29696 (assuming no issues)

- Feb 23-Mar 3 – [ETHDenver](https://www.ethdenver.com/) BUIDLWeek & hackathon

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024) hackathon

- Mar 19-21 – [ETH Canal](http://ethcanal.xyz) (Panama City, Panamá) conference & hackathon

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) hackathon & conference 

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

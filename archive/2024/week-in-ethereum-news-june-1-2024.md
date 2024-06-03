---
title: "Week in Ethereum News <br> June 1, 2024"
date: "2024-06-01"
---

## Eth News and Links

PeerDAS included in Pectra upgrade but with separate activation epoch, proposal to extend ENS to Layer 2 & Biden vetos congressional disapproval of SEC SAB 121

**All core devs**

- [All core devs – consensus (ACDC) #134](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-call-134/20174).  Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-134/):
    - **Pectra (Prague + Electra) upgrade**:
        - **Discussion on when/what to ship**:
            - Options included splitting Pectra ([Lodestar proposal](https://blog.chainsafe.io/lodestar-pectra-roadmap-vision/)) or replacing EIPs with PeerDAS
            
            - **EIP7594 PeerDAS:** included in Pectra but with separate activation epoch to allow moving to a later upgrade if needed
            
            - **Blob size increase**: no decision ([blob target of 3 reached](https://x.com/hildobby_/status/1795931542780522885) this week) 
            
            - **EIP7688 change SSZ data to StableContainer**: no decision, discuss at next ACDC, need more implementation progress

- Tim Beiko: [process improvement proposals](https://ethereum-magicians.org/t/allcoredevs-network-upgrade-ethmagicians-process-improvements/20157) for All Core Devs, network upgrades & Eth Magicians, discuss at next ACDE

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- [Future of EOA/AA breakout #3](https://ethereum-magicians.org/t/future-of-eoa-aa-breakout-room-3/20164): EIP7702 [refinements](https://github.com/ethereum/EIPs/pull/8561) to be merged, [next breakout](https://github.com/ethereum/pm/issues/1054) June 5 to discuss potential changes, ERC-standardized proxy contract & wallet best practices

[**Osaka + F starname**](https://eips.ethereum.org/EIPS/eip-7607) **upgrade**

- [Verkle progress](https://x.com/rudolf6_/status/1796098587366998449), best case ~2025

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido increased to 29%**](https://dune.com/hildobby/eth2-staking)**, too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~55% majority 
    
    - Consensus layer: **Prysm 38%**
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Péter Szilágyi: [full node space requirements](https://x.com/peter_szilagyi/status/1795012642857271306), 800GB for blocks & receipts + 250GB for active state & Geth snapshots

- Proposed [issuance reduction FAQ](https://ethresear.ch/t/faq-ethereum-issuance-reduction/19675)

- [Blob impact on reorgs](https://ethresear.ch/t/big-blocks-blobs-and-reorgs/19674), increasing by 2.3 blobs increases reorg probability to 0.59%

- [Gossipsup performance](https://ethresear.ch/t/gossip-iwant-ihave-effectiveness-in-ethereums-gossipsusb-network/19686) in P2P, average effectiveness ratio is more than 1:10 across topics

- Terence: [delayed execution](https://ethresear.ch/t/advantage-of-pipelining-consensus-and-execution-delayed-execution/19668), benefit of pipelining consensus & execution in ePBS

**Client Releases**

- Execution layer:
    - Besu [v24.5.2](https://github.com/hyperledger/besu/releases/tag/24.5.2): default Bonsai storage mode to use code storage by code hash & use flat db and new RPC methods to get/set vanity extra data in a built block

**For Stakers**

- Obol [staking mastery program](https://obol-dvt.notion.site/Obol-Staking-Mastery-Program-03bcde8a01324262a2e2ccb429ae1bde) to develop educational leaders

**Layer 2**

- [Base gas target increased](https://x.com/jessepollak/status/1796296848178864519) to 7.5 Mgas/s

- OP Stack [custom gas token](https://x.com/oplabspbc/status/1795933890617438601), beta

- [Taiko](https://taiko.mirror.xyz/Pizjv30FvjsZUwEG-Da7Gs6F8qeDLc4CKKEBqy3pTt8) live, plans to become optimistic-zk hybrid based rollup

- L2BEAT: [Layer 3 projects TVL](https://l2beat.com/scaling/summary#layer3s)

- Ed Felten: [selling MEV separately can give more revenue](https://research.arbitrum.io/t/do-shared-mev-auctions-actually-increase-revenue/9606) than shared MEV auctions

- Vitalik: [Layer 2s as cultural extensions of Ethereum](https://vitalik.eth.limo/general/2024/05/29/l2culture.html)

**EIPs/Standards**

- EIPs:
    - [EIP7716](https://github.com/ethereum/EIPs/pull/8598/files): Anti-correlation attestation penalties

- ERCs (application layer):
    - [ERC7717](https://github.com/ethereum/ERCs/pull/453/files): Deterministic AA wallet

**Stuff for developers**

- [Compiler fingerprinting](https://jbecker.dev/research/evm-compiler-fingerprinting) using bytecode-specific heuristics 

- Runtime Verification [Simbolik](https://github.com/runtimeverification/simbolik-vscode#readme): Solidity debugger VS Code extension, private beta

- 0xngmi [Etherscan verification](https://etherscan-verification.0xngmi.com/): verify an already verified contract on another chain

- RareSkills: [guide to ABI encoding for function calls](https://www.rareskills.io/post/abi-encoding)

- Ape [v0.8.0](https://github.com/ApeWorX/ape/releases/tag/v0.8.0) (Python contract framework): major refactor

- [Tevm](https://github.com/evmts/tevm-monorepo#readme) (TypeScript EVM toolkit): in browser devnet & Solidity scripting

- [TracEVM](https://github.com/ioterw/tracevm#readme): track values & addresses of slots in a contract

- [R55](https://hackmd.io/@leoalt/r55): Rust contract compiled to RISCV bytecode run inside an execution client

- CTFs:
    - OpenZeppelin Ethernaut new level: [Stake](https://ethernaut.openzeppelin.com/level/31)

- Red Guild: [devcontainers](https://blog.theredguild.org/where-do-you-run-your-code/), preconfigured dev sandbox in a Docker container

**Security**

- Normie token [exploit](https://x.com/ProfoundWatcher/status/1794629010531693005) on Base, via transfer function check for balance matching team wallet

**Ecosystem**

- [ETHBerlin](https://projects.ethberlin.org/submissions/results) hackathon winners

- Devcon [supporter program](https://blog.ethereum.org/2024/05/29/devcon7-supporters-impact) to assist impact teams with free tickets

* * *

### Job Listings

- [Alchemy](https://www.alchemy.com/careers) - Wallet Services: [Engineering Manager](https://grnh.se/cc56a4365us) and [Full-Stack Engineer](https://grnh.se/5a40c3b55us)

- ChainSafe: [Head of Protocol Engineering](https://grnh.se/c6e27e794us), [DevRel](https://grnh.se/6627a6284us) - Sygma and [more jobs](https://grnh.se/108a0afd4us)

- Privacy and Scaling Explorations: [ZK Circuits Engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 2.1 to 75.6 gwei, with 10.4 gwei average
    - Zero net issuance currently at 23.3 gwei 
    
    - 9k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,712 - $3,959, currently $3,758

- [ETHBTC](https://ratiogang.com/): currently 0.056 (Flippening at ~0.16)

**Notable at app layer**

- ENS Labs [ENSv2 proposal](https://discuss.ens.domains/t/ens-labs-development-proposal-ensv2-and-native-l2-support/19232) to extend to Layer 2 (either select an L2 or create their own)

- [Uniswap Foundation](https://x.com/UniswapFND/status/1796590521072119927) postpone fee reward vote

- [MEV scanner](https://x.com/mevscanner/status/1796181821715087775): reports amount of MEV for an address via website, X/Telegram/Discord bot

**Regulation/business/tokens**

- Biden [vetos congressional disapproval of SEC Staff Accounting Bulletin 121](https://www.whitehouse.gov/briefing-room/presidential-actions/2024/05/31/a-message-to-the-house-of-representatives-on-the-presidents-veto-of-h-j-res-109/) that precluded banks offering crypto custody
    - Democrats [still doing anti crypto actions](https://x.com/SGJohnsson/status/1796216669100036525), despite recent [campaign outreach](https://www.theblock.co/post/297504/biden-campaign-shifts-crypto-stance-engages-crypto-industry-presidential-elections-2024) 

- SEC [ordered to pay $1.8M in legal expenses](https://www.ibtimes.com/judge-orders-sec-pay-18-million-dismisses-bad-faith-debt-box-case-3733101) for “bad faith” crypto lawsuit

- US Treasury [NFT risk assessment](https://home.treasury.gov/news/press-releases/jy2382), rarely used for terrorist financing, susceptible to use in fraud/scams & being stolen

- SEC Commissioner Peirce [proposes opening UK sandbox to US](https://www.sec.gov/news/statement/peirce-boe-fca-comment-05292024)

- Former FTX executive [Ryan Salame sentenced](https://www.justice.gov/usao-sdny/pr/former-ftx-executive-ryan-salame-sentenced-90-months-prison) to 7.5 years

- [Matter Labs](https://x.com/the_matter_labs/status/1796581973277700296) (zkSync) applied for ZK trademark

**General**

- Vitalik: [Bitcoin block size war reflections](https://vitalik.eth.limo/general/2024/05/31/blocksize.html), embrace new tech or stagnate

- [SPDZ](https://leku.blog/spdz/): colab notebook for generic MPC scheme split into preprocessing & online phases

- [Length Extension Attacks](https://tiagofneto.com/posts/length-extension/): hash functions using Merkle–Damgård construction are vulnerable

- [Ticketmaster data breach](https://www.bleepingcomputer.com/news/security/live-nation-finally-confirms-massive-ticketmaster-data-breach/) via third-party cloud database provider

- Reminder: [Week in Ethereum News (ES)](https://weekinethereumnewses.substack.com/): Spanish translation of the newsletter

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-june-1-2024](https://weekinethereumnews.com/week-in-ethereum-news-june-1-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jun 14 – [EF EIP4844 data challenge](https://esp.ethereum.foundation/data-challenge-4844) deadline

- Jun 21-23 – [ETHKyiv](https://ethkyiv.org/) hackathon & conference

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 29-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 2-4 – [Ethereum Argentina](https://ethereumargentina.org/) conference & hackathon

- Aug 15-17 – [Ethereum Uruguay](https://twitter.com/EthereumUruguay/status/1786144213328879817) hackathon & conference

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 23-26 – [ETHTokyo](https://www.ethtokyo.com/) hackathon & conference

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- Sep 5-8 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 9-15 – [ETHSafari](https://ethsafari.xyz/) (Kenya)

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- **Sep 13-14 –** [**Ethereum México**](https://x.com/ethereum_mexico/status/1792677234324767081)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Sep 26-27 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 4-6 – [Ethereum Kuala Lumpur](https://www.2024.ethkl.org/) conference & hackathon

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

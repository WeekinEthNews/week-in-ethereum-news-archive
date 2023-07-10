---
title: "Week in Ethereum News <br> July 8, 2023"
date: "2023-07-07"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=Voavkk8Es5E&t=78s). Notes from [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-execution-call-165/):
    - [Impact of EIP6404/6466 SSZ transition](https://docs.google.com/document/d/1p-1VvOGwI5GHkwaGMzJYDL7Affofm6rVLa6cvnmoqGI/edit) on existing contracts using RLP: EIP6404 is low impact whilst EIP6466 is manageable due to upgradeability of 3 impacted projects \[Reminder: SSZ EIPs already removed from Dencun upgrade\]
    
    - Dencun updates: [devnet issue tracker](https://notes.ethereum.org/@parithosh/dencun-issue-tracker), plan to stress test EIP4844 on devnet 7 & in parallel develop full set of Dencun EIPs for devnet 8
    
    - Discussion on Engine API flag for EL to suggest CL use local block building

- EIP4844:
    - [Last chance to contribute to KZG ceremony](https://ceremony.ethereum.org/), closes July 23, use an account with at least 8 transactions

**Client releases**

- Consensus layer:
    - Lighthouse [v4.3.0](https://github.com/sigp/lighthouse/releases/tag/v4.3.0): bandwidth reductions and slasher breaking changes: broadcasting enabled by default & backend reverted to LMDB

- Execution layer:
    - Reth [v0.1.0-alpha.2](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.2): Engine API stability improved, fixes for out of memory issues, RPC corner cases fixed including for tracing and added new metrics

**For Stakers**

- [MEV-Boost dashboard](https://twitter.com/nero_eth/status/1675777429904797696) adds charts for optimistic relaying, shows increased win ratio

**Research**

- Enshrined PBS proposal: [payload-timeliness committee](https://ethresear.ch/t/payload-timeliness-committee-ptc-an-epbs-design/16054) (PTC), subset of attestation committee votes on whether builder released their execution payload on time

- [Transaction fee mechanism design](https://twitter.com/tim_roughgarden/status/1676980165316886530), a proof that MEV makes it impossible for UX to be simple and for validators to be incentivized towards proper behavior 

- [Distributed block building](https://collective.flashbots.net/t/distributed-blockbuilding-networks-via-secure-knapsack-auctions/1955): privacy preserving knapsack auctions using MPC

**Layer 2**

- Patrick McCorry: [overview of bridges](https://www.cryptofrens.info/p/bridging-databases-part-2)

**EIPs/Standards**

- EIPs:
    - [EIP7266](https://github.com/ethereum/EIPs/pull/7266/files): Remove blake2f (0x09) precompile

- ERCs (application layer):
    - [ERC7265](https://github.com/ethereum/EIPs/pull/7265/files): Circuit breaker
    
    - [ERC7272](https://github.com/ethereum/EIPs/pull/7272/files): Ethereum access token (authorize function calls from offchain service)
    
    - [ERC7280](https://github.com/ethereum/EIPs/pull/7280/files): NFT metadata extension like JSON-LD
    
    - [ERC7281](https://github.com/ethereum/EIPs/pull/7281/files): Sovereign bridged token (xERC20)
    
    - [ERC7291](https://github.com/ethereum/EIPs/pull/7292/files): Purpose bound money (ERC1155 extension)

**Stuff for developers**

- [Compare GitHub contracts against Etherscan verified code](https://blog.theredguild.org/how-to-diff-smart-contracts-etherscan/) using Diffyscan

- [Scaffold-ETH 2](https://github.com/scaffold-eth/scaffold-eth-2#readme) updated to wagmi v1 & viem

- [Svelte Wagmi](https://github.com/softwarecurator/svelte-wagmi#readme): Svelte stores & functions using wagmi for connecting & signing

- [Vitest-solidity-coverage](https://twitter.com/wighawag/status/1675803846147178497): Hardhat plugin for solidity-coverage with Vitest

- Ape [v0.6.12](https://github.com/ApeWorX/ape/releases/tag/v0.6.12) (contract dev framework): adds [EIP5202 blueprint support](https://twitter.com/fubuloubu/status/1677436142679994369), coverage and install & compile dependencies

- Huff [style guide](https://github.com/jtriley-eth/huff-style-guide#readme)

- RareSkills: [overview of contract security tools](https://www.rareskills.io/post/smart-contract-audit-tools)

- CTFs:
    - Curta CTF: [Ping Pong](https://www.curta.wtf/puzzle/13)
    
    - Secureum RACE #19: [8 question Solidity quiz & answers](https://ventral.digital/posts/2023/7/3/race-19-of-the-secureum-bootcamp-epoch-infinity)

- Guide to [create custom Uniswap v4 hooks](https://soliditydeveloper.com/uniswap4)

- [Reth-indexer](https://github.com/joshstevens19/reth-indexer#readme): reads from Reth (EL client) database, indexes into Postgres & generates API

- [Circomkit](https://github.com/erhant/circomkit#readme): simple interface & testing utilities to develop Circom circuits

**Security**

- Azuki DAO (disgruntled Azuki holders) [35 ETH exploit](https://twitter.com/MetaSleuth/status/1675783739174166528) via missing check for signature replay

- Tincho: [question driven approach](https://blog.theredguild.org/question-until-it-crashes/) to review code

**Ecosystem**

- [Etherscan adds ENS](https://twitter.com/etherscan/status/1675856302013284352) to search bar auto-lookup

**Notable at app layer**

- [Zora network](https://twitter.com/ourzora/status/1677346773281669121) (OP Stack L2) supported by OpenSea

- [SUBMINT](https://submint.io/) (ENS subname minting) live on mainnet, set pricing & token gate minting

- Gas guzzler of the week: VMPX ERC20 token [required proof of work to mint](https://twitter.com/0xCygaar/status/1676699126682075136)

* * *

### Job Listings

- Solidity team need a highly skilled [Developer Advocate](https://jobs.lever.co/ethereumfoundation/b9e33c9e-48ee-464f-a672-d51eece2b99d)

- Devconnect Istanbul: [Production Assistant](https://jobs.lever.co/ethereumfoundation/db6e2775-39d3-4eb9-9313-dfb15dfab9bc) and [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/401e0af5-f4a2-4e66-a724-4accb003113e)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Gemini sues DCG](https://twitter.com/cameron/status/1677327395869581316), alleging Barry Silbert fraud

- [Kraken ordered to hand over account info to IRS](https://www.coindesk.com/policy/2023/06/30/court-orders-kraken-to-turn-over-history-transaction-and-account-information-to-irs) for users who transacted over $20k in a year

- [CFTC Digital Asset Markets subcommittee](https://www.cftc.gov/PressRoom/PressReleases/8740-23) include BlackRock, BNY Mellon, Goldman Sachs, HSBC, JPMorgan, Moody's, Nasdaq, Polygon, Societe Generale and Uniswap

**General**

- Multichain (Anyswap) bridge [$126 million exploit](https://twitter.com/peckshieldalert/status/1677124413274353664), revoke contract approvals

- Poly Network bridge [$4 million exploit](https://rekt.news/poly-network-rekt2/), apparent misuse of 3 out of 4 private keys

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-8-2023](https://weekinethereumnews.com/week-in-ethereum-news-july-8-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jul 17 – [CLRFund round 9](https://blog.clr.fund/round-9-is-underway/) ends

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 20–23 – [Pragma Paris](https://ethglobal.com/events/pragma-paris) & [ETHGlobal Paris](https://ethglobal.com/events/paris2023) hackathon

- **Jul 23 –** [**KZG Ceremony**](https://ceremony.ethereum.org/) **closes**

- Aug 11-13 – [ETHMunich](https://ethmunich.de/) hackathon

- Aug 15-16 – [ETHToronto](https://www.ethtoronto.ca/) & [ETHWomen](https://www.ethwomen.com/)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org/) (Buenos Aires)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 31 - Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 15-17 – [ETHChicago](https://www.ethchicago.xyz/) conference & hackathon

- Sep 18-21 – [ETH Montréal](https://ethmontreal.xyz/) conference & hackathon

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 6-27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 13-15 – [Ethereum Kuala Lumpur](https://hack.ethkl.org/) conference & hackathon

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) application deadline

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://twitter.com/ethbrno/status/1652198745902137344)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 17-19 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

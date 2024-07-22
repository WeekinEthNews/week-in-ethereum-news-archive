---
title: "Week in Ethereum News <br> July 20, 2024"
date: "2024-07-20"
---

## Eth News and Links

EOF remains in Pectra for now, Virgil Griffith sentence reduced, spot ETH ETFs launch July 23 in US and WazirX (Indian exchange) $230M exploit

**All core devs**

- [All Core Devs - Execution (ACDE) #192](https://ethereum-magicians.org/t/all-core-devs-execution-acde-call-192-july-18-2024/20565):
    - **Pectra (Prague + Electra) upgrade:**
        - **Pectra-devnet-1**: local testing found some issues, plan to launch Thursday with all clients
        
        - **EOF**:
            - Remains in Pectra for now, requires extensive testing & fuzzing across clients
            
            - Risks of a consensus bug & costs vs benefits debated; Geth strongly against & won’t champion testing/support, Solidity for
            
            - Legacy EVM still needs to be supported, migration is years away, if ever
            
            - Mainnet still sets defaults for L2s, L2s won’t lead yet
        
        - **EIP7702**: spec unchanged for now, discussed CODERESET proposal
        
        - **Logs for system contracts**: review async & decide at next ACDC
        
        - **EIP7742 decouple blob count for CL/EL**: discuss at next ACDC
        
        - [**RIP7212**](https://hackmd.io/@ulerdogan/B1QikMxdC) **secp256r1 precompile on L1**: review async & decide on inclusion (soon)

[**Osaka + F starname**](https://eips.ethereum.org/EIPS/eip-7607) **upgrade**

- [Verkle implementers call #21](https://ethereum-magicians.org/t/verkle-implementers-call-21-july-15-2024/20566): proposal to reduce witness size, updates to EIP6800 & EIP2935 and cost of code chunking

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 29.15%**](https://dune.com/hildobby/eth2-staking)**, still too close to 33.3% threshold**

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~55% majority 
    
    - Consensus layer: **Prysm 35%**
    
    - Any client bug over 33.3% could mean loss of finality
    
    - **Potuz:** [**stress of potential consensus bugs**](https://x.com/potuz_eth/status/1814263448638828899) **on majority client developers**

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Layer 1**

- Blocknative: [data viz of self-built blocks](https://www.blocknative.com/blog/how-self-built-blocks-unintentionally-introduce-base-fee-volatility), unintentionally increase base fee volatility

- EIP7732 ePBS:
    - [ePBS breakout #5](https://ethereum-magicians.org/t/epbs-breakout-5-july-19-2024/20591): short call, proposer IP leaks requesting headers from builder and consensus spec tests fixes in progress

- Nethermind [EVMYulLean](https://github.com/NethermindEth/EVMYulLean#readme): EVM + Yul specification, executable, in Lean

**Research**

- Anders Elowsson: [sealed execution auction](https://ethresear.ch/t/sealed-execution-auction/20060), Vickrey slot auction of execution proposal rights, attesters supervise commit/reveal scheme facilitated by builders & beacon proposer

- [Multi-round MEV-Boost](https://ethresear.ch/t/based-preconfirmations-with-multi-round-mev-boost/20091): mitigate negatives of based preconfs & retain benefits of based rollups

**Client Releases**

- Consensus layer:
    - Lodestar [v1.20.2](https://github.com/ChainSafe/lodestar/releases/tag/v1.20.2): patch for publishing blinded blocks using Lodestar beacon node & Lighthouse/Nimbus validator client with MEV-Boost

- Execution layer:
    - Reth [v1.0.3](https://github.com/paradigmxyz/reth/releases/tag/v1.0.3): fix for Base mainnet & async Backfill stream

**Layer 2**

- [Scroll](https://x.com/Scroll_ZKP/status/1814275555681771784) delayed finalization to investigate potential ecosystem incident, confirmed [Rho Markets](https://rekt.news/rho-market-rekt/) was application specific

- L2BEAT [Badges](https://x.com/l2beat/status/1813173391639101587): visual display of L2 features

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7745](https://github.com/ethereum/EIPs/pull/8740/files): Two dimensional log filter data structure

- ERCs (application layer standards):
    - [ERC7743](https://github.com/ethereum/ERCs/pull/539/files): Multi-owner non-fungible tokens (MO-NFT)
    
    - [ERC7744](https://github.com/ethereum/ERCs/pull/542/files): Code index (index contract bytecode)
    
    - [ERC7746](https://github.com/ethereum/ERCs/pull/543/files): Composable security middleware hooks

- [EIP.tools](https://eip.tools/) adds RIPs (rollup improvement proposals)

**Stuff for developers**

- Solidity [via-IR compilation pipeline](https://soliditylang.org/blog/2024/07/12/a-closer-look-at-via-ir/) explainer: translates Solidity into Yul (intermediate representation) for optimization rather than direct to bytecode, plan to make default with EOF

- [Solidity hidden overflow](https://x.com/sigp_io/status/1813773082789855554): math expression types cast to highest type used by variables

- Solady (Solidity snippets): adds [ERC1967 minimal proxies with immutable args](https://warpcast.com/optimizoor/0x0802be66), auto verified on Etherscan

- Z0r0z [sstore3](https://github.com/z0r0z/sstore3#readme), read/write contract storage using balance & address, license: AGPL v3

- [Rindexer](https://github.com/joshstevens19/rindexer#readme), EVM indexing tool in Rust, beta

- [Reth Execution Extension](https://github.com/paradigmxyz/reth-exex-examples#readme) (ExEx) examples

- Echidna [v2.2.4](https://github.com/crytic/echidna/releases/tag/v2.2.4): improves fuzzing speed & user experience, adds support for transient opcodes

- [Audit Wizard](https://www.auditwizard.io/blog/announcing-a-new-code-scanning-tool-in-audit-wizard-cyfrin-aderyn) adds Cyfrin Aderyn (Solidity static analyzer)

- [Spice](https://github.com/paradigmxyz/spice/#readme) (Python): export data from Dune API

- CTFs:
    - Damn Vulnerable DeFi [v4](https://www.damnvulnerabledefi.xyz/v4-release/): migrated to Foundry, new challenges: curvy puppet, shards, withdrawal & rewarder

**Security**

- WazirX (Indian exchange) [$230M exploit](https://x.com/WazirXIndia/status/1813981143437611440) via multisig compromise

- LiFi [$11.6M exploit](https://li.fi/knowledge-hub/incident-report-16th-july/) on mainnet & Arbitrum via arbitrary call, after contract facet added, infinite approvals impacted

- Minterest [$1.4M exploit](https://minterest.com/blog/minterest-security-incident-post-mortem-report/) on Mantle L2 via reentrancy

- Security Alliance (SEAL): [incident response to Squarespace domain compromise](https://securityalliance.notion.site/A-Squarespace-Retrospective-or-How-to-Coordinate-an-Industry-Wide-Incident-Response-fead693b66c14543a48283d85aec19ad)  

**Ecosystem**

- [ETHGlobal Brussels](https://twitter.com/ETHGlobal/status/1812498110087938399) finalists

**Enterprise**

- Enterprise Ethereum Alliance [DeFi risk assessment guidelines](https://entethalliance.org/specs/defi-risks/)

* * *

### Job Listings

- [EF Protocol Support](https://jobs.lever.co/ethereumfoundation/60a70892-cea9-461e-9db2-199cb95f7d43): generalist to help with ACD, EPF, SoP & more

- Nethermind: [Senior Device Security Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4336487101), Senior DevOps Engineer [AMER](https://boards.eu.greenhouse.io/nethermind/jobs/4363348101) & [APAC](https://boards.eu.greenhouse.io/nethermind/jobs/4363281101), [Full Stack Lead](https://boards.eu.greenhouse.io/nethermind/jobs/4356246101) APAC, [Post-Grad Internship](https://boards.eu.greenhouse.io/nethermind/jobs/4364252101) & [Chief Marketing Officer](https://boards.eu.greenhouse.io/nethermind/jobs/4363412101)

- EF seek a [European/Civil Law qualified Legal Counsel](https://jobs.lever.co/ethereumfoundation/204e2031-e60b-4c43-835a-e6837cef00b2)

- Aragon: [Senior Smart Contract Developer](https://jobs.lever.co/aragon/fba68080-9e98-49d7-8ed7-ac05d047d4b0)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 0.9 to 41.7 gwei, 6.8 gwei average; zero net issuance at 23.6 gwei 
    
    - 13k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,121 - $3,538, currently $3,488, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.053 (Flippening at ~0.164)

**Regulation/business/tokens**

- [Virgil Griffith sentence reduced](https://x.com/aurbelis/status/1813593386710102378) by 7 months, should be going home soon

- Spot ETH ETFs launch July 23 in US ([CETH](https://www.cboe.com/us/equities/notices/new_listings/details/?etf=true&firm_name=21Shares+US+LLC&first_trade_dt=2024-07-23&ipo=true&symbols=CETH), [FETH](https://www.cboe.com/us/equities/notices/new_listings/details/?etf=true&firm_name=Fidelity&first_trade_dt=2024-07-23&ipo=true&symbols=FETH), [EZET](https://www.cboe.com/us/equities/notices/new_listings/details/?etf=true&firm_name=Franklin+Templeton&first_trade_dt=2024-07-23&ipo=true&symbols=EZET), [QETH](https://www.cboe.com/us/equities/notices/new_listings/details/?etf=true&firm_name=Invesco&first_trade_dt=2024-07-23&ipo=true&symbols=QETH) & [ETHV](https://www.cboe.com/us/equities/notices/new_listings/details/?etf=true&firm_name=VanEck&first_trade_dt=2024-07-23&ipo=true&symbols=ETHV))

**General**

- [Fractal ID](https://app.fractal.id/documents/id/breach-notification.pdf) (KYC) data breach, includes uploaded images/documents

- EF updates mailing list [compromise was via Google Workspace bug](https://x.com/fredriksvantes/status/1813824630412722387)

- [CrowdStrike](https://www.crowdstrike.com/blog/statement-on-falcon-content-update-for-windows-hosts/) update caused Windows hosts to blue screen of death

- [Craig Wright](https://x.com/dr_cswright/status/1813547003676164132) is not Satoshi, as per legal notice he is required to share

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-july-20-2024](https://weekinethereumnews.com/week-in-ethereum-news-july-20-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jul 29-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 2-4 – [Ethereum Argentina](https://ethereumargentina.org/) conference & hackathon

- Aug 7-9 – [Science of Blockchain Conference](https://www.sbc-conference.com/) (New York)

- Aug 15-17 – [Ethereum Uruguay](https://www.ethereumuruguay.org/) hackathon & conference

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 23-26 – [ETHTokyo](https://www.ethtokyo.com/) hackathon & conference

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- Sep 5-8 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 9-15 – [ETHSafari](https://ethsafari.xyz/) (Kenya)

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 13-14 – [Ethereum México](https://ethmexico.org/)

- Sep 20-22 – [ETHCapeTown](https://www.ethcapetown.com/) hackathon

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Sep 26-27 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 4-6 – [Ethereum Kuala Lumpur](https://www.2024.ethkl.org/) conference & hackathon

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

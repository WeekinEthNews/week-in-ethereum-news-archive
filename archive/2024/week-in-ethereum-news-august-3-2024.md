---
title: "Week in Ethereum News <br> August 3, 2024"
date: "2024-08-03"
---

## Eth News and Links

Ethereum ninth anniversary of mainnet launch & Underhanded Solidity contest 

**All core devs**

- [All Core Devs - Execution (ACDE) #193](https://ethereum-magicians.org/t/all-core-devs-execution-acde-193-august-1-2024/20648):
    - **Pectra (Prague + Electra) upgrade:**
        - [**Pectra-devnet-2**](https://pectra-devnet-2.ethpandaops.io/): same spec as devnet-1 (broken by EIP7702 testing), a few client issues found so far, won’t test EIP7702
        
        - **EIP7702:** [latest spec](https://github.com/ethereum/EIPs/pull/8775) will be included in pectra-devnet-3
        
        - **EOF**: working on fuzzing & writing tests before adding to a devnet
        
        - **EIP6110 request objects encoding**: hold off on changing from JSON to SSZ
        
        - **Engine API engine\_getBlobsV1** (CLs get blobs from EL): general support, decide at next ACDC
        
        - **RIP7212 secp256r1 precompile on L1**: review inclusion in a few months, champions need to help improve testing
    
    - **Quantum resistance**: need overall plan for Verkle, blobs & account abstraction, continue discussion on cryptography channel in Eth R&D Discord
    
    - **Verkle:**
        - **Trie alternatives**: discuss on Verkle implementers call, could swap out Verkle
        
        - [**EIP7736 leaf-level state expiry**](https://docs.google.com/presentation/d/1zCTf54E7OaMrppUeA_T2S4YWvvgGixvlGt4j0E0s1zg/edit) proposal, slows state growth, could enable in upgrade after Verkle
    
    - **EIP4444**
        - [**Torrent prototype**](https://ethresear.ch/t/torrents-and-eip-4444/19788) added EIP7463 proofs

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade, likely targeting Q1 2025**

- [Future of EOA/AA breakout #6](https://ethereum-magicians.org/t/future-of-eoa-aa-breakout-6-july-31-2024/20654):
    - EIP7702 (execution abstraction for EOAs) converging on final spec for Pectra, won’t include migration to contract wallets, additional features would need separate EIPs

[**Osaka + F starname**](https://eips.ethereum.org/EIPS/eip-7607) **upgrade**

- [Verkle implementers call #22](https://ethereum-magicians.org/t/verkle-implementers-call-22-july-29-2024/20664):
    - Witness size could be reduced by 50%, fixes to EIP7612 & EIP-6800 and EIP7748 created for state migration from Merkle Patricia Tree to Verkle

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.8%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~55% majority 
    
    - Consensus layer: Prysm 35%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Layer 1**

- [Geth state history databases overview](https://s1na.substack.com/p/the-tale-of-5-dbs-24-07-26): ethdb, triedb, hashdb, pathdb & statedb  

- [Builder playground](https://github.com/flashbots/builder-playground#readme): locally test a builder with MEV-Boost-Relay, Lighthouse & Reth

- Terence: [Inclusion list timing constraints](https://ethresear.ch/t/inclusion-list-timing-constraints/20198), no perfect design due to trade offs within a slot

- EIP7732 [ePBS breakout #6](https://ethereum-magicians.org/t/epbs-breakout-6-august-2-2024/20665):
    - No spec changes, Prysm implementation in progress with Lodestar starting & discussion on slot auctions

**Research**

- [Restaking risks framework](https://arxiv.org/abs/2407.21785), quantify conditions that validators can be reused across multiple services

**Client Releases**

- Consensus layer:
    - Nimbus [v24.7.0](https://github.com/status-im/nimbus-eth2/releases/tag/v24.7.0): beacon API improvements and fixes

- Execution layer:
    - Besu [v24.7.1](https://github.com/hyperledger/besu/releases/tag/24.7.1): adds experimental [parallel transaction execution](https://www.hyperledger.org/blog/introducing-parallel-transaction-execution-in-hyperledger-besu) with 25-45% block processing improvement
    
    - Erigon:
        - Otterscan [v2.6.0 alpha](https://github.com/otterscan/otterscan/releases/tag/v2.6.0): dark mode, ABI guessing of non-verified contracts via WhatsABI and option to broadcast raw transactions

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - Interface [EIP7749](https://github.com/ethereum/EIPs/pull/8774/files): Add wallet\_signIntendedValidatorData method
    
    - [EIP7212 secp256r1 precompile](https://github.com/ethereum/EIPs/pull/8779) deleted (previously moved to [RIP7212](https://eip.tools/rip/7212))

**Stuff for developers**

- [Underhanded Solidity contest](https://soliditylang.org/blog/2024/07/31/underhanded-solidity-contest-2024-announcement/): transient storage theme, deadline August 31

- Hardhat [v2.22.7](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.22.7): adds RIP7212 secp256r1 precompile support

- Remix [v0.52](https://medium.com/remix-ide/remix-release-v0-52-0-b0761c5e0df6): updated Git plugin & URL to load a GitHub folder into Remix

- Brock: [Interval addition in Solidity](https://brocke.xyz/interval-math)

- [EVMRepl](https://evmrepl.com): adds multi file support & load contract by address

- Coinbase OnchainKit [Transaction](https://x.com/onchainkit/status/1818400608707387603) React component: wraps transaction flow

- smlXL [sim](https://blog.smlxl.io/sim-a-canvas-for-your-ideas-aa80d20e6fa8): create APIs & webhooks using real time onchain data

**Security**

- Convergence Finance [$200k exploit](https://medium.com/@cvg_wireshark/post-mortem-08-01-2024-e80a49d108a0) via lack of input validation, code removed post audit for gas optimization

**Ecosystem**

- Ethereum ninth anniversary of [mainnet launch](https://blog.ethereum.org/2015/07/30/ethereum-launches)
    - Lefteris names the faces in the [launch photo](https://x.com/lefterisjp/status/1818225466022429142)

- Devcon:
    - [Speaker application](https://speak.devcon.org/devcon7-sea/cfp) deadline extended to August 4
    
    - [Community hubs](https://forum.devcon.org/t/rfp-8-devcon-sea-community-hubs/3746) proposals wanted

- Etherscan [funded by](https://x.com/etherscan/status/1818977955437232367): view address & transaction that funded an EOA

* * *

### Job Listings

- [Sablier](https://sablier.notion.site/Careers-at-Sablier-d3771d8eefbf44a8a8428436fb950a1d) are hiring a Business Development Lead and Frontend Engineer

- EF seek a [European/Civil Law qualified Legal Counsel](https://jobs.lever.co/ethereumfoundation/204e2031-e60b-4c43-835a-e6837cef00b2)

- Nethermind: [Senior Device Security Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4336487101), Senior DevOps Engineer [AMER](https://boards.eu.greenhouse.io/nethermind/jobs/4363348101) & [APAC](https://boards.eu.greenhouse.io/nethermind/jobs/4363281101), [Full Stack Lead](https://boards.eu.greenhouse.io/nethermind/jobs/4356246101) APAC, [Post-Grad Internship](https://boards.eu.greenhouse.io/nethermind/jobs/4364252101) & [App Security Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4363291101)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 0.8 to 53.8 gwei, 4.8 gwei average; zero net issuance at 23.7 gwei 
    
    - 14k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,960 - $3,391, currently $2,963, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.048 (Flippening at ~0.164)

**Notable at app layer**

- [Compound](https://rekt.news/the-humpy-dance/) agrees to staked COMP product in exchange for Humpy canceling proposal

- Synthetix [USDx](https://x.com/synthetix_io/status/1819472406437859519) (collateralized stablecoin) on Arbitrum, 0% interest borrowing

**Regulation/business/tokens**

- [Jonathan Mann](https://x.com/songadaymann/status/1817959200930041978) (Song a Day) is suing the SEC to clarify sale of NFT art isn’t an unregistered security

- [BitClout founder charged by SEC](https://www.sec.gov/newsroom/press-releases/2024-91) for fraud & offering unregistered securities

- [Alleged crypto recovery scammer](https://manhattanda.org/d-a-bragg-announces-charges-against-man-who-used-scam-crypto-recovery-website-to-steal-from-hopeful-customers) charged by Manhattan DA

**General**

- [Ferrari exec foiled deepfake audio](https://archive.is/hgJi7); Reminder: [ask security questions](https://vitalik.eth.limo/general/2024/02/09/securityquestions.html)

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-august-3-2024](https://weekinethereumnews.com/week-in-ethereum-news-august-3-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Aug 7-9 – [Science of Blockchain Conference](https://www.sbc-conference.com/) (New York)

- Aug 15-17 – [Ethereum Uruguay](https://www.ethereumuruguay.org/) hackathon & conference

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 23-26 – [ETHTokyo](https://www.ethtokyo.com/) hackathon & conference

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- **Aug 31 –** [**Underhanded Solidity contest**](https://soliditylang.org/blog/2024/07/31/underhanded-solidity-contest-2024-announcement/) **deadline**

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

- **Oct 17-20 –** [**ETHLisbon**](https://ethlisbon.org/) **hackathon**

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

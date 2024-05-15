---
title: "Week in Ethereum News <br> May 11, 2024"
date: "2024-05-11"
---

## Eth News and Links

**All core devs – execution (ACDE)**

- ACDE #187 [call video](https://www.youtube.com/watch?v=yYfzpSme7Cg&t=155s).  Recap from [Tim Beiko](https://twitter.com/TimBeiko/status/1788621887884439869).  Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-187/):
    - [**Pectra-devnet-0**](https://notes.ethereum.org/@ethpandaops/pectra-devnet-0#Client-implementation-tracker): launch early next week, some client teams completed implementations
    
    - **EIP7702 set EOA account code for one transaction:** successor to EIP3074, aimed at improving EOAs and aligned with ERC4337 account abstraction
        - Broad support for including in Pectra
    
    - **SSZ priority**: client teams didn’t support changing to SSZ in Pectra
    
    - **EOF:** Meta EIP & EIP7698 creation transaction added to Pectra considered for inclusion
    
    - **EIP7623 increase calldata costs:** [gas sheltering](https://docs.google.com/presentation/d/1IUJ2TmcNdJbagPEjpZoBohpXEyjfaTJ8FZT4kydJDak) concerns theoretically possible but deemed not viable
    
    - **Reentrancy protection:** EIP7705 reentrancy opcodes proposed to lower protection cost

**Pectra (Prague + Electra) upgrade (meta** [**EIP7600**](https://eips.ethereum.org/EIPS/eip-7600)**), small fork targeting late 2024**

- consensus-specs [v1.5.0-alpha.2](https://github.com/ethereum/consensus-specs/releases/tag/v1.5.0-alpha.2): test case fixes for Electra and fixes for PeerDAS initial interop

- [EVM Object Format (EOF)](https://evmobjectformat.org/) website, work in progress

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.7%**](https://dune.com/hildobby/eth2-staking) **still too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)
    - [**Proposal to create Lido Research**](https://research.lido.fi/t/regoose-updated-goals-for-lido-in-the-light-of-mvi-and-restaking/7462) **to contribute to minimal viable issuance research**

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: **Geth ~62%** majority
        - [**Figment**](https://twitter.com/figment_io/status/1787534701617414422) **went Geth free**
    
    - Consensus layer: **Prysm 37%**
    
    - Any client bug over 33.3% could mean loss of finality
    
    - [**Options for validators to share client info**](https://ethresear.ch/t/research-report-allowing-validators-to-share-client-information-privately-a-project-by-nethermind-research/19506)**: graffiti, gossip or voting**

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Account abstraction breakout #2 [call video](https://www.youtube.com/watch?v=GPdbQxmsXR8&t=4s)
    - Native account abstraction on Layer 1 not expected for several years (after Osaka upgrade)
    
    - EIP7702 succeeds EIP3074, account abstraction aligned with form factor of EIP5806 (new transaction type) & user experience of EIP3074
    
    - Discussion on need for chain ID & nonce in EIP7702

- Vitalik: [multidimensional gas pricing](https://vitalik.eth.limo/general/2024/05/09/multidim.html)

- [History growth viz](https://www.paradigm.xyz/2024/05/how-to-raise-the-gas-limit-2): history growing ~8x faster than state, nodes using 2TB drives will need to upgrade in 2-3 years unless EIP4444 adopted to halve the storage burden

- [Builder market centralization](https://twitter.com/data_always/status/1787181210885615977): private order flow & why builders win blocks

**Research**

- [Fork choice attacks](https://notes.ethereum.org/@fradamt/das-fork-choice) and PeerDAS

- [Asynchrony-resilient sleepy](https://arxiv.org/abs/2309.05347) Total-Order Broadcast (TOB) protocols

**Client Releases**

- Consensus layer:
    - Grandine [v0.4.0/1](https://medium.com/@grandine/grandine-0-4-1-released-fb98daef6d60): optimizations, new attestations packer, in-memory mode, improved compatibility with other validator clients, integrations with Eth-docker & Ethereum on Arm

- Execution layer:
    - Geth [v1.14.3](https://github.com/ethereum/go-ethereum/releases/tag/v1.14.3): block processing & RPC API improvements

**For Stakers**

- Geth [DoS vulnerability via malicious p2p message](https://github.com/ethereum/go-ethereum/security/advisories/GHSA-4xc9-8hmq-j652), patched in v1.13.15

- EthStaker: [hardware recommendations](https://ethstaker.cc/staking-hardware)

**Layer 2**

- Rollcall (L2 standards) #5 [call video](https://www.youtube.com/watch?v=gHYDD5cvQYg): RIP7212 (secp256r1 precompile) spec clarification & pricing, [RIP7696](https://github.com/get-smooth/crypto-lib/blob/main/doc/RollCall_8_5_2024.pdf) presentation (generic double scalar multiplication precompile) and Layer 1 update

- [Commitment Boost](https://ethresear.ch/t/based-proposer-commitments-ethereum-s-marketplace-for-proposer-commitments/19517): proposal to standardize how proposers register & send/receive commitments

- Overview on [based sequencing & preconfirmations](https://research.chainbound.io/examining-the-based-sequencing-spectrum)

**EIPs/Standards**

- EIPs:
    - [EIP7702](https://eips.ethereum.org/EIPS/eip-7702): Set EOA account code for one transaction
    
    - [EIP7703](https://github.com/ethereum/EIPs/pull/8529/files): Increase calldata cost (alternative to [EIP7623](https://eips.ethereum.org/EIPS/eip-7623))
    
    - [EIP7705](https://github.com/ethereum/EIPs/pull/8543/files): NONREENTRANT & REENTRANT opcodes

- ERCs (application layer):
    - [ERC7704](https://github.com/ethereum/ERCs/pull/414/files): Soul resonance token

**Stuff for developers**

- Forge-std [v1.8.2](https://github.com/foundry-rs/forge-std/releases/tag/v1.8.2): adds cheat codes including prompt, blobhashes & ensNamehash

- [Solady](https://github.com/Vectorized/solady#readme) (Solidity snippets): adds UpgradeableBeacon for ERC1967 beacon proxies

- Frangio: [Solidity compiler code generation for stack-based EVM](https://frang.io/blog/codegen-for-stack-machines/) & stack too deep errors

- Viem [experimental](https://viem.sh/experimental) adds ERC6492 signature utilities

- Slitherin (custom Slither detectors) [v0.7.0](https://github.com/pessimistic-io/slitherin/releases/tag/v0.7.0): adds detectors for Arbitrum Chainlink sequencer uptime, readonly reentrancy with Balancer/Curve & price manipulation via token transfers

- [Betterscan](https://github.com/shortdoom/betterscan-v1#readme): inspect verified contracts

- [Profiling Echidna](https://blog.trailofbits.com/2024/05/08/using-benchmarks-to-speed-up-echidna/) found memory leak in hevm

- Guide to [building a tracer using Geth](https://mariusvanderwijden.github.io/blog/2024/05/06/LiveTracer/) for transactions involving a set of addresses

- Etherscan [converter tools](https://twitter.com/etherscan/status/1788906812227666418): Base64, block & date, UTF-8 and method ID

- CTFs:
    - Secureum RACE #29: [answers to 8 question Solidity quiz](https://twitter.com/kamensec/status/1786970628387389781)

**Security**

- Bloom [$600k exploit](https://twitter.com/BloomOnBlast/status/1788695722952421689) on Blast related to rebasing yield, 90% of funds recovered

**Ecosystem**

- Etherscan: [address poisoning attack](https://twitter.com/etherscan/status/1788550675993174409) explainer

- [ETHGlobal Sydney](https://twitter.com/ethglobal/status/1787026754630295566) finalists

- [Verify RLN Proofs](https://vac.dev/rlog/rln-light-verifiers/) in resource restricted devices using subtrees

- [Threshold encryption schemes](https://hackmd.io/@guruvamsi-policharla/new-threshold-schemes) for transaction pool privacy & timelock encryption

* * *

### Job Listings

- [stakefish](https://stake.fish/): [DevOps Engineer](https://apply.workable.com/stakefish/j/8FC077923F/) & [Full-stack Engineer](https://apply.workable.com/stakefish/j/5218ED958E/)

- Devcon: [Production Magician](https://jobs.lever.co/ethereumfoundation/aa4c69f8-f564-4036-9c5e-3e09f0eb27df) & [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/e93dae67-65a6-495c-8638-46e3db28cb64)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 2.6 to 28 gwei, with 5.6 gwei average
    - Zero net issuance currently at 23.3 gwei 
    
    - 13k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,888 - $3,202, currently $2,914

- [ETHBTC](https://ratiogang.com/): currently 0.048 (Flippening at ~0.16)

**Notable at app layer**

- [Fantasy.top](https://twitter.com/hildobby_/status/1787525375440167262) (CryptoTwitter fantasy sports game) 50% of mainnet NFT volume 

- Tokenize.it [Crowdinvesting](https://medium.com/corpus-ventures/crowdinvesting-with-gmbh-token-is-live-9c3969287545): security tokens for German limited liability companies

- [BlackRock-backed Securitize](https://forum.arbitrum.foundation/t/securitize-markets-buidl-step-application/23652) applies for Arbitrum RWA incentives

- [Zora](https://twitter.com/ourzora/status/1787862836301169016) acquired mint.fun

- Splits [v2](https://splits.org/blog/v2-launch/): adds push flow, split can hold any token and splitters & token storage are separate

**Regulation/business/tokens**

- [Robinhood](https://newsroom.aboutrobinhood.com/robinhood-response-to-receipt-of-wells-notice-from-the-u-s-securities-and-exchange-commission/) received Wells Notice from SEC

- [President Biden](https://twitter.com/noelleinmadrid/status/1788667522998247548) plans to veto congressional disapproval of SEC Staff Accounting Bulletin 121
    - [Trump attacks Biden](https://www.politico.com/news/2024/05/10/trump-crypto-biden-00157051) for being anti-crypto

- [Crypto super PACs raised $102M](https://www.citizen.org/article/cryptobros-united-fairshake-super-pac-2024-elections/) for 2024 US elections

- Reminder: [you can write to Virgil Griffith](https://virgil.gr/)

**General**

- [Next.js Server Actions](https://www.assetnote.io/resources/research/digging-for-ssrf-in-nextjs-apps) Server-Side Request Forgery (SSRF) vulnerability

- [Dell data breach](https://www.bleepingcomputer.com/news/security/dell-warns-of-data-breach-49-million-customers-allegedly-affected/) of customer name & physical address

- [Spanish police identified Catalan activist](https://techcrunch.com/2024/05/08/encrypted-services-apple-proton-and-wire-helped-spanish-police-identify-activist/) via Wire & Proton Mail

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-may-11-2024](https://weekinethereumnews.com/week-in-ethereum-news-may-11-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/) hackathon

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- May 31-Jun 5 – [ETH Belgrade](https://ethbelgrade.rs/) hackathon & conference

- Jun 14 – [EF EIP4844 data challenge](https://esp.ethereum.foundation/data-challenge-4844) deadline

- Jun 21-23 – [ETHKyiv](https://ethkyiv.org/) hackathon & conference

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 26-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- **Aug 2-4 –** [**Ethereum Argentina**](https://twitter.com/etherargentina/status/1789007740968284434)

- **Aug 15-17 –** [**Ethereum Uruguay**](https://twitter.com/EthereumUruguay/status/1786144213328879817) **hackathon & conference**

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 23-26 – [ETHTokyo](https://www.ethtokyo.com/) hackathon & conference

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- Sep 5-8 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 9-15 – [ETHSafari](https://ethsafari.xyz/) (Kenya)

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Sep 26-27 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

---
title: "Week in Ethereum News <br> May 25, 2024"
date: "2024-05-25"
---

## Eth News and Links

**All core devs**

- All core devs – execution (ACDE) #188 [call video](https://www.youtube.com/live/jO-BbmSsT_0?t=318s).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1793679999809306810) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-188/):
    - **Pectra (Prague + Electra) upgrade**:
        - **Discussion on when/what to ship**:
            - EF testing team [upgrade options](https://notes.ethereum.org/@ethpandaops/pectra-fork-thoughts), prefer splitting Pectra into two upgrades
            
            - [Reth](https://docs.google.com/document/d/1IfOnozIhp93qkqZ7Jt-jVUvcdRDAv7HOdP4lnsOpu74/edit) propose shipping a big upgrade in Q1 2025 with PeerDAS & EOF
            
            - Including EOF delays Pectra by ~3 months, support from some EL teams & Solidity
                - [EOF benchmarks](https://notes.ethereum.org/@ipsilon/solidity_eof_poc) show some reductions in code size & gas 
            
            - PeerDAS & blob size increase priorities to be discussed by CL teams at ACDC, then finalize Pectra scope at next ACDE
        
        - **EIP7702** replaces EIP3074, CFId, add to next devnet, breakout room needed to [finalize spec](https://github.com/ethereum/EIPs/pull/8561) (optional nonce & chain ID) before including in Pectra
    
    - Execution API proposal to optionally include return data in transaction receipts
    
    - Minimum priority fee: Geth defaults to 1 gwei, evaluate lowering, no need to standardize
    
    - Using Portal network’s history network for history expiry

- Client team interop (Kenya) focused on Pectra, PeerDAS & Verkle:
    - [Pectra-devnet-0 & peerdas-devnet-0](https://x.com/parithosh_j/status/1791897641837596833) launched 
    
    - [EOF breakout](https://hackmd.io/@shemnon/nyota-eof-breakout): discussion on whether to include in Pectra & spec updates
    
    - [PeerDAS](https://notes.ethereum.org/@fradamt/peer-das-design-interop): design simplifications
    
    - [History expiry plan](https://hackmd.io/@6iQDuIePQjyYBqDChYw_jg/BkgzJ3EmR)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.5%**](https://dune.com/hildobby/eth2-staking) **still too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)
    - [**Lido node operator (Numic)**](https://research.lido.fi/t/lido-on-ethereum-node-operator-numic-security-incident-disclosure-may-21-2024/7536) **breach of dev machine with encrypted key backups**

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~55% majority 
    
    - Consensus layer: Prysm 37%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Data Always: [min-bid setting effectiveness](https://x.com/data_always/status/1792650204107219303)

**Research**

- [Anonymous Inclusion Lists (anon-ILs)](https://ethresear.ch/t/anonymous-inclusion-lists-anon-ils/19627): distributed mechanism for anonymizing IL proposers

**Client Releases**

- Consensus layer:
    - Nimbus [v24.5.1](https://github.com/status-im/nimbus-eth2/releases/tag/v24.5.1): beacon & builder API improvements and fixes v24.5.0 compatibility issue with certain hardware

**Layer 2**

- Vitalik: [Layer 2s vs execution sharding](https://vitalik.eth.limo/general/2024/05/23/l2exec.html)

- L2BEAT proposed [data availability risk framework](https://gov.l2beat.com/t/data-availability-risk-framework-call-for-feedback/275)

- [Taiko](https://taiko.mirror.xyz/RjxK3mrDw_ek1w-P768h0Oqghpv8pdfSQ-A51n-izZg) airdrop, eligible GitHub contributors need to bind an address

**EIPs/Standards**

- EIPs:
    - [EIP7709](https://github.com/ethereum/EIPs/pull/8578/files): Read BLOCKHASH from storage and update cost
    
    - [EIP7713](https://github.com/ethereum/EIPs/pull/8594/files): Box types for EIP712 messages 

- RIPs (Rollup Improvement Proposals):
    - [RIP7711](https://github.com/ethereum/RIPs/pull/22/files): RIP7560 transactions bundle transaction type
    
    - [RIP7712](https://github.com/ethereum/RIPs/pull/23/files): Enable RIP7560 transactions using a two-dimensional nonce

- ERCs (application layer):
    - [ERC7710](https://github.com/ethereum/ERCs/pull/433/files): Contract delegation interfaces
    
    - [ERC7714](https://github.com/ethereum/ERCs/pull/435/files): Simple permissions checks
    
    - [ERC7715](https://github.com/ethereum/ERCs/pull/436/files): Request permissions from wallets

**Stuff for developers**

- Solidity [v0.8.26](https://soliditylang.org/blog/2024/05/21/solidity-0.8.26-release-announcement): require with custom errors (via-IR only), Yul optimizer improved default sequence and JSON output format slightly changed

- Remix [v0.49](https://medium.com/remix-ide/remix-release-v0-49-0-b396ab7fff2b): RemixAI improvements & TOML syntax highlighting

- Foundry:
    - [Reusable workflows](https://github.com/sablier-labs/reusable-workflows#readme) for GitHub Actions
    
    - [Merkle Multiproof](https://github.com/sigp/multiproof#readme) (Solidity): generate inputs for OpenZeppelin MerkleProof library for fuzz testing
    
    - [Kontrol](https://x.com/rv_inc/status/1792968702914339268) (formal verification) adds support for native Foundry cheatcode assertions

- [Snekmate](https://github.com/pcaversaccio/snekmate/commit/459ec3f4a643a4decc26b9ad7e2f083e1ff7dc36) (Vyper): adds Halmos symbolic tests for ERC20/721/1155 & math contracts

- [Ape-AWS](https://x.com/apeframework/status/1793068323606798635): Ape plugin to use AWS Key Management Service & IAM access

- [Viem](https://viem.sh/docs/siwe/actions/verifySiweMessage) adds EIP4361 Sign-In with Ethereum support

- [EVM Diff](https://x.com/msolomon44/status/1793071526167843069): adds all chain comparison table to existing side by side compare

- micro-eth-signer [v0.9](https://github.com/paulmillr/micro-eth-signer/releases/tag/0.9.0): fetch account history & token balances from archive node, SSZ in 900 lines

- Vacp2p [stealth-address-kit](https://github.com/vacp2p/stealth-address-kit#readme) v0.1: derived from ERC5564, Rust & C bindings

**Security**

- Gala Games [$22M exploit](https://rekt.news/gala-games-rekt/) via mint using admin access

- [SEAL wargame with Base & Optimism](https://www.coinbase.com/en-au/blog/strengthening-our-defenses-with-seal-wargame-simulations): simulated vulnerability in bridge withdrawals 

**Ecosystem**

- EF [working on formal policy](https://x.com/ayamiyagotchi/status/1793965259524653058) for potential conflicts of interest
    - [Justin Drake](https://twitter.com/drakefjustin/status/1792143477163106787) & [Dankrad Feist](https://x.com/dankrad/status/1792741374447534083) advising EigenFoundation

- [Devcon tickets](https://x.com/EFDevcon/status/1793602979632971821) go live in June

* * *

### Job Listings

- ChainSafe: [Head of Protocol Engineering](https://grnh.se/c6e27e794us), [DevRel](https://grnh.se/6627a6284us) - Sygma and [more jobs](https://grnh.se/108a0afd4us)

- Privacy and Scaling Explorations: [ZK Circuits Engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4)

- [stakefish](https://stake.fish/): [DevOps Engineer](https://apply.workable.com/stakefish/j/8FC077923F/) & [Full-stack Engineer](https://apply.workable.com/stakefish/j/5218ED958E/)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 1.9 to 111.5 gwei, with 9.1 gwei average
    - Zero net issuance currently at 23.3 gwei 
    
    - 11k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,063 - $3,913, currently $3,723

- [ETHBTC](https://ratiogang.com/): currently 0.054 (Flippening at ~0.16)

**Notable at app layer**

- Optimism [Retro Funding](https://retrofunding.optimism.io/) round 4: 10M OP for Superchain deployers

- [Yuga Labs to no longer touch Punks](https://x.com/cryptogarga/status/1792694910904136028) after [Super Punk World](https://x.com/cryptopunksnfts/status/1792594316172341315) backlash

**Regulation/business/tokens**

- [SEC approved eight spot ETH ETF proposals](https://www.sec.gov/files/tm/lk87adfs99.pdf), they go live when S-1 approval occurs

- [US House passed FIT21 bill](https://financialservices.house.gov/news/documentsingle.aspx?DocumentID=409277), would give CFTC jurisdiction over digital commodities
    - It’s a [bad bill](https://x.com/stephendpalley/status/1793361140723941677) yet still a [big victory](https://www.axios.com/2024/05/22/crypto-legislation-fit21-house-passes)

- [Genesis $2B settlement](https://ag.ny.gov/press-release/2024/attorney-general-james-secures-settlement-worth-2-billion-crypto-firm-genesis) with New York Attorney General

**General**

- [Time-based cryptography from weaker assumptions](https://eprint.iacr.org/2024/769): randomness beacons & delay functions

- [Kabosu](https://x.com/AyaMiyagotchi/status/1793994458268369211) (the Doge) passed away

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-may-25-2024](https://weekinethereumnews.com/week-in-ethereum-news-may-25-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- May 26 – [Ethereum Protocol Fellowship](https://blog.ethereum.org/2024/05/13/epf-5-announcement) cohort 5 application deadline

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- May 31-Jun 5 – [ETH Belgrade](https://ethbelgrade.rs/) hackathon & conference

- Jun 14 – [EF EIP4844 data challenge](https://esp.ethereum.foundation/data-challenge-4844) deadline

- Jun 21-23 – [ETHKyiv](https://ethkyiv.org/) hackathon & conference

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 29-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 2-4 – [Ethereum Argentina](https://twitter.com/etherargentina/status/1789007740968284434)

- Aug 15-17 – [Ethereum Uruguay](https://twitter.com/EthereumUruguay/status/1786144213328879817) hackathon & conference

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 23-26 – [ETHTokyo](https://www.ethtokyo.com/) hackathon & conference

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- Sep 5-8 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 9-15 – [ETHSafari](https://ethsafari.xyz/) (Kenya)

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Sep 26-27 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 4-6 – [Ethereum Kuala Lumpur](https://www.2024.ethkl.org/) conference & hackathon

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

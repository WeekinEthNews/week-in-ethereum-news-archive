---
title: "Week in Ethereum News <br> May 18, 2024"
date: "2024-05-18"
---

## Eth News and Links

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade, small fork targeting late 2024**

- [Pectra-devnet-0](https://dora.pectra-devnet-0.ethpandaops.io/) launched

[**Osaka + F starname**](https://eips.ethereum.org/EIPS/eip-7607) **upgrade**

- Dankrad Feist: [benefits of Verkle](https://x.com/dankrad/status/1790721271321256214), increase block size 10x, simplify node architecture, reduce sync time, reduce node cost & enable path to light nodes

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.6%**](https://dune.com/hildobby/eth2-staking) **still too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: **Geth ~55% majority** 
        - [**Lido 46.6% Geth**](https://app.hex.tech/8dedcd99-17f4-49d8-944e-4857a355b90a/app/3f7d6967-3ef6-4e69-8f7b-d02d903f045b/latest?tab=client-diversity) **at end of Q1**
        
        - [**Kiln went Geth free**](https://x.com/abcoathup/status/1791363720503066835)**, 100% Nethermind**
    
    - Consensus layer: Prysm 37%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Data Always: [timing games as a service viz](https://twitter.com/data_always/status/1790130377622687909)

- Piper Merriam: [storing large SSZ objects in Portal Network](https://ethresear.ch/t/distributed-storage-and-cryptographically-secured-retrieval-of-ssz-objects-for-portal-network/19575) to archive Ethereum’s state data

- [Nethermind (execution layer client) scaling roadmap](https://twitter.com/urozmej/status/1790482152011812980) via optimizations, Paprika, parallelization & compiling bytecode to native

**Research**

- [Abstracted execution tickets](https://collective.flashbots.net/t/where-the-execution-ticket-discussion-actually-should-start/3425)

**Client Releases**

- Consensus layer:
    - Lodestar [v1.18.1](https://github.com/ChainSafe/lodestar/releases/tag/v1.18.1): hotfix to disable flood publishing for local block builders with orphaned/missed block proposals

- Execution layer:
    - Besu [v24.5.1](https://github.com/hyperledger/besu/releases/tag/24.5.1): snap sync server (early access) and receipt storage size reduced
    
    - Erigon [v2.60.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.60.0): last planned v2 release, fixes logs pruning issue in v2.59

**Layer 2**

- [Degen & Apex rollups](https://twitter.com/conduitxyz/status/1790065376975552549) stopped posting batches for more than 24 hours after config change, first batches triggered reorgs

- [User-defined penalties](https://ethresear.ch/t/user-defined-penalties-ensuring-honest-preconf-behavior/19545): proposal for preconf crypto-economic security

**EIPs/Standards**

- EIPs:
    - [EIP7706](https://github.com/ethereum/EIPs/pull/8552/files): Separate gas type for calldata
    
    - [EIP7707](https://github.com/ethereum/EIPs/pull/8563/files): Incentivize access list provisioning
    
    - [EIP7708](https://github.com/ethereum/EIPs/pull/8575/files): ETH transfers emit a log

**Stuff for developers**

- Hardhat [v2.22.4](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.22.4): adds BigInt task argument type

- Guide to [Hardhat Ignition deployment using Ledger](https://blog.nomic.foundation/secure-deployments-with-hardhat-ignition-and-ledger-hardware-wallets-028080159e77)

- [Foundry roadmap](https://x.com/gakonst/status/1790770389523583163) of planned 2024 features

- Heimdall-rs [v0.8.0](https://jbecker.dev/research/heimdall-0-8-0): decompilation & decode improvements and more modular code base

- [Wagmi](https://wagmi.sh/vue/getting-started) adds Vue support

- [Betherscan](https://github.com/tiagofneto/betherscan#readme) (browser extension): adds data fields to Etherscan, including block header RLP, contract storage root, EOA nonce and transaction signature (v, r, s)

- [ERC5189 (account abstraction via endorsed operations) bundler](https://erc5189.io/): execute account abstraction transactions (e.g. ERC4337)

- Vitalik: [proposal for MACI with votes offchain by default](https://ethresear.ch/t/maci-with-mostly-off-chain-happy-path/19527)

**Security**

- Sonne Finance (Compound v2 fork) [~$20M exploit](https://rekt.news/sonne-finance-rekt/) on Optimism via known donation attack
    - [$6.5M saved](https://x.com/tonyke_bot/status/1790547461611860182)

- Predy Finance [~$0.5M exploit](https://predyfinance.medium.com/postmortem-report-on-the-details-of-the-events-of-may-14-2024-8690508c820b) on Arbitrum via a callback

**Ecosystem**

- Vitalik: [improving permissionlessness & decentralization in short/mid term](https://vitalik.eth.limo/general/2024/05/17/decentralization.html), MEV, liquid staking & node hardware

- [Ethereum Protocol Fellowship](https://blog.ethereum.org/2024/05/13/epf-5-announcement) cohort 5 applications open

- [EF Q1 grantees](https://blog.ethereum.org/2024/05/14/esp-allocation-q124) share $11M in funding

- Etherscan [contract statistics](https://etherscan.io/dashboards/contract-statistics) of most called functions & language versions

* * *

### Job Listings

- [stakefish](https://stake.fish/): [DevOps Engineer](https://apply.workable.com/stakefish/j/8FC077923F/) & [Full-stack Engineer](https://apply.workable.com/stakefish/j/5218ED958E/)

- Devcon: [Production Magician](https://jobs.lever.co/ethereumfoundation/aa4c69f8-f564-4036-9c5e-3e09f0eb27df) & [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/e93dae67-65a6-495c-8638-46e3db28cb64)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 2.3 to 45.9 gwei, with 5.9 gwei average
    - Zero net issuance currently at 23.3 gwei 
    
    - 13k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,874 - $3,116, currently $3,096

- [ETHBTC](https://ratiogang.com/): currently 0.046 (Flippening at ~0.16)

**Notable at app layer**

- Rune: [Dai endgame](https://forum.makerdao.com/t/reconciling-the-two-opposing-paths-for-decentralized-stablecoins/24280), NewStable (USD pegged with real world asset collateral) & PureDai (floating peg with decentralized collateral) 

- Words3 [infinite](https://x.com/0xsmallbrain/status/1790960226260443271) live on Redstone, scrabble with fluctuating price letter tiles

**Regulation/business/tokens**

- Tornado Cash developer [Alex Pertsev sentenced to 64 months in prison](https://gist.github.com/MicahZoltu/ced4f886b44c31108721ed0513f0eba7) for money laundering

- [US Senate voted](https://x.com/AlexanderGrieve/status/1791147474243162279) to repeal anti-crypto SEC Staff Accounting Bulletin 121 that precluded banks offering crypto custody

- [“Low carb crusader” brothers charged](https://www.justice.gov/usao-sdny/pr/two-brothers-arrested-attacking-ethereum-blockchain-and-stealing-25-million) with wire fraud & conspiracy to commit money laundering
    - Reminder: [MEV-Boost relay exploit on April 3, 2023](https://collective.flashbots.net/t/post-mortem-april-3rd-2023-mev-boost-relay-incident-and-related-timing-issue/1540) & [low carb crusader disclosure](https://collective.flashbots.net/t/disclosure-mitigation-of-block-equivocation-strategy-with-early-getpayload-calls-for-proposers/1705)

**General**

- [P-256 hash-seed still hasn’t been found](https://twitter.com/pcaversaccio/status/1790671134574231994), RIP7212 secp256r1 precompile being added by rollups

- [RLN-v3](https://vac.dev/rlog/rln-v3/) adds epoch-based message rate-limiting scheme

- Notes on [collaborative zkSNARKS](https://www.leku.blog/co-snarks/)

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-may-18-2024](https://weekinethereumnews.com/week-in-ethereum-news-may-18-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/) hackathon

- **May 26 –** [**Ethereum Protocol Fellowship**](https://blog.ethereum.org/2024/05/13/epf-5-announcement) **cohort 5 application deadline**

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

- **Oct 4-6 –** [**Ethereum Kuala Lumpur**](https://www.2024.ethkl.org/) **conference & hackathon**

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

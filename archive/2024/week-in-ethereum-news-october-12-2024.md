---
title: "Week in Ethereum News <br> October 12, 2024"
date: "2024-10-11"
---

## Eth News and Links

**Eth R&D protocol call (All Core Devs)**

- [Eth R&D protocol call](https://ethereum-magicians.org/t/all-core-devs-execution-acde-198-october-10-2024/21314) focused on execution layer (ACDE #198):
    - **Pectra upgrade:**
        - [**Pectra-devnet-3**](https://pectra-devnet-3.ethpandaops.io/): issues being found & fixed
        
        - **Pectra-devnet-4**: plan to launch next week
        
        - **EIP2537 BLS precompile**: [breakout](https://github.com/ethereum/pm/issues/1176) to finalize gas pricing & specs
        
        - **Public testnet**: launch by Devcon
    
    - **Proposed EIPs:**
        - **EIP7783 gradually increase gas limit**: can implement without an upgrade
        
        - **EIP7782 reduce slot time to 8 seconds**: alternative to raising blob count
    
    - **EIP4444**: Nethermind continuing Portal network integration

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- Base [blob increase proposal](https://docs.google.com/document/d/19jZcm5CgWM12Eqg1HRwG_ppd1EL9tduheckBmoFBCNM/edit): recommends target of 5 & max of 8 blobs (up from 3/6), implementing engine\_getBlobsV1 & IDONTWANT and disabling flood publishing

- Consensus-specs [v1.5.0-alpha.8](https://github.com/ethereum/consensus-specs/releases/tag/v1.5.0-alpha.8): pectra-devnet-4 target

- [Weekly testing call #8](https://ethereum-magicians.org/t/pectra-testing-call-8-7-october-2024/21310)

[**Fusaka**](https://eips.ethereum.org/EIPS/eip-7607) **(Osaka + Fulu) upgrade**

- [Peerdas-devnet-3](https://peerdas-devnet-3.ethpandaops.io/): launched with peerdas-devnet-2 spec, issue caused clients to be on different forks

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 27.9%**](https://dune.com/hildobby/eth2-staking)**, moving away from** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~52% majority
    
    - Consensus layer: **Prysm 36%**
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Layer 1**

- Vitalik: [surgical EVM scaling](https://docs.fileverse.io/0x7248Fe92e7087d02D3604396b057295026FC62A1/11#key=TzTUg8bvpPrvJBfdfd7jp7xOgXW0hZM2sakCrewfH_cESgipb3i7QetgyUSTXNfq), EVMMAX + SIMD and reduce some opcode gas costs

- EIP7732 ePBS:
    - [ePBS breakout #11](https://ethereum-magicians.org/t/epbs-breakout-11-october-11-2024/21323): Prysm aim to launch devnet in 2 weeks

**Research**

- Fork-Choice enforced Inclusion Lists (FOCIL):
    - Terence: [transaction invalidation in FOCIL](https://hackmd.io/@ttsao/tx-invalidation-complexity) & impact on block producers/verifiers
    
    - [Uncrowdability of FOCIL](https://mirror.xyz/julianma.eth/Gnd8N1IsoHuGHRisp6nCldlt72ZacoXUA-O76qQN3mc): outsourcing inclusion list construction rights is not individually profitable

- [Silent threshold encryption](https://www.paradigm.xyz/2024/10/removing-the-relays) combined with ZK or TEEs to remove MEV-Boost relays

**Client Releases**

- Consensus layer:
    - Teku [v24.10.0](https://github.com/Consensys/teku/releases/tag/24.10.0): adds engine\_getBlobsV1 & IDONTWANT support and disabled flood publishing; [v24.10.1](https://github.com/Consensys/teku/releases/tag/24.10.1): hotfix for validators proposer config that prevented startup in v24.10.0

- Execution layer:
    - Nethermind [v1.29.0](https://github.com/NethermindEth/nethermind/releases/tag/1.29.0): adds heuristics-based censorship detection for high-paying transactions & addresses
    
    - Reth [v1.1.0](https://github.com/paradigmxyz/reth/releases/tag/v1.1.0): Engine 2.0 enabled by default (except op-reth), new metrics & RPC improvements

**Layer 2**

- Flashbots [Rollup-Boost](https://writings.flashbots.net/introducing-rollup-boost): block building using TEEs, starting with 250ms Flashblocks (partial blocks) and priority ordering

- [L2 standards meeting](https://ethereum-magicians.org/t/rollcall-8-october-9-2024/21311) (RollCall #8): RIP7755 cross-L2 calls presentation, Pectra upgrade expected Q1 2025 (optimistically February) & upcoming breakout on [future of EVM on L2](https://github.com/ethereum/pm/issues/1171)

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7782](https://eips.ethereum.org/EIPS/eip-7782): Reduce slot time for lower peak bandwidth
    
    - [EIP7783](https://github.com/ethereum/EIPs/pull/8933/files): Add controlled gas limit increase strategy
    
    - [EIP7784](https://github.com/ethereum/EIPs/pull/8935/files): GETCONTRACT opcode

- ERCs (application layer):
    - [ERC7785](https://github.com/ethereum/ERCs/pull/669/files): Onchain registration of chain identifiers 

**Stuff for developers**

- Solidity [v0.8.28](https://soliditylang.org/blog/2024/10/09/solidity-0.8.28-release-announcement/): adds transient storage state variables for value types, generates JSON for Yul ASTs on demand to reduce memory usage and adds ability to request bytecode/IR for subset of contracts

- RareSkills: [storage slots for dynamic types](https://www.rareskills.io/post/solidity-dynamic) in Solidity (mappings, arrays, strings & bytes)

- Circom [v2.2.0](https://github.com/iden3/circom/releases/tag/v2.2.0): adds buses (groups related signals under one name)

- [Circuitscan](https://circuitscan.org/): submit/browse verified Circom circuits

**Security**

- EigenLayer [$6M stolen](https://rekt.news/eigenoops/) via compromised investor email thread, token vesting not enforced onchain but via legal documents

**Ecosystem**

- Ethereum Foundation [EcoDev research fellowships](https://blog.ethereum.org/2024/10/11/research-fellowship-app) (6 months), deadline November 15

- Hackathon projects: [Ethereum Kuala Lumpur](https://ethkl-24.devfolio.co/projects) & [ETHRome](https://taikai.network/ethrome/hackathons/ethrome-24/projects)

**Enterprise**

- Stripe [Pay with Crypto](https://docs.stripe.com/crypto/pay-with-crypto): US businesses can accept USDC on mainnet, settled in USD

* * *

### Job Listings

- Sigma Prime is hiring Rust developers and security engineers. [Remote roles](https://github.com/sigp/positions-vacant)!

- [Executive Director](https://docs.google.com/document/d/16qSjXRk2r9v6EnRRVSCoQjrPyJB6icoWgBkCxAme8Nc/edit) for Enterprise Ethereum Alliance

- Nethermind [InfoSec Head](https://job-boards.eu.greenhouse.io/nethermind/jobs/4371138101), [Sr Dev](https://job-boards.eu.greenhouse.io/nethermind/jobs/4387067101), [SRE Lead](https://job-boards.eu.greenhouse.io/nethermind/jobs/4390680101), [Sr Embedded Dev](https://job-boards.eu.greenhouse.io/nethermind/jobs/4391152101) & [UX UI designer](https://job-boards.eu.greenhouse.io/nethermind/jobs/4418511101)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 1.9 to 129.9 gwei, 15.1 gwei average; zero net issuance at 24.3 gwei 
    
    - 7k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,346 - $2,504, currently $2,440, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.039 (Flippening at ~0.164)

**Notable at app layer**

- [ZKP2P Tickets](https://tickets.zkp2p.xyz/how-it-works): lower fee secondary market for Ticketmaster, zk proof of transfer

**Regulation/business/tokens**

- SEC:
    - [Crypto.com received Wells notice](https://crypto.com/company-news/complaint)
    
    - [Cumberland DRW charged](https://x.com/CumberlandSays/status/1844424478660624806) for allegedly operating as an unregistered dealer

- [FTX bankruptcy plan approved](https://www.coindesk.com/policy/2024/10/07/delaware-judge-approves-ftx-estates-bankruptcy-plan/), customers to receive cash for 118% on average of holdings value at the time of bankruptcy

- [FBI charge projects & market makers](https://www.justice.gov/usao-ma/pr/eighteen-individuals-and-entities-charged-international-operation-targeting-widespread) for market manipulation & wash trading, [NexF token](https://etherscan.io/address/0x16ca471ae755f8a2cd4ec315a4a7439dcfebe54c#code) created on mainnet as part of investigation

**General**

- [TD Bank plead guilty](https://www.justice.gov/opa/pr/td-bank-pleads-guilty-bank-secrecy-act-and-money-laundering-conspiracy-violations-18b) to US Bank Secrecy Act & money laundering conspiracy violations, $1.8B in penalties, no individuals charged

- [US broadband attack](https://archive.is/aISAy) linked to China, may have had access to wiretap infrastructure

- Internet Archive [Wayback Machine](https://x.com/brewster_kahle/status/1844183111514603812) offline after DDoS attack & data breach

- [WHIR](https://eprint.iacr.org/2024/1586): IOP of proximity for constrained Reed-Solomon codes, verifier runs in hundreds of microseconds

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-october-12-2024](https://weekinethereumnews.com/week-in-ethereum-news-october-12-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Oct 16 – [Gitcoin Grants 22](https://grants.gitcoin.co/), OSS application deadline

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Oct 25-27 – [ETHSydney](https://2024.ethsydney.net/) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

- Dec 6-8 – [ETHIndia](https://ethindia.co/) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

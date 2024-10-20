---
title: "Week in Ethereum News <br> October 19, 2024"
date: "2024-10-18"
---

## Eth News and Links

**Eth R&D protocol call (All Core Devs)**

- [Consensus layer focused protocol call](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-144-october-17-2024/21354) (ACDC #144):
    - **Pectra upgrade:**
        - Spec refinement discussions
        
        - **Blob increase:**
            - Base [blob increase proposal](https://docs.google.com/document/d/19jZcm5CgWM12Eqg1HRwG_ppd1EL9tduheckBmoFBCNM/edit) presented: target 5, max 8 blobs
            
            - [engine\_getBlobsV1 initial results](https://hackmd.io/@ttsao/get-blobs-early-results): bandwidth reduced for download but increased for upload
            
            - EIP7742 uncouple blob count between CL/EL: makes changing blob count easier, consensus layer teams support scheduling for inclusion, review on next week's call with execution layer teams
    
    - **EIP7783 controlled gas limit increase**
    
    - **EIP7782 reduce slot time to 8s**: 2-4s would be more attractive option, needs more analysis, could conflict with future potential upgrades

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- [Pectra-devnet-4](https://pectra-devnet-4.ethpandaops.io/): launched; 20% offline (10% Grandine & 10% Erigon)

- [Weekly testing call #9](https://ethereum-magicians.org/t/pectra-testing-call-9-14-october-2024/21377): fusaka-devnet-0 planned for ~2 weeks time & [ssz-devnet-0](https://ssz-devnet-0.ethpandaops.io/) launched

- EIP2537 BLS precompiles:
    - Feedback wanted on [planned EIP2537 usage](https://hackmd.io/@ralexstokes/eip-2537-rfc) & need for subgroup checks
    
    - [EIP2537 BLS breakout](https://ethereum-magicians.org/t/eip2537-bls-breakout-october-14-2024/21356): discussed removing subgroup checks & precompiles are underpriced

[**Fusaka**](https://eips.ethereum.org/EIPS/eip-7607) **(Osaka + Fulu) upgrade**

- [PeerDAS breakout #10](https://ethereum-magicians.org/t/peerdas-breakout-10-october-15-2024/21353): continuing to debug peerdas-devnet-3, unfinalized for over a week

- [EOF implementers call #60](https://ethereum-magicians.org/t/eof-implementers-call-60-october-16-2024/21313): discussed ERC721 support using EXTCODE/HASCODE, EXT\*CALL return codes and EOFCREATE hashing

**Layer 1**

- Giulio Rebuffo (Erigon): proposal to [raise the gas limit via EIP7783](https://giulioswamp.substack.com/p/are-we-finally-ready-for-a-gas-limit)

- ProbeLab [Hermes](https://www.probelab.network/blog/hermes-a-monitoring-light-node-for-gossipsub-based-networks): GossipSub listener & tracer for libp2p

- Péter Szilágyi: [Geth prototype of ExEx](https://github.com/ethereum/go-ethereum/pull/30611) (Reth Execution Extensions)

- [Ephemery testnet incentives](https://notes.ethereum.org/5O-S9QP1SxSYS8Eado6Wbg) for genesis validators, infrastructure & client implementations

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~52% majority
    
    - Consensus layer: **Prysm 37% & Lighthouse 33.4%**
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Client Releases**

- Consensus layer:
    - Besu [v24.10.0](https://github.com/hyperledger/besu/releases/tag/24.10.0): adds support for blobs in multiple transactions to engine\_getBlobsV1 and Ephemery testnet support
    
    - Prysm [v5.1.2](https://github.com/prysmaticlabs/prysm/releases/tag/v5.1.2): hotfix for v5.1.1 to recover from panic; [v5.1.1](https://github.com/prysmaticlabs/prysm/releases/tag/v5.1.1): experimental state enabled by default and adds IDONTWANT support

- Execution layer:
    - Nethermind [v1.29.1](https://github.com/NethermindEth/nethermind/releases/tag/1.29.1): improved memory usage on Linux and improved OP Stack sync
    
    - Teku [v24.10.2](https://github.com/Consensys/teku/releases/tag/24.10.2): hotfix for v24.10.x preventing startup on Windows

**Layer 2**

- [World Chain](https://world.org/blog/announcements/world-chain-now-open-every-human) (OP Stack rollup) open to public

- [Fuel Ignition](https://fuel.mirror.xyz/U2xqey0oZFCrIBf7bO3yYyFplJKiJ0sfzAyYmhrPjag) (FuelVM) live, UTXO based

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7788](https://github.com/ethereum/EIPs/pull/8972/files): Dynamic target blob count
    
    - Informational [EIP7790](https://github.com/ethereum/EIPs/pull/8974/files): Parameter recommendations for controlled gas limit increase strategy

- RIPs (rollup improvement proposals):
    - [RIP7789](https://github.com/ethereum/RIPs/pull/40/files): Cross rollup contingent transactions 

- ERCs (application layer):
    - [ERC7786](https://github.com/ethereum/ERCs/pull/673/files): Cross-chain messaging gateway
    
    - [ERC7787](https://github.com/ethereum/ERCs/pull/674/files): Soulbound degradable governance

**Stuff for developers**

- [Underhanded Solidity contest](https://soliditylang.org/blog/2024/10/14/announcing-the-underhanded-contest-winners-2024/): Gerard Persoon solo winner with fallback from transient storage

- OpenZeppelin Contracts [v5.1](https://blog.openzeppelin.com/introducing-openzeppelin-contracts-v5.1): adds P256 & RSA signature validation; MerkleTree, CircularBuffer & Heap data structures; StorageSlot, ReentrancyGuardTransient & SlotDerivation utilities; updated Arrays, Base64, CREATE2, Strings & Math 

- Guide to [invariant testing](https://getrecon.substack.com/p/first-day-at-invariant-school) using Recon Builder for scaffolding a Foundry project

- Echidna [v2.2.5](https://github.com/crytic/echidna/releases/tag/v2.2.5): adds Cancun support, warns if an assert isn’t hit in assert mode, adds cheat codes and collects coverage during deployment

- Pcaversaccio [white hat frontrunning](https://github.com/pcaversaccio/white-hat-frontrunning#readme): Bash script using Foundry cast & chisel to secure funds from compromised wallets

**Security**

- Radiant Capital [$50M exploit](https://medium.com/@RadiantCapital/radiant-post-mortem-fecd6cd38081) on Arbitrum & BSC via compromised devices of 3/11 signers; revoke approvals on all chains

**Ecosystem**

- Vitalik on Ethereum improvements being considered:
    - [Proof of Stake (the Merge)](https://vitalik.eth.limo/general/2024/10/14/futures1.html): single slot finality, 1 ETH staking, single secret leader election, faster transaction confirmations, 51% attack recovery, increasing quorum threshold for finality and quantum resistance
    
    - [Scaling (the Surge)](https://vitalik.eth.limo/general/2024/10/17/futures2.html): data availability sampling, data compression, generalized Plasma, maturing L2 proof systems, cross-L2 interoperability and scaling L1 execution

- Propose [Devcon satellite events](https://esp.ethereum.foundation/devcon-grants)

* * *

### Job Listings

- Sigma Prime is hiring Rust developers and security engineers. [Remote roles](https://github.com/sigp/positions-vacant)!

- [Executive Director](https://docs.google.com/document/d/16qSjXRk2r9v6EnRRVSCoQjrPyJB6icoWgBkCxAme8Nc/edit) for Enterprise Ethereum Alliance

- Nethermind: [Sr Dev](https://job-boards.eu.greenhouse.io/nethermind/jobs/4387067101) (Rust, Go) & [Sr Contract Auditor](https://job-boards.eu.greenhouse.io/nethermind/jobs/4411504101) (Rust)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 5.3 to 111.8 gwei, 16.4 gwei average; zero net issuance at 24.3 gwei 
    
    - 6k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,436 - $2,671, currently $2,641, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.039 (Flippening at ~0.164)

**Notable at app layer**

- [dGEN1](https://www.freedomfactory.io/) (mobile device): runs ethOS, ships 2025, pre-order via mint on Base

- [Towns](https://blog.towns.com/go-to-town): gated group chats using River & Base

- [Trump promoted](https://x.com/realDonaldTrump/status/1846326266011762820) World Liberty Financial token sale

**General**

- FBI arrested [alleged SEC Twitter SIM swapper](https://www.justice.gov/usao-dc/pr/fbi-arrests-alabama-man-january-2024-sec-x-hack-spiked-value-bitcoin)

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-october-19-2024](https://weekinethereumnews.com/week-in-ethereum-news-october-19-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Oct 25-27 – [ETHSydney](https://2024.ethsydney.net/) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

- Dec 6-8 – [ETHIndia](https://ethindia.co/) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

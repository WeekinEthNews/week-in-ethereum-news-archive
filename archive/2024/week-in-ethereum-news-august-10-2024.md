---
title: "Week in Ethereum News <br> August 10, 2024"
date: "2024-08-10"
---

## Eth News and Links

**All core devs**

- [All Core Devs - Consensus (ACDC) #139](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-139-august-8-2024/20705):
    - **Pectra (Prague + Electra) upgrade:**
        - [**Pectra-devnet-2**](https://pectra-devnet-2.ethpandaops.io/): a few client issues, tested recovery from non-finality
        
        - **Pectra-devnet-3**: expected soon with EIP7702 (set EOA account code) 
        
        - **Weekly testing call:** starts Monday
        
        - **EIP7594 PeerDAS**: sampling to be ignored on next PeerDAS devnet
    
    - [**Node monitoring using discv5**](https://probelab.io/ethereum/discv5/2024-31/): 42% of nodes use Lighthouse, 36% in US, 50% in data centers

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade, likely targeting Q1 2025**

- consensus-specs [v1.5.0-alpha.4](https://github.com/ethereum/consensus-specs/releases/tag/v1.5.0-alpha.4): fixes off-by-one in MaxEB consolidation processing

- PeerDAS:
    - [PeerDAS without peer sampling](https://hackmd.io/@fradamt/no-peer-sampling) (SubnetDAS) proposal, minimal form of DAS which can be shipped in a few months
    
    - [PeerDAS breakout #5](https://ethereum-magicians.org/t/peerdas-breakout-5-august-5-2024/20706)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.8%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~55% majority 
    
    - Consensus layer: **Prysm 36%**
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Layer 1**

- Flashbots: [TEE-Boost](https://collective.flashbots.net/t/tee-boost/3741), proposal for validators to accept TEE proofs directly from block builders, reduce & eventually remove relays in MEV-Boost

**Research**

- [BRAID](https://x.com/_charlienoyes/status/1820502474521727475): multi-proposers by running multiple consensus processes in parallel, early stage

**Client Releases**

- Consensus layer:
    - Lighthouse [v5.3.0](https://github.com/sigp/lighthouse/releases/tag/v5.3.0): faster beacon node startup, improved block proposal reliability, improved validator client broadcast and gossipsub IDONTWANT support
    
    - Lodestar [v1.21.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.21.0): docker image changed to debian, adds execution layer client info to graffiti and performance improvements via napi-rs BLST bindings
    
    - Teku [v24.8.0](https://github.com/Consensys/teku/releases/tag/24.8.0): updated metrics, requires Java 21+

- Execution layer:
    - Erigon [v3.0.0-alpha2](https://erigon.tech/erigon-3-alpha-2-introducing-blazingly-fast-sync-on-archive-nodes-with-ottersync-and-other-improvements/): adds OtterSync fast sync by downloading state via BitTorrent, improves chain tip performance and reduces disk footprint
    
    - Reth [v1.0.4](https://github.com/paradigmxyz/reth/releases/tag/v1.0.4): RPC fixes and resolves IO deadlock edge case during sync

**Layer 2**

- Arbitrum Orbit chains [bridged USDC as gas token](https://blog.arbitrum.io/announcing-bridged-usdc-as-a-custom-gas-token-for-orbit-chains/)

- Mode, Zora & Metal [upgrade ownership changed](https://x.com/conduitxyz/status/1821592449544016112) to Optimism Foundation & security council

**EIPs/Standards**

- ERCs (application layer):
    - [ERC7750](https://github.com/ethereum/ERCs/pull/573/files): Decentralized employment system
    
    - [ERC7751](https://github.com/ethereum/ERCs/pull/578/files): Wrapping of bubbled up reverts
    
    - [ERC7752](https://github.com/ethereum/ERCs/pull/579/files): Equity token
    
    - [ERC7753](https://github.com/ethereum/ERCs/pull/584/files): Algorithmically generated NFT
    
    - [ERC7754](https://github.com/ethereum/ERCs/pull/585/files): Tamperproof web immutable transaction 

**Stuff for developers**

- Solhint [v5.0.3](https://github.com/protofire/solhint/releases/tag/v5.0.3): adds imports-order rule to sort Solidity imports topologically & alphabetically

- Viem [experimental](https://viem.sh/experimental/eip7702) adds EIP7702 (set EOA account code) support

- Rindexer (EVM indexing): adds [streaming data](https://rindexer.xyz/docs/start-building/streams) & [chatbot](https://rindexer.xyz/docs/start-building/chatbots) support

- Rainbow wallet extension [impersonation mode](https://x.com/rainbowdotme/status/1821989351913660433)

- [Tbl](https://github.com/paradigmxyz/tbl#readme): CLI to read/edit Parquet files

**Security**

- Ronin bridge [$12M exploit](https://rekt.news/roninnetwork-rektII/) via uninitialized parameter after upgrade, MEV bots front ran, funds have been returned, $500k bounty

* * *

### Job Listings

- [Sablier](https://sablier.notion.site/Careers-at-Sablier-d3771d8eefbf44a8a8428436fb950a1d) are hiring a Business Development Lead and Frontend Engineer

- EF seek a [European/Civil Law qualified Legal Counsel](https://jobs.lever.co/ethereumfoundation/204e2031-e60b-4c43-835a-e6837cef00b2)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 0.8 to 701.7 gwei, 10.3 gwei average; zero net issuance at 23.9 gwei 
    
    - 10k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,197 - $3,004, currently $2,601, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.043 (Flippening at ~0.164)

**Notable at app layer**

- Zora [secondary market](https://zora.co/writings/onchain-secondary-markets) for mints via hybrid ERC1155/ERC20 on Uniswap

- Safe [social recovery module](https://safe.global/blog/introducing-candides-social-recovery) by Candide

**Regulation/business/tokens**

- [SEC subpoena 3 crypto VCs](https://www.dlnews.com/articles/regulation/sec-subpoenas-three-crypto-vcs-as-crypto-crackdown-grows) in fishing expedition

- [SEC loses to Ripple](https://storage.courtlistener.com/recap/gov.uscourts.nysd.551082/gov.uscourts.nysd.551082.973.0.pdf): judge sets fine at $125M, SEC had asked for $2B

- New York Fed: [Tornado Cash sanctions analysis](https://www.newyorkfed.org/medialibrary/media/research/staff_reports/sr1112.pdf)

**General (Defcon edition)**

- Gubsheep: [programmable cryptography](https://0xparc.org/blog/programmable-cryptography-1)

- [Dark Skippy](https://darkskippy.com/): malicious signing device can leak secret keys in transaction signatures

- [Sinkclose](https://www.wired.com/story/amd-chip-sinkclose-flaw/) AMD CPU vulnerability, run code in System Management Mode, requires kernel access

- [GhostWrite](https://ghostwriteattack.com/) direct CPU bug in vulnerable RISC-V CPUs

- [Garuda and Pari](https://eprint.iacr.org/2024/1245): fast & small SNARKs via equifficient polynomial commitments

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-august-10-2024](https://weekinethereumnews.com/week-in-ethereum-news-august-10-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Aug 15-17 – [Ethereum Uruguay](https://www.ethereumuruguay.org/) hackathon & conference

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 23-26 – [ETHTokyo](https://www.ethtokyo.com/) hackathon & conference

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- Aug 31 – [Underhanded Solidity contest](https://soliditylang.org/blog/2024/07/31/underhanded-solidity-contest-2024-announcement/) deadline

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

- Oct 17-20 – [ETHLisbon](https://ethlisbon.org/) hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

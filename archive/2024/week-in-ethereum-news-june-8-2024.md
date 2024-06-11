---
title: "Week in Ethereum News <br> June 8, 2024"
date: "2024-06-08"
---

## Eth News and Links

**EOF** included in **Pectra upgrade**, largest upgrade ever planned (19 EIPs), likely targeting Q1 2025

**All core devs**

- [All core devs – execution (ACDE) #189](https://ethereum-magicians.org/t/all-core-devs-execution-acdc-call-189/20186):
    - **Pectra (Prague + Electra) upgrade**:
        - Prague scope finalized after 6 months (Electra still to be finalized)
        
        - **EOF** included in Pectra
            - [Nethermind](https://github.com/ethereum/pm/issues/1052#issuecomment-2152417008), [Besu](https://consensys.io/blog/besu-maintainers-on-the-pectra-fork), [EthereumJS](https://notes.ethereum.org/C2xqg0pKRW2TL7WfFqka_Q), Reth ([EOF benefits](https://hackmd.io/aZurva_kR2GQdOgJfS7B6A)) & Erigon support EOF before Verkle, Geth skeptical of upgrade size & priority of EOF
            
            - Discussed splitting Pectra, if EOF blocks Pectra move to separate upgrade
        
        - **EIP7702** included in Pectra, replaces EIP3074, iterate on revocability design
        
        - **Pectra-devnet-1:** will include interop/devnet-0 spec changes, add EIP7702 (revocability may change) but exclude EOF (work on static tests first)
    
    - **EIP158 state clearing**: EOA with EIP7702 could be empty but have storage, may need to remove EIP158 either with EIP7702 or Verkle
    
    - **EIP4444 history expiry**: client teams working on Portal network but have competing priorities
    
    - **ACD process improvements**: new EIPs to be reviewed async, EIP proposed for inclusion (PFI) status to be used in upgrade planning

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- [Future of EOA/AA breakout #4](https://ethereum-magicians.org/t/future-of-eoa-aa-breakout-room-4/20165) (EIP7702):
    - Concerns around revocability, use optional nonce unless alternative found (max nonce & nonce manager non-starters), signing address vs code discussion & [wallet best practices](https://hackmd.io/@rimeissner/eip7702-best-practices)

- Alex Stokes: [PeerDAS & raising blob count](https://hackmd.io/@ralexstokes/rJhC_vkSR), proposal to decouple layers for setting blob count and consensus clients to have maximum blob count flag for local block building

[**Osaka + F starname**](https://eips.ethereum.org/EIPS/eip-7607) **upgrade**

- [Verkle implementers call #18](https://ethereum-magicians.org/t/verkle-implementers-call-18/20226):
    - Conversion from Merkle state to Verkle took ~16 days, potential EIP158 issue with EIP7702, warming system contracts & gas cost updates to EIP4762

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.92%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~55% majority 
    
    - Consensus layer: Prysm 38%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- ePBS
    - [ePBS breakout #2](https://hackmd.io/@ttsao/epbs-breakout2): Prysm only client team to have started implementation
    
    - Terence: [out-of-protocol timelines under ePBS](https://hackmd.io/@ttsao/comp_epbs_timelines), using MEV-Boost with ePBS is worst of both worlds

- [Portal network summit](https://blog.ethportal.net/posts/2024-portal-prague): History network & Beacon network largely feature complete, State network initial phase targeting Devcon

- [Gossipsub performance](https://ethresear.ch/t/gossipsub-network-dynamicity-through-grafts-and-prunes/19750): network dynamicity through GRAFTs & PRUNEs

**Client Releases**

- Consensus layer:
    - Lodestar [v1.19.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.19.0): flood publish disabled by default, Nodejs v22 default and AMD64 & ARM64 binaries

- Execution layer:
    - Erigon [v2.60.1](https://github.com/ledgerwatch/erigon/releases/tag/v2.60.1): set tracer-observable value of a delegatecall to match parent value
    
    - Geth [v1.14.5](https://github.com/ethereum/go-ethereum/releases/tag/v1.14.5): hotfix for peer discovery; [v1.14.4](https://github.com/ethereum/go-ethereum/releases/tag/v1.14.4): 5-7% faster block import speeds, ETH supply live tracer and default minimum tip dropped to 0.001 gwei
    
    - Reth [v0.2.0-beta.9](https://github.com/paradigmxyz/reth/releases/tag/v0.2.0-beta.9): fix for docker; [v0.2.0-beta.8](https://github.com/paradigmxyz/reth/releases/tag/v0.2.0-beta.8): ensure Fork Choice Updated messages not missed when pruner active & changes to support OP mainnet

**For Stakers**

- [Anti correlation penalties](https://github.com/dapplion/anti-correlation-penalties-faq#readme) to defend solo staker viability

- Toni Wahrstätter: [MEV-Boost vs local block building](https://ethresear.ch/t/is-it-worth-using-mev-boost/19753), only small increase in APY

**Layer 2**

- Consensys [Linea](https://x.com/LineaBuild/status/1797283402745573837) paused sequencer & censored Velocore attacker addresses

- [Rollup.wtf dashboard](https://rollup.wtf/): L2 real time performance showing TPS, MGas/s & KB/s

**EIPs/Standards**

- EIPs:
    - [EIP7718](https://github.com/ethereum/EIPs/pull/8629/files): Portal Wire Protocol a framework for discv5
    
    - [EIP7719](https://github.com/ethereum/EIPs/pull/8630/files): P2P History Network

**Stuff for developers**

- Foundry adds [Vyper support](https://x.com/klkvrr/status/1799192548466167937): deploy, test, debug & write scripts

- Hardhat [v2.22.5](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.22.5): adds limited support for blob transactions & hardhat-tracer reenabled

- Slither [v0.10.3](https://github.com/crytic/slither/releases/tag/0.10.3): reduces false positives & improves performance

- [Snekmate](https://x.com/pcaversaccio/status/1798316207432401324) (Vyper building blocks): module-friendly contracts, uses Vyper v0.4.0rc6

- [Prool](https://github.com/wevm/prool/#readme): simulate local/bundler/indexer node over HTTP for TypeScript test runners e.g. Vitest

- [EVMole](https://x.com/cdump/status/1798764700718780777): improved accuracy in function argument extraction

- Contract read/write:
    - Etherscan [NatSpec comments](https://x.com/etherscan/status/1797967858816983251) used in read/write contract tab
    
    - [ABI Ninja](https://x.com/buidlguidl/status/1798369520605700429): adds proxy support, interact without an ABI & shareable link for contracts
    
    - Evm.codes [contract reader](https://x.com/smlxldotio/status/1798783588327891052)

**Security**

- Velocore (DEX) [$6.8M exploit](https://velocorexyz.medium.com/velocore-incident-post-mortem-6197020ec3e9) on zkSync & Linea via faulty logic

- [Security Alliance](https://securityalliance.notion.site/Introducing-the-First-Legal-Defense-Fund-to-Support-Crypto-Whitehats-e6792614a5b34c9f9f3f529caf975750) (SEAL) partnership with Security Research Legal Defense Fund to assist whitehats using safe harbor agreement

**Ecosystem**

- Hackathon projects: [ETH Belgrade](https://taikai.network/ethbelgrade/hackathons/eth-belgrade-hackathon-2024/projects), [ETHDublin](https://taikai.network/ethireland/hackathons/ethdubs2024/projects) & [ETHPrague](https://ethprague2024.devfolio.co/projects)

- [Devcon scholars program](https://blog.ethereum.org/2024/06/07/devcon7-scholars) for community organizers, law students/legal professionals, artists/sci-fi writers & builders, applications close July 7

- Interactive version of [Ethereum roadmap](https://ethroadmap.com/)

* * *

### Job Listings

- Nethermind: [Preconfirmations Senior Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4344191101), [Protocol Researcher](https://boards.eu.greenhouse.io/nethermind/jobs/4347537101), [Site Reliability Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4321978101), [Research Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4297652101) - Starknet & [Senior Marketing Manager](https://boards.eu.greenhouse.io/nethermind/jobs/4346942101)

- Gnosis is hiring: [Discord Moderator](https://gnosis.jobs.personio.com/job/1166297?_pc=1517287) and [Senior Web3 Software Dev (Wallet)](https://gnosis.jobs.personio.com/job/1569366?display=en&_pc=1517287)

- IMC: [Quant Developer](https://imczug.recruitee.com/o/quant-developer-defi) for DeFi and MEV focused team

- [Alchemy](https://www.alchemy.com/careers) - Wallet Services: [Engineering Manager](https://grnh.se/cc56a4365us) and [Full-Stack Engineer](https://grnh.se/5a40c3b55us)

- Privacy and Scaling Explorations: [ZK Circuits Engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4)

- ChainSafe: [Head of Protocol Engineering](https://grnh.se/c6e27e794us), [DevRel](https://grnh.se/6627a6284us) - Sygma and [more jobs](https://grnh.se/108a0afd4us)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 3.2 to 115.8 gwei, with 12.4 gwei average
    - Zero net issuance currently at 23.4 gwei 
    
    - 8k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,642 - $3,874, currently $3,686

- [ETHBTC](https://ratiogang.com/): currently 0.053 (Flippening at ~0.16)

**Notable at app layer**

- [IYK platform](https://iyk.notion.site/IYK-Platform-Changelog-4dc56c7f57974f6f8956961b76c3c3c8) public, link physical items to digital using NFC chips

**Regulation/business/tokens**

- [Stand with Crypto US](https://x.com/brian_armstrong/status/1798446241455673437) reached 1M members

- Appellate court [slaps down SEC regulatory overreach](https://storage.courtlistener.com/recap/gov.uscourts.ca5.215539/gov.uscourts.ca5.215539.123.1.pdf)

- [Evolved Apes creators charged](https://www.justice.gov/usao-sdny/pr/three-united-kingdom-nationals-charged-connection-evolved-apes-nft-scam) in alleged NFT rug pull

- [Matter Labs](https://x.com/the_matter_labs/status/1797343779189403825) (zkSync) dropping all trademark applications for ZK term

**General**

- [CoinGecko data breach](https://www.coingecko.com/learn/getresponse-data-breach-june-2024) via third-party email platform; name, email, IP & location of email opens compromised 

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-june-8-2024](https://weekinethereumnews.com/week-in-ethereum-news-june-8-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- **Jun 11 –** [**PeerDAS breakout #1**](https://github.com/ethereum/pm/issues/1059)

- Jun 14 – [EF EIP4844 data challenge](https://esp.ethereum.foundation/data-challenge-4844) deadline

- Jun 21-23 – [ETHKyiv](https://ethkyiv.org/) hackathon & conference

- **Jul 7 –** [**Devcon scholars program**](https://blog.ethereum.org/2024/06/07/devcon7-scholars) **deadline**

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

- Sep 13-14 – [Ethereum México](https://x.com/ethereum_mexico/status/1792677234324767081)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Sep 26-27 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 4-6 – [Ethereum Kuala Lumpur](https://www.2024.ethkl.org/) conference & hackathon

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

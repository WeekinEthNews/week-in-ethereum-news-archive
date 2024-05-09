---
title: "Week in Ethereum News <br> May 4, 2024"
date: "2024-05-04"
---

## Eth News and Links

**Pectra (Prague + Electra) upgrade (meta** [**EIP7600**](https://eips.ethereum.org/EIPS/eip-7600)**)**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=LazOhUu1Tew&t=160s). Recap from [Alex Stokes](https://twitter.com/abcoathup/status/1786133901477335094).  Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-133/):
    - [**Confirmation rule**](https://arxiv.org/abs/2405.00549) **research**: algorithm determines if block always in canonical chain
    
    - [**Pectra-devnet-0**](https://notes.ethereum.org/@ethpandaops/pectra-devnet-0#Client-implementation-tracker): plan to launch in ~10 days, client teams making good progress, attestation refactoring for EIP7549 taking extra time
    
    - **EIP7684 return deposits for distinct credentials**: proposal to mitigate deposit front-running for staking pools
    
    - **PeerDAS**: client teams making progress, synchrony assumption on sampling discussion

- consensus-specs/releases [v1.5.0-alpha.1](https://github.com/ethereum/consensus-specs/releases/tag/v1.5.0-alpha.1): CL spec target of pectra-devnet-0, bug fixes for test cases & new fork tests

- EIP2537 BLS12 precompile [benchmarks](https://ethereum-magicians.org/t/eip-2537-bls12-precompile-discussion-thread/4187/76)

- [Future of EOA/AA breakout call #2](https://github.com/ethereum/pm/issues/1032) scheduled for May 7
    - Yoav Weiss: [Account Abstraction roadmap](https://notes.ethereum.org/@yoav/AA-roadmap-May-2024), towards native AA starting with L2

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.68%**](https://dune.com/hildobby/eth2-staking) **still too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~63% majority
    
    - Consensus layer: Prysm 38%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- [Erigon](https://twitter.com/erigoneth/status/1785598455571796348) switching development to v3

- [Slashing Proofoor](https://ethresear.ch/t/slashing-proofoor-on-chain-slashed-validator-proofs/19421): prove a validator hasn’t been slashed using EIP4788 beacon block root in EVM

- Terence: [builder reveal timing game](https://ethresear.ch/t/builder-reveal-timing-game-in-epbs/19424) post ePBS

**Client Releases**

- Consensus layer:
    - Nimbus [v24.4.0](https://github.com/status-im/nimbus-eth2/releases/tag/v24.4.0): stability & performance improvements

- Execution layer:
    - Erigon
        - Otterscan [v2.5.0 alpha](https://github.com/otterscan/otterscan/releases/tag/v2.5.0): improved Optimism support

**For Stakers**

- [Teku adds client info to graffiti](https://mirror.xyz/0x65a63ceE206bFA6B2a3287479D28c8902B4055E9/8u3oxjWyAU1JVBhu7U1y0luO5hRBXFj1Plrby-X1kMI): appends client types & versions to improve client diversity data, opt-out

**Layer 2**

- Lattice [Redstone](https://lattice.xyz/blog/start-your-engines-redstone-live) live, uses [Plasma mode](https://specs.optimism.io/experimental/plasma.html) offchain data availability

**EIPs/Standards**

- EIPs:
    - [EIP7701](https://github.com/ethereum/EIPs/pull/8516/files): Native account abstraction with EOF

- ERCs (application layer):
    - [ERC7700](https://github.com/ethereum/ERCs/pull/404/files): Cross-chain storage router protocol 

**Stuff for developers**

- [EIP5792 site](https://eip5792.xyz/) (wallet call API): API reference, capabilities & ecosystem support

- Wagmi [v2.8.0](https://github.com/wevm/wagmi/releases/tag/wagmi%402.8.0): adds experimental EIP5792 actions & hooks

- [Reth Execution Extensions](https://www.paradigm.xyz/2024/05/reth-exex) (ExEx): post-execution hooks for building offchain infrastructure

**Security**

- Pike [~$2M in two exploits](https://mirror.xyz/pikefinance.eth/klLV4rRqNYxjRQp0NAfVLboLYtX98P9iYOOf06FUapg), first via weak security handling of cross-chain transfer protocol transfers (identified by auditor) and second via faulty upgrade to pause the protocol

- [DeFi risk modeling](https://blog.yacademy.dev/2024-05-03-merging-economics-and-security/): security implications of economic research 

**Ecosystem**

- Ethereum reached [1 million validators](https://twitter.com/terencechain/status/1784789672759279661)

* * *

### Job Listings

- [stakefish](https://stake.fish/): [DevOps Engineer](https://apply.workable.com/stakefish/j/8FC077923F/) & [Full-stack Engineer](https://apply.workable.com/stakefish/j/5218ED958E/)

- Devcon: [Production Magician](https://jobs.lever.co/ethereumfoundation/aa4c69f8-f564-4036-9c5e-3e09f0eb27df) & [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/e93dae67-65a6-495c-8638-46e3db28cb64)

- ChainSafe: [Head of Protocol Engineering](https://grnh.se/c6e27e794us) and [Developer Relations - Sygma](https://grnh.se/6627a6284us)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 3.4 to 91.4 gwei, with 8.4 gwei average
    - Zero net issuance currently at 23.2 gwei 
    
    - 11k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,859 - $3,342, currently $3,102

- [ETHBTC](https://ratiogang.com/): currently 0.049 (Flippening at ~0.16)

**Notable at app layer**

- [Fantasy.top](http://fantasy.top) (CryptoTwitter fantasy sports game) live on Blast.
    - If you [need a signup code](https://twitter.com/evan_van_ness/status/1785757716549349748)

- [Friendtech v2](https://chronicle.castlecapital.vc/p/friend-tech-v2-opportunity-bloodbath): adds clubs & $friend airdrop

- Eigen [token](https://blog.eigenfoundation.org/announcement/), non-transferable & airdrop geoblocked after allowing deposits from those countries

- [Aave proposed roadmap](https://governance.aave.com/t/temp-check-aave-2030/17539): v4, cross-chain liquidity layer, real world asset products built around GHO stablecoin and Aave network

- [Paragraph](https://dev.mirror.xyz/_JH3B2prRmU23wmzFMncy9UOmYT7mHj5wdiQVUolT3o) acquires Mirror

- DefiLama [airdrops](https://defillama.com/airdrops): check any address, no signing or signup required

- [Gitcoin Grants](https://ggwrapped.gitcoin.co/) donation history for an address

- A look at [yields in DeFi](https://mirror.xyz/nexusmutant.eth/x2upCQnePe6KIzSAkpPpYKrCtfGUbo79WmzGnNjta7A) this week

**Regulation/business/tokens**

- Former Binance CEO [CZ sentenced](https://twitter.com/nikhileshde/status/1785383646394024380) to four months prison

- [ENS](https://twitter.com/ensdomains/status/1786045291365638621) challenge Unstoppable Domains patent

**General**

- Vitalik: [Binius](https://vitalik.eth.limo/general/2024/04/29/binius.html), efficient proofs over binary fields

- [Dutch arrest](https://www.fiod.nl/12-million-seized-and-arrested-in-investigation-into-gambling-platform-scam/) ZKasino rugpuller

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-may-4-2024](https://weekinethereumnews.com/week-in-ethereum-news-may-4-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- May 7 – [Gitcoin Grants 20](https://grants.gitcoin.co/) ends

- May 10-11 – [ETH Bratislava](https://www.ethbratislava.com/) conference & hackathon

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

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 23-26 – [ETHTokyo](https://www.ethtokyo.com/) hackathon & conference

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- Sep 5-8 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 9-15 – [ETHSafari](https://ethsafari.xyz/) (Kenya)

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- **Sep 26-27 –** [**ETHMilan**](https://www.ethmilan.xyz/) **conference**

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

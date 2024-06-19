---
title: "Week in Ethereum News <br> June 15, 2024"
date: "2024-06-15"
---

## Eth News and Links

Electra upgrade scope not finalized yet, Devcon ticket dates and Curve liquidations

**All core devs**

- [**All core devs – consensus (ACDC) #135**](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-call-135/20284):
    - **Pectra (Prague + Electra) upgrade**:
        - **pectra-devnet-1**: consensus layer client teams expect to be ready in 1-2 weeks and agreed to append committee bits field to end of attestation 
        
        - **EIP7594 PeerDAS**: building on top of Deneb upgrade for now rather than Electra, aim for peerdas-devnet-1 in 2 weeks
        
        - **Blob count increase**: discussion on increase with/without PeerDAS or PeerDAS without an increase, needs analysis on devnets and proposal to uncouple blob count from execution layer
        
        - **SSZ:** EIP7688 change to SSZ StableContainer: devnet planned before next ACDC to help decide whether or not to include in Pectra
    
    - [Naming F-starname upgrade discussion](https://ethereum-magicians.org/t/f-star-name-for-consensus-layer-upgrade-after-electra/20285) for upgrade after Electra

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade, likely targeting Q1 2025**

- Consensus-specs [v1.5.0-alpha.3](https://github.com/ethereum/consensus-specs/releases/tag/v1.5.0-alpha.3): specs for pectra-devnet-1

- [PeerDAS breakout #1](https://ethereum-magicians.org/t/peerdas-breakout-1/20275): client implementation progress, proposal to move max blobs to config & uncouple blob count from execution layer, keep activation logic same for devnet-1 and bandwidth concerns for home stakers

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.75%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~55% majority 
    
    - Consensus layer: Prysm 38%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Toni Wahrstätter: [MEV-Boost users are reorged less](https://ethresear.ch/t/blobs-reorgs-and-the-role-of-mev-boost/19783) & can better handle 6 blob blocks compared with non MEV-Boost users but they include less blobs as not incentivized

- Parithosh: [proposal to use torrents for distributing pre-merge data](https://ethresear.ch/t/torrents-and-eip-4444/19788) (EIP4444 history expiry)

- Vitalik: [inclusion list proposal](https://ethresear.ch/t/one-bit-per-attester-inclusion-lists/19797) using one-bit-per-attester

- Potuz: [preconfirmation designs](https://ethresear.ch/t/the-contention-between-preconfs-and-epbs/19770) compatibility with proposed ePBS

**Client Releases**

- Consensus layer:
    - Lighthouse [v5.2.0](https://github.com/sigp/lighthouse/releases/tag/v5.2.0): adds in-memory [tree-states](https://x.com/sproulM_/status/1800419983648002148), optimized epoch & block processing and execution client version in graffiti

- Execution layer:
    - Besu [v24.6.0](https://github.com/hyperledger/besu/releases/tag/24.6.0): Java v21 now minimum version and historic trie log data removed by default

**For Stakers**

- Reth + Prysm [archive node on $189 NanoPC-T6 board](https://x.com/ethereumonarm/status/1800436894418805198) using ~10w

- [Lighthouse attestation simulator](https://lighthouse-blog.sigmaprime.io/attestation-sim.html): Prometheus metrics for use with Grafana to track Beacon Node performance; suggests running in APAC impacts performance

**Layer 2**

- OP Stack [fault proofs](https://optimism.mirror.xyz/izdAoJ8ooyhDfwFLFoCcUfB1icPLFn8AImBws4oaqw8) live on OP mainnet, now a stage 1 L2 (limited training wheels)

- [RIP7212 secp256r1 precompile](https://getclave.notion.site/2295a4513abe46f5a49a41097b88def0) deployment status on L2s

- ZKsync [airdrop](https://blog.zknation.io/zk-token/), GitHub users need to associate an address

- [Based preconfs](https://x.com/drakefjustin/status/1801321889152835758) live on devnet

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - Meta [EIP7723](https://github.com/ethereum/EIPs/pull/8662/files): Network upgrade inclusion stages

- RIPs (rollup improvement proposals):
    - [RIP7724](https://github.com/ethereum/RIPs/pull/26/files) (clone of EIP7667 for zk rollups): Raise gas costs of hash functions

- ERCs (application layer standards):
    - [ERC838](https://github.com/ethereum/ERCs/pull/477/files) (resurrected): ABI specification for REVERT reason string
    
    - [ERC7720](https://ercs.ethereum.org/ERCS/erc-7720): Deferred token transfer (ERC20)
    
    - [ERC7721](https://github.com/ethereum/ERCs/pull/466/files): Lockable extension for ERC1155
    
    - [ERC7722](https://github.com/ethereum/ERCs/pull/468/files): Opaque token

**Stuff for developers**

- Foundry [show-progress flag](https://x.com/lucasmanuel_eth/status/1801353643410530393): live progress of fuzz & invariant tests

- Remix [v0.50](https://medium.com/remix-ide/remix-release-v0-50-0-1b0ca47ce2d9): QuickDapp plugin to create basic front end for contracts

- [Quantifying code complexity](https://medium.com/@devtooligan/quantifying-complexity-in-smart-contracts-the-adventures-of-uncle-bob-and-the-clean-code-crew-099bb2b5b397): CK, Martin & Halstead metrics using Slither printers

- Guide to [create a simple Solidity linter using Slang](https://blog.nomic.foundation/how-to-write-your-own-solidity-linter-using-slang-356e7565ad1b) (Nomic Foundation’s compiler APIs)

- RareSkills: [ERC7201 namespaced storage layout](https://www.rareskills.io/post/erc-7201) explainer

- [Scaffold-ETH-Svelte](https://github.com/ByteAtATime/scaffold-eth-svelte/#readme): Scaffold-ETH v2 port to Svelte

- [EF JavaScript team](https://docs.google.com/presentation/d/1ya-SlYR6WdnQ0oMqbeCl2FH75j_zMLcnB87jwmoAgwU/edit) roadmap

- Data Always [PBS snapshot](https://github.com/dataalways/pbs-snapshot#readme) (Python script): create MEV data snapshots

**Security**

- UwU (Aave v2 fork) [$23M exploit](https://rekt.news/uwulend-rekt/) via oracle manipulation
    - A further [$3.7M stolen](https://x.com/BarryFried1/status/1801234097303437699) after unpausing protocol

- [Loopring smart wallet exploit](https://x.com/loopringorg/status/1799791898296451515) via compromised 2FA service for wallets with only the Loopring guardian

**Ecosystem**

- [Devcon tickets & tracks](https://blog.ethereum.org/2024/06/11/devcon7-ticket-detail):
    - Ticket raffle/auction starts June 18, discount applications open July 9 & general admission waves start July 16
    
    - Speaker applications open July 9

- Clr.fund [Southeast Asian Ethereum communities](https://blog.ethereum.org/2024/06/14/devcon7-qf-sea) quadratic funding round

* * *

### Job Listings

- ChainSafe: [Head of Protocol Engineering](https://grnh.se/c6e27e794us), [DevRel](https://grnh.se/6627a6284us) - Sygma and [more jobs](https://grnh.se/108a0afd4us)

- [Alchemy](https://www.alchemy.com/careers) - Wallet Services: [Engineering Manager](https://grnh.se/cc56a4365us) and [Full-Stack Engineer](https://grnh.se/5a40c3b55us)

- Gnosis is hiring: [Discord Moderator](https://gnosis.jobs.personio.com/job/1166297?_pc=1517287) and [Senior Web3 Software Dev (Wallet)](https://gnosis.jobs.personio.com/job/1569366?display=en&_pc=1517287)

- IMC: [Quant Developer](https://imczug.recruitee.com/o/quant-developer-defi) for DeFi and MEV focused team

- Privacy and Scaling Explorations: [ZK Circuits Engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4)

- Nethermind: [Preconfirmations Senior Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4344191101), [Protocol Researcher](https://boards.eu.greenhouse.io/nethermind/jobs/4347537101), [Site Reliability Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4321978101), [Research Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4297652101) - Starknet & [Senior Marketing Manager](https://boards.eu.greenhouse.io/nethermind/jobs/4346942101)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 2.4 to 104.0 gwei, with 10.7 gwei average
    - Zero net issuance currently at 23.5 gwei 
    
    - 9.7k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,367 - $3,713, currently $3,480, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.053 (Flippening at ~0.16)

**Notable at app layer**

- Curve co-founder [Michael Egorov liquidated](https://x.com/newmichwill/status/1801255607137165390), triggered by UwU exploit, causing ~$10M of bad debt which he has already repaid

- [100x](https://medium.com/100xfinance/introducing-100x-b86bb13fbe6a) (perps) live on Blast, up to 20x leverage on ETH & BTC, with Blast gold for orderbook liquidity \[[Starbloom](https://twitter.com/starbloomvent) portfolio\]

- [Uniswap Labs](https://x.com/uniswap/status/1800196800684732423) acquired Crypto: The Game (onchain Survivor)

**Regulation/business/tokens**

- SEC Chair Gensler “envision\[s\]” [spot ETH ETFs S-1s to be approved](https://x.com/evan_van_ness/status/1801303162848219569) over US summer but dodges question of whether ETH is a commodity

- [Alex Pertsev attempting to be released](https://www.dlnews.com/articles/regulation/tornado-cash-dev-alexey-pertsev-battles-to-get-out-of-jail) while he appeals

**General**

- Privacy and Scaling Explorations trusted setup ceremonies via a browser:
    - [Anon Aadhaar v2](https://x.com/AnonAadhaar/status/1800209133477720564)
    
    - [Semaphore V4](https://x.com/privacyscaling/status/1800478650200166866) phase 2

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-june-15-2024](https://weekinethereumnews.com/week-in-ethereum-news-june-15-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- **Jun 21 –** [**EF EIP4844 data challenge**](https://esp.ethereum.foundation/data-challenge-4844) **extended deadline**

- Jun 21-23 – [ETHKyiv](https://ethkyiv.org/) hackathon & conference

- Jul 7 – [Devcon scholars program](https://blog.ethereum.org/2024/06/07/devcon7-scholars) deadline

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 29-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 2-4 – [Ethereum Argentina](https://ethereumargentina.org/) conference & hackathon

- **Aug 7-9 –** [**Science of Blockchain Conference**](https://www.sbc-conference.com/) **(New York)**

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

---
title: "Week in Ethereum News <br> March 30, 2024"
date: "2024-03-29"
---

## Eth News and Links

**Pectra (Prague + Electra) upgrade (meta** [**EIP7600**](https://eips.ethereum.org/EIPS/eip-7600)**)**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=cSQmbCVwGUk&t=86s).  Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1773421360112635964) & [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-184/):
    - **Missed slots**: blocks gossiped with missing blobs, circuit breaker to local building not triggered, base fee variability due to EIP1559 being block rather than time based
        - bloXroute [post mortem](https://gist.github.com/benhenryhunter/687299bcfe064674537dc9348d771e83): resolved by disabling propagation of blocks containing blobs via their distribution network
    
    - **State & history growth**:
        - [Paradigm research](https://docs.google.com/presentation/d/12qF9RnyQiY5jNA0ZEoZssbncZ8i3lpeLd8lhANs3M2w/edit#slide=id.p): history is 10x state growth
        
        - Continue work on EIP4444 (history expiry) & provide downloadable history so can stop serving on p2p
    
    - **Retroactive EIPs:** agreed to include EIP7610 (revert contract creation for non-empty storage) and EIP7523 (deprecate empty accounts)
    
    - **Pectra upgrade** (small fork targeting late 2024)
        - **EIP2537 BLS precompile:** [gas cost benchmarks](https://notes.ethereum.org/@MariusVanDerWijden/BkdJeFWJC)
        
        - **Candidate for inclusion**:
            - **EIP7547 IL**: design issue with account abstraction & options to mitigate
        
        - **Potential EIP updates** (no decisions yet, client teams to review, aim to decide scope at ACDE in 2 weeks)
            - EIP5920 PAY opcode
            
            - EIP7609 decrease cost of TSTORE/TLOAD
            
            - EIP2935 save historical block hashes in state
            
            - EIP7545 Verkle proof verification precompile
            
            - EOF (Ethereum Object Format)
            
            - RIP7212 secp256r1 precompile
            
            - EIP7664 Access-Key opcode
            
            - EIP6493 SSZ transaction signature scheme 

- EIP7251 maxEB (increase max effective balance):
    - Breakout [call video](https://www.youtube.com/watch?v=cGcjxna5HSg) & [notes](https://hackmd.io/@philknows/BJCaLJf1A)
    
    - [Inactivity leak](https://lighthouse-blog.sigmaprime.io/maxeb-inactivity-leak.html) under maxEB: ejection balance should remain as 16 ETH

- EIP7547 IL (inclusion lists):
    - Potuz: [inclusion lists & EIP3074 incompatibilities](https://hackmd.io/@potuz/BkWngLly0)

**Osaka + F starname upgrade (meta** [**EIP7607**](https://eips.ethereum.org/EIPS/eip-7607)**)**

- Verkle:
    - Implementers [call video](https://www.youtube.com/watch?v=sMbCzWyCqPg) & [notes](https://twitter.com/rudolf6_/status/1773494895233335759)
    
    - [Verkle from genesis devnet-5](https://verkle-gen-devnet-5.ethpandaops.io/) live

* * *

**This newsletter is sponsored by** [**Pashov Audit Group**](https://www.pashov.net/)**!** 

![Pashov Audit Group](https://weekinethereumnews.com/wp-content/uploads/2024/03/Pashov-Audit-Group-1024x341.webp)

What if you can get a good security review from elite security researchers _without spending a single penny_? 

We offer a FREE **pre-audit review**on your code.

Our review will check for common vulnerabilities and suggest best practices to ensure that your codebase will get the most out of an audit.  

We bet that this free service is better than some that cost 5 figures on the market.

We will be offering this service forever, but if you ping in the following 72hrs after the newsletter is out, you get a guaranteed high priority for reviewing your code. Reach out - [t.me/pashovkrum](https://t.me/pashovkrum)

* * *

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 30.11%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth 66% majority
    
    - Consensus layer: Prysm 38% plurality
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- [Erigon++](https://erigon.tech/erigonpp/): Silkworm (C++ block execution, RPC & p2p using evmone) running inside Erigon, enabled by command line flag(s), experimental

- [MEV-Boost min-bid provides 7% of censorship resistance](https://hackmd.io/@dataalways/resilience): changing to opt-out is simpler alternative to inclusion lists

**Client Releases**

- Consensus layer:
    - Lighthouse [v5.1.3](https://github.com/sigp/lighthouse/releases/tag/v5.1.3): hotfix for duplicate lookup requests and to run fork choice after all block imports
    
    - Prysm [v5.0.2](https://github.com/prysmaticlabs/prysm/releases/tag/v5.0.2): optimizations, UX improvements & bug fixes; defaults to local block if external builder less than 10% additional value
    
    - Nimbus [v24.3.0](https://github.com/status-im/nimbus-eth2/releases/tag/v24.3.0): additional beacon API support, reduces CPU usage & improves resilience; defaults to local block if external builder less than 10% additional value
    
    - Teku [v24.3.1](https://github.com/Consensys/teku/releases/tag/24.3.1): reduces CPU & bandwidth usage; defaults to local block if external builder less than 10% additional value

- Execution layer:
    - Erigon [v2.59.2](https://github.com/ledgerwatch/erigon/releases/tag/v2.59.2): patch for MDBX size/performance regression introduced in v2.58.0
    
    - Reth [v0.2.0-beta.4](https://github.com/paradigmxyz/reth/releases/tag/v0.2.0-beta.4): performance & storage improvements

**Research**

- Vitalik: [extend anti-correlation incentives](https://ethresear.ch/t/supporting-decentralized-staking-through-more-anti-correlation-incentives/19116) to support decentralized staking

- [Out-of-protocol blob inclusion pre-confirmations](https://ethresear.ch/t/blob-preconfirmations-with-inclusion-lists-to-mitigate-blob-contention-and-censorship/19150) to mitigate blob contention & censorship

**Layer 2**

- Base [gas target increased to 3.75mgas/s](https://twitter.com/jessepollak/status/1773085753850925073), planning increase to 5 mgas/s next week

- [Polygon zkEVM outage](https://forum.polygon.technology/t/polygon-zkevm-recent-network-outage-report/13702): synchronizer didn’t detect mainnet reorg, emergency state approved by Security Council to upgrade network

- Based sequencing & pre-confirmations [call video](https://www.youtube.com/watch?v=IsYISmTmPmQ) & [notes](https://docs.google.com/document/d/1hWJU20EwQT3K3uB3GiwDsFlsK3uKuJX20noAN7ZqreA/edit#heading=h.u40p2e7q3vvz)

**EIPs/Standards**

- EIPs:
    - [EIP7664](https://github.com/ethereum/EIPs/pull/8357/files): Access-Key opcode
    
    - Vitalik’s draft EIPs:
        - [Remove identity precompile](https://notes.ethereum.org/@vbuterin/evmify_identity)
        
        - [Raise gas costs of hash functions](https://notes.ethereum.org/@vbuterin/raise_hash_gas_costs)
        
        - [Remove bloom filters](https://notes.ethereum.org/@vbuterin/remove_blooms)

- ERCs (application layer):
    - [ERC7660](https://github.com/ethereum/ERCs/pull/347/files): Release tokens on predefined periods
    
    - [ERC7661](https://github.com/ethereum/ERCs/pull/344/files): Extended multiphase fractional NFTs
    
    - [ERC7662](https://github.com/ethereum/ERCs/pull/348/files): AI agent NFTs

**Stuff for developers**

- Remix [v0.46.0](https://medium.com/remix-ide/remix-release-v0-46-0-f90a4948fff0): defaults Remix VM EVM version to Cancun & Solidity compiler to v0.8.25

- [BidDog](https://github.com/Bunniapp/biddog#readme) (Solidity): auction managed AMM, AGPL-3.0

- Gaslite Drop [deploy ERC20 token](https://drop.gaslite.org/deploy/erc20) using Bytecode20 ([currently can’t verify on Etherscan](https://twitter.com/poppunkonchain/status/1773772944373682674))

- web3.py [WebSocketProvider](https://snakecharmers.ethereum.org/websocketprovider/) in v7 beta

- Lattice MUD [v2](https://lattice.xyz/blog/mud-2-is-ready) (game framework): adds Store (runtime defined storage) & World (contract framework) 

- Curta CTF [number heist solution](https://hackmd.io/@billh/Curta-NumberHeist)

- EthPandaOps [Xatu dataset](https://ethpandaops.io/posts/open-source-xatu-data/) available in Parquet format for mainnet and Sepolia & Holešky testnets

**Security**

- Munchables [$62M exploit](https://rekt.news/munchables-rekt/) on Blast by rogue dev, funds returned to multisig

- Prisma Finance [$11.6M exploit](https://rekt.news/prismafi-rekt/) via unvalidated input, [revoke delegate approvals](https://twitter.com/PrismaFi/status/1773426990114062497)

- Curio [$113k exploit](https://investcurio.medium.com/curiodaos-recovery-plan-1255427f35de) on mainnet via flawed voting power access control

- Baseline on Blast [vulnerability disclosed](https://twitter.com/plotchy/status/1773426302089109711) 

**Ecosystem**

- Vitalik: [Ethereum after blobs](https://vitalik.eth.limo/general/2024/03/28/blobs.html), L1 progress less disruptive for apps, scaling work in the background, apps need to be built for 2020s Ethereum workflow (e.g. on L2, private & with account abstraction)

- [EIP7503 (zk wormholes)](https://ethereum2077.substack.com/p/eip-7503-zero-knowledge-wormholes) explainer: mechanism for privacy-preserving transfers

- Hackathon projects: [ETHTaipei](https://taikai.network/ethtaipei/hackathons/hackathon-2024/projects) & [ETHSamba](https://taikai.network/ethsamba/hackathons/ethsambahack-2/projects)

- Optimism [Retro Funding](https://gov.optimism.io/t/upcoming-retro-rounds-and-their-design/7861) (expanded from public goods) experimenting with impact juries & metrics based evaluation for focused rounds: onchain builders, OP Stack, governance & dev tooling

**Enterprise**

- [Google search](https://twitter.com/rajanpatel/status/1772804743745921131) for an address shows balance on Arbitrum One & OP Mainnet as well as mainnet

* * *

### Job Listings

- Nethermind [Mechanism Designer](https://grnh.se/e78eb182teu), [Protocol Research Manager](https://grnh.se/8f2a6c32teu), [Research Engineer](https://grnh.se/887df932teu)

- Devcon: [Community Supporter](https://jobs.lever.co/ethereumfoundation/6ad3d8e7-17cb-4d5c-820d-c279e8002551), [Production Magician](https://jobs.lever.co/ethereumfoundation/aa4c69f8-f564-4036-9c5e-3e09f0eb27df) & [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/e93dae67-65a6-495c-8638-46e3db28cb64)

- Certora is hiring: [Head of Product](https://hubs.ly/Q02n-d-X0), [SR-Rust](https://hubs.ly/Q02n-fmD0), [Compiler Developer](https://hubs.ly/Q02n-b_20) & [FV Wizard](https://hubs.ly/Q02n-fyx0)

- 🔥OpenZeppelin seeks Security Researchers in [Canada](https://grnh.se/3d8f61e53us), [Australia](https://grnh.se/bb2348b83us), [LatAm](https://grnh.se/3b4915233us) & [USA](https://grnh.se/54d2bd163us)

- [Waku](https://waku.org/about) is hiring! [Protocol Engineer](https://grnh.se/a240b11b1us), [Waku SDK Software Engineer](https://grnh.se/0a63ae031us) & [Researcher](https://grnh.se/b96ad7111us)

- [IFT](https://free.technology/)/[Logos](https://logos.co/): [ZK Researcher](https://boards.greenhouse.io/nomos/jobs/5664663) (Nomos); [ZK Researcher](https://boards.greenhouse.io/vac/jobs/5453093) (Vac) & [ZK Engineer](https://boards.greenhouse.io/vac/jobs/5543856) x2

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 11.2 to 105.5 gwei, with 26.5 gwei average
    - Zero net issuance currently at 22.6 gwei 
    
    - 3k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,303 - $3,664, currently $3,523

- [ETHBTC](https://ratiogang.com/): currently 0.05 (Flippening at ~0.16)

**Notable at app layer**

- [Blobs](https://dune.com/hildobby/blobs) being used for inscriptions, activating blob fee market

- Splits [multichain](https://splits.org/blog/multichain/): single view of activity across mainnet & Layer 2

- Privacy & Scaling Explorations: [Anon Aadhaar v2](https://twitter.com/anonaadhaar/status/1773732144151486864) adds selective disclosure & simplified nullifier

- [Crypto: The Game](https://www.cryptothegame.com/) (onchain Survivor) season 2 starts April 2, players/jury represented as NFTs

**Regulation/business/tokens**

- [Alex Pertsev's 2 day trial completed](https://www.dlnews.com/articles/people-culture/tornado-cash-dev-alexey-pertsev-cant-comprehend-prosecution/) in Netherlands, verdict expected May 14

- [SBF](https://twitter.com/innercitypress/status/1773340043744010640) sentenced to 25 years

- [KuCoin](https://www.justice.gov/usao-sdny/pr/prominent-global-cryptocurrency-exchange-kucoin-and-two-its-founders-criminally) charged with bank secrecy act & unlicensed money transmission offenses

- [Beba](https://twitter.com/BebaCollection/status/1773165078918905897) (apparel) sued SEC, claims free airdrop is not a securities transaction

- [ETH correlation analysis](https://twitter.com/BitwiseInvest/status/1773427635919458551) in spot ETH ETF filing: strong correlation between spot & futures market

**General**

- Vitalik: [memecoins](https://vitalik.eth.limo/general/2024/03/29/memecoins.html) for public goods & creating games/fun

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-march-30-2024](https://weekinethereumnews.com/week-in-ethereum-news-march-30-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) virtual hackathon

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Apr 12-14 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- Apr 16-18 – [EY Global blockchain summit](https://web.cvent.com/event/e0ad2c12-3e65-41a9-bafb-a436754cf4ae/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7) (London)

- Apr 19-21 – [ETH Tallinn](https://www.ethtallinn.org/) hackathon

- **Apr 20-21 –** [**ETHDubai**](https://www.ethdubaiconf.org/) **conference & hackathon**

- Apr 23-May 7 – [Gitcoin Grants 20](https://twitter.com/gitcoin/status/1772698797723774991) **(applications open Apr 2-16)**

- Apr 26-28 – [ETHBoston](https://ethboston.xyz/) hackathon & conference

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- **May 10-11 –** [**ETH Bratislava**](https://www.ethbratislava.com/) **conference & hackathon**

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/) hackathon

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- May 31-Jun 5 – [ETH Belgrade](https://ethbelgrade.rs/) hackathon & conference

- Jun 14 – [EF EIP4844 data challenge](https://esp.ethereum.foundation/data-challenge-4844) deadline

- **Jun 21-23 –** [**ETHKyiv**](https://www.ethkyiv.org/) **hackathon & conference**

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 26-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- **Aug 23-26 –** [**ETHTokyo**](https://www.ethtokyo.com/) **hackathon & conference**

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- **Sep 5-8 –** [**ETHWarsaw**](https://www.ethwarsaw.dev/) **conference & hackathon**

- **Sep 9-15 –** [**ETHSafari**](https://ethsafari.xyz/) **(Kenya)**

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- **Oct 4-6** – [ETHRome](https://ethrome.org/)

- **Oct 17-19 –** [**ETHSofia**](https://www.ethsofia.com/) **hackathon & conference**

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

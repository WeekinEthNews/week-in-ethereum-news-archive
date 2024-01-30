---
title: "Week in Ethereum News <br> January 27, 2024"
date: "2024-01-26"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- [Final public testnets](https://blog.ethereum.org/2024/01/24/sepolia-holesky-dencun) upgrade to Dencun Jan 30 (Sepolia) & Feb 7 (Holešky)
    - Lightweight beaconcha.in explorers: [mainnet](https://light-mainnet.beaconcha.in), [Holešky](https://light-holesky.beaconcha.in) & [Sepolia](https://light-sepolia.beaconcha.in)

- L2s testing blobs:
    - RollCall (L2 standards) [EIP4844 readiness call](https://www.youtube.com/watch?v=V8d0fQoMeP4): L2s testing on Goerli or waiting for Sepolia & improving communications with core devs
    
    - [OP & Base devnets](https://twitter.com/roberto_bayardo/status/1750598068326822032) posting batches via blobs on Goerli testnet
    
    - [Starknet](https://twitter.com/dimahledba/status/1750459892039565685) sent state diff blob on Goerli testnet

- Dencun interop testing [call video](https://www.youtube.com/watch?v=wiOGbAPL144&t=208s): high memory usage after blob spamming, max churn limit (EIP7514) will be tested on Goerli and first blobs expire on Goerli Feb 5

- EF DevOps [Attacknet](https://notes.ethereum.org/@ethpandaops/attacknet-planning): chaos testing tooling, plan to open source after Dencun

**Pectra (Prague + Electra) upgrade (meta** [**EIP7600**](https://github.com/ethereum/EIPs/pull/8121/files)**)**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=_pFRJ1it608&t=227s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-126/):
    - Electra upgrade scope (small cross layer fork targeting late 2024):
        - **Client team priorities**: [Lighthouse](https://hackmd.io/@dapplion/lighthouse_pectra), [Lodestar](http://blog.chainsafe.io/lodestar-proposals-for-next-electra-cancun-fork) & [Prysm](https://medium.com/offchainlabs/prysm-electra-upgrade-f827c20d0fd2)
        
        - **Electra EIPs**: EIP6110 (validator deposits onchain), EIP7002 (EL triggerable exits) & EIP7549 (move committee index outside attestation)
        
        - **Not in Electra**: EIP6914 (reuse validator indices)
        
        - **Discussions ongoing**: EIP7251 (increase max effective balance), EIP7547 (inclusion lists), EIP7594 (PeerDAS) & SSZification EIPs

**Client releases for Sepolia & Holešky testnets Dencun upgrade**

- Consensus layer:
    - Lighthouse [v4.6.0](https://github.com/sigp/lighthouse/releases/tag/v4.6.0)
    
    - Lodestar [v1.15.0-rc.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.15.0-rc.0)
    
    - Nimbus [v24.1.2](https://github.com/status-im/nimbus-eth2/releases/tag/v24.1.2)
    
    - Prysm [v4.2.1-rc.2](https://github.com/prysmaticlabs/prysm/releases/tag/v4.2.1-rc.2)
    
    - Teku [v24.1.1](https://github.com/Consensys/teku/releases/tag/24.1.1)

- Execution layer:
    - Besu [v24.1.1](https://github.com/hyperledger/besu/releases/tag/24.1.1)
    
    - Erigon [v2.57.1](https://github.com/ledgerwatch/erigon/releases/tag/v2.57.1)
    
    - Geth [v1.13.11](https://github.com/ethereum/go-ethereum/releases/tag/v1.13.11)
    
    - Nethermind [v1.25.3](https://github.com/NethermindEth/nethermind/releases/tag/1.25.3)
    
    - Reth [v0.1.0-alpha.16](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.16)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.84%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth 78% supermajority, could cause a chain split & [lose your staked ETH](https://labrys.io/insights/geth-staking)
        - [Allnodes](https://twitter.com/Allnodes/status/1750519886286295117) & [P2P](https://twitter.com/p2pvalidator/status/1750550082934472885) migrated to Besu
        
        - [Lido](https://twitter.com/LidoFinance/status/1749860092885819577) & [Kiln](https://twitter.com/kiln_finance/status/1750195042587685031) reducing Geth usage
        
        - [Coinbase](https://twitter.com/coinbasecloud/status/1749614211532198311) & [Kraken](https://twitter.com/matthewbarby/status/1749826741302866165) “taking a look” at client diversity
    
    - Consensus layer: Prysm 39%, any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Nethermind [mainnet consensus issue](https://github.com/NethermindEth/nethermind/issues/6588) on Jan 21, v1.23-1.25 were affected, [patched](https://twitter.com/NethermindEth/status/1749508268676764118)

- [Data viz](https://ethresear.ch/t/on-block-sizes-gas-limits-and-scalability/18444) on whether we can increase the gas limit

- [Validator in-protocol consolidation](https://notes.ethereum.org/@fradamt/maxeb-consolidation) in EIP7251 (increase max effective balance), to allow large stakers to consolidate without having to fully exit validators & redeploy

**Research**

- [Potential changes to staking rewards & penalties](https://ethresear.ch/t/properties-of-issuance-level-consensus-incentives-and-variability-across-potential-reward-curves/18448/2) to reduce issuance moderately at high staking levels

**For stakers**

- Rated [list of solo stakers](https://github.com/rated-network/solo-stakers) in CSV format (first 500k indices)

* * *

### **Support the** [**Roman Storm & Alex Pertsev legal defense fund**](https://juicebox.money/@free-pertsev-and-storm)

![Open source is not a crime](https://weekinethereumnews.com/wp-content/uploads/2024/01/open-source-is-not-a-crime-1024x341.jpg)

The Biden administration is attempting to criminalize open source software development as part of its war on crypto.

Donate to [defend our innocent Ethereum heroes](https://juicebox.money/@free-pertsev-and-storm).  Retweet to [spread awareness](https://twitter.com/rstormsf/status/1749490246000238942).

* * *

**Layer 2**

- [RARI](https://mirror.xyz/0xAf2C35857711BD4C51e8bCa28307ea6CFf191963/_R9odZC2uwTvUs9vKD7058rgp-728A33tn5jdeQqy6M) L3 (Arbitrum Orbit) live, with NFT royalty enforcement

- [Public Goods Network, Aevo & Lyra](https://twitter.com/conduitxyz/status/1750596065609572398) (OP Stack) changed to Optimiums (sidechain DA)

**EIPs/Standards**

- ERCs (application layer):
    - [ERC7601](https://github.com/ethereum/ERCs/pull/217/files): Dapp permission framework
    
    - [ERC7602](https://github.com/ethereum/ERCs/pull/218/files): Ethereum mixing transaction supervision
    
    - [ERC7603](https://github.com/ethereum/ERCs/pull/220/files): Context-dependent multi-asset tokens (ERC1155 extension)

**Stuff for developers**

- Solidity [v0.8.24](https://soliditylang.org/blog/2024/01/26/solidity-0.8.24-release-announcement/):
    - Cancun support (via EVM version flag): tstore & tload transient storage (EIP1153), blobhash & blobbasefee (EIP4844) and mcopy (EIP5656)
    
    - Apple silicon support

- [Mutexer](https://github.com/jtriley-eth/mutexer): Solidity mutexes (contract, function & custom level), using Cancun transient storage (EIP1153)

- [Forge proposal simulator](https://github.com/solidity-labs-io/forge-proposal-simulator): framework to create proposals (multisig, timelock & Governor Bravo) and deployment scripts/tests

- Ape (Python contract framework) [custom network support](https://twitter.com/apeframework/status/1748476463626547237)

- CTFs:
    - [SmartSecRiddles](https://github.com/marjon-call/SmartSecRiddles): 7 challenges based on vulnerabilities with writeups
    
    - Audit wizard [find the bug](https://app.auditwizard.io/challenge) challenge

**Security**

- Concentric [$1.7M exploit](https://mirror.xyz/concentrictreasury.eth/duXXwBErblGw4CjbsA2JPoRAJqVNsDtiUsK4R6_vhD0) on Arbitrum using social engineering to compromise deployer

**Ecosystem**

- Academic paper on [transparency & concentration](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4691000) in Ethereum governance

- [Suggest a city](https://forum.devcon.org/t/new-suggest-your-city-for-future-ethereum-gatherings/3332) for a future Devcon or Devconnect

* * *

### Job Listings

- Status is hiring: Technical Chief Operating Officer - [Apply here](https://grnh.se/0ecdaa981us)

- Nethermind: [Distributed System Engineer](https://grnh.se/893258d2teu), [Lead Engineer](https://grnh.se/e2d52f72teu), [Protocol Researcher](https://grnh.se/53b888b2teu)

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

- EF seek an [Executive Assistant](https://jobs.lever.co/ethereumfoundation/444bc50a-236e-4a4e-8385-c0454b0044e9) to support senior decision makers

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 6.3 to 82.4 gwei, with 17.6 gwei average
    - Zero net issuance currently at 22.0 gwei 
    
    - 4k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,186 - $2,491, currently $2,267

- [ETHBTC](https://ratiogang.com/): currently 0.054 (Flippening at ~0.16)

**Notable at app layer**

- [Synthetix](https://blog.synthetix.io/scaling-andromeda/) Perps v3 live on Base (Andromeda)

- UMA [Oval](https://medium.com/uma-project/announcing-oval-earn-protocol-revenue-by-capturing-oracle-mev-877192c51fe2) live on mainnet, protocols can capture oracle extractable value

- 0x [Tx Relay API](https://0x.org/post/introducing-tx-relay-api) live on mainnet, gasless swaps & approvals

- Ethereum Attestation Service [MetaMask Snap](https://twitter.com/eas_eth/status/1750919007711174845) decodes EAS attestation data for signing

**Regulation/business/tokens**

- [SEC Twitter account](https://www.sec.gov/secgov-x-account) compromised in January SIM swap had 2FA disabled since July 2023

**General**

- [Support Roman Storm & Alex Pertsev legal defense](https://juicebox.money/@free-pertsev-and-storm) via Juicebox fundraiser

- [USDT on Tron](https://liamhorne.com/stablecoins) is majority of consumer stablecoin transactions & how Ethereum can compete

- [Field Merkle Tree](https://hackmd.io/@0xKanekiKen/H1ww-qWKa): commit multiple STARKs using binary Merkle Tree 

- [Apple fixed WebKit confusion zero day](https://www.bleepingcomputer.com/news/apple/apple-fixes-first-zero-day-bug-exploited-in-attacks-this-year/), update your devices

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-january-27-2024](https://weekinethereumnews.com/week-in-ethereum-news-january-27-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jan 30 – [Sepolia testnet](https://eips.ethereum.org/EIPS/eip-7569#activation) Dencun upgrade epoch 132608

- Feb 2-4 – [ETH Cinco de Mayo](https://ethcincodemayo.com/) hackathon (Cholula, Puebla)

- Feb 3 – [Ethereum Lima Day](https://ethlimaday.org/)

- Feb 7 – [Holešky testnet](https://eips.ethereum.org/EIPS/eip-7569#activation) Dencun upgrade epoch 29696

- Feb 23-Mar 3 – [ETHDenver](https://www.ethdenver.com/) BUIDLWeek & hackathon

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024) hackathon

- Mar 19-21 – [ETH Canal](http://ethcanal.xyz) (Panama City, Panamá) conference & hackathon

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) hackathon & conference 

- Mar 29-31 – [ETH Seoul](https://www.ethseoul.org/) hackathon

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) virtual hackathon

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Apr 12-14 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/) hackathon

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- Jun 3-5 – [ETH Belgrade](https://ethbelgrade.rs/) conference

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 26-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

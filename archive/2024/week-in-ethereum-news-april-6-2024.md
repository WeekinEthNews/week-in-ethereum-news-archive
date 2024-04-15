---
title: "Week in Ethereum News <br> April 6, 2024"
date: "2024-04-05"
---

## Eth News and Links

**Pectra (Prague + Electra) upgrade (meta** [**EIP7600**](https://eips.ethereum.org/EIPS/eip-7600)**)**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=ZqxDq1aJxHc&t=73s). Recap from [Alex Stokes](https://twitter.com/abcoathup/status/1775972681453858953).  Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-131/):
    - **Missed slots**: Lighthouse & Prysm updated to allow Beacon API submission of blobs even if block observed on p2p
    
    - **Pectra upgrade** (small fork targeting late 2024)
        - **Electra included EIPs**:
            - **Pectra-devnet-0** spec [EIP client implementation tracker](https://notes.ethereum.org/@ethpandaops/pectra-devnet-0#Client-implementation-tracker)
            
            - **EIP6110 validator deposits onchain**: mostly ready
            
            - **EIP7002 execution layer triggerable exits:** needs updating to handle partial withdrawals
            
            - **EIP7251 maxEB**: community input wanted on need for custom ceilings & EL initiated consolidations (touches EIP7002) at cost of added complexity
            
            - **EIP7549 committee index outside attestation**: may update for better packing efficiency
        
        - **Electra candidates for inclusion:**
            - **EIP7547 IL (inclusion lists)**: EIP3074 compatibility issues
        
        - **EIP7594 PeerDAS**: work on in parallel to Electra, if going to be longer term could alternatively include EIP7659 to increase blob throughput

- EIP7251 maxEB (increase max effective balance)
    - Breakout call [notes](https://hackmd.io/@philknows/Sy2kQAq1C): custom ceilings, min activation balance constant, week subjectivity issues and concerns from Lido

- EIP7547 IL (inclusion lists)
    - Breakout call [notes](https://hackmd.io/@ttsao/ryCG0cTJA): potential solutions for validity & availability issues

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 29.68%**](https://dune.com/hildobby/eth2-staking) **finally drops below 30%, still too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: **Geth 63%** majority
        - [**Stakefish**](https://twitter.com/stakefish/status/1775712832882884698) **migrated to 50% Nethermind**
    
    - Consensus layer: Prysm 38%
    
    - Any client bug over 33.3% could mean loss of finality
    
    - [**Strategy to target largest concentrated actor**](https://ethresear.ch/t/blue-shell-strategy-discouraging-the-most-concentrated-actor-as-an-optimal-path/19200) **with discouragement attack**

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- [Reward curve with tempered issuance](https://ethresear.ch/t/reward-curve-with-tempered-issuance-eip-research-post/19171): trade-offs, security considerations and endgame

**Client Releases**

- Consensus layer:
    - Prysm [v5.0.3](https://github.com/prysmaticlabs/prysm/releases/tag/v5.0.3): patch with enhancements & bug fixes

- Execution layer:
    - Reth [v0.2.0-beta.5](https://github.com/paradigmxyz/reth/releases/tag/v0.2.0-beta.5): fixes Merkle pipeline stage out of memory issue, adds pruner timeout and supports running on NFS volumes

**Layer 2**

- [Base gas target](https://twitter.com/jessepollak/status/1774933406083846299) increased to 5 mgas/s

**EIPs/Standards**

- EIPs:
    - [EIP7666](https://eips.ethereum.org/EIPS/eip-7666): EVM-ify the identity precompile
    
    - [EIP7667](https://eips.ethereum.org/EIPS/eip-7667): Raise gas costs of hash functions
    
    - [EIP7668](https://eips.ethereum.org/EIPS/eip-7668): Remove bloom filters
    
    - [EIP7669](https://github.com/ethereum/EIPs/pull/8369/files): Linear EVM memory limits
    
    - [EIP7670](https://github.com/ethereum/EIPs/pull/8372/files): Reduced attestation format
    
    - [EIP7675](https://github.com/ethereum/EIPs/pull/8389/files): Retroactively included EIPs
    
    - [EIP7676](https://github.com/ethereum/EIPs/pull/8385/files): EOF - Prepare for address space extension

- ERCs (application layer):
    - [ERC7672](https://github.com/ethereum/ERCs/pull/353/files): Event-driven NFT utilities
    
    - [ERC7673](https://github.com/ethereum/ERCs/pull/354/files): Distinguishable base256emoji addresses
    
    - [ERC7674](https://github.com/ethereum/ERCs/pull/358/files): Temporary approval extension for ERC20
    
    - [ERC7677](https://github.com/ethereum/ERCs/pull/360/files): Paymaster web service capability
    
    - [ERC7679](https://github.com/ethereum/ERCs/pull/361/files): UserOperation builder

**Stuff for developers**

- [Solidity Developer Survey 2023 results](https://soliditylang.org/blog/2024/04/03/solidity-developer-survey-2023-results/):
    - Hardhat usage at 33%, Foundry 32% & Remix 26% 
    
    - Solidity v0.8 usage at 82%

- Guide to [migrate from from hardhat-deploy to Hardhat Ignition](https://blog.nomic.foundation/migrating-to-hardhat-ignition-from-hardhat-deploy-c17311bb658f)

- [Tweak](https://twitter.com/i2huer/status/1775367173281608031) (Foundry fork): alter onchain verified contracts (e.g. add console.log) & replay historical transactions

- Hayden asked [should Uniswap v4 remove events](https://twitter.com/haydenzadams/status/1775907308372922464) & move to call traces for 1% gas saving on swaps
    - Lefteris: [need agreement & standardization](https://twitter.com/lefterisjp/status/1776036222827204632) for any alternative

- Coinbase [Solidity style guide](https://github.com/coinbase/solidity-style-guide#readme)

- [OpenSea ERC721C support](https://opensea.io/blog/articles/creator-earnings-erc721-c-compatibility-on-opensea): enforced creator royalties but restricted to OpenSea & Magic Eden

- Fuzz-utils [v0.2.0](https://github.com/crytic/fuzz-utils/releases/tag/0.2.0): generate Echidna/Medusa compatible fuzzing harnesses

- [Sigmund](https://github.com/wavefnx/sigmund#readme) (CLI): collect function selectors from any contract

- Swiss knife [determine contract address](https://contract-address.swiss-knife.xyz/) using deployer address & nonce

- [SIWE AAbstractor](https://siwe.aabstr.actor/): connect smart accounts to apps via Sign in with Ethereum

- Viem [experimental](https://viem.sh/experimental): support for draft EIP5792 (batch transactions with paymaster capability)

- [Noble-post-quantum](https://github.com/paulmillr/noble-post-quantum#readme) (JavaScript): minimal implementations of ML-KEM, ML-DSA & SLH-DSA

- [Open Labels Initiative](https://github.com/openlabelsinitiative/OLI#readme): framework & data model for EVM address labeling

- CTFs:
    - [Secureum RACE #28](https://ventral.on.fleek.co/posts/2024/4/2/race-28-of-the-secureum-bootcamp-epoch-infinity/): 8 question Solidity quiz & answers

**Security**

- Geth [DoS vulnerability disclosed](https://iosiro.com/blog/geth-out-of-order-eip-application-denial-of-service), nodes with exposed RPC could be crashed by applying EIPs out of order during an eth\_call, fixed in v1.13.13

**Ecosystem**

- Vitalik: [next steps in the Purge](https://notes.ethereum.org/@vbuterin/purge_2024_03_31), precompiles, history (via EIP4444), log reform & moving to SSZ

- [Road to Devcon](https://devcon.org/en/road-to-devcon/) event calendar

- Hackathon winners: [ETHBucharest](https://ethbucharest.notion.site/ETHBucharest-Hacker-Handbook-cf0fb82f622340b4a41815b289eaef81) & [ETHSeoul](https://ethseoul2024.devfolio.co/projects?prizes=12054b55e2bc48ebad0a0432f5d2f23e&show_winners=false)

**Enterprise**

- [Project Agorá](https://www.bis.org/press/p240403.htm): BIS & 7 central banks explore tokenization of cross-border payments

* * *

### Job Listings

- ChainSafe: [Head of Protocol Engineering](https://grnh.se/c6e27e794us) and [Senior Product Manager](https://grnh.se/8736d15d4us)

- Devcon: [Community Supporter](https://jobs.lever.co/ethereumfoundation/6ad3d8e7-17cb-4d5c-820d-c279e8002551), [Production Magician](https://jobs.lever.co/ethereumfoundation/aa4c69f8-f564-4036-9c5e-3e09f0eb27df) & [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/e93dae67-65a6-495c-8638-46e3db28cb64)

- Nethermind [Mechanism Designer](https://grnh.se/e78eb182teu), [Protocol Research Manager](https://grnh.se/8f2a6c32teu), [Research Engineer](https://grnh.se/887df932teu)

- Certora is hiring: [Head of Product](https://hubs.ly/Q02n-d-X0), [SR-Rust](https://hubs.ly/Q02n-fmD0), [Compiler Developer](https://hubs.ly/Q02n-b_20) & [FV Wizard](https://hubs.ly/Q02n-fyx0)

- Solidity: [C++ Software Engineer](https://jobs.lever.co/ethereumfoundation/a6e4598e-6c12-493e-8426-438cb0a5eeca) and [Programming Language Researcher](https://jobs.lever.co/ethereumfoundation/d510dfd7-d5dd-435c-9111-1c50112715c1)

- 🔥OpenZeppelin seeks Security Researchers in [Canada](https://grnh.se/3d8f61e53us), [Australia](https://grnh.se/bb2348b83us), [LatAm](https://grnh.se/3b4915233us) & [USA](https://grnh.se/54d2bd163us)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 8.6 to 120.5 gwei, with 25.8 gwei average
    - Zero net issuance currently at 22.7 gwei 
    
    - 2.8k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,224 - $3,641, currently $3,325

- [ETHBTC](https://ratiogang.com/): currently 0.049 (Flippening at ~0.16)

**Notable at app layer**

- [Maker's big bet](https://cryptobanking.network/money-view-of-the-makerdao-morpho-ethena-drama/) on Ethena
    - [Aave proposes](https://governance.aave.com/t/arfc-risk-parameters-for-dai-update/17211) 0% LTV for Dai in response

- [Blob inscriptions](https://twitter.com/roberto_bayardo/status/1775910723539112169) fizzle out

- [Synthetix v3](https://blog.synthetix.io/synthetix-v3-on-base/) live on Base, using USDC as collateral 

- [Gitcoin Grants 20](https://grants.gitcoin.co/) applications open until April 16; open source software rounds: infrastructure, dev tooling, apps and hackathon alumni

**Regulation/business/tokens**

- US vs Roman Storm: amicus briefs from [Blockchain Association](https://theblockchainassociation.org/blockchainassociation-files-amicus-brief-in-dojs-case-against-tornado-cash-developers/), [Coin Center](https://www.coincenter.org/coin-center-files-a-court-brief-in-defense-of-tornado-cash-developer/) & [DeFi Education Fund](https://twitter.com/amandatums/status/1776293907929714757)

- SEC Commissioner Peirce: [improving communication between public & SEC](https://www.sec.gov/news/speech/peirce-remarks-sec-speaks-040224)

- Bank of England & FCA [digital securities sandbox](https://www.bankofengland.co.uk/paper/2024/cp/digital-securities-sandbox-joint-bank-of-england-and-fca-consultation-paper) consultation, feedback by May 29

**General**

- Vitalik: [degen communism](https://vitalik.eth.limo/general/2024/04/01/dc.html) \[posted April 1\], chaos aligned with common good, e.g. memecoin issuance to charity, public goods funding, fork out concentrated players, land value taxes and Harberger taxes on IP

- [XZ Utils (compression library) backdoored](https://www.openwall.com/lists/oss-security/2024/03/29/4), v5.6.0/1 impacted, found after logins via ssh 0.5s slower

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-april-6-2024](https://weekinethereumnews.com/week-in-ethereum-news-april-6-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Apr 12-14 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- Apr 16-18 – [EY Global blockchain summit](https://web.cvent.com/event/e0ad2c12-3e65-41a9-bafb-a436754cf4ae/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7) (London)

- Apr 19-21 – [ETH Tallinn](https://www.ethtallinn.org/) hackathon

- Apr 20-21 – [ETHDubai](https://www.ethdubaiconf.org/) conference & hackathon

- Apr 23-May 7 – [Gitcoin Grants 20](https://grants.gitcoin.co/) (application deadline Apr 16)

- Apr 26-28 – [ETHBoston](https://ethboston.xyz/) hackathon & conference

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- May 10-11 – [ETH Bratislava](https://www.ethbratislava.com/) conference & hackathon

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/) hackathon

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- May 31-Jun 5 – [ETH Belgrade](https://ethbelgrade.rs/) hackathon & conference

- Jun 14 – [EF EIP4844 data challenge](https://esp.ethereum.foundation/data-challenge-4844) deadline

- Jun 21-23 – [ETHKyiv](https://www.ethkyiv.org/) hackathon & conference

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

- Oct 4-6 – [ETHRome](https://ethrome.org/)

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

---
title: "Week in Ethereum News <br> March 9, 2024"
date: "2024-03-08"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- Reminder: [mainnet upgrades to Dencun](https://blog.ethereum.org/2024/02/27/dencun-mainnet-announcement) March 13, epoch 269568, update your nodes
    - Metrika: [node readiness](https://app.metrika.co/ethereum/dashboard/network/network-upgrade?tr=1w) tracker, 58% already updated

**Pectra (Prague + Electra) upgrade (meta** [**EIP7600**](https://eips.ethereum.org/EIPS/eip-7600)**)**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=imBLUhGYnWs&t=190s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-129/):
    - Electra upgrade scope (small cross layer fork targeting late 2024):
        - **EIP7549 move committee index outside attestation**: [onchain aggregate optimization](https://hackmd.io/@n0ble/eip7549_onchain_aggregates) discussion
        
        - **Issuance adjustment**: mixed community feedback, ongoing discussions, small code change, aim for go/no go mid year on including in Electra
        
        - **EIP7547 inclusion lists** (candidate for Electra): breakout call next week, spec ~75% ready
        
        - **EIP7251 max effective balance** (candidate for Electra): greater support for including in Electra, previous pushback was complexity which Prysm will review again
    
    - Discussions: keymanager API auth standardization, Beacon API block value standardization, specifying late block behavior and ePBS payload boost

**Client Releases**

- Consensus layer:
    - Teku [v24.3.0](https://github.com/Consensys/teku/releases/tag/24.3.0): improved block rewards calculation performance

- Execution layer:
    - Besu [v24.3.0](https://github.com/hyperledger/besu/releases/tag/24.3.0): Bonsai storage format & Snap sync now default and Bonsai updated to reduce disk usage

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.06%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth 72% supermajority, could cause a chain split
    
    - Consensus layer: Prysm 37%, any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- [State growth viz](https://www.paradigm.xyz/2024/03/how-to-raise-the-gas-limit-1): ERC20 is 27.2% of state, ERC721 is 21.6%; consumer hardware predicted to sustain current growth rates for a decade

- Geth [dropping support for pre-merge networks](https://twitter.com/peter_szilagyi/status/1765016675131301958) & [almost halved CPU usage](https://twitter.com/vdWijden/status/1765657745502404948)

- Light clients breakout call [notes](https://hackmd.io/@philknows/ryMFFQUpT)

**Inclusion Lists (**[**EIP7547**](https://eips.ethereum.org/EIPS/eip-7547)**)**

- [Proof of Concept](https://notes.ethereum.org/@mikeneuder/il-poc-spec) specification

- Terence:
    - [Inclusion lists variation](https://ethresear.ch/t/inclusion-list-eip-7547-end-to-end-workflow/18810), current slot inclusion list summary is committed within a block
    
    - [Address censorship](https://hackmd.io/@ttsao/ByO9D-Uaa) in relayers & builders by allowing validators to include own transactions

- Discussion on [whether inclusion lists are the right solution](https://twitter.com/koeppelmann/status/1765357711187759201)

**For Stakers**

- Lighthouse [user survey results](https://lighthouse-blog.sigmaprime.io/lighthouse-user-survey.html)

**Research**

- [Execution tickets](https://ethresear.ch/t/economic-analysis-of-execution-tickets/18894) economic analysis: tickets must be sold at their intrinsic value otherwise value would leak into a secondary market

* * *

### **Support the** [**Roman Storm & Alex Pertsev legal defense fund**](https://juicebox.money/@free-pertsev-and-storm)

![Open source is not a crime](https://weekinethereumnews.com/wp-content/uploads/2024/01/open-source-is-not-a-crime-1024x341.jpg)

The Biden administration is attempting to criminalize open source software development as part of its war on crypto.

**The fundraiser ends March 15.** Donate to [defend our innocent Ethereum heroes](https://juicebox.money/@free-pertsev-and-storm).  

* * *

**Layer 2**

- EIP4844 blobs:
    - Optimism Superchain [savings estimator](https://welovetheblobs.xyz/) and [methodology](https://oplabs.notion.site/Superchain-Savings-Estimator-100e62675cd849488b6c275a2e09ca0c)
    
    - zk rollup [saving estimates](https://twitter.com/louthinge/status/1765411197367857571)
    
    - [Rollup spending on posting data](https://twitter.com/0xkofi/status/1764684311297503644) in February, prior to changing to blobs

- OP Stack adds [snap sync](https://twitter.com/optimism/status/1766068852935598221)

- [Fast finality](https://ethresear.ch/t/why-wait-a-week-fast-finality-optimistic-rollups/18868) optimistic rollup proposal, use check-in based model to reduce 7 day window, honest minority assumption

**EIPs/Standards**

- EIPs:
    - [EIP7645](https://github.com/ethereum/EIPs/pull/8283/files): Alias ORIGIN to SENDER

- ERCs (application layer):
    - [ERC7646](https://github.com/ethereum/ERCs/pull/293/files): Metadata management for NFTs
    
    - [ERC7647](https://github.com/ethereum/ERCs/pull/295/files): Fungible NFTs (hybrid ERC20/721)
    
    - [ERC7648](https://github.com/ethereum/ERCs/pull/296/files): NFT recursive synthesis asset
    
    - [ERC7649](https://github.com/ethereum/ERCs/pull/300/files): Bonding curve-embedded liquidity for NFTs

**Stuff for developers**

- Hardhat:
    - [v2.21.0](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.21.0): adds Ethereum Development Runtime (EDR) in Rust, replaces TypeScript based Hardhat Network
    
    - [Multichain-deploy](https://github.com/ChainSafe/hardhat-plugin-multichain-deploy#readme): Hardhat plugin using Sygma

- Gaslite [Bytecode20](https://github.com/PopPunkLLC/gaslite-core/blob/main/src/Bytecode20.sol): gas optimized ERC20 in EVM bytecode

- [Return bombing](https://twitter.com/0xkarmacoma/status/1763746082537017725): how to safely process revert data

- Titanoboa (Vyper interpreter) [Boa Solidity](https://github.com/z80dev/boa-solidity#readme): adds Solidity support

- Snekmate [v0.0.5](https://github.com/pcaversaccio/snekmate/releases/tag/v0.0.5): for Vyper v0.3.10, adds multi-role-based timelock controller

- [Verifier alliance](https://verifieralliance.org/blog/hello-world.html) (VERA): shared database for verified contract source code

- [ERC4337 first year](https://twitter.com/schorlukas/status/1764064836520947874): 3M accounts, limited adoption depth, low retention, fragmentation, only $200k in bundler revenue and multiple entry point upgrades

- Guide for [dapps to adopt EIP6963](https://github.com/nfwsncked/eip-6963-tutorial#readme) (multi injected provider discovery)

- Wallet Test Framework [test report 2](https://wtf.allwallet.dev/week-47/)

- CTFs:
    - [Secureum RACE #27](https://ventral.digital/posts/2024/3/4/race-27-of-the-secureum-bootcamp-epoch-infinity/): 8 question Solidity quiz & answers

- [Goerli testnet](https://twitter.com/potuz_eth/status/1765734505921265993) no longer finalizing, Prysm users please update to latest release candidate

**Security**

- WOOFi [$8.75M exploit](https://woo.org/blog/en/woofi-spmm-exploit-post-mortem) on Arbitrum via price manipulation

**Ecosystem**

- ETHDenver [videos](https://www.youtube.com/@ETHDenver/videos) and hackathon [top 15 projects](https://www.ethdenver.com/buidl-judging)

* * *

### Job Listings

- [Waku](https://waku.org/about) hiring! [Protocol Engineer](https://grnh.se/a240b11b1us), [Waku SDK Software Engineer](https://grnh.se/0a63ae031us) & [Researcher](https://grnh.se/b96ad7111us)

- [IFT](https://free.technology/)/[Logos](https://logos.co/): [ZK Researcher](https://boards.greenhouse.io/nomos/jobs/5664663) (Nomos); [ZK Researcher](https://boards.greenhouse.io/vac/jobs/5453093) (Vac) & [ZK Engineer](https://boards.greenhouse.io/vac/jobs/5543856) x2

- ChainSafe seek a [Head of Protocol Engineering](https://grnh.se/c6e27e794us)

- [Sr. Developer Relations Manager](https://wellfound.com/jobs/2933743-sr-developer-relations-manager-at-powerloom-protocol) & [Technical Writer](https://wellfound.com/jobs/2931135-technical-writer-at-powerloom-protocol) at [Powerloom](https://powerloom.io/)

- Devcon: [Community Supporter](https://jobs.lever.co/ethereumfoundation/6ad3d8e7-17cb-4d5c-820d-c279e8002551), [Production Magician](https://jobs.lever.co/ethereumfoundation/aa4c69f8-f564-4036-9c5e-3e09f0eb27df) & [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/e93dae67-65a6-495c-8638-46e3db28cb64)

- [TechOps](https://techops.services) are looking for [DevOps](https://apply.workable.com/techops-services/j/5AD8CF90E0/). Work on projects such as MakerDAO.

- Nethermind: [Distributed Systems Dev Lead](https://grnh.se/c3fd6842teu) & [Cryptography Researcher](https://grnh.se/51fa8652teu) 

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 30.3 to 394.1 gwei, with 66.3 gwei average
    - Zero net issuance currently at 23.0 gwei 
    
    - 33.6k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,360 - $3,998, currently $3,897

- [ETHBTC](https://ratiogang.com/): currently 0.057 (Flippening at ~0.16)

**Notable at app layer**

- Maker [voted](https://vote.makerdao.com/executive/template-executive-vote-out-of-schedule-executive-vote-increase-edsr-increase-stability-fees-decrease-gsm-delay-usdc-psm-throughput-change-trigger-spark-proxy-spell-march-8-2024) to change DSR to 15%, Stability Fees to 15-17.25% & GSM to 16 hours

- Kwenta [Perps v3](https://mirror.xyz/kwenta.eth/L1URqNbXQmXdxueT4qRELzHMTGX3lFZppKRbojvsus0) live on Base, beta

- [Power perpetuals](https://research.opyn.co/everything-is-a-perp) include stablecoins, margined perpetual futures and AMMs

**Regulation/business/tokens**

- [SEC cease & desist](https://www.sec.gov/files/litigation/admin/2024/34-99676.pdf) against ShapeShift; SEC Republican members [dissent](https://www.sec.gov/news/statement/peirce-uyeda-statement-a-crypto-world-turns-03-06-24)

- Wyoming [Decentralized Unincorporated Nonprofit Association](https://a16zcrypto.com/posts/article/duna-for-daos/) (DUNA) signed into law, allows DAOs to setup a legal entity

- Optimism’s RetroPGF: [moving to narrow scope rounds](https://gov.optimism.io/t/retro-funding-moving-from-broad-to-narrow-scoped-rounds/7759) & [badgeholders paid for voting](https://gov.optimism.io/t/retro-citizen-rewards-retro-funding-3/7758)

**General**

- [Twitter calling enabled by default](https://techcrunch.com/2024/03/04/elon-musk-x-twitter-calling-privacy-switch-off/), leaks IP address, change your settings on mobile

- [STIR (Shift To Improve Rate)](https://eprint.iacr.org/2024/390): IOPP for RS codes, compared with FRI has shorter arguments & faster verifier with fewer hashes

- OpenZeppelin: [incorrect computation of last challenge](https://eprint.iacr.org/2024/398) in KZG-based PLONK verifier implementation

* * *

**End of service:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-march-9-2024](https://weekinethereumnews.com/week-in-ethereum-news-march-9-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Mar 13 – [mainnet Dencun upgrade](https://eips.ethereum.org/EIPS/eip-7569#activation) epoch [269568](https://beaconcha.in/epoch/269568), ([watch party](https://www.youtube.com/watch?v=iL0cZRkyrV0))

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024) hackathon

- Mar 18 – [ZK grants round](https://esp.ethereum.foundation/zk-grants) application deadline

- Mar 19-21 – [ETH Canal](http://ethcanal.xyz) (Panama City, Panamá) conference & hackathon

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- Mar 22-24 – [ETHSamba](https://ethsamba.org/) (Rio)

- **Mar 24-29 –** [**Ethaly**](http://ethaly.io/) **(Savelletri di Fasano, Italy)**

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) conference & hackathon

- Mar 29-31 – [ETH Seoul](https://www.ethseoul.org/) hackathon

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) virtual hackathon

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Apr 12-14 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- Apr 16-18 – [EY Global blockchain summit](https://web.cvent.com/event/e0ad2c12-3e65-41a9-bafb-a436754cf4ae/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7) (London)

- **Apr 19-21 –** [**ETH Tallinn**](https://www.ethtallinn.org/) **hackathon**

- Apr 26-28 – [ETHBoston](https://ethboston.xyz/) conference & hackathon

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/) hackathon

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- **May 31-Jun 5** – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 14 – [EF EIP4844 data challenge](https://esp.ethereum.foundation/data-challenge-4844) deadline

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 26-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- **Aug 29-31 –** [**ETHAccra**](https://ethaccra.xyz) **hackathon**

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Oct 6-8 – [ETHRome](https://ethrome.org/)

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

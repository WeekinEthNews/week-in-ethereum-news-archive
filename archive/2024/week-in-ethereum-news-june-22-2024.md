---
title: "Week in Ethereum News <br> June 22, 2024"
date: "2024-06-22"
---

## Eth News and Links

Blob fee market issues, SEC drops Consensys case and CertiK withdrew ~$3M from Kraken without authorization

**All core devs**

- [All core devs – execution (ACDE) #190](https://ethereum-magicians.org/t/all-core-devs-execution-acde-call-190/20306):
    - Pectra (Prague + Electra) upgrade:
        - [**pectra-devnet-1**](https://notes.ethereum.org/@ethpandaops/pectra-devnet-1): aim to launch next week with subset of clients, will include execution layer triggered withdrawals & current version of EIP7702
        
        - **EIP7702**: discussion of [delegation designation proposal](https://github.com/ethereum/EIPs/pull/8677) (revoke by redelegating), [breakout #5](https://github.com/ethereum/pm/issues/1081) June 26
        
        - **EOF**: rebasing to build on top of Prague upgrade, [EOF readiness tracker](https://github.com/ipsilon/eof/blob/main/spec/implementation_matrix.md)

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade, likely targeting Q1 2025**

- Frangio: [ERC721/1155 issue with EOF](https://ethereum-magicians.org/t/evm-object-format-eof/5727/96), safe transfer checks if token recipient is a contract using code size

[**Osaka + F starname**](https://eips.ethereum.org/EIPS/eip-7607) **upgrade**

- [Verkle implementers call #19](https://ethereum-magicians.org/t/verkle-implementers-call-19/20305):
    - transition tests mostly passing on Geth, support increasing code size limit, testnet relaunch targeting July & preimage distribution discussion

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.78%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~55% majority 
    
    - Consensus layer: Prysm 38%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Blob fee market issues, highlighted by [price spike](https://x.com/mcutler/status/1803876002734735381):
    - Potuz: [market for blobs is broken](https://x.com/potuz_eth/status/1803885117384917228)
    
    - Terence: [ideas to fix](https://x.com/terencechain/status/1803891723246145841)
    
    - Data viz of [slot inclusion rates](https://ethresear.ch/t/slot-inclusion-rates-and-blob-market-combinatorics/19817) and analysis of blob market strategies

- Dankrad: [blob strategies to help self builders](https://notes.ethereum.org/@dankrad/self-builder-strategies)

- ePBS:
    - [ePBS breakout #3](https://hackmd.io/@ttsao/epbs-breakout3) 
    
    - Terence: [ePBS FAQ](https://hackmd.io/@ttsao/epbs-faq0)

**Research**

- Anders Elowsson: [analysis of burn incentives](https://ethresear.ch/t/burn-incentives-in-mev-pricing-auctions/19856) in MEV pricing auctions

- [Fork-choice enforced inclusion lists](https://ethresear.ch/t/fork-choice-enforced-inclusion-lists-focil-a-simple-committee-based-inclusion-list-proposal/19870) (FOCIL): committee-based inclusion list design

**Client Releases**

- Consensus layer:
    - Prysm [v5.0.4](https://github.com/prysmaticlabs/prysm/releases/tag/v5.0.4): fixes p2p peer for Windows users, Beacon API retrieving old blobs & initial sync avoids redundant blob downloads
    
    - Teku [v24.6.0](https://github.com/Consensys/teku/releases/tag/24.6.0): performance improvements & fixes; [v24.6.1](https://github.com/Consensys/teku/releases/tag/24.6.1): fix for v24.6.0 startup failure

- Execution layer:
    - Nethermind [v1.27.0](https://github.com/NethermindEth/nethermind/releases/tag/1.27.0): ~150% improvement to block processing & intra-block cache 

**For Stakers**

- Lighthouse: [guide to missed attestations](https://lighthouse-blog.sigmaprime.io/attestation-analysis.html), common issues & tuning parameters

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP discussions](https://ethereum-magicians.org/t/template-for-discussion-to-threads/20347) proposal, highlight updates, reviews & outstanding issues

- ERCs (application layer standards):
    - [ERC7725](https://github.com/ethereum/ERCs/pull/498/files): Exponential curves
    
    - [ERC7726](https://github.com/ethereum/ERCs/pull/500/files): Common quote oracle
    
    - Guide to [writing an ERC](https://x.com/jtriley_eth/status/1803811612773781914)

- [EIP.tools](https://eip.tools/): view & search EIP/ERCs

**Stuff for developers**

- Foundry [afterInvariant](https://x.com/lucasmanuel_eth/status/1803432948219171301) hooks: test state at end of an invariant test run

- [Transience](https://github.com/ethereum-optimism/transience#readme) (Solidity library): manage transient storage

- Vyper [v0.4.0](https://x.com/vyperlang/status/1804234870400376888): adds module system (code reuse via composition), Venom optimizer pipeline & [archive creation](https://x.com/vyperlang/status/1804105359058960790) of a build for sharing

- [Sneko](https://github.com/wolovim/sneko#readme): terminal GUI for compiling Vyper & Solidity contracts

- Alloy [v0.1](https://www.paradigm.xyz/2024/06/alloy-release): rewrite of ethers-rs & Solidity type system in Rust

- [Revmc](https://www.paradigm.xyz/2024/06/revmc): EVM bytecode to native code compiler

- ethPandaOps: [build an L2 devnet using Kurtosis ethereum-package](https://ethpandaops.io/posts/kurtosis-l2/)

- Viem
    - [NonceManager](https://viem.sh/docs/accounts/createNonceManager): manage/generate nonces for a local accounts transactions
    
    - [Deployless Calls](https://viem.sh/docs/actions/public/call#deployless-calls): call a function on a contract that hasn’t been deployed

- Vacp2p stealth address kit [v0.2.0](https://github.com/vacp2p/stealth-address-kit/releases/tag/v0.2.0): adds pallas & vesta, bw6\_761 & baby\_jub\_jub curves

- [Relayscan bids archive](https://github.com/flashbots/relayscan/blob/main/docs/2024-06_bidcollect.md): builder bids for all relays, uploaded nightly, CC0 license

**Security**

- Kraken [balance inflation vulnerability](https://x.com/c7five/status/1803403565865771370) disclosed & patched
    - [CertiK](https://x.com/CertiK/status/1803450205389402215) withdrew ~$3M over 5 days before reporting, funds now returned

**Ecosystem**

- Devcon: [ticket raffle & auction](https://raffle.devcon.org/) live on Arbitrum, 20 tickets for highest auction bids, 184 tickets for raffle winners, minimum entry is 0.08 ETH

**Enterprise**

- Enterprise Ethereum Alliance: [survey on business usage of Ethereum](https://docs.google.com/forms/d/e/1FAIpQLScH5rkFrogy9fBE8YKoU0HJ1eXJpt8fzvfkhJOVqQ2OsGXHmg/viewform)

* * *

### Job Listings

- [Alchemy](https://www.alchemy.com/careers) - Wallet Services: [Engineering Manager](https://grnh.se/cc56a4365us) and [Full-Stack Engineer](https://grnh.se/5a40c3b55us)

- Nethermind: [Preconfirmations Senior Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4344191101), [Protocol Researcher](https://boards.eu.greenhouse.io/nethermind/jobs/4347537101), [Site Reliability Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4321978101), [Senior Content Marketing](https://boards.eu.greenhouse.io/nethermind/jobs/4351446101) & [Senior Marketing Manager](https://boards.eu.greenhouse.io/nethermind/jobs/4346942101)

- IMC: [Quant Developer](https://imczug.recruitee.com/o/quant-developer-defi) for DeFi and MEV focused team

- Privacy and Scaling Explorations: [ZK Circuits Engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4)

- Gnosis is hiring: [Discord Moderator](https://gnosis.jobs.personio.com/job/1166297?_pc=1517287) and [Senior Web3 Software Dev (Wallet)](https://gnosis.jobs.personio.com/job/1569366?display=en&_pc=1517287)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 1.9 to 95.6 gwei, 6.5 gwei average; zero net issuance at 23.5 gwei 
    
    - **Blob gas: spiked to 8,405 gwei; 251 ETH burnt**
    
    - 12.5k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,387 - $3,632, currently $3,511, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.055 (Flippening at ~0.16)

**Regulation/business/tokens**

- [SEC formally notifies Consensys](https://assets.ctfassets.net/gjyjx7gst9lo/6BtUdxsw1vlatBjIspkJN9/792adab194b9ac71c1eeeded42b01615/Termination_Notice_K._Schwartz_6.18.24.pdf) that it will not be charged

- [Fortune](https://archive.is/juR1U): CFTC probing Jump Crypto

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-june-22-2024](https://weekinethereumnews.com/week-in-ethereum-news-june-22-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jul 7 – [Devcon scholars program](https://blog.ethereum.org/2024/06/07/devcon7-scholars) deadline

- **Jul 9–** [**Devcon ticket raffle & auction**](https://raffle.devcon.org/) **deadline**

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 29-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 2-4 – [Ethereum Argentina](https://ethereumargentina.org/) conference & hackathon

- Aug 7-9 – [Science of Blockchain Conference](https://www.sbc-conference.com/) (New York)

- Aug 15-17 – [Ethereum Uruguay](https://taikai.network/ethuruguay/hackathons/buildathon-2024) hackathon & conference

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 23-26 – [ETHTokyo](https://www.ethtokyo.com/) hackathon & conference

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- Sep 5-8 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 9-15 – [ETHSafari](https://ethsafari.xyz/) (Kenya)

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 13-14 – [Ethereum México](https://ethmexico.org/)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Sep 26-27 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 4-6 – [Ethereum Kuala Lumpur](https://www.2024.ethkl.org/) conference & hackathon

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

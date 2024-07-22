---
title: "Week in Ethereum News <br> July 13, 2024"
date: "2024-07-13"
---

## Eth News and Links

Multiple domains compromised, SEC drops Paxos BUSD case, Devcon ticket sales open, Alex Pertsev denied bail and Roman Storm granted trial delay

**All core devs**

- [**All core devs – consensus (ACDC) #137**](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-call-137-july-11-2024/20481):
    - **Pectra (Prague + Electra) upgrade**:
        - **Pectra-devnet-1**: aim to launch next week 
        
        - **EIP7594 PeerDAS**:
            - peerdas-devnet-2 launching early next week with fixes from previous devnet
            
            - Decouple layers for blob count: max blob check on execution layer is redundant & can be removed, proposal for target blob count to be driven by consensus layer (needs to be included in execution layer block header)
    
    - [Fork choice compliance testing](https://docs.google.com/presentation/d/1W2DUwcu411cebQXi_9m-zVk1MASirpIop1cPdqg8dGE/edit) presentation, model based test generation, test suite run with Teku

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade, likely targeting Q1 2025**

- Marius Van Der Wijden: [case against EOF in Pectra](https://mariusvanderwijden.github.io/blog/2024/07/12/EOF/)

- [PeerDAS breakout #3](https://ethereum-magicians.org/t/peerdas-breakout-3-july-9-2024/20482):
    - Relaunch devnet with client fixes, proposal to use custody groups instead of subnets to decouple core & network layers and agreed consensus layer should send max & target blob counts in execution layer header

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 29%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~55% majority 
    
    - Consensus layer: Prysm 37%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Layer 1**

- Toni Wahrstätter: [attestations analysis](https://ethresear.ch/t/deep-diving-attestations-a-quantitative-analysis/20020), node operator performance, best/worst validators, big block & blob impact and proposer timing games

- Data Always: [censorship resistance proposal](https://hackmd.io/@dataalways/censorship-resistance-today), limit missed proposer income & increase localBlockValueBoost

- Constantine [v0.1](https://ethresear.ch/t/releasing-constantine-v0-1-0-a-modular-cryptography-stack-for-ethereum/19990): implementations of BLS signatures, BN254 & BLS12-381 precompiles and KZG polynomial commitments for blobs; bindings in C, Go, Nim & Rust

- Péter Szilágyi: [SSZ library](https://github.com/karalabe/ssz#readme) implemented in Go

**Research**

- Anders Elowsson: [dynamic pricing auction of execution proposal rights](https://ethresear.ch/t/mev-resistant-dynamic-pricing-auction-of-execution-proposal-rights/20024), induces less new MEV & produces high aggregate MEV burn

**Client Releases**

- Consensus layer:
    - Lodestar [v1.20.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.20.0): lodestar/api package changes exported types, flag to use SSZ APIs with validator client and testnet bootnode ENRs updated

- Execution layer:
    - Besu [v24.7.0](https://github.com/hyperledger/besu/releases/tag/24.7.0): adds eth\_maxPriorityFeePerGas support and improvements to sync, peering & startup performance
    
    - Erigon [v2.60.3](https://github.com/ledgerwatch/erigon/releases/tag/v2.60.3): adds optional include precompiles flag to tracing
    
    - Geth [v1.14.7](https://github.com/ethereum/go-ethereum/releases/tag/v1.14.7): hotfix for concurrent map read/write bug in v1.14.6
    
    - Reth [v1.0.1](https://github.com/paradigmxyz/reth/releases/tag/v1.0.1): full node performance improvements, ExEx backfill & RPC fixes

**For Stakers**

- Stereum [v2.2](https://github.com/stereum-dev/ethereum-node/releases/tag/v2.2.0): multi-setup support and connection check to test network stability & connectivity

**Layer 2**

- OP Stack [Fjord upgrade](https://x.com/oplabspbc/status/1811072244124188999), cheaper smart wallet passkey verification via RIP7212 secp256r1 precompile and 5-15% lower data availability costs via Brotli channel compression

- [RollCall (L2 standards) #6](https://ethereum-magicians.org/t/rollcall-6-july-10-2024/20426):
    - L1 blob basefee spike on June 20 discussion and presentations on [RIP7728 L1SLOAD precompile](https://docs.google.com/presentation/d/1k4vnlkmCil2zrdu9xGBqxkA8AZbh97tXP5Gkte3886o/edit) & RIP7740 preinstall deterministic deployment factories

- Titan Builder [eth\_sendBlobs](https://x.com/titanbuilderxyz/status/1809231370243211601): send permutations of blob transactions from a single sender

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7742](https://github.com/ethereum/EIPs/pull/8735/files): Uncouple blob count between CL and EL

- RIPs (rollup improvement proposals):
    - [RIP7740](https://github.com/ethereum/RIPs/pull/30/files): Preinstall deterministic deployment factories

- ERCs (application layer standards):
    - [ERC7737](https://github.com/ethereum/ERCs/pull/523/files): Custom data access model
    
    - [ERC7738](https://github.com/ethereum/ERCs/pull/530/files): Permissionless script registry
    
    - [ERC7739](https://github.com/ethereum/ERCs/pull/441/files): Readable typed signatures for smart accounts
    
    - [ERC7741](https://github.com/ethereum/ERCs/pull/536/files): Authorize operator (via EIP712 secp256k1 signatures)

- [EIP.tools](https://eip.tools/) adds EIP-GPT, AI generated summary of an EIP/ERC

**Stuff for developers**

- [Web-solc](https://github.com/gnidan/web-solc#readme): adapter to fetch/run specific version of Solidity compiler in the browser

- RareSkills: [guide to OpenZeppelin Contracts Initializable](https://www.rareskills.io/post/initializable-solidity)

- [ERC3770](https://github.com/Rjected/erc3770#readme) (Rust): helper method for ERC3770 chain specific addresses

- Nethermind [Clear](https://medium.com/nethermind-eth/clear-prove-anything-about-your-solidity-smart-contracts-04c6c7381402): formal verification framework for Yul code 

- [Byteracing](https://www.byte.racing/): maze solver in Solidity, try to make it more gas efficient

**Security**

- Dough Finance [$2M exploit](https://twitter.com/ImmuneBytes/status/1811762723124093431) via unvalidated calldata

**Ecosystem**

- [Devcon updates](https://blog.ethereum.org/2024/07/09/devcon-7-tickets):
    - Ticket sales are open
        - Self-claimable discounts (using Ethereum address or GitHub)
        
        - Application based discounts
        
        - General admission wave 1 July 16
    
    - [Speaker](https://x.com/efdevcon/status/1811428764586561641) & [volunteer](https://docs.google.com/forms/d/e/1FAIpQLSfs7S3ywsJ7MbDP30Lnn-_A6z-FiODtINnn-pwGL3c4jgsotw/viewform) applications are open
    
    - [Bangkok](https://devcon.org/en/city-guide/) city guide

- [EthCC](https://ethcc.io/archive) videos

- RicMoo’s[Firefly Pixie](https://x.com/ricmoo/status/1811760465581675008): open source hardware wallet

* * *

### Job Listings

- Nethermind: [Senior Device Security Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4336487101), Senior DevOps Engineer [AMER](https://boards.eu.greenhouse.io/nethermind/jobs/4363348101) & [APAC](https://boards.eu.greenhouse.io/nethermind/jobs/4363281101), [Full Stack Lead](https://boards.eu.greenhouse.io/nethermind/jobs/4356246101) APAC, [Post-Grad Internship](https://boards.eu.greenhouse.io/nethermind/jobs/4364252101) & [Chief Marketing Officer](https://boards.eu.greenhouse.io/nethermind/jobs/4363412101)

- EF seek a [European/Civil Law qualified Legal Counsel](https://jobs.lever.co/ethereumfoundation/204e2031-e60b-4c43-835a-e6837cef00b2)

- Aragon: [Senior Smart Contract Developer](https://jobs.lever.co/aragon/fba68080-9e98-49d7-8ed7-ac05d047d4b0)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 1.0 to 28.6 gwei, 3.6 gwei average; zero net issuance at 23.5 gwei 
    
    - 15k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,866 - $3,185, currently $3,133, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.054 (Flippening at ~0.164)

**Notable at app layer**

- [Multiple domains registered with Squarespace compromised](https://github.com/security-alliance/advisories/blob/main/2024-07-squarespace.pdf) including [Compound Labs](https://x.com/compoundfinance/status/1811624013841727702) & [Celer](https://x.com/CelerNetwork/status/1811394743794114866):
    - Google Domains users migrated to Squarespace should enable 2FA & remove excess contributor accounts

- Fileverse [dDocs](https://docs.fileverse.io/about): browser based word processor, end to end encrypted

**Regulation/business/tokens**

- [SEC formally notifies Paxos](https://x.com/paxos/status/1811405877733097703) that it will not be charged for BUSD

- [SEC Staff Accounting Bulletin 121](https://archive.is/9kGaw): SEC allows some exceptions to balance sheet reporting, House failed to overturn Presidential veto of repeal

- Republican party [adopts very pro-crypto platform](https://www.marketwatch.com/story/history-has-been-made-why-promises-by-trump-gop-platform-to-defend-crypto-are-a-big-deal-for-the-industry-17eeff8f)

- [Alex Pertsev denied bail](https://www.dlnews.com/articles/regulation/dutch-court-rejects-bail-for-tornado-cash-dev-alexey-pertsev/) to prepare for appeal

- [Roman Storm granted trial delay](https://www.therage.co/roman-storm-judge-grants-delay-of-tornado-cash-trial/) until December

**General**

- Tayvano: [example of a Lazarus attack](https://x.com/tayvano_/status/1810455262320570416), contact via socials and then compromise via GitHub repo

- [AT&T breach](https://www.sec.gov/ix?doc=/Archives/edgar/data/0000732717/000073271724000046/t-20240506.htm), data includes records of calls & texts of nearly all customers

- [Signal desktop](https://x.com/naomibrockwell/status/1809291643838951716) stores decryption key in plain text file, [encryption work started](https://github.com/signalapp/Signal-Desktop/pull/6849#issuecomment-2218845070) after backlash

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-july-13-2024](https://weekinethereumnews.com/week-in-ethereum-news-july-13-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jul 29-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 2-4 – [Ethereum Argentina](https://ethereumargentina.org/) conference & hackathon

- Aug 7-9 – [Science of Blockchain Conference](https://www.sbc-conference.com/) (New York)

- Aug 15-17 – [Ethereum Uruguay](https://www.ethereumuruguay.org/) hackathon & conference

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 23-26 – [ETHTokyo](https://www.ethtokyo.com/) hackathon & conference

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- Sep 5-8 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 9-15 – [ETHSafari](https://ethsafari.xyz/) (Kenya)

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 13-14 – [Ethereum México](https://ethmexico.org/)

- **Sep 20-22 –** [**ETHCapeTown**](https://www.ethcapetown.com/) **hackathon**

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Sep 26-27 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 4-6 – [Ethereum Kuala Lumpur](https://www.2024.ethkl.org/) conference & hackathon

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

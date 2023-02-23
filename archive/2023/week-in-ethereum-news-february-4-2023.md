---
title: "Week in Ethereum News <br> February 4, 2023"
date: "2023-02-04"
---

## Eth News and Links

**Shapella (Shanghai + Capella) upgrade**

- Zhejiang public testnet is live to test Shapella upgrade:
    - [Run a node](https://notes.ethereum.org/@launchpad/zhejiang) to test deposit, BLS change and exit
    
    - [3 faucets](https://zhejiang.ethpandaops.io/) to get Zhejiang testnet ETH
    
    - Guide to [run a Lighthouse+Geth node](https://github.com/eth-educators/ethstaker-guides/blob/main/zhejiang.md)
    
    - Zhejiang upgrades to Shapella on February 7

- Latest all core devs execution (ACDE) [call video](https://www.youtube.com/watch?v=E0w8NX5ksWo&t=169s).  Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1621209312050954240) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-execution-call-154/):
    - Withdrawals are coming: Sepolia testnet to be upgraded first after Zhejiang (due to smaller validator set) followed by Goerli testnet and then mainnet
    
    - Sepolia upgrade date to be selected next week at all core devs consensus call
    
    - EIP4844 discussions on precompile gas price benchmarking, zero blob transactions and decoupling blobs from blocks
    
    - Discussion on moving execution layer from RLP to SSZ

**Dencun (Cancun + Deneb) upgrade**

- KZG Ceremony:
    - [32,000+ contributors](https://ceremony.ethereum.org/), 4000+ in the lobby, still 30+ days in _first_ general contribution period
    
    - [C++ client implementation](https://github.com/PatriceVignola/cpp-kzg-ceremony-client#readme)

- Latest EIP4844 implementers [call video](https://www.youtube.com/watch?v=O1LLyKIMHUM). Notes from [Terence](https://twitter.com/terencechain/status/1620471913398280192)

**Layer 1**

- Patrick McCorry’s PoS series: [staker registration & withdrawal process](https://stonecoldpat.substack.com/p/registration-and-withdrawal-process)

- [OFAC impact on block builders](https://blog.toniwahrstaetter.com/builder-censorship.html): economically rational choice maybe building censored blocks

**Client releases**

- Consensus layer:
    - Lodestar [v1.4.0](https://blog.chainsafe.io/lodestar-v1-4-0-release-and-a-look-ahead-8f0a99c2e708): production ready; [v1.4.1](https://github.com/ChainSafe/lodestar/releases/tag/v1.4.1): hotfixes to discv5

- Execution layer:
    - Erigon [v2.37.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.37.0): bug fixes

**Research**

- [Benchmark zk proofs on AI primitives](https://medium.com/@ModulusLabs/chapter-5-the-cost-of-intelligence-da26dbf93307), using metrics of proof generation time & peak prover memory usage 

**Layer 2**

- Optimism’s [Bedrock upgrade explainer](https://community.optimism.io/docs/developers/bedrock/explainer/)

**EIPs/Standards**

- Tim Beiko’s proposal to [fork ERCs from EIPs repository](https://ethereum-magicians.org/t/proposal-forking-ercs-from-eips-repository/12804)

- [EIP6404](https://github.com/ethereum/EIPs/pull/6404/files): SSZ transactions, receipts and withdrawals

- [ERC6160](https://github.com/ethereum/EIPs/pull/6403/files): Multichain token

* * *

### **This newsletter is made possible thanks to** [**Hardhat**](https://hardhat.org/)**’s VSCode extension!**

![](https://weekinethereumnews.com/wp-content/uploads/2021/06/hardhat-rectangle-1024x325.png)

The Hardhat for Visual Studio Code extension adds comprehensive language support for Solidity to Visual Studio Code and enhances editor integration for Hardhat projects.  

Key features include code completion, go to definition, symbol renaming, and inline code validation from compiler errors/warnings. 

The extension also provides helpful code actions, hover help, and support for adding access modifiers and virtual/override keywords to function signatures. 

Get it from the [VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=NomicFoundation.hardhat-solidity)

* * *

**Stuff for developers**

- Solidity [v0.8.18](https://blog.soliditylang.org/2023/02/01/solidity-0.8.18-release-announcement/): Paris default EVM version, adds block.prevrandao & deprecates block.difficulty, adds flag to not append CBOR metadata, deprecates selfdestruct and improves bytecode generation from Yul

- [Codeslaw](https://www.codeslaw.app/): search verified contracts

- [ERC721X](https://github.com/indeliblelabs/contracts/blob/main/src/contracts/extensions/ERC721X.sol): ERC721 extension to auto expire transfer approvals after 30 days

- Guide to [libraries in Solidity](https://medium.com/@MarqyMarq/deep-dive-into-solidity-libraries-e9bd7f9061fb)

- Ape [v0.6.0](https://twitter.com/apeframework/status/1620843786497847296) (Python contract framework): beta support for Multicall3, adds per-function encode/decode methods and run scripts in nested subdirectories

- MatchboxDAO’s 0xMonaco race entries: [first](https://github.com/marktoda/monaco), [second](https://typefully.com/gretzke/DTU1xJn), [third](https://twitter.com/NotDeGhost/status/1619845952998887424) & [disqualified bug exploiter](https://twitter.com/zellic_io/status/1620844495226179586)

- Secureum RACE #14: [8 question Solidity quiz & answers](https://ventral.digital/posts/2023/1/30/race-14-of-the-secureum-bootcamp-epoch-infinity)

- CTF solutions using Ape & Vyper: [Ethernaut](https://github.com/0xJCN/Ethernaut-CTF), [Damn vulnerable DeFi](https://github.com/0xJCN/Damn-Vulnerable-DeFi-V3-CTF) & [EthernautDAO](https://github.com/0xJCN/EthernautDAO-Challenges)

- [Guide to using SMTChecker](https://www.truscova.com/blog_article_5.php) with Hardhat

- [Halmos](https://github.com/a16z/halmos#readme): symbolic testing reusing Foundry tests for formal verification

- [Wagmi CLI](https://twitter.com/wagmi_sh/status/1620097176738357248) (React hooks): generate code, connect to Foundry/Hardhat projects & create plugins

- [Universal bridge](https://github.com/ZeframLou/universal-bridge#readme): common interface to send a message to a supported network using official bridges

- [zkLLVM compiler](https://blog.nil.foundation/2023/02/02/circuit-compiler.html): circuit compiler for languages such as C/C++

- [Spartan-ecdsa](https://personaelabs.org/posts/spartan-ecdsa/): verify secp256k1 ECDSA signatures in zk, proofs in browser in 5 seconds

- [In-browser recursive proving & verification](https://twitter.com/nibnalin/status/1621059453570412544) added to Nova & Nova Scotia

**Security**

- Orion Protocol [$2.8 million exploit on Ethereum](https://twitter.com/BlockSecTeam/status/1621263393054420992) via reentrancy

- ENS subgraph [null byte vulnerability reversion](https://ens.mirror.xyz/9GN77d-MqGvRypm72FcwgxlUnPSuKWhG3rWxddHhRwM), lookalike domains couldn’t be distinguished using only the subgraph, $20k bounty paid

- Prestwich: [LayerZero trusted-party vulnerabilities](https://prestwich.substack.com/p/zero-validation), application default settings delegate trust to LayerZero multisig

**Ecosystem**

- Total Ether supply [post-merge making new lows](https://twitter.com/evan_van_ness/status/1620908514242871296) due to higher mainnet gas prices this week

- Jon Charbonneau: [Ethereum modeled in a spreadsheet](https://twitter.com/jon_charb/status/1619705380875169794)

**Enterprise**

- [European Investment Bank priced £50 million digital bond](https://www.eib.org/en/press/all/2023-030-eib-issues-its-first-ever-digital-bond-in-british-pounds) using Ethereum for transparency

- [zkEVM as execution framework](https://www.mesh.xyz/insights/the-zkevm-a-natural-execution-framework-for-enterprise-baseline-applications) for Baseline Protocol applications

**Application layer**

- OpenSea Seaport [v1.2](https://twitter.com/z0age/status/1621239991983816704): bulk listings, contracts as offerers, more powerful zones, improved events and optimizations

- [Sorare licensing deal](https://medium.com/sorare/sorare-partners-with-premier-league-to-launch-digital-player-cards-and-fantasy-competitions-c8b5c5e195b3) with Premier League for player NFTs and fantasy football

- [Crypto protocols](https://leighton.mirror.xyz/_Xx2iDckpjhz6JIGTbI-Fd9C9wFzaMunR4JFXEJemcs) are not companies nor DAOs

* * *

### Job Listings

- [Cyfrin.io](https://www.cyfrin.io/) is hiring [senior security engineers](https://github.com/ChainAccelOrg/SecurityEngineerReq) $190k-$300k.

- Arx, creators of KONG Cash and HaLo tags is hiring a [Solidity developer](https://arx.org/jobs).

- Ethereum Foundation are hiring a [Community Lead for ethereum.org](https://jobs.lever.co/ethereumfoundation/89ff5705-3351-422d-a5d1-b0805e95edec?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)

- [Lighthouse seeking support tech](https://github.com/sigp/positions-vacant/blob/master/lighthouse-support.md) to help its stakers

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [UK Treasury](https://www.gov.uk/government/consultations/future-financial-services-regulatory-regime-for-cryptoassets) to provide regulatory clarity for crypto, seeks comments by April 30

- [Australian Treasury](https://treasury.gov.au/consultation/c2023-341659) mapping crypto activities to existing regulation, feedback by March 3

- St Louis Federal Reserve: [Tornado Cash & privacy primer](https://research.stlouisfed.org/publications/review/2023/02/03/tornado-cash-and-blockchain-privacy-a-primer-for-economists-and-policymakers) for economists

- Celsius (CeFi lender) [bankruptcy examiners 476 page report](https://cases.stretto.com/public/x191/11749/PLEADINGS/1174901312380000000039.pdf) \[PDF\]

- ZachXBT: [FBI seize BAYC, Doodle & crypto](https://twitter.com/zachxbt/status/1621576193152634881) from alleged phishing scammer

**General/crypto**

- Nic Carter’s [guide to centralized exchanges Proof of Reserves](https://medium.com/@nic__carter/proof-of-reserves-for-policymakers-ae59c4b1f917) for policy makers

- [Ordinals NFTs on Bitcoin](https://read.pourteaux.xyz/p/illegitimate-bitcoin-transactions) using OP\_RETURN post Taproot make it [100x cheaper to stall the chain](https://dataalways.mirror.xyz/ql-UNhjNZ6M70g4KvDDVUvBZJDA6yMwwvYBFR8XN7Es)

- [Google Fi SIM swap attacks](https://www.bleepingcomputer.com/news/security/google-fi-data-breach-let-hackers-carry-out-sim-swap-attacks/) after data breach

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-february-4-2023](https://weekinethereumnews.com/week-in-ethereum-news-february-4-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Feb 24 - Mar 1 – [ETHDenver BUIDLWeek](https://www.ethdenver.com/)

- Feb 27 – deadline for [EF academic grants round](https://esp.ethereum.foundation/academic-grants-2023)

- Mar 2-5 – [ETHDenver Hackathon](https://www.ethdenver.com/)

- Mar 10-29 – [Scaling Ethereum](https://ethglobal.com/events/scaling2023) (ETHGlobal) virtual

- Mar 15-16 – [ETHDubai](https://www.ethdubaiconf.org/)

- Mar 16-18 – [ETH Porto](https://ethporto.org/)

- Mar 28-30 – [Ethereum Rio](https://www.ethereumbrasil.com/ethereumrio)

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- Apr 14-16 – [ETHGlobal Tokyo](https://tokyo.ethglobal.com/)

- Apr 14-16 – [ETHZurich](https://ethereumzuri.ch/) conference & hackathon

- Apr 21-23  – [EthTaipei](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) hackathon

- Apr 24-25  – [EthTaipei](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) conference

- **Apr 27-30  –** [**Istanbul ETH Privacy**](https://www.leadingprivacy.com/istanbul) **conference & hackathon**

- May 5-7 – [ETHMalaysia](https://ethmalaysia.com/) conference & hackathon

- **May 19-23 – [Edcon](https://edcon.io/) Podgorica, Montenegro**

- May 20-21 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- **May 24-26 –** [**Spaghett ETH**](https://naples.spaghett-eth.com/) **(Naples) conference**

- May 26–28 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Jun 23–25 – [ETHGlobal Toronto](https://ethglobal.com/events/toronto)

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–25 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

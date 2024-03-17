---
title: "Week in Ethereum News <br> March 16, 2024"
date: "2024-03-16"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- Mainnet successfully [upgraded to Dencun](https://twitter.com/parithosh_j/status/1767973626987606190)
    - Consensus-specs [v1.4.0](https://github.com/ethereum/consensus-specs/releases/tag/v1.4.0) for Dencun mainnet release

- EIP4844 (blobs)
    - Layer 2:
        - L2 fees drop to cents & below: [L2 Fees](https://l2fees.info/), [Gas Fees](https://www.gasfees.io/) & [grow the pie](https://fees-growthepie.streamlit.app/)
        
        - L2s using blobs: [zkSync Era](https://twitter.com/zksync/status/1767983026443579448), [Starknet](https://twitter.com/starknet/status/1767915153700290839), [Optimism](https://twitter.com/Optimism/status/1768076340803367305) & [Base](https://twitter.com/jessepollak/status/1768071129854562698), Zora, [Mode](https://twitter.com/JRossTreacher/status/1768193428641181830), [Arbitrum](https://twitter.com/arbitrum/status/1768306107318178061) and [Paradex](https://twitter.com/tradeparadex/status/1768306190596153799)
        
        - L2Beat [data availability](https://l2beat.com/scaling/data-availability) dashboard
        
        - Dune blob dashboards: [Hildobby](https://dune.com/hildobby/blobs) and [0xRob](https://dune.com/0xRob/blobs)
    
    - View blobs on [Blobscan](https://blobscan.com/) & [Etherscan](https://twitter.com/etherscan/status/1767970586146533449)
    
    - Finematics [EIP4844 explainer](https://finematics.com/eip-4844-explained/)
    
    - Reminder: write a data blog post for [EF EIP4844 data challenge](https://esp.ethereum.foundation/data-challenge-4844)

**Pectra (Prague + Electra) upgrade (meta** [**EIP7600**](https://eips.ethereum.org/EIPS/eip-7600)**)**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=US8T0ZoGF8s&t=109s). Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1768377163554897955) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-183/):
    - **Pectra upgrade** (small fork targeting late 2024)
        - **EIP2537 BLS**: discussions on adding decompress precompiles & exposing operations
        
        - **Potential EIP discussions** (but no decisions yet on what else to include):
            - **EIP3074 AUTH/AUTHCALL opcodes**: Dan Finlay (MetaMask) [case for](https://twitter.com/danfinlay/status/1768291044683288808)
            
            - **EIP7547 inclusion lists**: breakout call Monday
            
            - **EIP7623 increase CALLDATA cost**: [analysis](https://ethresear.ch/t/analyzing-eip-7623-increase-calldata-cost/19002), need feedback from L2s
            
            - **EIP7645 alias ORIGIN to SENDER**: alternatively raise price

- [EIP6110 supply validator deposits onchain](https://ethereum2077.substack.com/p/eip-6110-supply-validator-deposits-onchain) explainer

- [Case for inclusion lists](https://notes.ethereum.org/@mikeneuder/the-case-for-ilectra) (EIP7547) in Electra

* * *

**This newsletter is sponsored by** [**Pashov Audit Group**](https://www.pashov.net/)**!** 

![Pashov Audit Group](https://weekinethereumnews.com/wp-content/uploads/2024/03/Pashov-Audit-Group-1024x341.webp)

Are you developing a blockchain protocol? Make sure to get a high-quality audit. Audits are not silver bullets, but a good one drastically decreases the chances of a successful attack. An “internal review” by your developers is not an audit. Without a formal one many users won’t trust your protocol because you are putting their funds at risk.

In Pashov Audit Group we know for a fact that we can help you secure your code in a painless, high-quality and express manner. We are looking for established projects who invest in security and are looking for the highest quality security partner.

We still have a couple of slots available over the next couple of months. Reach out for security help - [pashov.net](https://www.pashov.net/)

* * *

**Osaka + F starname upgrade (meta** [**EIP7607**](https://eips.ethereum.org/EIPS/eip-7607)**)**

- Verkle implementers [call video](https://www.youtube.com/watch?v=0Zd4zK2Zupg) & [notes](https://twitter.com/rudolf6_/status/1767565116101525567):
    - Kaustinen-5 testnet soon
    
    - DoS vector means [clients need to handle trie depth of 14-16](https://notes.ethereum.org/hmqCk1tiTq6TdrxO_CKhuw)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 30.81%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth 72% supermajority, could cause a chain split
    
    - Consensus layer: **Prysm 38%**, any client bug over 33.3% could mean loss of finality
    
    - [**Prysm bug found on Goerli testnet**](https://twitter.com/potuz_eth/status/1768418899111113125) **highlights need for client diversity**

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- [Reth](https://www.paradigm.xyz/2024/03/reth-beta) (Rust based execution layer client) now in beta

- [Grandine](https://medium.com/@grandine/grandine-is-open-sourced-b1815cf0ae39) (Rust based consensus layer client), open sourced with GPL v3.0 license

- Vitalik: [quantum emergency upgrade plan](https://ethresear.ch/t/how-to-hard-fork-to-save-most-users-funds-in-a-quantum-emergency/18901) to save most user funds 

**Client Releases**

- Consensus layer:
    - Lighthouse [v5.1.1](https://github.com/sigp/lighthouse/releases/tag/v5.1.1): hotfix
    
    - Lodestar [v1.17.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.17.0): optimization update
    
    - Prysm [v5.0.1](https://github.com/prysmaticlabs/prysm/releases/tag/v5.0.1): minor patch release

- Execution layer:
    - Reth [v0.2.0-beta.2](https://github.com/paradigmxyz/reth/releases/tag/v0.2.0-beta.2): resync required upgrading from alpha; [v0.1.0-alpha.22](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.22): bug fix

**For Stakers**

- Stereum [v2.1](https://github.com/stereum-dev/ethereum-node/releases/tag/v2.1.0) (node launcher): adds Obol support and SSV Network encrypted keys

**Research**

- [Stake distribution analysis](https://ethresear.ch/t/initial-analysis-of-stake-distribution/19014): change in issuance won’t change staking distribution

- [Data availability sampling strategies](https://ethresear.ch/t/lossydas-lossy-incremental-and-diagonal-sampling-for-data-availability/18963): lossy, incremental and diagonal sampling

**Layer 2**

- Blast [stopped producing blocks](https://twitter.com/Blast_L2/status/1767933586487890427) after mainnet Dencun upgrade, resolved

**EIPs/Standards**

- EIPs:
    - [EIP7650](https://eips.ethereum.org/EIPS/eip-7650): Programmable access lists

- ERCs (application layer):
    - [ERC7651](https://github.com/ethereum/ERCs/pull/305/files): Fractionally represented NFT
    
    - [ERC7652](https://github.com/ethereum/ERCs/pull/306/files): ERC721 guarantee extension
    
    - [ERC7653](https://github.com/ethereum/ERCs/pull/320/files): Named NFT (ERC721 extension)
    
    - [ERC7654](https://github.com/ethereum/ERCs/pull/315/files): Request method types
    
    - [ERC7655](https://github.com/ethereum/ERCs/pull/318/files): ERC5189 operation receipts

**Stuff for developers**

- Solidity [v0.8.25](https://soliditylang.org/blog/2024/03/14/solidity-0.8.25-release-announcement/): Cancun default EVM version, MCOPY used in code generator and TSTORE usage warnings reduced to once per compilation

- Remix [v0.45.0](https://medium.com/remix-ide/remix-release-v0-45-0-dcb16ff6bf03): pin deployed contracts, VM state is saved and fetch code for Blockscout verified contracts

- Hardhat [v2.22.1](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.22.1): Hardhat Ignition default deployment system; [v2.22.0](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.22.0): Cancun default EVM version for Hardhat Network

- [Ethernaut-cli](https://github.com/theethernaut/ethernaut-cli#readme) (tool box): AI (requires OpenAI API key), utils, Hardhat tasks and Ethernaut challenges; alpha

- Foundry:
    - Forge-std [v1.8.0](https://github.com/foundry-rs/forge-std/releases/tag/v1.8.0): uses native assertions, supports packed variables, adds TOML read/write cheatcodes, native string manipulation cheatcodes and implements interfaces in mock tokens
    
    - Tip: [console.log to debug a deployed contract](https://twitter.com/bytes032/status/1766857786258825373) using vm.etch on a fork

- [Evm.codes](https://www.evm.codes/?fork=cancun) adds Cancun opcodes

- Tincho: [solc skips code size check](https://blog.theredguild.org/a-call-a-precompile-and-a-compiler-walk-into-a-bar/) for external calls with return data, including precompiles

- web3py [middleware](https://snakecharmers.ethereum.org/web3py-middleware/) (v7 beta): class-based middleware replaces functional programming paradigm

- micro-eth-signer [v0.8](https://github.com/paulmillr/micro-eth-signer/releases/tag/0.8.0): adds EIP4844 blob transaction support

- Curta CTF [CurtaLending solution](https://www.curta.wtf/puzzle/base:7/write-up)

- [Node Guardians](https://twitter.com/nodeguardians/status/1768362572699271389) (gamified learning) adds Solidity & Huff quests

- Reminder: supported testnets
    - [Sepolia](https://github.com/eth-clients/sepolia#readme): use for application layer testing
    
    - [Holešky](https://github.com/eth-clients/holesky#readme): use for staking & infrastructure testing
    
    - [Ephemery](https://ephemery.dev/): use for testing validator setups

**Security**

- Unizen [$2.1M exploit](https://rekt.news/unizen-rekt/) via external call vulnerability after contract upgrade

- Mozaic [$2M drained](https://twitter.com/Mozaic_Fi/status/1768754080271196178) by malicious developer using private key

- Blastoff (yield aggregator) [150 ETH exploit](https://twitter.com/blastozone/status/1767104856609673667) on Blast

- Juice staking [54 ETH exploit](https://medium.com/@juicebotapp/juice-staking-exploit-next-steps-95e218b3ec71)

- [FindAudit](https://twitter.com/bytes032/status/1767206788061954395): p2p security marketplace

**Ecosystem**

- EF Devcon Bangkok venue: [Queen Sirikit National Convention Center](https://blog.ethereum.org/2024/03/14/devcon-sea-venue)

* * *

### Job Listings

- Certora is hiring: [Head of Product](https://hubs.ly/Q02n-d-X0), [SR-Rust](https://hubs.ly/Q02n-fmD0), [Compiler Developer](https://hubs.ly/Q02n-b_20), [FV Wizard](https://hubs.ly/Q02n-fyx0).

- 🔥OpenZeppelin is hiring: [Open Source Development Manager](https://grnh.se/49275c7e3us) & [Product Manager](https://grnh.se/6bc6836b3us)

- [IFT](https://free.technology/)/[Logos](https://logos.co/): [ZK Researcher](https://boards.greenhouse.io/nomos/jobs/5664663) (Nomos); [ZK Researcher](https://boards.greenhouse.io/vac/jobs/5453093) (Vac) & [ZK Engineer](https://boards.greenhouse.io/vac/jobs/5543856) x2

- ChainSafe seek a [Head of Protocol Engineering](https://grnh.se/c6e27e794us)

- [Waku](https://waku.org/about) is hiring! [Protocol Engineer](https://grnh.se/a240b11b1us), [Waku SDK Software Engineer](https://grnh.se/0a63ae031us) & [Researcher](https://grnh.se/b96ad7111us)

- [TechOps](https://techops.services) are looking for [DevOps](https://apply.workable.com/techops-services/j/5AD8CF90E0/). Work on projects such as MakerDAO.

- Devcon: [Community Supporter](https://jobs.lever.co/ethereumfoundation/6ad3d8e7-17cb-4d5c-820d-c279e8002551), [Production Magician](https://jobs.lever.co/ethereumfoundation/aa4c69f8-f564-4036-9c5e-3e09f0eb27df) & [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/e93dae67-65a6-495c-8638-46e3db28cb64)

- Nethermind: [Distributed Systems Dev Lead](https://grnh.se/c3fd6842teu) & [Cryptography Researcher](https://grnh.se/51fa8652teu)

- [Sr. Developer Relations Manager](https://wellfound.com/jobs/2933743-sr-developer-relations-manager-at-powerloom-protocol) & [Technical Writer](https://wellfound.com/jobs/2931135-technical-writer-at-powerloom-protocol) at [Powerloom](https://powerloom.io/)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 21.9 to 190.0 gwei, with 55.3 gwei average
    - Zero net issuance currently at 22.9 gwei 
    
    - 25k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,590 - $4.071, currently $3,743

- [ETHBTC](https://ratiogang.com/): currently 0.054 (Flippening at ~0.16)

**Notable at app layer**

- Maker [roadmap](https://forum.makerdao.com/t/makerdao-endgame-launch-season/23857): phase 1 (mid year): launch new brand, stable & governance tokens, lockstake engine and Spark SubDAO; phase 2: scale; phase 3; new L1; phase 4: end game

- Optimism [We ❤️ The Art](https://optimism.mirror.xyz/I6g_dbBkZXxCiKNS0lp0Zul-qhzjtnbvjHTv5y6B_dU) NFT winners

- [Internet of Agents research](https://davidecrapis.notion.site/The-Internet-of-Agents-23aa09799b9c4620a1a287926bcfd6af) into AI agents running on blockchain infrastructure

**Regulation/business/tokens**

- [Ethereum institutional thesis](https://www.bitooda.io/research/ethereum-institutional-thesis-a-store-of-value-with-cash-flow): a store of value with cash flow 

- [London Stock Exchange](https://docs.londonstockexchange.com/sites/default/files/documents/crypto_etn_admission_factsheet.pdf) accepting applications for ETH Exchange Traded Notes (ETNs)

- FT: [Nigeria pressing Binance](https://archive.is/2024.03.12-184145/https://www.ft.com/content/9c1394de-0492-4597-b075-cbf19e0b6e83) for info on top 100 users, 2 staff being held

- [Roman Sterlingov](https://www.justice.gov/opa/pr/bitcoin-fog-operator-convicted-money-laundering-conspiracy) convicted in US for operating Bitcoin Fog mixer
    - Professor J.W. Verret says [Sterlingov was merely an early user](https://cointelegraph.com/news/bad-blockchain-forensics-convict-roman-sterlingov)

- [US Copyright Office & PTO](https://newsroom.loc.gov/news/u.s.-copyright-office-and-u.s.-patent-and-trademark-office-conclude-joint-study-on-non-fungible-toke/s/b0780cc9-0e6c-42fb-90a6-31eaf061434c): new laws not required for infringement related to NFTs

- Paradigm: [19% of US registered voters bought crypto](https://policy.paradigm.xyz/writing/March-2024-Polling)

**General**

- [Summer of Protocols 2024](https://summerofprotocols.com/research/sop2024) applications open for protocol improvement grants, protocol pill challenge & partner program

- [UK High Court judge ruled Craig Wright is not Satoshi](https://www.opencrypto.org/2024-03-14-Justice-Mellor-Rules-That-Craig-Wright-Is-Not-Satoshi-Nakamoto-in-COPA-v-Wright-Trial/) in COPA v Wright trial

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-march-16-2024](https://weekinethereumnews.com/week-in-ethereum-news-march-16-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Mar 18 – [ZK grants round](https://esp.ethereum.foundation/zk-grants) application deadline

- Mar 19-21 – [ETH Canal](http://ethcanal.xyz) (Panama City, Panamá) conference & hackathon

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- Mar 22-24 – [ETHSamba](https://ethsamba.org/) (Rio) hackathon

- Mar 24-29 – [Ethaly](http://ethaly.io/) (Savelletri di Fasano, Italy)

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) conference & hackathon

- Mar 29-31 – [ETH Seoul](https://www.ethseoul.org/) hackathon

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) virtual hackathon

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Apr 12-14 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- Apr 16-18 – [EY Global blockchain summit](https://web.cvent.com/event/e0ad2c12-3e65-41a9-bafb-a436754cf4ae/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7) (London)

- Apr 19-21 – [ETH Tallinn](https://www.ethtallinn.org/) hackathon

- Apr 26-28 – [ETHBoston](https://ethboston.xyz/) conference & hackathon

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/) hackathon

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- May 31-Jun 5 – [ETH Belgrade](https://ethbelgrade.rs/) hackathon & conference

- Jun 14 – [EF EIP4844 data challenge](https://esp.ethereum.foundation/data-challenge-4844) deadline

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 26-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Oct 6-8 – [ETHRome](https://ethrome.org/)

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

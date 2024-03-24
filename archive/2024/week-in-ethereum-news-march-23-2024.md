---
title: "Week in Ethereum News <br> March 23, 2024"
date: "2024-03-22"
---

## Eth News and Links

**Pectra (Prague + Electra) upgrade (meta** [**EIP7600**](https://eips.ethereum.org/EIPS/eip-7600)**)**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=3rRJ1H0MJDY&t=432s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-130/):
    - Proposal to set default local block boost to 10%
    
    - **Pectra upgrade** (small fork targeting late 2024)
        - **EIP7251 maxEB** (increase max effective balance): added to Pectra
        
        - **EIP7547 IL (inclusion lists)**: considered for inclusion in Pectra, review in 4 weeks, doing both maxEB + IL increases upgrade complexity and deprioritizes peerDAS
        
        - **EIP7659 increase blob throughput** proposal to increase to target of 8 & maximum of 16 blobs per block (up from 3/6) over 4 months
        
        - **Light client proposals**: EIP7658 light client data backfill & EIP7657 sync committee slashings
    
    - P2P proposals: network shards, IDONTWANT control message & deprecate mplex

- EIP7251 maxEB (increase max effective balance):
    - Breakout call [notes](https://hackmd.io/@philknows/BkEL0Fu0p)

- EIP7547 IL (inclusion lists):
    - Breakout [call video](https://www.youtube.com/watch?v=GVdkDXZTtnw&t=145s) and [notes](https://hackmd.io/@ttsao/Bkg53AHAT): plan to finalize proof of concept (PoC) specs, begin client PoC implementations & interop on a devnet
    
    - Terence: [changes to support blob transactions](https://hackmd.io/@ttsao/ryzAw9PRa) within existing IL design

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 30.59%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: **Geth 66% majority**
        - [**Coinbase**](https://twitter.com/coinbasecloud/status/1770866720246219152) **migrated to ~50% Nethermind**
        
        - **Geth** [**vulnerability disclosed**](https://blog.ethereum.org/2024/03/21/sepolia-incident)**: all EL clients updated to safe RPC limits**
        
        - **Nethermind** [**post mortem**](https://hackmd.io/@nethermindclient/ByW9sX_R6) **of January block processing issue**
    
    - Consensus layer: Prysm 38% majority
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Eric Conner & Mariano Conti [campaign to raise the gas limit to 40M](https://pumpthegas.org/)

- [Calldata.pics](https://calldata.pics/): live charts of calldata & blob usage

- ethPandaOps:
    - [Attacknet](https://ethpandaops.io/posts/attacknet-introduction/): inject faults into a devnet, uses Kurtosis & Chaos Mesh
    
    - [Dencun upgrade analysis](https://ethpandaops.io/posts/dencun-fork-analysis/): open questions on reorg rate, attestation effectiveness & safely increasing blob parameters

- [Dencun diary](https://stateful.mirror.xyz/x7uPWur2ELBP6jkKEILKhAwPCJvCv10s3UrS1y1qpcc): contributor reflections, future priorities & improvement suggestions 

**Client Releases**

- Consensus layer:
    - Lighthouse [v5.1.2](https://github.com/sigp/lighthouse/releases/tag/v5.1.2): hotfix for block lookup duplicate requests and to stop propagation of slashings for slashed attesters 

- Execution layer:
    - Erigon [v2.59.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.59.0): post Dencun fixes
    
    - Reth [v0.2.0-beta.3](https://github.com/paradigmxyz/reth/releases/tag/v0.2.0-beta.3): fix critical in static files that could lead to inconsistent storage state

**Research**

- [Discouragement attack](https://medium.com/@nfett/addressing-systemic-risks-discouragement-attacks-against-centralized-validator-sets-d95769da4bb8) against centralized validator sets

**Layer 2**

- [Optimism fault proofs](https://blog.oplabs.co/open-source-and-feature-complete-fault-proofs-bring-permissionless-validation-to-the-op-sepolia-testnet/) live on OP Sepolia testnet

**EIPs/Standards**

- EIPs:
    - [EIP7657](https://github.com/ethereum/EIPs/pull/8340/files): Sync committee slashings
    
    - [EIP7658](https://github.com/ethereum/EIPs/pull/8341/files): Light client data backfill
    
    - [EIP7659](https://github.com/ethereum/EIPs/pull/8343/files): Stepwise blob throughput increase

- ERCs (application layer):
    - [ERC7656](https://github.com/ethereum/ERCs/pull/327/files): Generalized token-linked contracts

**Stuff for developers**

- Etherscan [contract verification updated](https://twitter.com/etherscan/status/1769688918780416342): multichain verification with single API key and suggest name tags, labels & URL

- OpenSea [Seaport v1.6](https://opensea.io/blog/articles/introducing-seaport-1-6): adds Seaport hooks

- [555 NFT](https://github.com/fiveoutofnine/555#readme): onchain audio & SVG

- Guide to [implementing stateful invariant testing](https://a16zcrypto.com/posts/article/implementing-stateful-invariant-testing-with-halmos/) with Halmos

- [Ethernaut-cli](https://mirror.xyz/theethernaut.eth/0HP3L4mWzb4isXYERfsncBQgzT1T99uQTH8tvJvICmE) (tool box): built on Hardhat tasks, AI requires OpenAI API key; beta

- [Ec](https://github.com/ralexstokes/ethereum-consensus/blob/main/ethereum-consensus/src/bin/ec/README.md) (Rust library): convert bytes into minimal number of blobs

- [Lodestar Prover](https://blog.chainsafe.io/introducing-lodestar-prover/): middleware wrapper around light client for dapps

- CTFs:
    - OpenZeppelin [Ethernaut CTF 2024](https://github.com/OpenZeppelin/ctf-2024#readme) challenges & solutions

- Cyfrin Updraft adds [web3 DevOps](https://updraft.cyfrin.io/courses/wallet-and-deployment) & [Assembly & Formal Verification](https://updraft.cyfrin.io/courses/formal-verification) courses

- Reminder: [Goerli testnet](https://blog.ethereum.org/2023/11/30/goerli-lts-update) sunsets Apr 17, most validators have shutdown, opportunity to [research long-range attacks](https://twitter.com/jcksie/status/1771161091919192503)
    - Use [Sepolia testnet](https://github.com/eth-clients/sepolia#readme) for application layer testing

**Security**

- Super Sushi Samurai [$4.8M exploit](https://rekt.news/sss-rekt/) on Blast via transferring to self to double balance, [white hat](https://twitter.com/SSS_HQ/status/1771168070054375596)

- Dolomite [$1.8M exploit](https://twitter.com/dolomite_io/status/1770499040741859645) of old contracts, revoke approvals

- ParaSwap [Augustus V6 contract vulnerability](https://twitter.com/paraswap/status/1770313086072742263), white hat, revoke approvals

- AirDAO [LP drained](https://twitter.com/airdao_io/status/1770713655530651687) via social engineering

- [Finding an ERC4626 vault reentrancy](https://twitter.com/hoshiyari420/status/1770819387433377940), $3M was at risk

- Trail of Bits: [weAudit](https://blog.trailofbits.com/2024/03/19/read-code-like-a-pro-with-our-weaudit-vscode-extension/) (VSCode extension), collaborative note taking & highlight code regions

**Ecosystem**

- Pascal Caversaccio: [Ethereum cypherpunk manifesto](https://hackmd.io/@pcaversaccio/the-ethereum-cypherpunk-manifesto)

- [ETHGlobal London](https://twitter.com/ethglobal/status/1769417544329240965) hackathon winners

**Enterprise**

- [Enterprise Ethereum Alliance](https://entethalliance.org/enterprise-ethereum-alliance-announces-new-leadership-and-vision/) new leadership team: Karen Scarbrough - Executive Director, Paul Brody - Chairperson and Vanessa Grellet joins board

- [Google search](https://www.google.com/search?q=ethereum.eth) for an ENS address shows Ether balance

* * *

### Job Listings

- [Waku](https://waku.org/about) is hiring! [Protocol Engineer](https://grnh.se/a240b11b1us), [Waku SDK Software Engineer](https://grnh.se/0a63ae031us) & [Researcher](https://grnh.se/b96ad7111us)

- [IFT](https://free.technology/)/[Logos](https://logos.co/): [ZK Researcher](https://boards.greenhouse.io/nomos/jobs/5664663) (Nomos); [ZK Researcher](https://boards.greenhouse.io/vac/jobs/5453093) (Vac) & [ZK Engineer](https://boards.greenhouse.io/vac/jobs/5543856) x2

- Certora is hiring: [Head of Product](https://hubs.ly/Q02n-d-X0), [SR-Rust](https://hubs.ly/Q02n-fmD0), [Compiler Developer](https://hubs.ly/Q02n-b_20) & [FV Wizard](https://hubs.ly/Q02n-fyx0)

- Devcon: [Community Supporter](https://jobs.lever.co/ethereumfoundation/6ad3d8e7-17cb-4d5c-820d-c279e8002551), [Production Magician](https://jobs.lever.co/ethereumfoundation/aa4c69f8-f564-4036-9c5e-3e09f0eb27df) & [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/e93dae67-65a6-495c-8638-46e3db28cb64)

- 👾OpenZeppelin seeks Security Researchers in [Canada](https://grnh.se/3d8f61e53us), [Australia](https://grnh.se/bb2348b83us), [LatAm](https://grnh.se/3b4915233us) & [USA](https://grnh.se/54d2bd163us)

- [TechOps](https://techops.services) are looking for [DevOps](https://apply.workable.com/techops-services/j/5AD8CF90E0/). Work on projects such as MakerDAO.

- ChainSafe seek a [Head of Protocol Engineering](https://grnh.se/c6e27e794us)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 16.4 to 121.8 gwei, with 32.4 gwei average
    - Zero net issuance currently at 22.8 gwei 
    
    - 7k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,107 - $3,757, currently $3,305

- [ETHBTC](https://ratiogang.com/): currently 0.052 (Flippening at ~0.16)

**Notable at app layer**

- [BlackRock](https://securitize.io/learn/press/blackrock-launches-first-tokenized-fund-buidl-on-the-ethereum-network) USD institutional digital liquidity fund (BUIDL), stable token pays dividends in tokens monthly for qualified investors

- Nexus Mutual [bundled protocol cover](https://nexusmutual.io/blog/bundled-protocol-cover-is-live), protection for multiple protocols under a single listing

**Regulation/business/tokens**

- [Ethereum is first (“profitable”) chain](https://twitter.com/tokenterminal/status/1770169951057572340) where burned transaction fees are greater than lifetime issuance

- Fortune: [SEC issues subpoenas](https://archive.is/ZNt54) regarding dealings with EF
    - [EF removed warrant canary](https://github.com/ethereum/ethereum-foundation-website/commit/769b30603504b4b5e8f601f8014691a8d1821390) from website in Feb 26 commit: “received a voluntary enquiry from a state authority that included a requirement for confidentiality”

- [SEC sanctioned](https://twitter.com/iampaulgrewal/status/1769835308559032608) for bad faith conduct in DEBT Box case

- [Genesis](https://www.sec.gov/news/press-release/2024-37) $21M settlement with SEC for charges of unregistered offer & sale of securities

**General**

- [Polygon PoS](https://twitter.com/0xpolygon/status/1770512885657080137) added secp256r1 curve precompile (RIP7212)

- [GoFetch](https://gofetch.fail/): side channel attack using data memory-dependent prefetchers in Apple silicon

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-march-23-2024](https://weekinethereumnews.com/week-in-ethereum-news-march-23-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) conference & hackathon

- Mar 29-31 – [ETH Seoul](https://www.ethseoul.org/) hackathon

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) virtual hackathon

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Apr 12-14 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- Apr 16-18 – [EY Global blockchain summit](https://web.cvent.com/event/e0ad2c12-3e65-41a9-bafb-a436754cf4ae/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7) (London)

- Apr 19-21 – [ETH Tallinn](https://www.ethtallinn.org/) hackathon

- **Apr 23-May 7 –** [**Gitcoin Grants 20**](https://twitter.com/gitcoin/status/1768725669377118479)

- Apr 26-28 – [ETHBoston](https://ethboston.xyz/) hackathon & conference

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

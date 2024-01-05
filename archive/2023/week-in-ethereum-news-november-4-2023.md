---
title: "Week in Ethereum News <br> November 4, 2023"
date: "2023-11-03"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=dAStyB2Vv4s&t=330s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-121/):
    - Agreed to Deneb simplification (blob sidecar inclusion proof), ~3 weeks to implement, delays next devnet but gives safer mainnet
    
    - [**Devnet 11**](https://dencun-devnet-11.ethpandaops.io/) launched

- Consensus-specs [v1.4.0-beta.4](https://github.com/ethereum/consensus-specs/releases/tag/v1.4.0-beta.4): adds blob sidecar inclusion proof

- Dencun interop testing [call video](https://www.youtube.com/watch?v=C8757wvksr0&t=14s)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.34%**](https://dune.com/hildobby/eth2-staking) **continues to reduce but still far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~85% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm 43% & Lighthouse 34%, any client bug over 33.3% could mean loss of finality

- [Geographic diversity needed for stakers & nodes](https://nodewatch.io/), particularly outside of US/Canada/EU

**Layer 1**

- Guide to [run Reth](https://blog.merkle.io/blog/run-a-reth-node) (Rust EL client) + Lighthouse on Ubuntu v20.04

- [Node on Playstation 4](https://notes.ethereum.org/@MarioHavel/EthereumOnPS): syncs Holešky testnet

- Verkle implementers call [notes](https://twitter.com/rudolf6_/status/1719755477121372563)

**For Stakers**

- Beacon chain: [millionth validator index number](https://beaconcha.in/validator/1000000) assigned

**Client releases**

- Execution layer:
    - [EthereumJS releases](https://x.com/EFJavaScript/status/1720039238232588608): Holešky testnet support, Dencun devnet 11 support & EVM profiler

**Research**

- [CeFi-DeFi arbitrage influence](https://ethresear.ch/t/the-influence-of-cefi-defi-arbitrage-on-order-flow-auction-bid-profiles/17258) on order-flow auction (OFA) bid profiles

**Layer 2**

- Vitalik: [types of layer 2s](https://vitalik.eth.limo/general/2023/10/31/l2types.html), rollup & validium spectrum, dimensions of withdrawing security & reading security

**EIPs/Standards**

- EIPs
    - [EIP7547](https://github.com/ethereum/EIPs/pull/7943/files): Inclusion lists
    
    - [EIP7549](https://github.com/ethereum/EIPs/pull/7944/files): Move committee index outside Attestation

- ERCs (application layer):
    - [ERC7548](https://github.com/ethereum/ERCs/pull/77/files): Open IP protocol (remix ERC721 NFTs)
    
    - [ERC7550](https://github.com/ethereum/ERCs/pull/81/files): Transient ERC20 approvals
    
    - [ERC7551](https://github.com/ethereum/ERCs/pull/85/files): Crypto security token contract interface
    
    - [ERC7552](https://github.com/ethereum/ERCs/pull/87/files): Decentralized embedding registry

**Stuff for developers**

- Hardhat:
    - Hardhat [v2.19.0](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.19.0): adds configuration variables (stored in plain text)
    
    - Guide to [deploying a contract with Hardhat Ignition](https://medium.com/nomic-foundation-blog/how-to-automate-a-headache-free-deployment-with-hardhat-ignition-fb2936ae2cfb)

- [Gaslite Splitter](https://github.com/PopPunkLLC/gaslite-core/blob/main/src/GasliteSplitter.sol): gas optimized contract for splitting ERC20 & ETH payments

- [Solid-grinder](https://github.com/Ratimon/solid-grinder#readme): reduce L2 gas cost by encoding calldata, front end snippets & CLI

- [Reinforced-Concrete-Huff](https://github.com/rymnc/reinforced-concrete-huff#readme): hash function for bn254 curve, ported to Huff

- Fe (language) [v0.26.0](https://github.com/ethereum/fe/releases/tag/v0.26.0): option to produce runtime bytecode and verify onchain contracts against local source code

- [Addreth](https://github.com/bpierre/addreth#readme): React component to display ETH addresses

- [Web3py-discord-bot](https://github.com/wolovim/web3py-discord-bot#readme): example repo using web3.py websocket provider

- Paradigm CTF [write up](https://twitter.com/kalos_security/status/1719977150928032002) (from 2nd placed Kalos)

- [Securing C (language) code](https://blog.ethereum.org/2023/11/02/writing-robust-c): best practices used to secure c-kzg-4844 C library 

**Security**

- Onyx protocol (Compound v2 fork) [$2.1M exploit](https://rekt.news/onyx-protocol-rekt/) via precision loss vulnerability

- Unibot router [$600k exploit](https://rekt.news/unibot-rekt/) via suspected lack of input validation allowing arbitrary call

- Astrid Finance [$230K exploit](https://twitter.com/MetaSec_xyz/status/1718229037460730260) via lack of input validation in withdraw

**Ecosystem**

- ETHGlobal [ETHOnline finalists](https://twitter.com/ETHGlobal/status/1717944373713973732)

- Gitcoin Grants 19 [applications open](https://grants.gitcoin.co)

- Etherscan [address highlighting](https://twitter.com/etherscan/status/1720401243728928982) on hover

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 7.4 to 95.2 gwei, with 21.1 gwei average
    - Zero net issuance currently at 21.6 gwei 
    
    - 450 ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $1,774 - $1,865, currently $1,828

- [ETHBTC](https://ratiogang.com/): currently 0.053 (Flippening at ~0.16)

**Notable at app layer**

- [WalletConnect](https://twitter.com/pedrouid/status/1720526568701800811) reenabling access to Russia & occupied Ukraine after previously blocking based on legal & OFAC guidance

- [Aragon Association](https://blog.aragon.org/a-new-chapter-for-the-aragon-project/) dissolving

- [Drawtech](https://twitter.com/0xsmallbrain/status/1719550772244033935) live on Base, shared canvas onchain mobile game

- [OpenSea](https://twitter.com/nadavahollander/status/1720524932369547671) staff layoffs

* * *

### Job Listings

- Nethermind: [Smart Contract Auditor](https://grnh.se/cf4858b2teu), [Smart Contract Auditor (Rust)](https://grnh.se/e2a692a2teu) & [BizDev](https://grnh.se/9fbf4582teu)

- Gnosis seek [DevRels](https://gnosis.jobs.personio.com/job/1296307?_pc=1517287&display=en), [Senior Web Devs (Wallet)](https://gnosis.jobs.personio.com/job/1239306?_pc=1517287&display=en) & [Backend Devs](https://gnosis.jobs.personio.com/job/1284509?_pc=1517287)

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

- [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db) wanted by EF

**Job listings: $600 for four issues** (75 character limit).  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [SBF found guilty](https://twitter.com/innercitypress/status/1720226132136468805) on all 7 counts, sentencing set for March 28

- [SafeMoon executives charged](https://www.justice.gov/usao-edny/pr/founders-and-executives-digital-asset-company-charged-multi-million-dollar) with securities fraud, wire fraud and money laundering

- [SEC crypto accounting bulletin](https://twitter.com/jchervinsky/status/1719408896006123820) should have been submitted to Congress

- [PayPal received SEC subpoena](https://www.coindesk.com/policy/2023/11/02/us-sec-subpoenas-paypal-about-usd-stablecoin-company-says) for PYUSD stablecoin

- [UK Treasury response](https://www.gov.uk/government/consultations/future-financial-services-regulatory-regime-for-cryptoassets) to crypto regulation consultation

**General**

- [DPRK target blockchain engineers](https://www.elastic.co/security-labs/elastic-catches-dprk-passing-out-kandykorn) with macOS malware

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-november-4-2023](https://weekinethereumnews.com/week-in-ethereum-news-november-4-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul), [**update 2**](https://blog.ethereum.org/2023/11/03/devconnect-ist-update-2)

- **Nov 15-21 –** [**DCxPrague**](https://dcxprague.org) **(Devconnect satellite event in Prague)**

- Nov 15-29 – [Gitcoin Grants 19](https://grants.gitcoin.co/#GG19-Rounds)

- Nov 16-19 – [Pragma](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Nov 18 – [Ethereum Costa Rica](https://www.meetup.com/ethereumcr/events/295894129/)

- **Nov 30 –** [**Road to Devcon grants**](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) **deadline (max $1k for local meetups)**

- Dec 4 – [ETHVenice](https://ethvenice.com/)

- Dec 6-7 – [Columbia CryptoEconomics workshop](http://columbiacryptoeconomics.org/) (New York)

- Dec 8-10 – ETHGlobal [ETHIndia](https://ethindia.co/) (Bangalore) 

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

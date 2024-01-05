---
title: "Week in Ethereum News <br> October 7, 2023"
date: "2023-10-06"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=US-aOBVsN6w&t=262s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-119/):
    - Devnet-9: testing [finding issues](https://twitter.com/M25Marek/status/1709972302907978192), MEV-Boost testing started (20% of the network)
    
    - Devnet-10: launch once no issues on devnet-9, short lived, to include KZG ceremony
    
    - Goerli testnet upgrade timing: still too early to set a date

- Dencun interop testing [call video](https://www.youtube.com/watch?v=o1ET9AuEK9c&t=63s)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 32.13%**](https://dune.com/hildobby/eth2-staking) **has slightly reduced but still far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~80% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm at 45%, any client bug over 33.3% could mean loss of finality

- [Geographic diversity needed for stakers & nodes](https://nodewatch.io/), particularly outside of US/Can/EU

**Layer 1**

- [Blutgang](https://github.com/rainshowerLabs/blutgang#readme): RPC load balancer & cache, in Rust

- Revm [v3.5.0](https://github.com/bluealloy/revm/releases/tag/v26): transitioned to Alloy types

- [Geth & Reth](https://twitter.com/gakonst/status/1709278476103283172) allow sync to historical hash

- Besu (execution layer client) [Bonsai Tries](https://consensys.io/blog/bonsai-tries-guide) storage explainer

- Verkle implementers [call notes](https://twitter.com/rudolf6_/status/1709672165573058673)

**For Stakers**

- Stakesaurus: [guide to home staking](https://stakesaurus.gitbook.io/eth-full-home-staking-setup-guide), aimed at novices

**Client releases**

- Execution layer:
    - Erigon [v2.51.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.51.0): fixes

**Layer 2**

- [OP Stack fault proof system](https://blog.oplabs.co/op-stack-fault-proof-alpha/) live on OP Goerli testnet, alpha

- [Metis](https://twitter.com/metisdao/status/1709965430591463763) (optimistic rollup) reverting to storing transaction data on mainnet

- [EIP4844 economics](https://arxiv.org/abs/2310.01155): model rollup costs for posting on blobs and blocks

**EIPs/Standards**

- EIPs
    - [EIP7530](https://github.com/ethereum/EIPs/pull/7809/files): EVM profiles for zk rollups

- ERCs (application layer):
    - [ERC7527](https://github.com/ethereum/EIPs/pull/7797/files): Token bound function oracle AMM contract
    
    - [ERC7528](https://github.com/ethereum/EIPs/pull/7808/files): ETH (native asset) address convention (0xe)
    
    - [ERC7529](https://github.com/ethereum/EIPs/pull/7815/files): Contract discovery and eTLD+1 association
    
    - [ERC7531](https://github.com/ethereum/EIPs/pull/7817/files): Staked ERC721 ownership recognition

* * *

### **Holding Lido publicly accountable:** [**interview with Ben Edgington**](https://podcasters.spotify.com/pod/show/web3builderspodcast/episodes/Holding-Lido-Publicly-Accountable-W-Ben-Edgington-e2a8b6f)

![Ben Edgington interview on web3 Builders podcast](https://weekinethereumnews.com/wp-content/uploads/2023/10/web3-Builders-Ben-Edgington-interview-1024x576.jpg)

Lido governance is not fit for purpose.  Don’t miss this [episode with Ben Edgington](https://podcasters.spotify.com/pod/show/web3builderspodcast/episodes/Holding-Lido-Publicly-Accountable-W-Ben-Edgington-e2a8b6f). (Watch on [YouTube](https://www.youtube.com/watch?v=WcGpHXTepcA))

Ben also talks about his Upgrading Ethereum book and Ethereum governance.

* * *

**Stuff for developers**

- OpenZeppelin Contracts [v5](https://blog.openzeppelin.com/introducing-openzeppelin-contracts-5.0):
    - Adds AccessManager, GovernorStorage, ERC2771Forwarder, ERC1967Utils, Nonces, MessageHashUtils and Time
    
    - Removals include: Address.isContract, Counters, ERC777, SafeMath, TokenTimelock, escrow contracts and all presets
    
    - Uses custom errors, explicit imports and Solidity compiler minimum of v0.8.20

- Hardhat [v2.18.0](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.18.0): adds support for scoped tasks  

- Foundry:
    - Forge-std [v1.7.0](https://github.com/foundry-rs/forge-std/releases/tag/v1.7.0)/[v1.7.1](https://github.com/foundry-rs/forge-std/releases/tag/v1.7.1): adds serializeJson cheat code, unixTime, marks parseJsonKeys as pure and renames exit\_code to exitCode
    
    - Vulcan [v0.4.0](https://twitter.com/nomoixyz/status/1708965012511801575): adds unwrap to obtain result value, set custom revert message with expect, isOk & isError for improved error handling and interaction with external HTTP servers
    
    - [Scope](https://github.com/g-01234/scope#readme) (VS Code extension): Remix-like & visual wrapper of some Foundry features, alpha

- Huff:
    - [Huff-test](https://github.com/horsefacts/huff-test#readme): macros for pure Huff test assertions
    
    - [Py-huff](https://github.com/Philogy/py-huff#readme): Huff compiler in Python
    
    - [Zyclone](https://github.com/AmadiMichael/Zyclone#readme): mixer in Huff (similar to Tornado Cash), gas optimized ~5x cheaper to deposit

- Vyper [v0.3.10](https://github.com/vyperlang/vyper/releases/tag/v0.3.10): adds codesize optimization mode, pragma directives, uses MCOPY in generated code and generates selector tables with O(1) performance

- CTFs:
    - Secureum RACE #22: [8 question Solidity quiz & answers](https://ventral.digital/posts/2023/10/3/race-22-of-the-secureum-bootcamp-epoch-infinity) by Tincho

**Ecosystem**

- Vitalik on [enshrining & de-enshrining features in the protocol](https://vitalik.eth.limo/general/2023/09/30/enshrinement.html): account abstraction, zk-EVMs, proposer-builder separation, private transaction pools, liquid staking and precompiles

- [Ethereum.org writers cohort 2](https://ethereumwriterscohort.carrd.co/) starts October 20

- Etherscan [event log advanced filter](https://twitter.com/etherscan/status/1709917362613633489)

**Enterprise**

- [UBS pilot tokenized Variable Capital Company (VCC) fund](https://www.ubs.com/global/en/media/display-page-ndp/en-20230927-first-blockchain-native.html?caasID=CAAS-ActivityStream) as part of Monetary Authority of Singapore’s Project Guardian

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 4.7 to 93.7 gwei, with 9.9 gwei average
    - Negative issuance currently at 21.2 gwei 
    
    - 8.6k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $1,611 - $1,736, currently $1,646

- [ETHBTC](https://ratiogang.com/): currently 0.059 (Flippening at ~0.16)

**Notable at app layer**

- Winding down: [Yield Protocol](https://yield-protocol.medium.com/winding-down-yield-protocol-0974b38066cc) and [Utopia product](https://utopia.beehiiv.com/p/winding-down)

- NFT no code creation:
    - [OpenSea Studio](https://opensea.io/blog/articles/introducing-opensea-studio) (10% mint fee)
    
    - [mint.fun create](https://twitter.com/mintdotfun/status/1709252670274630114) (0.0002 ETH mint fee)
    
    - [Zora](https://twitter.com/ourZORA/status/1709599808334499988) (gas free creation on Zora Network, 0.000111 ETH mint fee)

- [RAC’s Deadline NFT](https://twitter.com/RAC/status/1709629083578220615) live on Base, purchase from mainnet or Layer 2 \[Andrew minted\]

- Friend Tech [add/remove log in methods](https://twitter.com/friendtech/status/1709661643028976110) after SIM swap attacks

- Nature: [DAOs for scientific communities](https://www.nature.com/articles/s41587-023-02005-1) and alternative research funding

* * *

### Job Listings

- eBay Web3 team seeking [Lead Solidity Engineer](https://jobs.ebayinc.com/us/en/job/R0060412/Lead-Solidity-Engineer)

- Aave seek a [UX Engineer](https://jobs.eu.lever.co/aave/2ce6fc26-729f-4cbf-a8f0-070321663262?lever-origin=applied&lever-source%5B%5D=WeekinEthereumNews) and a [Staff Rust Engineer](https://jobs.eu.lever.co/aave/46c3f25c-2c74-4b31-903e-bfbdfbd63d66?lever-origin=applied&lever-source%5B%5D=WeekinEthereumNews)

- [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db) wanted by EF

- EF Privacy & Scaling Explorations team seek a [Technical Project Coordinator](https://jobs.lever.co/ethereumfoundation/c826b9a1-ede0-465e-9639-f34029304374)

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

**Job listings: $600 for four issues** (75 character limit).  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Coinbase](https://www.coinbase.com/blog/coinbase-obtains-major-payment-institution-licence-from-the-monetary) licenced by the Monetary Authority of Singapore

- VanEck to [donate 10% of EFUT ETF profits to Protocol Guild](https://twitter.com/vaneck_us/status/1707888396171977036)

- [ENS DAO reducing Lido exposure](https://discuss.ens.domains/t/metagov-working-group-weekly-meeting-11am-et-tuesday/15981/43#h-2-endowment-discussion-karpatkey-steakhouse-10) to maximum 20%

**General**

- [Roman Storm](https://twitter.com/rstormsf/status/1709347584375160990) available for work

- Vitalik reflects on [Zuzalu](https://www.palladiummag.com/2023/10/06/why-i-built-zuzalu/) (popup mini city)

- Guide to [secure Discord servers](https://github.com/0xngmi/discord-server-guidelines/blob/master/README.md)

- [zk-Bench](https://eprint.iacr.org/2023/1503): benchmarking framework for SNARKs

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-october-7-2023](https://weekinethereumnews.com/week-in-ethereum-news-october-7-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Oct 13-15 – [Ethereum Kuala Lumpur](https://hack.ethkl.org/) conference & hackathon

- Oct 21 – [Ethereum México](https://twitter.com/ethereum_mexico/status/1684649652639924224)

- Oct 22-24 – [ETH Hong Kong](https://www.ethhongkong.co/)

- Oct 27-29 – [ETH London](https://www.encode.club/eth-london) hackathon

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Oct 28-30 – [Paradigm CTF](https://ctf.paradigm.xyz/)

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) deadline (max $1k for local meetups)

- Nov 3-5 – [ETHBrno](https://ethbrno.cz)

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 16-19 – [Pragma](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- **Nov 18 –** [**Ethereum Costa Rica**](https://www.meetup.com/ethereumcr/events/295894129/)

- Dec 4-5 – [ETHVenice](https://ethvenice.com/)

- Dec 8-10 – ETHGlobal [ETHIndia](https://ethindia.co/) (Bangalore) 

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

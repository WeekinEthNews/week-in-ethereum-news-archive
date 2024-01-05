---
title: "Week in Ethereum News <br> September 30, 2023"
date: "2023-09-29"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call](https://www.youtube.com/watch?v=CPt3f3ughFM&t=86s) video. [Recap](https://mirror.xyz/abcoathup.eth/SCgGDQ26piZSyl8K3V07mxQGdUfYt10ovbq4mjmfUPo) by Tim Beiko.  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1707464366629781768) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-171/):
    - Devnet-9 using EIP4788 mainnet address & manual deployment and plan to test MEV-Boost; KZG ceremony trusted setup expected next week
    
    - EIP7514 (max churn limit) to be tested on short lived devnet-10 with high number of validators
    
    - EIP4788 (beacon root) issues fixed from 3 audits: 0 timestamp & ring buffer size
    
    - Discussion on proposed [EIP7503](https://docs.google.com/presentation/d/1omnj-y2L59wERsOBQRKjoIKHm5VQ1A6Sdmc2_Oa75IM/edit?pli=1#slide=id.p) (onchain privacy via reminting burnt ETH)

- [Devnet-9](https://dencun-devnet-9.ethpandaops.io/) launched

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 32.23%**](https://twitter.com/lidodominance/status/1707757122291646495) **far too close to risky** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~80% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm at 45%, any client bug over 33.3% could mean loss of finality

- Need more [geographic diversity for both stakers & nodes](https://nodewatch.io/), particularly outside of US/Can/EU

**Layer 1**

- [91% of blocks](https://twitter.com/uriklarman/status/1706716871024615723) are via MEV-Boost relays controlled by just four entities

- [Censorship dashboard](https://twitter.com/nero_eth/status/1706594750155931953): OFAC compliance of validators, relays & builders

- [Mempool dumpster](https://twitter.com/metachris/status/1706274142071488649) (transactions in Parquet & CSV): adds inclusion status & inclusion delay

**Client releases for Holešky testnet**

- Consensus layer:
    - Lighthouse [v4.5.0](https://github.com/sigp/lighthouse/releases/tag/v4.5.0): experimental QUIC support
    
    - Lodestar [v1.11.3](https://github.com/ChainSafe/lodestar/releases/tag/v1.11.3)
    
    - Nimbus [v23.9.1](https://github.com/status-im/nimbus-eth2/releases/tag/v23.9.1)
    
    - Prysm [v4.1.0-alpha.1](https://github.com/prysmaticlabs/prysm/releases/tag/v4.1.0-alpha.1)
    
    - Teku [v23.9.1](https://github.com/Consensys/teku/releases/tag/23.9.1): Holešky testnet requires GLIBC v2.34 on Linux

- Execution layer:
    - Besu [v23.7.3](https://github.com/hyperledger/besu/releases/tag/23.7.3)
    
    - Erigon [v2.49.3](https://github.com/ledgerwatch/erigon/releases/tag/v2.49.3): Holešky; [v2.50.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.50.0): implements Cancun EIPs
    
    - Geth [v1.13.2](https://github.com/ethereum/go-ethereum/releases/tag/v1.13.2): fixes for path db storage schema corner cases
    
    - Nethermind [v1.21.0](https://github.com/NethermindEth/nethermind/releases/tag/1.21.0): executable renaming, throttling RPC calls, Trie recovery & sync time reduction
    
    - Reth [v0.1.0-alpha.9](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.9): implements Cancun EIPs, revm state handling API reworked and pruning improvements; [v0.1.0-alpha.10](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.10): Holešky

**Research**

- Preparing for danksharding: [data visualization on the propagation time of big blocks](https://blog.codex.storage/big-blocks-on-mainnet/) on mainnet

- [Relay-constructed inclusion list](https://ethresear.ch/t/resistance-is-not-futile-cr-in-mev-boost/16762): proposal for censorship resistance in MEV-Boost

- Framework for [design of optimal dynamic fees](https://arxiv.org/abs/2309.12735) for multiple resources

**Layer 2**

- OP Stack: [social decentralization & Fault Proof VM](https://blog.oplabs.co/fault-proof-vm/) and [dispute games](https://blog.oplabs.co/dispute-games/)

- [Roll-op](https://github.com/0xFableOrg/roll-op/#readme): script to configure & deploy OP Stack network

**EIPs/Standards**

- EIPs
    - [EIP7525](https://github.com/ethereum/EIPs/pull/7776/files): Expire state of the inactive accounts

- ERCs (application layer):
    - [ERC7524](https://github.com/ethereum/EIPs/pull/7775/files): PLUME signature in wallets
    
    - [ERC7526](https://github.com/ethereum/EIPs/pull/7781/files): Onchain NFT royalty enforcement

**Stuff for developers**

- [Holešky testnet](https://github.com/eth-clients/holesky#readme) launched for staking, infrastructure & protocol testing
    - Explorers: [Etherscan](https://holesky.etherscan.io/), [beaconcha.in](https://holesky.beaconcha.in/) & [Otterscan](https://holesky.otterscan.io/)
    
    - 1000 holETH distributed to contract deployers (mainnet & Goerli testnet)
    
    - Faucets: [pk910 PoW faucet](https://holesky-faucet.pk910.de/) & Etherscan’s [Blockscan chat](https://twitter.com/etherscan/status/1707712285115056469)
    
    - Replacement for deprecated [Goerli](https://github.com/eth-clients/goerli#readme)
    
    - Use [Sepolia testnet](https://github.com/eth-clients/sepolia#readme) for app layer testing

- Remix [v0.36.0](https://medium.com/remix-ide/remix-release-v0-36-0-36bae12abb1f): uses ChatGPT to explain a function, generate documentation & explain compiler errors, adds more quick fixes and support for Ephemery testnet

- Hardhat [v2.17.4](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.17.4): supports debug\_traceCall

- [Branching Tree Technique examples](https://github.com/PaulRBerg/btt-examples#readme): specification framework for writing structured Solidity tests

- [Solmate](https://github.com/transmissions11/solmate/#readme) (contract library) adds ERC6909 (minimal multi-token interface) implementation

- SSTORE gas:
    - [OpenZeppelin ReentrancyGuard avoids resetting to zero](https://forum.openzeppelin.com/t/understanding-the-refund-logic-in-reentrancyguard/37948/2) to maximize gas refund
    
    - [EVM uses SSTORE current vs final value](https://medium.com/eulerfinance/have-you-heard-about-this-sstore-quirk-anon-6a1ae870e57c) and not intermediate values for reduced gas cost

- [Comparison of borrowing protocol architectures](https://hackernoon.com/borrowing-on-ethereum-comparing-architecture-evolution-of-makerdao-yield-aave-compound-and-euler): MakerDAO, Compound, Aave, Euler & Yield

- Huffathon challenges: [1](https://github.com/devtooligan/huffathon-2023-challenge-0-1#readme), [2](https://github.com/devtooligan/huffathon-2023-challenge-0-2#readme), [3](https://github.com/PraneshASP/huffathon-challenge-2#readme) & [4](https://github.com/RareSkills/rareskills-huffathon-challenge#readme)

- wagmi [v2 alpha](https://github.com/wagmi-dev/wagmi/discussions/3068): TanStack Query support, connect multiple connectors, switch chains while disconnected and EIP6963 support

- ERC4337 (account abstraction):
    - [Permissionless.js](https://github.com/pimlicolabs/permissionless.js#readme): TypeScript library to interact with bundlers & paymasters, built on viem
    
    - Alchemy’s [Rundler](https://github.com/alchemyplatform/rundler#readme): ERC4337 bundler in Rust

- [Solidity Next.js starter v2](https://github.com/tomhirst/solidity-nextjs-starter#readme): uses Hardhat, viem, wagmi, Tailwind CSS & RainbowKit

- [Ether binder](https://github.com/m8b-dev/ether-binder#readme) beta, PHP utilities to interact with Ethereum, uses PHP 8.2

- Curta CTF [Philosopher's Stone writeup](https://twitter.com/eth_call/status/1706029458275119205)

- [Guide to using Cryo](https://mteam88.github.io/posts/analyzing-ethereum-with-cryo/) & Polars for data analysis

- Banteg: [create heatmap](https://banteg.xyz/posts/heatmap/) of ERC20 transfers

- RareSkills: [Circom tutorial](https://www.rareskills.io/post/circom-tutorial)

**Security**

- [SEAL 911 members saved $200k](https://twitter.com/frankresearcher/status/1706740009997369775) from Dice9win mid exploit

- GMX (DEX on Arbitrum) [price skew vulnerability disclosed](https://www.collider.vc/post/gmx-granted-million-dollar-bug-bounty-to-collider-the-bug-aftermath), fixed with $1M bounty paid

**Ecosystem**

- Dankrad: [Ethereum values need to be protected by the community](https://twitter.com/dankrad/status/1707014810565566962), they are not automatically guaranteed by economic incentives

- EF [data collection grants](https://esp.ethereum.foundation/data-collection-grants), applications close October 23, wish list includes projects for [XATU](https://twitter.com/samcmau/status/1707604513086189869) (network monitoring), testnets and data collection

- [ERC4337 (account abstraction) adoption analysis](https://sixdegree.xyz/research/Half-Year-Data-Report-of-ERC4337-by-Sixdegree.pdf): 687k wallets, 2M UserOps, majority of wallets used 5 times or less

- ETHGlobal [New York hackathon finalists](https://twitter.com/ETHGlobal/status/1706049363464569232)

**Enterprise**

- Bank of International Settlements [Project Mariana](https://www.bis.org/publ/othp75.pdf): proof of concept for cross-border exchange of wholesale CBDCs using AMMs on Sepolia testnet

- [Buenos Aires digital identity](https://zksync.mirror.xyz/w4_Dyhbx1X2BEGpYNCn8rEAS_2uC1hV0qPQl_m5AChk): QuarkID wallet can be used to claim birth & marriage certificates, uses zkSync Era

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 5.5 to 74.1 gwei, with 10.7 gwei average
    - Negative issuance currently at 20.9 gwei 
    
    - 7.9k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $1,569 - $1,684, currently $1668

- [ETHBTC](https://ratiogang.com/): currently 0.062 (Flippening at ~0.16)

**Notable at app layer**

- Arbitrum [Odyssey](https://arbitrumfoundation.medium.com/arbitrum-odyssey-reignited-a98f627d42ef) relaunched, 7 week campaign for users to try apps & collect badges

- [Pudgy Toys](https://www.prnewswire.com/news-releases/pudgy-penguins-debuts-toyline-in-major-retail-stores-across-us-301939099.html): physical Pudgy Penguin plushies, sold in Walmart, licensing royalties shared with NFT holders, purchasers can claim a Forever Pudgy on zkSync

- Nouns DAO [burn proposal](https://w.mirror.xyz/AmHOzH-FQZVO3IhGXHSvCRxRSf2MO6VCZdmMwNEIyKE): incentivize spending the treasury otherwise excess ETH can be burnt

- [Paris Hilton promoting MareBear NFTs](https://twitter.com/ParisHilton/status/1707410178969137532): Tamagotchis pets

* * *

### Job Listings

- Aave seek a [UX Engineer](https://jobs.eu.lever.co/aave/2ce6fc26-729f-4cbf-a8f0-070321663262?lever-origin=applied&lever-source%5B%5D=WeekinEthereumNews) and a [Staff Rust Engineer](https://jobs.eu.lever.co/aave/46c3f25c-2c74-4b31-903e-bfbdfbd63d66?lever-origin=applied&lever-source%5B%5D=WeekinEthereumNews)

- [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db) wanted by EF

- EF Privacy & Scaling Explorations team seek a [Technical Project Coordinator](https://jobs.lever.co/ethereumfoundation/c826b9a1-ede0-465e-9639-f34029304374)

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

**Job listings: $600 for four issues** (75 character limit).  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- VanEck announced upcoming [ETH futures ETF](https://www.vaneck.com/us/en/press-releases/vaneck-prepares-to-launch-ethereum-futures-etf-efut.pdf) (EFUT)

- [Coinbase](https://www.coinbase.com/blog/coinbase-receives-regulatory-approval-to-enable-retail-perpetual-futures?__cf_chl_f_tk=NQFPKqxhWtw.O7q1bDHMnWlVb7p7j5_Tu2v3l0Qp2Hk-1695944027-0-gaNycGzNDHs) approved by Bermuda Monetary Authority to offer perpetual futures trading, non-US

- New York & Boston Feds: [stablecoin flight to safety dynamics](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4580392) resemble money market funds

- [Chase UK](https://www.coindesk.com/policy/2023/09/26/chase-uk-to-block-crypto-payments-citing-fraud-scams/) will decline crypto related payments

**General**

- Exchange hacks: [$200M for Mixin Network](https://rekt.news/mixin-rekt/) and [$8M for HTX (formerly Huobi)](https://twitter.com/justinsuntron/status/1706311251024822748)

- [Sigmabus](https://eprint.iacr.org/2023/1406): efficient computation of elliptic curve group operations in generic SNARK circuits

- [Naysayer proofs](https://eprint.iacr.org/2023/1472): accept proofs optimistically and only check when necessary

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-30-2023](https://weekinethereumnews.com/week-in-ethereum-news-september-30-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 13-15 – [Ethereum Kuala Lumpur](https://hack.ethkl.org/) conference & hackathon

- Oct 21 – [Ethereum México](https://twitter.com/ethereum_mexico/status/1684649652639924224)

- Oct 22-24 – [ETH Hong Kong](https://www.ethhongkong.co/)

- Oct 27-29 – [ETH London](https://www.encode.club/eth-london) hackathon

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Oct 27-29 – [ETH Vietnam](https://www.eth-vietnam.com/)

- Oct 28-30 – [Paradigm CTF](https://ctf.paradigm.xyz/)

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) deadline (max $1k for local meetups)

- Nov 3-5 – [ETHBrno](https://ethbrno.cz)

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 16-19 – [Pragma](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Dec 4-5 – [ETHVenice](https://ethvenice.com/)

- Dec 8-10 – ETHGlobal [ETHIndia](https://ethindia.co/) (Bangalore) 

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

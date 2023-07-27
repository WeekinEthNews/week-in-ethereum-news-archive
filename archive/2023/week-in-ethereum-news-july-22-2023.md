---
title: "Week in Ethereum News <br> July 22, 2023"
date: "2023-07-22"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=pTWm4EyStYg&t=259s). Summary by [Tim Beiko](https://twitter.com/abcoathup/status/1682151447033688065).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1682078353736744960) and [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-execution-call-166-writeup/):
    - Dencun testing continues with devnet 7 and a [Sepolia shadow fork](https://twitter.com/parithosh_j/status/1682386409494138886)
    
    - Client teams implementing Dencun EIPs ready for [devnet 8](https://notes.ethereum.org/@ethpandaops/dencun-devnet-8)
    
    - EIP6780 (selfdestruct only in same tx) edge cases clarification, burn used by some L2s 
    
    - Discussions on adding parent beacon block roots to execution payload, adding getBlockReceipts & removing mining from Execution API and standardizing JWT location
    
    - EIP/ERC repo split ([EIP7329](https://eips.ethereum.org/EIPS/eip-7329)): core devs in favor, Greg Colvin (EIP editor) still opposed

- [KZG Ceremony](https://ceremony.ethereum.org/) 122k contributions, lobby closes July 23 (tomorrow!)

**Prague + Electra upgrade**

- [EIP7251 FAQ](https://notes.ethereum.org/@mikeneuder/eip-7251-faq): would allow more than 32 ETH to be staked

- [Suggest a name](https://ethereum-magicians.org/t/name-needed-for-combined-el-cl-prague-electra-upgrade/15122) for the Prague + Electra upgrade

**Layer 1**

- Ben Edgington: [Upgrading Ethereum book](https://eth2book.info/capella/part2/consensus/) new sections on LMD GHOST & Casper FFG

**Client releases**

- Consensus layer:
    - Lodestar [v1.9.2](https://github.com/ChainSafe/lodestar/releases/tag/v1.9.2): hotfix for gossip blocks with unknown block parent errors and changed block production wait cutoff
    
    - Nimbus [v23.7.0](https://github.com/status-im/nimbus-eth2/releases/tag/v23.7.0): validator client optimisations and improves validator performance
    
    - Teku [v23.6.2](https://github.com/Consensys/teku/releases/tag/23.6.2): minor bug fixes and dependencies updates

- Execution layer:
    - Nethermind [v1.20.1](https://github.com/NethermindEth/nethermind/releases/tag/1.20.1): fix for v1.20.0 which caused Prysm error
    
    - Reth [v0.1.0-alpha.4](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.4): removed downloader heuristic preventing syncing, jemallocator default on UNIX and added transaction pool maintenance metrics

**For Stakers**

- [Staking directory](https://www.staking.directory/): directory of staking providers 

**Research**

- [Data availability sampling (DAS) eprint](https://eprint.iacr.org/2023/1079): prove existing constructions secure, propose new constructions with benchmark & trade-offs

- [Threshold encrypted transaction pools](https://arxiv.org/abs/2307.10878): tradeoffs of using for MEV mitigation

**Layer 2**

- [Celo propose rollup migration](https://forum.celo.org/t/clabs-proposal-for-celo-to-transition-to-an-ethereum-l2/6109), initially OP Stack, decentralized sequencer using Celo’s validator set, offchain data availability via Eigen Layer and 1-block finality

- [zkSync Era](https://zksync.mirror.xyz/HJ2Pj45EJkRdt5Pau-ZXwkV2ctPx8qFL19STM5jdYhc) shadow testing Boojum (STARK-based proof system)

- [Mantle](https://www.mantle.xyz/blog/announcements/mantle-network-mainnet-alpha) (optimistic rollup) alpha is live

- Consensys [Linea](https://twitter.com/LineaBuild/status/1681283676791873536) (zk rollup) alpha is live

- L2BEAT: [upgrade process of L2s](https://drive.google.com/file/d/182ycEW8C2wk5tGd3X1tG8oQfUy9WmSJk/view) \[PDF\]

**EIPs/Standards**

- ERCs (application layer):
    - [ERC7336](https://github.com/ethereum/EIPs/pull/7336/files): Interactive across multiple registries
    
    - [ERC7361](https://github.com/ethereum/EIPs/pull/7361/files): Metadata hash with decentralized validation (ERC721 extension)

* * *

### **This newsletter is made possible thanks to** [**Mimic v3**](https://medium.com/mimicfi/introducing-mimic-v3-diving-into-new-depths-of-efficiency-4e564ad2714a)

![](https://weekinethereumnews.com/wp-content/uploads/2023/07/Mimic-1024x388.png)

[Mimic v3](https://medium.com/mimicfi/introducing-mimic-v3-diving-into-new-depths-of-efficiency-4e564ad2714a) is a platform that helps you model and automate operations in DeFi.

Do you need:

- Recurring payments

- To collect fees across various chains?

- To automate your portfolio rebalancing?

Mimic gives you a customizable workflow with modular cross-chain connectors.  [Request a demo](https://www.mimic.fi/#contact).

Trusted by top-tier projects such as Trust Wallet, Balancer, ParaSwap, and Decentraland.  Backed by Starbloom Ventures.

* * *

**Stuff for developers**

- Solidity [v0.8.21](https://soliditylang.org/blog/2023/07/19/solidity-0.8.21-release-announcement/):
    - Language features: access events from other contracts & immutable variable initialization restrictions relaxed
    
    - Addresses “stack too deep” errors for unoptimized code from IR-based code generation
    
    - Bug fixes: legacy code generation [always generate code for expression in <expression>.selector](https://soliditylang.org/blog/2023/07/19/missing-side-effects-on-selector-access-bug/) and Yul optimizer [FullInliner evaluation order](https://soliditylang.org/blog/2023/07/19/full-inliner-non-expression-split-argument-evaluation-order-bug/)
    
    - website [makeover](https://twitter.com/solidity_lang/status/1681658620935647232)

- Create a [stake & reward contract](https://hackernoon.com/how-to-implement-a-stake-and-reward-contract-in-solidity)

- [Reproduce a simple MEV attack](https://medium.com/immunefi/how-to-reproduce-a-simple-mev-attack-b38151616cb4) in Solidity using Hardhat or Foundry

- Guide to [fuzzing onchain contracts with Echidna](https://blog.trailofbits.com/2023/07/21/fuzzing-on-chain-contracts-with-echidna/)

- Sothis [v0.4.0](https://github.com/rainshowerLabs/sothis/releases/tag/0.4.0): replay historical state on a local Anvil/Hardhat node

- The Graph: [Substreams-powered subgraphs](https://thegraph.com/blog/substreams-powered-subgraphs/)

- Secureum [A-MAZE-X CTF solutions](https://ventral.digital/posts/2023/7/16/secureum-a-maze-x-ctf-2023-at-defi-security-summit)

- Celer [Brevis](https://blog.celer.network/2023/07/18/brevis-alpha-now-live-introducing-zk-co-processing-and-data-attestation-sdks-for-developers/): zk co-processing & data attestation SDKs, alpha

**Security**

- Conic Finance [$3 million exploit](https://twitter.com/ConicFinance/status/1682385596700844032) via read-only reentrancy

- Immunefi: [top ten common vulnerabilities](https://medium.com/immunefi/the-top-10-most-common-vulnerabilities-in-web3-bf7a921d489f)

**Ecosystem**

- EthCC:
    - Videos by stage: [main](https://www.youtube.com/playlist?list=PLM-Xjhvin-uURP4lmYyP0iys2mxq-rCKU), [Eiffel](https://www.youtube.com/playlist?list=PLm6V2qdPAeaUBG-qBewmpopLdgVtpqaXM), [Versailles](https://www.youtube.com/playlist?list=PLUt355rCCNrTliK_38XZpLzt1JGrKr2Dq), [Bastille](https://www.youtube.com/playlist?list=PLSJ8gU1sECuzy2pLKFvyPjFn6jaIx_p1C), [Notre Dame](https://www.youtube.com/playlist?list=PLhM7rBgpVV-KN8mM17IRSFIGsL0EaGA_m), [Louvre](https://www.youtube.com/playlist?list=PL-owlDp9BBasiGOoq5sK3gg0zKS_2WXLP) & [Saint Victor](https://www.youtube.com/playlist?list=PLqL60kqgLPBAM-gy8Dop9tTREOuq1q2QV)
    
    - [EthCC 2024](https://twitter.com/EthCC/status/1682040349857050627) will be in Brussels

- Etherscan [advanced filter updates](https://twitter.com/etherscan/status/1682351432543113218)

**Notable at app layer**

- [Aave GHO](https://aave.mirror.xyz/t7qcU668gSp9teT_SBhJb9_AVcbv8kpzvd0IpP39lBw) (overcollateralized stablecoin) live on mainnet, Aave v3 supplied assets used as collateral

- [UniswapX](https://blog.uniswap.org/uniswapx-protocol) (aggregator): gas-free swaps with MEV protection & no cost for failed transactions, beta

- [Ajna](https://www.ajna.finance/) (lending) live on mainnet, no governance or external price feeds

- OpenSea [Deals](https://twitter.com/opensea/status/1682077991029932032): create offers to swap NFTs for NFTs & WETH

- [Mint.fun](https://twitter.com/mintdotfun/status/1681696385555648514) (NFT minting) adds support for NFTs on Optimism & Zora

* * *

### Job Listings

- EF Privacy & Scaling Explorations team seek [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Financial Stability Board](https://www.fsb.org/2023/07/fsb-finalises-global-regulatory-framework-for-crypto-asset-activities) (FSB) recommended framework for crypto assets

- [UK Financial Conduct Association](https://www.fca.org.uk/publication/guidance-consultation/gc23-2.pdf) (FCA) guidance warns memes can breach promotion rules

- [France issues crypto license to Societe Generale Forge](https://www.coindesk.com/policy/2023/07/19/societe-generale-becomes-first-company-to-win-french-crypto-license) to buy/sell, exchange & custody assets

- [Nasdaq](https://www.coindesk.com/business/2023/07/19/nasdaq-halts-plan-for-crypto-custody-service-due-to-us-regulatory-conditions/) halts plans for crypto custody service due to US regulatory environment

* * *

### Evan’s new podcast: web3 Builders

- Subscribe to [web3 Builders](https://podcasters.spotify.com/pod/show/web3builderspodcast) podcast. First episode should drop this week, there may be advantages to subscribing. 👀

* * *

**General**

- [Gnosis Pay](https://twitter.com/gnosispay/status/1680874992509272065): payment network on Gnosis chain L2 with linked Visa Debit card

- [GitHub social engineering attacks](https://github.blog/2023-07-18-security-alert-social-engineering-campaign-targets-technology-industry-employees/), using repo invites & malicious npm dependencies

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-22-2023](https://weekinethereumnews.com/week-in-ethereum-news-july-22-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jul 23 – [KZG Ceremony](https://ceremony.ethereum.org/) closes

- **Jul 23 –** [**Devconnect scholars**](https://blog.ethereum.org/2023/06/26/devconnect-instanbul-scholars) **application deadline**

- **Aug 4-18 –** [**ETHGlobal Superhack**](https://ethglobal.com/events/superhack) **virtual**

- Aug 11-13 – [ETHMunich](https://ethmunich.de/) hackathon

- Aug 15-16 – [ETHToronto](https://www.ethtoronto.ca/) & [ETHWomen](https://www.ethwomen.com/)

- **Aug 15-29 –** [**Gitcoin Grants 18**](https://twitter.com/gitcoin/status/1681747409435787264)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org/) (Buenos Aires)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 31 - Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 7-9 – [ETHAccra](https://www.ethaccra.xyz/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 15-17 – [ETHChicago](https://www.ethchicago.xyz/) conference & hackathon

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 6-27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 13-15 – [Ethereum Kuala Lumpur](https://hack.ethkl.org/) conference & hackathon

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) application deadline

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://twitter.com/ethbrno/status/1652198745902137344)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 17-19 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

---
title: "Week in Ethereum News <br> December 24, 2022"
date: "2022-12-24"
---

## **Eth News and Links**

**Shapella (Shanghai + Capella) upgrade**

- Shapella [withdrawal-devnet-1](https://withdrawalsdevnet1.ethpandaops.io/) is [finalizing](https://twitter.com/evan_van_ness/status/1606390617088659472)

- The Merge had pandas, Capella has owls: [Lodestar](https://github.com/ChainSafe/lodestar/pull/4815) & [Nimbus](https://github.com/status-im/nimbus-eth2/pull/4442) display owls at Capella transition for [withdr**OWL**s](https://twitter.com/Renethftw/status/1595451793349255170)

**Cancun + D-starname upgrade**

- EIP4844 (proto-danksharding) [devnet 3](https://hackmd.io/@inphi/Hk_cLBJFo) user guide

**Layer 1**

- [TX-Fuzz](https://github.com/MariusVanDerWijden/tx-fuzz#readme) v1.0.0: create random transactions, used to break withdrawal-devnet-0

- Afri: [configure a network to use PoS from genesis](https://dev.to/q9/how-to-merge-an-ethereum-network-right-from-the-genesis-block-3454), with Geth + Lodestar

- Lido: [Distributed Validator Technology (DVT) pilot with Obol Network](https://blog.lido.fi/dvt-pilot-with-obol-network/) on testnet

- Evolution of [Gasper (Ethereum Proof of Stake protocol)](https://github.com/ethereum/pos-evolution/blob/master/pos-evolution.md)

**Research**

- Flashbots: [running Geth inside SGX](https://writings.flashbots.net/geth-inside-sgx/)

**Client releases**

- Consensus Layer:
    - Nimbus [v22.12.0](https://github.com/status-im/nimbus-eth2/releases/tag/v22.12.0): improves doppelganger detection in the Nimbus validator client

**Layer 2**

- Polygon zkEVM [testnet updated](https://polygon.technology/blog/final-approach-last-testnet-for-an-upgraded-polygon-zkevm) with recursion, faster proof time & batch aggregation  

- Intmax (zk-rollup) [testnet](https://medium.com/@intmax/the-missing-piece-for-the-ethereum-endgame-intmax-testnet-v1-launch-a2f40d406b42), command line only

- Justin Drake: [SGX as pragmatic hedge against zk-rollup SNARK vulnerabilities](https://ethresear.ch/t/2fa-zk-rollups-using-sgx/14462)

- Arbitrum:
    - [Solutions to delay attacks on rollups](https://offchain.medium.com/solutions-to-delay-attacks-on-rollups-434f9d05a07a)
    
    - [Batch posting strategy on mainnet](https://arxiv.org/abs/2212.10337)

- Taiko: [rollup decentralization](https://mirror.xyz/labs.taiko.eth/sxR3iKyD-GvTuyI9moCg4_ggDI4E4CqnvhdwRq5yL0A), definitions & high-level ideas

**EIPs/Standards**

- [EIP6170](https://github.com/ethereum/EIPs/pull/6172/files): Cross chain messaging interface

- [EIP6188](https://github.com/ethereum/EIPs/pull/6188/files): Nonce cap

- [EIP6189](https://github.com/ethereum/EIPs/pull/6189/files): Alias contracts

- [EIP6190](https://github.com/ethereum/EIPs/pull/6190/files): Functional SELFDESTRUCT

- [EIP6206](https://eips.ethereum.org/EIPS/eip-6206): EOF - JUMPF instruction

* * *

### **This newsletter is made possible thanks to** [**Mimic**](https://mimic.fi/)**!**

![mimic](https://weekinethereumnews.com/wp-content/uploads/2022/10/mimic-banner-1024x427.png)

Does your DAO want to **delegate treasury management but keep custody?** Or **trustlessly automate your yield?**

Check out our [Smart Vaults](https://medium.com/mimicfi/introducing-smart-vaults-3438bacc843d) to automate DeFi operations in a secure, trustless, and non-custodial way.

**For DeFi projects**: you can also automate collecting your fees across chains and swapping/distributing them.

Previously Mimic’s co-founders helped build POAP, Balancer, and OpenZeppelin, among others.  _Backed by Starbloom Ventures._

* * *

**Stuff for developers**

- [SELFDESTRUCT is deprecated](https://eips.ethereum.org/EIPS/eip-6049), avoid using it as functionality will change

- [Solarray](https://github.com/evmcheb/solarray#readme): helper to initialize dynamic arrays in one line, useful for Foundry tests

- [Quickpoc](https://github.com/zobront/quickpoc#readme): create a sandbox for a mainnet verified contract including dependencies using Foundry

- [Bash Foundry helpers](https://gist.github.com/jameswenzel/86d2e1a524ffc66eb424770f74165a49): convenience methods & aliases

- [Exploring upgradeable contracts](https://runtimeverification.com/blog/using-foundry-to-explore-upgradeable-contracts-part-1) by implementing a basic proxy

- Overview of [Solidity storage packing](https://twitter.com/ylv_io/status/1605642285198106624)

- [Nexth](https://github.com/wslyvh/nexth#readme): Next.js starter kit with Chakra UI, TypeScript, ConnectKit & wagmi

- Guide to [understanding transaction call data](https://degatchi.com/articles/reading-raw-evm-calldata)

- TrueBlocks [docker](https://github.com/TrueBlocks/trueblocks-docker#readme): local indexing & data access, beta

- [Sourcify-snap](https://github.com/therealharpaljadeja/sourcify-snap#readme): MetaMask snap displays function NatSpec from Sourcify

- Fleek [Non Fungible Apps](https://github.com/fleekxyz/non-fungible-apps#readme): NFT with on-chain metadata about an app, proof of concept

- Go-waku [v0.3.0](https://github.com/waku-org/go-waku/releases/tag/v0.3.0): adds new protocols peer exchange & device pairing

- Wallet devs [call notes](https://twitter.com/_samwilsn_/status/1605976265084780547)

**Security**

- High level process for [understanding a code base](https://twitter.com/zachobront/status/1606132664422891520)

**Ecosystem**

- [ETHGlobal 2023 events](https://ethglobal.medium.com/announcing-the-2023-ethglobal-season-3cc1960de7b4): Tokyo, Istanbul, Toronto, Paris, New York & Devcon plus virtual events Scaling Ethereum & ETHOnline

- Columbia [CryptoEconomics workshop videos](https://www.youtube.com/playlist?list=PLpktWkixc1gUqkyc1-iE6TT0RWQTBJELe)

- [Ethereum.org non-English pageviews doubled](https://twitter.com/samonchain/status/1605966933022494728) from 14% to 28% in past year

- Nethermind: [Systematization of Knowledge for decentralized identities & verifiable credentials](https://medium.com/nethermind-eth/systematization-of-knowledge-for-decentralized-identities-verifiable-credentials-phase-1-of-e972cf5ec153)

**Enterprise**

- [Visa experiments with automated payments](https://usa.visa.com/solutions/crypto/auto-payments-for-self-custodial-wallets.html) using account abstraction on StarkNet

**Application layer**

- Synthetix [Perps v2](https://blog.synthetix.io/synthetix-perps-v2-is-now-live/) live on Optimism; trading on Kwenta & [Decentrex](https://twitter.com/DecentrexHQ/status/1606066286185680896)

- [Seatbelt](https://www.scopelift.co/blog/seatbelt-for-governance) (simulate on-chain DAO proposals) adds support for OpenZeppelin Governors

- [Zodiac governor module](https://twitter.com/GnosisGuild/status/1603794129741352960): enable DAO on-chain voting for a Safe multi-sig

- Guide to [reviewing a governance action](https://hackernoon.com/how-to-review-a-governance-action)

- [SushiSwap voted to divert 100% of xSushi fees](https://thedefiant.io/sushi-proposal-debate-revenue-hot-water) to treasury

- [3th.ws](https://twitter.com/xGozzy/status/1604725634999398402): uncensored ENS IPFS resolver with dynamic Tor onion services

- Giveth [holiday giving DeFi4Good campaign](https://twitter.com/Givethio/status/1605594294974152706)

* * *

### Job Listings

- Join a16z-backed Story Protocol as a founding [smart contract developer](https://jobs.lever.co/storyprotocol/e08066d4-8d73-46ab-975c-dd5a284e1a83).

- Alchemy seeking [Product Managers](https://grnh.se/43e96eeb5us) to build the future of web3.

- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [SBF released on bail](https://www.reuters.com/legal/ftx-founder-bankman-fried-make-us-court-appearance-after-extradition-2022-12-22/) after being extradited to US; Tornado Cash developer Alex Pertsev remains jailed in the Netherlands for a 5th month

- [Caroline Ellison (former Alameda CEO) & Gary Wang (FTX co-founder) pled guilty](https://www.justice.gov/usao-sdny/pr/united-states-attorney-announces-extradition-ftx-founder-samuel-bankman-fried-united) to fraud and are cooperating with authorities

- Brian Armstrong: [what regulatory clarity looks like](https://www.coinbase.com/blog/regulating-crypto-how-we-move-forward-as-an-industry-from-here)

- [Swiss judge mandates ConsenSys shareholder vote](https://www.politico.com/news/2022/12/19/legal-fight-web3-ownership-crypto-00074629) on transfer of MetaMask, Infura & Truffle to VC-backed entity

- New York Fed: [DeFi better protects investors](https://libertystreeteconomics.newyorkfed.org/2022/12/can-decentralized-finance-provide-more-protection-for-crypto-investors/) but needs to mitigate contract & oracle risk

- $30 billion in [NFT wash trading](https://community.dune.com/blog/nft-wash-trading-on-ethereum), 44% of volume traded

**General**

- [LastPass attacker copied customer password vaults](https://blog.lastpass.com/2022/12/notice-of-recent-security-incident/), users with a weak master password should change everything

- [TikTok confirms its employees accessed data of US users](https://archive.vn/tX9ei), including reporters

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-24-2022](https://weekinethereumnews.com/week-in-ethereum-news-december-24-2022)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jan 8 – [Solidity developer survey](https://blog.soliditylang.org/2022/12/07/solidity-developer-survey-2022-announcement/) deadline

- **Jan 11 – Flashbots** [**MEV Roast: Privacy**](https://collective.flashbots.net/t/mev-roast-privacy-january-11th-2023/935)

- Jan 17-31 – [Gitcoin grants round](https://go.gitcoin.co/blog/announcing-the-gitcoin-alpha-tests)

- Jan 31 – [KZG ceremony grants](https://blog.ethereum.org/2022/12/15/kzg-ceremony-grants-round) deadline

- **Feb 24 - Mar 1 –** [**ETHDenver BUIDLWeek**](https://www.ethdenver.com/)

- Mar 2-5 – [ETHDenver Hackathon](https://www.ethdenver.com/)

- **Mar 10-29 –** [**Scaling Ethereum**](https://ethglobal.com/events/scaling2023) **(ETHGlobal) virtual**

- Mar 15-16 – [ETHDubai](https://www.ethdubaiconf.org/)

- **Mar 28-30 –** [**Ethereum Rio**](https://www.ethereumbrasil.com/ethereumrio)

- Apr 3-6 – [Edcon](https://edcon.io/) Vienna

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- **Apr 14-16 –** [**ETHGlobal Tokyo**](https://tokyo.ethglobal.com/)

- **May 26–28 –** [**ETHGlobal Istanbul**](https://ethglobal.com/events/istanbul)

- **Jun 23–25 –** [**ETHGlobal Toronto**](https://ethglobal.com/events/toronto)

- **Jul 17-20 –** [**EthCC**](https://ethcc.io/) **(Paris)**

- **Jul 21–23 –** [**ETHGlobal Paris**](https://ethglobal.com/events/paris2023)

- **Sep 22–24 –** [**ETHGlobal New York**](https://ethglobal.com/events/newyork2023)

- **Oct 6–25 –** [**ETHOnline**](https://ethglobal.com/events/ethonline2023) **(ETHGlobal) virtual**

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

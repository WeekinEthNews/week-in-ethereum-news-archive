---
title: "Week in Ethereum News <br> April 29, 2023"
date: "2023-04-29"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=ajLQVC3E_mk&t=160s). Summary by [Tim Beiko](https://twitter.com/TimBeiko/status/1651613083931119617).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1651991286738743296) and [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-execution-call-160/):
    - Cancun upgrade to include: EIP4844 (protodankscaling), EIP6780 (SELFDESTRUCT only in same tx), EIP1153 (transient storage) & EIP6475 (SSZ optional type)
    
    - Cancun may potentially include: EIP4788 (beacon block root in EVM), EIP6493 (SSZ tx signature scheme) & EIP2537 (BLS precompile)
    
    - EOF not in Cancun, discussed making main feature of future upgrade

- [EIP4844 devnet 5](https://4844-devnet-5.ethpandaops.io/) successfully launched

- [KZG Ceremony](https://ceremony.ethereum.org/): 91,000+ contributions, contribute with an [account nonce of 64](https://twitter.com/carlbeek/status/1651640315504361474)

**Layer 1**

- [MEV-Boost relay vulnerability disclosed](https://collective.flashbots.net/t/disclosure-mitigation-of-block-equivocation-strategy-with-early-getpayload-calls-for-proposers/1705), block equivocation strategy with early getPayload calls

- [Rinkeby testnet](https://twitter.com/peter_szilagyi/status/1651606721532506112) Q2/Q3 shutdown proposed for June 1

- [Geth](https://twitter.com/peter_szilagyi/status/1651593996483870724) removing Clique & PoW support

**Client releases**

- Consensus layer:
    - Nimbus [v23.4.0](https://github.com/status-im/nimbus-eth2/releases/tag/v23.4.0): fixes missed proposals (low probability)
    
    - Teku [v23.4.0](https://github.com/ConsenSys/teku/releases/tag/23.4.0): fix for slow block processing with multiple voluntary exits

- Execution layer:
    - Erigon [v2.43.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.43.0): adds [Caplin](https://erigon.substack.com/p/announcing-caplin-erigon-full-consensus) phase 1 (embedded Consensus Layer); [diagnostics](https://github.com/ledgerwatch/diagnostics#readme) web app

**Research**

- [MEV-Boost & fork choice rule](https://www.paradigm.xyz/2023/04/mev-boost-ethereum-consensus): impact of latency on consensus

- [Overview of dankscaling](https://a16zcrypto.com/content/article/an-overview-of-danksharding-and-a-proposal-for-improvement-of-das/): proposal to use 25% of samples for reconstruction

- [Post quantum stealth addresses](https://ethresear.ch/t/towards-practical-post-quantum-stealth-addresses/15437) using Commutative Supersingular isogenies (CSIDH)

- [Confirmation rule](https://www.adiasg.me/confirmation-rule-for-ethereum/): typically under 1 minute, weaker guarantee than finality

**Layer 2**

- Proposal for [cross layer communication](https://ethresear.ch/t/cross-layer-communication-trivially-provable-and-efficient-read-access-to-the-parent-chain/15396) using a precompile to read the Layer 1 state root

**EIPs/Standards**

- EIPs:
    - [EIP6953](https://github.com/ethereum/EIPs/pull/6953/files): Network upgrade activation triggers

- ERCs:
    - [ERC6927](https://github.com/ethereum/EIPs/pull/6927/files): NFT fusing protocol
    
    - [ERC6932](https://github.com/ethereum/EIPs/pull/6933/files): Subscription-based token
    
    - [ERC6944](https://github.com/ethereum/EIPs/pull/6944/files): ERC5219 resolve mode

* * *

### **This newsletter is made possible thanks to the funding received from Optimism’s** [**RetroPGF**](https://optimism.mirror.xyz/Upn_LtV2-3SviXgX_PE_LyA7YI00jQyoM1yf55ltvvI?rpgf)**!**

![Optimism's RetroPGF: Week in Ethereum News](https://weekinethereumnews.com/wp-content/uploads/2023/04/RetroPGF-WiEN-1024x546.png)

Thank you to [Optimism’s RetroPGF round 2](https://optimism.mirror.xyz/Upn_LtV2-3SviXgX_PE_LyA7YI00jQyoM1yf55ltvvI?rpgf) which generously funded Week in Ethereum News for “months, not weeks.”

* * *

**Stuff for developers**

- Foundry Forge-std [v1.5.4](https://github.com/foundry-rs/forge-std/releases/tag/v1.5.4): adds set breakpoint cheat and count overload to expectCall cheat

- [Forge-deploy](https://github.com/wighawag/forge-deploy#readme): track deployments by name and reuse in Solidity

- [Solc-ast-rs](https://github.com/hrkrshnn/solc-ast-rs#readme): Rust bindings for Solidity AST & visitors

- [Slitherin](https://github.com/pessimistic-io/slitherin#readme): custom Slither detectors with higher sensitivity but higher false positives

- [Equivalence checker](https://medium.com/certora/how-to-optimize-your-gas-consumption-without-getting-rekt-695ece5354ca): compare code in Yul/assembly, Solidity or Certora Verification Language

- [Contract Fiesta](https://twitter.com/gf_256/status/1650512743349338119): dataset of source code for 150k unique contracts

- Safe: [ERC2535 (Diamond proxy) unsuitable for smart accounts](https://safe.mirror.xyz/P83_rVQuUQJAM-SnMpWvsHlN8oLnCeSncD1txyMDqpE) (account abstraction)

- [Governance proposal simulation framework](https://medium.com/@elliotfriedman3/secure-governance-testing-framework-f7bd735e024e): catch incorrectly linked contracts, invalid state transitions, broken dependencies and logic errors

- Curta CTF [Groovy Fruit Fiesta solution](https://twitter.com/gf_256/status/1651346013792227332)

- All Wallet Devs [call video](https://www.youtube.com/watch?v=JRmvcd2Ld50) and [notes](https://twitter.com/_SamWilsn_/status/1650549875816247320)

- Zokrates [v0.8.7](https://github.com/Zokrates/ZoKrates/releases/tag/0.8.7): Nova experimental support

- [zkLLVM & Proof Market](https://blog.nil.foundation/2023/04/26/proof-market-and-zkllvm-pipeline.html): guide to integrating zk proofs

**Security**

- [Mysterious wallet drainer](https://mirror.xyz/blockmage-labs.eth/Kpb0z8WruhXOtNEal3AAjROzLlleGiu5JprgkHp2QgE) (described by Taylor last week): victims encouraged to come forward

- Merlin DEX on zkSync [$1.8 million stolen](https://rekt.news/merlin-dex-rekt/), devs had unlimited approval

- Blur NFT marketplace [canceled bids were accepted](https://twitter.com/PacmanBlur/status/1649650815592972288)

- Trust wallet [browser extension vulnerability disclosed](https://blog.ledger.com/Funds-of-every-wallet-created-with-the-Trust-Wallet-browser-extension-could-have-been-stolen/), mnemonics could be found by brute force, $100k bounty paid

- [Profanity Brute-force](https://github.com/rebryk/profanity-brute-force#readme): reconstruct a private key generated using Profanity

**Ecosystem**

- [Staking deposit queue](https://twitter.com/wenmerge2022/status/1651473751803072512) flipped exit queue

**Notable at app layer**

- ENS manager app [v3](https://twitter.com/dr3a_eth/status/1650996926806933505) and [ENS Name Wrapper](https://twitter.com/sadaf_eth/status/1651635520919961600) live

- Gitcoin Passport [Unique Humanity Score](https://twitter.com/gitcoinpassport/status/1650883101717848066) of 15 needed for Gitcoin Grants Beta Round matching

- [Stelo Explore](https://blog.stelolabs.com/stelo-explore-safe-sharable-transactions-on-stelo-com/): universal contract interface

- Eric Wall’s [Orb](https://eric.orb.land/) NFT: holder can ask Eric a question a week, 300% Harberger tax

* * *

### Job Listings

- [Snr React Native UI Dev](https://grnh.se/2fada6031us) at Status: [All jobs](https://grnh.se/9fc6e6fc1us)

- Solidity team need a highly skilled [Developer Advocate](https://jobs.lever.co/ethereumfoundation/b9e33c9e-48ee-464f-a672-d51eece2b99d)

- Mimic seek a [blockchain engineer](https://mimic-fi.notion.site/Blockchain-engineer-f70df67acbba4dd1a39e974767f9c709) 

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Professor Gary Gensler in 2018 MIT course: “[3/4 of the market is non-securities](https://twitter.com/ZK_shark/status/1650689125580668931)“

- Binance US terminated [$1 billion purchase deal of Voyager assets](https://twitter.com/investvoyager/status/1650921887512272917)

- [UK tax proposal](https://www.gov.uk/government/consultations/the-taxation-of-decentralised-finance-involving-the-lending-and-staking-of-cryptoassets/the-taxation-of-decentralised-finance-defi-involving-the-lending-and-staking-of-cryptoassets--2) to not treat DeFi transactions as disposals

- Paul Brody: [enjoy the final Crypto Winter](https://www.coindesk.com/consensus-magazine/2023/04/26/us-crypto-regulations-end-crypto-winter-opinion)

**General/crypto**

- [TxRank](https://arxiv.org/abs/2304.12749): transaction anomaly detection tool using a Large Language Model

- [HyperNova](https://eprint.iacr.org/2023/573): recursive arguments for customizable constraint systems

- [Zator](https://github.com/lyronctk/zator/tree/main#readme): verified inference of a 512-layer neural network using recursive SNARKs

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-april-29-2023](https://weekinethereumnews.com/week-in-ethereum-news-april-29-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- May 5-10 – [ETHTallinn](https://ethtallinn.org/) hackathon & [NFT Tallinn](https://nfttallinn.com/) conference

- May 9 – [Gitcoin Grants Beta Round](https://grants.gitcoin.co/) ends **(support** [**Week in Eth News**](https://explorer.gitcoin.co/#/round/1/0xaa40e2e5c8df03d792a52b5458959c320f86ca18/0xaa40e2e5c8df03d792a52b5458959c320f86ca18-53)**)**

- May 9-12 – [EY blockchain summit](https://web.cvent.com/event/c066d44d-4e50-4d7e-b6fb-3cc0abdae7ff/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7)

- **May 11-14 –** [**Pragma Lisbon**](https://ethglobal.com/events/pragma-lisbon) & [ETHGlobal Lisbon](https://ethglobal.com/events/lisbon) hackathon

- May 19-23 – [EDCON](https://edcon.io/) Montenegro (changed from Vienna)

- May 20-21 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 24-26 – [Spaghett ETH](https://naples.spaghett-eth.com/) (Naples) conference

- May 26-28 – [ETHDublin](https://www.ethdublin.io/) hackathon

- Jun 2-4 – [ETH Seoul](https://2023.ethseoul.org/)

- Jun 2-7 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 9-11 – [ETHPrague](https://ethprague.com/) conference & hackathon

- Jun 23–25 – [ETHGlobal Waterloo](https://ethglobal.com/events/waterloo2023) (changed from Toronto)

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Aug 13-16 – [ETHToronto](https://www.ethtoronto.ca/) & [ETHWomen](https://www.ethwomen.com/)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org/) (Buenos Aires)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 30 – Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 18-21 – [ETH Montréal](https://ethmontreal.xyz/) hackathon & conference

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- **Oct 5-6 –** [**ETHMilan**](https://www.ethmilan.xyz/) **conference**

- Oct 6–27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 27–29 – [ETH Miami](https://ethmiami.net/) festival + hackathon

- Oct 28–30 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 17-19 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

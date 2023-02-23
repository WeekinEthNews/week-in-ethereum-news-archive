---
title: "Week in Ethereum News <br> December 11, 2021"
date: "2021-12-11"
---

## **Eth News and Links**

**Mainnet execution layer**

- [Arrow Glacier](https://twitter.com/TimBeiko/status/1469035839443193860) upgrade pushing back the difficulty bomb was successful
- Latest [core devs call video](https://www.youtube.com/watch?v=Py1_Bw0frO0&t=48s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1469388841375059971):
    - PoW switch off key tasks: optimistic sync, fork choice rules for competing terminal PoW blocks, authentication between execution & consensus layers and lots of testing
    - EIP4488 (call data gas price reduction) will not be done before PoW switch off
    - Post PoW proposals need to be prioritized with community input, e.g. withdrawals vs sharding/EIP4488
- Besu [v21.10.3](https://github.com/hyperledger/besu/releases/tag/21.10.3): log4j zero-day vulnerability, update immediately or manually mitigate
- Piper Merriam’s [Aperture Portal Network update](https://snakecharmers.ethereum.org/the-aperture-vol-4/): changing focus from State network to Chain History network 

**EIPs/Standards**

- [EIP4515](https://github.com/ethereum/EIPs/blob/6ea92279acd07388138d34b11022a44e04a2f64b/EIPS/eip-xtndr-family.md): XTNDR opcode family
- [EIP4520](https://eips.ethereum.org/EIPS/eip-4520): Multi-byte opcodes prefixed by EB and EC
- [EIP4524](https://github.com/ethereum/EIPs/blob/7758dcbcd1b5cc531c72483115de8ff0c3548528/EIPS/eip-4524.md): Safer ERC20
- [EIP4527](https://github.com/ethereum/EIPs/blob/f99d356388f29cbbff0133bd5e3a7373bbafb471/EIPS/eip-4527.md): QR Code data transmission protocol for the Ethereum wallets

**Proof of Stake consensus layer**

- Guide to [join PoW switch off devnet-3](https://github.com/remyroy/ethstaker/blob/main/merge-devnet.md)
- Teku [security update](https://github.com/ConsenSys/teku/security/advisories/GHSA-mwfw-vm54-g3p7) (v21.12.1): log4j zero-day vulnerability, Teku not believed to be vulnerable but update immediately or manually mitigate
- Nimbus [v1.5.5](https://github.com/status-im/nimbus-eth2/releases/tag/v1.5.5): optimizations, 6x epoch processing & 2x Altair block processing
- [Lodestar consensus light-client demo](https://lodestar-light-client-demo.netlify.app/): tracks the head trustlessly, sync to head is 25KB/day of data, follow head is 81KB/day
- [Light nodes](https://our.status.im/light-nodes-ethereum-endgame/) can offer similar security guarantees as full nodes if enough people run full and light nodes, need to make them easy to run on consumer hardware

**Layer2**

- [Mir team joins Polygon](https://blog.polygon.technology/polygon-takes-a-major-lead-in-zk-rollups-welcomes-mir-a-groundbreaking-zk-startup-in-a-400m-deal) to build Polygon Zero zk-rollup, pivot from Layer 1 to an Ethereum Layer 2
- [Aztec Connect](https://twitter.com/aztecnetwork/status/1469121178228994051): private bridge live on testnet, aggregates like transactions from Aztec users to interact with Layer 1 DeFi
- Proto’s EVM equivalence endgame is [Yellow-Paper equivalence](https://twitter.com/protolambda/status/1463930245820596225)
- [dYdX state explorer](https://twitter.com/l2beatcom/status/1468890316946264069) to be built by L2BEAT, showing decoded calldata on Layer 1 and allow forced exits & trades by sending a Layer 1 transaction
- [L2BEAT](https://medium.com/l2beat/is-the-6b-locked-in-l2-secure-895cba23d026): how to monitor that $6 billion locked in Layer 2 is secure
- Polynya’s rollup fees [explainer](https://polynya.medium.com/how-rollup-fees-work-ddaa34f64c08): why they get cheaper to use as Layer 2 adoption increases

* * *

### **This newsletter is made possible thanks to [Celer Network](https://www.celer.network/)!**

![Celer](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

Celer Network is a layer-2 scaling platform that brings fast, secure and low-cost blockchain applications.

[cBridge](https://cbridge.celer.network/) has done almost $1.5b in volume moving ETH, USDT, and USDC between Ethereum mainnet, Optimism, Arbitrum, Avalanche, Boba, Fantom, BSC and Polygon.

LIQUIDITY MINING [launches December 15th](https://blog.celer.network/2021/12/10/cbridge-liquidity-mining-session-one-is-launching-on-12-15-2021/) for $ETH, $USDT and $USDC, with rewards paid in $CELR 

* * *

**Stuff for developers**

- [Solidity](https://twitter.com/ethchris/status/1467833132032606209) prototype of user-defined operators on user-defined types
- Ethers.js [update](https://blog.ricmoo.com/highlights-ethers-js-december-2021-dc1adb779d1a): ENS avatars in v5; v6 assumes ES2016, TypeScript changes, uses new crypto libraries, dynamic & typed Contract methods, Network object makes Layer 2 providers easier to create & use
- [Foundry](https://www.paradigm.xyz/2021/12/introducing-the-foundry-ethereum-development-toolbox/): fast testing framework for tests written in Solidity, Rust reimplementation of dapptools
- [kryptology](https://github.com/coinbase/kryptology): Coinbase cryptographic library, Apache-2.0 license
- Slither [v0.8.2](https://github.com/crytic/slither/releases/tag/0.8.2): Solidity v0.8 feature support (custom errors, top level functions, immutable variables) and detectors for in loop delegatecall & msg.value
- truffle-plugin-verify [v0.5.20](https://github.com/rkalis/truffle-plugin-verify/releases/tag/v0.5.20): verifies proxy implementation on Etherscan and flags as a proxy
- [Argent X](https://github.com/argentlabs/argent-x): browser extension StarkNet wallet, currently ~4 minutes to deploy on Goerli, ~2 hours on mainnet
- [Tenderly](http://blog.tenderly.co/you-can-now-use-arbitrum-on-tenderly/) adds Arbitrum support
- [Batch data retrieval](https://twitter.com/libevm/status/1467376978697211904) using GraphQL on Geth
- [Dodoc](https://github.com/primitivefinance/primitive-dodoc): documentation generation from Solidity, zero-config Hardhat plugin

**Security**

- BadgerDAO’s $121 million [exploit post mortem](https://badger.com/technical-post-mortem), Cloudflare Workers script deployed using compromised API key, intermittently phished ERC20 token approvals
- dYdX [deposit proxy post mortem](https://dydx.exchange/blog/deposit-proxy-post-mortem), contract had user ERC20 approvals and could make arbitrary calls, $200k stolen, $500k bug bounty paid

**Ecosystem**

- Vitalik’s [scalable blockchain endgame](https://vitalik.ca/general/2021/12/06/endgame.html): block production may become centralized due to network effects within rollups or cross-domain MEV, but with decentralized validation and anti-censorship protection
- Flashbots Protect RPC [v0.4.0](https://docs.flashbots.net/flashbots-protect/rpc/releases/#040): adds free transaction cancellations
- Josh Stark’s draft [guide to joining the Ethereum ecosystem](https://docs.google.com/document/d/1VaMg0h04LWigDWg1Eh5dqHXYPzvYNiVvOuUShTuCrXU/edit) \[Google doc\], to be sent to 1000+ applicants for EF internship, contributions welcome

**Enterprise**

- [Reddit expanding Community Points](https://www.reddit.com/community-points) to additional subreddits; [pros and cons](https://www.reddit.com/r/ethereum/comments/rcyenl/hearing_a_lot_about_community_points_around_here/) of points
- [Pepsi](https://micdrop.pepsi.com/) 1,893 profile pic NFTs, free + gas via US only waitlist
- [WhiteCastle](https://twitter.com/WhiteCastle/status/1469034170357854217) changes Twitter handle to ENS
- [CryptoPunk #6457](https://twitter.com/jkrantz/status/1468967566827679752) sponsored by hair loss serum

**Application layer**

- [Messari Governor](https://messari.io/article/introducing-messari-governor-the-first-to-market-governance-aggregator-and-voting-platform): governance aggregator, supports Snapshot, Governor Alpha & Bravo
- [Coinbase](https://blog.coinbase.com/coinbase-makes-it-easy-to-earn-yield-with-defi-bd38156e2715) offers yield on Dai using Compound, covers gas fees, available in 70 countries (excludes US)
- [Pods](https://blog.pods.finance/integrating-with-arbitrum-5fdb759149b2) on-chain options protocol live on Arbitrum
- Enso Finance [vampire attack](https://medium.com/ensofinance/vampire-attack-6-protocols-8d1a1454ec3f) of index projects
- [xToken](https://medium.com/xtoken/guide-to-xtoken-launch-on-arbitrum-faf2d85627cc) lending protocol live on Arbitrum
- [dHEDGE](https://twitter.com/dHedgeOrg/status/1468791653469020168) decentralized hedge funds live on Optimism
- [WAVEFORM](https://opensea.io/assets/0x7908e11e21fb82429a0d2687770472723ae8148d/680564733841876926926749214863536422913) 1/1 music NFT produced by 3LAU with full master recording & publishing rights
- [Sound](https://www.sound.xyz/): limited edition song NFTs
- [Unlock](https://unlock-protocol.com/blog/optimism) NFTs as memberships live on Optimism
- [WorthInNFT](https://www.worthinnft.com/): value of NFT assets for an address, supports ENS
- [Inb0x](https://medium.com/parallel-life/engineering-inb0x-7e3acddcb1a9): address to address messaging with end to end encryption

* * *

### **Job Listings**

- Kwenta is hiring! [Frontend Engineer](https://blog.kwenta.io/kwenta-open-position-front-end-developer/), [Solidity Engineer](https://blog.kwenta.io/kwenta-open-position-solidity-engineer/) & [Marketing Lead](https://blog.kwenta.io/kwenta-open-position-marketing-manager/)
- OpenZeppelin are hiring a [Community Manager](https://openzeppelin.com/jobs/opening/?gh_jid=4847457003)
- Ethereum Foundation: [DevOps](https://ethereum.bamboohr.com/jobs/view.php?id=53&source=weekinethnews) for Consensus Layer clients in lead up to merge
- Trail of Bits [summer internship 2022](https://jobs.lever.co/trailofbits/de190abd-ec89-4c72-bda8-d411741a4c32)
- Nethermind 1-3 month [internship program](https://www.notion.so/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)

**Reach developers experienced with Ethereum.  DECEMBER SPECIAL: $200** for two issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US derivatives exchange [CME Group](https://www.cmegroup.com/media-room/press-releases/2021/12/06/cme_group_announceslaunchofmicroetherfutures.html) launches Micro Ether futures (1/10th of an Ether)
- [xDai & Gnosis token merger](https://twitter.com/xdaichain/status/1468275625114972165) on track to happen
- [Decentralized governance structures](https://medium.com/fei-protocol/decentralized-governance-structures-9c4eb8a3e452): token governance (direct democracy), optimistic governance (representative democracy) and security guardian (conditional omnipotence)
- [Graph-based analysis](https://twitter.com/epfl_scistimm/status/1468162434703757314) of NFT transactions
- [Challenges in blockchain gaming](https://mirror.xyz/sylve.eth/6QJ6taBcobFAWMbijs4WrQrFZ_FGq5wXmJ_NIXW-GmQ): multi-accounting, key management, hiding information on-chain and cheat-to-earn

**General**

- Blockchain-based approach for [collaborative formalization of mathematics & programs](https://twitter.com/0xjinxinglim/status/1468111277708873728)
- [Novi digital wallet](https://twitter.com/skasriel/status/1468722859648307201) US pilot, sending and receiving USDP on WhatsApp
- Machine-readable [fuzzing corpora directory](https://github.com/guidovranken/fuzzing-corpora-directory) 
- Practical [asynchronous Distributed Key Generation](https://eprint.iacr.org/2021/1591)
- Java logging library [Log4j2 zero-day](https://www.lunasec.io/docs/blog/log4j-zero-day/) remote code execution

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-11-2021](https://weekinethereumnews.com/week-in-ethereum-news-december-11-2021)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Dec 11 – [Codeless Conduct](https://medium.com/@alexnmr/announcing-codeless-conduct-no-coding-skills-needed-efa0a409b360) no-code hackathon (virtual)
- Dec 16 – [Gitcoin Grants Round 12](https://gitcoin.co/blog/whats-new-in-the-gitcoin-grants-product/) ends (support [Week in Eth News](https://gitcoin.co/grants/2785/week-in-ethereum-news))
- **Jan 22-23 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)**
- Jan 24-26 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford University)
- Feb 17 – [Schelling Point](https://schellingpoint.gitcoin.co/) (Denver) 
- Feb 18-20 – [ETHDenver](https://www.ethdenver.com/)
- Mar 28-30 – [ETHDubai](https://www.ethdubai.xyz/)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

---
title: "Week in Ethereum News<BR> March 9, 2020"
date: "2020-03-09"
---

## **Eth News and Links**

**Eth1**

- Latest [core devs call](https://youtu.be/kham8c0qhmw) on ProgPoW and EIP1962/curve precompiles. [Notes](https://twitter.com/TimBeiko/status/1235924874973138944). ProgPoW appears to be dead.
- A [ProgPoW exploit](https://github.com/kik/progpow-exploit) from Kikx. Kristy’s [explanation](https://twitter.com/OhGodAGirl/status/1235358803668975617)
- Trinity [v0.1.0-alpha.35](https://trinity-client.readthedocs.io/en/latest/release_notes.html#trinity-0-1-0-alpha-35-2020-03-03), Beam Sync with better pivots, -goerli flag, ENRs
- [DHT solution to solve data retrieval problem](https://ethresear.ch/t/dht-based-solution-for-the-data-retrieval-problem-under-the-stateless-paradigm/7070) in stateless Ethereum

**Eth2**

- Latest [what’s new in Eth2](https://hackmd.io/@benjaminion/wnie2_200306)
- [Prysmatic client](https://medium.com/prysmatic-labs/eth-2-0-dev-update-45-cross-compiles-slashing-protection-2e6359e15195) update - big RAM reduction, first slashing success, updated to latest spec
- [Lighthouse client](https://lighthouse.sigmaprime.io/update-22.html) update - 70% faster block processing, 110 blocks/sec sync, big RAM reduction
- [zk tooling for an ewasm EE](https://ethresear.ch/t/zero-knowledge-tooling-for-an-eth-2-0-wasm-execution-layer/7080)
- [Combining Ghost and Casper](https://arxiv.org/abs/2003.03052) paper proving safety and liveness under various assumptions

**Layer2**

- iden3’s [zk-rollup is live](https://blog.iden3.io/announcing-zkrollup-first-public-testnet.html) on Goerli testnet, ongoing work to reduce the proof generation bottleneck

**Stuff for developers**

- [any.sender tutorial](https://github.com/PISAresearch/docs.any.sender/tree/master/docs/echoWalkthrough) - tx relayer that ensures block inclusion by a certain time
- [Kollateral](https://twitter.com/kollateralco/status/1235994141055574016) flash loan pool aggregator, available through JS or Solidity (though unaudited!)
- [Why ENS had to migrate](https://medium.com/the-ethereum-name-service/lets-talk-ens-migration-a92d5c21df28) due to samczsun’s bughunting
- [Easy multi-contract analysis](https://blog.mythx.io/misc/easy-multi-contract-security-analysis-using-mythril/) with Mythril
- [Fast modular multiplication in Go](https://hackmd.io/@zkteam/modular_multiplication) library
- [BSol](https://medium.com/@giulio.rebuffo/bsol-benchmarking-solidity-smart-contract-acd78f3b259b): benchmarking Solidity computation and gas usage
- Truffle [v5.1.16](https://github.com/trufflesuite/truffle/releases/tag/v5.1.16) - better debugger/decoder with Solc v0.6.3
- [Understanding event logs](https://medium.com/mycrypto/understanding-event-logs-on-the-ethereum-blockchain-f4ae7ba50378)
- [Terminal and IPFS for easy frontend deployment](https://medium.com/coinmonks/terminal-co-ipfs-web3-deployment-simplified-da70efee7e74)
- Argent’s [method for easy wallet access](https://medium.com/argenthq/faster-cheaper-and-safer-dapp-access-70057611ed46), one click transactions, available as npm package
- web3connect is now [web3modal](https://www.npmjs.com/package/web3modal), still focused on being a web3 solution for all wallets

**Ecosystem**

- [Semaphore](https://medium.com/@weijiek/release-announcement-semaphore-a-zero-knowledge-gadget-for-ethereum-5b671cd360d4): a generic privacy layer using snarks, audited and ready for devs to build on
- [Zeropool, live on testnet](https://twitter.com/ZeroPoolNetwork/status/1235220309596393473)
- [Questions DeFi users should ask](https://diligence.consensys.net/blog/2020/03/questions-defi-users-should-be-asking-defi-developers/) their DeFi apps
- Linda Xie’s [list of oracles](https://docs.google.com/spreadsheets/d/1zdCqw5E4ljSL1KYpjimX6RVrkg_2leHMZGEikv610ac/edit#gid=0) per DeFi project
- [EthCC videos](https://www.reddit.com/r/ethereum/comments/fcsolo/ethcc_3_livestreams/) are already online.

**Enterprise**

- [EY, Microsoft and ConsenSys announce the Baseline Protocol](https://consensys.net/blog/press-release/ey-and-consensys-announce-formation-of-baseline-protocol-initiative-to-make-ethereum-mainnet-safe-and-effective-for-enterprises/), using mainnet as a message bus for enterprise that is private using snarks
- Paul Brody’s [Baseline Protocol explainer](https://www.reddit.com/r/ethfinance/comments/fds4sy/a_sort_of_baseline_explainer_faq/), based around the enterprise volume procurement prototype
- “[Morningstar Rates First Ethereum Security In $40 Million Fatburger Deal](https://www.forbes.com/sites/michaeldelcastillo/2020/03/08/morningstar-rates-first-ethereum-debt-security-in-40-million-fatburger-deal/#1326e6292abd),” with the deal structurer aiming at doing 500m USD in projects this year on mainnet

**Governance, DAOs, and standards**

- An [update on EIP1559](https://eipupdate.substack.com/p/eip-update-issue-1-eip-1559) - predictable transaction fees and intrinsically tying ETH to the protocol
- [OracleDAO](https://hackmd.io/@oracle-dao/Sk-uHkX78) - a MolochDAO style booster of Augur/REP
- [0x governance](https://blog.0xproject.com/0x-governance-in-2020-and-beyond-9e7703bc1c54) update, progressing toward full decentralization

**Application layer**

- [PieDAO](https://medium.com/piedao/introducing-piedao-the-asset-allocation-dao-1af9eec5ee4), a DeFi asset allocation DAO, where governance tokens vote for allocations with fees accruing to the token
- [Providing insurance on Opyn](https://medium.com/opyn/providing-insurance-on-opyn-b370e67a709a) to earn premiums from your ETH
- [Building liquidity into token distribution](https://medium.com/balancer-protocol/building-liquidity-into-token-distribution-a49d4286e0d4), highlighting the flexibility of Balancer
- [Hegic Protocol](https://ethresear.ch/t/announcing-hegic-protocol-and-the-concept-of-a-hedge-contract/7023), on-chain options trading protocol
- [Golem Hive](https://blog.golemproject.net/golem-hive/), PoC of a virtual network of Docker containers on Golem
- [Unstoppable Domains adds a Chromium-based browser](https://unstoppabledomains.com/browser) running a local IPFS node
- Sell [music tracks](https://twitter.com/zpl1t/status/1235859268630228992) with Unlock + IPFS + ENS
- Instadapp’s [DeFi accounts](https://blog.instadapp.io/defi-smart-accounts/) to abstract things away for DeFi users
- [Messaging and privacy in Status](https://our.status.im/breaking-down-the-private-secure-messenger/)

**Tokens/Business/Regulation**

- India’s Supreme Court [reverses crypto banking ban](https://www.reuters.com/article/us-india-cryptocurrency-idUSKBN20R0KV)
- [pTokens](https://medium.com/provable/ptokens-launch-on-mainnet-8c0a0cffa24f) launch on mainnet, starting with pBTC
- [Decrypt will launch its own OST token](https://decrypt.co/21234/decrypt-announces-the-launch-of-its-own-token)

**General**

- Guido Vranken releases his [fuzzing engine](https://github.com/guidovranken/vfuzz)
- Lego Factory: [why I’m stewarding the 1 million Eth devs movement](https://medium.com/1milliondevs/why-im-stewarding-the-one-million-developers-movement-2536c1be26fe)
- Two Eth2 staking user surveys from [Aqeel/Lighthouse](https://docs.google.com/forms/d/e/1FAIpQLSfDgb4KX23jFqkTj9z5ly2wp5Nc6O2Yyn3f5Ihx2q4m5dY6YA/viewform) and [CodeFi](https://www.surveygizmo.com/s3/5478500/3b7114adf13d)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Mar 14 - [Augur v1 cutoff](https://github.com/AugurProject/augur-app/releases/tag/v1.16.10)
- **Mar 16-30 - Gitcoin’s [Funding the Future](https://hackathons.gitcoin.co/funding-the-future) virtual hackathon**
- Mar 29-Apr4 - [EthLagos](https://ethlagos.io/)
- Apr 3-6 - [NonCon](https://noncon.org/) (Vienna)
- Apr 13 - Deadline to apply for [50k euro for blockchain startup](https://blockchers.eu/open-calls/)s in Europe
- Apr 24-26 - [EthTurin](https://ethturin.com/)
- Apr 29-30 - [SoliditySummit](https://solidity-summit.ethereum.org/) (Berlin)
- May 7 - [SmartCon0](https://blog.chain.link/announcing-the-smart-contract-summit-smartcon-0-powered-by-chainlink/) (NYC)
- May 8-9 - [Ethereal Summit](https://www.etherealsummit.com/) (NYC)
- May 15-17 - [ETHNYC](https://nyc.ethglobal.co/)
- May 15 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

* * *

## **Thank you, ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum News. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

* * *

## **I really want you to link to [weekinethereumnews.com](https://weekinethereumnews.com/)**

Issue permalink: [https://weekinethereumnews.com/week-in-ethereum-news-march-9-2020/](https://weekinethereumnews.com/week-in-ethereum-news-march-9-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

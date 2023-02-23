---
title: "Week in Ethereum News <BR> September 13, 2020"
date: "2020-09-13"
---

## **Eth News and Links**

**Eth1**

- Geth [v1.9.21](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.21), stabilized RAM use in fast sync, extends call tracing
- [OpenEthereum’s vision for Parity client](https://medium.com/openethereum/vision-for-openethereum-ex-parity-client-eb7b11f6eef8): focus on Eth mainnet. As such, deprecating IPFS/Swarm as well as Kovan testnet and other non-Ethereum chains, backporting features to the v2.5 codebase
- Latest [Turbogeth weekly alpha release](https://github.com/ledgerwatch/turbo-geth/releases/tag/v2020.09.02), RPC Daemon improvements and new RPC calls
- Intro to [Nethermind’s discovery protocol](https://medium.com/nethermind-eth/introduction-to-nethermind-discovery-protocol-4bb17ea31d1f)
- Tim Beiko is looking to talk to [heavy gas users, wallets, exchanges, miners, infra about the proposed eip1559 fee market change](https://twitter.com/TimBeiko/status/1303028695641120770)

**EIPs/Standards**

- A [proposed EIP process overhaul](https://hackmd.io/@axic/eip-overhaul) from axic
- Martin Swende benchmarks [cost of calling precompiles](https://gist.github.com/holiman/7153e088af8941379cf21c0e4610d51f)
- [EIP2972](https://eips.ethereum.org/EIPS/eip-2972): Wrapped Legacy Transactions

**Eth2**

- Latest [Nimbus client](https://our.status.im/nimbus-update-september-11th/) update - faster sync, better db pruner
- Latest [Prysmatic client](https://medium.com/prysmatic-labs/eth-2-0-dev-update-56-road-to-mainnet-3fbd50dde484) update - getting ready for mainnet, hardening to DoS attacks, no more eth1 node support
- Somer Esat’s [guide to staking with Nimbus](https://medium.com/@SomerEsat/guide-to-staking-on-ethereum-2-0-ubuntu-medalla-nimbus-5f4b2b0f2d7c?source=friends_link&sk=ee272e7d2c5c53f9e69f302155cb1714) using Ubuntu
- [Clock sync as oracle](https://ethresear.ch/t/clock-sync-as-a-decentralized-trustless-oracle/7959)

**Layer2**

- [A general-purpose L2-friendly ENS standard](https://ethereum-magicians.org/t/a-general-purpose-l2-friendly-ens-standard/4591)

* * *

### **This newsletter is made possible thanks to [Matcha by 0x](https://matcha.xyz/)!**

![Matcha](https://weekinethereumnews.com/wp-content/uploads/2020/06/matcha-avatar.png)

Matcha aggregates liquidity across decentralized exchange networks to offer you the best price on every token swap. [Trade 30+ DeFi tokens](https://matcha.xyz/) on Matcha today!

* * *

**Stuff for developers**

- Solidity is finally a [first class Github citizen](https://twitter.com/NomicLabs/status/1303010441954762754): automatic Solidity detection
- OpenZeppelin Contracts [v3.2](https://forum.openzeppelin.com/t/openzeppelin-contracts-3-2/3783), adds proxy contracts in Solidity v0.6
- Waffle now [supports the Jest testing framework](https://medium.com/ethworks/introducing-waffle-support-for-jest-experimental-331f39d630bd)
- Truffle [v5.1.44](https://github.com/trufflesuite/truffle/releases/tag/v5.1.44), debugger prints location on tx failure, node v12 works
- [EthOver VScode](https://diligence.consensys.net/blog/2020/08/actionable-smart-contract-addresses-for-vscode/) plugin for viewing source code, bytecode, disassembling
- Static analyzer Slither [v0.6.13](https://github.com/crytic/slither/releases/tag/0.6.13), better Solidity v0.6 support, some Yul support
- Py-RLP [v2](https://pypi.org/project/rlp/2.0.0a1/) (much faster due to internals in Rust)
- Headlong [v3.8](https://github.com/esaulpaugh/headlong/releases/tag/v3.8.0) - ABI v2/RLP for the JVM
- A walkthrough of [changes in Solidity v0.7](https://forum.openzeppelin.com/t/changes-in-solidity-0-7-0/3758)
- [Sharing common data using libraries](https://medium.com/coinmonks/sharing-common-data-using-libraries-6573857d328c)
- [Everything about events and logs](https://medium.com/linum-labs/everything-you-ever-wanted-to-know-about-events-and-logs-on-ethereum-fec84ea7d0a5) in Eth reference guide
- Using [TheGraph](https://soliditydeveloper.com/thegraph/) tutorial
- A [guide for devs new to Ethereum](https://snakecharmers.ethereum.org/a-developers-guide-to-ethereum-pt-1/) using Python

**Ecosystem**

- [Data challenge for the Medalla testnet](https://ethereum.org/en/eth2/get-involved/medalla-data-challenge/) - data viz, analysis, tools. Prizes up to 15k, submissions due October 20th
- Ethereum Foundation’s [q2 grant recipients](https://blog.ethereum.org/2020/09/08/esp-q2-updates/)
- MyCrypto’s [guide to eth2](https://medium.com/mycrypto/eth2-0-everything-you-need-to-know-eb32fbfe0bd) for casual Ethereum users
- [EthGas](https://ethgas.app/).app, a nice viz of the recent gasprice history as well as current prediction
- Chainlink’s [fair sequencing service](https://blog.chain.link/chainlink-fair-sequencing-services-enabling-a-provably-fair-defi-ecosystem/) research: let an oracle network order transactions to thwart MEV ([miner extractable value](https://arxiv.org/pdf/1904.05234.pdf), link to Daian, _et al_ paper). Required computation currently unfeasible, working on improvements

**Application layer**

- [SushiSwap’s Chef Nomi gives the 38k eth back](https://twitter.com/NomiChef/status/1304442495342796800)
- [yearn is going to compete with Maker](https://medium.com/iearn/introducing-stablecredit-a-new-protocol-for-decentralized-lending-stablecoins-and-amms-7252a43ee56)
- POAP as [proof of unique human](https://medium.com/@poap/the-core-value-proposition-of-poap-explained-dc379aca332d)
- Lots of likely useless forks this week, which you can see on Etherscan’s new [yield farming page](https://etherscan.io/yieldfarms)
- [LexCorpus](https://medium.com/lexdaoism/enter-lexdao-corpus-contracts-df01d8518019) a collection of code for registry, organization, tokens, and escrow to help form legal agreements

**Tokens/Business/Regulation**

- Investment firm [Arca calls for Gnosis to return money](https://www.theblockcrypto.com/post/76453/arca-gnosis-defi-project-call) to tokenholders
- [Organic growth in DeFi](https://medium.com/@vadymnesterenko/organic-growth-in-defi-19f4d71c0c9f)

**Crypto/General**

- [UltraPLONK](https://hackmd.io/Iuu9P7S5Sca0TCoYJ-sFdA): Plonk with Plookup gates
- [Lunar](https://eprint.iacr.org/2020/1069): a Toolbox for More Efficient Universal and Updatable zkSNARKs and Commit-and-Prove Extensions
- Vitalik: [coordination, collusion, and forks](https://vitalik.ca/general/2020/09/11/coordination.html)
- John Adler: [Nakamoto Consensus requires social coordination and subjectivity](https://talk.lazyledger.io/t/nakamoto-consensus-requires-social-coordination-and-subjectivity/28)

* * *

## **Job Listings**

- [OpenZeppelin](https://openzeppelin.com/jobs): Security Researcher, Security Platform Dev & Open Source Dev
- DeFi devs! Yield is hiring for Solidity and front-end - contact@yield.is
- Nexus Mutual: [experienced Solidity dev](https://angel.co/company/nexus-mutual-1/jobs/967538-smart-contract-engineer); prefer European timezones
- 0x is hiring devs! [Full-stack, back-end, front-end or Solidity](https://0x.org/about/jobs)
- Celer Network: hiring Solidity and Go devs. Email: hiring@celer.network
- Pioneer Chainlink’s QA frameworks as the very first [test engineer](https://careers.smartcontract.com/o/senior-software-engineer-test)
- Trail of Bits hiring elite [blockchain security engineers](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & an [R&D engineer](https://jobs.lever.co/trailofbits/94f47428-7c88-43dd-846d-93e3d3059337)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH/DAI/USDC to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **Staking pools get in touch**

With eth2 due to launch in a matter of weeks, I’m going to recommend staking pools to those of you who want to stake but don’t want to run their own stakers (which is preferred over a pool!). If you’re a [staking pool and want to do my diligence process](https://twitter.com/evan_van_ness/status/1303695151814963200), get in touch.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow me on twitter: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-13-2020/](https://weekinethereumnews.com/week-in-ethereum-news-september-13-2020/)

Did you get **forwarded** this newsletter? **[Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **Sep 14 - [Gitcoin grant](https://gitcoin.co/grants/) matching round starts**
- Sep 17 - [Q&A for devs new to Ethereum](https://twitter.com/ljxie/status/1301588925006319618)
- **Sep30 - Oct25 - [EthPlanet hackathon](https://ethplanet-hackathon.devfolio.co/)**
- Oct 1-30 - [EthOnline hackathon](https://www.ethonline.org/)
- **Oct 20 - [submission deadline for Medalla data challenge](https://ethereum.org/en/eth2/get-involved/medalla-data-challenge/)**
- Nov 6-7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)
- Nov 16 - [MetaMask Provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7)

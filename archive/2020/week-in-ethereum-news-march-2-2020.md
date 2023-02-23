---
title: "Week in Ethereum News<BR> March 2, 2020"
date: "2020-03-03"
---

## **Eth News and Links**

**Eth1**

- Notes from the [latest stateless ethereum call](https://blog.ethereum.org/2020/02/28/eth1x-files-digest-no-3/). Witness format and the data retrieval problem
- Latest [Nethermind fixes some peering issues](https://github.com/NethermindEth/nethermind/releases/tag/1.6.25)

**Eth2**

- the [Eth2 explainer to read first](https://ethos.dev/beacon-chain/)
- Latest [Eth2 call](https://www.youtube.com/watch?v=tLiMgFoG_vs). Notes from [Mamy](https://gist.github.com/mratsim/80d4a9f313c8c5cac3ac433d7ce810e4) and [Ben](https://hackmd.io/@benjaminion/SygoFBrVL)
- [Getting to Eth1 finality with Eth2](https://ethresear.ch/t/on-the-way-to-eth1-finality/7041)
- [Nimbus client](https://our.status.im/nimbus-status-update-february-so-far/) update. discv5, BLS sigs, lightweight stack traces
- The [train-and-hotel EE](https://ethresear.ch/t/the-train-and-hotel-ee/7021/2)
- [Rewards and penalties](https://codefi.consensys.net/blog/rewards-and-penalties-on-ethereum-20-phase-0) in eth2

**Layer2**

- [Loopring launches zk-rollup exchange](https://medium.com/loopring-protocol/loopring-launches-zkrollup-exchange-loopring-io-d6a85beeed21) doing 100 tx per second (with 2000 possible as the relayer gets optimized). Due to [snark prover optimizations](https://medium.com/loopring-protocol/zksnark-prover-optimizations-3e9a3e5578c0), it costs just 0.01 cents (ie, $0.000124) per trade
- Run [Fuel optimistic rollup in NodeJS in a few minutes](https://medium.com/@fuellabs/fuel-in-nodejs-in-under-10-minutes-adc5c2986672)
- PlasmaLeap is [switching to rollups](https://leapdao.org/blog/mainnet-shutdown/)

**Stuff for developers**

- Making [Solidity stack traces and console.log](https://medium.com/nomic-labs-blog/making-solidity-stack-traces-and-console-log-even-more-useful-c3c526d1860f) more useful with a JSON-RPC interface to connect to Buidler EVM from wallets and front ends
- A [linked list implementation](https://kauri.io/a-linked-list-implementation-for-ethereum/2b40f522f07a45f391dafebfaadc444d/a) in Solidity
- [Sokt](https://blog.web3labs.com/making-manual-solidity-version-management-a-thing-of-the-past): a library for managing multiple Solidity versions for Java or Kotlin
- Writing [upgradeable contracts in OpenZeppelin](https://simpleaswater.com/upgradable-smart-contracts/) tutorial
- Dapp starter kit using [Buidler + Waffle + TypeChain + Vue (TypeScript)](https://github.com/proofoftom/buidler-waffle-typechain-vue)
- [tx2uml](https://github.com/naddison36/tx2uml) generates a UML sequence diagram of all the contract calls, even in big txs
- [Gas stipends, the 1/64 rule, contract calls, and the insufficient gas griefing attack](https://ronan.eth.link/blog/ethereum-gas-dangers/)
- [Solfuzz](https://github.com/b-mueller/solfuzz/): assertion checker for Solidity contracts using gray box fuzzing
- [gnark](https://hackmd.io/@zkteam/gnark): fast groth16 snark verification library in Go

**Ecosystem**

- [ETHLondon winners](https://twitter.com/ETHGlobal/status/1234132358657380352). All [ETHLondon submissions](https://ethlondon.devpost.com/submissions).
- All the [EthDenver submissions](https://medium.com/ethdenver/all-of-the-ethdenver-2020-project-submissions-a29124035332)
- Taylor Monahan’s [DeFi and Risk essay](https://medium.com/mycrypto/risky-business-defi-and-ethereums-coming-of-age-story-4d99465ad102)
- [Flash attacks will be the new normal](https://medium.com/dragonfly-research/flash-loans-why-flash-attacks-will-be-the-new-normal-5144e23ac75a)
- [Check by address all of your token approvals](https://tokensaver.xyz/index.html)

**Enterprise**

- Hyperledger [Besu v1.4](https://media.consensys.net/hyperledger-besu-1-4-is-now-available-528e18e7e5d9) - better tx signing, better APIs, better sync

**Governance, DAOs, and standards**

- [ERC2537](https://github.com/ethereum/EIPs/blob/ca5ac71b8fd3ab5fb41e9322381e044b490bbc3e/EIPS/eip-2537.md): BLS12-381 curve operations
- [ERC2539](https://github.com/ethereum/EIPs/blob/41dea96153774201ec403169cf2b25d6794ebe17/EIPS/eip-2539.md): BLS12-377 curve operations
- [ERC2542](https://github.com/ethereum/EIPs/blob/39461da12c50e5efac88bed0c8d3e81233efdb8b/EIPS/eip-2542.md) add TXGASLIMIT, CALLGASLIMIT, TXGASREFUND opcodes
- [ERC2541](https://github.com/ethereum/EIPs/blob/9c30e6d28860ac2cee1e0955f2b47c6fb2b6626b/EIPS/eip-2541.md): EY SW6-Bis curve operations
- [ERC2535](https://github.com/ethereum/EIPs/issues/2535): Diamond standard for upgradeable contracts
- [ERC2547](https://github.com/ethereum/EIPs/blob/2587c1461a2f7bc2aa917b893fa896956a6f97c1/EIPS/eip-2547.md): composable multiclass token
- [EIP2544](https://ethereum-magicians.org/t/eip-2544-ens-wildcard-resolution/4061): ENS Wildcard resolution
- [EIP2538](https://github.com/MidnightOnMars/EIPs/blob/master/EIPS/eip-2538.md): Anti-ProgPoW statement from community members
- It seems that when the DAG hits [4GB that a decent amount of hashpower will be knocked offline](https://www.reddit.com/r/ethereum/comments/f973yr/this_is_why_the_majority_of_the_e3_asics_will/), both ASIC and GPU
- [Compound announces a governance token](https://medium.com/compound-finance/compound-governance-5531f524cf68) (with delegated voting!) to control all parts of the protocol. I bet this will be widely emulated.

**Application layer**

- A [postmortem on the iearn.finance trades](https://medium.com/@andre_54855/post-mortem-28-02-2020-6d675a85a33b) that had tongues wagging this week
- [Zora](https://www.ourzora.com/introducing-zora): a marketplace for Unisocks-style sales, from Saint Frame
- [Nori](https://medium.com/nori-carbon-removal/how-to-save-the-planet-and-make-climate-change-just-go-away-using-blockchain-and-cryptocurrency-f6e33917089d): a marketplace for carbon removal, and how it fixes the problems with carbon offsets
- If you didn’t play Ethernal’s multi-user dungeon alpha release, [here’s how it went](https://medium.com/@EthernalWorld/ethernal-alpha-1-0-update-a2b7dcade4e3)
- [Melon Terminal v2](https://medium.com/melonprotocol/introducing-the-melon-terminal-a81a9c5e766e), a new frontend for Melon to go with [Melon v1.1](https://medium.com/melonprotocol/melon-protocol-upgrade-to-v1-1-0-9e72499dd2f0) adding assets and Uniswap/0x v3
- [Creepts](https://medium.com/cartesi/cartesi-creepts-tower-defense-dapp-testnet-launches-6be22ff4503d), a tower defense tournament on Rinkeby testnet
- Due to sponsors, [PoolTogether is higher EV](https://bankless.substack.com/p/prize-savings-the-ultimate-money) than just holding cDai/cUSDC. Much higher variance of course.
- PoolTogether tickets are now tokenized, here’s [how to get a free one](https://twitter.com/PoolTogether_/status/1233103891849498628)

**Tokens/Business/Regulation**

- [What the Internet did to data, Ethereum will do to finance](https://medium.com/@davidschwartz_34333/2020s-the-rise-of-ethereum-a01a19f806d8)
- [SEC charges Steven Seagal](https://www.sec.gov/news/press-release/2020-42) with touting unregistered securities offering
- A winery is selling [tokenized wine on OpenSea](https://www.wiv.io/wiv-technology-and-opensea-bring-finewine-trading-to-a-new-generation/). It’s [live now](https://twitter.com/wivteam/status/1233060076488941568). If you want to support this newsletter, here’s a [referral link to buy fancy French wine](https://opensea.io/assets/0x1e1b3525388e8a63988f8455638aee87f68eeaa7/17?ref=0xe65764f2fd5696fa49498f359b1815aa9b8f9ed4).

**General**

- [Geokeys](https://github.com/oscar-davids/geokeytool/blob/master/README.md): key recovery system through location and password
- It [appears that Huobi/Binance powered up their customers’ STEEM](https://twitter.com/meeseeking/status/1234565130270248960) in order to participate in a TRON attack on the Steem chain. DPOS in action.
- ApexE3 launches a beta of [advanced tools for retail crypto traders](http://beta.apexe3.com/)
- [MACI anonymization using rerandomizable encryption](https://ethresear.ch/t/maci-anonymization-using-rerandomizable-encryption/7054)
- A [sketch for a STARK-based VM](https://ethresear.ch/t/a-sketch-for-a-stark-based-vm/7048)
- [STARK for Schnorr sigs verification](https://ethresear.ch/t/zk-stark-for-schnorr-signature-verification/7034)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Mar 3-5 - [EthCC](https://ethcc.io/) (Paris)
- Mar 14 - [Augur v1 cutoff](https://github.com/AugurProject/augur-app/releases/taghttps://github.com/AugurProject/augur-app/releases/tag/v1.16.10/v1.16.9)
- Mar 29-Apr4 - [EthLagos](https://ethlagos.io/)
- **Apr 3-6 - [NonCon](https://noncon.org/) (Vienna)**
- Apr 13 - Deadline to apply for [50k euro for blockchain startup](https://blockchers.eu/open-calls/)s in Europe
- Apr 24-26 - [EthTurin](https://ethturin.com/)
- Apr 29-30 - [SoliditySummit](https://solidity-summit.ethereum.org/) (Berlin)
- **May 7 - [SmartCon0](https://blog.chain.link/announcing-the-smart-contract-summit-smartcon-0-powered-by-chainlink/) (NYC)**
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

Issue permalink: [https://weekinethereumnews.com/week-in-ethereum-news-march-2-2020/](https://weekinethereumnews.com/week-in-ethereum-news-march-2-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

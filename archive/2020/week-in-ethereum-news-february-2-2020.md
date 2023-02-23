---
title: "Week in Ethereum News<BR> February 2, 2020"
date: "2020-02-02"
---

## **Eth News and Links**

**Eth1**

- [Stateless Ethereum](https://blog.ethereum.org/2020/01/28/eth1x-files-the-stateless-ethereum-tech-tree/): how all the research pieces fit together
- Parity [v2.7.1](https://github.com/paritytech/parity-ethereum/releases/tag/v2.7.1) - no more dual-track releases, breaking database changes
- Nethermind [v1.5.8](https://github.com/NethermindEth/nethermind/releases/tag/1.5.8) - Nethermind is constantly releasing improvements

**Eth2**

- [Lighthouse client update](https://lighthouse.sigmaprime.io/update-21.html). Big block processing and sync speedups. fork choice algo optimized for CPU cycles
- [Prysmatic client update](https://medium.com/prysmatic-labs/eth-2-0-dev-update-42-rapid-iteration-7abdd62109e3). 10x sync speedup. Plus a [script for faster setup of Prysmatic testnet](https://www.youtube.com/watch?v=7qqYHaN2CcY)
- Notes from latest [Eth2 networking call](https://hackmd.io/@benjaminion/HJTHyWyf8)
- [Gossipsub benchmarks](https://whiteblock.io/testing-gossipsub-with-genesis/) from Whiteblock
- [Stateless EEs and delayed block inclusion](https://ethresear.ch/t/stateless-ees-and-delayed-block-inclusion/6839)

**Stuff for developers**

- Solidity [v0.6.2](https://github.com/ethereum/solidity/releases/tag/v0.6.2) - CREATE2, interfaces inherit from inheritances
- [Try/catch in Solidity v0.6.x](https://blog.ethereum.org/2020/01/29/solidity-0.6-try-catch/)
- Embark [v5.1](https://blog.embarklabs.io/news/2020/01/28/embark-5-1/) - new libraries/interfaces config settings, getEVMversion for conditional tests, and a Nethermind plugin
- Subspace [v1.2](https://blog.embarklabs.io/news/2020/01/29/subspace-1-2/) - event/state tracking in React. adds httpProvider support
- [PleaseRelayMe](https://medium.com/blockrocket/pleaserelayme-truly-free-meta-transactions-for-dapps-and-users-5b0f0f1753eb) - allows dapps to use rDai to fund a metatransaction relay hub. live on Kovan testnet
- Results of MetaMask’s [generalized metatransaction standard hackathon](https://medium.com/metamask/our-metatransaction-hackathon-winner-a620551ccb9b)
- [Zinc](https://medium.com/matter-labs/release-of-zinc-v0-1-8d949aa9a2f2): Rust-like language for zero knowlege proof circuits from Matter Labs
- Add [editable user profiles](https://medium.com/coinmonks/add-editable-ipfs-based-user-profiles-to-your-dapp-in-less-than-30-mins-abae8c9a05e6) with 3Box to your app in under 30 minutes
- Using the [web3J Solidity debugger](https://medium.com/web3labs/debugging-solidity-smart-contracts-b641dee46428)
- An [intro to symbolic execution](https://forum.openzeppelin.com/t/symbolic-execution/2158)
- Using MythX’s [symbolic analysis and fuzzing in Remix](https://medium.com/coinmonks/advanced-smart-contract-security-verification-in-remix-9630b43695e5)
- Q&A with [Sam Sun on how he finds vulnerabilities](https://diligence.consensys.net/blog/2020/01/interview-with-samczsun/)
- [Frontend security best practices](https://blog.embarklabs.io/news/2020/01/30/dapp-frontend-security/)
- Integrating [MythX and CircleCI](https://blog.mythx.io/howto/mythx-and-continuous-integration-part-1-circleci/)
- Start to finish [OpenZeppelin CLI workflow](https://forum.openzeppelin.com/t/guide-full-start-to-finish-openzeppelin-workflow-for-cli-deployment-and-upgrades/2191)
- Kauri links for [learning Eth app development](https://kauri.io/tips-for-starting-dapp-development/a6f8cae18e574e1595bd870010100c80/a)
- [Node-gyp-cache](https://github.com/frangio/node-gyp-cache) - cache native dependencies
- web3connect [v1.0.0-beta.29](https://github.com/web3connect/web3connect/releases/tag/1.0.0-beta.29) - cache user’s last provider for auto-load
- New [EthersJS version](https://twitter.com/ethersproject/status/1222753027888685061) with updated ENS registry address
- web3JS [v1.2.6](https://github.com/ethereum/web3.js/releases/tag/v1.2.6) updated ENS registry address and [revert reason strings](https://www.soliditydeveloper.com/web3-1-2-5-revert-reason-strings/)

**Ecosystem**

- Aztec launches [private transactions](https://medium.com/@tompocock/launching-aztec-c9fb271605d7) with hidden amounts. It’s live on mainnet with an SDK.
- [Tornado.cash’s UI had a vulnerability](https://medium.com/@tornado.cash/tornado-cash-vulnerability-alert-787e0552f950). Check to see if you’re affected.
- A [history of Plasma](https://medium.com/dragonfly-research/the-life-and-death-of-plasma-b72c6a59c5ad) and how it morphed into rollup
- ENS [Registry contract is migrating to a new address](https://medium.com/the-ethereum-name-service/ens-registry-migration-bug-fix-new-features-64379193a5a) on Feb 3-5 due to a potential vulnerability found by Sam Sun.

**Enterprise**

- Faster [enterprise blockchain apps](https://pegasys.tech/how-your-enterprise-can-build-production-grade-blockchain-applications-with-ease-using-pegasys-orchestrate/) with PegaSys Orchestrate
- EEA Mainnet Working Group forms Task Force [“EMINENT” (Ethereum Mainnet Integration for Enterprises](https://entethalliance.org/eea-mainnet-working-group-forms-task-force-eminent-ethereum-mainnet-integration-for-enterprises/))

**Governance and standards**

- [ERC2494](https://github.com/ethereum/EIPs/blob/41569d75e42da2046cb18fdca79609e18968af47/eip-draft_babyjubjub.md): BabyJubjub
- [ERC2502](https://github.com/ethereum/EIPs/blob/1aad6b032a1916648f0c11491a8dbda2404ebb95/EIPS/eip-2502.md): µTopic Delegation

**Application layer**

- [0x API aggregates liquidity](https://blog.0xproject.com/access-all-dex-liquidity-through-0x-api-d5dd9a45af31) from 0xMesh, Kyber, Uniswap, Oasis, etc
- [Stablecoin.services](https://stablecoin.services/) - gas-free DAI/CHAI transfers, Uniswap trades, and DAI/CHAI conversion
- [Dai Stability Fee at 8%, and DSR at 7.75%](https://twitter.com/MakerDAO/status/1221546505888157696). The first [auction of surplus DAI](https://twitter.com/nanexcool/status/1223795452790943744) was last night. Keep track of [MCD Auctions](https://daiauctions.com/).
- [Negative votes in quadratic funding](https://ethresear.ch/t/negative-votes-in-quadratic-funding/6855). An idea in Vitalik’s [response](https://vitalik.ca/general/2020/01/28/round4.html) to [Gitcoin grants round 4](https://gitcoin.co/blog/gitcoin-grants-round-4/)
- [Switzerland approves IPO/equity shares](https://pressat.co.uk/releases/switzerland-approves-the-first-articles-of-incorporation-natively-on-the-blockchain-4137e244dfd0f277a94bab09a41e2449/) on Ethereum
- Mashable on DeFi: “[I took out a loan with cryptocurrency and didn’t sign a thing](https://mashable.com/article/defi-guide-ethereum-decentralized-finance/)”
- PoolTogether [hit 1 million DAI](https://twitter.com/spencernoon/status/1223060411232079872) for the first time

**Tokens/Business/Regulation**

- [Ethereum is eating Bitcoin’s payments use case](https://medium.com/@safetythird/ethereum-is-killing-bitcoin-payments-d51d6ea72a12)
- Reuben Bramanathan: [what I learned tokenizing myself](https://medium.com/@bramanathan/what-i-learned-from-tokenizing-myself-bb222da07906)
- How to [make money on digital art](https://bankless.substack.com/p/how-to-make-money-on-digital-art)
- [Thin Applications](https://www.placeholder.vc/blog/2020/1/30/thin-applications) from Joel Monegro

**General**

- Boneh, Drake, Fisch, Gabizon: [Efficient polynomial commitment schemes](https://eprint.iacr.org/2020/081) for multiple points and polynomials
- Kraken [cracks Trezor with 15 minutes](https://blog.kraken.com/post/3662/kraken-identifies-critical-flaw-in-trezor-hardware-wallets/) of physical access. Hardware wallets are susceptible to an attacker having physical access.
- [CacheOut attack](https://cacheoutattack.com/): Intel CPUs leaking data, including SGX
- A satirical guide to [becoming a crypto thought leader on Twitter](https://medium.com/coinmonks/how-to-become-a-cryptocurrency-thought-leader-on-twitter-f10ac1c26488)
- [Blockchain and Cryptocurrency for Noobs](https://blog.makerdao.com/the-benefits-of-cryptocurrency-and-blockchain-technology/), part 1 of a 6 part series from Maker

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Feb 8 - [Augur v1 cutoff](https://twitter.com/AugurProject/status/1214545983205494784)
- Feb 14-16 - [ETHDenver](https://www.ethdenver.com/)
- Feb 20 - [Decentraland launch](https://decentraland.org/blog/announcements/decentraland-announces-publich-launch/)
- Feb 28-Mar 1 - [ETHLondon UK](https://ethlondon.com/)
- Mar 3-5 - [EthCC](https://ethcc.io/) (Paris)
- **Mar 6-8 - [EthParis2020](https://www.hackparis.io/)**
- Mar 29-Apr4 - [EthLagos](https://ethlagos.io/)
- Apr 3-7 - [Edcon](https://www.edcon.io/) (Vienna)
- **Apr 13 - Deadline to apply for [50k euro for blockchain startups](https://blockchers.eu/open-calls/) in Europe**
- April 24-26 - [EthTurin](https://ethturin.com/)
- May 8-9 - [Ethereal Summit](https://www.etherealsummit.com/) (NYC)
- May 15 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum News. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

It’s amazing to me how many people email me when every issue has a link at the bottom saying not to email me to get in the newsletter.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **I want your links, because Google needs help: [weekinethereumnews.com](https://weekinethereumnews.com/)**

Archive on the web if you’re linking to it:  [https://weekinethereumnews.com/week-in-ethereum-news-february-2-2020/](https://weekinethereumnews.com/week-in-ethereum-news-february-2-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

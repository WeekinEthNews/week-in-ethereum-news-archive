---
title: "Week in Eth News <BR> October 18, 2020"
date: "2020-10-18"
---

## **Eth News and Links**

**Eth1**

- Latest [geth v1.9.23](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.23), some security bugfixes and disc v5.1
- Beiko’s [1559 update](https://hackmd.io/@timbeiko/1559-updates/https%3A%2F%2Fhackmd.io%2F%40timbeiko%2F1559-update-002) and Vitalik’s [1559 slides](https://vitalik.ca/files/misc_files/EIP_1559_Fee_Structure.pdf); slowly but surely
- Latest [core dev call](https://www.youtube.com/watch?v=LDSTqo0LKUM). Beiko’s [notes](https://twitter.com/TimBeiko/status/1317138984984694784). Discussion of binaries tries, code merkleization, what goes into the next hard fork
- [Getting an EIP in a hard fork](https://medium.com/nethermind-eth/the-life-of-eip-8031e2c079d1) from Tomasz Stańczak
- First draft [binary trie format](https://hackmd.io/uCWOpSrUQaytBgcO0MVkTQ) spec
- First draft of [Eth witness](https://github.com/ethereum/devp2p/blob/eddb347e6ba1781646612d67c4965f578718e0f6/caps/wit.md) spec
- [EVM384 update](https://notes.ethereum.org/@poemm/evm384-update3): miller loop, but not final exponentation

**EIPs/Standards**

- [EIP3041](https://eips.ethereum.org/EIPS/eip-3041): Adds `baseFee` to `eth_getBlockByHash`
- [EIP3044](https://eips.ethereum.org/EIPS/eip-3044): Adds `baseFee` to `eth_getBlockByNumber`
- [EIP3045](https://eips.ethereum.org/EIPS/eip-3045): Adds `baseFee` to `eth_getUncleByBlockHashAndIndex`
- [EIP3046](https://eips.ethereum.org/EIPS/eip-3046): Adds `baseFee` to `eth_getUncleByBlockNumberAndIndex`
- [ERC3000](https://github.com/izqui/EIPs/blob/649e23b5a50c7eb1c7c2a10d4fe98a0b6954c0bb/EIPS/eip-3000.md): Optimistic enactment governance standard

**Proof of Stake launch**

- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_201018); deposit contract any day now, **CLIENT DIVERSITY A MUST FOR EVERYONE WHO DOES NOT HATE MONEY**
- Latest [proof of stake launch call](https://youtu.be/L4Dvlgxku1g) after a successful Zinken testnet launch. Notes from [Ben](https://hackmd.io/@benjaminion/HyGGLCBww)
- Latest [Lighthouse client](https://lighthouse.sigmaprime.io/update-30.html) update, last audits before mainnet
- Prysm’s browser [GUI for stakers](https://medium.com/prysmatic-labs/prysm-eth2-client-web-interface-now-live-feb278f4aa15)
- [eth2 ETL](https://github.com/blockchain-etl/ethereum2-etl)
- [A fee market contract for eth2 shards in eth1](https://ethresear.ch/t/a-fee-market-contract-for-eth2-shards-in-eth1/8124)

**Layer2**

- Arbitrum’s [optimistic rollup](https://medium.com/offchainlabs/arbitrum-rollup-testnet-full-featured-and-open-to-all-da3255b562ea) is live on Kovan testnet. Copy and paste your Solidity code
- [ENS on layer2 update](https://discuss.ens.domains/t/results-of-the-first-ens-layer-2-meeting/256)
- AZTEC’s [zkrollup with 300 private transactions per second](https://medium.com/aztec-protocol/aztec-zkrollup-layer-2-privacy-1978e90ee3b6) by default, live on Ropsten testnet. Mainnet ETA: 2020

* * *

### **This newsletter is made possible thanks to Chainlink!**

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fabc38264-5f66-4ae5-a095-6f550562b7d6_925x285.png)](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fabc38264-5f66-4ae5-a095-6f550562b7d6_925x285.png)

Want to join the team of world-class researchers and engineers building the leading decentralized oracle networks? Chainlink Labs is hiring. [Explore our open roles.](https://www.chainlinklabs.com/careers?utm_source=newsletter&utm_medium=email&utm_campaign=wie)

* * *

**Stuff for developers**

- Nomic Labs [gets rid of node-gyp dependencies](https://medium.com/nomic-labs-blog/turning-a-page-in-ethereum-javascript-history-4ec89136fccc) across the Ethereum ecosystem and replaces with pure JS cryptography primitives
- “[Verify your contracts on Etherscan 100% of the time](https://kndrck.co/posts/verify-contracts-etherscan-100/)” with solc-sjw
- Truffle [v5.1.49](https://github.com/trufflesuite/truffle/releases/tag/v5.1.49), compatible with Node14, new package `abi-utils`
- vyper [v0.2.7](https://vyper.readthedocs.io/en/latest/release-notes.html#v0-2-7), security bugfixes
- More on the nascent [Fe](https://snakecharmers.ethereum.org/fe-a-new-language-for-the-ethereum-ecosystem/), a pythonic language (with some elements from Rust) written in Rust and targeting Yul
- Ethworks on security first process: [test-driven pair programming with Buidler and Waffle](https://medium.com/ethworks/pragmatic-smart-contracting-tdd-pairing-waffle-buidler-335e42c8762d)
- Kendrick Tan’s [opinions on devtools](https://kndrck.co/posts/building-on-ethereum-mainnet-an-opinionated-guide) for devs new to the space
- Why OpenZeppelin [Upgrades Plugins](https://forum.openzeppelin.com/t/building-for-interoperability-why-we-re-focusing-on-upgrades-plugins/4088)? To make running upgrades in production easier for devs
- [Cheaper gas upgradable proxy](https://forum.openzeppelin.com/t/a-more-gas-efficient-upgradeable-proxy-by-not-using-storage/4111) without using storage
- Paul Berg’s off the shelf Solidity [contracts library](https://twitter.com/PaulRBerg/status/1315794604755738626)
- Andre Cronje’s [liquidity delegated governance](https://andrecronje.medium.com/one-click-governance-tokens-with-liquidity-timelock-and-stop-loss-b906d801f90b) boilerplate
- Certora’s writeup of a [corrupted storage bug in Solidity](https://www.certora.com/blog/corruptedStorage.html)
- A gotcha in forking [SushiSwap if you don’t have governance](https://medium.com/@DraculaProtocol/sushiswap-smart-contract-bug-and-quality-of-audits-in-community-f50ee0545bc6)
- Updating [contract data in Unity](https://medium.com/coinmonks/updating-smart-contract-data-in-unity-419473bafb03)
- [Resend a transaction](https://www.quiknode.io/guides/web3-sdks/how-to-re-send-a-transaction-with-higher-gas-price-using-ethers-js) bumping gas price using ethersjs
- A guide to [erc20 permit](https://soliditydeveloper.com/erc20-permit)
- Nifty.ink’s tutorial on [building with TheGraph](https://azfuller20.medium.com/nifty-notes-building-with-thegraph-a39048e2f0bd)

**Ecosystem**

- [Embrace and cultivate Ethereum’s dark forest](https://medium.com/@trenton.v/ethereums-dark-forest-is-worth-cultivating-3cffa440aa4f)
- [Be careful of brainwallets](https://blog.bitmex.com/call-me-ishmael/). Bitmex hashes some fiction passages and gets insta-sweeped (with dark forest action)

**Enterprise**

- Luxury [watchmaker Breitling adds Eth NFTs](https://medium.com/@marketing_31541/enhance-your-breitling-luxury-watch-experience-with-arianee-1427e540538e) for authenticity and history/repairs tracking
- Stream [private chain events to PostgresSQL](https://medium.com/geora/technical-deep-dive-the-geora-event-sourcing-architecture-27188bc1eb1a)

**Application layer**

- Andre Cronje-mania struck again with a [twist on pool2 design](https://andrecronje.medium.com/crypto-economics-perpetual-liquidity-and-il-offsets-197558347a53): with an LBI token on a bonding curve that people started market buying on Uniswap. [Andre on the aftermath](https://andrecronje.medium.com/unpacking-my-involvement-in-defi-cdb6479e337d): I don’t build for speculators
- Perez, _et al_ paper [analyzing Compound liquidations](https://arxiv.org/pdf/2009.13235.pdf)
- [Numerai Signals](https://medium.com/numerai/building-the-last-hedge-fund-introducing-numerai-signals-12de26dfa69c): becoming the last hedge fund
- [Mia and the marbles](https://medium.com/@miaandthemarbles/what-a-hamster-and-blockchain-have-in-common-3c9e5af8eb7c): hamster-powered marble race betting
- [MakerDAO to cover itself using Nexus Mutual](https://forum.makerdao.com/t/makerdao-protocol-cover-using-nexus-mutual/4761)?
- Synthetix’s [Kwenta is live](https://blog.kwenta.io/kwenta-is-now-live/)
- [CirclesUBI is live](https://twitter.com/CirclesUBI/status/1317089513009762304)

**Regulation/business/tokens**

- [CFTC Chair Tarbert](https://www.coindesk.com/heath-tarbert-invest-eth-fireside): “If Bitcoin is email, a one trick pony but obviously revolutionary…Ethereum goes far beyond that, it's more like the internet.”
- Financial Stability Board’s [stablecoin recommendations for central banks](https://www.fsb.org/2020/10/fsb-publishes-high-level-recommendations-for-regulation-supervision-and-oversight-of-global-stablecoin-arrangements/)
- Paradigm’s [open questions about Uniswap LP strategies](https://www.paradigm.xyz/open-problems/index.html)
- [Linking usage to valuations](https://www.wmougayar.com/blog/2020/10/13/there-is-an-elusive-value-to-usage-linkage-in-crypto-markets-token-valuations)
- [NFTs as Bowie’s “gray space in the middle”](https://www.nichanank.com/blog/2020/10/9/gray-space-in-the-middle) between creators and fans
- web3 as [read-write-own](https://www.himgajria.com/writings/web-3-0)

**General**

- [Quarks](https://eprint.iacr.org/2020/1275.pdf): quadruple-efficient transparent SNARKs
- [The Tally](https://tally.substack.com/p/the-tally-newsletter-issue-1), a newsletter on decentralized app governance
- [OkEx suspends withdrawals](https://www.okex.com/support/hc/en-us/articles/360051090391) amidst rumors that founder has been arrested
- part 2 of Reason’s [cypherpunks](https://www.youtube.com/watch?v=n4qonsvSgAg) video series

* * *

## **Job Listings**

- 0x hiring a [Matcha marketing manager](https://boards.greenhouse.io/0x/jobs/4923909002) and [all flavors of developers](https://0x.org/about/jobs)
- [Dune Analytics](https://careers.duneanalytics.com/): hiring 1st non-founder team members – remote ~CET time zone
- Own Chainlink’s gaming strategy as [VRF Product Manager](https://jobs.lever.co/chainlink/9b67120c-932e-4280-829e-00cff2d78efa)
- Trail of Bits hiring elite [blockchain security engineers](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & [app security](https://jobs.lever.co/trailofbits/8b7f7fc1-efb0-4e89-b406-784c3a2d77e4)
- Celer hiring Solidity and Go devs. Email: hiring@celer.network

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **Wanton self-promotion section**

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow the newsletter on twitter: [@WeekinEthNews](https://twitter.com/WeekInEthNews)

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-eth-news-october-18-2020/](https://weekinethereumnews.com/week-in-eth-news-october-18-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Oct 19-26 - [EthLagos energy hackathon](https://ethlagos.io/)
- **Oct 20 - Golem’s [layer2 event](https://www.eventbrite.com/e/golem-3-layer-2-tickets-124704770325)**
- Oct 20 - [submission deadline for Medalla data challenge](https://ethereum.org/en/eth2/get-involved/medalla-data-challenge/)
- **Oct 21-23 - ACM’s [Advances in Financial Technologies](https://aft.acm.org/)**
- **Oct 23 - ETHOnline’s [Future of Ethereum](https://ethonline.org/future/) summit**
- Oct 29 - [ETHBKK](https://pages.atato.com/ethbkk)
- Oct 31 - [submission deadline for Underhanded Solidity Contest](https://underhanded.soliditylang.org/)
- Nov 6-7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)
- Nov 16 - [MetaMask Provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7)
- **Nov 19 - [Talk Show - EthBerlin 2.5](https://medium.com/ethberlin/move-over-netflix-theres-a-new-zoom-talk-show-in-town-db48c75d35af)**
- Dec 3 - [Ethereum in the Enterprise - Asia Pacific](https://twitter.com/EntEthAlliance/status/1314652848655872000)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

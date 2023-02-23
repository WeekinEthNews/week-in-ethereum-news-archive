---
title: "Week in Ethereum News<BR> March 15, 2020"
date: "2020-03-15"
---

## **Eth News and Links**

**Eth1**

- [Overlay method for hex to binary tree conversion](https://ethresear.ch/t/overlay-method-for-hex-bin-tree-conversion/7104)
- A summary of the post-EthCC [Stateless Eth meetings](https://blog.ethereum.org/2020/03/12/eth1x-files-stateless-summit-summary/). Renewed focus on sync, particularly getNodeData

**Eth2**

- Latest [Eth2 call](https://www.youtube.com/watch?v=orVYfqP_YuQ). Notes from [Ben](https://hackmd.io/@benjaminion/BkW_92PrU) and [Mamy](https://gist.github.com/mratsim/b81f488911496e93fbdde16d966468b6). Phase 1 prototyping coming soon
- Latest phase0 spec [v0.11](https://github.com/ethereum/eth2.0-specs/releases/tag/v0.11.0), the target for stable multi-client testnet
- Ben Edgington’s [notes from networking call](https://hackmd.io/@benjaminion/rk2OEQ64L)
- [Nimbus client](https://our.status.im/nimbus-status-update-march-6th/) update - interop this month, discussion around constraints of running eth2 client on mobile devices
- Two phase2 ethresearch posts: [Appraisal of Non-sequential Receipt Cross-shard Transactions](https://ethresear.ch/t/appraisal-of-non-sequential-receipt-cross-shard-transactions/7108) and [Atomic Cross Shard Function Calls using System Events, Live Parameter Checking, & Contract Locking](https://ethresear.ch/t/atomic-cross-shard-function-calls-using-system-events-live-parameter-checking-contract-locking/7114)
- Vitalik’s [Using polynomial commitments to replace state roots](https://ethresear.ch/t/using-polynomial-commitments-to-replace-state-roots/7095), though this is not likely to hit the current roadmap. More context from listening to [Justin Drake and Vitalik Buterin on Zero Knowledge](https://www.zeroknowledge.fm/120)

**Stuff for developers**

- Solidity [v0.6.4](https://github.com/ethereum/solidity/releases/tag/v0.6.4)
- A [storage layout for proxy contracts](https://medium.com/1milliondevs/new-storage-layout-for-proxy-contracts-and-diamonds-98d01d0eadb) taking advantage of Solidity v0.6.4
- EthGlobal’s [survey of Eth developers](https://ethglobal.typeform.com/to/RxHlK8)
- [10x smaller Javascript signer/verifier](https://www.reddit.com/r/ethereum/comments/fh18yj/i_just_published_10x_smaller_ethereum/)
- [Interacting with Ethereum using a shell through Incubed](https://blog.slock.it/blockchain-in-a-shell-45b6626dc2c0) ultra-light client
- [Groth16 bellman proof verifier](https://github.com/arnaucube/go-bellman-verifier)
- Templates with [pre-filled contract ABIs, addresses and subgraphs](https://twitter.com/PaulRBerg/status/1237398422380056577) for Aave, Compound, Sablier, Uniswap
- Prysmatic’s [service registry pattern in Go](https://rauljordan.com/2020/03/10/building-a-service-registry-in-go.html)
- Implementing [Merkle Trees and Patricia Tries in Node.js](https://medium.com/coinmonks/implementing-merkle-tree-and-patricia-trie-b8badd6d9591)
- Pipline [onchain interpreted language](https://www.youtube.com/watch?v=nZ8XFbCQqX0&feature=emb_title) vid
- Austin Griffith vid on [wallet module for eth.build](https://www.youtube.com/watch?v=E2cU3bpa0F0&feature=youtu.be)
- OpenZeppelin points out that a [malicious deployer can backdoor your Gnosis Safe](https://blog.openzeppelin.com/backdooring-gnosis-safe-multisig-wallets/)
- [SmartBugs](https://joaoff.com/2020/03/05/smartbugs-an-execution-framework-for-automated-analysis-of-smart-contracts/): framework for executing Solidity automated analysis tools, with an academic paper comparing tool performance

**Crypto carnage, Maker liquidations**

- Thursday’s global selloff of risk assets led to the most negative price action day of crypto’s short history. The selloff inflated gas prices (~200 gwei) which caused trouble for Maker. The Maker oracles stopped working for an hour or two.
- Maker liquidation auctions went off for nearly 0 DAI as bots bidding on those auctions got caught in high gas prices and ran out of DAI, leading several different bot maintainers to make ~8m USD in ETH by bidding just above zero in a few disparate time periods.
- As a result, the Maker system surplus became a 5.7m Dai deficit (as of the time of publication). To improve incentives, Maker [governance changed some parameters](https://blog.makerdao.com/recent-market-activity-and-next-steps/) and to recoup the debt [MKR will be auctioned onchain](https://blog.makerdao.com/mkr-debt-auction-announcement-and-details/) for lots of 50,000 Dai on the morning (UTC) of March 19th.
- Community members have started a [backstop to ensure the deficit is covered](https://www.reddit.com/r/ethfinance/comments/fi7pja/join_the_dai_backstop_syndicate_in_signalling/)
- Here is a [writeup of the Maker liquidations](https://medium.com/@whiterabbit_hq/black-thursday-for-makerdao-8-32-million-was-liquidated-for-0-dai-36b83cac56b6) with data and graphs
- Just published: [Maker governance proposal](https://forum.makerdao.com/t/proposal-for-immediate-changes-and-executive-vote/1545) to change DSR to 0 and Stability Fee to 0.5%, GSM to 4 hours, and a decentralized circuitbreaker for auctions

**Ecosystem**

- Prysmatic’s Raul Jordan: [Eth2 is happening, it is shipping, and we’re going to make it a reality no matter what](https://medium.com/@rauljordan/on-the-brink-84e365dd1a25)
- [EthIndia’s online hackathon winners](https://devfolio.co/blog/announcing-winners-of-ethindia-online-hackathon/)
- DuneAnalytic’s [stats for smart contract wallets](https://twitter.com/tschubotz/status/1236235928399745024)
- 4GB [DAG size and potential hashrate impact](https://medium.com/@eric.conner/ethereum-dag-size-and-hash-rate-impact-cda7a54d59db)
- So far, [9 attendees of EthCC have tested positive](https://twitter.com/drakefjustin/status/1238721126387331079) for COVID-19

**Enterprise**

- [End to end transport layer security](https://pegasys.tech/end-to-end-transport-layer-security-on-hyperledger-besu-1-4/) with Hyperledger Besu v1.4
- [DAML now available on Besu](https://www.ledgerinsights.com/daml-smart-contract-hyperledger-besu/)
- [Paul Brody talks Baseline Protocol](https://podcast.ethhub.io/paul-brody-bringing-ethereum-to-enterprise) on Into the Ether
- How [Citi and ConsenSys use Ethereum for commodities trade finance](https://consensys.net/blog/enterprise-blockchain/how-citi-and-consensys-are-using-blockchain-technology-to-help-modernize-the-commodity-trading-market/)

**Governance, DAOs, and standards**

- Livepeer’s [proposed governance roadmap](https://medium.com/livepeer-blog/livepeer-governance-roadmap-proposal-69a6e9e33f80)
- [SingularDTV announces snglsDAO Foundation](https://www.prnewswire.com/news-releases/singulardtv-launches-snglsdao-foundation-to-govern-blockchain-powered-entertainment-industry-on-ethereum-301019969.html) for their media protocol press release
- Aragon [removes AGP voting for ANT holders](https://twitter.com/AragonProject/status/1238505001288380418)
- What [DAOs can learn from the Swedish Pirate Party](https://medium.com/@goldfarbas/how-to-buidl-a-movement-what-the-swedish-pirate-party-teaches-us-about-scaling-daos-805a9d4f7024)
- How to [quickly create your own DAOstack DAO](https://medium.com/@ingamar/how-to-create-run-your-own-dao-5e3eadd96962)
- [FakerDAO](https://www.scopelift.co/blog/fakerdao) - pool your MKR to sell votes to highest bidder

**Application layer**

- Numerai’s [ErasureBay](https://erasurebay.org/) live on mainnet. A marketplace for any kind of information, where the buyer can slash the seller if they don’t like the information
- DeFiSaver’s [1click transaction CDP closing using flashloans](https://medium.com/defi-saver/introducing-1-transaction-cdp-closing-powered-by-flash-loans-8a83456226f4)
- Gnosis’ Gibraltar-regulated [Sight political markets are live](https://blog.gnosis.pm/foresight-is-2020-b1dec3c72f9a)
- Update on [Augur v2](https://twitter.com/AugurProject/status/1238525901953880064). tldr: it’s close
- [Balancer’s code is open source](https://medium.com/balancer-protocol/balancer-contracts-are-open-sourced-33bde904f38f)
- bZx’s [mea culpa](https://bzx.network/blog/mea-culpa) post mortem of the attacks. They also paid 1inch the full bug bounty two weeks ago.
- [Bluestone](https://www.reddit.com/r/ethereum/comments/fgi66s/bluestone_when_pooltogether_meets_compound_a_defi/) fixed rate loans and deposits, live on Rinkeby testnet
- Maker’s [Dai Gaming Initiative](https://blog.makerdao.com/dai-gaming-initiative/)
- VirtuePoker’s [final beta launches March 16th](https://medium.com/@VirtuePoker/beta-2-5-launches-march-16-bd80d96d9085)
- [HavenSocial](https://www.reddit.com/r/ethereum/comments/fgjrg4/im_building_an_encrypted_social_platform_with_no/), a web3 alternative to Facebook where you own your own data

**Tokens/Business/Regulation**

- David Hoffman: [Ethereum as emergent structure](https://bankless.substack.com/p/ethereum-is-an-emergent-structure)
- USDC: [programmable dollars](https://blog.circle.com/2020/03/10/programmable-dollars-for-your-internet-business/) with business accounts and APIs
- [Uniswap volume](https://twitter.com/UniswapExchange/status/1237424559134998528) is now tracked on Coinmarketcap
- [wBTC passes Lightning Network](https://twitter.com/defipulse/status/1237519206700036096) in value locked up
- Matthew Green: [US congressional bill EARN IT is a direct attack on e2e encryption](https://blog.cryptographyengineering.com/2020/03/06/earn-it-is-an-attack-on-encryption/)

**General**

- Contribute [computing cycles to fight COVID-19](https://twitter.com/JonnyRhea/status/1238643297184251910)
- [Stay private in DeFi with email](https://bankless.substack.com/p/how-to-stay-private-in-defi-with)
- Brave’s nightly release features [random browser fingerprints per session](https://www.zdnet.com/article/brave-to-generate-random-browser-fingerprints-to-preserve-user-privacy/)
- [Load Value Injection](https://lviattack.eu/) attack on Intel SGX
- [Jacobians of hyperelliptic curves](https://asz.ink/2020/03/08/jacobians-of-hyperelliptic-curves/) explainer from Alan Szepieniec

* * *

## **Dates of Note**

Upcoming dates of note _(_new in **bold**_)_**:**

_ETHNYC/SmartCon0 postponed indefinitely, EthBarcelona postponed until June, most events go virtual_

- **Mar 16-30 - Gitcoin’s [Funding the Future](https://hackathons.gitcoin.co/funding-the-future) virtual hackathon**
- **Mar 19 - [MKR auction](https://blog.makerdao.com/mkr-debt-auction-announcement-and-details/)**
- **Mar 23 - [Gitcoin Grants CLR, round 5](https://gitcoin.co/grants/) starts**
- Mar 29-Apr4 - [EthLagos](https://ethlagos.io/)
- Apr 3-6 - [NonCon](https://noncon.org/) (Vienna) - **[now virtual](https://twitter.com/ParallelePolis/status/1237450754761293830)**
- Apr 13 - Deadline to apply for [50k euro for blockchain startup](https://blockchers.eu/open-calls/)s in Europe
- Apr 24-26 - [EthTurin](https://ethturin.com/) - **now virtual**
- Apr 29-30 - [SoliditySummit](https://solidity-summit.ethereum.org/) (Berlin) - **[now virtual](https://twitter.com/ethchris/status/1237833026257764359)**
- May 8-9 - [Ethereal Summit](https://www.etherealsummit.com/) (NYC) - **[now virtual](https://www.etherealsummit.com/news/join-us-for-the-ethereal-virtual-summit-2020)**
- **June 17 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop**

* * *

## **Thank you, ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum News. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

* * *

## **I really want you to link to [weekinethereumnews.com](https://weekinethereumnews.com/)**

Issue permalink: [https://weekinethereumnews.com/week-in-ethereum-news-march-15-2020/](https://weekinethereumnews.com/week-in-ethereum-news-march-15-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

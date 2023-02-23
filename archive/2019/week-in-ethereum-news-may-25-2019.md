---
title: "May 25, 2019"
date: "2019-05-26"
---

## **Ethereum News and Links**

**Layer 1**

- [Eth2.0 implementers call](https://www.youtube.com/watch?v=dw2GmEuLr5k). [Notes](https://gist.github.com/mratsim/81ffa60648e53b1facccf999d088e8eb).
- [Lighthouse](https://lighthouse.sigmaprime.io/update-11.html) eth2 client update - Disc v5 in rust libp2p, SSZ updates, RESTful API instead of JSONRPC
- [Prysmatic Labs](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-27-prysmatic-labs-8b65dbdf9381) eth2 client update - updating to current spec
- Eth2 Javascript client [Lodestar will focus on light client support in the browser](https://medium.com/chainsafe-systems/lodestar-roadmap-updates-87783c517b9f). Yeeth and Lodestar to [work on eth2 components in AssemblyScript](https://medium.com/yeeth/yeeth-updates-3-d2e1f8bb97ef)
- Lots of phase2 execution work coming out of eth2 meetings in New York. To wit:
- Vitalik’s [Eth2, phase2, proposal2](https://notes.ethereum.org/w1Pn2iMmSTqCmVUTGV4T5A?viewPhase#)
- [Eth Execution Environment proposal](https://ethresear.ch/t/eth-execution-environment-proposal/5507)
- [Current idea on eth1->eth2 migration](https://twitter.com/VitalikButerin/status/1132380238997012480): take the Eth1 state root and port into Eth2 execution environment
- [Ewasm Scout](https://ethresear.ch/t/phase-2-execution-prototyping-engine-ewasm-scout/5509), eth2 phase2 execution prototyping engine
- Drake: [Blind VDF and timelock outputs](https://ethresear.ch/t/blinded-vdfs-and-timelocks/5494)

**Client releases**

- [Trinity v0.1.0-alpha.24](https://github.com/ethereum/trinity/releases/tag/v0.1.0-alpha.24)

**Layer 2**

- [Plasma implementer](https://www.youtube.com/watch?v=AWLCmdawWWU) call. [Notes](https://www.notion.so/Plasma-Implementers-Call-2-0-2018-05-22-fae4d4ab1eb740198591273961e21b7f).
- PlasmaLeapDao [streaming payment and royalty distribution demo](https://leapdao.org/blog/Rights-Management-Onchain-Cannes-Film/) on their Plasma chain at Cannes Film Festival
- [Mosendo as a consumer-friendly Venmo-esque frontend](https://medium.com/depfi/ethereum-is-actually-delivering-peer-to-peer-cash-heres-how-447be424f4e2) for Connext’s state channels.
- [Gas Station Network as potential state channel watchtower](https://hackernoon.com/sha-zam-b01cf9c7126a)
- [Celer’s state channels deployed onto Matic](https://medium.com/celer-network/celer-x-matic-towards-an-integrated-future-of-layer-2-scaling-solutions-b497f114add3)’s Plasma MVP chain. More on [Matic Plasma](https://ethresear.ch/t/account-based-plasma-morevp/5480).

**Stuff for developers**

- Vyper [v0.1.0-beta.10](https://github.com/ethereum/vyper/releases/tag/v0.1.0-beta.10)
- Truffle [v5.0.19](https://github.com/trufflesuite/truffle/releases/tag/v5.0.19)
- [Etherlime v2.0](https://github.com/LimeChain/etherlime/releases/tag/etherlime%402.0.0)
- [Right-To-Left-Override as Solidity attack vector](https://skylightcyber.com/2019/05/12/ethereum-smart-contracts-exploitation-using-right-to-left-override-character/). A detection tool added to Slither
- [Provable fair ransom](https://medium.com/consensys-diligence/provable-fair-ransom-1547ba894d0) to profit from otherwise non-exploitable vulnerabilities
- Visual Eth IDE [Pipeline is on Remix-alpha](https://www.reddit.com/r/ethereum/comments/bsu2m2/pipeline_visual_ethereum_ide_brief_guide_now_on/)
- [Intro to AZTEC](https://medium.com/aztec-protocol/an-introduction-to-aztec-47c70e875dc7) for developers
- Loredana’s [PoC for her universal filesystem](https://www.reddit.com/r/ethereum/comments/bq4wgl/universal_os_filesystem_by_consensus_for_ethereum/), dType
- Process Ethereum [data with Pubsub and Dataflow](https://github.com/allenday/ethereum-streaming-analytics-demo)
- Vitalik’s [design for a minimal mixer](https://hackmd.io/s/rJj9hEJTN)

**Ecosystem**

- [Ethereum Foundation Q2 update](https://blog.ethereum.org/2019/05/21/ethereum-foundation-spring-2019-update/) and how it will spend $30m this year
- We should [standardize a p2p network for offchain messages](https://ethereum-magicians.org/t/we-need-to-standardize-a-p2p-network-for-offchain-messages/3298)
- [MetaMask user metrics](https://medium.com/metamask/metamask-metrics-fbec0e2ceaa7). 265k MAUs in April.
- [ETHNewYork submissions](https://ethnewyork.devpost.com/submissions)
- [Where we are with Eth2 testnets](https://www.tokendaily.co/blog/eli5-explanation-of-the-ethereum-2-0-testnet) explainer

**Enterprise**

- [EEA real estate use cases playbook](https://entethalliance.org/real-estate-leaders-unveil-enterprise-ethereum-alliance-blockchain-use-case-playbook/)

**Governance and Standards**

- Latest [core devs](https://www.youtube.com/watch?v=lF_XxqxgVuA) call. Tim Beiko’s [notes in tweetstorm](https://twitter.com/TimBeiko/status/1131929965174415360) form
- Updated [proposed list of possible EIPs](https://github.com/ethereum/EIPs/blob/02904c52f28fa509bdd5d563adc25d346ac33b79/EIPS/eip-1679.md) for Instanbul upgrade fork
- [EIP2045](https://eips.ethereum.org/EIPS/eip-2045): Fractional gas costs for EVM opcodes
- [EIP2046](https://eips.ethereum.org/EIPS/eip-2046): Reduced gas cost for static calls made to precompiles
- [ProgPoW audit has been delayed](https://ethereum-magicians.org/t/progpow-audit-delay-issue/3309), so it is unlikely to make it into the Istanbul hard fork
- [Futarchy appellate Aragon courts](https://blog.aragon.one/futarchy-courts/) using staked ANT

**Live on mainnet**

- [Compound v2 live on mainnet](https://medium.com/compound-finance/compound-v2-is-live-157db0b7cfc8)
- [Nexus Mutual live on mainnet](https://medium.com/nexus-mutual/nexus-mutual-launch-how-our-digital-cooperative-will-work-711822c2931d), a digital cooperative to offer smart contract cover to insure against bugs

**Application layer**

- Set did the [first rebalances](https://medium.com/set-protocol/a-milestone-success-the-first-sets-rebalance-b895de1d88b2) on its automated rebalancing portfolio
- Guide to [DxDAO launch on May 29](https://docs.google.com/document/d/1PIgWibaN1n1UF3oMx-Ca-ebFK8tHmT2JVQbOC_xSQSg/edit).
- Veil’s explanation for [why it forked Augur and created AugurLite](https://medium.com/veil-blog/augurlite-follow-up-59fefaf240c9). They want 2020 US presidential campaign markets now instead of waiting for v2
- Comparison of [Maker, dydx, Compound, and Dharma](https://medium.com/dydxderivatives/decentralized-lending-an-overview-1e00fdc2d3ee) decentralized lending
- [Defi users over time](https://medium.com/alethio/the-defi-series-a-closer-look-into-user-community-356a8d8ba2f5) data viz from Alethio
- [Multi-collateral Dai testnet release](https://blog.makerdao.com/update-the-road-to-multi-collateral-dai-kovan-release-v0-2-6/) v0.26. Also, the Stability Fee is [back up for a vote to lower to 17.5%](https://blog.makerdao.com/executive-vote-stability-fee-17-5-may-24/) (last week I incorrectly assumed the vote would pass. It did not and appears it may fail again this week)
- [VirtuePoker is in private beta](https://www.reddit.com/r/ethereum/comments/bs3zqv/the_virtue_poker_beta_launches_today_play_for/) with a bunch of promotions

**Interviews, Podcasts, Videos, Talks** 

- [Barry Whitehat](https://www.youtube.com/watch?v=maDHYyj30kg) on privacy at Taipei Eth meetup
- [Token Summit videos](https://www.youtube.com/playlist?list=PLuQ-imDgTi5j0nv6vsmi9MCoUZg1eDneQ)
- Ren’s [Loong Wang](https://thebitcoinpodcast.com/hashing-it-out-46/) on Hashing It Out

**Tokens / Business / Regulation**

- Circle on why [SEC Framework is making Poloniex delist](https://blog.circle.com/2019/05/23/our-take-interpreting-recent-signals-from-us-regulatory-agencies/) a bunch of assets for the US
- Fred Wilson: [US regulatory uncertainty keeps crypto projects out of the US](https://twitter.com/fredwilson/status/1132045551594352646)
- [Building the Commons Stack](https://medium.com/giveth/introducing-the-commons-stack-scalable-infrastructure-for-community-collaboration-6886eb97413e) (“infrastructure for collaboration”) from Giveth and BlockScience
- Felix Feng on [Ethereum’s moat](https://twitter.com/felix2feng/status/1130268154742026241)

**General**

- Setty IACR paper: [Efficient SNARKs without trusted setup](https://eprint.iacr.org/2019/550.pdf)
- [Awesome zero knowledge proofs](https://github.com/matter-labs/awesome-zero-knowledge-proofs)
- Mustafa Al-Bassam’s LazyLedger: [data availability blockchain with sub-linear full block validation](https://ethresear.ch/t/a-data-availability-blockchain-with-sub-linear-full-block-validation/5503)
- BBC reports that [Facebook’s stablecoin will be called Globalcoin](https://www.bbc.com/news/business-48383460), and may attempt to peg to a basket of fiat currencies.
- Lots of [cell phone sim card](https://medium.com/coinmonks/the-most-expensive-lesson-of-my-life-details-of-sim-port-hack-35de11517124?sk=4c29b27bacb2eff038ec8fe4d40cd615) porting attacks in the last week. If you give an online service your cell number, your account is insecure

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- May 27-28 - [EthCon Korea](https://ethcon.kr/) (Seoul)
- **May 29 - [DxDAO launches](https://docs.google.com/document/d/1PIgWibaN1n1UF3oMx-Ca-ebFK8tHmT2JVQbOC_xSQSg/edit)**
- **June 5-7 - [Scaling Ethereum](https://twitter.com/ScalingETH/status/1131350847047311362) research workshop (Toronto)**
- June 8-9 - [WASM in blockchains](https://avive.github.io/wasm_on_the_blockchain/#/) (Berlin)
- June 10-11 [Blockchain for Social Impact conference](https://conference.blockchainforsocialimpact.com/) (NYC)
- June 22-24 - [Zcon1](https://www.zfnd.org/zcon/) (Split, Croatia)
- July 3-5 - [WindingTree’s HackTravel](https://windingtree.com/hacktravel-lisbon-2019) (Lisbon)
- July 19 - [BuildETH](https://www.buildeth.io/) (San Francisco)
- Aug 2-4 - [ETHIndia](https://ethindia.co/) (Bangalore)
- Aug 2-4 - [TruffleCon](https://www.truffleframework.com/trufflecon2019) (Redmond)
- Aug 21-23 - [Dappcon](https://dappcon.io/) (Berlin)
- Aug 23-25 - [ETHBerlin](https://ethberlinzwei.com/)
- September 15 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff/)
- Sep 16-17 - [Starkware sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- Oct 8-11 - [DeVcon](https://devcon.org/) (Osaka)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I own Week In Ethereum. Editorial control has always been 100% me. 

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **It’s annoying how many link to the old URL. This is the new one: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: 

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

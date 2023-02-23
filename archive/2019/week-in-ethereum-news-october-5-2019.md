---
title: "Week in Ethereum News <BR> October 5, 2019"
date: "2019-10-05"
---

## **Eth News and Links**

**Eth1**

- Nethermind [v1.1.0](https://github.com/NethermindEth/nethermind/releases/tag/1.1.0). ~50gb database.
- Geth [v1.9.6](https://www.reddit.com/r/ethereum/comments/dcon81/geth_v196_elasa_light_client_fixes_and_huge_disk/) light client improvement sync and the 10x reduction in disk i/o
- Eth tests [v7.0.0-beta.1](https://github.com/ethereum/tests/releases/tag/v7.0.0-beta.1) including Istanbul
- Latest [all core devs call](https://www.youtube.com/watch?v=rPD2EpDDI-0). Pooja’s [notes](https://github.com/ethereum/pm/blob/eca93a683edd7f8384af117d85fb7c23c7e8091b/All%20Core%20Devs%20Meetings/Meeting%2072.md). If you were wondering about the Ropsten Istanbul confusion, it’s because someone started heavily mining Ropsten but did not support the Istanbul fork
- A [proposed CALLWITHSCHEDULE opcode](https://medium.com/@earlz/a-simple-ethereum-proposal-e19efd9c3f72) to guard against reentrancy
- Gas golfing [storage pricing in Istanbul](https://medium.com/@agusx1211/evm-istambul-storage-pricing-5befaac32403). Interesting [debate on Reddit](https://www.reddit.com/r/ethereum/comments/dbxij1/evm_istambul_storage_pricing_or_how_to_hack_the/).

**Eth2**

- [What’s New in Eth2](https://notes.ethereum.org/@ChihChengLiang/Sk8Zs--CQ/Sk8Zs--CQ?type=book), includes Ben’s bullish thoughts on the possibility of phases 1 and 2 also going live in 2020
- Ryuya argues for [FMD GHOST](https://ethresear.ch/t/saving-strategy-and-fmd-ghost/6226)
- The [security calculations](https://ethresear.ch/t/security-level-of-random-sampling-with-sharding/6230?u=benjaminion) of random sampling for committee 
- [Dev experience in Eth2](https://thebitcoinpodcast.com/hio-panels-1/) a podcast with panel of folks from Nimbus, Lighthouse, Prysmatic, EF, and ConsenSys
- [Run a 5 client testnet with this shell](https://github.com/status-im/nim-beacon-chain/tree/interop/multinet)
- [Prysmatic](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-36-prysmatic-labs-3ea492024c4d) client update. restarted testnet, massive BLS improvements.

**Layer 2**

- Counterfactual and Magmo [merging their generalized state channel codebases](https://medium.com/statechannels/state-channels-developer-update-0-counterfactual-and-magmo-are-joining-forces-4acfabf3fc98) under the State Channels name.
- [Hodor](https://medium.com/matter-labs/meet-hodor-matter-labsstark-prover-implementation-c759a6ef4c98), Matter Lab’s open STARK prover implementation
- [Matic beta](https://blog.matic.network/matic-beta-mainnet-is-here/) release includes Plasma predicates

**Stuff for developers**

- Solidity v[0.5.12](https://github.com/ethereum/solidity/releases/tag/v0.5.12). loop support for the SMT solver, Yul optimizer improvements
- [Solidity debugging with stack traces](https://medium.com/nomic-labs-blog/better-solidity-debugging-stack-traces-are-finally-here-dd80a56f92bb) using Buidler EVM
- [ZoKrates as a Remix plugin](https://medium.com/@edi.sinovcic/zokrates-zksnarks-on-ethereum-made-easy-8022300f8ba6)
- 3Box’s [IdentityWallet SDK](https://medium.com/3box/introducing-identitywallet-sdk-4750d6afa519), JavaScript for wallets to natively integrate with 3box
- [Burner Wallet 2](https://medium.com/@dmihal/introducing-the-burner-wallet-2-542604dc8d28): modular components for building burner wallets
- How to [avoid subsidizing bad actors in your Gas Station Network app](https://forum.openzeppelin.com/t/advanced-gsn-gsnbouncersignature-sol/1414)
- [Mexa](https://medium.com/biconomy/mexa-magical-experiences-anytime-anywhere-7a9c0c364221): meta transaction SDK
- Explore your data with [Grid + Geth + GraphQL](https://medium.com/ethereum-grid/exploring-ethereum-with-geth-graphql-and-grid-6df38f2a86c)
- [web3data.js](https://medium.com/amberdata/same-code-no-node-web3datajs-the-easiest-blockchain-library-8df4d96a60e) from Amberdata adds RPC support
- [Hookpad](https://medium.com/hookpad/hookpad-beta-is-here-6e8a63713219): listen to any EVM chain, and filter the events you need
- Samczsun: [taking undercollateralized loans for fun and for profit](https://samczsun.com/taking-undercollateralized-loans-for-fun-and-for-profit/)
- Slither [v0.6.7](https://github.com/crytic/slither/releases/tag/0.6.7) - flattener and auto-generated patches
- Brownie python framework: [evaluating Solidity code coverage via opcode tracing](https://medium.com/coinmonks/brownie-evaluating-solidity-code-coverage-via-opcode-tracing-a7cf5a92d28c)

**Ecosystem**

- Swarm [v0.5](https://www.reddit.com/r/ethswarm/comments/dbqcbv/swarm_v050_is_released/)
- Vac: [p2p data sync with remote log](https://vac.dev/remote-log)
- ENS short name auctions hit a [snag with some OpenSea bugs](https://medium.com/opensea/how-were-resolving-the-issues-with-the-ens-short-name-auctions-93c78158de48). Some stolen names were returned for a bounty. Since auctions were paused, some will be extended. ENS also adds [text records for names](https://medium.com/the-ethereum-name-service/new-text-records-now-available-for-ens-names-in-manager-a0ebb9cda73a).
- Slockit’s [Incubed](https://blog.slock.it/incubed-secure-blockchain-access-for-iot-db4687b3dfa1) stateless client that fits on a microcontroller
- Benchmarking shows [GPU miners will be able to transcode on Livepeer](https://medium.com/livepeer-blog/livepeer-gpu-miner-update-663a3e19de56) without hashrate loss and may even lower their power consumption (!)
- [zkay paper](https://files.sri.inf.ethz.ch/website/papers/ccs19-zkay.pdf) on EthZurich’s new language for data privacy
- Mimblewimble on Ethereum: [Send ERC20 privately using zk-SNARKs](https://ethresear.ch/t/ethereum-9-send-erc20-privately-using-mimblewimble-and-zk-snarks/6217)

**Enterprise**

- Hyperledger [Besu v1.3](https://github.com/hyperledger/besu/releases/tag/1.3.0)
- Built on Besu: [how PegaSys Plus helps enterprises go from PoC to production](https://pegasys.tech/how-pegasys-plus-will-help-enterprises-take-their-blockchain-from-poc-to-production/)
- Quorum [v2.3](https://github.com/jpmorganchase/quorum/releases/tag/v2.3.0)
- [Hyperledger Avalon](https://www.hyperledger.org/blog/2019/10/03/introducing-hyperledger-avalon), the evolution of the EEA’s trusted compute spec
- How to use [POA Network’s arbitrary message bridge](https://forum.poa.network/t/how-to-develop-a-cross-blockchain-application-by-using-amb-bridge/2963)
- Tradeshift and Monerium facilitate a retailer [purchasing goods from Ikea and paying onchain](https://monerium.com/press/20191001-monerium-and-tradeshift/) with Monerium’s licensed e-money.
- [Morningstar looking to offer credit opinions](https://www.forbes.com/sites/michaeldelcastillo/2019/10/01/morningstar-is-building-a-blockchain-bridge-to-the-117-trillion-debt-securities-industry/#22f4024c3612) and ratings on cryptoassets, possibly through an onchain oracle

**Standards and governance topics**

- An overview of [MolochDAO functionality and its progeny](https://medium.com/odyssy/moloch-primer-for-humans-9e6a4f258f78)
- [ERC2304](https://github.com/Arachnid/EIPs/blob/ccb740147775b701bc3f0dbabbac0e785633baa7/EIPS/eip-2304.md): Multichain address resolution for ENS

**Application layer**

- Maker’s [Dai Stability Fee at 10.5%](https://twitter.com/nanexcool/status/1178415837616754693) and under a vote to go to 8.5%
- A tool to help you [find the best Uniwap liquidity pools](https://pools.fyi/#/)
- [Golem v0.21 Brass](https://blog.golemproject.net/brass-golem-beta-0-21-0-hello-mainnet-gwasm/) puts gwasm on mainnet
- UMA paper [BitDEX](https://twitter.com/UMAprotocol/status/1179045704918011906): a decentralized Bitmex
- [Tokenizing ISA contracts using OpenLaw](https://medium.com/@openlawesq/tokenizing-contracts-on-openlaw-and-ethereum-129cfdf5d659)
- [BlitzPredict is live](https://medium.com/@blitzpredict1/beta-release-roadmap-update-8df9b8ac9969) on Kovan testnet
- You can now buy [Set Procotol’s Sets with stablecoins](https://medium.com/set-protocol/introducing-pay-with-stablecoins-60c98a329c5f)
- The [rise and fall of the Fairwin ponzi](https://medium.com/@PhABC/the-collapse-of-fairwins-125m-ponzi-scheme-61a66b273420)
- Brave users can now [withdraw their earned BAT](https://basicattentiontoken.org/brave-partners-with-uphold-to-launch-wallet-that-rewards-users-for-browsing/) by KYCing with Uphold

**Tokens / Business / Regulation**

- [Ether: a new model for money](https://medium.com/@TrustlessState/ether-a-new-model-for-money-17365b5535ba). The article version of David Hoffman’s Ethereal Tel Aviv talk.
- Dether new release: cash for in-person eth to fiat trades. Their token model involves [staking tokens for a zone with Harberger taxes](https://medium.com/@dether/your-new-cash-to-eth-on-off-ramp-releasing-the-new-dether-app-3e9f0c14ce1).
- Exchanges and OTC desks form [Crypto Ratings Council to quantify likelihood](https://blog.coinbase.com/introducing-the-crypto-rating-council-d6ee33a8f34d) of SEC categorizing a token as a security.
- [EOS pays SEC 24m](https://www.sec.gov/news/press-release/2019-202) for raising billions to settle unregistered security case, meanwhile [Sia pays 225k to settle with the SEC](https://sia.tech/settlement2019) for raising 120k five years ago. Sure doesn’t look fair.
- Bipartisan duo in the US House asks the [Federal Reserve if they’re developing a digital dollar](https://www.coindesk.com/us-congressmen-ask-fed-to-consider-developing-national-digital-currency)
- Eli Dourado: [Bitcoin’s 21m cap meme may be put to the test in 2020](https://elidourado.com/blog/bitcoin-fee-market/)

**General**

- September edition of 30 days of [Ethereum ecosystem shipping](https://concourseopen.com/blog/30-days-of-eth-september-2019/)
- Brave’s VPN⁰ [research on a distributed VPN](https://brave.com/vpn0-a-privacy-preserving-distributed-virtual-private-network/)
- [Side-channel attacks against shielded transactions in ZCash](https://crypto.stanford.edu/timings/). Now fixed.
- Paypal [drops out of Facebook’s Libra](https://twitter.com/CNBCnow/status/1180207114385547264)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Oct 5-6 - [Cryptoeconomics System Summit](https://cryptoresearch.pubpub.org/) (Boston)
- Oct 7 - [ENS workshop](https://medium.com/the-ethereum-name-service/ens-workshop-applications-are-now-open-f46db6c63384) (Osaka)
- Oct 8-11 - [Devcon](https://devcon.org/agenda) (Osaka). Link to agenda.  Social events: [OffDevcon](https://www.offdevcon.com/) and [Kickback](http://osaka.kickback.events/events/)
- Oct 19-20 - [Crosslink](https://crosslink.taipei/) (Taipei)
- Oct 26 - [Zero Knowledge Summit](https://www.zeroknowledge.fm/summit) (SF)
- Nov 1 - [Ledger EU](https://ledgerproject.eu/) apply for 200k euro startup funding
- Nov 5-6 - [Decentralized insurance D1Conf](https://blog.etherisc.com/d1conf-2019-to-focus-on-blockchain-adoption-november-5-6th-in-malta-3b8b582ac7b4) (Malta)
- Nov 8-10 - [ETHWaterloo](https://ethwaterloo.com/)
- Jan 1 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff-update/)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

It’s amazing to me how many people email me when every issue has a link at the bottom saying not to email me to get in the newsletter.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **This headline stays as long as so many people continue to link to old URL and not the right one: [weekinethereumnews.com](https://weekinethereumnews.com/)**

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/week-in-ethereum-news-october-5-2019/](https://weekinethereumnews.com/week-in-ethereum-news-october-5-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

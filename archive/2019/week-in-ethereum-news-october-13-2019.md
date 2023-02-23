---
title: "Week in Ethereum News <BR> October 13, 2019"
date: "2019-10-14"
---

## **Eth News and Links**

**Eth2**

- A tactical shift for eth2: [less shards (64?) but faster cross-shard comms](https://notes.ethereum.org/@vbuterin/HkiULaluS) and 8x higher throughput per shard
- [Lighthouse client](https://lighthouse.sigmaprime.io/update-16.html) update - it’s still networking season
- Some excellent [phase0 slides](https://docs.google.com/presentation/d/1MZ-E6TVwomt4rqz-P2Bd_X3DFUW9fWDQkxUP_QJhkyw/edit?pli=1#slide=id.g621e2d5823_0_205) from Devcon
- This was the week that Vitalik decided to write up ideas that you likely already knew if you read this newsletter, but apparently Coindesk reporters do not. To wit:
- The [eth1 to eth2 transition plan](https://ethresear.ch/t/the-eth1-eth2-transition/6265)
- [Formalizing eth2’s approach toward finalization of invalid shard blocks](https://ethresear.ch/t/formalizing-and-improving-eth2s-approach-toward-finalization-of-invalid-shard-blocks/6263)
- [Sharding does not break defi composability](https://ethresear.ch/t/cross-shard-defi-composability/6268). .
- A [design pattern for partially sharding apps](https://ethresear.ch/t/partially-sharding-single-threaded-apps-a-design-pattern/6287).
- [Beacon chain saved contracts](https://ethresear.ch/t/on-beacon-chain-saved-contracts/6295). Expensive, but possible.
- Why a [2way bridge is hard between eth1 and eth2](https://ethresear.ch/t/two-way-bridges-between-eth1-and-eth2/6286), but options for how it can be done

**Layer 2**

- Plasma Group and Uniswap ran an [Optimistic Rollup demo at Devcon](https://decrypt.co/10030/plasma-group-and-uniswap-release-new-ethereum-scaling-solution-at-devcon), which enables hundreds of transactions per second
- Celer releases the [specification of its state channels](https://www.celer.network/docs/celercore/)
- [Cross zk-Rollup transfer protocol](https://ethresear.ch/t/trustless-and-secure-cross-zk-rollup-transfer-protocol/6255/2)

**Stuff for developers**

- Metamask: [web3 plugins](https://medium.com/metamask/introducing-the-next-evolution-of-the-web3-wallet-4abdf801a4ee). Verified scripts loaded over ENS, IPFS, or Swarm. The new “focus \[is\] on implementing APIs that enable second-order innovation, like the APIs above”
- [ZoKrates v0.5](https://github.com/Zokrates/ZoKrates/releases/tag/0.5.0). Structs, arrays, and JSON-ABI
- [OpenZKP](https://blog.0xproject.com/introducing-openzkp-1dea6b22dceb): 0x opensources a STARK implementation in Rust
- [Azure’s latest Eth dev kit](https://cloudblogs.microsoft.com/opensource/2019/10/08/microsoft-azure-blockchain-dev-kit-updates-ethereum-devcon/) for VS code natively supports OpenZeppelin and [Infura](https://blog.infura.io/infura-now-natively-supported-in-the-azure-blockchain-development-kit-for-ethereum-430fb02f1c9b)
- a writeup of [Solidity Visual Auditor](https://diligence.consensys.net/blog/2019/10/solidity-visual-auditor-extension-for-vs-code/) for VS code
- [Checking custom correctness properties](https://medium.com/consensys-diligence/checking-custom-correctness-properties-of-smart-contracts-using-mythx-25cbac5d7852) using MythX
- Kovan testnet [successfully hardforked](https://twitter.com/kovantestnet/status/1183326400784158721) into Istanbul
- [Source code of the Eveem](https://github.com/eveem-org/panoramix) decompiler
- Phil Daian’s [Complete Knowledge proofs](https://twitter.com/phildaian/status/1181822995993681921) to fight bribery
- [Mutant testing tool](https://medium.com/swlh/introduction-into-mutation-testing-d6512dc702b0) to find out how good your test suite really is
- Lexon demo of [natural language Eth code](http://demo.lexon.tech/apps/editor/)
- [Live Eth data with BigQuery and Pub/sub](https://medium.com/google-cloud/live-ethereum-and-bitcoin-data-in-google-bigquery-and-pub-sub-765b71cd57b5). How to [query ENS and Ox events](https://medium.com/@medvedev1088/query-ens-and-0x-events-with-sql-in-google-bigquery-4d197206e644)
- [Subspace](https://subspace.status.im/) event tracking and autosyncing. Saves state to local db so app syncs from the last known point
- [Remix IDE on desktop](https://medium.com/remix-ide/remix-desktop-8c1e9e946ee1)

**Ecosystem**

- Live [video feeds from Devcon](https://slideslive.com/ethereum). You’ll likely need the [agenda](https://devcon.org/agenda) to find the talks you want to see.
- [EthDNS](https://medium.com/the-ethereum-name-service/ethdns-9d56298fa38a): ENS + IPFS everywhere and its DNS over https service
- Unstoppable Domains [built its .crypto domains on ETH](https://medium.com/unstoppabledomain/crypto-ac3eec150768)
- [Ethereum on ARM](https://www.reddit.com/r/ethereum/comments/dehcq9/ethereum_on_arm_nanopct4_rockpro64_and_raspberry/). New images for NanoPC-T4, Rockpro64 & Raspberry Pi. Run a full node with Geth/Parity/Trinity. Plus: Status.im, Raiden, IPFS, Swarm and Vipnode. Or an eth2 testnet with Prysmatic.
- Kobi Gurkan found a bug in the snark implementation of the MIMC hash function in circomlib. Thus, [Tornado.cash had to hack itself](https://medium.com/@tornado.cash.mixer/tornado-cash-got-hacked-by-us-b1e012a3c9a8), but everything is fine. They migrated everything to a new contract and updated the UI. Privacy was never lost.

**Enterprise**

- An interview with [EY’s Paul Brody about Nightfall](https://decrypt.co/10241/inside-eys-radical-plan-to-get-major-businesses-using-ethereum)
- EEA’s updated [client spec and trusted compute spec](https://entethalliance.org/enterprise-ethereum-alliance-unveils-token-enabled-blockchain-in-action-at-devcon-5/), plus trusted reward tokens for consortia
- EU Blockchain Observatory [legal and regulatory report](https://www.eublockchainforum.eu/sites/default/files/reports/report_legal_v1.0.pdf?width=1024&height=800&iframe=true)
- [Fatburger to use Cadence for a $30m bond](https://www.forbes.com/sites/benjaminpirus/2019/10/09/fatburger-and-others-feed-30-million-into-ethereum-for-new-bond-offering/#1f647b2e115b) offering with the tokens issued on Ethereum mainnet

**Standards and governance topics**

- Interesting Decrypt report on [Orochi, a Moloch fork, solving coordination problems](https://decrypt.co/10286/orochi-the-mysterious-dao-powering-events-at-devcon-5) in event planning

**Application layer**

- Multi-collateral Dai scheduled to [launch on November 18th](https://blog.makerdao.com/breaking-launch-date-of-multi-collateral-dai-announced-at-devcon-5/)
- [Compound’s plans for MCD](https://medium.com/compound-finance/support-for-multi-collateral-dai-c8691d0ef794). Users are responsible for migrating their Dai.
- Compound is moving all their [administrative functions to a 2 day time delay](https://twitter.com/compoundfinance/status/1183111626607738892)
- [Crop insurance product in Keny](https://www.reddit.com/r/ethereum/comments/dg0zmb/sprout_climate_insurance_powered_by_etherisc/)a for farmers using the Etherisc protocol. Going live next year.
- SetProtocol’s [Rebalancing Dashboard](https://medium.com/set-protocol/introducing-the-rebalancing-dashboard-9130e31435d9) so you can participate in rebalancing events
- [Vulcan Swap](https://www.reddit.com/r/ethfinance/comments/ddlbqx/just_found_vulcan_swap_a_decentralized_dca_order/) - decentralized dollar cost averaging, live on Rinkeby testnet
- Alethio’s [DeFi/dex data viz](https://twitter.com/AlethioEthstats/status/1181055545987366912) for the week before devcon
- Brave is at [8 million monthly active users](https://twitter.com/BrendanEich/status/1181370032032321536)
- Augur will ship [v2 in q1 with Dai integration and cheap order creation in 0x](https://www.augur.net/blog/v2-and-beyond/), as well as both trading and betting UIs
- the Sacramento Kings [NBA franchise launching a tokenized blockchain reward program](https://www.nba.com/kings/news/sacramento-kings-and-blockparty-launch-nbas-first-blockchain-driven-token-power-predictive) for predicting things in their game

**Tokens / Business / Regulation**

- “It is my view as Chairman of the CFTC that [ether is a commodity](https://www.cftc.gov/PressRoom/PressReleases/8051-19)”
- SEC gets an [injunction to stop the Telegram sale](https://www.sec.gov/news/press-release/2019-212), and also seeks to make Telegram give all ~$2b back
- [Stripe, ebay, Visa, and Mastercard](https://decrypt.co/10277/stripe-ebay-mastercard-quit-facebook-libra) join Paypal in quitting Libra
- [Democratizing real estate ownership](https://medium.com/realtplatform/becoming-the-landlord-of-the-future-6071abc2812a) through tokenization
- On Oct 21st, NBA star Spencer Dinwiddie still planning to [tokenize a part of his contract](https://twitter.com/SDinwiddie_25/status/1183455939774599170) in the face of NBA resistance

**General**

- Ethereum.org now [available in 11 languages](https://ethereum.org/languages/)
- [New (beta) version of MyCrypto](https://medium.com/mycrypto/live-now-try-the-new-mycrypto-4ee7d5fa7700) with multi-account management and new UX
- Hasu, Prestwich, Curtis: a model for [Bitcoin (in?)security under declining block rewards](https://uncommoncore.co/research-paper-a-model-for-bitcoins-security-and-the-declining-block-subsidy/)
- [NuCypher launches a public testnet](https://blog.nucypher.com/the-final-countdown/)
- [Aethereum](https://medium.com/avalabs/athereum-ethereum-on-avalanche-consensus-ava-labs-7effcb94b797) - a hard spoon from Ava, ie Eth state imported into an Ava chain.
- [UNICEF will now receive, hold, and spend ETH/BTC](https://www.forbes.com/sites/michaeldelcastillo/2019/10/08/6-billion-united-nations-agency-launches-bitcoin-ethereum-crypto-fund) out of a dedicated UNICEF Crypto Fund

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Oct 19-20 - [Crosslink](https://crosslink.taipei/) (Taipei)
- Oct 26 - [Zero Knowledge Summit](https://www.zeroknowledge.fm/summit) (SF)
- **Oct 28-Nov 1 - [SF Blockchain Week](https://sfblockchainweek.io/)**
- Nov 1 - [Ledger EU](https://ledgerproject.eu/) apply for 200k euro startup funding
- Nov 5-6 - [Decentralized insurance D1Conf](https://blog.etherisc.com/d1conf-2019-to-focus-on-blockchain-adoption-november-5-6th-in-malta-3b8b582ac7b4) (Malta)
- Nov 8-10 - [ETHWaterloo](https://ethwaterloo.com/)
- Jan 1 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff-update/)
- **Feb 9-15 - [EthLagos](https://ethlagos.io/)**

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

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/week-in-ethereum-news-october-13-2019/](https://weekinethereumnews.com/week-in-ethereum-news-october-13-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

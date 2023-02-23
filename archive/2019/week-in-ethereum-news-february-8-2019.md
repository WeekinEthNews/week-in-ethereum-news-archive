---
title: "February 8, 2019"
date: "2019-02-09"
---

## **Ethereum News and Links**

**Layer 1**

- \[eth1\] [Eth1 roadmap q&a](https://ethereum-magicians.org/t/eth-roadmap-ama-webinar-feb-6th-8am-pst-1700-utc-1/2518/2) video and notes
- \[eth1\] Alexey Akhunov on the [Eth1 workshop](https://medium.com/@akhounov/looking-back-at-the-ethereum-1x-workshop-26-28-01-2019-part-1-70c1ebd93266), and parts [two](https://medium.com/@akhounov/looking-back-at-the-ethereum-1x-workshop-26-28-01-2019-part-2-d3d8fdcede10) and [three](https://medium.com/@akhounov/looking-back-at-the-ethereum-1x-workshop-26-28-01-2019-part-3-cc162ca04e9f)
- \[eth2\] eth2 [spec v0.2](https://github.com/ethereum/eth2.0-specs/releases/tag/v0.2.0).
- \[eth2\] [Vitalik](https://www.reddit.com/r/ethtrader/comments/alpwlx/today_marks_the_very_first_eth20_version_release/efgov9n/): “If you followed the 1.0 release process back in 2014-15, the spec is arguably more significant than a testnet”
- \[eth2\] Soleimani/Slipper/Tsui [report on Eth2 implementation](https://docs.google.com/document/d/1PS0k9MaKPdPwEw3Uh9rq7USjq7LcSpT6ICQUXRij4YE/edit#heading=h.tptc9denl7ak) sparked lots of chat.
- \[eth2\] Ben Edgington responded to this report in [What’s New in Eth2](https://notes.ethereum.org/c/Sk8Zs--CQ/https%3A%2F%2Fbenjaminion.xyz%2Fnewineth2%2F20190208.html): “It's not wrong, it just kind of misses the point…. Rather than throwing in the towel by reverting to old-school ways of working, I would dearly love to see more good thinking on how we might do decentralisation better. There is certainly scope for doing better, this I do agree with.”
- \[eth2\] [Justin Drake](https://www.reddit.com/r/ethereum/comments/anji4w/the_state_of_ethereum_20/efwo25w/?context=3#eftwwhc) on Eth2 timelines: “2019, 2020, 2021 for phases 0, 1, 2 respectively.”
- \[eth2\] More [Justin](https://www.reddit.com/r/ethereum/comments/anji4w/the_state_of_ethereum_20/efwo25w/?context=3#efwh4az): “Phase 1 is significantly simpler than both phases 0 and 2. I expect it to come relatively soon after phase 0. Phase 1 can provide scaling by being the data availability layer for L2 execution engines…. The hard part of phase 1 is getting libp2p/gossipsub production-ready.” Parts of phase 1 and 2 are being worked on in parallel with phase 0.
- \[eth2\] Speaking of phase 1 networking: [Why libp2p](https://medium.com/paritytech/why-libp2p-13085ed0c9c8)? a networking layer explainer from Parity
- \[eth2\] Vitalik is [bullish on the Eth2 roadmap](https://twitter.com/VitalikButerin/status/1093736438808510464): “My latest position is that the current quadratic beacon chain architecture is all we'll need for a long long time. Maybe forever.”
- \[eth2\] More on what’s in the Eth2 roadmap in the latest [Eth2 implementer call notes](https://github.com/ethereum/eth2.0-pm/blob/master/eth2.0-implementers-calls/call_011.md)
- \[eth2\] Logic and economics around [how long to process a stake withdrawal](https://ethresear.ch/t/rate-limiting-entry-exits-not-withdrawals/4942)
- \[eth2\] [Lighthouse](https://lighthouse.sigmaprime.io/update-07.html) dev update. Sets expectations for q1 testnet: cross-client public testnet, may only be short-lived. This update was particularly readable even for non-Eth2 experts
- \[eth2\] [Yeeth](https://medium.com/yeeth/yeeth-updates-1-5474eb78c319) dev update
- \[eth2\] Rocketpool has a [beacon chain simulator](https://medium.com/rocket-pool/development-update-6th-feb-2019-850e6c01657e) they’ll use for a staking pool test, with RPL rewards for testers.
- \[eth2\] Eth2 [implementer workshop notes](https://hackmd.io/8Wka34uPT2unwJoYvkRYew?view) and [video](https://www.youtube.com/watch?v=3_ZFdQHivJQ)
- \[eth2\] A short and high level [overview of the Beacon Chain](https://twitter.com/cemozer_/status/1090399936938532864), eth2’s phase 0
- If you’re a developer who wants to know how Eth2 will affect your code, [ask your question here](https://twitter.com/0xstark/status/1093550638825381896).

**Layer 2**

- LeapDAO (fka ParsecLabs) [Plasma testnet](https://leapdao.org/blog/Plasma-Testnet-Launched/): More Viable Plasma, single operator for ERC20 & 721 tokens
- Streamr teases their [“Monoplasma” ETHDenver demo](https://medium.com/streamrblog/ethdenver-streamr-2019-8c3806b703cf) to pay many addresses, but no details yet. Sounds a bit like Nick Johnson’s [multisends with one-time addresses](https://medium.com/@weka/how-to-send-ether-to-11-440-people-187e332566b7) or RicMoo’s [Merkle AirDrops](https://blog.ricmoo.com/merkle-air-drops-e6406945584d)
- A proposed [POA sidechain like xDAI for mili-Eth](https://forum.poa.network/t/could-another-chain-be-like-poa-xdai-but-backed-by-eth/1909). The mEth chain.
- Privacy and scaling [problems of layer2 watchtower services](https://medium.com/crypto-punks/lightning-vs-raiden-watchtowers-monitoring-services-solutions-e243f7793d19)
- state channel dev updates: [Celer](https://medium.com/celer-network/celer-network-23rd-weekly-project-progress-report-2-4-2-8-80d029e5f7bb), [Connext](https://medium.com/connext/connext-biweekly-update-7-a374d834b03c), [Magmo](https://medium.com/magmo/dev-update-2-nitro-sneak-peek-b4e0e0a3979b)

**Client releases - get ready for the fork!**

- Parity v[2.3.2-beta](https://github.com/paritytech/parity-ethereum/releases/tag/v2.3.2) and [v2.2.9-stable](https://github.com/paritytech/parity-ethereum/releases/tag/v2.2.9) fixing a JSONRPC vuln that allowed attacker to crash node
- [EthereumJS VM v2.6.0 (Petersburg/Goerli)](https://github.com/ethereumjs/ethereumjs-vm/releases/tag/v2.6.0) 

**Stuff for developers**

- [Solidity graph debugger](https://github.com/fergarrui/ethereum-graph-debugger) v2. Rewritten with new UI and API
- Formal Verification explainer series, pt 2: [proving the correctness of a token](https://medium.com/ethworks/formal-verification-for-n00bs-part-2-proving-the-correctness-of-a-token-74085f5cd6c1) in KLAB
- [Graph Explorer](https://medium.com/graphprotocol/announcing-graph-explorer-a39318ffb569) launches with Dharma, Compound, Uniswap, ENS, Origin, Decentraland, and Livepeer as partners, so devs can explore data on all those projects.
- [Getting started with the Görli testnet](https://mudit.blog/getting-started-goerli-testnet/). Etherscan now [supports Goerli](https://goerli.etherscan.io/).
- [Getting started with EthPM and web3.py](https://snake-charmers.ethereum.org/2019/01/24/ethpm.html)
- Taylor Monahan: [building user confidence, not dapps](https://medium.com/mycrypto/building-confidence-not-dapps-d8a3bc1f29d1)
- [Vuethereum](https://blog.matryx.ai/vuethereum-the-vue-library-ethereum-deserves-de5dc66f1839): a Vue.js frontend library. And a [vue.js Solidity IDE](https://github.com/System-Glitch/Solidity-IDE)
- ENS Manager [supports EIP1577 contenthash](https://medium.com/the-ethereum-name-service/the-new-ens-manager-now-supports-eip1577-contenthash-82e2d6724fae)
- [LimePay](https://limepay.io/): enable your users to execute Eth transactions with fiat
- [Groundhog Network](https://medium.com/groundhog-network/its-now-groundhog-day-all-year-long-5867a7424ac7): subscription crypto payments for merchants, who can also convert to fiat.
- Build your own embeddable [frontend on Dether](https://medium.com/dether/the-dether-protocol-towards-a-decentralized-cash-to-crypto-otc-protocol-for-dapps-939a96fae85b) for in person fiat transactions
- [Upgradeability is a Bug](https://medium.com/consensys-diligence/upgradeability-is-a-bug-dba0203152ce). This used to be a more common theme of debate.
- [Testing real world upgrades](https://blog.zeppelinos.org/testing-real-world-contract-upgrades/?utm_campaign=wie-technical-testing-contract-upgrades&utm_medium=wie&utm_source=weekinethereumnews) from ZeppelinOS. And what makes a [good EVM Package](https://blog.zeppelinos.org/building-blocks:-what-makes-a-good-evm-package/?/&utm_campaign=zos-technical-evmpackages&utm_medium=social&utm_source=weekinethereum)
- 3Box’s [Spaces](https://medium.com/3box/introducing-spaces-app-specific-private-data-storage-4d75ccc2a859): app-specific data storage, permissioned by users
- [web3.js v1.0.0-beta.44](https://github.com/ethereum/web3.js/releases/tag/v1.0.0-beta.44)
- Embark tutorial: [building a decentralized Reddit](https://embark.status.im/news/2019/02/03/building-a-decentralized-reddit-with-embark-part-1/), pt1
- [Buidler](https://medium.com/nomic-labs-blog/buidler-the-new-smart-contract-development-tool-14d81428757c) beta release. Task runner with plugins for web3.js 0.2.x, web3.js 1.x, Truffle 4, Truffle 5, and Ethers.js

**zk**

- [zkSNARKs in WebAssembly](https://community.zkproof.org/t/zksnarks-in-webassembly-running-demo-and-discussion/30) with online demo
- Remco Bloemen’s [intro to STARKs](https://hackmd.io/s/rJHYnQ3Z4) 
- Starkware: [STARK math](https://medium.com/starkware/stark-math-the-journey-begins-51bd2b063c71), part 1
- [Eli Ben Sasson](https://www.youtube.com/watch?v=lMr3lbY5FpE) conversation with Balaji Srinivasan
- More on [Aztec Protocol’s Huff language](https://medium.com/aztec-protocol/from-zero-to-nowhere-smart-contract-programming-in-huff-1-2-ba2b6de7fa83), which basically macros of EVM assembly opcodes. They wrote it for their library for validating zero-knowledge proofs
- [ZCash found a cryptographic vulnerability](https://z.cash/blog/zcash-counterfeiting-vulnerability-successfully-remediated/), kept it secret for almost a year, fixed it with Sapling, and now discloses it. No one thinks an exploitation likely occurred, as only ~12 people ever had access to the MPC transcript necessary to exploit.

**Ecosystem**

- Afri wants you to [vote on upcoming release (fork) names](https://www.reddit.com/r/ethtrader/comments/ao412z/the_exclusive_ethereum_hardfork_naming_finals/)
- [ECF 2.0](https://medium.com/@EthereumECF/ecf-network-more-than-grants-7bfa571458fb), how it’s restructuring for 2019
- web3 [design decision framework](https://medium.com/@lyricalpolymath/web3designdecisionframework-e84075816515)
- All the ways [ETHDenver is dogfooding](https://medium.com/ethdenver/ethdenver-2019-experiential-buidlathon-to-put-blockchain-tech-use-cases-in-the-palm-of-attendees-750e1d524c75)
- Despite some reports, EF hasn’t decided to [spend 15m on VDF](https://twitter.com/drakefjustin/status/1093667807861067776)s. It’s half that, under discussion and not an imminent decision. So far EF has funded five figure amounts for VDF researchers.
- In Norway, Denmark, and Sweden, [Opera tests letting its users buy Eth](https://breakermag.com/web-3-0-opera-browser-launches-instant-crypto-purchases/) instantly in the browser through Swedish exchange Safello.

**Enterprise**

- Microsoft video on [Azure Logic App Connector to Ethereum](https://www.youtube.com/watch?v=lrFXN1-3m14)
- [Indonesian farming platform](https://breakermag.com/in-indonesia-blockchain-powered-farming-blossoms/) on a private chain
- Bloomberg on [JPMorgan’s blockchain payments](https://www.bloomberg.com/news/articles/2019-01-29/jpmorgan-says-blockchain-is-making-progress-outside-of-crypto) efforts

**Governance and Standards**

- A proposal [lost in Aragon vote](https://blog.aragon.org/final-results-from-aragon-network-vote-1/). Things losing votes seems like a good thing to start happening occasionally. (Missed this last week due to Twitter wrongfully banning me)

**Application layer**

- [Reddit is exploring using Ethereum](https://www.reddit.com/r/ethtrader/comments/an5577/a_communityled_initiative_to_decentralize_donuts/) to tokenize karma (eg, r/ethtrader’s donuts)
- Maker to [double the stability fee to 1%](https://medium.com/makerdao/increasing-the-stability-fee-f586830c4e0c), pending Feb 12 vote. Also, [Dai by the numbers](https://medium.com/makerdao/dai-in-numbers-2710d8a5633a).
- [Kyber integrated Uniswap](https://twitter.com/KyberSwap/status/1092792253888819201) for better DAI/MKR rates
- [Streamr and FOAM](https://discourse.foam.space/t/foam-streamr-for-pollution-monitoring-a-project-i-have-been-working-on/550) for pollution monitoring
- [VegaRelay](https://coinlist.co/build/0x/projects/9d596d96-c914-4b2c-b2ec-10d269467e8c): a 0x relayer for volatility markets on Augur
- A [Forex relay on 0x](https://alpha.fordex.co/)
- A guide to [Veil’s orderbook](https://medium.com/veil-blog/off-chain-trading-with-augur-and-0x-e2f0c05db3bd)
- [Grid+ goes live selling electricity](https://blog.gridplus.io/gridplus-is-live-in-texas-efc83c814601) for most Texans

**Interviews, Podcasts, Videos, Talks** 

- [Taylor Monahan](https://podcast.ethhub.io/taylor-monahan-of-mycrypto-interacting-with-the-ethereum-blockchain) on Into the Ether
- NEAR’s [Alex Skidanov sharding research](https://youtu.be/UTs9ZkX401M) talk
- Latest [TCR call](https://www.youtube.com/watch?v=BdQaHuGTDW0)
- Latest [Curation Markets call](https://www.youtube.com/watch?v=PgfwRSAeTdA)
- NuCypher’s [Bogdan Opanchuk and John Pacific](https://www.zeroknowledge.fm/63) on Zero Knowledge
- Melonport M1 conf [day 2](https://www.youtube.com/watch?v=Opj_5ORbyXA). Day 1 blocked due to copyright.
- [Ale Machado and Alex Gladstein](https://www.youtube.com/watch?v=Z6UTF8fex3c) on crypto in Venezuela with Brian Armstrong

**Tokens / Business / Regulation**

- [TCR Party](https://www.reddit.com/r/ethereum/comments/an3ud1/tcr_party_a_twitter_curated_registry/) - a TCR experiment where you make testnet transactions through Twitter to control membership of a Twitter RT list. Fun to play with, not sybil resistant nor necessarily representative of mainnet
- Collectible [NFT art made physical](https://medium.com/coinmonks/adventures-in-art-1b068ab0ebed)
- [Bonding curve playground](https://bondingplayground.netlify.com/)
- Panvala expands [token grants to include scalability](https://medium.com/@Panvala/make-ethereum-scale-panvala-token-grants-for-scaling-projects-20393d50b269)
- 0x open sources its [legal thinking on decentralized finance](https://blog.0xproject.com/new-legal-resources-for-the-0x-ecosystem-55044a21a3d2)
- [SEC Commish Hester Peirce speech](https://www.sec.gov/news/speech/peirce-regulation-view-inside-machine) on how she thinks about cryptoassets

**General**

- Quadriga was everywhere in the news this week. The founder died, some think he faked his death, they’re behind on payments, and apparently they [never had cold wallets anyway](https://twitter.com/tayvano_/status/1092439754849759233)? I have no idea, but it’s a reminder that you should take charge of your cryptoassets by having them on private keys that you control.
- Brave browser & [BAT on Coinbase Earn](https://blog.coinbase.com/earn-bat-while-trying-out-the-blockchain-friendly-brave-browser-ee8409d192bd)
- Convert [fiat on AirSwap with Wyre](https://medium.com/fluidity/convert-fiat-on-airswap-with-wyre-48c6d044d8cb)
- Gemini [shut down some OTC trading desks](https://www.coindesk.com/winklevoss-crypto-gemini-gusd-stablecoin-redemption) when they tried to redeem Gemini’s GUSD dollarcoin
- Kraken [acquires futures trading platform](https://blog.kraken.com/post/2089/kraken-acquires-crypto-derivatives-trading-platform-and-index-provider-crypto-facilities-in-nine-figure-deal-official-press-release/)
- Facebook has been [paying teens to spy](https://techcrunch.com/2019/01/29/facebook-project-atlas/) on their every mobile move.

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Feb 14 - [Eth Magicians](https://hackmd.io/s/rklzFyVX4) (Denver)
- Feb 15-17 - [ETHDenver](https://www.ethdenver.com/) hackathon (ETHGlobal) 
- Feb 27 - [Constantinople](http://didtheethereumblockchainreach1tbyet.5chdn.co/) (block 7280000)
- Mar 4 - [Ethereum Magicians](https://ethereum-magicians.org/t/council-of-paris-2019-announcement/2438) (Paris)
- Mar 5-7 - [EthCC](https://ethcc.io/) (Paris)
- Mar 8-10 - [ETHParis](https://ethparis.com/) (ETHGlobal)
- Mar 8-10 - [EthUToronto](https://www.ethuoft.ca/)
- Mar 22 - [Zero Knowledge Summit 0x03](https://www.zeroknowledge.fm/summit) (Berlin)
- Mar 27 - Infura [end of legacy key support](https://blog.infura.io/infura-dashboard-update-9f02d0643eb3) 
- April 4-5 - [Deconomy](https://deconomy.com/seoul2019/) (Seoul)
- April 8-14 - [Edcon](https://www.edcon.io/) hackathon and conference (Sydney)
- Apr 19-21 - [ETHCapetown](http://ethcapetown.com/) (ETHGlobal)
- Apr 24-26 - [Truffle Elevate](https://www.eventbrite.com/e/truffle-elevate-dublin-2019-blockchain-development-workshop-tickets-53831596755) (Dublin)
- May 10-11 - [Ethereal](https://etherealsummit.com/?ref=weekinethereum) (NYC)
- May 17 - Deadline to accept [proposals for Instanbul upgrade](https://en.ethereum.wiki/roadmap/istanbul) fork

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)

  
I own Week In Ethereum. Editorial control has always been 100% me. 

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **New URL: [weekinethereumnews.com](https://weekinethereumnews.com/) & suspended from Twitter (again!)**

Archive on the web if you’re linking to it:  [](https://weekinethereumnews.com/february-8-2019/)[https://weekinethereumnews.com/february-8-2019/](https://weekinethereumnews.com/february-8-2019/)

Cent link for the night view:  [https://beta.cent.co/+4zsouo](https://beta.cent.co/+4zsouo)

* * *

**Suspended from Twitter**: I was wrongfully suspended from Twitter for part of the week, which definitely impacts newsletter quality. Sorry! The best part is that they unbanned me and [apologized for wrongfully banning me, only to wrongfully ban me again 30 minutes later](http://Permalink ∞). You can’t make this up.

_Censorship resistance_ matters.

* * *

Assuming I’m not suspended, follow me on Twitter, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

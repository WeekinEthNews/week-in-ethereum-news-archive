---
title: "June 15, 2019, Ethereum News"
date: "2019-06-16"
---

## **Ethereum News and Links**

**Layer 1**

- [Eth2 spec v0.7](https://github.com/ethereum/eth2.0-specs/releases/tag/v0.7.0) - phase 1 now executable
- [Lighthouse eth2 client update](https://lighthouse.sigmaprime.io/update-12.html). spec update, REST API into spec, fuzzing, BLS sigs optimization, discv5 networking discovery
- Parity’s Shasper eth2 [client updates to 0.7](https://github.com/paritytech/shasper/pull/158)
- Latest [Eth2 implementer call](https://www.youtube.com/watch?v=izspfej05lE). [Notes](https://github.com/ethereum/eth2.0-pm/blob/066a48e7b6587bb5857d867154bc319196880cb5/eth2.0-implementers-calls/call_019.md).
- [Eth2 deposit Merkle tree](https://medium.com/@josephdelong/ethereum-2-0-deposit-merkle-tree-13ec8404ca4f)
- Runtime Verification: [Formal verification of Eth2 deposit contract](https://runtimeverification.com/blog/formal-verification-of-ethereum-2-0-deposit-contract-part-1/)
- Bégassat, et al, arxiv: [Practical Multi-Signature Aggregation for Large Byzantine Committees](https://arxiv.org/abs/1906.05132)
- Vitalik: [Universal fee market execution environment to rule them all](https://ethresear.ch/t/one-fee-market-ee-to-rule-them-all/5608)

**Client releases**

- Parity v[2.5.2-beta](https://github.com/paritytech/parity-ethereum/releases/tag/v2.5.2) or v[2.4.7-stable](https://github.com/paritytech/parity-ethereum/releases/tag/v2.4.7)
- Swarm [v0.4.1](https://github.com/ethersphere/swarm/blob/master/CHANGELOG.md). See also [Swarm on Wasm](https://medium.com/fair-data-society/swarm-on-wasm-swasm-7ec58fc78ab0?sk=9564ae13fd6a1f91a52ff597f61eac12)

**Layer 2**

- [Deep dive into StarkDEX, part 1](https://medium.com/starkware/starkdex-deep-dive-introduction-7b4ef0dedba8)
- [Rollup Plasma for mass exits & complex disputes](https://plasma.build/t/rollup-plasma-for-mass-exits-complex-disputes/90)

**Stuff for developers**

- [ethers.js v5 beta](https://blog.ricmoo.com/beta-release-ethers-js-v5-59d0db222d7b)
- [Gas golf the eth2 deposit contract](https://twitter.com/drakefjustin/status/1139989022577758211) in the next week
- [Managing Eth events with Drizzle](https://medium.com/truffle-suite/managing-ethereum-smart-contract-events-with-drizzle-58f3f9afbdad)
- Truffle [v5.0.22](https://github.com/trufflesuite/truffle/releases/tag/v5.0.22) - some debugger improvements
- [Metamask auditing their dependencies](https://medium.com/metamask/dependency-audit-retrospective-june-2019-df6e573ecb5d)
- [Portis white paper on its e2e private key encryption](https://assets.portis.io/white-paper/latest.pdf)
- How does [Bloom (identity) Share Kit](https://bloom.co/blog/how-does-share-kit-work/) work?
- A tutorial in [getting data off your own node](https://medium.com/@tjayrush/counting-shit-on-ethereum-39844b37259c)
- Add [Rimble UI to web3React](https://github.com/crisgarner/web3-connector)
- [Vyper GUI v0.3](https://github.com/ssteiger/Vyper-Contract-GUI/releases)
- [Hook BigQuery up to Ethereum using Chainlink](https://cloud.google.com/blog/products/data-analytics/building-hybrid-blockchain-cloud-applications-with-ethereum-and-google-cloud). Interesting use case for submarine sends over an hour.
- [Request Network API](https://request.network/en/2019/06/12/introducing-request-api-electronic-invoicing-made-easy/) to create and read invoices
- Dex.ag API to [embed best dex price in a widget on your site](https://concourseopen.com/blog/dex-ag-sdk-best-price-with-5-lines-of-code/)
- [Handling revert exceptions](https://blog.polymath.network/try-catch-in-solidity-handling-the-revert-exception-f53718f76047) in Solidity
- Shadowlands: [create CLI dapps without the web](https://levelup.gitconnected.com/ethereum-dapps-without-the-web-309f09513b64)
- [Bugue](https://github.com/dr6kl/buguet)t: eth debugger
- [Poke](https://medium.com/reserve-currency/poke-a-cli-tool-for-ethereum-development-b4bb66f4e438?postPublishedType=initial): cobra CLI tool for Eth dev
- [Grid](https://medium.com/ethereum-grid/introducing-ethereum-grid-1e65e7fb771e): desktop (Electron) app as a base for ecosystem clients and tools
- [3Box theads, a chat system for dapps](https://medium.com/3box/3box-threads-a-chat-system-for-decentralized-apps-7a77be49680c) using IPFS and OrbitDB

**Ecosystem**

- Devcon [speaker applications are open](https://blog.ethereum.org/2019/06/10/devcon-in-osaka-applications-now-open/), with ticket sales to begin in mid-July
- How the [Grid+ SafeCard is a viable cold storage option](https://blog.gridplus.io/understanding-the-safecard-18fdd8722c7d)
- [FindEth](https://findeth.io/), a tool to find lost Ether
- [Deploy Gnosis Safe from a Burner Wallet](https://www.youtube.com/watch?v=ONlB-LK3D0g&feature=youtu.be). Obviously from Austin Griffith.
- [MetaTransactions to scale Ethereum](https://hackernoon.com/how-meta-transactions-will-scale-ethereum-e98c848f7719): yes, Gas Stations Network is awesome.
- [Timeline for 3-6 character ENS domains](https://medium.com/the-ethereum-name-service/timeline-for-3-6-character-name-reservation-auction-and-instant-registrations-e39aa2f89dc9). Tentatively: reserve in July, auction in Sept
- EtherCattle and Rivet: [making Eth node infrastructure easier to manage](https://blog.openrelay.xyz/ether-cattle-operationally-manageable-ethereum-clients/)

**Enterprise**

- [Pantheon Essentials Certification](https://learn.consensys.net/catalog/info/id:151) course
- How [Nightfall makes token transactions private](https://medium.com/@chaitanyakonda/nightfall-makes-token-transactions-on-ethereum-private-how-does-it-work-acf2ffd0aa7a)

**Governance and Standards**

- r/ethtrader appears to have turned against “donuts” (Reddit’s community points) as a coinvote governance mechanism. [One of several threads](https://www.reddit.com/r/ethtrader/comments/bz0vbj/can_we_get_rid_of_donuts/).
- iExec on how [upgradeable contracts is governance](https://medium.com/iex-ec/poco-series-6-smart-contract-upgradeability-and-governance-68d2cdecd120).
- [dOrg launches limited liability DAO](https://www.gravelshea.com/2019/06/dorg-launches-first-limited-liability-dao/) under Vermont regulatory regime.

**Live on mainnet**

- [Opyn live on mainnet](https://medium.com/opyn/opyn-is-live-on-mainnet-49e26f77b). Noncustodial margin trading platform on top of Compound, Uniswap, & DAI.
- bZx margin trading launches with [750k in liquidity](https://medium.com/bzxnetwork/fulcrum-launches-with-over-750-000-of-liquidity-aa1d28a66510).

**Application layer**

- [Austria’s Post Office is selling stamps](https://www.reddit.com/r/ethtrader/comments/c07g4n/the_cryptokitties_of_stamps/) with associated ERC721 collectibles
- [Maker/CDP data viz](https://medium.com/alethio/the-defi-series-statistics-around-maker-cdps-loans-and-top-users-67d5a634c58c) from Alethio
- [Instadapp](https://medium.com/instadapp/bridge-protocols-eb14b2dd0fe7) and [CDP Saver](https://www.reddit.com/r/ethereum/comments/c05d27/cdp_saver_adds_compound_support_generate_cdai/) built similar bridges between Maker and Compound. Transact easily between the two to generate cDai or repay CDP
- Stats and graphs on [defi lending in May](https://medium.com/bloqboard/decentralized-finance-defi-lending-snapshot-may-2019-66abe2dd1637)
- A [market map](https://puntium.github.io/electric-crypto-market-map-v0_5.pdf) from Electric Capital
- TruSet and Imbrex partnering for [state by state collection of residential real estate contracts](https://www.truset.com/news/2019/6/5/truset-and-imbrex-partner-to-create-the-first-blockchain-based-state-by-state-collection-of-residential-real-estate-contracts)
- Sablier: if [time is money, why isn’t it continuous](https://medium.com/sablier-app/making-money-flow-f1d18330cd20)?
- [Standard Bounties v2](https://medium.com/bounties-network/ushering-in-a-new-era-of-bounties-2cc56621956e)
- A [thought experiment to understand prediction markets](https://www.augur.net/blog/thought-experiment/)
- FOAM does [proof of location over radio](https://discourse.foam.space/t/foam-location-update-and-demo-documentation/859)
- [Tokenized and tradable income share agreements](https://medium.com/@josh.ma91/a-new-kind-of-student-loan-tokenizing-income-share-agreements-and-trading-them-using-openlaw-c2566800b20d) with OpenLaw
- [Ubisoft considering putting game accessories onchain](https://www.reddit.com/r/ethtrader/comments/bzaovz/ubisoft_ethereum/)

**Interviews, Podcasts, Videos, Talks** 

- [Ameen Soleimani](https://ethhub.substack.com/p/talking-ethereum-with-ameen-soleimani) on Into the Ether
- AllInfra’s [Dave Sandor and Bill Kentrup](https://media.consensys.net/the-bkp-podcast-episode-1-how-blockchain-is-making-infrastructure-investments-more-accessible-6e3d0e497dc9) on BKP Podcast
- Quickblocks’ [Jay Rush](https://www.youtube.com/watch?v=rOWDO-IydyQ) on Daxia
- [Nick Johnson](https://anchor.fm/blockhash-exploring-the-blockchain/episodes/Nick-Johnson---Lead-Developer-for-ENS-e4aokv/a-ah12ap) on Blockhash

**Tokens / Business / Regulation**

- Iceland regulators approve [Monerium on mainnet to provide European fiat payment services](https://www.coindesk.com/icelandic-regulators-approve-startups-plan-for-fiat-payments-on-ethereum).
- Bittrex [delisting 42 assets](https://bittrex.zendesk.com/hc/en-us/articles/360029523891) for Americans
- [Wrapped Cryptokitties](https://wrappedkitties.com/): make your erc721 into erc20
- [DAI/USDC on dydx](https://medium.com/dydxderivatives/dai-usdc-market-launches-on-dydx-bde957c48e2e). You read that right: you can restore the peg or play Soros.
- de la Rouviere: [Maximizing blockchain collectible cconomies](https://blog.simondlr.com/maximising-blockchain-collectible-economies)

**General**

- An [intro to zero knowledge](https://medium.com/@kscarbrough1/blockchain-is-just-one-chapter-in-the-larger-story-being-written-by-cryptography-right-now-a6d6a94ff372) in the context of the history of cryptography
- Enigma releases their [Discovery developer testnet](https://blog.enigma.co/the-discovery-testnet-developer-release-is-live-57db09fa23e)
- BBC covers [Bounties Network’s trash cleanup in Manila](http://www.bbc.com/future/story/20190613-a-simple-online-system-that-could-end-plastic-pollution)
- [Zilliqa enables smart contracts](https://blog.zilliqa.com/zilliqa-has-now-successfully-enabled-the-first-ever-smart-contract-platform-built-on-sharding-426748b47d32) and thus becomes the first sharded chain with contracts.

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- June 22-24 - [Zcon1](https://www.zfnd.org/zcon/) (Split, Croatia)
- **June 24- July 10 - [Gitcoin’s Beyond Blockchain](https://gitcoin.co/blog/beyond-blockchain-hackathon/) virtual hackathon**
- **June 25-27 - [EthPlanet hackathon](https://www.huodongxing.com/event/8495466131800) (Beijing)**
- July 3-5 - [WindingTree’s HackTravel](https://windingtree.com/hacktravel-lisbon-2019) (Lisbon)
- July 19 - [BuildETH](https://www.buildeth.io/) (San Francisco)
- **July 19-21 - [State of Scale](https://www.stateofscale.com/) (Los Angeles)**
- July 22-23 - [Buidl](https://www.buidl.asia/) 2019 (Seoul)
- Aug 2-4 - [ETHIndia](https://ethindia.co/) (Bangalore)
- Aug 2-4 - [TruffleCon](https://www.truffleframework.com/trufflecon2019) (Redmond)
- Aug 21-23 - [Dappcon](https://dappcon.io/) (Berlin)
- Aug 23-25 - [ETHBerlin](https://ethberlinzwei.com/)
- Sep 3 - Deadline to [apply for EU Horizon Prize](https://ec.europa.eu/info/funding-tenders/opportunities/portal/screen/opportunities/topic-details/blockchain-eicprize-2019). 1m € each to 5 "Blockchains for Social Good" projects
- Sep 6-8 - [EthBoston](https://eth.boston/)
- Sep 15 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff/)
- Sep 15 - [Ethereal Tel Aviv](https://etherealsummit.com/events/ethereal-tel-aviv/)
- **Sep 15-16** \- [StarkWare sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- Oct 8-11 - [DeVcon](https://devcon.org/) (Osaka)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I 100% own Week In Ethereum. Editorial control has always been by me.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **Link to this URL: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [](https://weekinethereumnews.com/june-15-2019-week-in-ethereum-news/)[https://weekinethereumnews.com/june-15-2019-week-in-ethereum-news/](https://weekinethereumnews.com/june-15-2019-week-in-ethereum-news/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

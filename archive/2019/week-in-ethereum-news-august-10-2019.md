---
title: "Week in Ethereum News <BR> August 10, 2019"
date: "2019-08-11"
---

## **Ethereum News and Links**

**Layer 1**

- The latest [what's new in Eth2](https://notes.ethereum.org/c/Sk8Zs--CQ/https%3A%2F%2Fbenjaminion.xyz%2Fnewineth2%2F20190802.html)
- [Prysmatic Eth2 client update](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-32-prysmatic-labs-1fce63459403), networking and optimizations
- [Nimbus Eth2 client update](https://our.status.im/nimbus-development-update-aug-5/). eth2 genesis testing environment, working on networking
- [What does “finalization” mean in Eth2](https://our.status.im/two-point-oh-justification-and-finalization/)?

**Layer 2**

- [Connext v2](https://medium.com/connext/v2-0-is-on-testnet-805e91116008) is on testnet, planning on mainnet around EthBerlin in a few weeks

**Stuff for developers**

- [ENS can be used for non-Ethereum things](https://medium.com/the-ethereum-name-service/what-the-ethereum-means-in-ethereum-name-service-17171141d688)
- [Galois](https://github.com/GuildOfWeavers/galois): a JavaScript/WASM library for finite field arithmetic
- Trail of Bits releases [aggregate data from all their Eth code audit](https://blog.trailofbits.com/2019/08/08/246-findings-from-our-smart-contract-audits-an-executive-summary/)s. They find 1) many bugs are catchable with automated tools, 2) vulnerabilities are similar to other systems, 3) unit testing doesn’t prevent much. Trail of Bits also released new version of symbolic execution tool: [Manticore v0.3.1](https://github.com/trailofbits/manticore/releases/tag/0.3.1)
- Slockit’s [Piet](https://blog.slock.it/analyzing-solidity-smart-contracts-with-piet-6db33a733e79) - inheritance structure graph, a GUI to interact with contracts
- web3.js [2.0.0-alpha.1](https://github.com/ethereum/web3.js/releases/tag/v2.0.0-alpha.1) and v[1.2.1](https://github.com/ethereum/web3.js/releases/tag/v1.2.1)
- [Pantheon-ethers](https://github.com/naddison36/pantheon-ethers) extends Ethers.js with Pantheon APIs including private transactions
- Running a [Pantheon node in Java integration tests](https://kauri.io/article/7dc3ecc391e54f7b8cbf4e5fa0caf780/running-a-pantheon-node-in-java-integration-tests)
- [Tokenizing products with Uniswap and OpenLaw](https://medium.com/@openlawesq/tokenizing-products-using-uniswap-and-openlaw-part-1-a4f30d1740e1)
- Portis’ [One Click Pay](https://medium.com/@portis/introducing-portis-one-click-pay-48ec3670f363) for when buyer doesn’t have enough Eth. Sign the transaction and only submit it once there is enough Eth.
- Writing [accurate time-dependent Truffle tests](https://medium.com/sablier/writing-accurate-time-dependent-truffle-tests-8febc827acb5)

**Live on mainnet**

- [Tornado.cash mixer](https://medium.com/@tornado.cash.mixer/introducing-private-transactions-on-ethereum-now-42ee915babe0) live on mainnet. It’s limited to 0.1 ETH as the trusted setup was done by them on a single machine with plans to [use Gnosis/Matter’s ceremony](https://www.reddit.com/r/ethereum/comments/clvex0/tornadocash_is_deployed_on_mainnet_give_it_a_try/evz77kj/?context=3).
- [Gas Station Network](https://medium.com/tabookey/united-we-stand-in-a-trustless-way-fd28ecf4126f) live on mainnet. Decentralized meta transaction relayer so you can [pay to onboard your users](https://medium.com/coinmonks/eth-onboarding-solution-90607fb81380).

**Ecosystem**

- Avsa on the [direction of the Ethereum Foundation](https://medium.com/universal-ethereum/where-ethereum-is-going-ef4dad35d748)
- [MetaCartel DAO’s first grants](https://medium.com/metacartel/metacartel-dao-wave-1-funding-9e2beb1fcd8e) - Mintbase, Odyssy, Kickback, NFTs for reputation
- [ETH declared compliant with Islamic law](https://amanieadvisors.com/shariah-white-paper-on-ethereum/)
- [VAC](https://vac.dev/vac-overview) - modular p2p messaging stack focused on secure messaging

**Enterprise**

- [Aya Miyaguchi joins the EEA’s board and EEA has a new working group, the Mainnet Initiative](https://entethalliance.org/enterprise-ethereum-alliance-appoints-ethereum-foundation-aya-miyaguchi-to-the-eea-board-and-launches-mainnet-initiative/)
- [Quorum v2.2.5](https://github.com/jpmorganchase/quorum/releases/tag/v2.2.5)

**Governance and Standards**

- Swende: More frequent and smaller [EIP-centric forking](https://notes.ethereum.org/s/S1ELAYY7S) instead of setting deadlines and rushing to get EIPs into the fork.
- [Computer aided governance](https://medium.com/block-science/computer-aided-governance-cag-a-revolution-in-automated-decision-support-systems-9faa009e57a2) in the Commons Stack
- [ERC2229](https://github.com/ethereum/EIPs/issues/2229): Ping interface for inactive tokens

**Application layer**

- OpenLaw’s [integration framework](https://medium.com/@OpenLawOfficial/introducing-openlaws-integration-framework-making-it-easy-to-integrate-third-party-services-into-f28eb779856b). Bring things like DocuSign or Chainlink into your org through API.
- Augur v2’s [faster market resolution system](https://www.augur.net/blog/v2-resolution/)
- [AirSwap Trader](https://medium.com/fluidity/introducing-airswap-trader-63a0ef9e67c0) - OTC trades through escrow in onchain code
- WindingTree lands a [deal with Etihad Airways](https://www.reuters.com/article/us-blockchain-airlines-etihad-idUSKCN1UY2A9)

**Interviews, Podcasts, Videos, Talks** 

- Prysmatic’s [Raul Jordan](https://www.zeroknowledge.fm/89) on Zero Knowledge
- Latest [curation markets call](https://www.youtube.com/watch?v=lqPEcPNhLls)
- [Vitalik Buterin](https://www.youtube.com/watch?v=2L2fyeoS99c) on MaiCoin
- [Vitalik Q&A](https://youtu.be/nRBcOWpjs-4?t=29365) from ETHIndia
- ConsenSys Diligence’s [Steve Marx](https://thebitcoinpodcast.com/hashing-it-out-55/) on Hashing It Out
- POA’s [Igor Barinov](https://epicenter.tv/episode/299/) on Epicenter
- SuperRare’s [John Crain](https://anchor.fm/wizardofdapps/episodes/Episode-14-SuperRare-with-John-Crain-e4siin/a-akcufk) on Wizard of Dapps

**Tokens / Business / Regulation**

- Ryan Sean Adams: [ETH is money, and it matters](https://thedefiant.substack.com/p/ethereum-only-wins-if-eth-is-money)
- Seychelles stock exchange [lists security token](https://www.coindesk.com/national-stock-exchange-becomes-worlds-first-to-list-a-tokenized-security)
- Linda Xie’s [Future of DeFi](https://lindajxie.com/2019/08/07/the-future-of-decentralized-finance/)
- Livepeer [participation rate passes 50%](https://forum.livepeer.org/t/livepeer-participation-rate-passes-50/853), an interesting experiment in how stakers respond as inflation rate stops increasing and transaction fees increase

**General**

- [Randomness in blockchain protocols](https://nearprotocol.com/blog/randomness-in-blockchain-protocols/)
- [Binance KYC data leaked](https://www.coindesk.com/a-bitcoin-extortion-gone-wrong-inside-binances-negotiations-with-its-kyc-hacker). Centralization strikes again.
- [How Coinbase defeated Firefox day 0 vulnerability](https://blog.coinbase.com/responding-to-firefox-0-days-in-the-wild-d9c85a57f15b) exploitation
- [Federal Reserve to introduce real time payments](https://www.pymnts.com/news/payments-innovation/2019/federal-reserve-to-launch-fednow-instant-payments) system… in 2023 or 2024

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- **Aug 15 - [Devcon tickets on sale again](https://twitter.com/EFDevcon/status/1159573388433723392) (3pm CEST)**
- Aug 15 - [Grow Ethereum](https://hackathons.gitcoin.co/grow-ethereum/) virtual hackathon ends
- Aug 16 - 18 - [ConsenSys Grants hackathon](https://pages.consensys.net/toronto-grants-hackathon) (Toronto)
- Aug 21-23 - [Dappcon](https://dappcon.io/) (Berlin)
- Aug 23 - [Last day for IDEX withdrawals](https://medium.com/idex/idex-kyc-transition-period-and-updated-asset-availability-for-us-markets-set-to-begin-d45e945f842d) without KYC
- Aug 23-25 - [ETHBerlin](https://ethberlinzwei.com/)
- Aug 29-30 - [ERC1400 security token hackathon](https://medium.com/@ramvi/invitation-to-hackathon-in-oslo-29-30-august-1d8ec54a26ad) (Oslo)
- Sep 2-16 - [Decentraland SDK virtual hackathon](https://hack.decentraland.org/?with=weekinethereum) (250k USD in prizes. There’s a referral code on that link that gets both you and me something extra)
- Sep 3 - Deadline to [apply for EU Horizon Prize](https://ec.europa.eu/info/funding-tenders/opportunities/portal/screen/opportunities/topic-details/blockchain-eicprize-2019). 1m € each to 5 "Blockchains for Social Good" projects
- Sep 6-8 - [ETHBoston](https://eth.boston/)
- Sep 15 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff/)
- Sep 15 - [Ethereal Tel Aviv](https://etherealsummit.com/events/ethereal-tel-aviv/)
- **Sep 16 - [Tachyon accelerator application](https://labs.consensys.net/tachyon/) deadline**
- Sep 15-16- [StarkWare sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- Sep 22 - [IDEO virtual hackathon](https://coinlist.co/build/ideo) ends
- Oct 7 - [ENS workshop](https://medium.com/the-ethereum-name-service/ens-workshop-applications-are-now-open-f46db6c63384) (Osaka)
- Oct 8-11 - [DeVcon](https://devcon.org/) (Osaka) **and [Devcon social events calendar](http://osaka.kickback.events/events/)**
- **Nov 8-10 - [ETHWaterloo](https://ethwaterloo.com/)**

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I own 100% Week In Ethereum. Editorial control has always been me.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **This headline stays as long as so many people continue to link to old URL and not the right one: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [](https://weekinethereumnews.com/week-in-ethereum-news-august-10-2019/)[https://weekinethereumnews.com/week-in-ethereum-news-august-10-2019/](https://weekinethereumnews.com/week-in-ethereum-news-august-10-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

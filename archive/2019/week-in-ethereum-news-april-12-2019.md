---
title: "April 12, 2019"
date: "2019-04-13"
---

## **Ethereum News and Links**

**Layer 1**

- [Prysmatic eth2 dev update](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-25-prysmatic-labs-5322a7762bba) - faster processing, multi-validators per machine, much more
- Akhunov: [Estimation of the size of contracts](https://medium.com/@akhounov/estimation-approximate-of-the-size-of-contracst-in-ethereum-4642fe92d6fe)
- Phase one and done: [eth2 as data availability engine](https://ethresear.ch/t/phase-one-and-done-eth2-as-a-data-availability-engine/5269) from Casey Detrio
- The Inspector: [An efficient finality test for CBC Casper](http://hackingresear.ch/cbc-inspector/)

**Stuff for developers**

- [websnark: fast zkSnarks generation](https://www.iden3.io/post/websnark-zksnarks-generation-browser-now-fast-and-easy) in the browser. 50k constraint proof in under 10 seconds
- [ZoKrates v0.4.4](https://medium.com/zokrates/building-identity-linked-zksnarks-with-zokrates-a36085cdd40) - building identity-based snarks. adds BabyJubJub
- [ZEXE on Plasma](https://devpost.com/software/zexe-on-ethereum) from Edcon hackathon
- [Developing Eth games with Enjin](https://www.youtube.com/watch?v=cw24ySJoGYk&feature=youtu.be) - video live demo
- Easily [embed a Status chat room](https://github.com/status-im/status-chat-widget) in your website
- “[Drop in solution for building Ethereum dApps in React](https://github.com/NoahZinsmeister/web3-react)” with support for all the web3 providers
- [Buidler, beta 4](https://medium.com/nomic-labs-blog/buidler-beta-4-new-solhint-solpp-plugins-2ab676395d29)
- [Truffle Teams](https://truffleframework.com/teams), zero-configuration continuous integration for Eth code
- Truffle [v5.0.12](https://github.com/trufflesuite/truffle/releases/tag/v5.0.12)

**Client releases**

- [Geth v1.8.26](https://github.com/ethereum/go-ethereum/releases/tag/v1.8.26)
- [Parity v2.5.0-beta](https://github.com/paritytech/parity-ethereum/releases/tag/v2.5.0) and [v2.4.5-stable](https://github.com/paritytech/parity-ethereum/releases/tag/v2.4.5)
- Pantheon too - link in enterprise

**Ecosystem**

- Opera on desktop now comes with [native web3 support and Eth wallet](https://blogs.opera.com/desktop/2019/04/opera-60-reborn-3- -3-0-vpn-ad-blocker/)
- [Parity’s Fether](https://medium.com/paritytech/parity-fether-is-on-ethereum-mainnet-105ed0c7b491) light client desktop wallet in beta on mainnet
- What [Status learned from Chaos Unicorn Day](https://our.status.im/chaos-unicorn-day-what-we-learned-by-breaking-status/) when it turned off Infura/Etherscan
- Marc-André Dumas turned his [full node into an archive node](https://medium.com/@marcandrdumas/are-ethereum-full-nodes-really-full-an-experiment-b77acd086ca7) using a low-end PC
- [VIPnode incentive layer to run Dappnode](https://medium.com/dappnode/vipnode-x-dappnode-d1d4ab55fa42)
- proof of concept for [messaging using Swarm, PSS and Feeds](https://discuss.status.im/t/hello-staples-swarm-pss-feeds-poc-for-buidlweek/1166)
- Quantstamp writeup of their [EthDenver VDF randomness simulation](https://quantstamp.com/blog/presenting-quantstamps-ethdenver-beacon-chain-implementation)
- Onboarding people with Austin Griffith: [Emojicoin exchange](https://medium.com/gitcoin/emojicoin-exchange-53f9658c9e3b). Also Amy Jung’s writeup of her experience [onboarding her friends with a Burner Wallet Party](https://medium.com/@sharedrealities/burn-and-merge-onboarding-tidbits-from-a-burner-wallet-party-cd6e57f55d8)
- [Flash Boys](https://pdaian.com/flashboys2.pdf). Phil Daian, et al, paper on frontrunning argues that bad dex design may even provide miners with incentive to destabilize consensus. If you find academic papers to be dense, try Phil’s [tweetstorm](https://twitter.com/phildaian/status/1116155236433956865)

**Enterprise**

- Pantheon v[1.0.3](https://github.com/PegaSysEng/pantheon/releases/tag/1.0.3) with EEA permissioning and privacy standards

**Governance and Standards**

- Latest [core devs call](https://youtu.be/gfC92gQKKnI?t=959). [Agenda](https://github.com/ethereum/pm/issues/93) to follow along.
- A call for [Ethereum Foundation transparency](https://www.reddit.com/r/ethereum/comments/bbmjxm/a_call_for_basic_ethereum_foundation_transparency/)
- Aragon proposes that the Ethereum Foundation put some [Eth in an Aragon DAO](https://forum.aragon.org/t/ethdao-governance/747) to be spent through on-chain governance
- Proposal to [prohibit Aragon from spending money to work on Polkadot](https://forum.aragon.org/t/agp-42-keep-aragon-focused-on-ethereum-not-polkadot/795).
- Maker [stability fee vote on going to 11.5%](https://blog.makerdao.com/executive-vote-stability-fee-11-5/). Maker will also [revamp its board](https://blog.makerdao.com/upgrades-to-maker-ecosystem-foundation-structure/), which [Nikolai does not like](https://nikolai.fyi/2019-4-7-statement/).
- [ERC1925](https://github.com/ethereum/EIPs/pull/1925/files): zkSNARK verifier registry standard
- [EIP1930](https://github.com/wighawag/EIPs/blob/call_strict_gas/EIPS/eip-1930.md): Allows specification of a strict amount of gas for calls

**Application layer**

- [All about Augur v2](https://www.augur.net/blog/augur-v2/): adding Dai, invalid as a tradable outcome, use it or lose it in a fork, affiliate marketing support, and lots more. Code is ready for audit.
- Augur/0x sports frontend [BlitzPredict is live on Kovan](https://medium.com/@blitzpredict1/alpha-testnet-exchange-is-live-19a34a699ca4) testnet
- [Flux](https://medium.com/@fluxmarket/flux-derivatives-on-startups-69fdc683cfe2) - p2p derivatives on startups, so that you can short the next Theranos. Markets in everything!
- [DaiPrice](https://daiprice.info/). find the best price to buy Dai
- [Loopring v3 using snarks for app-specific rollup scalability](https://medium.com/loopring-protocol/loopring-protocol-3-0-zksnarks-for-scalability-845b35a8b75b)
- Ocean Protocol’s [Nile testnet](https://blog.oceanprotocol.com/a-dip-into-the-nile-beta-network-51afd6145b6c)
- [uPort v1.6](https://medium.com/uport/leading-the-way-to-a-better-ux-for-decentralized-identity-f3edcf8f959b)
- From LarvaLabs/Cryptopunks: [Autoglyphs](https://www.larvalabs.com/autoglyphs). Unlike CryptoPunks or CryptoKitties, the artwork lives on-chain. Interesting [interview with Matt and John](https://www.artnome.com/news/2019/4/08/autoglyphs-generative-art-born-on-the-blockchain).
- [Omisego - public alpha release](https://blog.omisego.network/public-alpha-announcement-6d1f0bede278) on Rinkeby, 2700 transactions per second so far.
- [Dharma](https://blog.dharma.io/experience-magical-internet-money-with-dharma-4f67eb694be0) launch with better UX to borrow/lend Eth or Dai

**Interviews, Podcasts, Videos, Talks** 

- Celer Network’s [Mo Dong](https://podcast.ethhub.io/celer-network-scaling-ethereum-via-layer-2-with-mo-dong) on Into the Ether
- Video of [EF research team press conference](https://www.youtube.com/watch?v=oeOcJeAOLeE) at Edcon
- Counterfactual’s [Nima Vaziri](https://medium.com/@TrustlessState/pov-crypto-episode-43-counterfactuals-playground-generalized-state-channels-w-nima-vaziri-15082e9f1803) on POV Crypto
- Matter’s [Alex Vlasov and Alex Gluchowski](https://www.zeroknowledge.fm/72) on Zero Knowledge
- [Simon de la Rouviere](http://epicenter.tv/282) on Epicenter

**Tokens / Business / Regulation**

- [New ZRX model](https://blog.0xproject.com/0x-roadmap-2019-part-4-proposal-for-stake-based-liquidity-incentive-52c16558df29): 0x to add small fee to order takers, market makers who stake ZRX receive liquidity reward
- [DeFi liquidity models](https://www.placeholder.vc/blog/2019/4/9/defi-liquidity-models): p2p v MMORPG v FPS
- [Augmented bonding curves](https://medium.com/giveth/deep-dive-augmented-bonding-curves-3f1f7c1fa751)
- [Short selling without counterparty using bonding curve](https://medium.com/bandprotocol/short-selling-without-counterparty-using-bonding-curve-c499e35c3dc2)
- Set Protocol planning to launch its [automatic managed portfolio tokens](https://medium.com/set-protocol/the-road-to-mainnet-ab4877b73066) in the next month
- France allows [life insurance and investment funds to own crypto](https://www.lesechos.fr/finance-marches/banque-assurances/exclusif-le-bitcoin-a-desormais-sa-place-dans-les-contrats-dassurance-vie-1008678)

**General**

- Joe Lubin: [Why Ethereum Will Become the Global Settlement Layer](https://media.consensys.net/joe-lubin-why-ethereum-will-become-the-global-settlement-layer-9b5f90d85be2)
- Vitalik comment on Reddit about [Ethereum progress](https://www.reddit.com/r/ethtrader/comments/bcl9mi/vitalik/eks94h6/)
- [Karl and Vitalik Edcon](https://www.youtube.com/watch?v=j7MeJionPMA) rap video. “This is what happens when you code a lot”
- Facebook is trying to [raise a billion to collateralize](https://twitter.com/nathanielpopper/status/1115331482384388098) the Zuck coin
- [Building on bulletproofs](https://medium.com/@cathieyun/building-on-bulletproofs-2faa58af0ba8)
- 2019 [IPFS roadmap](https://blog.ipfs.io/78-ipfs-2019-roadmap/)
- NEAR’s new [“Whale Fishing” sharding design](https://ethresear.ch/t/whale-fishing-a-new-sharding-design/5275)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- April 15-30 - Gitcoin/Microsoft [Ethereal virtual hackathon](https://medium.com/gitcoin/the-ethereal-hackathon-4f5dc2eb56d6)
- **April 16 - [RunEVM](https://runevm.com/) (Berlin)**
- April 17-18 - [Magicians Istanbul planning](https://ethereum-magicians.org/t/istanbul-eth1x-roadmap-planning-meeting-april-17th-18th-in-berlin/2899) (Berlin)
- Apr 19-21 - [ETHCapetown](http://ethcapetown.com/)
- Apr 29 - [Oslo Blockchain Day](https://osloblockchainday.no/)
- May 4 - [ENS Permanent Registrar](https://medium.com/the-ethereum-name-service/dns-permanent-registrar-and-hackathons-ens-development-summary-03-2019-401a30e6316d) launches
- May 9 - [Fluidity Summit](https://www.fluiditysummit.com/) (NYC)
- May 10-11 - [Ethereal](https://etherealsummit.com/?ref=weekinethereum) (NYC)
- May 16 - [Token Summit](http://tokensummit.com/) (NYC)
- May 17-19 - [ETHNewYork](http://ethnewyork.com/)
- May 17 - Deadline to accept [proposals for Instanbul upgrade](https://en.ethereum.wiki/roadmap/istanbul) fork
- May 23-25 - [Swarm Orange Summit](https://www.eventbrite.com/e/swarm-orange-summit-madrid-2019-tickets-57378034245) (Madrid)
- **May 27-28 - [EthCon Korea](https://ethcon.kr/) (Seoul)**
- June 22-24 - [Zcon1](https://www.zfnd.org/zcon/) (Split, Croatia)
- Aug 2-4 - [ETHIndia](https://ethindia.co/) (Bangalore)
- Aug 2-4 - [TruffleCon](https://www.truffleframework.com/trufflecon2019) (Redmond)
- Aug 21-23 - [Dappcon](https://dappcon.io/) (Berlin)
- Aug 23-25 - [ETHBerlin](https://ethberlinzwei.com/)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)

  
I own Week In Ethereum. Editorial control has always been 100% me. 

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **Update links to new URL: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/april-12-2019/](https://weekinethereumnews.com/april-12-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

---
title: "February 15, 2019"
date: "2019-02-16"
---

## **News and Links**

**Layer 1**

- \[eth1\] Alexey: [state fees proposal 3](https://ethresear.ch/t/state-fees-formerly-state-rent-pre-eip-proposal-version-3/4996)
- \[eth2\] [Phase 0 and phase 1 spec v0.3](https://github.com/ethereum/eth2.0-specs/releases/tag/v0.3.0)
- \[eth2\] Overview of [Eth2 networking](https://medium.com/@mikerahqc/networking-in-serenity-eth2-0-8bbdb5bd6dd4) particularly important for phase 1
- \[eth2\] [Vitalik](https://github.com/ethereum/pm/blob/872f32493c898555a4e8a6362302ced51f28c8f9/All%20Core%20Devs%20Meetings/Meeting%2055.md): “we should not fall into the mindset of thinking that first Phase 0 gets done then Phase 1 gets done then Phase 2 gets done without working a lot of work between them in parallel. Because if we don't parallelize then we are going to take them to 2021 or whatever the trolls are saying.”
- \[eth2\] Vitalik: [phase 2 pre-spec: cross-shard mechanics](https://ethresear.ch/t/phase-2-pre-spec-cross-shard-mechanics/4970)
- \[eth2\] Latest [Eth2 implementers call](https://www.youtube.com/watch?v=p1qHM2B8cGc). [Agenda](https://github.com/ethereum/eth2.0-pm/issues/29) to follow along.
- \[eth2\] [Prysmatic Labs update](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-22-prysmatic-labs-b5b88ace0441): Beacon Chain testnet successfully deployed with 8 local validators through a Görli testnet kickstart
- \[eth2\] Parity’s [Shasper client short-lived testnet](https://github.com/paritytech/shasper/wiki/Shasper-Testnet-Plans)
- \[eth2\] [Lodestar dev update](https://medium.com/chainsafe-systems/lodestar-bi-weekly-update-2-e93ad5072159)

**Plasma**

- LeapDAO [Plasma MoreVP](https://leapdao.org/blog/Plasma-Mainnet-Launched/) on mainnet, though not yet audited so beware when testing your ERC20 or 721 transfers.
- OmiseGo’s [Plasma MoreVP alpha release](https://blog.omisego.network/omisegos-alpha-release-ari-8419afade8a8). You can test it out by [playing Hoard’s Plasma Dog](https://ethdenverplasmadog.hoard.exchange/) on Rinkeby testnet and try to make the leaderboard.
- More LeapDAO: [EVM code on Plasma](https://leapdao.org/blog/Smart-Contracts-on-Plasma/) with Truebit-style computation verification games
- A Loom [Plasma Cash chain tutorial](https://hackernoon.com/solving-scalability-of-ethereum-through-loom-sidechains-tutorial-2837307d454)
- [Efficient RSA accumulator proof generation for Plasma Prime](https://ethresear.ch/t/towards-efficient-rsa-accumulator-proof-generation-plasma-prime/4972)

**State channels**

- [Celer releases new version of Gomoku](https://medium.com/celer-network/celer-network-24th-weekly-project-progress-report-2-11-2-15-72f120b5e420) on state channels, complete with weekly ETH prizes for the top players on the leaderboard.
- [Raiden Network explainer](https://medium.com/raiden-network/raiden-protocol-explained-489b429fcd90)
- Magmo releases [TicTacToe demo of the ForceMove state channels](https://medium.com/magmo/introducing-our-second-state-channel-app-aab42cea36a4) protocol
- PISA: [State channels with optimistic contracts](https://medium.com/pisa-research/state-channels-with-state-assertions-b182ae939212), which improves gas cost in the worst case, but assumes participants are online

**Client releases - get ready for the fork!**

- Parity [v2.3.3-beta](https://github.com/paritytech/parity-ethereum/releases/tag/v2.3.3) or [2.2.10-stable](https://github.com/paritytech/parity-ethereum/releases/tag/v2.2.10). Everyone should update now as scope of JSONRPC bug was wider than previously known.

**Stuff for developers**

- Solidity [v0.5.4](https://github.com/ethereum/solidity/releases/tag/v0.5.4)
- [Slither v0.6](https://github.com/trailofbits/slither/releases/tag/0.6.0) - latest version of Trail of Bits security tool
- [ZeppelinOS v2.2](https://github.com/zeppelinos/zos/releases/tag/v2.2.0). Also: [getting started with Zepkit](https://blog.zeppelinos.org/getting-started-with-zepkit/?utm_campaign=evanconnect&utm_medium=wi&utm_source=weekinethereum).
- Manuel Araoz: coding [scarce digital goods with life, death, and healing](https://maraoz.com/2019/02/11/digital-life/)
- TypeScript [Merkle tree with Solidity proof verifier](https://github.com/liamzebedee/typescript-solidity-merkle-tree)
- BokkyPooBah's [Gas-Efficient DateTime Library v1.01](https://github.com/bokkypoobah/BokkyPooBahsDateTimeLibrary/releases/tag/v1.01)
- [Etherlime adds debugger](https://medium.com/limechain/etherlime-debugger-is-here-to-unravel-transactions-d628a4e6686)
- ConsenSys’ [dev tools list](https://github.com/ConsenSys/ethereum-developer-tools-list) is now a comprehensive reference
- Mudit Gupta’s list of [tips to save gas in Solidity](https://blog.polymath.network/solidity-tips-and-tricks-to-save-gas-and-reduce-bytecode-size-c44580b218e6)
- Loom [giving away packs to devs building on Zombie Battleground](https://medium.com/loom-network/https-medium-com-loom-network-introducing-zombie-battleground-public-api-600-pack-giveaway-859fea0dc406) API
- Infura releases a [devp2p analysis tool](https://github.com/infura/devp2p-network) with PostgresDB and Metabase
- Uport’s [EthTypedData Javascript library](https://medium.com/uport/simplifying-typed-data-for-ethereum-915a72d576c3) to create, sign and verify Structure Types and EIP712 domains
- The code [architecture of Etherisc’s insurance framework](https://blog.etherisc.com/gif-smart-contracts-architecture-808ff31d0ba3)
- [Trick block explorers](https://medium.com/consensys-diligence/poison-block-explorer-byte-code-bcf034a5d132) into displaying the wrong byte code
- Tutorial: [Instagram dapp clone with Vue.js and IPFS](https://medium.com/openberry/https-medium-com-creating-an-instagram-like-dapp-with-ipfs-cc4fac85cbfe)
- Tutorial: [code your own confidential token with AZTEC](https://paulrberg.com/post/2019/02/15/confidential-tokens/) protocol
- Embark tutorial: [building a decentralized Reddit, pt2](https://embark.status.im/news/2019/02/11/building-a-decentralized-reddit-with-embark-part-2/)
- Constantinople isn’t being delayed due to CREATE2, but it should be understood. “Indeterminacy in init code needs to be viewed the same way as indeterminacy in normal code, via DELEGATECALL or CALLCODE.” Here’s [Jeff Coleman’s tweetstorm](https://twitter.com/technocrypto/status/1095854769183358976) with a tl;dr of “switch to CREATE2 as soon as possible.” Here’s [Jason Carver’s article and Reddit comment thread](https://www.reddit.com/r/ethereum/comments/aqb8yg/defend_against_wild_magic_in_the_next_ethereum/).

**Ecosystem**

- [Etherscan revamps its UI](https://medium.com/etherscan-blog/the-revamp-on-etherscan-io-dark-mode-additional-features-8e504c6d9725), adds Görli, and now you can verify Vyper code, plus more charts on gigabytes needed for Geth/Parity full/archive
- [0x & Coinlist hackathon winners](https://medium.com/coinlist/announcing-the-winners-of-the-0x-coinlist-hackathon-c4bc8ff4f79d)
- Enigma examines [dead man’s switch](https://blog.enigma.co/tell-no-tales-decentralizing-a-dead-mans-switch-6217e2f4361b) options
- [Vipnode v2](https://medium.com/vipnode/vipnode-2-0-released-9af1d65b4552)
- [MyEtherWallet v5](https://medium.com/myetherwallet/lets-make-it-official-mew-v5-myetherwallet-s-all-new-interface-is-here-2063117180a4)

**Enterprise**

- JPMorgan says it “[became the first U.S. bank to create](https://www.jpmorgan.com/global/news/digital-coin-payments) and successfully test a digital coin representing a fiat currency” running on Quorum, its Geth fork. Although [“first” might be a stretch](https://twitter.com/ConsenSysAndrew/status/1096054929901449216).
- [Enterprise Ethereum Alliance to form “token working group”](https://www.coindesk.com/enterprise-ethereum-alliance-is-forming-a-token-task-force)

**Governance and Standards**

- Latest [core devs call](https://www.youtube.com/watch?v=NUz9_SpG84g). [Notes](https://github.com/ethereum/pm/blob/872f32493c898555a4e8a6362302ced51f28c8f9/All%20Core%20Devs%20Meetings/Meeting%2055.md) to follow along. Discussion of testnet fork, CREATE2 education, difficulty of finding a ProgPOW auditor, how to use phase 0 to finalize the eth1 chain, and that phase2 spec work will parallel implementation of phases 0 and 1.
- In case you heard crypto media disinformation: [Constantinople has not been postponed again](https://twitter.com/hudsonjameson/status/1095430004182302720). The Augur market used as [evidence for the disinfo is based on date](https://www.reddit.com/r/ethereum/comments/apsp5x/augur_bets_on_ethereum_constantinople_delay_after/egb5gq6/?context=3), so the market is mainly pricing how fast blocks happen.
- ProgPoW signals: miners [can use extra-data field](https://twitter.com/5chdn/status/1095221531125448705?s=21). There’s also a [Carbonvote](http://www.progpowcarbonvote.com/). Personally I think these signaling exercises are a bit premature.
- TechCrunch overview of [Melon Council governance](https://techcrunch.com/2019/02/11/melonport-dissolves-in-favor-of-its-protocol-setting-a-new-bar-for-the-blockchain-world/) of Melonport
- 0x to vote on enabling [ZEIP23’s bundles of assets](https://blog.0xproject.com/zeip-23-trade-bundles-of-assets-fe69eb3ed960)
- Danny Ryan: “[Ethereum is strong because of abundant, world-class leadership](https://twitter.com/dannyryan/status/1094796259762700288).”
- [Phil Daian](https://a16z.com/2019/02/09/voting-blockchains-governance-security-cryptoeconomics/) with Ali Yahya talking voting on the a16z podcast
- [Chris Burniske, Joel Monegro, Denis Nazarov, and Jesse Walden](https://a16z.com/2019/02/11/cryptonetworks-economies-governance-capital-access-risk-capital/) debate crypto governance, also on the a16z podcast

**Application layer**

- [Dharma Lever](https://blog.dharma.io/the-new-dharma-lever-has-arrived-b13b9bcd6d3b) collateralized lending and borrowing launches to private alpha
- [Pixura Platform](https://medium.com/pixura/pixura-platform-is-live-b404cb920765) mainnet beta release. Create NFTs with a public marketplace.
- [Status Keycard](https://our.status.im/introducing-keycard-the-open-secure-contactless-hardwallet/amp/): contactless hardwallet and API, available for free to first 1000 devs. Also: [Status v0.9.33](https://our.status.im/0-9-33/)
- [World’s Fair](https://www.reddit.com/r/ethereum/comments/apbx7x/i_created_a_decentralized_application_on_based_on/): an attempt at a decentralized Patreon, live on Rinkeby testnet
- [Molecule](https://medium.com/molecule-blog/hello-world-hello-molecules-a25929bd3ebe) - curation markets for early stage pharma

**Interviews, Podcasts, Videos, Talks** 

- [Dan Robinson](https://thebitcoinpodcast.com/hashing-it-out-36/) on why HTLCs suck on Hashing It Out
- [Berlin Eth meetup January vids](https://www.youtube.com/watch?v=qOXfVgDRVzY&list=PLaM7G4Llrb7zbd_2PP0ZgXh3eXSoj0u4A): Chainsafe, Parity’s Shasper, and Quantstamp
- [Jenna Zenk](https://www.zeroknowledge.fm/64) on Zero Knowledge
- [Georgios Konstantopoulos](https://www.youtube.com/watch?v=EHqkA5wX5so&feature=youtu.be) talks Plasma Cash with NEAR
- Melonport [M1 conference talks](https://www.youtube.com/playlist?list=PLzdnEGRLbpgZrywI9gc9ZLrZRo8FKoNir)
- [Nadav Hollander](https://podcast.ethhub.io/lending-on-ethereum-nadav-hollander-of-dharma) on Into the Ether
- [Alexey Akhunov](https://epicenter.tv/episode/274/) on Epicenter

**Tokens / Business / Regulation**

- [Understanding Uniswap returns](https://medium.com/@pintail/understanding-uniswap-returns-cc593f3499ef)
- A look at [FOAM incentives](https://blog.foam.space/a-closer-look-at-challenges-and-incentives-on-the-foam-map-a8b2dac47538)
- de la Rouviere: [Verified Curation Markets & Graduating Token Bonding Curves](https://medium.com/@simondlr/verified-curation-markets-graduating-token-bonding-curves-b3885cd1108)
- Front-running resistant [batched bonding curves](https://medium.com/@billyrennekamp/batched-bonding-curves-ce69a57d8ae4)
- CFTC Commish Quintenz sings a much [more pro-innovation tune](https://coincenter.org/entry/how-the-cftc-can-take-a-pro-innovation-posture-while-maintaining-orderly-markets): “more work remains to be done to establish regulatory clarity.”  
    

**General**

- [SendCrypto bot works on Twitter](https://www.reddit.com/r/ethereum/comments/ap7opc/sendcrypto_bot_send_crypto_tips_and_payments_on/)
- Filecoin [open sources](https://filecoin.io/blog/opening-filecoin-project-repos/) its repos
- [Cosmos to launch mainnet](https://blog.cosmos.network/cosmos-hub-to-launch-mainnet-a453d2247a34) in a matter of weeks
- Coinbase Wallet offering [optional encrypted cloud backup of private keys](https://blog.coinbase.com/backup-your-private-keys-on-google-drive-and-icloud-with-coinbase-wallet-3c3f3fdc86dc)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Feb 15-17 - [ETHDenver](https://www.ethdenver.com/) hackathon (ETHGlobal) 
- **Feb 18 - [ZEIP23 vote](https://blog.0xproject.com/zeip-23-trade-bundles-of-assets-fe69eb3ed960) with ZRX**
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
- **May 9 - [Fluidity Summit](https://www.fluiditysummit.com/) (NYC)**
- May 10-11 - [Ethereal](https://etherealsummit.com/?ref=weekinethereum) (NYC)
- May 17 - Deadline to accept [proposals for Instanbul upgrade](https://en.ethereum.wiki/roadmap/istanbul) fork
- **June 22-24 - [Zcon1](https://www.zfnd.org/zcon/) (Split, Croatia)**

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)

  
I own Week In Ethereum. Editorial control has always been 100% me. 

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **Update links to new URL: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it:  [](https://weekinethereumnews.com/february-15-2019/)[https://weekinethereumnews.com/february-15-2019/](https://weekinethereumnews.com/february-15-2019/)

Cent link for the night view:  [](https://beta.cent.co/+63r2dn)[https://beta.cent.co/+63r2dn](https://beta.cent.co/+63r2dn)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

---
title: "March 29, 2019"
date: "2019-03-30"
---

## **Ethereum News and Links**

**Layer 1**

- Latest [What’s New in Eth2](https://notes.ethereum.org/c/Sk8Zs--CQ/https%3A%2F%2Fbenjaminion.xyz%2Fnewineth2%2F20190329.html). “I would never have imagined just nine months ago . . . that in such a brief time so much would be accomplished.”
- Nimbus eth2 [testnet is running](https://our.status.im/the-nimbus-mvp-testnet-is-here/)!
- Prysmatic Labs is “on the [brink of our public testnet release](https://medium.com/prysmatic-labs/ethereum-2-0-serenity-testnet-update-closer-than-ever-259cace9a1b1).” Lighthouse also says they will have a [testnet any day now](https://twitter.com/ethZed/status/1111499764418240512).
- Latest [Eth2 implementers call](https://www.youtube.com/watch?v=bC4v_a-gcrs). [Agenda](https://github.com/ethereum/eth2.0-pm/issues/35) to follow along.
- [Eth2 will use SHA256](https://github.com/ethereum/eth2.0-specs/pull/779)
- The [actor model and inter-shard communication](https://medium.com/spadebuilders/actor-factor-2b0005fde786). Related: Dan Finlay on [Ethereum object capabilities](https://ethereum-magicians.org/t/ethereum-object-capabilities/3035/1)
- Sergio Lerner proposes [Unitries](https://ethereum-magicians.org/t/unitrie-a-replacement-of-the-state-trie-in-eth-1-0-or-2-0/2958) for eth1 and/or eth2
- Akhunov: [data from the Ethereum stateless prototype](https://medium.com/@akhounov/data-from-the-ethereum-stateless-prototype-8c69479c8abc)
- [EVM stats by opcode](https://github.com/holiman/vmstats/blob/master/README.md) time from Martin Swende. relevant to eip1884

**Layer 2**

- Plasma Group: [understanding the generalized plasma architecture](https://medium.com/plasma-group/plapps-and-predicates-understanding-the-generalized-plasma-architecture-fc171b25741)
- [Dai on Plasma Leap](https://leapdao.org/blog/DAI-enabled-as-Plasma-Asset/)
- [Another simple exit game implementation for Plasma cashflow construction](https://ethresear.ch/t/another-simple-exit-game-implementation-for-plasma-cashflow-construction/5207)
- [POANetwork -> POSDAO](https://forum.poa.network/t/posdao-white-paper/2208) with HoneyBadgerBFT?
- [Penalties and conserved quantities in state channels](https://ethresear.ch/t/penalties-and-conserved-quantities-in-state-channels/5225)

**Stuff for developers**

- The experimental [ABIEncoderv2 had a bug,](https://blog.ethereum.org/2019/03/26/solidity-optimizer-and-abiencoderv2-bug/) so make sure to update to [Solidity v0.5.7](https://github.com/ethereum/solidity/releases/tag/v0.5.7)
- Truffle [v5.0.10](https://github.com/trufflesuite/truffle/releases/tag/v5.0.10)
- [Testing time dependent Solidity code](https://medium.com/fluidity/standing-the-time-of-test-b906fcc374a9) with Truffle and Ganache
- Overview of [ConsenSys Diligence’s security tools](https://medium.com/consensys-diligence/all-ethereum-security-tools-built-by-consensys-diligence-dd918248f978)
- A [simple GUI for compiling and interacting](https://github.com/ssteiger/Vyper-contract-GUI) with your Vyper code
- Infura [Websocket API upgrade](https://blog.infura.io/websocket-api-upgrade-now-live-e3406cc70d14)
- [Cava](https://medium.com/@furkankamaci/consensyss-cava-as-apache-tuweni-82bf8d755f82) - Java/JVM libraries to aid web3 devs - accepted into Apache Incubator Project as Apache Tuweni
- [Fluence devnet launches](https://medium.com/fluence-network/fluence-project-update-february-march-2019-b69a3e376ba4) to use a “decentralized SQL database app” using Ethereum and Swarm
- 3Box [decentralized comments API](https://medium.com/3box/3box-decentralized-comments-api-7e495d2ddd24)

**Client release**

- Parity v[2.4.3-beta](https://github.com/paritytech/parity-ethereum/releases/tag/v2.4.3) and v[2.3.8-stable](https://github.com/paritytech/parity-ethereum/releases/tag/v2.3.8)
- Pantheon [v1.0.2](https://github.com/PegaSysEng/pantheon/releases/tag/1.0.2)
- [EthereumJS VM v3](https://www.reddit.com/r/ethereum/comments/b79k5x/ethereumjs_vm_v300_stack_memory_refactoring_es6/)
- [EthArmbian and EthRaspian](https://www.reddit.com/r/ethereum/comments/b67bwh/ethereum_on_arm_raspberry_pi_image_ethraspbian_is/) custom Linux images update. Includes Swarm, IPFS, Raiden, and Status. The Status node will be useful on April 1st when Status is going to [turn off Infura for a day](https://our.status.im/bulletproofing-against-chaos-unicorns-with-status-on-arm/).

**Ecosystem**

- Virgil Griffith: [Ethereum is game-changing technology, literally](https://medium.com/@virgilgr/ethereum-is-game-changing-technology-literally-d67e01a01cf8). Ethereum changes many of the assumptions of game theory
- [0x Mesh](https://blog.0xproject.com/0x-roadmap-2019-part-3-networked-liquidity-0x-mesh-9a24026202b3): p2p order sharing network, planned for end of q2. [Remco](https://twitter.com/recmo/status/1111122952798388224): “extending libp2p with WebRTC support and compilation to WebAssembly. You will be able to run a full node in a browser”
- [Polaris oracle](https://medium.com/@mykelp/introducing-polaris-ced195dd798e) using the median of the last 15 Uniswap prices, with some incentives to help maintain the price checkpoints.

**Live on mainnet**

- UMA put a [synthetic index of US large cap equity](https://medium.com/uma-project/announcing-us-stock-index-token-powered-by-uma-and-dai-c394586c575a) on mainnet. Get exposure to US equity from anywhere in the world

**Enterprise**

- “Perutnina Ptuj, the largest poultry producer in Southeastern Europe, just launched” [provenance app using OriginTrail](https://medium.com/origintrail/new-poultry-provenance-consumer-app-powered-by-origintrail-ed9909d4d20d)
- Louis Vuitton to launch in a few months a [private chain using Quorum for authenticating luxury goods](https://www.coindesk.com/louis-vuitton-owner-lvmh-is-launching-a-blockchain-to-track-luxury-goods)

**Governance and Standards**

- Latest [core devs call](https://youtu.be/v8Psbo8zY4Y?t=276). [Agenda](https://github.com/ethereum/pm/issues/89) to follow along, or use [Tim Beiko’s contemporaneous tweets](https://twitter.com/TimBeiko/status/1106557410779512832) of the call
- A result of the call: [motion to require an audit for ProgPoW](https://ethereum-magicians.org/t/motion-to-not-include-progpow-without-audit/3027)
- [ProgPoW audit: goals & expectations](https://medium.com/ethereum-cat-herders/progpow-audit-goals-expectations-75bb902a1f01)
- Jean Cyr’s “[technical take on ProgPoW’s weakest link](https://ethereum-magicians.org/t/my-technical-take-on-progpows-weakest-link/2983)”
- Martin Swende on why [he supports ProgPoW](http://swende.se/blog/Progpow.html). Some [ProgPoW benchmarking](https://medium.com/@infantry1337/comprehensive-progpow-benchmark-715126798476?sk=8acbe3fb45ef704a20dc09c87a5890a8)
- [ProgPoW from an IC Design Engineer](https://ether4life.tumblr.com/post/183604547634/progpow-ic-asic-design-engineer-view)’s perspective which echoes [Alexey Akhunov’s perspective](https://medium.com/@akhounov/on-agile-hardware-development-bd1b9ceb44d) that ProgPoW will not be very ASIC resistant. [IfDefElse response](https://medium.com/@ifdefelse/the-cost-of-asic-design-a44f9a065b72). Also check out all of [IfDefElse’s responses](https://ethereum-magicians.org/t/progpow-a-compilation-of-reference-material/3040).
- Linzhi: [Open Chip Design for 1% cost/power increase](https://medium.com/@Linzhi/eip-1057-progpow-open-chip-design-for-only-1-cost-power-increase-eip-1057-progpow-d106d9baa6eb).
- [EIP1872](https://github.com/ethereum/EIPs/pull/1872/files): Network upgrade timeframes
- [ERC1882](https://github.com/ethereum/EIPs/issues/1882): Decentralized type system for EVM
- [EIP1884](https://github.com/ethereum/EIPs/pull/1884): reprice opcodes

**Application layer**

- [bZx Fulcrum](https://medium.com/bzxnetwork/introducing-fulcrum-tokenized-margin-made-dead-simple-e65ccc82393f) tokenized margin lending and trading using Kyber price feed. Live in early April.
- [Polaris oracle](https://medium.com/@mykelp/introducing-polaris-ced195dd798e) using the median of the last 15 Uniswap prices, with some incentives to help maintain the price checkpoints.
- Healthereum’s [beta launched](https://www.mobihealthnews.com/content/blockchain-platform-healthereum-life-portfolio-incentivizes-appointment-adherence-tokens) “to curb doctor’s appointments no-shows with redeemable incentives”
- Update on the [DutchX DAI/ETH auctions](https://www.reddit.com/r/ethereum/comments/b6k1ga/the_dutchx_a_price_finding_tool_with_more/)
- Giveth is [aiming to “create continuous streams of funding](https://medium.com/giveth/the-future-of-giving-is-crowdfunding-the-commons-ac265e3010b8) through the creation of economies around causes, by building a system of token bonding curves feeding cause-focused DAOs” on Giveth
- [Aragon Court v1](https://forum.aragon.org/t/aragon-court-v1/691). Related: the [Kleros TCR appeal system](https://blog.kleros.io/kleros-decentralized-token-listing-appeal-fees/)
- FunFair goes live with the [first licensed blockchain casino game](https://funfair.io/alice-cooper-rocks-the-blockchain-in-our-latest-launch/), themed on Alice Cooper’s School’s Out
- [Ching Dai point of sale system](https://medium.com/ching/ching-is-in-open-beta-6b99507b4d5c) in open beta
- MLB Champions (fka MLB Crypto) 2019 [draft is live](https://medium.com/mlb-champions/mlb-champions-introducing-packs-and-season-passes-9a829478a1c9)
- UjoMusic [streaming payments using Connext’s Dai payment channels](https://media.consensys.net/introducing-streaming-payments-for-ujo-with-connext-payment-channels-and-dai-16725929fe38)

**Interviews, Podcasts, Videos, Talks** 

- Counterfactual’s [Liam Horne](https://thebitcoinpodcast.com/hashing-it-out-40/) on Hashing It Out
- Maker’s Rune Christensen on [Into the Ether](https://podcast.ethhub.io/maker-establishing-stability-in-crypto-with-rune-christensen) and [Zero Knowledge](https://www.zeroknowledge.fm/70)
- All [EthParis videos](https://www.youtube.com/channel/UCfF9ZO8Ug4xk_AJd4aeT5HA/videos)
- Kobe van Reppelen started an Ethtrader profiles series with [Jeremiah Nichol](https://www.youtube.com/watch?v=6I2rDQCF7Fs&index=3&list=PLTzbA2lLaEj3O0PiYVP9p-YS3PoF_Le8L), [Vitalik Buterin](https://www.youtube.com/watch?v=e3vxt6l7ATw) and [Ameen Soleimani](https://www.youtube.com/watch?v=EopG76BU9hE)
- All [AraCon videos](https://www.youtube.com/playlist?list=PLdbM67oXoBoaAhNLWHj_lJNkoXH_Jqkk2)
- All [Zero Knowledge Summit videos](https://www.youtube.com/watch?v=DfEG5nhMRyQ&list=PLj80z0cJm8QHvg1ydi6rTEUK1SpxbtKnM)

**Tokens / Business / Regulation**

- [Worklock](https://blog.nucypher.com/the-worklock/) from NuCypher. Lockup your ETH for NuCypher tokens, if you do work, then you get your ETH back. Otherwise, the ETH gets burned.
- [ConsenSys is working with Satis Group](https://content.consensys.net/wp-content/uploads/CS_Satis-Press-Release.pdf) on security token offerings (pdf link)
- Gitcoin is adding a [10% bounty platform fee](https://medium.com/gitcoin/a-gitcoin-platform-fee-905a0507961f).

**General**

- Samsung Galaxy S10 apparently has a [crypto wallet only](https://decryptmedia.com/6129/samsung-galaxy-s10-crypto-wallet) in Germany, Korea and American versions.
- Trustology [launches TrustVault Personal Accounts](https://www.trustology.io/single-post/2019/03/27/Trustology-Launches-TrustVault-Personal-Accounts-in-the-UK-for-Managing-Cryptoassets) Ether custody for UK individuals in advance of offering it to financial institutions.
- Despite crypto media reports, [Omise flatly denies](https://twitter.com/Omise/status/1111878917629972482) that it has been acquired
- Starkware’s [STARK math, part 4](https://medium.com/starkware/low-degree-testing-f7614f5172db)
- Rachel O’Leary reports from [Kurdish Syria on crypto possibilities there](https://www.coindesk.com/sand-death-and-cryptocurrency-life-in-a-decentralized-syria)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- April 4-5 - [Deconomy](https://deconomy.com/seoul2019/) (Seoul)
- April 8-14 - [Edcon](https://www.edcon.io/) hackathon and conference (Sydney)
- April 15-30 - Gitcoin/Microsoft [Ethereal virtual hackathon](https://medium.com/gitcoin/the-ethereal-hackathon-4f5dc2eb56d6)
- April 17-18 - [Magicians Istanbul planning](https://ethereum-magicians.org/t/istanbul-eth1x-roadmap-planning-meeting-april-17th-18th-in-berlin/2899) (Berlin)
- Apr 19-21 - [ETHCapetown](http://ethcapetown.com/)
- Apr 29 - [Oslo Blockchain Day](https://osloblockchainday.no/)
- May 4 - [ENS Permanent Registrar](https://medium.com/the-ethereum-name-service/dns-permanent-registrar-and-hackathons-ens-development-summary-03-2019-401a30e6316d) launches
- May 9 - [Fluidity Summit](https://www.fluiditysummit.com/) (NYC)
- May 10-11 - [Ethereal](https://etherealsummit.com/?ref=weekinethereum) (NYC)
- May 16 - [Token Summit](http://tokensummit.com/) (NYC)
- May 17-19 - [ETHNewYork](http://ethnewyork.com/)
- May 17 - Deadline to accept [proposals for Instanbul upgrade](https://en.ethereum.wiki/roadmap/istanbul) fork
- May 23-25 - [Swarm Orange Summit](https://www.eventbrite.com/e/swarm-orange-summit-madrid-2019-tickets-57378034245) (Madrid)
- June 22-24 - [Zcon1](https://www.zfnd.org/zcon/) (Split, Croatia)
- **Aug 2-4 - [ETHIndia](https://ethindia.co/) (Bangalore)**

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)

  
I own Week In Ethereum. Editorial control has always been 100% me. 

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **Update links to new URL: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/ethereum-news-march-29-2019/](https://weekinethereumnews.com/ethereum-news-march-29-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

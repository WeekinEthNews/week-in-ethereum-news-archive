---
title: "Week in Eth News <BR> November 18, 2019"
date: "2019-11-18"
---

## **Eth News and Links**

**Eth1**

- Parity [v.2.5.10stable and v2.6.5beta](https://www.parity.io/release-parity-ethereum-goes-to-istanbul/). Ready for Istanbul, with some warp sync fixes in the beta release
- Trinity [v0.1.0-alpha.30](https://github.com/ethereum/trinity/releases/tag/v0.1.0-alpha.30), Istanbul-ready py-evm
- Aleth [v1.7](https://github.com/ethereum/aleth/releases/tag/v1.7.0), Istanbul ready
- Latest [core devs call](https://www.youtube.com/watch?v=3qZFiETlDtk). Notes [from call](https://twitter.com/TimBeiko/status/1195336502261272577)  
    

**Eth2**

- [Prysmatic client](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-39-prysmatic-labs-257d538d7f63) update. testnet relaunch, up to spec v0.9.1
- How [data availability affects light client](https://medium.com/@kimiwu/data-availability-on-ethereum-2-0-light-node-en-aec1ce6ac17c) design
- Devcon video on [developer experience in eth2](https://www.youtube.com/watch?v=0phnWn5ecyw&t=49m54s)  
    

**Layer2**

- [BLS rollup](https://skale.network/blog/introducing-bls-rollup/) on Skale  
    

**Stuff for developers**

- Solidity [v0.5.13](https://github.com/ethereum/solidity/releases/tag/v0.5.13). Istanbul-EVM compatible, more SMT, list overload candidates, export layout of storage variables, WIP ewasm-binary output
- Truffle [v5.1](https://github.com/trufflesuite/truffle/releases/tag/v5.1.0). ENS support, new data decoder, in-test debugging and better syntax highlighting while debugging
- web3.js [v1.2.4](https://github.com/ethereum/web3.js/releases/tag/v1.2.4) better Typescript type defs, out of gas bugfix
- Vyper [v0.1.beta14](https://vyper.readthedocs.io/en/latest/release-notes.html)
- How to [protect your contracts from re-entrancy after Istanbul](https://blog.openzeppelin.com/reentrancy-after-istanbul/)
- How Lucidity [dramatically reduced their Infura call volume](https://blog.infura.io/case-study-how-lucidity-optimized-their-infura-usage-to-save-time-and-money-a755f4ab4219) by caching its reads
- Aragon’s tips for winning the [struggle against contract size in the EVM](https://blog.aragon.one/rage-against-the-ev-machine-part-1/)
- Terminal’s [dapp monitoring platform](https://blog.terminal.co/introducing-terminals-dapp-monitoring-platform/)
- The [architecture of Dharma’s smart wallets](https://blog.dharma.io/why-smart-wallets-should-catch-your-interest-c85e4401b89a)
- Gonçalo Sá on [Solidity features in v0.5.13 and coming in v0.6](https://diligence.consensys.net/blog/2019/11/solidity-the-young-adult/)
- Slick interface to [buy Chainlink API data feeds](https://medium.com/clc-group/honeycomb-marketplace-101-for-ethereum-developers-c7c63c2d3049)  
    

**Ecosystem**

- Grants: [ConsenSys wave 2](https://consensys.net/blog/news/consensys-grants-wave-2-winners/), EF [Taiwan focused](https://blog.ethereum.org/2019/11/14/Announcing-a-Taiwan-specific-Wave/), MetaCartel [cohort 1](https://medium.com/metacartel/metacartel-cohort-1-6336cdca05db)
- Eric Conner’s [user guide to ENS domains](https://medium.com/@eric.conner/the-ultimate-guide-to-ens-names-aa541586067a)
- [ethereum.org update](https://blog.ethereum.org/2019/11/12/Ethereum.org-Development-Update-1/): adding the Studio web IDE, re-org’ing the format and Gitcoin bounties
- [Meson](https://hashcloak.com/blog/annoucements/Meson:%20A%20mixnet%20for%20ETH-based%20transactions/), a mixnet at the networking layer
- More [Devcon5 videos](https://www.youtube.com/channel/UCNOfzGXD_C9YMYmnefmPH0g/videos) are slowly trickling in  
    

**Enterprise**

- [Subscribing to events at scale](https://pegasys.tech/subscribing-to-events-at-scale-with-pegasys-plus/) by sending them to Kafka or Kinesis
- updated [uPort roadmap](https://medium.com/uport/connecting-and-building-trust-between-organizations-and-people-with-uport-serto-32ac6fffdc5e), mostly aimed at enterprise  
    

**Governance and standards**

- [ERC2362](https://github.com/ethereum/EIPs/blob/a8dc697723096094061522e06756138bd2f97400/EIPS/eip-draft_Pull_Oracle_Interface.md): Pull oracle interface
- Lessons learned from [establishing Hyperledger Besu’s maintenance process](https://www.hyperledger.org/blog/2019/11/07/best-practices-and-lessons-learned-from-hyperledger-besu-establishing-a-maintainer-process)
- [DisCOs](http://disco.coop/manifesto/): the p2p community’s alternative to DAOs
- Autark’s [“Open Enteprise” for Aragon](https://blog.autark.xyz/open-enterprise-mainnet/) is on mainnet. an “end-to-end suite of tools for management of open organizations”

**Application layer**

- [Brave v1](https://brave.com/brave-launches-next-generation-browser/). If you haven’t switched yet, I no longer even have the "slow new tab" problem. [Referral link](https://brave.com/wee307) (though my KYC is stuck and I can’t get my BAT!) I also enjoyed Brian Bondy’s [Brave founding story](https://brave.com/the-road-to-brave-one-dot-zero/). The best part is how they almost couldn’t connect by DM.
- You can [sell your browser data through Swash](https://swashapp.io/) browser extension and earn Streamr’s DATA token
- [Tokenizing open offers](https://medium.com/@rosscampbell9/tokenizing-open-offers-on-openlaw-and-ethereum-2a77dd8bb330) with OpenLaw
- [0x v3 passed and goes live Nov 25](https://blog.0xproject.com/0x-v3-vote-recap-upgrade-guide-f9299cd3aaea)
- Comparing [insurance-like solutions in DeFi](https://medium.com/@hugh_karp/comparing-insurance-like-solutions-in-defi-a804a6be6d48)
- A [taxonomy for LAOs](https://medium.com/@thelaoofficial/a-taxonomy-for-laos-making-sense-of-the-emerging-lao-ecosystem-1122b035fe1a) (DAOs with a legal entity)
- It’s multi-collateral Dai (MCD) launch day. One of the main reasons to switch is the [benefits of Dai Savings Rate](https://blog.makerdao.com/why-the-dai-savings-rate-is-a-game-changer-for-the-defi-ecosystem-and-beyond/). MCD also means revamped [Oasis dex](https://blog.makerdao.com/introducing-oasis-borrow-and-save/)

**Tokens / Business / Regulation**

- [Convexity protocol](https://drive.google.com/file/d/1YsrGBUpZoPvFLtcwkEYkxNhogWCU772D/view): ERC20 option tokens
- Chainlink on [embedding smart contracts into a legal fabric](https://blog.chain.link/embedding-smart-contracts-into-our-legal-fabric-2/)  
    

**General**

- [De-anonymization attacks from remote side channels](https://crypto.stanford.edu/timings/). Applicable to Monero and ZCash
- [Breaking Mimblewimble privacy](https://medium.com/dragonfly-research/breaking-mimblewimble-privacy-model-84bcd67bfe52) for $60 a week, “and I don’t believe there’s a way to fix it.”
- Mudit Gupta’s post on [problems with mixers](https://mudit.blog/mixers-are-insufficient/)
- Protests in Iran led to them [shutting off the internet](https://twitter.com/netblocks/status/1195775905907576832)
- You have 12 days to [register an Eth address to get tokenized r/ethtrader donuts](https://www.reddit.com/r/ethtrader/comments/dwiu4f/donutsonethereum_registration_is_open/)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Nov 18 - [Multi-collateral Dai](https://blog.makerdao.com/breaking-launch-date-of-multi-collateral-dai-announced-at-devcon-5/) launches
- **Dec 2-16 - Gitcoin [Global Communities virtual hackathon](https://hackathons.gitcoin.co/global-communities)**
- Dec 6 - [Istanbul network upgrade](https://ethernodes.org/istanbul)
- Jan 1 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff-update/)
- Jan 31 - deadline for [EU ledger 200k euro grants](https://fundingbox.com/spaces/ledger-ledger-news-and-updates/5dbfcb7d52317832f85906c8) for blockchain startups
- Feb 9-15 - [EthLagos](https://ethlagos.io/)
- Feb 14-16 - [ETHDenver](https://www.ethdenver.com/)
- Mar 3-5 - [EthCC](https://ethcc.io/) (Paris)
- **[Apr 3-7 - Edcon (Vienna)](https://www.edcon.io/)**

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

It’s amazing to me how many people email me when every issue has a link at the bottom saying not to email me to get in the newsletter.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **I want your links: [weekinethereumnews.com](https://weekinethereumnews.com/)**

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/week-in-eth-news-november-18-2019/](https://weekinethereumnews.com/week-in-eth-news-november-18-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

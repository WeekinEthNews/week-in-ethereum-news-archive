---
title: "March 1, 2019"
date: "2019-03-02"
---

## **Ethereum News and Links**

**Layer 1**

- \[eth1\] Constantinople is successful so far. [Eth issuance now comparable to BTC](https://twitter.com/RyanSAdams/status/1101227974051926018).
- \[eth2\] Eth2 [spec v0.4](https://github.com/ethereum/eth2.0-specs/releases/tag/0.4.0)
- \[eth2\] [phase 0 wire protocol](https://github.com/ethereum/eth2.0-specs/issues/692) from Matt Slipper
- \[eth2\] [Nimbus dev update](https://our.status.im/nimbus-development-update-feb-2019/) - testnet expected in March, network sim running
- \[eth2\] [Prysmatic dev update](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-23-prysmatic-labs-3d2d7cd7da8) - improving validator, attestation lifecycle, beacon node
- \[eth2\] [Lighthouse dev update](https://lighthouse.sigmaprime.io/update-08.html) - explains fork choice rules and some BLS basics
- \[eth2\] [Chainsafe dev update](https://medium.com/chainsafe-systems/lodestar-bi-weekly-update-3-9001f8d588aa) - “once merged all our state transitions will be implemented, this includes slot, block and epoch processing as well as the fork choice rule”
- \[eth2\] [eth2 implementers call](https://youtu.be/0ZWG8hMbxes?t=131). [Agenda](https://github.com/ethereum/eth2.0-pm/issues/31) to follow along.
- \[eth2\] Podcast: [Danny Ryan](https://www.zeroknowledge.fm/66) walks through Eth2 on Zero Knowledge. Also, Trent’s [notes](https://medium.com/@trenton.v/zero-knowledge-x-danny-ryan-e3526cf61210?sk=af56d7ebde0c3781ffc72643d1e82d6b) are very useful

**Client releases**

- [Pantheon v1 released](https://pegasys.tech/protecting-the-enterprise-permissioning-features-in-pantheon/). Written in Java, Apache2 licensed, enterprise-grade with permissioning and IBFT v2
- [Trinity v0.1.0-alpha.23 "Theodora"](https://github.com/ethereum/trinity/releases/tag/v0.1.0-alpha.23), includes Constantinople support

**Plasma and sidechains**

- Plasma Group: [toward a general purpose Plasma](https://medium.com/plasma-group/towards-a-general-purpose-plasma-f1cc4d49c1f4) to make it much easier for devs to write plasma apps.

**State channels**

- Magmo’s [Nitro Protocol paper](https://medium.com/magmo/nitro-protocol-c49b50f59df7) on n-party generalized state channel networks
- Three part video series from [Celer on how they solve the watchtower problem](https://www.youtube.com/watch?v=ofr9tRXTId0&list=PLXQx-6BZNAos4O9dgWeS-U8p-JTckGXQw)
- [Zk-channels: Private layer 2 payments on Ethereum](https://ethresear.ch/t/zk-channels-private-layer-2-payments-on-ethereum/5069)

**Stuff for developers**

- [Automate your Solidity workflow](https://medium.com/nomic-labs-blog/how-to-create-a-buidler-task-55658aa89aff) with Buidler
- [Solidity’s SMTChecker can automatically find real bugs](https://medium.com/@leonardoalt/soliditys-smtchecker-can-automatically-find-real-bugs-beb566c24dea)
- Truffle [v5.0.6](https://github.com/trufflesuite/truffle/releases/tag/v5.0.6) major debugger update
- [web3.js 1.0.0-beta.47](https://github.com/ethereum/web3.js/releases/tag/v1.0.0-beta.47)
- [Solidity implementation of elliptic curve secp256r1 / prime256v1 / p256](https://github.com/tdrerup/elliptic-curve-solidity)
- [Encoding and evaluating mathematical expression in Solidity](https://medium.com/bandprotocol/encoding-and-evaluating-mathematical-expression-in-solidity-f1bb062fa86e)
- 3box: [profile hovers](https://medium.com/3box/introducing-profile-hovers-30bae578459e) and [email verification service](https://medium.com/3box/launching-3box-email-verification-service-fc729981ec32)
- ConsenSysDiligence held a CTF, and [samczun cracked it fast](https://samczsun.com/consensys-ctf-writeup/)
- Maker [postmortem on Oasis upgrade](https://medium.com/makerdao/postmortem-oasis-contract-upgrade-71b11595976c)
- Perez, Livshits paper confirming that the sensationalist [“omg 21000 contracts are vulnerable” headline is nonsense](https://arxiv.org/pdf/1902.06710.pdf)
- [OpenLaw Elements](https://medium.com/@OpenLawOfficial/building-applications-faster-with-openlaw-the-release-of-openlaw-elements-8a0e29accf0c) - code to build and manage agreements for lending, IP, derivatives, etc
- [0x extensions](https://blog.0xproject.com/0x-extensions-enabling-new-types-of-exchange-1db0bf6125b6) for dutch auctions, whitelists, and forwarders
- Streamr [integration with IBM’s IoT Node-RED dev tool](https://medium.com/streamrblog/streamr-node-red-integration-tutorial-b0b410496354)
- Easy way to [claim .test ENS domains for testing](https://medium.com/the-ethereum-name-service/claim-test-ens-domain-for-easy-testing-1127e415c76d)

**Ecosystem**

- Upcoming [ENS root change for integration with 90% of TLDs](https://medium.com/the-ethereum-name-service/upcoming-changes-to-the-ens-root-a1b78fd52b38). Given that most of the unsupported TLDs are long-tail, that means ENS will support 99.99%+ domains. Also, ENS rewrote their [documentation](https://docs.ens.domains/)
- Alethio [investigates the four figure ETH transaction fees](https://medium.com/alethio/the-gas-fee-game-df9e0ce794f8) from last week. They think it is some kind of automation gone awry.
- User studies of [Parity’s Fether wallet](https://medium.com/@tbaut/fether-wallet-user-study-12b7ed966a01)
- More on the [Ethereum Cat Herders](https://medium.com/ethereum-cat-herders/further-introduction-the-ethereum-cat-herders-c42bf026fb7c)
- Public good funding: Moloch [processing memberships](https://twitter.com/MolochDAO/status/1100517160420397056) and starting with funding proposal. There’s also the [Gitcoin torch](https://docs.ethhub.io/other/gitcoin-torch/) that has 14000 DAI pledged to match donations to Gitcoin grants
- Step by step walkthrough of using Christian Lundkvist’s [simple multi-sig](https://medium.com/@alejandrodiaz_71295/simple-multisig-step-by-step-75429d9a4d61)
- RicMoo: Ethereum can [recover if quantum computing](https://blog.ricmoo.com/ethereum-post-quantum-recovery-dffc9ab0ca3e) were to ever break Ethereum

**Live on mainnet**

- [Melon v1](https://medium.com/melonport-blog/melon-v1-0-zahreddino-60105f51988d) released. capped at 5k/fund at UI level, bug bounties open.
- [Helena](https://media.consensys.net/helena-prediction-markets-platform-is-live-on-ethereum-mainnet-e2aef7b76777) - prediction market platform built on Gnosis. Industry insiders and obsessives participate in crypto-focused prediction markets, rewarded from bounty pools and eventually from subscription revenue.

**Enterprise**

- Pantheon released - see above in client releases section.
- Video on [i2i bank to bank transfers from UnionBank and ConsenSys](https://www.youtube.com/watch?v=E6US_fFxSMY) in the Philippines
- Alpine’s list of [enterprise projects making news](https://medium.com/alpineintel/alpine-private-key-1-payments-novel-platforms-and-a-flagship-phone-d3d03a5a2e67)
- Intel: [blockchain robots and the EEA Trusted Compute API](https://software.intel.com/en-us/blogs/2019/02/22/can-a-blockchain-controlled-robot-change-the-future?language=en)

**Governance and Standards**

- Latest [core devs call](https://www.youtube.com/watch?v=q3ylladkuYY). [Agenda](https://github.com/ethereum/pm/issues/82) to follow along.
- Proposed: [higher standards for EIPs](https://ethereum-magicians.org/t/higher-standards-for-eips/2781)
- [ERC1780](https://github.com/ethereum/EIPs/pull/1780/files): JSON-LD Contract Metadata for Semantic Web Ontologies
- [ERC1789](https://github.com/ethereum/EIPs/issues/1789): 20% of issuance dedicated to ecosystem development
- [ERC1803](https://github.com/ethereum/EIPs/pull/1803/files): Rename BALANCE, SHA3, GAS, NUMBER, GASLIMIT, and INVALID opcodes for clarity
- [EIP1805](https://github.com/ethereum/EIPs/pull/1805/files): Simple Streamable Serialize for network transport
- [ERC1775](https://github.com/ethereum/EIPs/pull/1775/files): App Keys, application specific wallet accounts. [FEM discussion](https://ethereum-magicians.org/t/eip-erc-app-keys-application-specific-wallet-accounts/2742/2)
- [ERC1776](https://github.com/ethereum/EIPs/issues/1776): Native meta transactions
- On-chain governance is hard. Aragon One’s John Light on [AGP1](https://blog.aragon.one/aragon-network-vote-1-review/): "While the Aragon Network Token contract showed around 20,000 unique addresses holding ANT at the time of the vote, only around 60 unique addresses participated. All together these 60 addresses controlled at most 7.85% of the ANT supply"
- ZEIP23 approved with [300 unique addresses voting](https://blog.0xproject.com/zeip-23-vote-post-mortem-311c9323e228).

**Application layer**

- [Tales from rural Oregon](https://blog.althea.org/tales-from-the-field/) where Althea is using Eth for micropayments on mesh networking
- [Status 0.10.0](http://our.status.im/0-10-0/) with blocking chats and better searching
- [DefiPulse](https://defipulse.com/) - stats on all the open finance projects.
- Games partnering with phone companies: [Decentraland and HTC](https://decentraland.org/blog/announcements/decentraland-partners-with-htc), [Enjin and Samsung](https://t.co/n1OpOP1fEF)
- [SetProtocol’s Strategy Enabled Tokens: automatic on-chain](https://www.medium.com/set-protocol/introducing-strategy-enabled-tokens-fd1090d98f8c) trading strategies, including asset rebalancing
- Vansa: the [road ahead for OmiseGo](https://medium.com/@vchatBKK/the-road-ahead-for-omisego-5003e76bb95)

**Interviews, Podcasts, Videos, Talks** 

- [Elena Nadolinski](https://itunes.apple.com/us/podcast/digitally-rare/id1413304564#) on Digitally Rare
- Aztec Protocol’s [Paul Berg](https://www.breaker.audio/stories-in-crypto/e/43455857) on Stories in Crypto
- [Cent](https://podcast.ethhub.io/cent-the-vision-for-earning-income-from-anywhere) on Into the Ether
- Latest [Token Curated Registry community call](https://www.youtube.com/watch?v=SGXhX1Rq7gc)

**Tokens / Business / Regulation**

- $750k in [onchain factoring loans to Amazon merchants](https://withcadence.io/blog/case-study-2/). Security tokens live on Ethereum.
- Proposed [ranking of apps in Status with SNT](https://github.com/andytudhope/Recollections)
- [TCRParty](https://medium.com/alpineintel/tcr-party-quick-lessons-and-v1-1-upcoming-features-4c8fdae1a21a) lessons learned and upcoming features
- Beylin: [TCRs 2.0 - Self curating lists](https://medium.com/bounties-network/tcrs-2-0-self-curating-lists-81447576d5e5)
- How [cryptofunds show how early we are](https://www.evanvanness.com/post/183089042961/crypto-funds-show-just-how-immature-web3-is) in the web3 tech cycle
- Pat Berarducci on [why state securities laws matter](https://twitter.com/PatBerarducci/status/1100160713409073154)

**General**

- Understanding [sparse Merkle multiproofs](https://medium.com/@jgm.orinoco/understanding-sparse-merkle-multiproofs-9b9f049e8f08)
- [Flyclients](https://eprint.iacr.org/2019/226): superlight POW clients from Bünz, Kiffer, Luu, Zamani. Proof size under 500KB for Ethereum through downloading “only a logarithmic number of block headers to synchronize and verify transactions while storing only a single block header between executions”
- [Zero knowledge for dexes](https://eprint.iacr.org/2018/962) from Bowe, Chiesa, et al
- How the [$7m EOS “hack” really happened](https://breakermag.com/heres-how-the-2-09-million-eos-hack-really-happened/). That is, it wasn’t a hack, just poor fundamental protocol design.
- MyCrypto goes over the basics: [why do we need transaction data](https://medium.com/mycrypto/why-do-we-need-transaction-data-39c922930e92)?
- [WebAssembly 100x faster](https://medium.com/wasmer/running-webassembly-100x-faster-%EF%B8%8F-a8237e9a372d) with Wasmer
- [Chromium broke Ledger support](https://github.com/LedgerHQ/ledgerjs/issues/306), which means Brave will likely break for Ledger too.

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Mar 4 - [Ethereum Magicians](https://ethereum-magicians.org/t/council-of-paris-2019-announcement/2438) (Paris)
- Mar 5-7 - [EthCC](https://ethcc.io/) (Paris)
- Mar 8-10 - [ETHParis](https://ethparis.com/) 
- Mar 8-10 - [EthUToronto](https://www.ethuoft.ca/)
- **Mar 15 - Next [core devs call](https://github.com/ethereum/pm/issues/83)**
- Mar 22 - [Zero Knowledge Summit 0x03](https://www.zeroknowledge.fm/summit) (Berlin)
- Mar 27 - Infura [end of legacy key support](https://blog.infura.io/infura-dashboard-update-9f02d0643eb3) 
- April 4-5 - [Deconomy](https://deconomy.com/seoul2019/) (Seoul)
- April 8-14 - [Edcon](https://www.edcon.io/) hackathon and conference (Sydney)
- Apr 19-21 - [ETHCapetown](http://ethcapetown.com/)
- Apr 24-26 - [Truffle Elevate](https://www.eventbrite.com/e/truffle-elevate-dublin-2019-blockchain-development-workshop-tickets-53831596755) (Dublin)
- May 9 - [Fluidity Summit](https://www.fluiditysummit.com/) (NYC)
- May 10-11 - [Ethereal](https://etherealsummit.com/?ref=weekinethereum) (NYC)
- **May 16 - [Token Summit](http://tokensummit.com/) (NYC)**
- May 17-19 - [ETHNewYork](https://medium.com/ethglobal/ethglobal-2019-updates-get-your-calendars-ready-1977e9315aee)
- May 17 - Deadline to accept [proposals for Instanbul upgrade](https://en.ethereum.wiki/roadmap/istanbul) fork
- **May 23-25 - [Swarm Orange Summit](https://www.eventbrite.com/e/swarm-orange-summit-madrid-2019-tickets-57378034245) (Madrid)**
- June 22-24 - [Zcon1](https://www.zfnd.org/zcon/) (Split, Croatia)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)

  
I own Week In Ethereum. Editorial control has always been 100% me. 

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **Update links to new URL: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/march-1-2019/](https://weekinethereumnews.com/march-1-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

---
title: "Week in Ethereum News <br> August 20, 2022"
date: "2022-08-20"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- Mainnet Merge [TTD: 58750000000000000000000 confirmed](https://twitter.com/TimBeiko/status/1560347372953018368?s=20&t=2Ilvv0d4JWukMf64eLOe5w)
- [TTD estimator](https://797.io/themerge/) predicts merge around September 15
- [Merge mainnet readiness checklist](https://github.com/ethereum/pm/blob/master/Merge/mainnet-readiness.md) is complete
- mainnet-shadow-fork-11 [merged successfully](https://twitter.com/TimBeiko/status/1560346663264219137), nicest shadow fork so far
- Flashbots [MEV-boost relay open sourced](https://writings.flashbots.net/writings/Flashbots-Relay-open-sourcing/), AGPL license, alpha, [OFAC compliant](https://twitter.com/bantg/status/1559948198508118016)
- [MEV redistribution](https://people.eecs.berkeley.edu/~ksk/files/MEV_Redistribution.pdf) \[PDF\] improves PoS economic security
- Proposal to [remove trusted relays in MEV-boost](https://ethresear.ch/t/removing-trusted-relays-in-mev-boost-using-threshold-encryption/13449) using threshold encryption

**Execution layer**

- Latest core devs [call video](https://www.youtube.com/watch?v=jJaCaS0WbIw&t=325s). Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1560345029511589888) and [Christine Kim](https://docsend.com/view/2magweham8bc6ewy):
    - MEV-boost relay discussion: transactions will be included as long as some validators don’t censor
    - Ethereum censorship resistance discussion: defense is user activated fork
    - Sepolia testnet post-merge upgrade now expected August 21
    - Kiln testnet to be shutdown September 6
    - Merge EIPs moved to last call: [EIP3675](https://eips.ethereum.org/EIPS/eip-3675) (upgrade to PoS) & [EIP4399](https://eips.ethereum.org/EIPS/eip-4399) (PREVRANDAO)
- Erigon [v2022.08.02-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.08.02): mainnet Merge TTD & fixes
- EIP4844 (proto-danksharding) [call video](https://www.youtube.com/watch?v=3s_od5WjN7Y&t=2s) and [notes](https://docs.google.com/document/d/1KgKZnb5P07rdLBb_nRCaXhzG_4PBoZXtFQNzKO2mrvc/edit): upcoming public devnet, fee market design, sync architecture and KZG ceremony
- KZG ceremony [call video](https://www.youtube.com/watch?v=6LsVjf9qARI): audit started, contributing users will be included in final transcript and UI wireframes being reviewed
- Geth team first [AMA](https://www.reddit.com/r/ethereum/comments/wpqmo1/ama_we_are_the_go_ethereum_geth_team_18_august/) on Reddit

**Proof of Stake consensus layer**

- Consensus layer specs [v1.2.0-rc.3](https://github.com/ethereum/consensus-specs/releases/tag/v1.2.0-rc.3): Bellatrix epoch and the Merge TTD
- [Client diversity improved](https://twitter.com/superphiz/status/1559667329574780935): Prysm 35% and Lighthouse 33%
- [Dappnode multiclient support](https://medium.com/dappnode/multiclient-on-ethereum-mainnet-has-arrived-this-is-all-you-need-to-know-7bc0cd8fadc5): single click to change consensus layer client
- Script to [download beacon chain blocks](https://www.symphonious.net/2022/08/18/beacon-rest-api-fetching-blocks-on-a-fork/) on a fork

**Layer2**

- Miden VM [v0.2](https://ethresear.ch/t/miden-vm-v0-2-new-vm-architecture-for-a-zk-rollup/13405) (zk-rollup): new VM architecture

**EIPs/Standards**

- [EIP5298](https://github.com/ethereum/EIPs/pull/5300/files): ENS as token holder
- [EIP5299](https://github.com/ethereum/EIPs/pull/5299/files): Storage scaling pattern
- [EIP5334](https://github.com/ethereum/EIPs/pull/5334/files): ERC721 user and expires & level extension
- [EIP5450](https://eips.ethereum.org/EIPS/eip-5450): EOF - stack validation
- [EIP5453](https://github.com/ethereum/EIPs/pull/5453/files): Contract crypto endorsement
- [EIP5478](https://github.com/ethereum/EIPs/pull/5478/files): Reducing the gas cost of contract creation with existing code
- [EIP5484](https://github.com/ethereum/EIPs/pull/5484/files): Consensual soulbound tokens
- [EIP5485](https://eips.ethereum.org/EIPS/eip-5485): Legitimacy, jurisdiction and sovereignty
- [EIP5489](https://github.com/ethereum/EIPs/pull/5489/files): NFT hyperlink extension
- [EIP5496](https://github.com/ethereum/EIPs/pull/5496/files): Multi-privilege management extension for ERC721
- [EIP5501](https://github.com/ethereum/EIPs/pull/5501/files): Rental & delegation NFT - ERC721 extension
- [EIP5503](https://github.com/ethereum/EIPs/pull/5503/files): Refundable token
- [EIP5507](https://github.com/ethereum/EIPs/pull/5507/files): Refundable NFTs

* * *

### **This newsletter is made possible thanks to** [**SpeedRunEthereum**](https://speedrunethereum.com/)**!**

![SpeedRunEthereum](https://weekinethereumnews.com/wp-content/uploads/2022/04/Screenshot-from-2022-04-01-15-39-52.png)

Are you a web2 dev who wants to get into web3?

The best way to go from _zero_ to **hero** is [SpeedRunEthereum.com](https://speedrunethereum.com/).

Learn how to build on Ethereum; the superpowers and the gotchas.

Then [speed run Ethereum](https://speedrunethereum.com/) by testing your skills in a [series of challenges](https://speedrunethereum.com/challenge/simple-nft-example) and [join web3](https://twitter.com/austingriffith/status/1493688828661432325).

* * *

**Stuff for developers**

- [Foundry](https://twitter.com/r_krasiuk/status/1559225181163470851) verification adds Sourcify support
- Chainlink’s [Huff starter kit](https://github.com/smartcontractkit/huff-starter-kit#readme): develop Huff contracts using Foundry
- [ERC721K](https://twitter.com/KamesGeraghty/status/1559516539149172736): dynamic on-chain SVG NFTs using data streams
- [Music NFT IPFS metadata](https://github.com/SweetmanTech/MUSIC-METADATA-IPFS#readme): on-chain music metadata
- [Lanyard](https://lanyard.build/): Merkle root generator for NFT allow lists
- [Seaport order validator](https://twitter.com/z0age/status/1560663421116248066): single RPC call for opinionated safety checks
- Deploy contracts using [a burner address](https://w1nt3r.mirror.xyz/TK4XduxDclnnXmKKDR93ytkLXYGAx55f31ZwLWvU-KM) or [OpenZeppelin Defender relay client](https://twitter.com/OpenZeppelin/status/1559559571462443008)
- [Contract automation solutions compared](https://medium.com/coinmonks/smart-contract-automation-state-of-the-art-hack-view-c153944b1a02): Gelato Ops, Keep3r Network, Chainlink Keepers and Open Zeppelin Defender
- ethers.js [v5.7.0](https://github.com/ethers-io/ethers.js/releases/tag/v5.7.0): fixes and improvements
- [Etherface](https://github.com/volsa/etherface#readme): signature database with source links, crawls GitHub/Etherscan/4Byte
- [RainbowKit](https://www.rainbowkit.com/docs/authentication) adds Sign-In with Ethereum + NextAuth.js support
- [Using mutants to improve static analysis](https://blog.trailofbits.com/2022/08/17/using-mutants-to-improve-slither/): comparing Slither with Securify & SmartCheck
- Ethernaut DAO CTF [switch solution](https://stermi.medium.com/ethernautdao-ctf-7-solution-switch-ff6d7ca0a59)

**Security**

- Sherlock [cross-protocol reentrancy](https://mirror.xyz/0xE400820f3D60d77a3EC8018d44366ed0d334f93C/LOZF1YBcH1eBdxlC6HP223cAMeTpNgQ-Kc4EjQuxmGA) disclosed, $250k bounty paid
- Celer’s cBridge front end [DNS cache poisoning](https://twitter.com/celernetwork/status/1560123830844411904)

**Ecosystem**

- Run DeFi front end (Aave) locally on [Windows](https://fishy-mailman-e0e.notion.site/Run-your-own-local-Front-End-from-zero-to-hero-b2cdb30a6e0046f0b28351fc431f03e0), [Mac](https://hazelstar2.notion.site/hazelstar2/Run-your-own-local-Aave-Front-End-from-zero-to-hero-MacOS-edition-9aa8d0c910224d68bdb99a1f9f8843f9) and [DAppNode](https://twitter.com/eduadiez/status/1560314041389780992)
- [Snitchy](https://snitchy.xyz/): check an RPC endpoint for US OFAC compliance
- Wallet devs [call video](https://www.youtube.com/watch?v=leEdlaZjc6I) and [notes](https://twitter.com/_SamWilsn_/status/1560666767051333633)
- [Yuga Labs](https://twitter.com/yugalabs/status/1560035176562016262) will only recognize NFTs on Ethereum PoS
- [NFT marketplace replay protection](https://twitter.com/z0age/status/1560229676328574977) against forks

**Application layer**

- [Dai bridge](https://twitter.com/MakerDAO/status/1559570668353720321) live on Arbitrum Nova
- [ENS](https://twitter.com/ensdomains/status/1559811577917755394): two million names created, one million in 3.5 months
- Nimi [beta v0.2](https://twitter.com/0xNimi/status/1559208188259418114): profile page, default for eth.limo, gasless updates via IPNS
- [dm3](https://medium.com/corpus-ventures/dm3-decentralized-messaging-for-web3-8d66f6e77b53): encrypted messaging for ENS users, beta
- [Safe](https://forum.gnosis-safe.io/t/proposal-safe-distribution-for-users/369) (formerly Gnosis Safe) proposed token distribution to users
- Karma [Discourse plugin](https://mirror.xyz/showkarma.eth/zYoSK7CDY-vJoXV8tPx67uW9aatEegqjm0lT60YL2Zk) shows DAO reputation data of users \[Disclosure: Starbloom portfolio\]

* * *

### **Job Listings**

- ØVIX + GOGO Protocol: [VP of Engineering](https://join.com/companies/cryptogogos/5463001-head-of-software-development-vp-engineering-at-crypto-start-up?utm_source=ETHnewsletter&utm_medium=email&utm_campaign=WeekInEthNews)
- Gnosis Chain looking for [Head of Bridges](https://grnh.se/9bed164e2us), [Head of Validators](https://grnh.se/e51fc7332us) & [DevRel Eng](https://grnh.se/571e88cc2us).
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)

**Job listings: $600** for four issues (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Coin Center: [US OFAC overstepped authority in sanctioning Tornado Cash contract addresses](https://www.coincenter.org/analysis-what-is-and-what-is-not-a-sanctionable-entity-in-the-tornado-cash-case/), potentially violates constitutional rights to due process & free speech
- [TRM Labs data](https://www.trmlabs.com/post/how-defi-platforms-are-using-data-from-trm-labs-to-respond-to-tornado-cash-sanctions) used by DeFi front ends to check addresses for sanctions risk
- Reasons for [financial privacy](https://twitter.com/danfinlay/status/1559583110861189120); privacy should be the default
- [US Fed supervised banks](https://www.federalreserve.gov/supervisionreg/srletters/SR2206.htm) have to notify the Fed before engaging in crypto related activities
- [US SEC sued Dragonchain](https://www.sec.gov/litigation/litreleases/2022/lr25468.htm) for selling an alleged unregistered security
- [Canadian exchanges impose $30k annual cap](https://twitter.com/jacobrobinsonjd/status/1560070769731846144) on token purchases in some provinces
- [US FDIC sends cease & desist letters](https://www.fdic.gov/news/press-releases/2022/pr22060.html) for statements about deposit insurance

**General**

- [CryptoStats.fyi](https://CryptoStats.fyi:): visualize data available from Crypto Stats
- [Plonky2](https://blog.polygon.technology/plonky2-is-now-open-source) (Polygon Zero's zk proving system) open-sourced
- [tlock](https://twitter.com/AnomalRoil/status/1558269374691250176): time based encryption/decryption using a drand threshold network
- [Apple fixed two zero-day vulnerabilities](https://www.bleepingcomputer.com/news/security/apple-security-updates-fix-2-zero-days-used-to-hack-iphones-macs) under active attack, out-of-bounds write in the Kernel and WebKit
- [Chrome fixed zero-day vulnerability](https://nakedsecurity.sophos.com/2022/08/17/chrome-browser-gets-11-security-fixes-with-1-zero-day-update-now/), insufficient validation of untrusted input in Intents
- [Signal users targeted](https://www.vice.com/en/article/qjkvxv/how-a-third-party-sms-service-was-used-to-take-over-signal-accounts) after Twilio compromised

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-20-2022](https://weekinethereumnews.com/week-in-ethereum-news-august-20-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Aug 23 – [Devcon wave 09 + 10 tickets](https://devcon.org/en/tickets/)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- **Aug 28 –** [**Ethereum a New Era**](https://go.ueth.org/) **(San Francisco)**
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev/) (hackathon & conference)
- Sep 2-28 – [ETHOnline](https://online.ethglobal.com/') (ETH Global)
- Sep 6 – [Bellatrix upgrade](https://github.com/ethereum/consensus-specs/releases/tag/v1.2.0-rc.2) (epoch: 144896)
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 7-22 – [Gitcoin Grants round 15](https://twitter.com/gitcoin/status/1558498622949523456)
- Sep 9 – [Merge Community Call #7](https://github.com/ethereum/pm/issues/599)
- Sep 9-11 – [Ethereum SP](https://www.ethereumbrasil.com/#next) (São Paulo)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- **Sep ~15 –** [**the Merge**](https://github.com/ethereum/execution-specs/pull/585) **(TTD: 58750000000000000000000)**
- Sep 16-18 - [EthBerlin](https://ethberlin.ooo/)
- Sep 23 - [ETH HCMC](https://2022.ethhcmc.com/) summit (Ho Chi Minh)
- Sep 23-24 - [ETHSantiago](https://ethsantiago.com/)
- Oct 7-16 – [Devcon week](https://devcon.org/en/devcon-week/) (Bogotá)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- Oct 7-9 – [Infinite hackathon](https://infinite-hackathons.eth.limo/) (Bogotá)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

---
title: "Week in Ethereum News <br> August 5, 2023"
date: "2023-08-05"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=X46mbG8N5XM&t=350s). Recap by [Tim Beiko](https://twitter.com/abcoathup/status/1687186385609052162).  Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1687568467409727488) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-167/):
    - EIP4788 (beacon block root in EVM): agreed to use a contract rather than a precompile, will need audit/formal verification, devnet 8 will wait for implementations
    
    - EF devops launched 2.1M validator testnet in prep for Holešky testnet
    
    - EIP5806 (delegate transaction) & EIP7377 (migration transaction) presented and broader discussions on account abstraction
    
    - [Verkle Trie update](https://docs.google.com/presentation/d/1Hgke4EHtjHBaYrIA6WbToGip6eho6INBgvwG76BIw1M): performance improvements, migration via overlay method and remaining questions

- Consensus-specs [v1.4.0-beta.1](https://github.com/ethereum/consensus-specs/releases/tag/v1.4.0-beta.1): data gas renamed blob gas & additional tests

- EIP4844:
    - Terence: [EIP4844 economics](https://twitter.com/terencechain/status/1686737819581202432)
    
    - [KZG Ceremony](https://ceremony.ethereum.org/) has 133k contributions, [lobby is empty](https://twitter.com/CarlBeek/status/1686723570234187776); list of [special contributions](https://blog.ethereum.org/2023/08/02/kzg-special-contributions) (from satellites to cats)
    
    - [GossipSub optimizations](https://twitter.com/jcksie/status/1687434139035750401) (IDontWant & Limit flood publishing) should reduce Nimbus CL client bandwidth consumption

**Layer 1**

- [Reorg.pics](https://twitter.com/nero_eth/status/1686347380159926272): dashboard of mainnet reorgs 

- [Epoch long reorg on Goerli testnet](https://twitter.com/potuz1/status/1685736037321166848), unlikely to happen on mainnet
    - Ben Edgington’s [explainer](https://eth2book.info/capella/part2/consensus/issues/#casper-ffgs-fork-choice-can-cause-long-reorgs) from Upgrading Ethereum book

- [SSZ++](https://github.com/OffchainLabs/sszpp#readme): fast SSZ library, 27ms deserialization & 23ms hashing on full beacon state without caching

- [Prototype EVMMAX API](https://twitter.com/teamipsilon/status/1687091771648671744) in evmone: allows implementing most precompiles

**For stakers**

- [Wenmerge](https://relay.wenmerge.com/) non-filtering MEV-Boost relay

**Client releases**

- Consensus layer:
    - Lodestar [v1.10.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.10.0): performance improvements, NodeJS v20, IPv6 support, bandwidth optimizations and builderOnly option for DVT users
    
    - Teku [v23.8.0](https://github.com/Consensys/teku/releases/tag/23.8.0): state caching improvements & minimum Java version updated to Java 17

**Research**

- Vitalik: [nuances of data recoverability in data availability sampling](https://ethresear.ch/t/nuances-of-data-recoverability-in-data-availability-sampling/16256)

- [Protocol-enforced proposer commitments](https://efdn.notion.site/PEPC-FAQ-0787ba2f77e14efba771ff2d903d67e4) (PEPC) FAQ

- [Relays post-ePBS](https://ethresear.ch/t/relays-in-a-post-epbs-world/16278) & proposed Top-of-Block (ToB) payments 

- Potuz: [three dichotomies in ePBS](https://ethresear.ch/t/three-dichotomies-in-epbs/16267)

**Layer 2**

- Offchain Labs [BOLD](https://offchain.medium.com/bold-permissionless-validation-for-arbitrum-chains-9934eb5328cc) (Bounded Liquidity Delay): proposed dispute protocol for permissionless validation of Arbitrum chains, eliminates [delay attack vector](https://twitter.com/DZack23/status/1687209094015504389)

- Popcorn: [zkEVMs criticize each other](https://twitter.com/gluk64/status/1687263207860166656) over attribution and marketing claims

**EIPs/Standards**

- EIPs:
    - [EIP7441](https://github.com/ethereum/EIPs/pull/7441/files): Upgrade block proposer election to Whisk

- ERCs (application layer):
    - [ERC7425](https://github.com/ethereum/EIPs/pull/7427/files): Tokenized reserve
    
    - [ERC7432](https://github.com/ethereum/EIPs/pull/7432/files): NFT roles
    
    - [ERC7439](https://github.com/ethereum/EIPs/pull/7443/files): Prevent ticket touting (ERC721 extension)
    
    - [ERC7444](https://github.com/ethereum/EIPs/pull/7444/files): Time locks maturity

**Stuff for developers**

- Hardhat [v2.17.1](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.17.1): Solidity v0.8.21 support, console.log in pure functions & improved flattening

- Foundry:
    - Tip: [generate local coverage reports](https://twitter.com/paulrberg/status/1686829173585649667) using lcov

- Dan Finlay’s [MATT auction](https://github.com/danfinlay/foundry-matt#readme) (maximize NFT revenue) in Foundry, uses ERC20 allowance as bid

- web3.py [WebSocketProviderV2](https://snakecharmers.ethereum.org/websockets-v2/): rewrite of WebsocketProvider, beta

- CryptoZombies [Optimism NFT course](https://cryptozombies.io/en/optimism): create, test & deploy

- [DeCipher](https://www.bunzz.dev/decipher): contract doc generator from block explorer URL

- Secureum RACE #20: [8 question Solidity quiz & answers](https://ventral.digital/posts/2023/7/30/race-20-of-the-secureum-bootcamp-epoch-infinity)

**Security**

- Vyper [malfunctioning reentrancy locks](https://twitter.com/big_tech_sux/status/1686417276680192001) in v0.2.15/16 & v0.3.0, [Curve $70M exploit](https://rekt.news/curve-vyper-rekt/) impacting Alchemix, JPEG'd & Metronome with some [Alchemix](https://twitter.com/alchemixfi/status/1687531017161105408) & [JPEG'd](https://twitter.com/jpegd_69/status/1687594063527038976) funds returned
    - Potentially [vulnerable Vyper contracts](https://github.com/banteg/vyper-reentrancy/#readme)

- LeetSwap (Solidly fork) on Base [exploited](https://twitter.com/blocksecteam/status/1686217464051539968), pool manipulated via internal function being public

- $20M sent to [address poisoning spammer](https://twitter.com/tayvano_/status/1686418992599273472), USDT was later frozen 

- [Whitehacks kit](https://github.com/emilianobonassi/whitehacks-kit#readme): Foundry template to perform actions in single transaction using Flashbots

- [Solidity audit report generator](https://github.com/aviggiano/solidity-audit-report-generator#readme) (VSCode extension) using comments

**Ecosystem**

- Eight years since [Ethereum mainnet launch](https://blog.ethereum.org/2015/07/30/ethereum-launches)

- Ethereum.org [translatathon](https://twitter.com/ethdotorg/status/1686377458529075200): translate the website to win prizes

**Notable at app layer**

- OndoFinance [USD Yield](https://twitter.com/nathanlallman/status/1687119596938260481) (USDY): tokenized note (US Treasuries & bank deposits), non-US only

- Karma [delegate registry](https://twitter.com/karmahq_/status/1687095733139177472): onchain DAO delegate info \[Disclosure: Starbloom portfolio\]

- [Umbra Cash stealth address anonymity](https://arxiv.org/abs/2308.01703): heuristics could link most recipients & suggested countermeasures

- Tx [chat](https://www.tx.cool/chat): chat like interface to browse an addresses onchain messages

- Golem [Octant Epoch Zero](https://golem.foundation/2023/07/28/epoch-zero-results.html): $1M distributed amongst ten public goods projects

- [Gitcoin Grants 18](https://twitter.com/gitcoin/status/1686291853446926336) applications open

* * *

### Job Listings

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

- Wyoming Stable Token Commission seek [Executive Director](https://www.governmentjobs.com/careers/wyoming/jobs/4126743/stc-0419-executive-director-cheyenne-or-laramie)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [GameStop removing iOS & browser extension wallets](https://wallet.gamestop.com/) due to regulatory uncertainty

- [Revolut](https://www.theblock.co/post/243200/revolut-shut-down-crypto-business-us) shutting down crypto services in US

- [Curve co-founder Michael Egorov](https://thedefiant.io/large-crv-backed-loans-threaten-to-destabilize-defi) deleveraging after Curve exploit

- [Ilya Lichtenstein admits](https://www.cnbc.com/2023/08/03/new-york-man-admits-being-original-bitfinex-hacker-during-guilty-plea-in-dc-to-bitcoin-money-laundering.html) to being Bitfinex 2016 hacker

- [US SEC charged Hex founder Richard Heart](https://www.sec.gov/news/press-release/2023-143) with unregistered offerings of securities and fraud for misappropriating proceeds

- [Kenya](https://www.reuters.com/world/africa/kenyan-government-suspends-activities-worldcoin-country-2023-08-02/) suspended local Worldcoin activities

- [FBI](https://www.ic3.gov/Media/Y2023/PSA230804) warns of NFT mint phishing scams

**General**

- [Rate-limiting nullifier](https://mirror.xyz/privacy-scaling-explorations.eth/iCLmH1JVb7fDqp6Mms2NR001m2_n5OOSHsLF2QrxDnQ) (RLN) for spam prevention whilst preserving anonymity.  Contribute to the trusted ceremony

- [ProtoGalaxy](https://eprint.iacr.org/2023/1106): efficient ProtoStar-style folding of multiple instances

- [X (Twitter)](https://twitter.com/jeremyvaught/status/1687223289482035200) takes @music username

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-5-2023](https://weekinethereumnews.com/week-in-ethereum-news-august-5-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Aug 11-13 – [ETHMunich](https://ethmunich.de/) hackathon

- Aug 15-16 – [ETHToronto](https://www.ethtoronto.ca/) & [ETHWomen](https://www.ethwomen.com/)

- Aug 15-29 – [Gitcoin Grants 18](https://twitter.com/gitcoin/status/1681747409435787264)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org/) (Buenos Aires)

- Aug 23 – [KZG Ceremony](https://ceremony.ethereum.org/) closes (extended)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 31 - Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 7-9 – [ETHAccra](https://www.ethaccra.xyz/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 15-17 – [ETHChicago](https://www.ethchicago.xyz/) conference & hackathon

- **Sep 15-16 –** [**ETHMobile Miami**](https://www.ethmobile.io/)

- **Sep 18-24 –** [**ETHSafari**](https://ethsafari.xyz/) **(Kilifi Kenya)**

- Sep 21–24 – [Pragma](https://ethglobal.com/events/pragma-newyork) & [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 6-27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 13-15 – [Ethereum Kuala Lumpur](https://hack.ethkl.org/) conference & hackathon

- Oct 21 – [Ethereum México](https://twitter.com/ethereum_mexico/status/1684649652639924224)

- **Oct 22-24 –** [**ETH Hong Kong**](https://www.ethhongkong.co/)

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Oct 27-29 – [ETH Vietnam](https://www.eth-vietnam.com/)

- **Oct 27-29 –** [**ETH London**](https://www.encode.club/eth-london) **hackathon**

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) application deadline

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://lu.ma/ethbrno3)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 16-19 – [Pragma](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

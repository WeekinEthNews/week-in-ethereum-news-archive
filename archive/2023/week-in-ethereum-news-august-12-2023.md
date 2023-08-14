---
title: "Week in Ethereum News <br> August 12, 2023"
date: "2023-08-12"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=LJt4cu3eG2g&t=23s). Notes from [Terence](https://github.com/ethereum/pm/issues/844#issuecomment-1673359012) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-115/):
    - Devnet 8 planned for early next week 
    
    - Fork-choice filtering change will be bundled with Deneb release

- EIP4788 (beacon block root in EVM) [draft assembly contract](https://github.com/lightclient/4788asm#readme), optimizations for gas welcome

- Latest Dencun testing [call video](https://www.youtube.com/watch?v=fQ6ugSRi3DA&t=160s) (previously EIP4844 call)

- [KZG Ceremony](https://ceremony.ethereum.org/) has 136k contributions, lobby closes August 23

**Layer 1**

- EthereumJS [v7](https://twitter.com/efjavascript/status/1689653616079208449): ESM support, removed Buffer, reduced dependencies & build sizes, default now Shanghai and Cancun support

- [Holešky testnet to start with 1.4M validators](https://twitter.com/parithosh_j/status/1689753694487646208) (twice the validators of mainnet) after EF devops spun up 3 large testnets to check sizing (2.1M validators had issues)

- [Kurtosis package](https://ethereum-magicians.org/t/introducing-eth2-package-a-tool-for-spinning-up-private-testnets-in-a-single-command/15390) to spin up multi-node EL/CL testnets in the cloud with any client combination (including Reth), comes with Grafana & Prometheus

- Verkle Tries
    - [Verkle preimage](https://hackmd.io/@jsign/vkt-preimage-generation-and-distribution) generation & distribution strategy
    
    - [Verkle Trie migration options](https://notes.ethereum.org/@rudolf/migration): read-only vs writeable Merkle Trees

- [Flashbots builder glitch](https://twitter.com/EigenPhi/status/1689887764077273088) included reverting transactions

**For stakers**

- Beacon chain [churn limit turned up to 11 per epoch](https://twitter.com/superphiz/status/1689918550050291713)

- [NanoPC-T6](https://twitter.com/EthereumOnARM/status/1689327953052577804): run a full node on ~$300 hardware

- [bloXroute ethical relay](https://twitter.com/bloxroutelabs/status/1690065892778926080) being sunset (filtered generalized frontrunning & sandwiching)

**Client releases**

- Execution layer:
    - Geth [v1.12.1](https://github.com/ethereum/go-ethereum/releases/tag/v1.12.1): maintenance release, includes development for Dencun
    
    - Reth [v0.1.0-alpha.6](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.6): follow up to fix in alpha.5 that handles reorgs 

**Research**

- [Second slot reorgs](https://ethresear.ch/t/the-second-slot-itch-statistical-analysis-of-reorgs/16333): slot indices impact likelihood of being reorged

- [Builders’ Behavioral Profiles](https://ethresear.ch/t/empirical-analysis-of-builders-behavioral-profiles-bbps/16327) (BBPs): metrics covering features & strategies when building blocks and bidding during MEV-Boost auctions

- [Protocol-Enforced Proposer Commitments](https://mirror.xyz/ohotties.eth/lBEXiiU7yK91OuSn8QyJPM9Db8GuyDFzCEUAj60BWyI) (PEPC) explainer

- [Quantum-resistant weak Verifiable Delay Function](https://eprint.iacr.org/2023/1197) but requires curves with unknown endomorphism rings as input

**Layer 2**

- Coinbase [Base](https://base.mirror.xyz/KPrKIukePtM2Iz945_3GpQJ-tgMf1hoato5isStLXJI) (OP Stack rollup) open to the public ([Onchain Summer](https://onchainsummer.xyz/) marketing campaign)

**EIPs/Standards**

- EIPs:
    - [EIP7480](https://github.com/ethereum/EIPs/pull/7480/files): EOF - Data instructions

* * *

### **Check out Austin Griffith on the Week in Ethereum** [**Web3 Builders podcast**](https://podcasters.spotify.com/pod/show/web3builderspodcast)

![Web3 Builders](https://weekinethereumnews.com/wp-content/uploads/2023/08/Web3-Builders.webp)

Check out [Austin Griffith on the first interview of web3 builders](https://www.youtube.com/watch?v=ivlUrYmJHw4). This was a great episode.

What does Austin think is **_by far_** _the worst part of building in web3_?  

More episodes on [YouTube](https://www.youtube.com/@web3builderspod), or listen on [Apple](https://podcasts.apple.com/us/podcast/web3-builders/id1697252853), [Spotify](https://podcasters.spotify.com/pod/show/web3builderspodcast) or [RSS](https://anchor.fm/s/e5abffc8/podcast/rss).  Or get pinged for new episodes on [Telegram](http://t.me/web3builderspod) or [Substack](https://web3builderspod.substack.com/).

Please like, subscribe, and share on social media if you enjoyed the episode. 

* * *

**Stuff for developers**

- Solmate [v6.2.0](https://github.com/transmissions11/solmate/pull/380): fix silent overflow edge case in SignedWadMath:wadMul; [found](https://twitter.com/Montyly/status/1688603604062482433) using Trail of Bits Medusa

- [Iter](https://github.com/jtriley-eth/iter-sol#readme): lazy evaluated iterators in Solidity 

- [Cove](https://twitter.com/msolomon44/status/1688656321053425664): contract verification, alpha is for Solidity Foundry projects using deployment tx hashes

- EVM Diff [updated](https://twitter.com/msolomon44/status/1689656505652690945)

- [Bulloak](https://github.com/alexfertel/bulloak#readme): Solidity test generator based on branching tree technique

- [Vyper compiler](https://jtriley.substack.com/p/the-vyper-compiler) deep dive

- Fe [v0.24.0](https://github.com/ethereum/fe/releases/tag/v0.24.0): adds support for user defined libraries

- Halmos [v0.1.2](https://github.com/a16z/halmos/releases/tag/v0.1.2) (symbolic testing): adds support for DELEGATECALL, CALLCODE, CREATE2, struct types as test parameters and library linking

- [Agent buttercup](https://github.com/Cozy-Finance/agent-buttercup#readme): agent-based simulation engine for DeFi researchers/engineers, uses revm

- yAcademy [zk auditing fellowship modules](https://twitter.com/yAcademyDAO/status/1687891681423634432): zk, Rate-limiting Nullifier & Spartan-ECDSA

- CTFs:
    - Flashbots [MEV-Share CTF solutions](https://github.com/minaminao/ctf-blockchain/tree/main/src/MEVShareCTF#readme)
    
    - Curta CTF [Billy the Bull solution](https://twitter.com/zachobront/status/1688247687613743105)

- [p0tion v1](https://mirror.xyz/privacy-scaling-explorations.eth/TuLZRdgCQsydC8JJgCNH4F7GzifRBQ6fr31DHGLFVWM): toolkit for Groth16 zk-application development

- [Noble curves typosquat](https://blog.phylum.io/typosquat-of-popular-ethereum-package-steals-private-keys/): malicious npm package sends private key to remote server

**Security**

- Steadefi on Arbitrum & alt-L1 [$1.1 million stolen](https://twitter.com/steadefi/status/1688638572608552960) via compromised deployer wallet

- [UniswapX order vulnerability disclosed](https://kebabsec.xyz/posts/critical_vulnerability_in_uniswapx/), fixed with $200k bounty paid

- [Vyper postmortem](https://hackmd.io/@vyperlang/HJUgNMhs2) of non-reentrancy lock vulnerability in v0.2.15/16 & v0.3.0

- [SEAL 911](https://twitter.com/samczsun/status/1688613385565528064): contact the security community in an emergency via a Telegram bot

**Ecosystem**

- [Danny responds to those trying to normalize centralization conversations](https://twitter.com/dannyryan/status/1688644951230267392): Lido over 33% of ETH staked is a threat to Ethereum

- EF Next Billion fellowship: [five human stories of cohort 3](https://blog.ethereum.org/2023/08/07/nb-fellows-cohort-3)

- Etherscan [similar contract search](https://twitter.com/etherscan/status/1689984336274284544) updated to search across Etherscan supported chains

**Enterprise**

- [PayPal USD stablecoin](https://newsroom.paypal-corp.com/2023-08-07-PayPal-Launches-U-S-Dollar-Stablecoin), issued by Paxos
    - [PYUSD contract](https://github.com/paxosglobal/pyusd-contract#readme) is upgradeable, balances can be frozen & wiped

- Visa experiments with [paying gas fees with card](https://usa.visa.com/solutions/crypto/paying-blockchain-gas-fees-with-card.html) on Goerli testnet

**Notable at app layer**

- Rune’s [Maker endgame](https://twitter.com/runekek/status/1688571159367823360) and [SubDAO farming overview](http://forum.makerdao.com/t/sparkdao-spk-pre-farming-airdrop-general-subdao-farming-overview/21595)

- Maker [Enhanced DSR](https://twitter.com/runekek/status/1688991177843019778) (Dai Savings Rate) started at 8% and reduced to 5.8%

- [Nexus Mutual](https://nexusmutual.io/blog/nexus-mutual-expands-cover-capacity-in-the-uk-with-on-chain-capital) providing small UK retailers coverage via Retail Mutual

- Safe [social login](https://twitter.com/safe/status/1689313162817093633): sign up with Google or Apple ID on iOS, experimental

- [MultiSafe](https://twitter.com/smoldapp/status/1689998191289139200): clone or deploy a Safe to multiple chains with the same address

- [Y00ts](https://twitter.com/y00tsNFT/status/1689404417072889867) NFTs migrating to Ethereum after previously migrating from Solana to Polygon

- DAO’s shutting down & distributing Arbitrum airdrop: [Saddle](https://www.saddle.community/t/sip-x-protocol-operations-and-treasury-management/632) (Curve fork) & [Hundred Finance](https://twitter.com/hundredfinance/status/1689358397898887168)

- Base apps:
    - [BasePaint](https://basepaint.xyz/): shared pixel canvas, open edition NFT every 24 hours
    
    - [Words3](https://twitter.com/0xsmallbrain/status/1689404151166570496): scrabble with fluctuating price letter tiles, game ends this weekend
    
    - [Friend Tech](https://twitter.com/phabcd/status/1690061905468010496): buy shares in people to DM, PWA on mobile, invite only

* * *

### Job Listings

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

- Wyoming Stable Token Commission seek [Executive Director](https://www.governmentjobs.com/careers/wyoming/jobs/4126743/stc-0419-executive-director-cheyenne-or-laramie)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US Federal Reserve](https://www.federalreserve.gov/newsevents/pressreleases/bcreg20230808a.htm) info on supervision program for banks crypto activities

- [Bittrex $24M settlement with US SEC](https://www.sec.gov/news/press-release/2023-150) for operating as an unregistered broker

- [SBF jailed](https://twitter.com/innercitypress/status/1690061503645229056): bail revoked for intimidating witnesses

- 1 year anniversary of [Alex Pertsev’s unjust arrest](https://twitter.com/PeppersecCOM/status/1689771500717723650) 

* * *

### **Evan’s new podcast: web3 Builders**

- [Austin Griffith comes on web3 builders](https://podcasts.apple.com/us/podcast/stealing-web2s-developers-with-austin-griffith/id1697252853?i=1000624167503) to talk about what he’s doing to bring in the next wave of developers 

- Evan and Will’s [weekly web3 show](https://podcasts.apple.com/us/podcast/web3-builders/id1697252853), discussing everything exciting over the last week. Current episode is a banger; next episode drops in a few hours.  

* * *

**ZK**

- Justin Thaler: [Lasso (lookup argument with faster prover) and Jolt (zkVM design)](https://a16zcrypto.com/posts/article/introducing-lasso-and-jolt/)

- Overview of [Folding schemes](https://taiko.mirror.xyz/tk8LoE-rC2w0MJ4wCWwaJwbq8-Ih8DXnLUf7aJX1FbU): Nova, Sangria, SuperNova, HyperNova & Protostar

- [CycleFold](https://eprint.iacr.org/2023/1192): folding-scheme-based recursive arguments over a cycle of elliptic curves

**General computer security (Defcon edition)**

- [Milk Sad](https://milksad.info/): Libbitcoin Explorer bx seed generated insecure private keys, only 32 bits of entropy

- [BitForge](https://www.fireblocks.com/blog/bitforge-fireblocks-researchers-uncover-vulnerabilities-in-over-15-major-wallet-providers): MPC implementation vulnerabilities, including GG-18, GG-20 and Lindell17

- CPU vulnerabilities: [Downfall](https://downfall.page/) (Intel including SGX) and [Inception](https://comsec.ethz.ch/research/microarch/inception/) (AMD Zen CPU)

- [VS Code secure token storage](https://cycode.com/blog/exposing-vscode-secrets/): malicious extensions could expose application tokens

- [Acoustic side channel attack on laptop keyboards](https://arxiv.org/abs/2308.01074) using deep learning & phone microphones

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-12-2023](https://weekinethereumnews.com/week-in-ethereum-news-august-12-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

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

- Sep 18-24 – [ETHSafari](https://ethsafari.xyz/) (Kilifi Kenya)

- Sep 21–24 – [Pragma](https://ethglobal.com/events/pragma-newyork) & [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 6-27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 13-15 – [Ethereum Kuala Lumpur](https://hack.ethkl.org/) conference & hackathon

- Oct 21 – [Ethereum México](https://twitter.com/ethereum_mexico/status/1684649652639924224)

- Oct 22-24 – [ETH Hong Kong](https://www.ethhongkong.co/)

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Oct 27-29 – [ETH Vietnam](https://www.eth-vietnam.com/)

- Oct 27-29 – [ETH London](https://www.encode.club/eth-london) hackathon

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) deadline (max $1k for local meetups)

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://lu.ma/ethbrno3)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 16-19 – [Pragma](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

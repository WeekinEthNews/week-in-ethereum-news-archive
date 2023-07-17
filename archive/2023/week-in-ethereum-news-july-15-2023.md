---
title: "Week in Ethereum News <br> July 15, 2023"
date: "2023-07-15"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=fBVIGBrKaFA&t=18s). Notes from [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-consensus-call-113/):
    - Dencun updates: devnet 7 had [9k blobs](https://blobscan.com/), mostly stable, excludes Erigon; [devnet 8](https://notes.ethereum.org/@ethpandaops/dencun-devnet-8) will be spun up after Hive tests pass & a local testnet run
    
    - Next CL upgrade named Electra; [proposed Electra EIPs so far](https://github.com/ethereum/consensus-specs/issues/3449): EIP7002 (EL triggerable exits), EIP6110 (supply validator deposits on chain) & EIP7251 (increase max effective balance)
    
    - Discussion on active validator set growth & proposal to cap validator churn limit

- EIP4844:
    - Latest EIP4844 implementer call. Notes from [Terence](https://twitter.com/terencechain/status/1678447832217395203): devnet 7 blob spamming, devnet 8 planning, blob retrieval endpoint usefulness for L2s & tuning blob gossip parameters
    
    - [KZG Ceremony](https://ceremony.ethereum.org/) 120k contributions, closes July 23

**Layer 1**

- Erigon [updated 2023 roadmap](https://twitter.com/erigoneth/status/1677731373262446597): single major EL upgrade and Caplin (CL client)

- [Curdleproofs](https://github.com/jsign/go-curdleproofs#readme): Go implementation of Whisk for secret single leader election (SSLE)

**Client releases**

- Consensus layer:
    - Prysm [v4.0.7](https://github.com/prysmaticlabs/prysm/releases/tag/v4.0.7): optimizations include faster slot 0 block proposal, improved fork choice attestation/aggregation using background routines and reduced lock surface

- Execution layer:
    - Nethermind [v1.20.0](https://github.com/NethermindEth/nethermind/releases/tag/1.20.0): improved logs with color, faster snap sync & improved full pruning
    
    - Reth [v0.1.0-alpha.3](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.3): hotfix for Grafana metrics

**For Stakers**

- [Ethstakers.club](https://ethstakers.club/) beacon explorer, beta, open source using PostgreSQL & Charts.js, MIT license

- [Intel](https://www.servethehome.com/intel-exiting-the-pc-business-as-it-stops-investment-in-the-intel-nuc/) exiting NUC business

**Research**

- [EF Research team AMA](https://www.reddit.com/r/ethereum/comments/14vpyb3/ama_we_are_ef_research_pt_10_12_july_2023/), discussions on: EIP7002 (EL triggerable exits), RANDAO manipulation, DVT, EIP7251 (increase max effective balance), SSLE, re-staking, technical roadmap, [MEV as a solved research problem](https://www.reddit.com/r/ethereum/comments/14vpyb3/comment/jrny7o2), easier staking, upgrades, [one-shot signatures](https://www.reddit.com/r/ethereum/comments/14vpyb3/comment/jrnyxa8/), zk, EF, EIP4844, execution sharding and rollups

- [RANDAO manipulation analysis](https://ethresear.ch/t/selfish-mixing-and-randao-manipulation/16081): no large-scale manipulation detected, manipulators could face social-slashing

- [Parallel EVM via claim verification](https://rakita.github.io/blog/blog/parallel-evm-claim/): ensure no inconsistencies when transactions are run in parallel

- EF Robust Incentives Group [posts, papers & talks](https://efdn.notion.site/Robust-Incentives-Group-homepage-802339956f2745a5964d8461c5ccef02)

**Layer 2**

- [Cross-chain communication](https://taiko.mirror.xyz/ryYEi4gAeOWwyERqYTs7CPbNEOYXaEeiMEui6gdlnyg): different approaches by L2s

- [Polygon zkEVM vulnerability disclosed](https://twitter.com/SpearbitDAO/status/1679189382907953180) (fixed), insufficient validation of division remainders

**EIPs/Standards**

- EIPs:
    - [Meta EIP7329](https://github.com/ethereum/EIPs/pull/7329/files): ERC/EIP repository split 

- ERCs (application layer):
    - [ERC7303](https://github.com/ethereum/EIPs/pull/7303/files): Token-controlled token circulation
    
    - [ERC7322](https://github.com/ethereum/EIPs/pull/7322/files): Soulbounds with recoverability
    
    - [ERC7331](https://github.com/ethereum/EIPs/pull/7331/files): Private equity

* * *

### **This newsletter is made possible thanks to** [**Sablier**](https://sablier.com/)

![Sablier](https://weekinethereumnews.com/wp-content/uploads/2023/07/Sablier-banner-1024x307.png)

Sablier V2 is a next-generation token streaming protocol that doubles down on our flagship Lockup design.

V2 pushes the boundaries of web3 payment protocols:

- Non-linear streaming: exponentials, logarithms, or any other curve

- Every stream is a transferable NFT

- Third-party UIs can monetize their Sablier integration with broker fees

[Introducing Sablier V2](https://twitter.com/Sablier/status/1679567031795056645)

* * *

**Stuff for developers**

- Foundry:
    - Forge-std [v1.6.0](https://github.com/foundry-rs/forge-std/releases/tag/v1.6.0): adds cheat codes readCallers, deployCodeTo, skip(bool) & assumeAddressIsNot and adds checked\_write\_int to StdStorage
    
    - [Branching tree technique](https://twitter.com/PaulRBerg/status/1679914755014942720) for Solidity tests
    
    - Tip: [ABI encode constructor arguments](https://twitter.com/paulrberg/status/1679184862928830479) with cast

- Hardhat [v2.17.0](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.17.0): adds support for solc v0.8.19/20 and Node v20

- [SSTORE3](https://github.com/philogy/sstore3#readme): library for Code-as-Storage (CaS) pattern, pointer can be packed with other variables

- [Diffusc](https://blog.trailofbits.com/2023/07/07/differential-fuzz-testing-upgradeable-smart-contracts-with-diffusc/): compare upgradeable contract implementations using static analysis & differential fuzzing

- [Temo](https://github.com/wolovim/temo#readme): example of block/account/contract functionality in a terminal UI; uses Ape, Anvil & Textual

- Curta CTF [Ping Pong solution](https://twitter.com/exp_table/status/1678260264893026305)

- [Private market](https://github.com/dmpierre/eth-private-market#readme): demo using zk-snarks to sell private keys, signatures and groth16 proofs

- RareSkills: [converting algebraic circuits to R1CS](https://www.rareskills.io/post/rank-1-constraint-system)

- [Circom-mutator](https://github.com/aviggiano/circom-mutator#readme): mutation testing tool for Circom

**Security**

- [Rodeo Finance $880k exploit](https://medium.com/@Rodeo_Finance/rodeo-post-mortem-overview-f35635c14101) on Arbitrum via TWAP oracle manipulation

- [Arcadia Finance $460k exploit](https://arcadiafinance.medium.com/post-mortem-72e9d24a79b0) on mainnet & Optimism via reentrancy

- [Libertify $450k exploit](https://twitter.com/peckshield/status/1678688731908411393) on mainnet & Polygon POS via reentrancy

- Ethscriptions [marketplace exploit](https://twitter.com/dumbnamenumbers/status/1679259067833786374), ownership of deposits could not be validated

- Trail of Bits: [evaluating codebase security maturity](https://blog.trailofbits.com/2023/07/14/evaluating-blockchain-security-maturity/)

- PRBMath [signed multiplication-and-division vulnerability](https://medium.com/certora/problems-in-solidity-fixed-point-libraries-certora-bug-disclosure-987f504daca4) disclosed

**Ecosystem**

- [Active validators reach 655k](https://twitter.com/nanexcool/status/1678055882708463616), churn limit increased to 10 activations/exits per epoch

- Ethereum.org [Q3 website roadmap](https://github.com/ethereum/ethereum-org-website/issues/10666)

- Etherscan [similar contract search](https://twitter.com/etherscan/status/1678387777254346754) updated

- ETHBarcelona [hackathon winners](https://ethbarcelona.devfolio.co/projects?show_winners=true)

**Enterprise**

- Central Bank of Brazil [CBDC pilot GitHub repo](https://twitter.com/0xCygaar/status/1678818653305819136)

**Notable at app layer**

- [Sablier v2](https://medium.com/sablier/introducing-sablier-v2-b72f1aa7e458) (token streaming): streams represented as transferable NFTs, adds non-linear streams, cliff support, batch creation and third parties can charge broker fees

- [Safe](https://safe.mirror.xyz/rjWPvQjH9XEC2bADp-9Q1ZEW675pMu41hWsoX5v0Ros) (multisig) adds ERC4337 support for account abstraction

- [CoW Hooks](https://blog.cow.fi/cow-hooks-you-are-in-control-480ccb40044a): pre & post swap intents can be executed with swaps in single transaction

- 0age [Ret↵rn](https://twitter.com/z0age/status/1678775028270370822): onchain generative audiovisual (SVG & Web Audio) NFT \[Evan & Andrew minted\]

- [Sound](https://sound.mirror.xyz/W5F4DasupahnF_AyT5TwXSzKWJcOqHLuxf9nI0piPOE) (Music NFTs) open to all artists

* * *

### Job Listings

- EF Privacy & Scaling Explorations team seek [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [SEC vs Ripple summary judgment](https://twitter.com/jbsdc/status/1679620520155783169): institutional sales were securities transactions but programmatic sales & distributions to employees were not

- [Alex Mashinsky](https://www.justice.gov/usao-sdny/pr/celsius-founder-and-former-chief-revenue-officer-charged-connection-multibillion) (former Celsius CEO) charged with fraud 

- Euler hacker apparently [arrested and held in French jail](https://www.dlnews.com/articles/defi/argentinian-euler-hacker-explains-exploit-from-a-paris-jail)

- [OpenSea spoofer](https://www.justice.gov/usao-sdny/pr/defendant-charged-theft-cryptocurrency-and-nfts-through-spoofing-opensea-marketplace) charged with wire fraud

- [Google Play policy](https://android-developers.googleblog.com/2023/07/new-blockchain-based-content-opportunities-google-play.html) updated to allow use of NFTs within Android apps & games

- [Bluechip](https://bluechip.org/news/stablecoin-rating-platform-bluechip-launches): stablecoin rating agency

- Ethereum [Q2 results](https://samuelandrew.substack.com/p/ethereum-q223-state-of-the-network) imagined as a quarterly earnings release, fees grew 56% quarter-on-quarter

* * *

### Evan’s new podcast: web3 Builders

- Subscribe to [web3 Builders](https://podcasters.spotify.com/pod/show/web3builderspodcast) podcast. There may be a Week in Ethereum News audio version

* * *

**General**

- [Multichain](https://twitter.com/multichainorg/status/1679768407628185600) bridge CEO & sister allegedly in custody, MPC nodes were run on CEO’s personal cloud server account

- [Polygon propose MATIC token upgrade](https://polygon.technology/blog/polygon-2-0-tokenomics), 1% emission for validator rewards on Polygon chains & 1% for a community treasury

- Flashbots [MEVM](https://writings.flashbots.net/mevm-suave-centauri-and-beyond): EVM with MEV precompiles to enable rewriting offchain MEV infrastructure as contracts on upcoming SUAVE

- Apple WebKit [zero-day](https://www.bleepingcomputer.com/news/apple/apple-re-releases-zero-day-patch-after-fixing-browsing-issue/), arbitrary code execution via malicious web page content

- Justin Thaler: [17 SNARK misconceptions](https://a16zcrypto.com/posts/article/17-misconceptions-about-snarks/)

- [Fiat-Shamir security](https://eprint.iacr.org/2023/1071) of FRI & family of FRI-based protocols including Plonky2 & ethSTARK

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-15-2023](https://weekinethereumnews.com/week-in-ethereum-news-july-15-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jul 17 – [CLRFund round 9](https://blog.clr.fund/round-9-is-underway/) ends

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 20–23 – [Pragma Paris](https://ethglobal.com/events/pragma-paris) & [ETHGlobal Paris](https://ethglobal.com/events/paris2023) hackathon

- Jul 23 – [KZG Ceremony](https://ceremony.ethereum.org/) closes

- Aug 11-13 – [ETHMunich](https://ethmunich.de/) hackathon

- Aug 15-16 – [ETHToronto](https://www.ethtoronto.ca/) & [ETHWomen](https://www.ethwomen.com/)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org/) (Buenos Aires)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 31 - Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- **Sep 7-9 –** [**ETHAccra**](https://www.ethaccra.xyz/) **hackathon**

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 15-17 – [ETHChicago](https://www.ethchicago.xyz/) conference & hackathon

- Sep 18-21 – [ETH Montréal](https://ethmontreal.xyz/) conference & hackathon

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 6-27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 13-15 – [Ethereum Kuala Lumpur](https://hack.ethkl.org/) conference & hackathon

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) application deadline

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://twitter.com/ethbrno/status/1652198745902137344)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 17-19 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

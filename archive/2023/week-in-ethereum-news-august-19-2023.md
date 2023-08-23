---
title: "Week in Ethereum News <br> August 19, 2023"
date: "2023-08-19"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=DyAtbK2MQG4&t=49s). Recap by [Tim Beiko](https://twitter.com/abcoathup/status/1692292943275778261).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1692283671481573538) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-168/):
    - [Devnet-8 launched](https://twitter.com/parithosh_j/status/1691927807230677133) with all Dencun EIPs, Besu & Erigon EL clients still to join
    
    - EIP4788 (beacon block root in EVM) contract to be deployed with a regular transaction
    
    - Holešky testnet to launch with 1.6B HETH supply
    
    - ERCs being split from EIP repo, EIP editors remaining as single group
    
    - EIP7212 (secp256r1 precompile) presented

- [KZG Ceremony](https://ceremony.ethereum.org/) has 138k contributions, lobby closes August 23

**Layer 1**

- Visualization of the [rise of integrated builder searchers](https://twitter.com/specialmech/status/1691178038640492544)

- Dapplion: [Whisk (SSLE) induces missed initial slots](https://hackmd.io/@dapplion/whisk_induced_missed_slots), proposal to fix edge case

**For stakers**

- [Lodestar v1.10 nodes with out of memory errors](https://x.com/lodestar_eth/status/1691495095948980224) should upgrade to nodeJS v20

- [Obol DVT performance testing](https://blog.obol.tech/performance-testing-distributed-validators/): less than 1% difference to traditional validators on testnet

**Client releases**

- Execution layer:
    - Geth [v1.12.2](https://github.com/ethereum/go-ethereum/releases/tag/v1.12.2): regression fixes

**Research**

- Proposed [inclusion list design](https://ethresear.ch/t/no-free-lunch-a-new-inclusion-list-design/16389), split into a proposer signed summary & an unsigned list of transactions, solves free data availability problem

**Layer 2**

- Arbitrum One [batch poster briefly stopped](https://twitter.com/hkalodner/status/1692586523919532348) during gas price spike, users could still make transactions

- [Rollup economics v2](https://davidecrapis.notion.site/Rollups-are-Real-Rollup-Economics-2-0-2516079f62a745b598133a101ba5a3de): running a surplus, cooperatives, federations & layer 3s

**EIPs/Standards**

- [EIP/ERC numbering](https://github.com/ethereum/EIPs/issues/6990#issuecomment-1648535814) changed to be sequential from 7500

- EIPs:
    - [EIP7495](https://github.com/ethereum/EIPs/pull/7495/files): SSZ PartialContainer

- ERCs (application layer):
    - [ERC7484](https://github.com/ethereum/EIPs/pull/7484/files): Registry adapters for smart accounts
    
    - [ERC7492](https://github.com/ethereum/EIPs/pull/7492/files): ERC20Spendable (ERC20 extension)
    
    - [ERC7500](https://github.com/ethereum/EIPs/pull/7500/files): NFT dynamic traits
    
    - [ERC7501](https://github.com/ethereum/EIPs/pull/7501/files): NFT redeemables

* * *

### **Check out Evan’s new podcast:** [**web3 Builders**](https://podcasters.spotify.com/pod/show/web3builderspodcast)

![Web3 Builders](https://weekinethereumnews.com/wp-content/uploads/2023/08/Web3-Builders.webp)

On the latest weekly show Evan and Will discuss Tether abandoning Bitcoin, timelines for Dencun/danksharding/getting our under 5 cent transaction fees, rollups piling on Optimism, Gitcoin + BigOil and Evan’s user review of FriendTech.

Watch web3 builders episodes on [YouTube](https://www.youtube.com/@web3builderspod), or listen on [Apple](https://podcasts.apple.com/us/podcast/web3-builders/id1697252853), [Spotify](https://podcasters.spotify.com/pod/show/web3builderspodcast) or [RSS](https://anchor.fm/s/e5abffc8/podcast/rss).  Or get pinged for new episodes on [Telegram](http://t.me/web3builderspod) or [Substack](https://web3builderspod.substack.com/).

Please like, subscribe, and share on social media if you enjoyed the episode. 

* * *

**Stuff for developers**

- Remix [v0.35.0](https://medium.com/remix-ide/remix-release-v0-35-0-9d955a9c853d): adds quick fix functionality for license, visibility & mutability

- Foundry:
    - [SKS](https://github.com/Will-Smith11/sks#readme): package manager script to install dependencies instead of submodules
    
    - Tip: [use src in contract import paths](https://x.com/paulrberg/status/1692245880584142978) for compatibility with Hardhat

- OpenZeppelin Contracts low-severity issue: [ERC2771Context used with custom forwarder](https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-g4vp-m682-qqmp) may lead to zero address \_msgSender, patched in v4.9.3

- RareSkills: [Solidity style guide](https://www.rareskills.io/post/solidity-style-guide)

- [Vyper clones with immutable arguments](https://github.com/banteg/vyper-cwia#readme): example contract compatible with CWIA proxy factory

- [ERC6909](https://twitter.com/bantg/status/1692239278158352778) (minimal multi-token interface) implemented in Vyper

- [Sol2uml diff](https://twitter.com/naddison/status/1692178021061738706) can compare Etherscan verified contracts to local files

- WhatsABI [v0.7](https://github.com/shazow/whatsabi/releases/tag/v0.7.0) (guesses ABI from bytecode): adds proxy contract support

- heimdall-rs [v0.5.0](https://twitter.com/BeckerrJon/status/1690453110265892865) adds contract snapshot module

- Nethereum [v4.16](https://github.com/Nethereum/Nethereum/releases/tag/4.16.0) (.NET): adds data services package to interact with Etherscan/Sourcify/4Bytes, multi query using RPC batching and extra extensions for ABI decoding & ABI storage

- [Wallet test framework](https://wtf.allwallet.dev/week-19/) testing the tests: currently requires window.ethereum (excludes mobile wallets) & custom network support

- Cryo [v0.2](https://github.com/paradigmxyz/cryo/releases/tag/0.2.0) (extract blockchain data): adds python adapter, contracts & native\_transfers datasets, transaction selectors, command chaining and summary report

- [Advanced guide to Dune SQL](https://web3datadegens.substack.com/p/advanced-wizard-guide-to-dune-sql) & Ethereum data analytics

- [ERC5564 (stealth addresses) bn254](https://github.com/rymnc/erc-5564-bn254#readme): generate derivable commitments for users belonging to other membership sets and add them to others, using arkworks-rs & RLN

**Security**

- Exactly Protocol on Optimism [$7M exploit](https://twitter.com/BlockSecTeam/status/1692533280971936059) via unverified input

- Zunami Protocol [$2M exploit](https://twitter.com/BlockSecTeam/status/1690931111776358400), price manipulation by donation

- RocketSwap on Base [$870k exploit](https://twitter.com/rocketswap_labs/status/1691229656593371136), deployer private key compromised

- [Auditor toolbox](https://hackmd.io/@Deivitto/The-Auditor-Toolbox): docker with Foundry, Halmos, Heimdall, Slither, Echidna & Mythril etc

- [Audit wizard](https://www.auditwizard.io/blog/audit-wizard-beta-launch): use contract address or GitHub, scan with Slither, view AST & generate graph, beta

- Trail of Bits: [Rekt Test](https://blog.trailofbits.com/2023/08/14/can-you-pass-the-rekt-test/) 12 yes/no questions for a project to assess security (modeled on Joel Test)

**Ecosystem**

- [Gitcoin Grants 18](https://www.gitcoin.co/blog/announcing-gitcoin-grants-18) is open

- [EF Q2 grantees](https://blog.ethereum.org/2023/08/15/allocation-update-q2-23) share $9 million in funding

- ETHGlobal [Superhack (OP Stack) finalists](https://twitter.com/ETHGlobal/status/1692603548180132114)

- ETHMunich [hackathon winners](https://twitter.com/ethmunich/status/1692603827550122004)

**Enterprise**

- Zynga [Sugartown](https://visitsugartown.com/faq) gaming platform announced, access via free mint of Ora NFTs

- [Shell](https://www.gitcoin.co/blog/gitcoin-shell-collaboration) donating to Gitcoin Grants climate solutions rounds; [Gitcoin](https://x.com/kbw/status/1691797028987162874) provides context

**Notable at app layer**

- OpenSea [creator royalties](https://opensea.io/blog/articles/creator-fees-update) being made optional, includes L2 & NFTs using marketplace filter

- CoW Swap [Time-Weighted Average Price (TWAP) orders](https://blog.cow.fi/cow-swap-launches-twap-orders-d5583135b472)

- [Connext governance token](https://blog.connext.network/announcing-the-next-airdrop-be764b1c548), airdrop is crosschain using xERC20

- Anish’s [FriendMEX](https://twitter.com/_anishagnihotri/status/1690455865382318081), pro style interface for Friend Tech on Base, no invite code needed

- [Brian Armstrong](https://twitter.com/brian_armstrong/status/1690790384757321728): Coinbase need to improve app UX for NFTs, Dapps & L2s

* * *

### Job Listings

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Bloomberg claims [SEC will allow Ether futures ETFs by October](https://archive.is/REUyS)

- Coinbase-funded [challenge to OFAC's Tornado Cash action](https://twitter.com/iampaulgrewal/status/1692260842585350334) loses in district court, on to 5th Circuit

- [FBI warns](https://www.ic3.gov/Media/Y2023/PSA230811) about increase in crypto recovery scams

- Singapore [stablecoin regulatory framework](https://www.mas.gov.sg/news/media-releases/2023/mas-finalises-stablecoin-regulatory-framework), issuer requirements include: value stability, minimum base capital, redemption at par and disclosure

- [PayPal pausing UK crypto purchases](https://www.reuters.com/technology/paypal-halt-uk-crypto-sales-until-2024-2023-08-16/) to work on compliance with promotion regulation

- [A left-wing argument](https://archive.is/x6ill) for crypto

- [Coinbase](https://www.coinbase.com/blog/coinbase-financial-markets-inc-secures-fcm-approval-to-bring-regulated) approved in US by National Futures Association to offer crypto futures trading

- US [stand with crypto alliance](https://www.standwithcrypto.org/), donation leaderboard & policy stance of elected officials

**General**

- Patrick McCorry: [crypto in Africa](https://www.cryptofrens.info/p/understanding-crypto-in-africa)

- [ZachXBT defamation lawsuit](https://x.com/zachxbt/status/1691116363891552256) dropped by MachiBigBrother (Jeffrey Huang), article [changed](https://github.com/0xmunger/zachxbt-machi/compare/main...0xmunger-changes?quick_pull=1) (diff), unused donations to be refunded

- [DefinitelySetup simplified trusted setup ceremony](https://twitter.com/privacyscaling/status/1692204728338551028), PR with circuit’s R1CS, wasm & config file

- Vitalik: [X (Twitter) community notes](https://vitalik.eth.limo/general/2023/08/16/communitynotes.html), mechanism design with “crypto values”

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-19-2023](https://weekinethereumnews.com/week-in-ethereum-news-august-19-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Aug 23 – [KZG Ceremony](https://ceremony.ethereum.org/) closes (extended)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 29 – [Gitcoin Grants 18](https://grants.gitcoin.co/) ends (**support** [**Week in Ethereum News**](https://explorer.gitcoin.co/#/round/10/0x2871742b184633f8dc8546c6301cbc209945033e/0x2871742b184633f8dc8546c6301cbc209945033e-122))

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

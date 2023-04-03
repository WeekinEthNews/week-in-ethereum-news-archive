---
title: "Week in Ethereum News <br> April 1, 2023"
date: "2023-04-01"
---

## Eth News and Links

**Shapella (Shanghai + Capella) upgrade**

- Update your nodes ready for [mainnet Shapella upgrade on April 12](https://github.com/ethereum/execution-specs/blob/master/network-upgrades/mainnet-upgrades/shanghai.md#upgrade-schedule), including both your beacon node & validator client

- Consensus layer mainnet releases:
    - Lighthouse [v4.0.1](https://github.com/sigp/lighthouse/releases/tag/v4.0.1)
    
    - Lodestar [v1.7.2](https://github.com/ChainSafe/lodestar/releases/tag/v1.7.2)
    
    - Nimbus [v23.3.2](https://github.com/status-im/nimbus-eth2/releases/tag/v23.3.2)
    
    - Prysm [v4.0.1](https://github.com/prysmaticlabs/prysm/releases/tag/v4.0.1)
    
    - Teku [v23.3.1](https://github.com/ConsenSys/teku/releases/tag/23.3.1)

- Execution layer mainnet releases:
    - Besu [v23.1.2](https://github.com/hyperledger/besu/releases/tag/23.1.2)
    
    - Erigon [v2.42.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.42.0)
    
    - Geth [v1.11.5](https://github.com/ethereum/go-ethereum/releases/tag/v1.11.5)
    
    - Nethermind [v1.17.3](https://github.com/NethermindEth/nethermind/releases/tag/1.17.3)

- MEV-Boost [v1.5.0](https://github.com/flashbots/mev-boost/releases/tag/v1.5.0)

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=RQ2WtyevRXE&t=106s). Summary by [Tim Beiko](https://twitter.com/abcoathup/status/1641600018145746944).  Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1641501763349155840) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-execution-call-158/):
    - Final Shapella mainnet shadow fork planned for next week
    
    - Flag for EL to suggest CL override external builder to be added before Cancun
    
    - SELFDESTRUCT removal (EIP6780) added as Cancun candidate
    
    - EOF spec updated to avoid code & gas observability, too big to include in Cancun
    
    - Proposal for trust-minimized CL access from EL inside the EVM 
    
    - Verkle trees readiness discussion for Prague upgrade

- EF [mainnet Shapella announcement](https://blog.ethereum.org/2023/03/28/shapella-mainnet-announcement)

**For Stakers**

- Beacon chain withdrawals [technical explainer](https://twitter.com/icebearhww/status/1641371721755398144)
    - [When to broadcast](https://hackmd.io/@potuz/H1P8X5xZn) BLS address change

- [Switch to a smaller pool after Shapella](https://twitter.com/dannyryan/status/1641679529188925442) to make Ethereum more resilient

- [Orange Pi 5 running Geth+Lighthouse](https://twitter.com/ethereumonarm/status/1640977418264379395), 139 €, syncs in ~27 hours

- [Mac mini M1 running Geth+Nimbus](https://twitter.com/ethereumonarm/status/1640375236418732034), syncs in ~18 hours

**Layer 2**

- [Polygon zkEVM mainnet beta](https://polygon.technology/blog/polygon-zkevm-mainnet-beta-is-live), gas pricing as EVM but lacks some precompiles, Security Council initially, AGPL v3 license

- [Linea](https://linea.mirror.xyz/6G30hwV2wPs_wPv0VEgHYaIdghMkIQaad-OI_0br1hM) (ConsenSys zkEVM) testnet now public

- Conduit [managed rollups](https://conduit.xyz/blog/introducing-conduit) using OP Stack, with block explorer, RPCs, metrics & transaction tracer

- L2BEAT [risk rosette](https://twitter.com/l2beat/status/1640302851900465154): visualization of risks

**EIPs/Standards**

- EIPs:
    - [EIP6780](https://eips.ethereum.org/EIPS/eip-6780): SELFDESTRUCT only in same transaction
    
    - [EIP6789](https://github.com/ethereum/EIPs/pull/6789/files): Rename gas to mana \[resurrected EIP102\]
    
    - [EIP6800](https://github.com/ethereum/EIPs/pull/6800/files): Ethereum state using a unified verkle tree

- ERCs:
    - [ERC6785](https://github.com/ethereum/EIPs/pull/6785/files): ERC721 utilities extension
    
    - [ERC6786](https://github.com/ethereum/EIPs/pull/6786/files): Registry for royalties payment for NFTs
    
    - [ERC6787](https://github.com/ethereum/EIPs/pull/6787/files): Order book DEX with two phase withdrawal
    
    - [ERC6806](https://github.com/ethereum/EIPs/pull/6806/files): ERC721 holding time tracking
    
    - [ERC6808](https://github.com/ethereum/EIPs/pull/6808/files): Fungible key bound token
    
    - [ERC6809](https://github.com/ethereum/EIPs/pull/6809/files): Non-fungible key bound token

* * *

### **This newsletter is made possible thanks to** [**Scaffold-Eth-2 hackathon**](https://hackathon.buidlguidl.com/)**!**

![Scaffold-Eth-2 hackathon](https://weekinethereumnews.com/wp-content/uploads/2023/04/Scaffold-Eth-2-hackathon-1-1024x576.jpg)

**BuidlGuidl presents:** [**Scaffold-Eth 2 hackathon**](https://hackathon.buidlguidl.com/)**.**

This is a great opportunity to build a prototype in a few days. There's no sign-up required, simply build something & submit it before April 8.

You can hack solo, bring a crew, or find a friend in the [Telegram Group](https://t.me/+-fGZ-MJ_UZ41MGUx) to work with.

To submit your project, all you need to do is record a short video showcasing your app and add it to the top of the README.md file in your repo along with the live URL. Submissions open on April 7.

* * *

**Stuff for developers**

- Foundry tip: [warp to present time in base test setup function](https://twitter.com/paulrberg/status/1641751420494856192) for more realistic testing

- [Vulcan template](https://github.com/nomoixyz/vulcan-template#readme): Foundry template using Vulcan development framework

- [Protect against donation attacks](https://twitter.com/naddison/status/1640549868442902528) on ERC4626 vaults & liquidity pools

- [Gambit](https://medium.com/certora/gambit-23ef5cab02f5): Solidity mutation generator in Rust, integrated with Certora Prover

- Curta CTF: what are buckets [solution](https://hackmd.io/@xNSnimr_Rk68TArjAjMQvw/HkypUNJW2)

- [Decipher EVM puzzles](https://github.com/zaryab2000/decipher_EVM_Puzzles?ref=zaryabs.com#readme): extension of Franco’s EVM puzzles

- [Ethereum-indexer](https://github.com/jolly-roger-eth/ethereum-indexer#readme): in-browser indexer in TypeScript for use in games/apps, [demo](https://jolly-roger-eth.github.io/ethereum-indexer/examples/#home)

- [P256 on EVM](https://twitter.com/Cometh/status/1641728767864320001): demo of user onboarding, wallet creation using WebAuthn

- [Arbiter v0.1.0](https://github.com/primitivefinance/arbiter#readme): agent based analysis tool in Rust, beta

- Ethereum Attestation Service [private data attestations](https://mirror.xyz/0xeee68aECeB4A9e9f328a46c39F50d83fA0239cDF/BiFUEFJKo6ZsIvPwsP9WPC2UZX0-x_9BdtrvmQo1FwY) using Merkle Trees

**Security**

- Tincho found [ENS DNSSEC vulnerability](https://blog.theredguild.org/how-to-almost-take-over-any-dns-domain-on-ens/) in undeployed code, any DNSSEC name could be taken over, 100k bounty recommended

- DAO [gas refund vulnerability](https://twitter.com/zachobront/status/1641105461389795328), refund pots can be drained for DAOs with inexpensive tokens

- Euler exploiter [returning funds](https://twitter.com/tayvano_/status/1640418058148917250)

- [Overview of sleuthing tools](https://community.thecreed.xyz/c/warez/sleuthing-toolbox-everything-you-need-to-reverse-engineer-web3-hacks): Phalcon, MetaSleuth, Transaction tracer, ethtx and Tenderly

**Ecosystem**

- Optimism’s retroactive public goods funding [round 2 recipients announced](https://optimism.mirror.xyz/Upn_LtV2-3SviXgX_PE_LyA7YI00jQyoM1yf55ltvvI?rpgf), 10 million OP shared by 195 projects

- Vitalik: [SNARK-verify layer 1](https://vitalik.eth.limo/general/2023/03/31/zkmulticlient.html) using multiple Type 1 zkEVMs

- [Etherscan](https://twitter.com/etherscan/status/1640327680179712000) adds option to use local time zone for time stamps

- ETHGlobal [Scaling Ethereum finalists](https://twitter.com/ethglobal/status/1641821457943605252)

**Enterprise**

- [Ticketmaster testing NFT gated ticket sales](https://decrypt.co/124607/ticketmaster-debuts-nft-gated-ticket-sales-starting-avenged-sevenfold) with metal band Avenged Sevenfold

**Notable at app layer**

- [Maker](https://vote.makerdao.com/polling/Qmbndmkr#vote-breakdown) voted for its constitution

- [DeFi Saver](https://twitter.com/DeFiSaver/status/1640387846069686278) adds limit orders & DCA strategies

- [Sound Swap](https://sound.mirror.xyz/sZSBTW1J4MS-6LQsVklaXaGceeC-kDIcUSDCHvTEqws) (music NFTs): 24 hour open editions & increasing price mints with instant selling

* * *

### Job Listings

- EF Ecosystem Support Program seek a [Grant Analyst & Liaison](https://jobs.lever.co/ethereumfoundation/92306cf4-1a7d-4e32-bc23-9762383522b1)

- [Nimbus](https://nimbus.team/#about) is hiring a [Site Reliability Engineer](https://jobs.status.im/?gh_jid=4797968)

- L2BEAT 💗 is hiring a Senior Software Engineer & Product Owner. [Apply here!](https://l2beat.notion.site/We-are-hiring-Work-at-L2BEAT-e4e637265ae94c5db7dfa2de336b940f)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [CFTC charged Binance & CZ](https://www.cftc.gov/PressRoom/PressReleases/8680-23) with law evasion & operating illegal derivatives exchange

- [FDIC wants former Signature Bank crypto customers](https://www.coindesk.com/policy/2023/03/28/fdic-gives-deadline-next-week-for-crypto-depositors-stranded-by-signature-failure/) to cash out by April 5

- [Bittrex exchange shutting US operations](https://bittrex.com/discover/important-message-for-bittrex-u-s-customers) due to regulatory uncertainty

- [NFT MEV strategies](https://frontier.tech/the-nft-mev-landscape): mints, arbitrage & liquidations

**General/crypto**

- [Near-Ultrasound Inaudible Trojan](https://sites.google.com/view/nuitattack/home): play commands at 16kHz-20kHz to attack voice assistants 

- [Bing CMS exploit](https://twitter.com/hillai/status/1641146508639600646) allowed take over of Office 365 accounts

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-april-1-2023](https://weekinethereumnews.com/week-in-ethereum-news-april-1-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Apr 5-8 – [ETH Beijing](https://www.ethbeijing.xyz/) hackathon

- **Apr 8 – deadline for** [**Scaffold-Eth-2 hackathon**](https://hackathon.buidlguidl.com/)

- Apr 12 – [Mainnet upgrades to Shapella](https://github.com/ethereum/execution-specs/blob/master/network-upgrades/mainnet-upgrades/shanghai.md#upgrade-schedule)

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- Apr 13-16 – [Pragma Tokyo](https://ethglobal.com/events/pragma-tokyo) & [ETHGlobal Tokyo](https://tokyo.ethglobal.com/) hackathon

- Apr 14-16 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference & hackathon

- Apr 21-25 – [EthTaipei](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) hackathon & conference

- Apr 27-30 – [Istanbul ETH Privacy](https://www.leadingprivacy.com/istanbul) conference & hackathon

- Apr 28 – deadline for EF’s [Next Billion fellowship cohort 3](https://blog.ethereum.org/2023/03/16/fellowship-cohort-3-applications)

- May 5-10 – [ETHTallinn](https://ethtallinn.org/) hackathon & [NFT Tallinn](https://nfttallinn.com/) conference

- May 9-12 – [EY blockchain summit](https://web.cvent.com/event/c066d44d-4e50-4d7e-b6fb-3cc0abdae7ff/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7)

- May 12-14 – [ETHGlobal Lisbon](https://ethglobal.com/events/lisbon)

- May 19-23 – [EDCON](https://edcon.io/) Montenegro (changed from Vienna)

- May 20-21 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 24-26 – [Spaghett ETH](https://naples.spaghett-eth.com/) (Naples) conference

- May 26-28 – [ETHDublin](https://www.ethdublin.io/) hackathon

- Jun 2-4 – [ETH Seoul](https://2023.ethseoul.org/)

- Jun 2-6 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 9-11 – [ETHPrague](https://ethprague.com/) conference & hackathon

- Jun 23–25 – [ETHGlobal Waterloo](https://ethglobal.com/events/waterloo2023) (changed from Toronto)

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- **Aug 13-16 –** [**ETHToronto**](https://www.ethtoronto.ca) **&** [**ETHWomen**](https://www.ethwomen.com/)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org) (Buenos Aires)

- **Aug 28-30 –** [**Science of Blockchain Conference**](https://cbr.stanford.edu/sbc23/) **(Stanford University)**

- Aug 30 - Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- **Oct 27–29 –** [**ETH Miami**](https://ethmiami.net/) **festival + hackathon**

- Oct 28–30 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- **November – Devconnect**

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

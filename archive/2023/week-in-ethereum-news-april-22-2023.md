---
title: "Week in Ethereum News <BR> April 22, 2023"
date: "2023-04-21"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- A list of what [exactly might make it into Dencun](https://ethereum-magicians.org/t/cancun-network-upgrade-meta-thread/12060) besides 4844 (protodankscaling). Discussion at the next call on April 27

- Latest [consensus layer devs call](https://www.youtube.com/watch?v=tJULkA5YgP4). Notes from [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-consensus-call-107/)
    - [EIP4788](https://eips.ethereum.org/EIPS/eip-4788) (expose CL state in EL) likely included in Dencun
    
    - 4844 devnet5 next week
    
    - discussion of [long-lived subnets](https://github.com/ethereum/consensus-specs/pull/3312) to reduce bandwidth use

- Latest [4844 implementor call](https://youtu.be/oCqfxb5CWAI)

- [KZG ceremony](https://ceremony.ethereum.org/) is open again for public contributions, but your Eth account needs over 128 mainnet transactions. If the waiting list declines, then the threshold will be reduced. [Follow @carlbeek](https://twitter.com/CarlBeek/status/1647752476328878080) to find out if threshold is reduced

**Layer 1**

- Four options for [transitioning to Verkle trees](https://notes.ethereum.org/@parithosh/verkle-transition) would look like

- [Two slots proposer builder separation with unconditional payment](https://hackmd.io/rin5jq_ITA2TBuWjAn0OxA)

- [Paprika](https://github.com/NethermindEth/Paprika), Nethermind’s experimental storage abstraction of Patricia tree

- [Equivocation attacks in MEV-boost and ePBS](https://ethresear.ch/t/equivocation-attacks-in-mev-boost-and-epbs/15338)

- [Optimistic relays increase validator profits and are cheaper to maintain](https://frontier.tech/optimistic-relays-and-where-to-find-them)

**For Stakers**

- How to [track the performance of your validator](https://offchain.medium.com/validator-performance-tracking-a2ea9ab44b3a)

- Benchmarking [bandwidth consumption with Shapella](https://decentralfocus.substack.com/p/bandwidth-usage-after-ethereum-withdrawals) (Geth and Lighthouse) finds ~20% increase

- Lighthouse [v4.1](https://github.com/sigp/lighthouse/releases/tag/v4.1.0) - fix excessive CPU usage

- Geth [v.1.11.6](https://github.com/ethereum/go-ethereum/releases/tag/v1.11.6)

- Rocketpool [Atlas upgrade](https://medium.com/rocket-pool/rocket-pool-atlas-upgrade-7c69e39a3d5f) live, allows staking with 8 ETH and triples Rocketpool’s capacity

- [How to start running a distributed validator](https://medium.com/dsrv/validators-note-10-how-to-start-running-a-distributed-validator-with-obol-f7c9179cbd7e) with Obol

**Layer 2**

- Client diversity coming with Optimism’s Bedrock upgrade:
    - Magi, a16z’s [Optimism client](https://a16zcrypto.com/content/article/building-magi-a-new-rollup-client-for-optimism/) in rust
    
    - [OP-Erigon](https://dev.optimism.io/client-diversity/), a fork of Erigon for Optimism

**EIPs/Standards**

- EIPs:
    - [EIP6888](https://github.com/ethereum/EIPs/pull/6888/files): EVM math checking
    
    - [EIP6913](https://github.com/ethereum/EIPs/pull/6913/files): SETCODE instruction
    
    - [EIP6914](https://github.com/ethereum/EIPs/pull/6914/files): Reuse withdrawn validator indices

- ERCs:
    - [ERC6882](https://github.com/ethereum/EIPs/pull/6882/files): sharable interface for borrowing
    
    - [ERC6884](https://github.com/ethereum/EIPs/pull/6884/files): Extendable Utility Tokens Derived from Origin NFTs
    
    - [ERC6916](https://github.com/ethereum/EIPs/pull/6916/files): Automatic reset of testnet
    
    - [ERC6912](https://github.com/ethereum/EIPs/pull/6912/files): Versioned TokenIDs for Dynamic NFTs
    
    - [ERC6909](https://github.com/ethereum/EIPs/pull/6909/files): simplified alternative to erc1155
    
    - [ERC6900](https://github.com/ethereum/EIPs/pull/6900/files): modular smart contracts

* * *

### **This newsletter is made possible thanks to the funding received from Optimism’s** [**RetroPGF**](https://optimism.mirror.xyz/Upn_LtV2-3SviXgX_PE_LyA7YI00jQyoM1yf55ltvvI?rpgf)**!**

[![](https://substackcdn.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F4f7fe68c-119b-4dfd-879f-1beb68fd6311_1500x800.png)](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F4f7fe68c-119b-4dfd-879f-1beb68fd6311_1500x800.png)

Thank you to [Optimism’s RetroPGF round 2](https://optimism.mirror.xyz/Upn_LtV2-3SviXgX_PE_LyA7YI00jQyoM1yf55ltvvI?rpgf) which generously funded Week in Ethereum News for “months, not weeks.”

* * *

**Stuff for developers**

- viem [v0.3.x](https://github.com/wagmi-dev/viem/releases), bugfixes and ethcall batch aggregation

- wagmi’s [plan for migrating to viem](https://github.com/wagmi-dev/wagmi/discussions/2207)

- [Diamond standard in Foundry](https://medium.com/@urataps/diamond-foundry-a-unified-toolset-for-web3-builders-d4073b6671ea)

- [ZeroMEV API](https://data.zeromev.org/docs/), transaction level MEV summary data

**Security**

- Hundred [hacked for 7.4m](https://rekt.news/hundred-rekt2/) on Optimism, due to poorly deployed fork of compound v2

**Ecosystem**

- [Scaffold-eth v2 hackathon winners](https://twitter.com/buidlguidl/status/1648820996005060608)

- [ETH Tokyo winners](https://twitter.com/ETHGlobal/status/1647524426450083840)

- Gas prices highest this week since the Merge (ie ~80 gwei during UTC day and ~35 gwei during UTC night) lead to [over 100k burned since the Merge](https://twitter.com/evan_van_ness/status/1648904903861960705)

- [Devconnect announced in Istanbul](https://blog.ethereum.org/2023/04/20/announcing-devconnect-ist) for November 13-19

**Enterprise**

- Société Générale launches [Euro stablecoin on mainnet](https://www.sgforge.com/societe-generale-forge-launches-coinvertible-the-first-institutional-stablecoin-deployed-on-a-public-blockchain/)

**Notable at app layer**

- [Kwenta launches SmartMargin](https://mirror.xyz/kwenta.eth/I9l_QSOvf6kGQos3SXltES9WCAvEklS56aIbKHccHUg) and currently has [3 different rewards programs](https://mirror.xyz/kwenta.eth/8KyrISnjOcuAX_VW-GxVqxpcbWukB_RlP5XWWMz-UGk) for traders

- [Use an onchain NFT](https://twitter.com/colingplatt/status/1648673944281464833) as your Uniswap frontend

- Brantly Millegan’s [proposal for an onchain follow protocol](https://twitter.com/BrantlyMillegan/status/1648794925754974209)

- Who is [delegating to you in DAOs](https://www.karmahq.xyz/dao/delegators)?

- Ameen announces [Hai](https://community.reflexer.finance/t/announcing-hai-a-multi-collateral-rai-fork-on-optimism/461), multi-collateral Rai fork on optimism

- Alchemix [self-repaying .eth domains](https://ens.alchemix.fi/)

- State of [zk-apps in Ethereum](https://mirror.xyz/andyguzman.eth/ZZRLBlx2KjlNnQ84v1doMKg_8QO-XRjYxFfT1Fm_ZDw)

- [What can you do with zk-ECDSA](https://mirror.xyz/privacy-scaling-explorations.eth/djxf2g9VzUcss1e-gWIL2DSRD4stWggtTOcgsv1RlxY) at the app layer?

* * *

### Job Listings

- [Snr React Native UI Dev](https://grnh.se/2fada6031us) at Status: [All jobs](https://grnh.se/9fc6e6fc1us)

- Solidity team are looking for a highly skilled [Dev Advocate](https://jobs.lever.co/ethereumfoundation/b9e33c9e-48ee-464f-a672-d51eece2b99d)

- EF Ecosystem Support Program seek a [Grant Analyst & Liaison](https://jobs.lever.co/ethereumfoundation/92306cf4-1a7d-4e32-bc23-9762383522b1)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Coinbase [licensed in Bermuda to launch derivatives exchange](https://archive.ph/Tz4Oa)

- Gensler repeatedly [refuses to say ETH is not a security](https://www.youtube.com/watch?v=VhA1dZXeao0), even though in 2018 he [recognized that ETH was not a security](https://www.youtube.com/watch?v=JPkgJwJHYSc&t=1104s)

- SEC labels [Algorand an unregistered security](https://www.sec.gov/litigation/complaints/2023/comp-pr2023-78.pdf) in complaint against Bittrex.
    - In 2019, [Gary Gensler caught on tape pumping Algorand](https://youtu.be/2D3SbYzzJLc?t=2753)

- Gary Gensler’s [contradiction in the middle](https://leighton.mirror.xyz/eHwKtQneGUCwWxuUflDrYuTW4-d7IjTGrO3ZFVemOTY)

- Europe votes for [uniform legal framework](https://www.europarl.europa.eu/news/en/press-room/20230414IPR80133/crypto-assets-green-light-to-new-rules-for-tracing-transfers-in-the-eu) for EU crypto markets

- Next week [Alex Pertsev to be released to house arrest](https://twitter.com/blockblanc/status/1648998168527360001) to prepare for June trial

**General/crypto**

- [Poseidon and Grobner basis attacks](https://twitter.com/Khovr/status/1648262661237350402)

- [Consensys reports data leak](https://consensys.net/blog/news/faq-customer-support-data-security-incident/) of Metamask support tickets

- Tayvano on a [mysterious wallet drainer](https://twitter.com/tayvano_/status/1648187031468781568), where there is no common thread between compromised keys

- If you haven’t yet, [make sure your iPhone and iOS are up to date](https://siliconangle.com/2023/04/10/apple-patches-vulnerabilities-used-target-iphones-ipads-macs/)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-april-22-2023/](https://weekinethereumnews.com/week-in-ethereum-news-april-22-2023/)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Apr 25 - May 9 – [Gitcoin Program Beta Round](https://gitcoin.notion.site/Gitcoin-Grantee-Portal-6adfc92627474bd48a5dfcd1e8438d20)

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

- Jun 2-7 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 9-11 – [ETHPrague](https://ethprague.com/) conference & hackathon

- Jun 23–25 – [ETHGlobal Waterloo](https://ethglobal.com/events/waterloo2023) (changed from Toronto)

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Aug 13-16 – [ETHToronto](https://www.ethtoronto.ca/) & [ETHWomen](https://www.ethwomen.com/)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org/) (Buenos Aires)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 30 - Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 18-21 – [ETH Montréal](https://ethmontreal.xyz/) hackathon & conference

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 27–29 – [ETH Miami](https://ethmiami.net/) festival + hackathon

- Oct 28–30 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- **Nov 13-19 –** [**Devconnect**](https://blog.ethereum.org/2023/04/20/announcing-devconnect-ist) **(Istanbul)**

- **Nov 17-19 -** [**ETHIstanbul**](https://ethglobal.com/events/istanbul) **(EthGlobal)**

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

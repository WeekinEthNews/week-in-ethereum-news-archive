---
title: "Week in Ethereum News <br> January 28, 2023"
date: "2023-01-28"
---

## Eth News and Links

**Shapella (Shanghai + Capella) upgrade**

- EF DevOps launch [devnet with 605k validators](https://twitter.com/BarnabasBusa/status/1618507444971540481) to test BLS key changes

- Withdrawal-mainnet-shadow-fork-1 [finalizing](https://twitter.com/vdwijden/status/1617530244302532615)

- Consensus specs [v1.3.0-rc.2](https://github.com/ethereum/consensus-specs/releases/tag/v1.3.0-rc.2): new Capella test cases, polynomial commitment spec updates & light client data change

**Dencun (Cancun + Deneb) upgrade**

- KZG Ceremony:
    - [23,000+ contributions](https://ceremony.ethereum.org/) after two weeks
    
    - [Session sign-out issue](https://twitter.com/trent_vanepps/status/1616741191957073922) fixed
    
    - Unique entropy generators: [Proof-of-Cat](https://proofof.cat/) & [marble run](https://twitter.com/Xofee3/status/1618406659659038720)
    
    - [Towers-of-pau](https://github.com/dknopik/towers-of-pau/tree/proper-client#readme) implementation in Go, survives suspending computer

- [EIP4844 decoupling gossip in Nimbus](https://notes.status.im/decoupled-eip4844#) design notes

- Proposed [transaction SSZ refactoring](https://notes.ethereum.org/@vbuterin/transaction_ssz_refactoring)

- [EOF v2 design](https://notes.ethereum.org/@ipsilon/eof2-design-space), based on discussions of past month

**Layer 1**

- Approaches for [decentralizing block builders](https://bittokoin.substack.com/p/block-builder-decentralization-is)

- [Kaustinen](https://twitter.com/gballet/status/1618907141418672130) PoS verkle testnet, replaces Condrieu testnet, includes proofs in blocks

**Client releases**

- Consensus layer:
    - Nimbus [v23.1.1](https://github.com/status-im/nimbus-eth2/releases/tag/v23.1.1): hotfix for client failing to start after enabling database pruning
    
    - Teku [v23.1.0](https://github.com/ConsenSys/teku/releases/tag/23.1.0): fixes, optimizations & new features; [v23.1.1](https://github.com/ConsenSys/teku/releases/tag/23.1.1): fixes docker permissions

- Execution layer:
    - Nethermind [v1.16.1](https://github.com/NethermindEth/nethermind/releases/tag/1.16.1): reported ~0.5% improvement in staking rewards, RAM consumption reduced and adds low disk space notification

**Layer 2**

- Patrick McCorry: [rollup permissive vs permissioned licensing](https://stonecoldpat.substack.com/p/rollups-need-an-eco-system-license)

**EIPs/Standards**

- [ERC6366](https://github.com/ethereum/EIPs/pull/6366/files): Permission token

- [ERC6372](https://eips.ethereum.org/EIPS/eip-6372): Contract clock

- [ERC6381](https://github.com/ethereum/EIPs/pull/6381/files): Emotable extension for NFTs

- [EIP6384](https://github.com/ethereum/EIPs/pull/6384/files): Humanly readable offline signatures

* * *

### **This newsletter is made possible thanks to Optimism’s** [**Retroactive Public Goods Funding**](https://gov.optimism.io/t/nominations-for-retropgf2/4636)

![Optimism](https://weekinethereumnews.com/wp-content/uploads/2023/01/OPTIMISM.png)

Optimism is running a [second round of their Retroactive Public Goods Funding](https://gov.optimism.io/t/nominations-for-retropgf2/4636).  Ten million OP tokens will be given out in this RetroPGF round!

Project nominations close January 31st at 19:00 GMT.

Nominate projects for a specific category using the links below:

- [Infrastructure and dependencies](https://gov.optimism.io/t/infrastructure-dependencies-nominations-for-rpgf2/4637)

- [Tooling and utilities](https://gov.optimism.io/t/tooling-utilities-nominations-for-rpgf2/4639)

- [Education](https://gov.optimism.io/t/education-nominations-for-rpgf2/4640) 

* * *

**Stuff for developers**

- Foundry:
    - ChugSplash [Foundry](https://github.com/chugsplash/chugsplash-foundry#readme): deploy & manage upgradeable contracts, upgrade OpenZeppelin Transparent proxies, supports mainnet & Optimism
    
    - [Deal cheat code](https://twitter.com/paulrberg/status/1619059764180434944) mints ERC20 tokens in tests

- [EVM call stipend](https://twitter.com/wadealexc/status/1619030019803848704) (2300 gas) explainer

- OpenZeppelin [proposal to mitigate ERC4626 inflation attacks](https://ethereum-magicians.org/t/address-eip-4626-inflation-attacks-with-virtual-shares-and-assets/12677) with virtual assets & shares

- [Sparse-arr-lib](https://github.com/clabby/sparse-arr-lib#readme): Solidity library for sparse arrays, work in progress

- [Optimizing using Yul](https://medium.com/@MarqyMarq/using-yul-to-optimize-gas-costs-b4feccdb5172) via example rock, paper & scissors contracts

- Samczsun’s [signature database](https://twitter.com/samczsun/status/1618161664624594945): exportable, add to canonical list via GitHub

- [Clipshot](https://clipshot.xyz/): ERC1155 token holder snapshots as CSV

- [Hydralisk](https://github.com/paulpierre/hydralisk#readme): Python CLI for bulk wallet creation

- [Walk through of building bear traps](https://paulbrower.codes/posts/bear-traps-in-the-dark-forest/) for MEV bot front-runners

- DamnVulnerableDefi [ABI smuggling solution](https://medium.com/@mattaereal/damnvulnerabledefi-abi-smuggling-challenge-walkthrough-plus-infographic-7098855d49a) 

- [Uniswap v3 math](https://uniswap.org/blog/uniswap-v3-math-primer) explainer

**Ecosystem**

- [1/3 of relayed blocks](https://twitter.com/ultrasoundmoney/status/1618552322380156928) not censoring Tornado Cash transactions

- 0xPARC [zk 4 week residency](https://0xparc.org/blog/2023-spring-residency) in Vietnam from mid-March

**Enterprise**

- [Cité Gestion](https://cmta.ch/news-articles/cite-gestion-becomes-cmta-certified-issuer-of-tokenized-shares) (Swiss bank) tokenized its shares on Ethereum

- Baseline [simple reference implementation](https://entethalliance.org/2023-01-25-new-baseline-protocol-reference-implementation-hits-milestone)

**Application layer**

- [Aave v3](https://twitter.com/aaveaave/status/1618903037761945601) live on mainnet

- RAI stablecoin:
    - Ameen: [reflections on ETH-only RAI & ungovernance](https://twitter.com/ameensol/status/1617981220146778114)
    
    - Vitalik: [how RAI-like systems could support staked ETH](https://community.reflexer.finance/t/can-oracles-double-as-co-stakers-how-rai-like-systems-might-safely-support-staked-eth/397)

- Index Coop [diversified staked ETH](https://indexcoop.com/blog/introducing-the-diversified-staked-eth-index): index token of Rocket Pool, Lido & StakeWise staked ETH

- [Maker voted](https://twitter.com/MakerDAO/status/1617577643200610335) to deploy 100M USDC from PSM into a Yearn vault

- Maple Finance adds [receivables financing pool](https://maple.finance/news/aqru-joins-maple-receivables-financing-on-chain/)

- [Migratooor](https://migratooor.com/): move tokens from one address to another

- [MoonPlace](https://www.reddit.com/r/CryptoCurrency/comments/10m5uow/moonplace_a_place_like_rplace_but_onchain_nfts_on/): r/Place like NFTs on Arbitrum Nova using r/CryptoCurrency community tokens

- [Texture Punx](https://texturepunx.com/): on-chain SVG NFTs with user selected traits, 50% of secondary sales donated to Protocol Guild \[Disclosure: Andrew minted three, one was free\]

* * *

### Job Listings

- Arx, creators of KONG Cash and HaLo tags is hiring a [Solidity developer](https://arx.org/jobs).

- [Status](https://status.im/) is hiring a [Technical Writer for Waku Product](https://grnh.se/41bd7e051us), [all other jobs here](https://grnh.se/9fc6e6fc1us)

- Ethereum Foundation are hiring a [Community Lead for ethereum.org](https://jobs.lever.co/ethereumfoundation/89ff5705-3351-422d-a5d1-b0805e95edec?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)

- [Lighthouse seeking support tech](https://github.com/sigp/positions-vacant/blob/master/lighthouse-support.md) to help its stakers

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US SEC Commissioner Peirce](https://www.sec.gov/news/speech/peirce-remarks-duke-conference-012023): approach crypto regulation carefully but don’t wait for regulators to solve problems

- Reuters: [US SEC probing investment advisers](https://www.reuters.com/technology/us-securities-regulator-probes-investment-advisers-over-crypto-custody-sources-2023-01-27/) on custody of clients crypto

- FBI: [Lazarus group behind $100M Horizon bridge theft](https://www.fbi.gov/news/press-releases/fbi-confirms-lazarus-group-apt38-cyber-actors-responsible-for-harmonys-horizon-bridge-currency-theft) in June 2022

- Outlier Ventures: [which products need a token](https://outlierventures.io/does-your-product-need-a-token/)

**General/crypto**

- [LocalCryptos](https://blog.localcryptos.com/after-5-years-localcryptos-is-saying-goodbye/) (LocalEthereum) winding down

- Worldcoin releases [hardware engineering files for Orb iris scanner](https://worldcoin.org/blog/tech/opening-orb-look-inside-worldcoin-biometric-imaging-device)

- Semaphore grants round [recipient projects](https://mirror.xyz/privacy-scaling-explorations.eth/5w1v6rxpP-E03rWDr3RliPyFJkptQwIPzet3Vb5jdcI)

- Introduction to [commitment schemes](https://blockdoc.substack.com/p/an-introduction-to-commitment-schemes)

- ZK MOOCs: [modern zk cryptography](https://zkiap.com/) and [zk proofs](https://zk-learning.org/)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-january-28-2023](https://weekinethereumnews.com/week-in-ethereum-news-january-28-2023)

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jan 31 – deadline for [Gitcoin grants round](https://go.gitcoin.co/blog/announcing-the-gitcoin-alpha-tests)

- Jan 31 – [KZG ceremony grants](https://blog.ethereum.org/2022/12/15/kzg-ceremony-grants-round) deadline

- Jan 31 – deadline to nominate for [Optimism retroactive public goods round 2](https://gov.optimism.io/t/nominations-for-retropgf2/4636)

- Feb 3 – deadline to nominate for [DAOdrops](https://daodrops.io/) retroactive public goods funding

- Feb 24 - Mar 1 – [ETHDenver BUIDLWeek](https://www.ethdenver.com/)

- Feb 27 – deadline for [EF academic grants round](https://esp.ethereum.foundation/academic-grants-2023)

- Mar 2-5 – [ETHDenver Hackathon](https://www.ethdenver.com/)

- Mar 10-29 – [Scaling Ethereum](https://ethglobal.com/events/scaling2023) (ETHGlobal) virtual

- Mar 15-16 – [ETHDubai](https://www.ethdubaiconf.org/)

- Mar 16-18 – [ETH Porto](https://ethporto.org/)

- Mar 28-30 – [Ethereum Rio](https://www.ethereumbrasil.com/ethereumrio)

- Apr 3-6 – [Edcon](https://edcon.io/) Vienna

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- Apr 14-16 – [ETHGlobal Tokyo](https://tokyo.ethglobal.com/)

- Apr 14-16 – [ETHZurich](https://ethereumzuri.ch/) conference **& hackathon**

- Apr 21-23  – [EthTaipei](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) hackathon

- Apr 24-25  – [EthTaipei](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) conference

- May 5-7 – [ETHMalaysia](http://ethmalaysia.com/) conference & hackathon

- **May 20-21 –** [**ETHDam**](https://www.ethdam.com/) **(Amsterdam) conference & hackathon**

- May 26–28 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Jun 23–25 – [ETHGlobal Toronto](https://ethglobal.com/events/toronto)

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–25 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

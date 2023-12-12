---
title: "Week in Ethereum News <br> January 21, 2023"
date: "2023-01-21"
---

## **Eth News and Links**

**Shapella (Shanghai + Capella) upgrade**

- [Withdrawals FAQ](https://notes.ethereum.org/@launchpad/withdrawals-faq#)

- Latest core devs execution [call video](https://www.youtube.com/watch?v=hVeMHoUUZ30&t=264s).  [Summary](https://twitter.com/abcoathup/status/1616167638241259521) by Tim Beiko.  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1616108684974903301) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-execution-call-153/):
    - withdrawal-devnet-3 tested EL & CL both using gwei units for withdrawals
    
    - Sepolia shadow fork went smoothly
    
    - Mainnet shadow fork next week
    
    - Withdrawal root in Execution Layer will remain RLP encoded (CL is SSZ)
    
    - EIP6049 (deprecation notice for SELFDESTRUCT) added to Shanghai
    
    - EOF EIPs added as candidates for inclusion in Cancun upgrade
    
    - [Eth Magicians to be used for community input](https://ethereum-magicians.org/t/proposal-network-upgrade-meta-threads/12552) on scope of future upgrades

- withdrawal-devnet-2 [retired](https://twitter.com/vdWijden/status/1615391553039499270): tx-fuzz found issues with EthereumJS sometimes producing bad blocks and Geth txpool not rejecting bad transactions

- [Zhejiang public testnet](https://twitter.com/abcoathup/status/1616537216167350272) for Shapella upgrade expected after the client interop next week

- Shapella community [call video](https://www.youtube.com/watch?v=uTWpSYn4MA8&t=162s) 

**Dencun (Cancun + Deneb) upgrade**

- Community discussion on [Cancun upgrade scope](https://ethereum-magicians.org/t/cancun-network-upgrade-meta-thread/12060)

- Latest EIP4844 implementers [call video](https://www.youtube.com/watch?v=zDjF3AGypbM). Notes from [Terence](https://twitter.com/terencechain/status/1615394497684463621): devnet 4 expected next week

- KZG Ceremony:
    - [12,000+ contributions](https://twitter.com/skylenet/status/1616425825435545601) in first week, average contribution taking 50 seconds
    
    - EF [ceremony announcement](https://blog.ethereum.org/2023/01/16/announcing-kzg-ceremony)

**Layer 1**

- Ethereum Cat Herders [client diversity survey](https://medium.com/ethereum-cat-herders/client-diversity-on-ethereum-network-3854b5c3c95f) for node runners

- Patrick McCorry’s [Proof of Stake explainer series](https://stonecoldpat.substack.com/p/how-proof-of-stake-ethereum-works)

**Client releases**

- Consensus layer:
    - Nimbus [v23.1.0](https://github.com/status-im/nimbus-eth2/releases/tag/v23.1.0): on-the-fly database pruning, 60-70 GB storage for typical beacon node

- Execution layer:
    - Erigon [v2.36.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.36.0): block body downloader fix and MDBX upgrade rolled back 

**Research**

- [Proofs of complete knowledge (CK)](https://medium.com/initc3org/complete-knowledge-eecdda172a81): prevent encumbrance of secrets using TEEs & mining ASICs

- Note on [fast amortized KZG proofs](https://eprint.iacr.org/2023/033)

- [Gradual Dutch Auctions](https://people.eecs.berkeley.edu/~ksk/files/GDA.pdf) \[PDF\] can be modified to be incentive compatible

**EIPs/Standards**

- [ERC6299](https://github.com/ethereum/EIPs/pull/6299/files): Lockable tokens

- [ERC6315](https://github.com/ethereum/EIPs/pull/6315/files): ERC2771 Account Abstraction 

- [ERC6327](https://github.com/ethereum/EIPs/pull/6327/files): Elastic signature

- [ERC6353](https://github.com/ethereum/EIPs/pull/6353/files): Charity token

- [ERC6357](https://github.com/ethereum/EIPs/pull/6357/files): Single-contract Multicall

- [ERC6358](https://github.com/ethereum/EIPs/pull/6358/files): Omniverse DLT

* * *

### **This newsletter is made possible thanks to** [**Mimic**](https://mimic.fi/)**!**

![mimic](https://weekinethereumnews.com/wp-content/uploads/2022/10/mimic-banner-1024x427.png)

Does your _app_ or _DAO_ want to automate your DeFi operations?  With Mimic, you can **automate swapping, bridging and treasury management**.

Check out our [Smart Vaults](https://medium.com/mimicfi/introducing-smart-vaults-3438bacc843d) to automate DeFi operations in a secure, trustless, and non-custodial way.

We’ll be at EthDenver if you want to [request a demo](https://airtable.com/shrSvH8fTJcbHq0xl) IRL. _Backed by Starbloom Ventures._

* * *

**Stuff for developers**

- Foundry:
    - Foundry [best practices](https://twitter.com/msolomon44/status/1616072891820539904)
    
    - forge-std [v1.3.0](https://github.com/foundry-rs/forge-std/releases/tag/v1.3.0): InvariantTest helper contract, Multicall3 interface & getTokenBalances helper, StdChains chain alias, parseJson & assumePayable cheat codes and decimal assertions
    
    - Invariant testing: [example](https://github.com/lucas-manuel/invariant-example/#readme) repo to experiment, also see Maple Finance [invariant tests](https://github.com/maple-labs/maple-core-v2/tree/main/tests/invariants) 
    
    - [forge doc](https://twitter.com/r_krasiuk/status/1615444642195202055): documentation generator using natspec, outputs markdown

- Solidity [preview of user-defined operators](https://forum.soliditylang.org/t/feature-preview-user-defined-operators/1435) in upcoming v0.8.18

- Fe language [bountiful round 2](https://blog.fe-lang.org/posts/bountiful-round-2/) bug bounty contest

- Beginners guide to [Yul (intermediate language)](https://medium.com/@markjonathas/beginners-guide-to-yul-12a0a18095ef)

- [Guide to contract decompilation](https://jbecker.dev/research/diving-into-decompilation/), as implemented by heimdall-rs (decompiler)

- [Solidity-merkle-trees](https://github.com/polytope-labs/solidity-merkle-trees#readme): Solidity library to verify multi-proofs of Merkle trees

- [ERC5267 demo website](https://eip5267.vercel.app/) to retrieve ERC712 domain

- [The Graph](https://twitter.com/graphprotocol/status/1615772852745027594) adds support for Arbitrum & Optimism

**Security**

- Echidna [v2.0.5](https://github.com/crytic/echidna/releases/tag/v2.0.5) (contract fuzzer): adds prank to override msg.sender for next external call

- Read-only reentrancy [explainer](https://twitter.com/bytes032/status/1616357019522400256)

**Ecosystem**

- Tim Beiko: [how Ethereum has staking rewards & deflation](https://twitter.com/timbeiko/status/1615047215319486464) as [Ether goes ultrasound](https://twitter.com/ultrasoundmoney/status/1614747580407111682) again

- Ethereum has [500,000 validators](https://www.reddit.com/r/ethstaker/comments/10dc6aq/500_000_validators_online/)

- Vitalik: [guide to stealth addresses](https://vitalik.eth.limo/general/2023/01/20/stealth.html)

- Wallet devs [call video](https://www.youtube.com/watch?v=G6p5Xh6a44k) and [summary](https://twitter.com/_SamWilsn_/status/1615934951077171200)

- Ethereum Foundation [second academic grants round](https://esp.ethereum.foundation/academic-grants-2023)

- [Mergooor Pass](https://twitter.com/zkdrop_io/status/1615716498000977921): non-transferrable NFT for Merge contributors to access major events

**Enterprise**

- [Nightfall v3](https://www.ey.com/en_gl/news/2023/01/the-ey-and-polygon-organizations-update-source-code-for-blockchain-privacy-based-protocol-nightfall) considered production beta

- Second Australian bank [creating AUD stablecoin](https://archive.is/ngPce)

- Enterprise Ethereum Alliance [QBFT spec](https://entethalliance.org/23-01-qbft-spec-version-1-released/), evolution of Istanbul BFT, formally verified

**Application layer**

- Uniswap [Permit2 live](https://twitter.com/Uniswap/status/1615824670825250816), token approvals expire every 30 days, sign to reauthorize

- [Maker vote to remove Gemini USD stable coin](https://www.coindesk.com/markets/2023/01/19/makerdao-votes-to-keep-gemini-usd-in-dai-stablecoins-reserves/) defeated at last minute, Paxos [offering 45% of the US federal funds rate](https://forum.makerdao.com/t/paxos-makerdao-partnership-usdp-psm/19469)

- MACI (anti-collusion) [v1.1.1](https://mirror.xyz/privacy-scaling-explorations.eth/ltCt68hslI5jmMf1AnfkrP2eUwkeZ8_fgkHc_WyD9Nc): adds granting users more votes without re-registering, reduce match amounts where contributions are highly correlated and sample coordinator service

- [Proof of Innocence](https://medium.com/@chainway_xyz/introducing-proof-of-innocence-built-on-tornado-cash-7336d185cda6): prove deposits to Tornado Cash are not from sanctioned addresses

- Unlock Protocol’s guide to [NFT ticketing](https://unlock-protocol.com/guides/ethdenver23tix/) for events

- Introduction to [zero-knowledge apps](https://mirror.xyz/andyguzman.eth/p4nNk7Rr-2i-uZDO_lTHJEWtNv3nYt2N2z3Cwly8RHc)

- [ETH dust collector](https://twitter.com/cory_eth/status/1614496165004992512): sweep dust from an address using legacy Type 0 transactions

* * *

### Job Listings

- Ethereum Foundation are hiring a [Community Lead for ethereum.org](https://jobs.lever.co/ethereumfoundation/89ff5705-3351-422d-a5d1-b0805e95edec?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)

- [Lighthouse seeking support tech](https://github.com/sigp/positions-vacant/blob/master/lighthouse-support.md) to help its stakers

- [Status](https://status.im/) is hiring a [Technical Writer for Waku Product](https://grnh.se/41bd7e051us), [all other jobs here](https://grnh.se/9fc6e6fc1us)

- Arx, creators of KONG Cash and HaLo tags is hiring a [Solidity developer](https://arx.org/jobs).

- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- CeFi lending platform [Genesis](https://www.businesswire.com/news/home/20230119005955/en) filed for bankruptcy

- [Nexo $45 million settlement](https://www.sec.gov/news/press-release/2023-11) with US SEC & states for failing to register retail lending product

- [BitConnect fraud victims](https://www.justice.gov/opa/pr/crypto-fraud-victims-receive-over-17-million-restitution-bitconnect-scheme) to share $17 million in restitution

- [US DoJ pre-announced](https://twitter.com/thejusticedept/status/1615740967939674116) enforcement action, ended up being arrest of [Russian owner of Bitzlato exchange](https://www.justice.gov/opa/pr/founder-and-majority-owner-cryptocurrency-exchange-charged-processing-over-700-million)

- [ConsenSys](https://consensys.net/blog/news/consensys-focuses-its-strategy-to-ensure-future-growth/) laying off ~100 employees

- [Coinbase](https://www.coinbase.com/blog/halting-operations-in-japan) halting operations in Japan

- Uniswap: [on-chain foreign exchange](https://uniswap.org/blog/uniswap-circle-foreign-exchange-defi) could reduce remittance cost by up to 80%

**General/crypto**

- [zkalc](https://crypto.ethereum.org/blog/zkalc): calculate time to perform cryptographic operations on selected computers

- [zk system benchmarking](https://delendum.xyz/2023/01/11/zk-system-benchmarking.html): standard benchmarks for comparing zk proof library performance

- [Halo2 FRI gadget](https://github.com/maxgillett/halo2-fri-gadget): FRI verifier circuit for BN254 scalar field

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-january-21-2023](https://weekinethereumnews.com/week-in-ethereum-news-january-21-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- **Jan 31 – deadline for** [**Gitcoin grants round**](https://go.gitcoin.co/blog/announcing-the-gitcoin-alpha-tests)

- Jan 31 – [KZG ceremony grants](https://blog.ethereum.org/2022/12/15/kzg-ceremony-grants-round) deadline

- Jan 31 – deadline to nominate for [Optimism retroactive public goods round 2](https://community.optimism.io/docs/governance/retropgf-2/#scope-of-retropgf-2)

- Feb 3 – deadline to nominate for [DAOdrops](https://daodrops.io/) retroactive public goods funding

- Feb 24 - Mar 1 – [ETHDenver BUIDLWeek](https://www.ethdenver.com/)

- **Feb 27 – deadline for** [**EF academic grants round**](https://esp.ethereum.foundation/academic-grants-2023)

- Mar 2-5 – [ETHDenver Hackathon](https://www.ethdenver.com/)

- Mar 10-29 – [Scaling Ethereum](https://ethglobal.com/events/scaling2023) (ETHGlobal) virtual

- Mar 15-16 – [ETHDubai](https://www.ethdubaiconf.org/)

- Mar 16-18 – [ETH Porto](https://ethporto.org/)

- Mar 28-30 – [Ethereum Rio](https://www.ethereumbrasil.com/ethereumrio)

- Apr 3-6 – [Edcon](https://edcon.io/) Vienna

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- Apr 14-16 – [ETHGlobal Tokyo](https://tokyo.ethglobal.com/)

- Apr 14-16 – [ETHZurich](https://ethereumzuri.ch/) conference

- Apr 21-23  – [EthTaipei](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) hackathon

- Apr 24-25  – [EthTaipei](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) conference

- **May 5-7 –** [**ETHMalaysia**](http://ethmalaysia.com/) **conference & hackathon**

- May 26–28 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Jun 23–25 – [ETHGlobal Toronto](https://ethglobal.com/events/toronto)

- **Jul 5-7 –** [**ETHBarcelona**](https://ethbarcelona.com/)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–25 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

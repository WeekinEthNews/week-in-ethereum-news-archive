---
title: "Week in Ethereum News <br> February 11, 2023"
date: "2023-02-11"
---

## Eth News and Links

**Shapella (Shanghai + Capella) upgrade**

- Sepolia testnet upgrades to Shapella on [Tuesday February 28, 4:04:48 AM UTC](https://github.com/eth-clients/sepolia/pull/30), a sync committee & historical roots boundary

- Zhejiang testnet [upgraded to Shapella](https://twitter.com/BarnabasBusa/status/1622975351520481280), processing [full & partial withdrawals and BLS changes](https://zhejiang.beaconcha.in/validators/withdrawals)
    - Guide to [run a Teku+Besu node](https://github.com/eth-educators/ethstaker-guides/blob/main/zhejiang-alt.md)

- Ephemery (ephemeral testnet) [upgraded to Shapella](https://twitter.com/TMIYChao/status/1622328088452374529)

- Latest all core devs - consensus (ACDC) [call video](https://www.youtube.com/watch?v=YMu50yNUz5Y&t=529s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/BJcVqOzpj) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-consensus-call-102/):
    - Sepolia testnet upgrade date selected, Goerli testnet could follow 1-2 weeks later (early/mid March) with mainnet a couple of weeks after that, assuming no issues
    
    - Fallback from MEV-Boost needs to be tested with Shapella
    
    - Discussion of positive EIP4844 block/blob decoupling simulation results
    
    - Tim Beiko proposed using EIPs for consensus layer & add core EIP editors
    
    - Engine API exchange transition config to be deprecated in Dencun upgrade

- Danny Ryan’s [Finalized update](https://blog.ethereum.org/2023/02/10/finalized-no-38): Shapella upgrade & reminder of EF academic grants round

**Dencun (Cancun + Deneb) upgrade**

- KZG Ceremony:
    - [39,000+ contributors](https://ceremony.ethereum.org/), 2500+ in the lobby, 30 days left in _first_ general contribution period
    
    - [Dappnode](https://twitter.com/eduadiez/status/1623963202500304896) adds support for contributing

- Latest EIP4844 implementers [call video](https://www.youtube.com/watch?v=vQGk9FDs_CM&t=5s). Notes from [Terence](https://twitter.com/terencechain/status/1623010406603317248): planning to decouple blobs from blocks

**Layer 1**

- [Lodestar](https://twitter.com/carlbeek/status/1623703738727731208) added as fifth consensus layer client to mainnet staking launchpad

- [Client team in person interop](https://blog.ethereum.org/2023/02/07/edelweiss-interop-recap) in Austria focused on Shapella & Dencun upgrades

- [Lido MEV Boost relay list](https://twitter.com/isdrsp/status/1624072920652816385) added Ultrasound, Agnostic & Aestus relays

**Client releases**

- Consensus layer:
    - Lodestar [v1.4.2](https://github.com/ChainSafe/lodestar/releases/tag/v1.4.2): peer scoring improvements & fix for isBetterUpdate light client issue

- Execution layer:
    - Erigon [v2.38.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.38.0): eth/68 support & fixes; [v2.38.1](https://github.com/ledgerwatch/erigon/releases/tag/v2.38.1): patch

**Research**

- [Metrics for network performance](https://ethresear.ch/t/approximating-user-welfare-and-surplus-with-transaction-data/14766): value generated (welfare) & value gained by users (surplus)

- [Rollup relay](https://hackmd.io/@echno/rollup-relay) to reduce trust assumptions in PBS relay

**Layer 2**

- Kelvin Fichter: [why 7 days is used for challenge period](https://kelvinfichter.com/pages/thoughts/challenge-periods/) in Optimistic Rollups

- [Ticking-Optimism](https://therealbytes.substack.com/p/presenting-ticking-optimism): ticking blockchain built on Optimism Bedrock, proof of concept

- [Optimism airdrop 2](https://optimism.mirror.xyz/lPZEkFF7LU2ZlrO-dsV3p_LtWQUaknFGfxFMgSz3vGA): OP tokens sent directly to delegators and power users

- Arbitrum [Stylus](https://offchain.medium.com/hello-stylus-6b18fecc3a22) announcement, programming environment & WASM VM for Arbitrum One/Nova, allows for programs in non-EVM languages such as Rust, C, C++, expected in 2023

**EIPs/Standards**

- EIPs:
    - [EIP6465](https://eips.ethereum.org/EIPS/eip-6465): SSZ withdrawals root
    
    - [EIP6466](https://github.com/ethereum/EIPs/pull/6466/files): SSZ transactions root
    
    - [EIP6475](https://eips.ethereum.org/EIPS/eip-6475): SSZ Optional

- ERCs:
    - [ERC6454](https://eips.ethereum.org/EIPS/eip-6454): Minimalistic non-transferrable NFTs
    
    - [ERC6464](https://github.com/ethereum/EIPs/pull/6464/files): Multi-operator per-token ERC721 approvals
    
    - [ERC6492](https://github.com/ethereum/EIPs/pull/6492/files): Signature validation for predeploy contracts
    
    - \[Resurrected\] [ERC223](https://github.com/ethereum/EIPs/pull/6485/files): Fungible token with communication model

* * *

### **This newsletter is made possible thanks to** [**Nexus Mutual**](https://app.nexusmutual.io/home)

![Nexus Mutual](https://weekinethereumnews.com/wp-content/uploads/2023/02/Nexus-Mutual-2-1024x330.png)

Nexus Mutual is the leading insurance alternative for crypto and more. Over $10m in claims paid across eight loss events including FTX and Hodlnaut. 

[Get covered](https://app.nexusmutual.io/cover) against smart contract, slashing, and other risks.

* * *

**Stuff for developers**

- Remix IDE [v0.30.0](https://medium.com/remix-ide/remix-ide-v0-30-0-release-8ee6bb8bcb5f): Solidity unit testing displays revert reason, ERC20 template expands Solidity unit test examples, view compiler input, added Mocha Chai test & Slither GitHub workflows and added Flatten & generate UML as internal plugins

- Foundry:
    - Foundry Book: [guide to invariant testing](https://book.getfoundry.sh/forge/invariant-testing)
    
    - [Visualize code coverage in Foundry tests](https://twitter.com/fiveoutofnine/status/1622639955720675330) using coverage gutters
    
    - [Fuzzing ordered Solidity arrays](https://twitter.com/paulrberg/status/1623981086551203841) in Foundry

- Hardhat [v2.12.7](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.12.7): Hardhat Network option for blocks with same timestamp, http\_proxy environment variable support, batch requests via WebSocket and config validation for optimizer runs

- [Solidity compiler bloating deployments](https://media.dedaub.com/i-see-dead-code-2a9c13d0b98e) by including library functions only called in the constructor in runtime bytecode 

- PRBMath [v3.3.0](https://github.com/PaulRBerg/prb-math/releases/tag/v3.3.0): adds Rust like type casting

- [Epoch commit/reveal](https://twitter.com/_MouseDev/status/1623044314983964682) for NFT randomness

- [ERC20Emit](https://twitter.com/clemlak/status/1622971215034957824): ERC20 logic implemented in events, don’t use in production, [beware of Solidity's evaluation order of event parameters](https://github.com/ethereum/solidity-underhanded-contest/blob/master/2022/submissions_2022/submission9_TynanRichards/SPOILERS.md#the-actual-exploit)

- [File pattern](https://mirror.xyz/horsefacts.eth/R5N_Dzm2XKVvSI3cM8e8EHuFzvpPBttG2TEtyEZDa10): single Solidity function that dispatches multiple setters

- [Storage Struct pattern](https://mirror.xyz/horsefacts.eth/EPB4o-eyDl0N8gu0gEz1uw7BTITheaZUqIAOEK1m-jE) for storage in upgradeable contracts

- [Query Storage Slot](https://twitter.com/apoorvlathey/status/1622660772538245120): web UI to read ERC1967 & custom proxy storage slots

- [Mr Steal Yo Crypto CTF solutions](https://github.com/0xToshii/mr-steal-yo-crypto-ctf-foundry#readme) in Foundry

- [EVM puzzle solution](https://twitter.com/0xkarmacoma/status/1623131882581012481) using Halmos symbolic testing

- [Slither Printers](https://twitter.com/0xtaylor_/status/1622359910230130688) to display/output contract info such as function summary & inheritance

- Palla’s [intro to coding zk proofs](https://dev.to/spalladino/a-beginners-intro-to-coding-zero-knowledge-proofs-c56): overview of Circom, Halo2 & Noir using rock/paper/scissors

- Semaphore [v3](https://mirror.xyz/privacy-scaling-explorations.eth/Yi4muh-vzDZmIqJIcM9Mawu2e7jw8MRnwxvhFcyfns8): CLI to create projects, Hardhat plugin to deploy Semaphore contract & boilerplate demo

**Security**

- dForce on Arbitrum & Optimism [~$3.65M exploit](https://twitter.com/BlockSecTeam/status/1623901011680333824) via read only reentrancy of Curve pool

- Sperax USDs rebasing token on Arbitrum [~$300k exploit](https://medium.com/sperax/usds-feb-3-exploit-report-from-engineering-team-9f0fd3cef00c) via internal balance bug, [funds returned](https://twitter.com/SperaxUSD/status/1623794992144699398) after exploiter identified

- Barter solver on CoW Swap [~$166k exploit](https://cow-protocol.medium.com/cow-swap-solver-exploit-post-mortem-07-02-2023-2faa9f918e29) via arbitrary execution code

**Ecosystem**

- Ethereum.org page on [staking withdrawals](https://ethereum.org/en/staking/withdrawals/)

- [Modeling withdrawals](https://dataalways.substack.com/p/partial-withdrawals-after-the-shanghai): extreme case of 110k ETH partial withdrawals on day 1 and 57.6k ETH full withdrawals per day

- EthStaker [staking survey results](https://lookerstudio.google.com/u/0/reporting/cafcee00-e1af-4148-bae8-442a88ac75fa/page/p_ja2srdhh2c): technical setup is barrier to solo staking

- Proposal for Lido [v2](https://blog.lido.fi/introducing-lido-v2/): withdrawals & Staking Router to allow permissionless onboarding of node operators

**Enterprise**

- [Shopify tools](https://twitter.com/ryancreatescopy/status/1623689892998914054) for tokengating merchant apps, includes Shopify connect wallet (built on wagmi React hooks)

**Application layer**

- [Flux Finance](https://blog.fluxfinance.com/flux-finance-is-live/) (tokenized US treasury bonds) live on mainnet, currently earning ~4.3% with $100k minimum and KYC required

- Backed [bCSPX](https://backed.fi/news-updates/introducing-bcspx): tokenized tracker for S&P UCITS ETF, non-US qualified investors only

- Nexus Mutual v2 [partial claims](https://twitter.com/NexusMutual/status/1622667601963884564) are live on mainnet, being used for FTX, BlockFi & Gemini claims

- [Aave’s GHO stablecoin](https://gho.xyz/) live on Goerli testnet

- [Spark Protocol](https://blog.element.fi/spark-into-defi-hyperdrive/) to use Element Finance’s [Hyperdrive AMM](https://twitter.com/element_fi/status/1622996238474915847) for fixed rate lending on Maker, competing with Aave

- [Synthetix](https://blog.synthetix.io/22-new-synthetix-perp-futures-market-are-now-live/) adds 22 perpetual futures markets, mostly crypto plus a few major FOREX markets

- tBTC [v2](https://blog.threshold.network/thresholds-tbtc-launches-minting-for-only-decentralized-permissionless-scalable-btc-bridge-to-defi/) (more “trustless” BTC) live via [optimistic minting](https://blog.threshold.network/minters-guardians-and-a-strong-tbtc/)

- Sound [curator rewards](https://sound.mirror.xyz/_TlNt5wOXGjnS7_2mMXPUlr-LSGKVQ_tlkE4px5yZEE): 5% on music NFT mints via referral links

- [53% of DAO delegates](https://twitter.com/karmahq_/status/1622963501311606784) have never voted 

* * *

### Job Listings

- [Request Network](https://request.network/en/) is hiring a [Community & Communication Manager](https://jobs.lever.co/request/76d0db8a-06bc-42c9-9816-69317c5f8c99)

- Shell Protocol team is hiring [senior Solidity devs & more](https://shellprotocol.io/posts/now-hiring-for-shell-protocol/), remote or Hawaii

- [Community Lead for ethereum.org](https://jobs.lever.co/ethereumfoundation/89ff5705-3351-422d-a5d1-b0805e95edec?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) sought by Ethereum Foundation

- [Cyfrin.io](https://www.cyfrin.io/) is hiring [senior security engineers](https://github.com/ChainAccelOrg/SecurityEngineerReq) $190k-$300k.

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- SEC shuts [Kraken’s staking as a service](https://blog.kraken.com/post/17619/settlement/) in US:
    - [SEC settlement](https://www.sec.gov/news/press-release/2023-25) for unregistered offer & sale of securities includes $30 million payment
    
    - Commissioner Peirce dissents: [paternalistic and lazy regulator](https://www.sec.gov/news/statement/peirce-statement-kraken-020923)
    
    - ETH to be unstaked after Shapella upgrade

- Paul Grewal: [Coinbase’s staking services are not securities](https://www.coinbase.com/blog/coinbases-staking-services-are-not-securities-and-heres-why)

- [Revolut (challenger bank) offers ETH staking](https://blog.revolut.com/staking/) in UK and parts of Europe

- Bank of England [digital pound (retail CDBC)](https://www.bankofengland.co.uk/paper/2023/the-digital-pound-consultation-paper) consultation, [may not use smart contracts](https://www.bankofengland.co.uk/-/media/boe/files/paper/2023/the-digital-pound-technology-working-paper.pdf) \[PDF\], feedback by June 7

- Nic Carter: [US government is using banking sector to crackdown against crypto](https://www.piratewires.com/p/crypto-choke-point)

- [Hermès](https://news.bloomberglaw.com/ip-law/hermes-gets-win-over-metabirkins-in-first-nft-trademark-trial) won trademark lawsuit against NFTs depicting Hermès handbag

**General/crypto**

- [Erigon to remove code for BSC & Polygon](https://erigon.substack.com/p/future-of-the-support-of-bnb-smart) unless they fund support & maintenance

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-february-11-2023](https://weekinethereumnews.com/week-in-ethereum-news-february-11-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Feb 24 - Mar 1 – [ETHDenver BUIDLWeek](https://www.ethdenver.com/)

- Feb 27 – deadline for [EF academic grants round](https://esp.ethereum.foundation/academic-grants-2023)

- **Feb 28 –** [**Sepolia testnet**](https://github.com/eth-clients/sepolia/pull/30) **upgrades to Shapella**

- Mar 2-5 – [ETHDenver Hackathon](https://www.ethdenver.com/)

- Mar 10-29 – [Scaling Ethereum](https://ethglobal.com/events/scaling2023) (ETHGlobal) virtual

- Mar 15-16 – [ETHDubai](https://www.ethdubaiconf.org/)

- Mar 16-18 – [ETH Porto](https://ethporto.org/)

- Mar 28-30 – [Ethereum Rio](https://www.ethereumbrasil.com/ethereumrio)

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- Apr 14-16 – [ETHGlobal Tokyo](https://tokyo.ethglobal.com/)

- Apr 14-16 – [ETHZurich](https://ethereumzuri.ch/) conference & hackathon

- Apr 21-25 – [EthTaipei](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) hackathon & conference

- Apr 27-30 – [Istanbul ETH Privacy](https://www.leadingprivacy.com/istanbul) conference & hackathon

- May 5-7 – [ETHMalaysia](https://ethmalaysia.com/) conference & hackathon

- **May 5-7 –** [**ETHTallinn**](https://ethtallinn.org/) **hackathon**

- **May 9-10 –** [**NFT Tallinn**](https://nfttallinn.com/) **conference**

- **May 19-23 –** [**EDCON**](https://edcon.io/) **Montenegro (changed from Vienna)**

- May 20-21 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 24-26 – [Spaghett ETH](https://naples.spaghett-eth.com/) (Naples) conference

- May 26–28 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- **Jun 2-4 –** [**ETH Seoul**](https://2023.ethseoul.org/)

- Jun 23–25 – [ETHGlobal Toronto](https://ethglobal.com/events/toronto)

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–25 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

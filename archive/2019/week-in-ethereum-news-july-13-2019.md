---
title: "Week in Ethereum News <BR>July 13, 2019"
date: "2019-07-14"
---

## **Ethereum News and Links**

**Layer 1**

- [Nimbus Eth2 client update](https://our.status.im/nimbus-development-update-12-07-2019/) - nearly up to frozen spec, 10-15x speedup in crosslink processing, better monitoring, nim libp2p, nim language for ewasm
- [Prysmatic Eth2 client update](https://medium.com/p/ethereum-2-0-development-update-30-prysmatic-labs-387ecabdfa79?_branch_match_id=642453322306233628) - up to date on spec, updated SSZ in Go
- [Eth2, phase 0 basics for new contributors](https://medium.com/coinmonks/eth2-0-phase-0-basics-for-new-contributors-8a0a22bc38c7)
- [Minimum committee size explained](https://medium.com/@chihchengliang/minimum-committee-size-explained-67047111fa20)
- Latest [Eth2 implementers call](https://www.youtube.com/watch?v=YB8o_5qjNBc). [Notes](https://github.com/ethereum/eth2.0-pm/blob/94a50a62b3b0c101236a09b3b538020a7697cfac/eth2.0-implementers-calls/call_021.md)

**Layer 2**

- Use [Bitcoin Cash as a data availability layer](https://ethresear.ch/t/bitcoin-cash-a-short-term-data-availability-layer-for-ethereum/5735) until phase 1?
- [Trustless Two-Way Bridges With Side Chains By Halting](https://ethresear.ch/t/trustless-two-way-bridges-with-side-chains-by-halting/5728)
- Celer’s state channel network went live on mainnet. See that section below.
- [Raiden Service registry](https://medium.com/raiden-network/raiden-service-bundle-explained-f9bd3f6f358d) for watchtower monitors and liquidity pathfinders
- Plasma Group’s [Optimistic Virtual Machine](https://medium.com/plasma-group/introducing-the-ovm-db253287af50), a correct-by-construction VM for all layer 2. Also applicable to phase2 of Eth2

**Client releases**

- [Geth v1.9.0](https://blog.ethereum.org/2019/07/10/geth-v1-9-0/) - a massive milestone release with performance improvements and tons of new features. [Lefteris’ tweetstorm summary](https://twitter.com/LefterisJP/status/1149370368068587520) of the changelog.
- [Parity v2.6.0-beta](https://github.com/paritytech/parity-ethereum/releases/tag/v2.6.0) and [v2.5.5-stable](https://github.com/paritytech/parity-ethereum/releases/tag/v2.5.5)

**Stuff for developers**

- White hat [samczsun found a bug in 0x code](https://blog.0xproject.com/shut-down-of-0x-exchange-v2-0-contract-and-migration-to-patched-version-6185097a1f39). As such 0x was down for a few hours last night, but the bug is now fixed. No one took advantage of it. Samczsun [explains the signature verification vulnerability](https://samczsun.com/the-0x-vulnerability-explained/)
- [Using automatic analysis tools with the MakerDAO governance code](https://forum.zeppelin.solutions/t/using-automatic-analysis-tools-with-makerdao-contracts/1021) that had a bug a few months ago.
- Runtime Verification: [how formal verification could have prevented Edgeware’s Lockdrop bug](https://runtimeverification.com/blog/how-formal-verification-could-help-to-prevent-gridlock-bug/)
- [Understanding meta transactions and native meta txs](https://medium.com/@andreafspeziale/understanding-ethereum-meta-transaction-d0d632da4eb2)
- [Alacrity](https://github.com/AlacrisIO/alacrity/blob/f1c0326ec5ebfe8c2b0fd539378071d34583947d/docs/paper.md): a DSL for simple, formally-verified code
- [Truffle DB](https://www.trufflesuite.com/blog/introducing-truffle-db-part-1): gradually introduce TruffleDB as the primary data store and slowly deprecate artifacts. Also Truffle [v5.0.27](https://github.com/trufflesuite/truffle/releases/tag/v5.0.27).
- Etherlime [v2.1.5](https://github.com/LimeChain/etherlime/releases/tag/etherlime%402.1.5) with ZeppelinOS and Chainlink integrations
- A [simple contract with the new Remix interface](https://medium.com/remix-ide/simple-contract-with-remix-7285af713d99)
- [Nethereum playground](https://twitter.com/juanfranblanco/status/1147765757171916800) now has vb.net support
- [Build an oracle with iExex](https://medium.com/iex-ec/how-to-build-a-decentralized-oracle-on-ethereum-a-step-by-step-guide-d8c14719b69f) tutorial
- OpenLaw adds [contract clauses as libraries](https://medium.com/@OpenLawOfficial/turning-contracts-into-software-libraries-with-openlaws-dynamic-contract-clauses-d4c1eaee105) to its markup language
- [Automated testing tutorial](https://forum.zeppelin.solutions/t/test-smart-contracts-like-a-rockstar/1001/1)
- [Atra adds relational database tables](https://medium.com/atra-blockchain-services/atra-releases-relational-database-tables-more-a8ffd4591e69) to its abstract-away-blockchain platform
- A dive into [Open Zeppelin’s ERC777 implementation](https://medium.com/coinmonks/deep-dive-openzeppelins-erc777-implementation-9db978ce1bea)
- How to build on [Celer’s state channel network using their gaming SDK](https://medium.com/celer-network/mainnet-developer-28a5903d7524)
- Samsung releases a [“blockchain SDK” for interacting with Ethereum](https://developer.samsung.com/blockchain)

**Ecosystem**

- [Distributed pre-image archive](https://blog.datafund.net/swarm-distributed-pre-image-archive-dpa-b13f5c683f0a) in Swarm
- ENS 3-6 character [name reservation process is now open](https://medium.com/the-ethereum-name-service/announcing-the-ens-3-6-character-eth-name-reservation-process-7f3cc4d13f65)
- Oracles: UMA publishes its [Data Verification Mechanism](https://twitter.com/hal2001/status/1149466877543845888). Joey Krug tweets his “[current state of Ethereum oracles](https://twitter.com/joeykrug/status/1150089167151386624)”

**Enterprise**

- Hyperledger founder John Wolpert: [Why businesses will learn to love the public Ethereum mainnet](https://www.coindesk.com/safety-without-silos-why-businesses-will-learn-to-love-public-ethereum)
- “[Uber Subsidiary Grants Ethereum Startup Access To Entire American Fleet](https://www.forbes.com/sites/michaeldelcastillo/2019/07/09/uber-subsidiary-grants-ethereum-startup-access-to-entire-american-fleet/#37be63e721b3)”
- Singapore Exchange [launches securities token exchange](https://www.coindesk.com/singapores-stock-exchange-backs-new-ethereum-security-token-platform)

**Governance and Standards**

- [ERC2182](https://github.com/ethereum/EIPs/blob/2962a396d7035b8bf9eba50b4beea073c39db2bd/EIPS/eip-2182.md): Reduce the Clique signer\_limit
- [ERC2181](https://github.com/ethereum/EIPs/blob/0433bed74daf244ca900a67c5c223fff619e5cfc/EIPS/eip-2181.md): Increase Clique’s diff\_inturn
- [ERC2183](https://github.com/ethereum/EIPs/pull/2183): Increase Clique min\_wait for out of turn blocks
- [dxDAO now owns DutchX](https://blog.gnosis.pm/gnosis-is-stepping-back-from-the-dxdao-5d368bc269a3), and Gnosis has stepped away from dxDAO

**Live on mainnet**

- [Celer’s state channel network](https://medium.com/celer-network/cygnus-979b92892481) live on mainnet. Play Gomoku or FishJump for Dai/Eth/tokens.
- [Nexus Mutual’s smart contract cover](https://medium.com/nexus-mutual/smart-contract-cover-is-now-live-91b3015f99eb) is now live on mainnet, so now you can insure yourself against bugs and hacks. That means [GovBlocks is also live](https://twitter.com/ishgoel/status/1148974322641276928) on mainnet for co-op governance.

**Application layer**

- Dai Stability Fee went up first to 18.5% a few days ago and then [today it went up to 20.5%](https://twitter.com/nanexcool/status/1150167445740687361). Also, [how to nominate tokens for multi collateral Dai](https://blog.makerdao.com/collateral-onboarding-guide-how-to-nominate-tokens-for-mcd/)
- Veil is [sunsetting its prediction markets product](https://medium.com/veil-blog/next-steps-for-veil-133777c4a774)
- [KyperSwap now has limit orders](https://medium.com/kyberswap/limit-orders-new-feature-on-kyberswap-e2957c5d51ae)
- [NiftySwap](https://twitter.com/PhABCD/status/1149774205300432896): a Uniswap fork for ERC1155 NFTs using Dai and metatransactions
- [Ocean Protocol went live](https://blog.oceanprotocol.com/announcing-pacific-network-live-poa-mainnet-6c343f48e866) on POAnet
- A [list of ENS + IPFS websites](http://almonit.club/blog/ens+ipfs/list-of_ENSIPFS-websites.html)
- BAT in [Brave Ads now available on Android](https://brave.com/brave-ads-on-android/) in US, Canada, UK, France and Germany. 22% clickthrough so far
- [Decentraland now has avatars](https://decentraland.org/blog/announcements/avatars/)
- [Panvala’s beta is live on Rinkeby](https://medium.com/@Panvala/panvala-beta-release-what-would-you-fund-22e4018a9cd3), so you can choose what slates get PAN tokens.
- FunFair’s [affiliate program now pays on-chain in real time](https://funfair.io/on-chain-affiliate-program-live/)
- Loanscan [q2 report on DeFi lending](https://medium.com/loanscan/digital-asset-lending-via-decentralized-lending-protocols-q2-2019-e10ec4d48098). It’s growing fast.
- Golem [v0.20 release with gwasm](https://blog.golemproject.net/brass-golem-beta-0-20-0-gwasm-and-raspa-have-arrived/)

**Interviews, Podcasts, Videos, Talks** 

- Compound’s [Robert Leshner](https://epicenter.tv/episode/295/) on Epicenter
- [ETHNewYork videos](https://www.youtube.com/playlist?list=PLXzKMXK2aHh6STXEnNfU45U2wIwo4ZhyC)
- [Billy Rennekamp on CadCAD](https://www.youtube.com/watch?v=5Eg360OC6Qg)
- Washington Post’s [Jarrod Dicker](https://www.youtube.com/watch?v=swUd-mac6G4&feature=youtu.be) talks media and web3 with Mike Kriak
- Truffle’s [Tim Coulter](https://medium.com/@TrustlessState/pov-crypto-episode-62-truffle-making-ethereum-sweet-with-tim-coulter-d0fa68257302) on POV Crypto
- TokenCard’s [Mel Gelderman](https://ethhub.substack.com/p/tokencard-path-to-a-self-sovereign) on Into the Ether
- Zexe's [Pratyush Mishra](https://www.zeroknowledge.fm/85) on Zero Knowledge
- Instadapp’s [Sowmay Jain](https://ethhub.substack.com/p/instadapp-a-bridge-to-decentralized) on Into the Ether

**Tokens / Business / Regulation**

- [FEC says federal candidates can give ERC20 loyalty tokens](https://www.fec.gov/files/legal/aos/2019-08/201908.pdf) to their volunteers
- Synthetix offers [incentives to Uniswap liquidity providers](https://blog.synthetix.io/uniswap-seth-pool-incentives/)
- SEC [approves RegA+ for YouNow’s Props Project](https://blog.propsproject.com/props-launches-the-first-sec-approved-crypto-token-for-consumers-a33fb7567900) so they can give away tokens to users. Blockstack also got approval.
- SEC/FINRA staff statement on [broker-dealer custody of cryptoassets](https://www.sec.gov/news/public-statement/joint-staff-statement-broker-dealer-custody-digital-asset-securities)
- “[Ethereum is quietly becoming the global platform for every asset](https://twitter.com/MuteDialog/status/1149047398532075526)”

**General**

- [tryethereum.today](https://tryethereum.today/): a site for beginners to discover things to do with Eth
- Shapeshift becomes a [non-custodial exchange](https://medium.com/shapeshift-stories/building-a-bridge-to-financial-sovereignty-5cad4323bfe6) where you have to use hardware wallets
- Summary of [Wasm for blockchain](https://medium.com/nearprotocol/wasm-for-blockchain-2019-d093bfeb6133) event last month
- Bowe: [Faster Subgroup Checks for BLS12-381](https://eprint.iacr.org/2019/814)
- Microsoft research: [leveraging Ethereum to make machine learning models more accessible](https://www.microsoft.com/en-us/research/blog/leveraging-blockchain-to-make-machine-learning-models-more-accessible/)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- **July 15 - [Eth2 researcher AMA](https://twitter.com/drakefjustin/status/1149700891253104640)**
- **July 17 - [Devcon ticket sales](https://twitter.com/EFDevcon/status/1149281591463686145), wave 1**
- July 19 - [BuildETH](https://www.buildeth.io/) (San Francisco)
- July 19-21 - [State of Scale](https://www.stateofscale.com/) (Los Angeles)
- July 19-21 - [ConsenSys Grants hackathon](https://pages.consensys.net/consensys-grants-hackathon-new-york) (Brooklyn)
- July 22-23 - [Buidl](https://www.buidl.asia/) 2019 (Seoul)
- Aug 2-4 - [ETHIndia](https://ethindia.co/) (Bangalore)
- Aug 2-4 - [TruffleCon](https://www.truffleframework.com/trufflecon2019) (Redmond)
- Aug 21-23 - [Dappcon](https://dappcon.io/) (Berlin)
- Aug 23-25 - [ETHBerlin](https://ethberlinzwei.com/)
- Sep 3 - Deadline to [apply for EU Horizon Prize](https://ec.europa.eu/info/funding-tenders/opportunities/portal/screen/opportunities/topic-details/blockchain-eicprize-2019). 1m € each to 5 "Blockchains for Social Good" projects
- Sep 6-8 - [EthBoston](https://eth.boston/)
- Sep 15 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff/)
- Sep 15 - [Ethereal Tel Aviv](https://etherealsummit.com/events/ethereal-tel-aviv/)
- Sep 15-16- [StarkWare sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- Oct 8-11 - [DeVcon](https://devcon.org/) (Osaka)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I own 100% Week In Ethereum. Editorial control has always been me.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **This headline stays as long as so many people continue to link to old URL and not the right one: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/week-in-ethereum-news-july-13-2019/](https://weekinethereumnews.com/week-in-ethereum-news-july-13-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

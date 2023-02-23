---
title: "Week in Ethereum News <BR> June 28, 2020"
date: "2020-06-28"
---

## **Eth News and Links**

**Eth1**

- Latest [core devs call](https://youtu.be/IZEcukn9J0Y). Tim Beiko’s [notes](https://twitter.com/TimBeiko/status/1276512216557260802): lots of discussion of needing more client diversity rather than more features, as well as sharing the testing load and simplification of the protocol.
- [Regenesis](https://ethresear.ch/t/regenesis-resetting-ethereum-to-reduce-the-burden-of-large-blockchain-and-state/7582): a Cosmos-like reset proposal from Alexey Akhunov
- [Sharding state with discovery and adaptive range filters](https://ethresear.ch/t/sharding-state-with-discovery-and-adaptive-range-filter-ads/7573)
- Latest [eip1559 call](https://www.youtube.com/watch?v=2qDfW83gnDA). Beiko’s [notes](https://twitter.com/TimBeiko/status/1272534442792419328).
- Barnabé Monnot’s [1559 and escalator analysis](https://github.com/ethereum/rig/blob/master/eip1559/notes-call3.md)
- Hasu and Georgios Konstantopoulos analyze [EIP2593’s escalator algo](https://insights.deribit.com/market-research/analysis-of-eip-2593-escalator/) to change the fee market, in conjunction with EIP1559. EIP2593 author [Dan Finlay’s response](https://twitter.com/danfinlay/status/1275826052846125056).

**Eth2**

- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200627)
- Danny Ryan’s [quick update](https://blog.ethereum.org/2020/06/23/eth2-quick-update-no-12/) - deposit contract rewritten in Solidity by Axic, formally verified by Runtime Verification. The Altona multi-client testnet starts June 29.
- Early [benchmarking of Eth2 clients](https://github.com/q9f/eth2-bench-2020-06/blob/master/res/2020-06-eth2-bench.pdf) - Lighthouse with the early lead
- Latest [eth2 call](https://www.youtube.com/watch?v=P1AEmUt9ltg). Notes from [Ben](https://hackmd.io/@benjaminion/r1PieQMAU) and [William Schwab](https://github.com/ethereum/eth2.0-pm/blob/555d787a21c372b5cec5d849ebc3ddf1b6f0aa5b/eth2.0-implementers-calls/call_042.md)
- [Architecture of a geth based eth1 engine](https://ethresear.ch/t/architecture-of-a-geth-based-eth1-engine/7574) inside of eth2
- [Secret shared validators](https://medium.com/@mara.schmiedt/secret-shared-validators-on-ethereum-2-0-ea29ab380016) in Eth2

**Layer2**

- [Web3Torrent](https://blog.statechannels.org/introducing-web3torrent/) “browser based torrenting client that supports incentivized peer-to-peer filesharing” using state channels for micropayments. live on Goerli testnet

**Crypto**

- StarkWare’s [VeeDo](https://medium.com/starkware/presenting-veedo-e4bbff77c7ae) Stark-based VDF, PoC live on mainnet

* * *

### **This newsletter is made possible thanks to [Chainlink](https://chain.link/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/05/FE39n5_g.png)

Building a DeFi application? Make sure you’re using the best possible [price data oracle](https://feeds.chain.link/) to access provably secure off-chain data. [Chainlink](https://chain.link/) is already used by leading teams like Synthetix, Aave, Set Protocol, Bancor, 1inch, Kyber and many more.

* * *

**Stuff for developers**

- [Sourcify FAQ](https://solidity.ethereum.org/2020/06/25/sourcify-faq/) decentralized opensource verification with NatSpec
- OpenZeppelin Contracts [v3.1](https://forum.openzeppelin.com/t/openzeppelin-contracts-v3-1/3159)
- Need [free access to an archive node](https://medium.com/@defidude/archivenode-io-the-public-access-ethereum-archive-node-72284a4b9797)?
- [Flash mintable asset backed tokens](https://blog.openzeppelin.com/flash-mintable-asset-backed-tokens/)
- [Debugging verified external contracts](https://www.trufflesuite.com/blog/debugging-verified-external-contracts-with-truffle-debugger) with Truffle
- Fast [event log searches](https://blog.openrelay.xyz/flume/) on your own node with Flume
- (unaudited) Solidity library to [use Uniswapv2 oracle with storage proofs](https://medium.com/@epheph/using-uniswap-v2-oracle-with-storage-proofs-3530e699e1d3)
- Comparing [queue routines in C and Solidity](https://medium.com/coinmonks/comparing-queue-routines-in-c-and-solidity-e44813e29f75)
- Shadowing [Solidity storage variables in memory](https://medium.com/coinmonks/shadowing-solidity-storage-variables-in-memory-b56f471edd81)
- Ethereum’s [merkle trees javascript tutorial](https://rockwaterweb.com/ethereum-merkle-patricia-trees-javascript-tutorial/)
- How to build a [decentralized auction](https://m-chrzan.xyz/blog/bst-auction.html)
- [Samczsun finds Atomic Loans vulnerabilities](https://atomic.loans/blog/vulnerability-disclosure-and-pause-new-loan-requests/), loans essentially disabled until v2
- Exploring [Solidity’s model checker](https://www.aon.com/cyber-solutions/aon_cyber_labs/exploring-soliditys-model-checker/)
- Check out this **newsletter’s weekly job listings** below the general section

**Ecosystem**

- [Book of Swarm](https://medium.com/ethereum-swarm/this-is-book-of-swarm-e7ba645cbe23) is published on Swarm, free and open source
- [HOPR incentivized mixnet](https://medium.com/hoprnet/introducing-hopr-your-next-generation-data-privacy-and-protection-platform-d4c8ef634fdc) has incentivized testnets
- [Stablecoins v2](https://medium.com/coinmonks/stablecoins-2-0-economic-foundations-for-defi-b9ab38500b87): a framework for analyzing risk of DeFi’s foundations
- [Unilogin](https://medium.com/universal-ethereum/unilogin-and-the-quest-for-a-better-txn-fees-ux-10bd9d6dd6e9): pay transaction fees with tokens or app pays for users

**Enterprise**

- Privacy improvements in [Hyperledger Besu v1.5](https://pegasys.tech/privacy-upgrades-for-hyperledger-besu-1-5/)
- Unibright and Fraunhofer [baselining additive manufacturing](https://medium.com/unibrightio/unibright-and-fraunhofer-ipk-collaborate-on-baselining-additive-manufacturing-7469c36143a3)
- Multisig for enterprise: [Multis gets a revamp](https://medium.com/multis/making-defi-beautiful-the-multis-app-revamp-6d5f72cb2b)

**DAOs and Standards**

- [EIP2751](https://github.com/ethereum/EIPs/blob/a2a2e5cb816d5663c076e996096cb2cb5cff4f35/EIPS/eip-draft_disable_selfdestruct.md): Disable SELFDESTRUCT opcode
- [ERC2746](https://github.com/ethereum/EIPs/blob/9de5a43863f242424702dd4f16ea1358eb50cff5/EIPS/eip-draft_rules_engine.md): Rules Engine Standard
- Jameson: [who is a core dev?](https://hudsonjameson.com/2020-06-22-what-is-an-ethereum-core-developer/)
- Golem’s [governance via preset preferences](https://blog.golemproject.net/governing-preferences/) proposal

**Application layer**

- [PolyMarket](https://poly.market/discover) prediction markets live on mainnet using USDC and Gnosis (unclear what was audited?)
- [SportX v2.5](https://blog.sportx.bet/introducing-sportx-v2-5/) - noncustodial betting app on Eth adds tournaments and referrals
- [HAL Recipes](https://medium.com/hal-xyz/introducing-recipes-1fa7cece5ac4) 1 click IFTTT for Ethereum
- [Status v1.4](https://our.status.im/v1-4-release-keycard-integration-and-notifications-for-android/) with Keycard integration and Android notifications
- A nugget to illustrate how dex volume (eg, [DuneAnalytics dex dashboard](https://explore.duneanalytics.com/public/dashboards/c87JEtVi2GlyIZHQOR02NsfyJV48eaKEQSiKplJ7)) is exploding: [Uniswap to do more volume this month than in all of 2019](https://twitter.com/haydenzadams/status/1276212570597347328)
- [Balancer minted their token](https://medium.com/balancer-protocol/bal-is-live-104ba56e1945), it reached 2 billion fully diluted valuation. Today: [~500k USD drained from deflationary token pools](https://etherscan.io/address/0xbf675c80540111a310b06e1482f9127ef4e7469a#internaltx)
- [MakerDAO changes](https://twitter.com/nanexcool/status/1277126687021576192) - KNC/ZRX collateral, 0.25% stability fee increase

**Tokens/Business/Regulation**

- [Tokenized ownership is the best coordination tool since equity](https://medium.com/fabric-ventures/tokenised-ownership-is-the-best-coordination-tool-since-equity-7c957a00d818)
- Dan Elitzer: [Aquaponic yield farming](https://bankless.substack.com/p/aquaponic-yield-farming)
- DeFiSaver: [experimenting with different settings for profits](https://medium.com/defi-saver/defi-saver-automation-performance-analysis-setting-up-for-maximum-profits-eb486b5c9ea6) (be careful!)
- [Yield farming tips](https://thedefiant.substack.com/p/top-defi-yield-farmers-share-secrets) in the Defiant
- [5 contrarian takes with DegenSpartan](https://bankless.substack.com/p/5-contrarian-takes-with-degenspartan)
- Tether is [migrating Tether previously on Tron into Ethereum](https://twitter.com/Tether_to/status/1275086995493191681)
- There is now over [10k btc on eth](https://btconethereum.com/) (11.1k at time of publication)
- [Mandated backdoors to all encryption bill](https://cyberlaw.stanford.edu/blog/2020/06/there%E2%80%99s-now-even-worse-anti-encryption-bill-earn-it-doesn%E2%80%99t-make-earn-it-bill-ok) introduced in US Senate

**General**

- [Phishing campaigns aimed at DeFi](https://medium.com/mycrypto/phishing-campaigns-take-aim-at-web3-defi-applications-19e224d9f207) apps
- Silk Road’s Ross Ulbricht has some things he [wishes Maker did differently](https://medium.com/@RossUlbricht/remaking-the-maker-protocol-4b29f879f11)
- Soon you can [buy crypto using Paypal/Venmo](https://www.coindesk.com/paypal-venmo-to-roll-out-crypto-buying-and-selling)
- [AMD/ConsenSys joint venture](https://media.consensys.net/w3bcloud-raises-20-5-million-to-roll-out-data-centers-for-the-blockchain-economy-a4639eab8afa) for “Ethereum blockchain data centers”
- All the videos for [a16z’s crypto startup school](https://a16z.com/crypto-startup-school/)

* * *

## **Job Listings**

- Blockchains, LLC is hiring [full stack](https://www.blockchains.com/careers/?gh_jid=4750540002&gh_src=dcb3016b2us), [front end](https://www.blockchains.com/careers/?gh_jid=4750551002&gh_src=07e5f4692us), & [back end](https://www.blockchains.com/careers/?gh_jid=4750478002&gh_src=7c1607432us) developers!
- Monolith is looking for an amazing [Finance & Treasury Manager](https://apply.workable.com/monolithweb3/j/2FD4CAC261/)! Interested?
- [0x is hiring](https://0x.org/about/jobs) full-stack, back-end, front-end engineers + 1 data scientist
- Chainlink: [Product Manager for Blockchain Integrations](https://careers.smartcontract.com/o/product-manager-blockchain-integrations) and [Lead Test Engineer](https://careers.smartcontract.com/o/lead-test-engineer-on-chainlink)
- Trail of Bits is looking for masters of low-level security. [Apply here](https://jobs.lever.co/trailofbits/8b7f7fc1-efb0-4e89-b406-784c3a2d77e4).
- Celer Network: [Android developer](https://www.celer.network/career.html)
- [Avantgarde Finance](https://avantgarde.finance/) ([Melon](https://melonprotocol.com/)): hiring for [senior solidity dev](https://www.notion.so/Senior-Smart-Contract-Developer-to-work-on-the-Melon-Protocol-641aef0d89cc419cba792445354f835b) & [frontend dev](https://www.notion.so/avantgardefinance/Front-end-developer-for-Avantgarde-Finance-6c95d0005ef3494c8d48ddedc90c3d80)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH/DAI/USDC to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **Housekeeping**

Follow me on Twitter [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get the **annotated edition of this newsletter** on Monday or Tuesday. Plus I tweet most of what makes it into the newsletter.

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-june-28-2020/](https://weekinethereumnews.com/week-in-ethereum-news-june-28-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- June 29 - [Swarm first public event](https://swarm-gateways.net/bzz:/alpha.swarm.eth/)
- **July 6 - [StarkWare VDF/randomness hackathon](https://starkware.co/10289000-2/)**
- July 3 - [Gitcoin donation matching](https://gitcoin.co/grants) ends
- July 6-Aug 6 - [HackFS](https://hackfs.com/) Filecoin/IPFS and Ethereum hackathon
- **July 10 - next core dev call**
- July 20 - [Fork the World](https://metagame.substack.com/p/fork-the-world-hackathon) MetaCartel hackathon
- **July 30 - EEA’s [Ethereum in the Enterprise 2020](https://www.conference.entethalliance.org/) virtual conference**
- Aug 2 - [ENS grace period](https://medium.com/the-ethereum-name-service/the-great-renewal-its-time-to-renew-your-eth-names-or-else-lose-them-afccea4852cb) begins to end
- Oct 2-Oct 30 - [EthOnline hackathon](https://www.ethonline.org/)

---
title: "Week in Ethereum News<BR> February 16, 2020"
date: "2020-02-17"
---

## **Eth News and Links**

**Eth1**

- Nethermind [v1.6.3](https://github.com/NethermindEth/nethermind/releases/tag/1.6.3) with Beam Sync preview on Goerli testnet
- [Turbo-geth uses 70% less disk space](https://medium.com/@giulio.rebuffo/turbo-geth-whats-different-the-database-5916e8ec834b) using B+- Trees as well as Bolt instead of leveldb. In production, this would reduce archive nodes to below 1tb
- [Semi-stateless initial sync experiment](https://medium.com/@mandrigin/semi-stateless-initial-sync-experiment-897cc9c330cb) using Turbo-geth
- [EVM-LLVM alpha](https://medium.com/etc-core/announcing-evm-llvm-alpha-release-the-next-level-in-smart-contract-evolution-91a2119bd442) release, to allow LLVM tooling to compile to EVM
- [Tricking frontrunners into being transaction relayers](https://ethresear.ch/t/surrogeth-tricking-frontrunners-into-being-transaction-relayers/6937)

**Eth2**

- [PrysmaticLabs client](https://medium.com/prysmatic-labs/eth-2-0-dev-update-44-more-optimizations-6ab9a4e328c9) update - optimizations, more user friendly, new team member
- Lighthouse can run [100k validators on 12 cheap (dual core, 4gb ram) AWS instances](https://twitter.com/paulhauner/status/1226817210057805825)
- How [LMD Ghost fork choice and Casper FFG work together](https://blog.ethereum.org/2020/02/12/validated-staking-on-eth2-2-two-ghosts-in-a-trench-coat/) to satisfy safety and liveness requirements
- Balance those 2 plus [timeliness detectors](https://ethresear.ch/t/timeliness-detectors-and-51-attack-recovery-in-blockchains/6925) to satisfy asynchronous requirements
- Tools to write [eth2 execution environments](https://twitter.com/matt_garnett/status/1228426170137481218) more easily
- How [state providers can keep the state cheaply](https://ethresear.ch/t/preventing-shard-state-data-loss-using-custody-roots/6952) using custody root
- [Time attacks and security models](https://ethresear.ch/t/time-attacks-and-security-models/6936)
- Correcting the [top 5 Eth2 misconceptions](https://medium.com/@trenton.v/eth2-misconceptions-top-5-6edafaeccac1)

**Layer2**

- Offchain Labs’ [Arbitrum rollup](https://medium.com/offchainlabs/arbitrum-rollup-is-live-on-testnet-c5fed0d0a266) is live on testnet, supports Solidity compiler
- [OVM alpha](https://medium.com/@optimismPBC/optimistic-virtual-machine-alpha-cdf51f5d49e) - how Optimism will offer full EVM support in their optimistic rollups
- Matic’s [incentivized testnet](https://twitter.com/maticnetwork/status/1227580874440335360) is live
- Perun’s [Ethna: Channel Network with Dynamic Internal Payment Splitting](https://eprint.iacr.org/2020/166)
- CelerNetwork releases [multi-hop state channels and open sourced the state channels node](https://medium.com/celer-network/celers-lyra-mainnet-launches-with-production-grade-open-source-code-214660abffa), as well as launched the [testnet for its guardian watchtower network](https://medium.com/celer-network/celer-launches-state-guardian-network-staking-testnet-with-open-source-code-release-a20040d74080)
- [StateChannels reduces gas cost by ~75%](https://medium.com/statechannels/state-channels-gas-optimization-on-ethereum-34bcdd7225d9) by reducing all storage to a minimum bytes32 slot

**Stuff for developers**

- OpenZeppelin [CLI v2.7](https://forum.openzeppelin.com/t/openzeppelin-cli-2-7/2252) - full Solidity v0.6 support, typechain artefacts
- Guide to use [Create2.sol library in OpenZeppelin Contracts 2.5](https://forum.openzeppelin.com/t/guide-to-using-create2-sol-library-in-openzeppelin-contracts-2-5-to-deploy-a-vault-contract/2268)
- [Subspace v1.3](https://github.com/embarklabs/subspace/releases/tag/1.3.0) - new methods to track blocks, gas price and blocktime
- Pisa’s [any.sender](https://medium.com/pisa-research/any-sender-transactions-made-simple-34b36ba7519b), a non-custodial way to abstract away your transactions via API
- Blocknative’s [internal transaction monitoring](https://blog.blocknative.com/blog/eth-internal-transactions)
- [Property-based Eth code testing](https://medium.com/@iamdefinitelyahuman/effective-smart-contract-testing-property-based-testing-9e2a2b1fe77e) with Brownie
- [Compiling Formality to Javascript](https://medium.com/@maiavictor/the-refreshing-simplicity-of-compiling-formality-to-anything-388a1616f36a)
- A look at the [Trueblocks frontend](https://medium.com/@tjayrush/trueblocks-first-quarter-2020-update-a02740b25e5b) to get all the data you want out from running your own node
- [QueryEthereum](https://www.reddit.com/r/ethereum/comments/f2ngcu/query_ethereum_chain_analysis_from_a_browser_tab/): GraphQL API from a browser tab
- [SplunkConnect](https://www.splunk.com/en_us/blog/it/introducing-splunk-connect-for-ethereum.html) for Ethereum, analytics platform connects to Infura or your node
- [Setting up your Eth dev environment](https://medium.com/compound-finance/setting-up-an-ethereum-development-environment-7c387664c5fe), a quick start guide from Compound
- [create-Eth-app](https://github.com/PaulRBerg/create-eth-app): CLI tool to create Ethereum-powered React apps with one command
- [Dapphero video tutorial](https://www.youtube.com/watch?v=cZ8eQRP0V5Y&feature=youtu.be) - web3 nocode
- [Terminal v2](https://blog.terminal.co/introducing-terminal-v2/) - Netlify on IPFS
- 3Box [Confidential Threads API](https://medium.com/3box/confidential-threads-api-17df60b34431)

**Ecosystem**

- How to [scale anonymous transactions](https://ethresear.ch/t/state-of-zeropool-scaling-anonymous-transactions-for-ethereum/6946) with Zeropool
- [ENSRegistry migration](https://medium.com/the-ethereum-name-service/ens-registry-migration-is-over-now-what-a-few-things-to-know-fb05f921872a): updating your resolver and subdomains
- [Authereum](https://medium.com/authereum/authereum-is-live-f97d88e7153e) is live on mainnet. Email and password, your account is recoverable as long as you maintain local storage or password.
- [Torus out of beta](https://medium.com/toruslabs/torus-v1-0-the-path-to-decentralized-custody-1bab14f798). Use your Google, Facebook, Reddit, Discord or Twitch accounts for your Eth account
- Chrome store now shows [1+ million for MetaMask](https://twitter.com/calchulus/status/1228152141677654018), though they actually [crossed 1 million](https://twitter.com/metamask_io/status/961628855328018434) two years ago
- [Waku spec v3](https://vac.dev/waku-update), Whisper-alternative, with some simulations for messaging scalability
- [Tornado.cash](https://medium.com/@tornado.cash/vulnerability-disclosure-f610fb7f2c8d) releases full details of recent UI vulnerability. Clicking “share URL” would store the note via API call in a bunch of 3rd party services.
- [Annotated versions of Week in Ethereum News](https://www.evanvanness.com/post/190777321891/annotated-edition-for-week-in-ethereum-news-feb-9) appear the day after publication on evanvanness.com

**Enterprise**

- Conor Svensson’s brief history of [enterprise Ethereum standards](https://blog.web3labs.com/a-brief-history-of-enterprise-ethereum-standards)
- [Vermont regulators using Trace to track hemp production](https://www.coindesk.com/vermont-turns-to-home-grown-blockchain-company-to-track-hemp-with-ethereum) on mainnet
- [Ship financing platform](https://www.securities.io/new-shore-invest-starts-a-new-ship-finance-platform/) on mainnet
- Reuters reports that [JPMorgan and ConsenSys are discussing the future of Quorum](https://www.reuters.com/article/us-jp-morgan-blockchain-exclusive-idUSKBN2051AW)
- [Besu v1.4](https://pegasys.tech/increase-adoption-and-cut-costs-with-multi-tenancy-on-hyperledger-besu/) - privacy multi-tenanted environment, e2e for RPC endpoints;

**Governance, DAOs, TheDAOv2, and standards**

- [MetaCartel Ventures DAO](https://defirate.com/mcv-launch/) is live on mainnet
- [Pre-registration open for theLAO](https://medium.com/@thelaoofficial/join-the-lao-a4ae9592a3a4), as it is set to launch in a few weeks for up to 100 accredited investors
- SignalDAO’s experiments with [automating DAO voting using Telegram bots](https://medium.com/abridged-io/recapping-the-1st-phase-of-signal-dao-looking-forward-to-future-experiments-cce4a143bed1)
- [Aragon Court](https://blog.aragon.org/launching-aragon-court/) is live on mainnet, arbitration for their DAOs. currently working on some moot/hypothetical cases
- [Kleros Governor](https://blog.kleros.io/introducing-kleros-governor/), the DAO to govern Kleros
- Nikolai says [Maker’s contracts already support a function to thwart the governance attack](https://nikolai.fyi/posts/transition-attack-not-applicable.html) but the UI does not expose it
- [DAOifying Uniswap’s pools](https://ethresear.ch/t/daoifying-uniswap-amm-pools/6945), an idea from Sunny Aggarwal
- [EIP2515](https://github.com/ethereum/EIPs/blob/3c0275603d4656ba46a507b09828a5febe141ef7/EIPS/eip-2515.md): Replace difficulty bomb with difficulty freeze

**Application layer**

- [Status v1](https://our.status.im/announcing-status-version-1-0/) is live on mainnet. A privacy-focused wallet, chat app, and web3 browser. It’s a breaking change from the beta, so backup your pre-v1 seed phrase
- [Opyn is live on mainnet](https://medium.com/opyn/opyn-launches-insurance-platform-to-protect-defi-users-fdcabaca7d97), tokenized options platform to speculate/insure.
- [Metacoin](https://ethresear.ch/t/announcing-metacoin-the-governance-minimized-decentralized-stablecoin/6897). Ameen proposes a solely-ETH collateral, onchain Uniswap oracle, and governance minimized stablecoin
- [Mstable](https://medium.com/mstable/introducing-mstable-4e1cecbdcdd4): basket of stablecoins and tokenized assets to diversify counterparty risk
- [Nuoscan](https://nuoscan.io/), a Nuo Network explorer
- [AdEx is out of beta](https://www.adex.network/blog/platform-out-of-private-beta/), now live for everyone. Advertising platform with instant Dai payouts using unidirectional payment channels
- [1 million dollars in virtual real estate sales](https://medium.com/play-to-earn/gamers-invested-1-million-dollars-in-virtual-land-this-week-256cddb0eec6) this week
- [Charged Particles](https://charged-particles.netlify.com/): interest-bearing NFTs
- Colony Network’s [BetaColony](https://blog.colony.io/introducing-the-betacolony/) - the experimental version of the MetaColony
- How [PoolTogether selects winners](https://medium.com/pooltogether/how-pooltogether-selects-winners-9301f8d76730)
- [bZx had an extreme arbitrage event](https://twitter.com/bzxHQ/status/1228787125740437504), using flashloans to push the oracle down. bZx will use their admin key to stream the remaining collateral to iEth holders. Check out the [data visualization of the transaction](https://twitter.com/spencernoon/status/1228775982699601926/photo/1) from bloxy.info

**Tokens/Business/Regulation**

- de la Rouviere: [Markets as medium](https://blog.simondlr.com/new-markets-in-the-arts-markets-as-medium)
- The [top25 tokens by market cap are all on Ethereum](https://twitter.com/drakefjustin/status/1227574343393255424)
- [Value capture in DeFi](https://bankless.substack.com/p/the-great-protocol-sink-market-monday-194): protocol sink
- [PE ratio](https://bankless.substack.com/p/are-defi-tokens-worth-buying) for tokens
- Former Eth foe Grayscale calls [ETH a store of value](https://twitter.com/spencernoon/status/1228040241652666368)
- [Balance sheet as business model](https://thedefiant.substack.com/p/balance-sheet-as-a-business-model) in synthetic asset platforms
- [QCAD](https://medium.com/@Stablecorp/introducing-qcad-by-stablecorp-bc7216194e82) - a collateralized Canadian dollar token
- The [rise of the cryptodollar](https://bankless.substack.com/p/rise-of-the-cryptodollar)
- [Barça joins major football clubs](https://www.bloomberg.com/news/articles/2020-02-13/fc-barcelona-to-issue-tokens-for-blockchain-based-fan-platform) in issuing Chiliz fan tokens
- [SKALE to launch its token on ConsenSys’ Activate](https://consensys.net/blog/press-release/consensys-codefi-announces-skale-network-as-the-first-project-to-launch-a-token-on-the-activate-platform) platform, focused on token distribution to users

**General**

- [Kate commitments from the Lagrange basis without FFTs](https://ethresear.ch/t/kate-commitments-from-the-lagrange-basis-without-ffts/6950)
- A [visual intro to Sparse Merkle Trees](https://blog.iden3.io/sparse-merkle-trees-visual-introduction.html)
- [Dai integrated in Coinbase Commerce](https://blog.makerdao.com/dai-integrated-as-a-payment-option-on-coinbase-commerce-offering-the-stablecoin-to-millions-via-shopify-woocommerce-and-other-merchants/). We should pay for everything in Dai/stablecoins that we can.
- MakerDao makes [Forbes Fintech 50](https://twitter.com/MakerDAO/status/1227625154819158016)
- [Coinbase brings back margin trading](https://blog.coinbase.com/margin-trading-is-now-available-on-coinbase-pro-b22743a0e07b) for 23 US states
- [What is a derivation path](https://medium.com/mycrypto/wtf-is-a-derivation-path-c3493ca2eb52), a MyCrypto explainer

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Feb 18-Mar 31 - [Social Impact hackathon/incubator](https://blockchainforsocialimpact.com/incubator/)
- Feb 20 - [NFT.NYC](https://www.nft.nyc/)
- Feb 20 - [Decentraland launch](https://decentraland.org/blog/announcements/decentraland-announces-publich-launch/)
- Feb 28-Mar 1 - [ETHLondon UK](https://ethlondon.com/)
- Mar 3-5 - [EthCC](https://ethcc.io/) (Paris)
- Mar 6-8 - [EthParis2020](https://www.hackparis.io/)
- Mar 29-Apr4 - [EthLagos](https://ethlagos.io/)
- Apr 3-7 - [Edcon](https://www.edcon.io/) (Vienna)
- Apr 13 - Deadline to apply for [50k euro for blockchain startup](https://blockchers.eu/open-calls/)s in Europe
- April 24-26 - [EthTurin](https://ethturin.com/)
- May 8-9 - [Ethereal Summit](https://www.etherealsummit.com/) (NYC)
- May 15-17 - [ETHNYC](https://nyc.ethglobal.co/)
- May 15 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

* * *

## **Thank you, ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum News. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

* * *

## **I really want you to link to [weekinethereumnews.com](https://weekinethereumnews.com/)**

Issue permalink: [https://weekinethereumnews.com/week-in-ethereum-news-february-16-2020/](https://weekinethereumnews.com/week-in-ethereum-news-february-16-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

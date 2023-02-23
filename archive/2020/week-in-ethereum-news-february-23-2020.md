---
title: "Week in Ethereum News<BR> February 23, 2020"
date: "2020-02-25"
---

## **Eth News and Links**

**Eth1**

- Geth [v1.9.11](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.11). DNS peer discovery, EIP2464 implementation, faster Geth console
- Latest [core devs call](https://youtu.be/zSRzlC_dCx8). [Notes](https://twitter.com/TimBeiko/status/1230854066718355456). Lots of next fork planning. EVM subroutines likely happening pending Solidity benchmarks, ProgPoW back on the agenda, lots of eip1962 precompile talk
- Draft [spec for block witnesses](https://github.com/ethereum/stateless-ethereum-specs/pull/1)
- [Stateless Eth1 update](https://blog.ethereum.org/2020/02/18/eth1x-files-the-statelessness-of-the-union/)
- draft EIP to [add BLS12-381 precompiles to the EVM](https://hackmd.io/@ralexstokes/rJegpNo7I)
- [Implementing account abstraction](https://ethereum-magicians.org/t/implementing-account-abstraction-as-part-of-eth1-x/4020) via new PAYGAS opcode
- [Rich transaction compile draft EIP](https://github.com/Arachnid/EIPs/blob/richtx/EIPS/EIP-draft-rich-transactions.md). allow transactions from EOAs to bytcode directly

**Eth2**

- Latest [what’s new in Eth2](https://notes.ethereum.org/@ChihChengLiang/Sk8Zs--CQ/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200221?type=book)
- Update on [fuzzing the beacon chain clients](https://blog.sigmaprime.io/beacon-fuzz-02.html). Finding bugs, expanding capabilities
- A short history and a [way forward for phase 2](https://ethresear.ch/t/a-short-history-and-a-way-forward-for-phase-2/6982)
- [Automated detection of dynamic state access](https://www.reddit.com/r/ethereum/comments/f7sw9a/automated_detection_of_dynamic_state_access_in/)
- Casey Detrio’s [simple protocol for cross-shard transfers](https://ethresear.ch/t/a-protocol-for-cross-shard-eth-transfers-even-more-simpler-and-transparent/6996)
- Quick demo on [getting an eth2 EE up and running](https://twitter.com/JonnyRhea/status/1230195894236086277) using Quilt’s [SEE](https://github.com/quilt/see) tool

**Layer2**

- Daniel Goldman: the [state of optimistic rollup](https://medium.com/molochdao/the-state-of-optimistic-rollup-8ade537a2d0f)
- Celer working on optimistic rollup using its [State Guardian Network as block producer](https://medium.com/celer-network/adding-hybrid-pos-rollup-sidechain-to-celers-coherent-layer-2-platform-d1d3067fe593)
- [Replay protection](https://ethresear.ch/t/zkrollup-optimistic-rollup-replay-protection/6999) in rollups by including networkID
- Cheaper zkrollups by using [generic snark circuits for state maintenance](https://ethresear.ch/t/zk-merklewitnessandsigrollup-a-generic-snark-circuit-for-stateless-contracts/7011)
- [Channelizing an Eth app](https://medium.com/statechannels/channelizing-an-ethereum-application-7656b76b91aa) using an API

**Stuff for developers**

- [dEth node](https://github.com/ethereum-ts/deth): claims to be 60% faster than Ganache
- [Security considerations around flash loan patterns](https://forum.openzeppelin.com/t/introduction-to-the-flash-loan-pattern-and-its-security-considerations/2331)
- Austin Griffith [video on flash loans](https://www.youtube.com/watch?v=VkXmhCUnInI)
- [Patterns for computing/accumulating interest](https://forum.openzeppelin.com/t/computing-and-accumulating-interest-on-chain-common-patterns-and-their-properties/2332)
- [Samczsun and Mudit Gupta find Nexus Mutual bugs](https://medium.com/nexus-mutual/responsible-vulnerability-disclosure-ece3fe3bcefa)
- [Email notifications](https://blog.embarklabs.io/news/2020/02/17/decentralized-notifications/) in dapps
- Solidity [unit testing using Remix tests, part 2](https://medium.com/remix-ide/solidity-unit-testing-using-remix-tests-part-2-50a9f486ab5d)
- Loredana’s [ChainLens contract searcher](https://twitter.com/lorecirstea/status/1231901527423541249) is available as a Remix plugin
- A video [intro to studio.ethereum.org IDE](https://www.youtube.com/watch?v=-tjk0yIIaIM)
- [Revert comments in Brownie](https://medium.com/coinmonks/effective-smart-contract-testing-developer-revert-comments-c7a6f250df0f)
- Embark [v5.2](https://blog.embarklabs.io/news/2020/02/19/embark-5-2-release/) - proxy contract support and scripts execution
- Math in Solidity series: [Numbers](https://medium.com/coinmonks/math-in-solidity-part-1-numbers-384c8377f26d) and [Overflow](https://medium.com/coinmonks/math-in-solidity-part-2-overflow-3cd7283714b4)
- [Realtime websocket integrations](https://medium.com/blockvigil/blockvigil-developer-updates-kicking-off-2020-with-websocket-integrations-for-ethereum-de38cd145656) via API, aimed at devs new to Eth
- [composable Airscript](https://ethresear.ch/t/composable-airscript/6984) v0.7
- [Eth2 things you can hack on](https://notes.ethereum.org/@djrtwo/ethdenver-bounties) at hackathons

**Ecosystem**

- Ethereum Foundation’s [wishlist for ecosystem support](https://ecosystem.support/wishlist/)
- [EthDenver finalists](https://medium.com/ethdenver/the-ethdenver-2020-finalists-buffidao-bounty-winners-627fd1b2427a)
- Waku [spec v0.4](https://specs.vac.dev/specs/waku/waku.html)
- Last week I mentioned [annotated versions of Week in Ethereum News](https://www.evanvanness.com/post/190777321891/annotated-edition-for-week-in-ethereum-news-feb-9) and then…got too busy to do one. It’ll happen this week.
- Register a .kred DNS domain, get [NFT that controls ENS and DNS records](https://medium.com/the-ethereum-name-service/ens-kred-major-integration-of-dns-and-ens-launches-e7efb4dd872a)
- Etherscan’s [2019 year in review charts](https://medium.com/etherscan-blog/ethereum-in-2019-through-the-lens-of-a-block-explorer-b67836611b0f)

**Enterprise**

- 4 key things [PegaSys Orchestrate fixes for enterprise blockchains](https://pegasys.tech/how-pegasys-orchestrate-solves-4-key-security-challenges-for-enterprise-blockchain-solutions/)
- Using Eth mainnet, [CargoX approved as bill of lading provider](https://cargox.io/press-releases/full/cargox-becomes-first-public-blockchain-ethereum-bill-lading-provider-approved-international-group-pi-clubs/) by shipping reinsurers
- [Utility Settlement Coin to work with Adhara](https://www.coindesk.com/secretive-digital-fiat-project-emerges-with-new-partner-as-cbdc-chatter-grows) on commercial bank money as alternative to central bank digital currencies

**Governance, DAOs, and standards**

- [Submit your startup to TheLAO](https://medium.com/@thelaoofficial/become-a-project-funded-by-the-lao-333e03cf5c) for funding
- [MolochDAOs on Aragon](https://1hive.org/getting-started-with-dandelion-organizations/) (Dandelion orgs) are live on mainnet
- ProgPoW returned as a debate topic this week, as core devs scheduled a separate hard fork for just ProgPoW. Meanwhile my Twitter feed is decidedly against ProgPoW, eg [here](https://twitter.com/econoar/status/1231684013795897345)
- [ERC2520](https://github.com/ethereum/EIPs/blob/77b8126032c17a9f6376243e434caf903354d2a7/EIPS/eip-draft_multiple_contenthash_records.md): Multiple contenthash records for ENS
- [ERC2525](https://github.com/ethereum/EIPs/blob/e1a75610c1e89b61549a1cab768b71264c29cb50/EIPS/eip-2525.md): ENS login

**bZx hacks**

- bZx hack using flashloans was the topic of the week after two attacks, here is bZx’s [post-mortem of the first attack](https://bzx.network/blog/postmortem-ethdenver). Meanwhile here is [Peckshield’s analysis](https://medium.com/@peckshield/bzx-hack-full-disclosure-with-detailed-profit-analysis-e6b1fa9b18fc): within one transaction, get a 10k eth flash loan from dydx, use as collateral on Compound to borrow wBTC, shorts on bZx which uses Kyber’s liquidity and inflates the price, sell the wBTC at that inflated price, repay the 10k flashloan for ~1300 ETH profit
- Here’s [that analysis in graphic form](https://twitter.com/kermankohli/status/1228817561220812800) from Kerman Kohli
- Check out the [transaction in Tenderly](https://dashboard.tenderly.dev/tx/main/0x762881b07feb63c436dee38edd4ff1f7a74c33091e534af56c9f7d49b5ecac15)
- Peckshield’s [analysis of the second hack](https://medium.com/@peckshield/bzx-hack-ii-full-disclosure-with-detailed-profit-analysis-8126eecc1360), netting ~2400 ETH
- [Palkeo’s analysis](https://www.palkeo.com/en/projets/ethereum/bzx.html) of both hacks, with a little more code. The first hack had a price check get bypassed, whereas in the second hack the price checks functioned
- 1inch says they found a [bZx bug months ago](https://medium.com/@1inch.exchange/yes-we-hacked-bzx-fulcrum-but-one-month-ago-3f7e5c437ee3) and apparently did not get paid for it
- Nexus Mutual [pays out the first claims for smart contract cover](https://medium.com/nexus-mutual/bzx-flash-loan-event-55753d19e52b) for bZx

**Application layer**

- [Decentraland’s Metaverse launches](https://decentraland.org/blog/announcements/decentraland-launch/), build on your land in a GUI or by SDK, as well as a marketplace, and a DAO that governs it all
- [Enjin Platform to create and manage game assets](https://blog.enjin.io/enjin-blockchain-game-development-platform-ethereum/) is live on mainnet
- Compound hits [200m in assets](https://twitter.com/rleshner/status/1229857396480040961)
- Melon as [asset management automator](https://medium.com/melonprotocol/automating-asset-management-protocol-8ff400c4f86b)
- Synthetix’s [Achernar release is live](https://blog.synthetix.io/the-achernar-release/), adding ETH as collateral
- the [tech stack for Status v1](https://our.status.im/the-status-mobile-app-technology-stack/)
- [1x.ag](https://twitter.com/k06a/status/1229125745282297857) - an automated leverage aggregator
- [Uniflash](https://github.com/uniflash/uniflash): a decentralized flash loans protocol, live on Goerli testnet. [Remco Bloemen](https://twitter.com/recmo/status/1229171153597386752), [Austin Williams](https://twitter.com/onewayfunction/status/1230689638076973058) and [Stephane Gosselin](https://twitter.com/thegostep/status/1230320671009333250) also have some flashmint contracts out there
- Dharma now has [fee-free debit card fiat<>Dai](https://blog.dharma.io/dharma-deposits-are-now-fee-free) deposits and withdrawals
- [Maker changes](https://vote.makerdao.com/executive-proposal/activate-the-dai-debt-ceiling-adjustment-set-dai-savings-rate-spread-set-sai-stability-fee-lower-surplus-auction-bid-set-governance-delay-module): activates 24 hour time delay on any governance changes, DSR spread to 0, Dai ceiling to 150m

**Tokens/Business/Regulation**

- [Enigma settles with SEC](https://www.sec.gov/news/press-release/2020-37) for unregistered securities offering
- [Personal gratitude tokens](https://blog.simondlr.com/posts/personal-tokens-2020-social-reputation): social money (or “challenge coins”) issued on a bonding curve
- Forking Gardens: [conditional tokens can change gaming](https://blog.gnosis.pm/tokens-gaming-and-forking-gardens-2681b1b76f15)

**General**

- Break RSA assumptions: [bounties for solving the adaptive root problem](https://rsa.cash/bounty-instances)
- More [PLONK benchmarks](https://medium.com/aztec-protocol/plonk-benchmarks-ii-5x-faster-than-groth16-on-pedersen-hashes-ea5285353db0): 5x faster than Groth16 on Pedersen Hashes
- [Trustless Groups of Unknown Order](https://eprint.iacr.org/2020/196.pdf) with Hyperelliptic Curve
- Barry Whitehat zk ideas: [private social network search](https://ethresear.ch/t/blind-find-private-social-network-search/6988) and [private order matching](https://ethresear.ch/t/peekabook-private-order-matching/6987)
- [WebAssembly/eWASM explainer](https://blog.embarklabs.io/news/2020/02/24/wasm-ewasm-what-and-why/)
- How [Nym improves on traditional mixnets](https://medium.com/nymtech/how-nym-improves-on-traditional-mixnet-designs-219cd36724a0)
- Andreas’ [Mastering Ethereum is looking for translations](https://twitter.com/aantonop/status/1230545400458817541); uses Creative Commons license

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- **Edcon and EthParis cancelled**
- Feb 28-Mar 1 - [ETHLondon UK](https://ethlondon.com/)
- Mar 3-5 - [EthCC](https://ethcc.io/) (Paris)
- **Mar 14 - [Augur v1 cutoff](https://github.com/AugurProject/augur-app/releases/tag/v1.16.9)**
- Mar 29-Apr4 - [EthLagos](https://ethlagos.io/)
- Apr 13 - Deadline to apply for [50k euro for blockchain startup](https://blockchers.eu/open-calls/)s in Europe
- Apr 24-26 - [EthTurin](https://ethturin.com/)
- **Apr 29-30 - [SoliditySummit](https://solidity-summit.ethereum.org/) (Berlin)**
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

Issue permalink: [https://weekinethereumnews.com/week-in-ethereum-news-february-23-2020/](https://weekinethereumnews.com/week-in-ethereum-news-february-23-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

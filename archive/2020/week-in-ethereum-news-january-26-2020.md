---
title: "Week in Ethereum News <BR> January 26, 2020"
date: "2020-01-26"
---

## **Eth News and Links**

**Eth1**

- Latest [core devs call](https://youtu.be/0-Vld7GTRhQ?t=446). Tim’s [notes](https://twitter.com/TimBeiko/status/1220703467536252937): lots of ungas talk
- Geth [v1.9.10](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.10) - light client checkpoint oracle, higher propagated transaction cap, bug fixes
- [Multiaddr, ENR and enodes](https://dean.eigenmann.me/blog/2020/01/21/network-addresses-in-ethereum/): network addresses explainer

**Eth2**

- Latest [what’s new in eth2](https://notes.ethereum.org/@ChihChengLiang/Sk8Zs--CQ/Sk8Zs--CQ?type=book)
- Latest [Eth2 call](https://www.youtube.com/watch?v=kt59-FEeWTI). Notes from [Mamy](https://gist.github.com/mratsim/e493503c3b1e7f1b7de448671b72859f) and [Ben](https://hackmd.io/@benjaminion/Bk9BW7PZI)
- Hsiao-Wei: [Attestation aggregation in Eth2](https://notes.ethereum.org/@hww/aggregation)
- Attestant: [understanding the validator lifecycle](https://www.attestant.io/posts/understanding-the-validator-lifecycle/)
- Runtime Verification [formally verified the eth2 deposit contract](https://runtimeverification.com/blog/end-to-end-formal-verification-of-ethereum-2-0-deposit-smart-contract/)
- [eth2stats](https://eth2stats.io)

**Layer2**

- Fuel’s [testnet is in open beta](https://medium.com/@fuellabs/announcing-the-fuel-v0-open-beta-565a2d340fc3), fraud proofs under 1m gas. Using colored coins (!)
- Miner [challenges Arbitrum is dealing with](https://medium.com/offchainlabs/fighting-censorship-attacks-on-smart-contracts-c026a7c0ff02)
- How Loopring aims to [make its zk rollup transactions composable](https://medium.com/loopring-protocol/composability-between-ethereum-layer-1-and-2-10650b7411e5) on layer1
- Jordi Baylina’s [Iden3 zk rollup slides](https://ipfs.io/ipfs/QmUHpp1nkFFeT3eodJHj9V9xWyhnwEpenxHAGYgB7Lzjgw)

**Stuff for developers**

- [Better Solidity debugging](https://medium.com/nomic-labs-blog/better-solidity-debugging-console-log-is-finally-here-fc66c54f2c4a): console.log and stack traces
- [ABDK’s online tools](https://toolkit.abdk.consulting/ethereum): key of an address, calculate address pre-deploy, RLP encoder/decoder, encode/decode raw signed/unsigned transactions
- [Securify v2](https://medium.com/chainsecurity/release-of-securify-v2-0-6304a40034f), free security scanner
- [Auditing your code with Web3j](https://blog.web3labs.com/auditing-smart-contracts-with-web3j) and its EVM
- [Sam Sun caught a vulnerability in Curve](https://blog.curve.fi/vulnerability-disclosure/), which was solved by moving front end to a fixed version.
- What are [Burner Wallet Plugins](https://medium.com/@dmihal/what-are-burner-wallet-plugins-5c497e4bd279)? Customizing your popup event/economy
- How to [run your own xDai chain with arbitrary message bridge](https://twitter.com/barinov/status/1220040934357860352)
- web3connect [v1beta.26](https://github.com/web3connect/web3connect/releases/tag/1.0.0-beta.26) - a single web3 provider for all wallets
- [What does Truffle and WalletConnect mean](https://medium.com/@sergiibomko/what-does-truffle-walletconnect-mean-861e4fd8b9f8)?
- a [lightweight directory access protocol](https://www.reddit.com/r/ethereum/comments/eqvz29/happy_to_release_aka_protocol_ldap_for_ethereum/)
- [Using CREATE2](https://hackernoon.com/using-ethereums-create2-nw2137q7) explainer
- [Smart contracts](https://twitter.com/austingriffith/status/1220745805880905730) on Austin Griffith’s eth.build
- [AirScript v0.6 and genSTARK v0.7](https://ethresear.ch/t/airassembly-a-low-level-language-for-zk-starks/6419/5) AirScript compiles to AirAssembly, which genSTARK uses to create a STARK

**Ecosystem**

- [Year in Ethereum 2019](https://medium.com/@jjmstark/the-year-in-ethereum-2019-242012e4276d) by Josh Stark and I
- [Scalability estimates for Waku](https://discuss.status.im/t/scalability-estimate-how-many-users-can-waku-and-the-status-app-support/1514) (Status’s Whisper alternative)
- A [style guide for ethereum.org](https://www.figma.com/file/rQK2dt9eaLOMmvTOf5ifdr/Ethereum.org-Style-Guide-(RC1)?node-id=602%3A1)

**Enterprise**

- Key factors in [choosing between Clique, Raft, and IBFT](https://pegasys.tech/key-factors-to-consider-when-choosing-a-blockchain-consensus-protocol/) for private chains
- Commodity giants consortium (Cargill, ADM, Glencore, Bunge, Dreyfus) chooses [Quorum, Orchestrate and Kaleido](https://consensys.net/blog/press-release/covantis-initiative-announces-technology-partner-consensys/) for their tech stack

**Governance and standards**

- [EIP2315](https://github.com/ethereum/EIPs/blob/457abdf1555bba27a5ca0c3a99b79ea75b83febb/EIPS/eip-2315.md): JUMPSUB and RETSUB for simple EVM subroutines
- [EIP2489](https://github.com/ethereum/EIPs/blob/b7aaabb95c79837ef0266504b30c14591a450e95/EIPS/eip-2489.md): deprecate GAS opcode
- [EIP2488](https://github.com/ethereum/EIPs/blob/213ea4237201a7cd5c6720e5c2b460f39f269281/EIPS/eip-2488.md): deprecate CALLCODE opcode
- [ERC2477](https://github.com/ethereum/EIPs/blob/2db9d4603612c78b51d23624e706fc970aa7f6ad/EIPS/eip-2477.md): NFT metadata integrity
- The [DigixDAO voted for dissolution](https://www.reddit.com/r/ethfinance/comments/ercat5/the_digixdao_dissolution_proposal_has_passed_with/). [TheLAO wants a DigixLAO](https://medium.com/@thelaoofficial/the-evolution-of-daos-to-laos-the-case-for-the-digix-lao-b2ec1013f7a6)
- [Social choice theory and voting on multiple outcomes](https://blog.kleros.io/kleros-and-social-choice-theory-voting/)
- What to expect when [summoning a MolochDAO](https://medium.com/totle/summoner-101-expectations-of-launching-your-own-moloch-dao-d6bb0fbbe600)
- [SignalDAO](https://medium.com/abridged-io/signal-dao-and-the-burgeoning-field-of-dao-ops-b767ece3e8c0), a signalling DAO for Metacartel/MolochDAO using a Telegram bot doing web3 calls via Abridged SDK

**Application layer**

- [Set Social Trading](https://medium.com/set-protocol/set-social-trading-is-now-live-on-tokensets-c981b5e67c5f) is live on mainnet. Automatically copy what your favorite trader is doing.
- a [URL shortener](https://www.reddit.com/r/ethereum/comments/esj4xe/url_shortener_built_on_ethereum_ens_ipfs_redireth/) using ENS + the lightweight director access protocol referenced above in dev tools
- How people are [using Pepo, crypto’s TikTok](https://medium.com/the-pepo-app/6-compelling-ways-people-are-using-pepo-for-mainstream-use-cases-ae480992cc37)
- [Ethernal](https://medium.com/@EthernalWorld/dungeon-crawler-32f693732a24): a text-based MUD. die and you lose your items!
- There’s now over [100 million Dai](https://twitter.com/MakerDAO/status/1220010151383457792)
- [Rocket](https://medium.com/@AlexMasmej/introducing-rocket-get-a-loan-against-your-nfts-f67b1b5738f0): get a loan against your NFTs, live on Ropsten testnet
- [Rho](https://twitter.com/maxcwolff/status/1220410979873325059): a spec for a float to fixed automated market maker swap protocol
- Synthetix: the [state of Synthetix](https://blog.synthetix.io/the-state-of-synthetix/) and [2020 roadmap](https://blog.synthetix.io/2020-roadmap) adding ETH as collateral

**Tokens/Business/Regulation**

- Davos was this week, so WEF issued a framework for [Central Bank digital currencies in the age of blockchain](https://www.weforum.org/projects/central-banks-age-of-blockchain)
- An onchain [NFT for accredited investors](https://twitter.com/lex_DAO/status/1219769643012886529)
- POAP event NFTs as a [sybil-resistant identity layer](https://medium.com/@poap/poap-retrospective-of-2019-b5b2181e054e)
- Tokenized real estate: [purchase to settlement in 15 minutes](https://medium.com/realtplatform/breaking-records-via-tokenization-round-2-6dcba37820b5) with RealT

**General**

- [How not to critique Ethereum](https://blog.theabacus.io/how-not-to-critique-ethereum-11b542b08206): a guide for Bitcoiners
- A curated [list of blockchain research papers](https://twitter.com/nrryuya/status/1219640438853984256)
- Benchmarking [Brave vs Chrome/Firefox/Opera](https://brave.com/brave-one-dot-zero-performance-methodology-and-results/) for speed and battery use
- Chris Dixon: blockchains are [computers that make commitments](https://cdixon.org/2020/01/26/computers-that-can-make-commitments)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Jan 31 - deadline for [EU ledger 200k euro grants](https://fundingbox.com/spaces/ledger-ledger-news-and-updates/5dbfcb7d52317832f85906c8) for blockchain startups
- Feb 8 - [Augur v1 cutoff](https://twitter.com/AugurProject/status/1214545983205494784)
- Feb 14-16 - [ETHDenver](https://www.ethdenver.com/)
- Feb 20 - [Decentraland launch](https://decentraland.org/blog/announcements/decentraland-announces-publich-launch/)
- Feb 28-Mar 1 - [ETHLondon UK](https://ethlondon.com/)
- Mar 3-5 - [EthCC](https://ethcc.io/) (Paris)
- Mar 29-Apr4 - [EthLagos](https://ethlagos.io/)
- Apr 3-7 - [Edcon](https://www.edcon.io/) (Vienna)
- April 24-26 - [EthTurin](https://ethturin.com/)
- **May 8-9 - [Ethereal Summit](https://www.etherealsummit.com/) (NYC)**
- May 15 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum News. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

It’s amazing to me how many people email me when every issue has a link at the bottom saying not to email me to get in the newsletter.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **I want your links, because Google needs help: [weekinethereumnews.com](https://weekinethereumnews.com/)**

Archive on the web if you’re linking to it:  [https://weekinethereumnews.com/week-in-ethereum-news-january-26-2020/](https://weekinethereumnews.com/week-in-ethereum-news-january-26-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

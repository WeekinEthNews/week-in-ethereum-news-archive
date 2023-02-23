---
title: "Week in Ethereum News <BR> January 12, 2020"
date: "2020-01-12"
---

## **Eth News and Links**

**Eth1**

- Latest [core devs call](https://youtu.be/snEdgekxJto). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1215631141975265285), discussion of EIPs 2456, 1962, 2348
- EthereumJS [v4.13](https://www.reddit.com/r/ethereum/comments/emmayz/ethereumjs_release_v413_muirglacier_bugfix_fixed/) - bugfix release for Muir Glacier
- Slockit released a stable version of their [Incubed](https://blog.slock.it/incubed-stable-release-c35b3a4ec10a) stateless ultralight client, aimed at IoT devices. 150kb to verify transactions or 500kb including EVM. incentive layer coming soon.

**Eth2**

- Latest [Eth2 implementer call](https://www.youtube.com/watch?v=u2w4EO9YepI). Notes from [Mamy](https://gist.github.com/mratsim/0f742236da1e5dbb6ca97b8fb55f061b) and from [Ben](https://hackmd.io/@benjaminion/ByYThFEgI).
- Latest [what’s new in Eth2](https://notes.ethereum.org/@ChihChengLiang/Sk8Zs--CQ/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200110?type=book)
- Spec version [v0.10](https://github.com/ethereum/eth2.0-specs/releases/tag/v0.10.0) with BLS standards
- Prysmatic [restarted its testnet](https://medium.com/prysmatic-labs/prysm-testnet-v0-9-3-release-info-fa0b77161a41) with a newer version of the spec and mainnet config
- [Lodestar](https://medium.com/chainsafe-systems/lodestar-grants-update-74452199dfa8?) update on light clients and dev tooling
- 3 [options for state providers](https://ethresear.ch/t/state-provider-models-in-ethereum-2-0/6750)
- [Eth2 for Dummies](https://medium.com/@chromaticcapital/eth2-for-dummies-11ff9b11509f)
- Exploring [validator costs](https://www.attestant.io/posts/exploring-ethereum-2-validator-costs/)

**Layer2**

- Optimistic rollup for tokens [Fuel ships first public testnet](https://twitter.com/fuellabs_/status/1215366571125878785)
- [Optimistic Game Semantics](https://plasma.group/optimistic-game-semantics.pdf) for a generalized layer2 client
- Loopring presents [full results of their zk rollup testing](https://medium.com/loopring-protocol/loopring-testing-phase-1-data-recap-ed0c67396870)
- [StarkEx says they can do 9000 trades per second](https://twitter.com/starkwareltd/status/1214236179551412232?s=21) at 75 gas per trade with offchain data, with the limiting factor being the prover, not onchain throughput.

**Stuff for developers**

- An [update on the Vyper compiler](https://blog.ethereum.org/2020/01/08/update-on-the-vyper-compiler/): there’s now two efforts, a new one in Rust using YUL to target both EVM & ewasm as well as the existing one in Python.
- A look at [vulnerabilities of deployed code over time](https://medium.com/@alethioEthstats/the-security-series-a-look-at-ethereums-smart-contracts-4f096f48f2b)
- a beginner’s [guide to the K framework](https://medium.com/@giulio.rebuffo/formal-verification-why-and-how-a104cd702c25)
- Vulnerability: [hash collisions with multiple variable length arguments](https://medium.com/swlh/new-smart-contract-weakness-hash--with-multiple-variable-length-arguments-dc7b9c84e493)
- [Verifying wasm transactions](https://medium.com/dlabvc/verifying-wasm-functions-part-1-ea524c04c094) (and [part2](https://medium.com/dlabvc/verifying-wasm-functions-part-2-i64-reverse-bytes-3590aedaa3c0))
- Austin Griffith’s [eth.build metatransactions](https://twitter.com/austingriffith/status/1215674830671843328)
- Build your own [customized Burner Wallet](https://medium.com/@dmihal/build-your-own-customized-burner-wallet-without-the-burner-factory-dfbe598cdada)
- [Abridged v2](https://medium.com/abridged-io/abridged-2020-83a4e917c645) aiming to make it easy to onboard new users of web2 networks
- Ethcode [v0.9](https://medium.com/quanta-network/ethcode-v0-0-9-beginning-the-20s-7be98a0b2a01) VSCode extension
- [Embark v5](https://github.com/embark-framework/embark/releases/tag/v5.0.0)

**Ecosystem**

- RicMoo: [SQRLing mnemonic phrases](https://blog.ricmoo.com/sqrl-ing-mnemonic-phrases-b68b2dc1f75b)
- [ethsear.ch](https://twitter.com/JonnyRhea/status/1215291699959926785) - Ethereum specific search engine
- Avado’s [RYO node](https://twitter.com/Avado_DServer/status/1215206214562349056) - nodes opt-in and let users access them via load balancer
- [30 days of Eth ecosystem shipping](https://concourseopen.com/blog/30-days-of-eth-december-2019/)
- Aztec’s BN-254 [trusted setup ceremony post-mortem](https://medium.com/aztec-protocol/aztec-crs-the-biggest-mpc-setup-in-history-has-successfully-finished-74c6909cd0c4). Confidential transactions launching this month

**Enterprise**

- [700m USD volume on Komgo](https://consensys.net/blog/enterprise-blockchain/komgos-blockchain-trade-finance-platform-january-2020-updates/) commodity trade finance platform
- TraSeable [seafood tracker article on the challenges](https://www.seafoodsource.com/news/environment-sustainability/traseable-s-blockchain-based-traceability-technology-overcomes-challenges-in-the-pacific) points out the troubles with no private chain interoperability
- [Caterpillar](https://github.com/orlenyslp/Caterpillar) business process management system
- [Q&A with Marley Gray](https://www.intelalley.com/cryptocurrency/taxonomy-qa-marley-gray-tti-part-i/) about the EEA’s Token Taxonomy Initiative

**Governance and standards**

- [EIP1559 implementation](https://ethereum-magicians.org/t/eip-1559-go-etheruem-implementation/3918) discussion
- [EIP2456](https://github.com/ethereum/EIPs/blob/d771a0d82de6975bdd0b395b35fa6675fcb0fade/EIPS/eip-2456.md): Time based upgrades
- Metamask’s bounty for a [generalized metatransaction standard](https://medium.com/metamask/announcing-a-generalized-metatransaction-contest-abd4f321470b)

**Application layer**

- [Flashloans within one transaction using Aave Protocol](https://medium.com/aave/pop-the-champagne-aave-protocol-is-live-721731763b58) are live on mainnet
- Orchid’s [decentralized VPN launches](https://blog.orchid.com/orchids-privacy-network-launches/)
- Data viz on [dexes in 2019](https://medium.com/alethio/dex-in-the-2019-a-recap-by-numbers-96d506ba1cb8)
- [ZRXPortal](https://blog.0xproject.com/introducing-zrx-portal-b529aec1a0a9) for ZRX holders to delegate their tokens to stakers
- Dai Stability Fee and Dai Savings Rate [go up to 6%](https://twitter.com/MakerDaiBot/status/1214857420964552704), while Sai Stability Fee at 5%
- EthHub’s [new Ethereum user guides](https://twitter.com/econoar/status/1215725972856561664)

**Tokens/Business/Regulation**

- David Hoffman: the [money game landscape](https://medium.com/@TrustlessState/ethereum-the-money-game-landscape-1b9fdb05f842)
- Australia [experimenting with a digital Aussie dollar](https://www.rba.gov.au/publications/submissions/payments-system/pdf/financial-and-regulatory-technology.pdf), with a prototype on a private Ethereum chain
- 3 [cryptocurrency regulation themes](https://www.forbes.com/sites/brianbrooks/2020/01/07/three-cryptocurrency-regulation-themes-for-2020--and-the-flawed-premises-behind-them/#4f037c0c63e3) for 2020
- OpenSea’s [compendium of NFT knowledge](https://opensea.io/blog/guides/non-fungible-tokens/)
- A newsletter to keep track of the [NFT space](https://andrewsteinwold.substack.com/p/nft-proof-of-work-jan-2020)
- [Initial Sardine Coin Offering](https://www.forbes.com/sites/francescoppola/2020/01/10/crypto-and-sardines-combine-to-create-an-investment-opportunity/#18f5069673c2)
- NBA guard [Spencer Dinwiddie’s tokenized contract](https://twitter.com/sdinwiddie_25/status/1215640393204871168?s=21) launches January 13
- [Progressive decentralization](https://a16z.com/2020/01/09/progressive-decentralization-crypto-product-management/): a dapp business plan

**General**

- Andrew Keys: [20 blockchain predictions for 2020](https://consensys.net/blog/news/andrew-keys-20-blockchain-predictions-for-2020)
- Haseeb Qureshi’s [intro to cryptocurrency class](https://nakamoto.com/introduction-to-cryptocurrency/) for programmers
- Ben Edgington’s [BLS12-381 for the rest of us](https://hackmd.io/@benjaminion/bls12-381)
- [Visualizing efficient Merkle trees](https://kndrck.co/posts/efficient-merkletrees-zk-proofs/) for zero knowledge proofs
- Eli Ben-Sasson’s catalog of the [Cambrian zero knowledge explosion](https://nakamoto.com/cambrian-explosion-of-crypto-proofs/)
- Bounty for [breaking RSA assumptions](https://rsa.cash/)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- **Jan 20-21 - Parity’s [OpenEthereum Rust client](https://www.eventbrite.com/e/openethereum-workshop-tickets-88507864405) workshop (Berlin)**
- Jan 21 - [Gitcoin grants](https://gitcoin.co/blog/gitcoin-grants-2020/) quadratic matching ends. **(my grant is [here](https://gitcoin.co/grants/237/week-in-ethereum-news)!)**
- Jan 31 - deadline for [EU ledger 200k euro grants](https://fundingbox.com/spaces/ledger-ledger-news-and-updates/5dbfcb7d52317832f85906c8) for blockchain startups
- **Feb 8 - [Augur v1 cutoff](https://twitter.com/AugurProject/status/1214545983205494784)**
- Feb 14-16 - [ETHDenver](https://www.ethdenver.com/)
- Feb 28-Mar 1 - [ETHLondon UK](https://ethlondon.com/)
- Mar 3-5 - [EthCC](https://ethcc.io/) (Paris)
- Mar 29-Apr4 - [EthLagos](https://ethlagos.io/)
- Apr 3-7 - [Edcon](https://www.edcon.io/) (Vienna)
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

Archive on the web if you’re linking to it:  [https://weekinethereumnews.com/week-in-ethereum-news-january-12-2020/](https://weekinethereumnews.com/week-in-ethereum-news-january-12-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

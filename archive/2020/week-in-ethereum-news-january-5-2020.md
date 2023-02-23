---
title: "Week in Ethereum News <BR> January 5, 2020"
date: "2020-01-05"
---

## **Eth News and Links**

**Eth1**

- Muir Glacier successfully hardforked on Jan 2nd.
- Nethermind [v1.4.2](https://github.com/NethermindEth/nethermind/releases/tag/1.4.2) - proper config file for Muir Glacier
- Update Parity clients to [v2.6.8beta](https://github.com/paritytech/parity-ethereum/releases/tag/v2.6.8) and [v2.5.13stable](https://github.com/paritytech/parity-ethereum/releases/tag/v2.5.13). An attacker found that Parity was only validating block header and so was crashing Parity nodes by sending valid header with invalid body
- An overview of [stateless Ethereum](https://blog.ethereum.org/2019/12/30/eth1x-files-state-of-stateless-ethereum/)
- [Protocol changes necessary for 4MB witness size](https://ethereum-magicians.org/t/protocol-changes-to-bound-witness-size/3885): binary tree, 3 gas per byte for calling contracts, gas costs go up for SLOAD to 2000. EXTCODESIZE, BALANCE, and \*CALL go up to 2400
- Data on [witness size using binary tries](https://medium.com/@mandrigin/stateless-ethereum-binary-tries-experiment-b2c035497768)

**Eth2**

- Simpler Eth2 [meta execution environment](https://ethresear.ch/t/an-even-simpler-meta-execution-environment-for-eth/6704)
- SigmaPrime’s update on [Beacon Fuzz](https://blog.sigmaprime.io/beacon-fuzz-01.html), their Eth2 client differential fuzzer
- Jim McDonald’s [Eth2 expectations for 2020](https://www.attestant.io/posts/anticipating-ethereum-2-in-2020/)

**Stuff for developers**

- Solidity [v0.6.1](https://github.com/ethereum/solidity/releases/tag/v0.6.1) and [v0.5.16](https://github.com/ethereum/solidity/releases/tag/v0.5.16) - Yul optimizer bugfix
- [Compiling Formality to the EVM](https://medium.com/@maiavictor/compiling-formality-to-the-evm-99aec75677dd). Run formally verified functional programs on the EVM
- [IPLD tutorial](https://simpleaswater.com/hands-on-ipld-tutorial-in-golang/) in Go
- Running [machine learning models in ewasm](https://github.com/jrhea/anomlee)
- Nethereum [v3.5](https://github.com/Nethereum/Nethereum/releases/tag/3.5.0)
- What’s new in [Microsoft’s Ethereum VSCode extension](https://twitter.com/Windozer/status/1212015084475731968) update

**Ecosystem**

- Best practices to stay [anonymous using Tornado.cash and other mixers](https://medium.com/@tornado.cash/how-to-stay-anonymous-with-tornado-cash-and-similar-solutions-efdecdbd7d37) and the Tornado UI is now available via IPFS and ENS [https://tornadocash.eth.link](https://tornadocash.eth.link)
- [Credible neutrality as Vitalik’s design principle](https://nakamoto.com/credible-neutrality/), written for the recently launched Nakamoto.com

**Enterprise**

- UN Secretary General says his [institution must embrace blockchain](https://www.forbes.com/sites/michaeldelcastillo/2019/12/28/secretary-general-says-united-nations-must-embrace-blockchain/#4ab7b4301379)
- UN pilot to [track cashmere supply chain](https://www.forbes.com/sites/rogerhuang/2019/12/28/un-pilot-in-mongolia-uses-blockchain-to-help-farmers-deliver-sustainable-cashmere/#18990bf617d9)

**Governance**

- How the “year of the DAO” became the [“year of the MolochDAO”](https://medium.com/@molochdao/moloch-2019-year-in-review-eb6f53dc035)
- Maker Foundation [transfers trademarks and software IP](https://blog.makerdao.com/the-maker-foundation-transfers-trademarks-and-software-ip-to-independent-dai-foundation/) to the Dai Foundation
- [Vocdoni architecting](https://blog.vocdoni.io/vocdoni-reimagining-governance/) for private, transmission-agnostic, open to quadratic voting/futarchy/etc

**Application layer**

- Missed this until now: [BULVRD](https://bulvrdapp.com/) app, trying to compete with Waze
- [Undercollateralized loans](https://medium.com/fabrx-blockchain/meet-zero-collateral-dcfe27fb3a2d) live on Ropsten testnet
- [Lock, vest, or schedule payouts](https://medium.com/lockprotocol/lock-protocol-use-cases-b24891c9ea7d) with Lock Protocol
- Lower your counterparty risk in trading Counterstrike: Go skins: [Sugarskins](https://twitter.com/ChainLinkGod/status/1212108331210272769?s=19)
- [Uniswap average daily volume up 6000%](https://twitter.com/uniswapexchange/status/1212092582223896578?s=21) in 2019
- Provide [Uniswap liquidity while maintaining ETH exposure](https://twitter.com/NodarJ/status/1213507574215200769) (understand the risks before you do it)
- UEFA tokenizing [20,000 VIP tickets for Euro2020](https://medium.com/alphawallet/uefas-exclusive-sales-agent-partners-with-alphawallet-for-blockchain-ticket-solution-49ab4fab1514) with AlphaWallet

**General**

- Financial Times: [DeFi promises high interest and no middlemen](https://archive.md/Bo5kM)
- Linda Xie’s [beginner’s guide to DeFi](https://nakamoto.com/beginners-guide-to-defi/)
- Nikolai [donated 3200 MKR to Carnegie Mellon](https://nikolai.fyi/cmu-donation) for game theory research in decentralized applications
- A look back at 2019’s [major blockchain security incidents](https://medium.com/mycrypto/2019-in-review-major-blockchain-crypto-security-incidents-adb0e87e0f25). Meanwhile the [latest “giving away Eth scam” tactic](https://decrypt.co/15931/youtubers-are-being-hijacked-for-crypto-scams) is hacking a verified Youtuber and changing the account name to impersonate someone in crypto

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Jan 6-20 - Gitcoin [take back the web online hackathon](https://gitcoin.co/hackathon/take-back-the-web/?)
- Jan 6-21 - [Gitcoin grants](https://gitcoin.co/blog/gitcoin-grants-2020/) quadratic matching
- Jan 31 - deadline for [EU ledger 200k euro grants](https://fundingbox.com/spaces/ledger-ledger-news-and-updates/5dbfcb7d52317832f85906c8) for blockchain startups
- Feb 14-16 - [ETHDenver](https://www.ethdenver.com/)
- **Feb 28-Mar 1 - [ETHLondon](https://ethlondon.com/)**
- Mar 3-5 - [EthCC](https://ethcc.io/) (Paris)
- Mar 29-Apr4 - [EthLagos](https://ethlagos.io/)
- Apr 3-7 - [Edcon](https://www.edcon.io/) (Vienna)
- May 15 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum News. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

It’s amazing to me how many people email me when every issue has a link at the bottom saying not to email me to get in the newsletter.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **I want your links, because Google needs help: [weekinethereumnews.com](https://weekinethereumnews.com/)**

Archive on the web if you’re linking to it:  [https://weekinethereumnews.com/week-in-ethereum-news-january-5-2020/](https://weekinethereumnews.com/week-in-ethereum-news-january-5-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

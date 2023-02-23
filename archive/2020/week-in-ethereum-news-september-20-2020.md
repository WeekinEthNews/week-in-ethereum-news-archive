---
title: "Week in Ethereum News <BR> September 20, 2020"
date: "2020-09-20"
---

## **Eth News and Links**

**Eth1**

- Latest [core dev call](https://youtu.be/HUUxwyoxU7k?t=226). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1306956314187243527). Related: ignore any incorrect info; ProgPoW is still shelved.
- “[I believe that Ethereum 1 can scale at least 10x even without sharding](https://github.com/AlexeyAkhunov/papers/blob/master/Turbo-Geth-Silkworm.pdf)” using Turbogeth
- Latest [Turbogeth release](https://github.com/ledgerwatch/turbo-geth/releases/tag/v2020.09.03), more RPC calls, updated to latest geth
- [EVM384](https://notes.ethereum.org/@poemm/evm384-interface-update) fast crypto in the EVM instead of compiles exploration update
- EIP2938’s [account abstraction](https://hackmd.io/@SamWilsn/ryhxoGp4D) explainer with Solidity example

**EIPs/Standards**

- [EIP2970](https://eips.ethereum.org/EIPS/eip-2970): `IS_STATIC` opcode
- [EIP2976](https://eips.ethereum.org/EIPS/eip-2976): Typed Transactions over Gossip
- [ERC2980](https://github.com/ethereum/EIPs/blob/441df4e6d7ae30ba14b1224d4a3b56e7d5dd3587/EIPS/eip-2980.md): ERC20 compatible Swiss Compliant Asset Token
- [ERC2981](https://github.com/ethereum/EIPs/blob/8462c8ed660291881de0c3110b6a024136c3d90c/EIPS/eip-2981.md): ERC721 Royalty Standard
- [EIP2982](https://github.com/ethereum/EIPs/blob/5dc1b8ddd645af01c81da8817b6bcc8ff883b9d6/EIPS/eip-2982.md): eth2 phase 0

**Eth2**

- See immediately above for EIP2982, the spec for eth2 phase 0
- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200919)
- Latest [eth2 quick update](https://blog.ethereum.org/2020/09/14/eth2-quick-update-no-16/) - deposit contract/genesis dress rehearsal on Sept 29
- [eth2 spec v0.12.3](https://github.com/ethereum/eth2.0-specs/releases/tag/v0.12.3) - slashing and inactivity penalties reduced 67-75% for first few months of eth2 launch
- Latest [Eth2 call](https://www.reddit.com/r/ethereum/comments/iuj7je/live_ethereum_20_call_48_2020917_1400_gmt/). Notes from [Ben](https://hackmd.io/@benjaminion/BJIQuJZSD) and [Mamy](https://gist.github.com/mratsim/0bafb17499e6a33b69085ec21de7cd91).
- [formally verifying the blst BLS sig library](https://galois.com/blog/2020/09/announcing-the-blst-bls-verification-project/) that Eth2 uses
- [Provable single secret leader election](https://ethresear.ch/t/provable-single-secret-leader-election/7971) to obviate DoS attacks on block producer
- An imperfect look at [client diversity through POAP data](https://www.reddit.com/r/ethstaker/comments/ith0h1/medalla_client_poap_awards_broken_down_by_fair/)
- Latest [Lighthouse client](https://lighthouse.sigmaprime.io/update-29.html) update, GossipSub v1.1, improving attestation inclusion, fuzzing networking
- Latest [Lodestar client](https://medium.com/chainsafe-systems/lodestar-update-38f58c14a39d) update, fixing networking and block production
- Teku’s [client updates are its release notes](https://github.com/PegaSysEng/teku/releases/tag/0.12.6)

**Layer2**

- [POA transition to optimistic rollup VM](https://ethresear.ch/t/poa-transition-to-optimistic-rollup-vm/7983)
- Peter Kim’s [demo of USDC on Matic](https://twitter.com/petejkim/status/1306957817702526976)

* * *

### **This newsletter is made possible thanks to [Chainlink](https://chain.link/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/05/FE39n5_g-1.png)

Interested in oracles? Apply for a [Chainlink Community Grant](https://blog.chain.link/introducing-the-chainlink-community-grant-program/) to help improve the most widely used oracle on Ethereum. If you’re interested in building oracles, we’re also [hiring for our core team](https://www.chainlinklabs.com/careers). 

* * *

**Stuff for developers**

- [Underhanded Solidity Contest](https://underhanded.soliditylang.org/) is underway! Submissions due Oct 31
- web3js [v1.3](https://github.com/ethereum/web3.js/releases/tag/v1.3.0), built in typescript, upgraded websockets
- Truffle [v5.1.45](https://github.com/trufflesuite/truffle/releases/tag/v5.1.45), hdwallet-provider improvements
- create-eth-app [v1.5](https://github.com/PaulRBerg/create-eth-app/releases/tag/v1.5.0) with web3modal so you can easily use MetaMask or WalletConnect
- [ethers-rs adds Ledger](https://twitter.com/gakonst/status/1307748834387341312) support
- [EEA has a dev tool survey](https://twitter.com/EntEthAlliance/status/1307010896250667009) to find out areas to improve for enterprise dev tools
- [q&a video for devs new to Eth](https://www.youtube.com/watch?v=uCk9-KG9cJA), lots of dev tool talk
- Meet the [Solidity team](https://solidity.ethereum.org/2020/09/18/meet-the-team/)
- How [diamond storage works](https://dev.to/mudgen/how-diamond-storage-works-90e)
- How to [use permit for gasless transactions](https://hackernoon.com/how-to-code-gas-less-tokens-on-ethereum-43u3ew4)
- Early work on [Fe](https://github.com/ethereum/fe), a pythonic EVM language written in Rust
- [bZx hacked](https://bzx.network/blog/incident); used admin key to delete attacker’s gains

**Ecosystem**

- This week we hit all time high for [number of transactions in a day](https://etherscan.io/chart/tx)
- If gas fees went up and you don’t have enough eth to cover gas fees on your Dai transfer, try the [out of eth](https://www.anydot.dev/uniswap/#/swap) tool
- The fork monitor [adds more clients and API providers](https://forkmon.ethdevops.io/)
- Matt Leising’s search for the [DAO attacker in Tokyo](https://www.bloomberg.com/news/articles/2020-09-16/a-trip-down-the-crypto-rabbit-hole-in-search-of-the-dao-hacker)

**Enterprise**

- [Accenture joins the Baseline Protocol](https://twitter.com/OASISopen/status/1305540779075678210)

**Application layer**

- [Uniswap released a governance token](https://uniswap.org/blog/uni/), including Merkle drops to users (even if their transaction failed). Liquidity mining included: Uniswap returns to #1 on DeFiPulse
- An interview with [NFT artist Pak/Archillect](https://thecontrol.co/who-is-pak-e89b12b0f0af), who has made 350k usd in ETH selling art
- Tim Daub: [web3 is stupid right now](https://timdaub.github.io/2020/09/08/web3/)
- ENS’s [decaying price period is over](https://medium.com/the-ethereum-name-service/the-results-of-the-decaying-price-premium-after-releasing-280k-names-7cf57e46b204), names now being released

**Tokens/Business/Regulation**

- Monegro: [don’t burn tokens](https://www.placeholder.vc/blog/2020/9/17/stop-burning-tokens-buyback-and-make-instead)
- [Fork defense strategies in DeFi](https://bankless.substack.com/p/fork-defense-strategies-in-defi)
- [Unikrn settles with the SEC](https://www.sec.gov/news/press-release/2020-211)
- LexDAO [fair guide launch, part 2](https://lexdao.substack.com/p/a-legal-engineers-guide-to-a-fair?)

**Crypto/General**

- Kraken gets [retail banking license](https://blog.kraken.com/post/6241/kraken-wyoming-first-digital-asset-bank/), initially for US only.
- [Winkle](https://www.benthamsgaze.org/2020/09/16/winkle-a-decentralised-checkpointing-for-proof-of-stake/): weak subjectivity checkpoints through transactions

* * *

## **Job Listings**

- [ChainSafe](http://chainsafe.io/) is hiring! Golang blockchain [devs](https://www.notion.so/chainsafe/Blockchain-Developer-Golang-d69bad0b1dd94c43a19db2b332a6f650) and [leads](https://www.notion.so/chainsafe/Technical-Lead-Golang-cbcb6f41d9434672af8b86c735dec865). careers@chainsafe.io
- Gnosis is hiring a [Marketing Manager](https://boards.greenhouse.io/gnosis/jobs/4831653002) for our core product [Gnosis Protocol DEX](https://docs.gnosis.io/protocol/)
- 0x is hiring devs! [Full-stack, back-end, front-end or Solidity](https://0x.org/about/jobs)
- Celer Network: hiring Solidity and Go devs. Email: hiring@celer.network
- Accelerate the growth of Chainlink’s ecosystem as [Head of Growth](https://chainlinklabs.com/careers#job-506559)
- Trail of Bits hiring elite [blockchain security engineers](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & an [R&D engineer](https://jobs.lever.co/trailofbits/94f47428-7c88-43dd-846d-93e3d3059337)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH/DAI/USDC to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **Staking pools get in touch**

🥩 🥩 🥩 I released my [questionnaire for staking pools](https://docs.google.com/document/d/1wrzKXff2XwY4Bu5ynVqvlPXI4xqM4-Hwx7Jh7_-1IGg/edit).

With eth2 due to launch in a matter of weeks, I’m going to recommend staking pools to those of you who want to stake but don’t want to run their own stakers (if you're technically competent, you should very much consider running your own staker especially now that penalties and slashes have been reduced for the first few months!).

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow me on twitter: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-20-2020/](https://weekinethereumnews.com/week-in-ethereum-news-september-20-2020/)

Did you get **forwarded** this newsletter? **[Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **Sep 29 - [eth2 deposit contract/genesis dress rehearsal](https://github.com/goerli/medalla/blob/master/spadina/README.md) (Spadina)**
- **Sep 29 - [ENS online workshop](https://medium.com/the-ethereum-name-service/ens-online-workshop-2020-date-announced-47b8deb69877)**
- Sep30 - Oct25 - [EthPlanet hackathon](https://ethplanet-hackathon.devfolio.co/)
- Oct 1-30 - [EthOnline hackathon](https://www.ethonline.org/) (**application deadline Sept 23**)
- **Oct 2 - [Gitcoin grants matching ends](https://gitcoin.co/grants/). Here’s my [Week in Eth News grant](https://gitcoin.co/grants/237/week-in-ethereum-news)**
- Oct 20 - [submission deadline for Medalla data challenge](https://ethereum.org/en/eth2/get-involved/medalla-data-challenge/)
- **Oct 31 - [submission deadline for Underhanded Solidity Contest](https://underhanded.soliditylang.org/)**
- Nov 6-7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)
- Nov 16 - [MetaMask Provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7)

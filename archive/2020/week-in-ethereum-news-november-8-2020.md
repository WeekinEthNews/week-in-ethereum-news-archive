---
title: "Week in Ethereum News <BR> November 8, 2020"
date: "2020-11-08"
---

## **Eth News and Links**

**Eth1**

- OpenEthereum [v3.1](https://github.com/openethereum/openethereum/releases/tag/v3.1.0) - continues from last stable release (v2.5.13), removes all non-core things from client; includes db migration tool for v2.7
- Péter Szilágyi benchmarks [snap sync v fast sync](https://twitter.com/peter_szilagyi/status/1323488829769175040)
- [Optimal chunking size for code merklization](https://ethresear.ch/t/optimal-chunking-size-for-code-merklization/8185)
- Video and notes from latest [1559 call](https://twitter.com/TimBeiko/status/1324406812045537280), lots of talk about how to do more tests
- Micah Zoltu: [we need 1559 so normal people can use Ethereum](https://medium.com/@MicahZoltu/dc9c8717906)

EIPs/standards

- [EIP3102](https://eips.ethereum.org/EIPS/eip-3102): Binary trie structure
- [EIP3091](https://github.com/ethereum/EIPs/pull/3091): Block explorer API routes

**Proof of Stake launch**

- [Deposit contract is live](https://blog.ethereum.org/2020/11/04/eth2-quick-update-no-19/) at [0x00000000219ab540356cBB839Cbe05303d7705Fa](https://etherscan.io/address/0x00000000219ab540356cbb839cbe05303d7705fa) or depositcontract.eth. Chain launch on Dec 1 if we get 16384 deposits (524288 ETH) by Nov 24.
    - you can use the [launchpad](https://launchpad.ethereum.org/) or [CLI deposit tool](https://github.com/ethereum/eth2.0-deposit-cli/)
    - Please verify with multiples sources the address/domain that I or anyone else gives you
    - Proof of stake spec [v1.0.0](https://github.com/ethereum/eth2.0-specs/releases/tag/v1.0.0)
- Vitalik: [why proof of stake](https://vitalik.ca/general/2020/11/06/pos2020.html); more decentralized, much better security
- Towards [formal semantics of the proof of stake spec](https://ethresear.ch/t/towards-formal-semantics-of-the-beacon-chains-pyspec/8181)
- Video of team [presentations from Medalla data challenge](https://www.youtube.com/watch?v=Gj7YMjBd1RQ)
- [Lighthouse update](https://lighthouse.sigmaprime.io/update-31.html): deposit contract launch
- [Prysm update](https://medium.com/prysmatic-labs/eth-2-0-dev-update-58-mainnet-announced-da1ebd8f301e): mainnet announcement and learnings from Medalla non-finalization

**Layer2**

- [Arbitrum ports Uniswap](https://medium.com/offchainlabs/arbiswap-our-port-of-uniswap-v2-on-arbitrum-rollup-2fe3c64bef00) to its rollup. 2k gas per trade, available using Kovan testnet as layer1

* * *

### **This newsletter is made possible thanks to [Matcha by 0x](https://matcha.xyz/?id=wien)!**

![Matcha](https://weekinethereumnews.com/wp-content/uploads/2020/06/matcha-avatar.png)

Matcha aggregates liquidity across decentralized exchange networks to offer you the best price on every token swap. [Trade 30+ DeFi tokens](https://matcha.xyz/?id=wien) on Matcha today!

* * *

**Stuff for developers**

- typechain [v4](https://twitter.com/krzKaczor/status/1324092593794416640)
- Tenderly adds [proxy support](https://twitter.com/TenderlyApp/status/1324348026631131136)
- [Solt](https://blog.jubb.xyz/post/solt-release/): contract verification from command line (formerly solc-sjw) regardless of framework/structure
- [Running a keeper from Keep3r Network](https://forum.openzeppelin.com/t/running-a-keeper-from-keep3r-network-on-defender/4396) on Zeppelin’s Defender
- Getting [randomness in an NFT](https://blog.chain.link/random-numbers-nft-erc721/) with Chainlink tutorial
- [BitQuery compares themselves to TheGraph](https://bitquery.io/blog/thegraph-and-bitquery)
- Learning about the [EVM by reading GasToken code](https://medium.com/coinmonks/gastoken-or-how-i-learned-to-stop-worrying-and-love-gas-price-surges-6aaee9fb0ba3)

**Security**

- [PercentFinance bug freezes balances](https://percent-finance.medium.com/important-announcement-d35f9a0df112). Forking good code and adding to it can easily make it buggy.
- [Axion](https://cointelegraph.com/news/certik-dissects-the-axion-network-incident-and-subsequent-price-crash) gets immediately hacked. CertiK says [malicious code added post-audit](https://twitter.com/certik_io/status/1323423417215913986)
- [Sandwich attack](https://arxiv.org/pdf/2009.14021.pdf) - frontrunning and backrunning your uniswap transaction to avoid the slippage tolerance

**Enterprise**

- AP records its American [election race calls on Ethereum](https://developer.ap.org/ap-elections-api/#election-race-calls-on-blockchain) mainnet
- [Verizon to log press releases on Mad Network](https://www.verizon.com/about/news/verizons-full-transparency-launches-blockchain-verification), an Ethereum sidechain

**Application layer**

- 1inch [v2](https://1inch-exchange.medium.com/introducing-1inch-v2-defis-fastest-and-most-advanced-aggregation-protocol-c42573dc3f85) - new algo for discovery and routing, new front end, fewer failed txs
- Request Network adds [recurring invoices](https://request.network/en/2020/11/04/automate-your-business-with-recurring-invoices/)
- Voting on Ethereum? Check out [Vocdoni](https://twitter.com/vocdoni/status/1324395257426051072)

**Regulation/business/tokens**

- SEC loosens [some security registration exemptions](https://www.sec.gov/news/press-release/2020-273)

**General**

- [Dilbert’s election day cartoon](https://dilbert.com/strip/2020-11-03) was about Ethereum
- ZenGo’s [Two Party Distributed RSA Modulus Generation](https://github.com/ZenGo-X/vice-city) in Rust
- Brave hits [20 million monthly active users](https://brave.com/20m-mau/)

* * *

## **Job Listings**

- Argent is hiring a [Senior Android Engineer](https://apply.workable.com/argent-1/j/6C69D299DE/) (Remote, Europe only)
- Celer hiring Solidity and Go devs. Email: hiring@celer.network
- Join Chainlink as a [Node Operator Community Manager](https://jobs.lever.co/chainlink/567f8933-d237-4d5a-ae0c-a1f5fb3cccf2?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Trail of Bits hiring [cryptography analyst](https://jobs.lever.co/trailofbits/56af8506-3205-4c7b-b28d-ba8292bd1a47) & [blockchain security engineers](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf)
- 0x looking for [Matcha marketing manager](https://boards.greenhouse.io/0x/jobs/4923909002) and [all flavors of developers](https://0x.org/about/jobs)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **Download The Crypto News Podcast**

Episode 2: Wyre’s [Michael Dunworth](https://thecryptonewspodcast.com/wyre-founder-michael-dunworth)

If you want to support Week in Ethereum News, download and subscribe to my podcast!

Find out [why Michael thinks ETH is going to $3000](https://thecryptonewspodcast.com/wyre-founder-michael-dunworth) and which corporate treasuries will buy BTC

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow the newsletter on twitter: [@WeekinEthNews](https://twitter.com/WeekInEthNews)

Permalink for this week’s issue:  [https://weekinethereumnews.com/week-in-ethereum-news-november-8-2020/](https://weekinethereumnews.com/week-in-ethereum-news-november-8-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Nov 12-13 - [Baseline Protocol Summit](https://www.eventbrite.com/e/baseline-protocol-summit-2020-registration-125941465313)
- Nov 16 - [MetaMask Provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7)
- Nov 19 - EthBerlin 2.5: [Talk Show](https://medium.com/ethberlin/move-over-netflix-theres-a-new-zoom-talk-show-in-town-db48c75d35af)
- **Nov 24 - last day to deposit to be in proof of stake genesis block**
- **Dec 1 - [Proof of stake launch](https://blog.ethereum.org/2020/11/04/eth2-quick-update-no-19/) (if enough deposits by Nov 24)**
- Dec 3 - [Ethereum in the Enterprise - Asia Pacific](https://twitter.com/EntEthAlliance/status/1314652848655872000)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

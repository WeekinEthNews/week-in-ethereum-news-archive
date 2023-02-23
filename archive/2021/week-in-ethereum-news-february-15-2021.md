---
title: "Week in Ethereum News <BR> Feb 15, 2021"
date: "2021-02-15"
---

## **Eth News and Links**

**Mainnet**

- Options for [controlling state size growth](https://hackmd.io/@HWeNw8hNRimMm2m2GH56Cw/state_size_management)
- Using [verkle tries for eth state](https://notes.ethereum.org/_N1mutVERDKtqGIEYc-Flw)
- A [pay-for-storage model for evolving tree hashed data structures](https://gist.github.com/zsfelfoldi/a207d216b3fa9ae4be6abe7a5d8e68d8)
- [GetNodeData DHT approach](https://ethresear.ch/t/state-availability-getnodedata-dht-approach-dev-update/8657) to state availability
- [Transaction gossip network](https://ethresear.ch/t/scalable-transaction-gossip/8660) for light clients

**Proof of Stake**

- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210213)
- Latest [eth2 call](https://youtu.be/z3Gj6TXgcb0?t=205). Notes from [Ben](https://hackmd.io/@benjaminion/H1p6GhG-d) and [Alex](https://twitter.com/ralexstokes/status/1359935655803899905), discussion of what goes in the first network upgrade, [draft spec](https://hackmd.io/QFm6Ih_-Si6_kSLCWTZQyw) in the next couple weeks to turn off PoW
- chaind [v0.2](https://github.com/wealdtech/chaind/releases/tag/v0.2.0), get data off your eth2 node
- [1 million in staking community grants](https://blog.ethereum.org/2021/02/09/esp-staking-community-grantee-announcement/) from EF
- Adrian Sutton’s [hard truths for eth stakers](https://www.symphonious.net/2021/02/13/hard-truths-for-eth-stakers/). Those truths didn’t seem that hard to me.
- Dankrad: [it’s important to go stateless](https://dankradfeist.de/ethereum/2021/02/14/why-stateless.html)

* * *

### **This newsletter is made possible thanks to [Celer](https://www.celer.network/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

[Celer](http://celer.network/) is a coherent layer-2 scaling platform on Ethereum powered by [Generalized State Channel Network](https://www.celer.network/docs/celercore/index.html) and [Hybrid Rollup](https://medium.com/celer-network/adding-hybrid-pos-rollup-sidechain-to-celers-coherent-layer-2-platform-d1d3067fe593) technology. Celer just launched [cBridge](https://blog.celer.network/2021/02/15/celer-cbridge-fast-and-low-cost-value-transfer-network-for-an-interconnected-layer2-and-layer1-future), a multi-chain network that enables instant, low-cost and ANY-to-ANY value transfers within and across Ethereum’s layer-2 chains, Ethereum main chain and in the future, other layer-1s, and layer-2 on top of those other layer-1 chains. Follow Celer on [twitter](https://twitter.com/CelerNetwork), [blog](https://blog.celer.network/), [discord](https://discord.com/invite/Trhab5w) and [telegram](https://t.me/celernetwork).

* * *

**Stuff for developers**

- solc-select [v0.2](https://github.com/crytic/solc-select/releases/tag/0.2.0) for easy switching between Solidity versions
- Remix IDE [v0.10.10](https://medium.com/remix-ide/remix-ide-release-0-10-10-630f43b7edbe)
- Intro to [Solidity’s fuzzing approach](https://blog.soliditylang.org/2021/02/10/an-introduction-to-soliditys-fuzz-testing-approach/)
- [Coding Roulette](https://soliditydeveloper.com/high-stakes-roulette) in Solidity tutorial
- [Automatically verify your code](https://medium.com/shard-labs/how-smart-contracts-can-be-automatically-verified-28ee1c5cf941) with Sourcify
- [Find the unit test failures in your code](https://consensys.net/diligence/blog/2021/02/fault-localisation-with-tarantula/) with Tarantula, implemented in a VScode plugin
- [Infura TX](https://blog.infura.io/itx-now-live-on-mainnet-ethdenver-bounties/), autobump gas prices metarelayer, is live on mainnet
- Hardhat [plugin to fetch the ABI](https://www.npmjs.com/package/hardhat-etherscan-abi) for you
- Setup a [vending machine that accepts crypto payments](https://blog.chain.link/cryptocurrency-vending-machine/) with Arduino device

**Security/incidents**

- Paradigm CTF solution writeups: [Christoph Michel](https://cmichel.io/paradigm-ctf-2021-solutions/), [Stephane](https://github.com/thegostep/paradigm-ctf), [Ansgar Dietrichs](https://hackmd.io/@adietrichs/paradigm-ctf-2021)
- yearn clone [BT](https://twitter.com/StaniKulechov/status/1358885698967896070) got hit for 1.5m with the same attack as last week’s yearn attack
- AlphaHomora [38m hack in a series of complicated transactions](https://blog.alphafinance.io/alpha-homora-v2-post-mortem/). If you were still confused, check out [Bartek Kiepuszewski’s explanation](https://twitter.com/bkiepuszewski/status/1361014447423250440)
- ArmorFi [bug bounty exploit writeup](https://immunefi.medium.com/armorfi-bug-bounty-postmortem-cf46eb650b38), a mistaken hardcoded value
- Dedaub finds [another no-source code exploit](https://medium.com/dedaub/killing-a-bad-arbitrage-bot-f29e7e808c7d), this time in an arb bot with no checks on who calls the function
- [Flashbots and MEV](https://medium.com/flashbots/flashbots-transparency-report-january-2021-922514de8b8a) over the last month. MEV-geth has 3-4% of hashrate
- Dependency confusion: [successful supply chain attacks](https://medium.com/@alex.birsan/dependency-confusion-4a5d60fec610) against BigTech. MetaMask’s [Lavamoat](https://github.com/lavamoat/lavamoat) tools for sandboxing your dependencies

**Ecosystem**

- Check for [claimable airdrops and POAP](https://claimable.vercel.app/)s
- Hackathon submissions from [MarketMake](https://hack.ethglobal.co/marketmake/showcase) and [EthDenver](https://ethdenver2021.devfolio.co/submissions), and the winners for [MarketMake](https://twitter.com/ETHGlobal/status/1359600343152287745) and [EthDenver](https://medium.com/ethdenver/ethdenver-coloradojam-2021-bounty-track-quadratic-funding-winners-805cf5f2de76)
- Coingecko adds an [easy way to get tokens into MetaMask](https://twitter.com/coingecko/status/1358724757110276099)
- Etherscan now shows the [cost for standard types of transactions](https://twitter.com/etherscan/status/1358829488994283525)
- Secureum with more case studies to [teach users how to read audits](https://secureum.substack.com/p/making-cover-safu-secureum-5)
- Although it’s long been clear that EIP1559 is the most popular EIP ever, there’s a [#SupportEIP1559 campaign](https://supporteip1559.org/)

**Enterprise**

- “[Mastercard will start supporting select cryptocurrencies directly on our network](https://www.mastercard.com/news/perspectives/2021/why-mastercard-is-bringing-crypto-onto-our-network/)”
- Amazon had [job listings up for digital payments in Mexico](https://www.coindesk.com/amazon-digital-currency-mexico), but after it was reported the job listings were removed
- BNYMellon developing a [prototype for digital asset custody](https://www.bnymellon.com/latam/en/about-us/newsroom/press-release/bny-mellon-forms-new-digital-assets-unit-to-build-industrypercent27s-first-multi-asset-digital-platform-130169.html) and administration. Deutsche Bank getting into [custody and prime brokerage](https://www.coindesk.com/deutsche-bank-crypto-custody-prime-brokerage)

**Application layer**

- Colony [v2 soft launches](https://blog.colony.io/colony-v2-launch/) DAO platform
- synthetix’s [$TSLA synth](https://twitter.com/DeFi_Dad/status/1360291045263687681), and with afterhours trading on Balancer
- YAM doing [ustonks on UMA](https://yamfinance.medium.com/degenerative-finance-presents-ustonks-4df596e11daf), 10 synthetic stocks of r/WallStreetBets’s favorites
- mStable does a [tokenized BTC basket](https://medium.com/mstable/mstable-launches-mbtc-e26a246dc0bb), mBTC
- Contribute to [clr.fund round 4; it's live](https://blog.clr.fund/round-4-launch/), using MACI’s snark magic to hide who you donate to
- [themanymatts.lol](https://twitter.com/mattgcondon/status/1360014178552066048): Matt Condon gives out NFTs to people who find the stickers he leaves around the world or who meet him and hit the chip in his hand.

**Regulation/business/tokens**

- Mark Cuban: "[ETH has an advantage over BTC as a store of value](https://thedefiant.substack.com/p/mark-cuban-eth-has-an-advantage-over-12f)"
- [St Louis Fed publishes DeFi overview](https://research.stlouisfed.org/publications/review/2021/02/05/decentralized-finance-on-blockchain-and-smart-contract-based-financial-markets) and review
- People have been talking privately about how much MetaMask is making, [Tom Schmidt tweeted it](https://twitter.com/tomhschmidt/status/1359393949568303104). They’re sustainable.
- Simon dlr: [exploring NFTs for authors](https://blog.simondlr.com/posts/exploring-nft-collectibles-for-authors), experimenting with NFTs for his novel

**General**

- Tim Swanson: [Bitcoin and other proof of work coins are an environmental nightmare](https://www.ofnumbers.com/2021/02/14/bitcoin-and-other-pow-coins-are-an-esg-nightmare/)
- [Matic rebrands as Polygon](https://polygontech.medium.com/matic-network-becomes-polygon-ethereums-internet-of-blockchains-expands-mission-and-tech-scope-364932c02cd0) to implement Mihailo Bjelic’s EVM network vision
- GridPlus’s [Lattice hardware wallet is back on sale](http://www.gridplus.io/?afmc=WeekInEthereumNews)! And now with an affiliate program - if you want to support this newsletter and haven’t yet bought the Ethereum community’s hardware wallet, then click the link

* * *

## **Job Listing**

- NEAR is looking for an [EVM interoperability engineer](https://boards.greenhouse.io/near/jobs/4844647002)
- Trail of Bits is looking for a [technical editor/writer](https://jobs.lever.co/trailofbits/8bf936ff-b86c-462e-80b2-4d58004bc68d) & [security engineer](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf)
- 0x looking for [devs of all types](https://0x.org/about/jobs) and a [data analyst](https://boards.greenhouse.io/0x/jobs/4220949002)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-feb-15-2021/](https://weekinethereumnews.com/week-in-ethereum-news-feb-15-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **Feb 28 - [Nimbus Grafana dashboard](https://twitter.com/ethnimbus/status/1360273972944920582) submissions due**
- Mar 5 - Financial Cryptography [DeFi academic workshop](https://fc21.ifca.ai/defi/)
- **Apr 9 - May 14 - ETHGlobal’s [Scaling Ethereum](https://scaling.ethglobal.co/) hackathon**
- May 14 - papers due for [WoSCA 2021](https://trailofbits.github.io/WoSCA/)
- Jul 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

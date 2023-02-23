---
title: "Week in Ethereum News <BR> September 22, 2019"
date: "2019-09-22"
---

## **Eth News and Links**

**Eth1**

- Geth [v1.9.5](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.5) - hot fix release for a larger 1.9.4 maintenance release that sets the blocks for the Ropsten, Rinkeby and Görli testnet forks
- Parity [v2.6.3 beta](https://github.com/paritytech/parity-ethereum/releases/tag/v2.6.3) and [v2.5.8 stable](https://github.com/paritytech/parity-ethereum/releases/tag/v2.5.8) - Istanbul-ready but without blocks set
- Nethermind [v1.0.8](https://github.com/NethermindEth/nethermind/releases/tag/1.0.8) - set for Istanbul
- Latest [core devs call](https://www.youtube.com/watch?v=OjJd2G0pmeM). Live [tweeted notes](https://twitter.com/TimBeiko/status/1175049798975741952).
- Perez, Livshits: [attack resource metering](https://arxiv.org/abs/1909.07220) in EVM. Bring on 1884’s repricing.
- BloXroute says their mainnet test shows they can [reduce block propagation time](https://medium.com/bloxroute/ethereum-miner-test-results-8fbee68b7088) by 25%

**Eth2**

- Danny Ryan: [Eth2 interop in review](https://blog.ethereum.org/2019/09/19/eth2-interop-in-review/). Check out the progress made on networking, tools, and running on raspberry pi's.
- Latest [What’s New in Eth2](https://notes.ethereum.org/@ChihChengLiang/Sk8Zs--CQ/https%3A%2F%2Fbenjaminion.xyz%2Fnewineth2%2F20190920.html?type=book), discussion of BLS sig standardization
- Latest [Eth2 implementers call](https://www.youtube.com/watch?v=pEdqjXO6euY). Notes from [Ben Edgington](https://docs.google.com/document/d/1tTeEwHoOL3twseTsoZwBvjMlqjgZngF8a6-5Krs49so/edit) and [Pooja Ranjan](https://github.com/ethereum/eth2.0-pm/blob/213decb59f9f78d0791b6273332b6aa11e760122/eth2.0-implementers-calls/call_025.md)
- [Prysmatic client](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-35-prysmatic-labs-d1f7515000cd) update - all about faster BLS sigs
- [Alternate phase 2 architecture proposal](https://notes.ethereum.org/YNnC-fakRxixbMCTEnNDXQ?view)

**Layer 2**

- Matter Labs releases their [zk rollup code](https://github.com/matter-labs/rollup)
- [Hijacking routes in payment channel networks](https://arxiv.org/pdf/1909.06890.pdf). arxiv paper showing how to DOS attack Lightning Network
- OmiseGo’s [More Viable Plasma](https://omisego.co/blog/omisego-more-viable-plasma-morevp)

**Stuff for developers**

- [Debugging Solidity with Remix and Ganache](https://medium.com/authereum/debugging-solidity-with-a-gui-remix-and-ganache-c6c16488fcfd)
- Decentralized [storage with 3box for Solidity tutorials](https://medium.com/remix-ide/intro-to-remix-workshop-c14733bdd60c) from within Remix
- [Terminal](https://blog.terminal.co/intro-to-terminal/), dev and manage artifacts in a unified workspace
- [Zabo](https://www.reddit.com/r/ethereum/comments/d5ie05/zabo/), a wrapper for any wallet/interface
- [Get started with ColonyJS](https://kauri.io/article/6325600fdb894517832a26a9cf0babc1/v3/get-started-with-colonyjs)
- Austin Griffith’s [Signatorio](https://twitter.com/austingriffith/status/1175085312659222528), a simple way sign, verify, and share messages signed with your Eth keys
- Intro to the [AZTEC toolkit](https://medium.com/aztec-protocol/the-aztec-toolkit-an-introduction-c4a5d6714c48): how to use their zk proofs

**Ecosystem**

- Gas limit has moved up around [10m per block](https://etherscan.io/chart/gaslimit), so we’re at all time highs in terms of throughput, and puts us in the low to mid 30s for possible transactions per second. However it seems like much of that gas has been used by a ponzi scheme marketed in Asia.
- List of [ENS names that resolve to TOR sites](https://medium.com/the-ethereum-name-service/list-of-ens-names-that-resolve-to-tor-onion-websites-99140a4c674f)
- [Joseph Lubin and Vitalik Buterin interview](https://www.youtube.com/watch?v=wDB4Ntj-RCE&t=3s) at Ethereal Tel Aviv
- Gitcoin CLR matching is live, and there will be [additional 1:1 matching for $50 grants](https://twitter.com/meeseeking/status/1173662455857389568)
- [ethereum.org dev update](https://blog.ethereum.org/2019/09/18/Development-Update-0-Ethereum.org/). Sam Richards leading web dev, website translated into 17 languages, specific pages for [Java devs](https://ethereum.org/java/) and [enterprise](https://ethereum.org/enterprise/)

**Enterprise**

- [Complete transaction privacy](https://kaleido.io/new-zero-knowledge-proof-services/) using Kaleido’s zero knowledge proof services
- Manage identities on [Hyperledger Besu](https://blog.monetha.io/guide-hyperledger-pantheon-digital-identity/)
- Harbor [tokenizes 100m of existing real estate funds](https://www.coindesk.com/harbor-tokenizes-real-estate-funds-worth-100-million-on-ethereum)
- [Deutsche Bank joins JPMorgan’s IIN](https://www.coindesk.com/deutsche-bank-joins-jpmorgans-crypto-payments-network) built on Quorum

**Standards and governance topics**

- [ERC2280](https://github.com/ethereum/EIPs/blob/51ebee319f2a8cc82ba9f04f1546d8cb1c9b06ff/EIPS/eip-2280.md): erc20 extension for native meta transactions support
- [ERC2294](https://github.com/ethereum/EIPs/issues/2294): Explicit bound to Chain ID size
- ProgPoW was again largely debated by the community this week, with [several](https://www.kialo.com/ethereum-and-programmatic-proof-of-work-progpow-30878) [places](https://trello.com/b/KrD25QI5/progpow) [trying](https://www.reddit.com/r/ethereum/comments/d5y8hi/request_for_community_comment_progpow_arguments/) to catalog pros and cons. I wonder how many miners know that in the next few months, they can [transcode video on Livepeer](https://medium.com/livepeer-blog/september-livepeer-ecosystem-update-34db639c0281) on their GPUs without loss of hashrate?
- [Get compensated when anyone uses your deployed code](https://ethresear.ch/t/developer-incentivization-in-protocol-contract-author-fee-rebates/6179)?
- Aragon having an interesting conversation about [whether the current system of voting on grants](https://forum.aragon.org/t/birds-of-a-feather/1277) is the best way to fund working on their stack

**Application layer**

- [Balancer](https://balancer.finance/whitepaper.html), a “non-custodial portfolio manager, liquidity provider, and price sensor” using automated market makers. The new thing from Nikolai
- [Maker and Tether will be added](https://compound.substack.com/p/vote-results-etherscan-and-coinbase) to Compound
- A [tour of the many flavors of Dai](https://medium.com/bzxnetwork/a-tour-of-the-varieties-of-dai-9ff155f7666c)
- Should there be [non-trustless assets in multi-collateral Dai](https://www.reddit.com/r/ethfinance/comments/d6y6mx/including_nontrustless_assets_in_mcd_a_hidden/)?
- Why did the Synthetix attacker get his balance deleted? Because his [frontrunning got frontrun](https://www.reddit.com/r/ethereum/comments/d4ulz0/addressing_claims_of_synthetix_deleted_balances/)
- [Nexus Mutual tracker](https://nexustracker.io/)
- Another week, another Set: [26dayEMA](https://medium.com/set-protocol/introducing-the-eth-26-day-ema-crossover-set-27cce2f08197)
- [AtStake](https://www.reddit.com/r/ethereum/comments/d62xod/looking_for_feedback_on_my_escrow_general/), an escrow app with an internal reputation system. 2 person agreements where ETH/tokens are later programmatically distributed. Disputes by pre-agreed 3rdparty
- [Hoard compiler on Golem Unlimited](https://blog.golemproject.net/hoard-compiler-on-gu-veni-vidi-vici/)
- [Codefi](https://media.consensys.net/introducing-consensys-codefi-the-blockchain-operating-system-for-global-commerce-and-finance-effbac4d91f2) (that’s ConsenSys DeFi) releases [DeFi Score](https://media.consensys.net/introducing-the-defi-score-an-open-source-methodology-to-evaluate-code-and-financial-risk-in-defi-6c8616de791c), an open source framework for evaluating DeFi risk.

**Tokens / Business / Regulation**

- [Neufund’s first retail security token](https://blog.neufund.org/the-first-retail-offering-on-neufund-starts-today-61d8235c7524) offering of Greyp, an electric bike maker
- first draft of the legal agreement for an [Income Share Agreement for American university](https://twitter.com/onggunhao/status/1175430122209517570)
- A [Fee Flippening](https://www.reddit.com/r/ethfinance/comments/d5w4we/ethereum_has_flipped_bitcoin_in_daily_fees_eth/) occurred this week. This has happened before, but the magnitudes of difference in fee volume between ETH/BTC and every other chain it underscores how only Bitcoin and Ethereum have any traction whatsoever.
- [SEC charges ICObox](https://www.sec.gov/news/press-release/2019-181) for selling a security and broker activity
- [Steven Nerayoff and Michael Hlady arrested for extortion](https://www.justice.gov/usao-edny/pr/two-arrested-extortion-startup-cryptocurrency-company) of a company that did a token sale. Nerayoff once [incorrectly claimed](https://www.reddit.com/r/ethtrader/comments/7p5o3a/psa_steven_nerayoff_is_not_a_cocreator_of/) to be a “co-creator” of Ethereum.
- [Ether is the best model for money](https://thedefiant.substack.com/p/ether-is-the-best-model-for-money)

**General**

- [Marlin](https://www.benthamsgaze.org/2019/09/19/a-marlin-is-one-of-the-fastest-snarks-in-the-ocean/) by Chiesa, Hu, Maller, Mishra, Vesely, and Ward. Compared to other SNARKs, small proof sizes and fast verifications, however it requires large Fast Fourier Transforms
- [BitPay to support Ethereum](https://bitpay.com/blog/bitpay-will-support-ethereum/)
- [Everyone’s skeptical EOS predictions have been proven true](https://www.coindesk.com/everyones-worst-fears-about-eos-are-proving-true).
- From [Zero to DeFi Hero](https://defipulse.com/blog/zero-to-defi-cdai/): a guide for crypto noobs to learn enough to earn high DeFi interest rates
- Maker and LoomNetwork creating [bridges to take Dai](https://medium.com/loom-network/making-a-multichain-dai-maker-and-loom-network-to-build-dai-gateways-to-tron-binance-and-other-39ca20bd2a1d) to other chains
- [Cryptoeconomics.study chapter 3](https://www.youtube.com/watch?v=4tlaM53H4hc)
- If you didn’t want to spend ETH to get the 3 year anniversary NFT, [Unlock now has a credit card onramp](https://unlock-protocol.com/blog/unlock-user-accounts/). I did another annotated edition which [anyone who has the NFT can read](https://weekinethereumnews.com/three-year-anniversary-edition/).

* * *

## **🎂 3 year anniversary 🎂**

Just to repeat the advertisement immediately above: you can [buy the limited edition NFT for 0.11 Eth](https://weekinethereumnews.com/three-year-anniversary-edition/) which will unlock the annotated edition.

All proceeds will be back into Ethereum somehow, likely donated to a public good, at my discretion.

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- **Sep 24 - Eth2 staking pool [Rocket Pool testnet beta](https://medium.com/rocket-pool/rocket-pool-beta-v2-guide-cc68ddf90e61) starts**
- Sep 27 - [ErasureCon](https://erasure.xxx/con) (password: information) (SF)
- **Sep 28 - [First ENS short name auctions](https://opensea.io/ens) end**
- Sep 30 - [Gitcoin CLR matching](https://gitcoin.co/blog/gitcoins-q3-match-100k-to-oss-projects/) ends
- **Oct 4 - [Enterprise Ethereum in Banking Summit](https://www.meetup.com/Seoul-Ethereum-Meetup/events/264911728/) (Seoul)**
- Oct 5-6 - [Cryptoeconomics System Summit](https://cryptoresearch.pubpub.org/) (Boston)
- Oct 7 - [ENS workshop](https://medium.com/the-ethereum-name-service/ens-workshop-applications-are-now-open-f46db6c63384) (Osaka)
- Oct 8-11 - [Devcon](https://devcon.org/) (Osaka) and [Devcon social events calendar](http://osaka.kickback.events/events/)
- Oct 19-20 - [Crosslink](https://crosslink.taipei/) (Taipei)
- **Nov 1 - [Ledger EU](https://ledgerproject.eu/) apply for 200k euro startup funding**
- Nov 5-6 - [Decentralized insurance D1Conf](https://blog.etherisc.com/d1conf-2019-to-focus-on-blockchain-adoption-november-5-6th-in-malta-3b8b582ac7b4) (Malta)
- Nov 8-10 - [ETHWaterloo](https://ethwaterloo.com/) **(applications open)**
- Jan 1 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff-update/)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

It’s amazing to me how many people email me when every issue has a link at the bottom saying not to email me to get in the newsletter.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **This headline stays as long as so many people continue to link to old URL and not the right one: [weekinethereumnews.com](https://weekinethereumnews.com/)**

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/week-in-ethereum-news-september-22-2019/](https://weekinethereumnews.com/week-in-ethereum-news-september-22-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

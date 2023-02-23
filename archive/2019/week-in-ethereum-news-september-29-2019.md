---
title: "Week in Ethereum News <BR> September 29, 2019"
date: "2019-09-29"
---

## **Eth News and Links**

**Eth1**

- [Beam Sync](https://medium.com/@jason.carver/intro-to-beam-sync-a0fd168be14a): gets all block headers, executes a recent block using the witness and subsequently fills in state as it executes blocks by getting data from peers. From the Trinity team, it can reduce sync time to minutes.
- Gary Rong [reduces disk i/o 10x](https://twitter.com/peter_szilagyi/status/1176056958568357889) during Geth full sync by patching levelDB
- evmone [v0.2.0](https://github.com/ethereum/evmone/releases/tag/v0.2.0) - 66% faster code processing and execution
- Parity [v2.5.9-stable](https://github.com/paritytech/parity-ethereum/releases/tag/v2.5.9) and [v2.6.4-beta](https://github.com/paritytech/parity-ethereum/releases/tag/v2.6.4) adds block numbers for the Istanbul testnet forks
- Hyperledger Besu [v1.2.4](https://github.com/hyperledger/besu/releases/tag/1.2.4) also adds testnet block numbers

**Eth2**

- “[Wasm execution engine \[running in\] the shard chain/client we built in lighthouse](https://twitter.com/wjvill/status/1176973082604572673)”
- [STARK-proving low-degree-ness of a data availability root](https://ethresear.ch/t/stark-proving-low-degree-ness-of-a-data-availability-root-some-analysis/6214)
- [Cross shard messaging in Casper CBC](https://ethresear.ch/t/cross-shard-messaging-system/6201)
- [Lodestar Eth2 client](https://medium.com/chainsafe-systems/lodestar-post-interop-update-be2caebb39e6) update, in the weeds on networking
- A guide to [getting started on the Prysmatic testnet](https://prysmaticlabs.gitbook.io/prysm/)
- Ben Edgington’s [review of the Eth2 interop lockin](https://media.consensys.net/how-30-eth-2-0-devs-locked-themselves-in-to-achieve-interoperability-175e4a807d92)

**Layer 2**

- [Connext v2 is on mainnet](https://medium.com/connext/connext-v2-0-is-on-mainnet-b818864d3687). Natively supports wallets, more trustless
- [Hierarchical Plasma](https://ethresear.ch/t/hierarchical-plasma-proposal/6171)
- Matic’s next release will [include Plasma predicates](https://blog.matic.network/plasma-predicates-one-step-towards-generalized-plasma/)

**Stuff for developers**

- Yakindu statechart tools for [model-driven Solidity development](https://medium.com/solidity-ide/model-driven-smart-contract-development-for-everyone-28ea066c9b83)
- [Create a Solidity tutorial](https://medium.com/remix-ide/remixide-create-a-workshop-for-solidity-d45f0755fe69) (“workshop”) in Remix
- ConsenSys Diligence’s Alex Wade found a [bug in the Vyper compiler](https://diligence.consensys.net/posts/2019/09/vyper-here-be-snakes)
- [Add comments to your dapp](https://medium.com/3box/introducing-3box-comments-plugin-c6a882d11f4a) with 3Box plugin
- [Recreating geth’s event library step by step](https://rauljordan.com/2019/09/23/how-to-write-an-event-feed-library.html) as a way to learn Go
- Implementing [holographic consensus in Aragon, pt 3](https://blog.aragon.one/my-first-aragon-app-voting-supercharged-with-daostacks-holographic-consensus-part-3/)
- [Intro to using web3j](https://web3developer.io/introduction-to-web3j/)
- Get a [UX audit](https://twitter.com/itsamyjung/status/1177223968299921409) at Devcon
- [Mass NFT minting](https://medium.com/@sean_44011/create-2-255-nfts-with-one-transaction-on-ethereum-b7b7200ce106) with Cargo. Interesting [backstory](https://medium.com/@sean_44011/my-journey-building-products-on-the-blockchain-5c7a99f24f2d) to the product.
- “[two types of bytecode on Ethereum but five different names](https://medium.com/authereum/bytecode-and-init-code-and-runtime-code-oh-my-7bcd89065904)”
- [Brownie v1](https://medium.com/@iamdefinitelyahuman/brownie-turns-1-0-0-3d1f8d736f98) - Python framework for Eth dev
- Ethereum.org now has a page for [Python devs](https://ethereum.org/python/). Submit those pull requests

**Ecosystem**

- The [Fairwin Ponzi scheme has critical security vulnerabilities](https://twitter.com/PhABCD/status/1177398583429140481). The vulnerability [got fully announced today](https://www.reddit.com/r/ethereum/comments/darmk9/vulnerability_disclosure_fairwin_frontrunning_in/), fortunately about half of the ETH has been withdrawn in the past couple days. Also relevant: [Daniel Luca’s tweetstorm](https://twitter.com/cleanunicorn/status/1177544181679558656).
- Guide to run a [full node on a RaspberryPi 4 (model B)](https://kauri.io/article/9695fcca217f46feb355245275835fc0)
- [DeFi Summit vids](https://www.youtube.com/playlist?list=PLhbK0NpGv8dWsjLpYA-OM4gQk-GdQe7X2)
- Dataviz of [mining pool % over time](https://twitter.com/AlethioEthstats/status/1176511383195783172)
- The most [popular names in the ENS auction](https://medium.com/the-ethereum-name-service/the-most-popular-eth-names-in-the-ens-short-name-auction-5ee13bb0eace)
- [Ethereal Blocks hackathon winners and submissions](https://gitcoin.co/blog/ethereal-blocks-retro-sponsors-winners-and-more/)

**Enterprise**

- WWF and ConsenSys develop [Impactio, a nonprofit funding platform](https://media.consensys.net/consensys-and-wwf-team-up-to-launch-impactio-f9780d168d6e)
- [uPort, Onfido and PwC](https://content.consensys.net/wp-content/uploads/uPort-with-Onfido-PWC-_-Sibos-2019.pdf) to partner on identities in UK financial services
- Hong Kong traded Link REIT partners with Allinfra to [tokenize a solar installation](https://allinfra.com/wp-content/uploads/2019/09/Allinfra-Link-REIT-Press-Release-23-Sep-2019.pdf)

**Standards and governance topics**

- ERC1620 [money streaming is in last call](https://github.com/ethereum/EIPs/issues/1620)
- Why wrapping [TheDao in Delaware LLC governance](https://medium.com/openlawofficial/unpacking-the-lao-e463f7357b4b) makes sense

**Application layer**

- Maker: [upgrading to multi-collateral Dai](https://blog.makerdao.com/looking-ahead-how-to-upgrade-to-multi-collateral-dai/) from current single-collateral Dai (it will be mandatory, though you’ll likely have a few months when it happens), and an update on the [new Oasis DEX](https://blog.makerdao.com/update-on-the-new-oasis/) - trade ETH for MCD assets
- Rune floats [ETH purity assets](https://twitter.com/RuneKek/status/1176393472552534018) (ie, single-collateral Dai) in MCD
- [DeFi Saver had a couple CDPs get liquidated](https://medium.com/defi-saver/automatic-cdp-protection-faux-pas-analysis-updates-in-place-and-next-steps-e238e0d3114). While they’re covering the cost, it’s always worth thinking about the risks for any product you use.
- [Nuo v2 margin trading](https://medium.com/nuo-news/introducing-all-new-margin-trading-on-nuo-caf549b688d4)
- Golem chooses a metric for how often to [verify wasm computation](https://blog.golemproject.net/gwasm-verification/): reputation combined with a user chosen variable
- How to [use SetProtocol if the front end is down](https://medium.com/set-protocol/operating-set-protocol-manually-bd14e917923f). More apps should do this
- [Dolomite launches exchange on Loopring](https://medium.com/dolomite-official/dolomite-is-live-228c58df5005) with negative maker fees and a fiat onramp through Wyre

**Tokens / Business / Regulation**

- IMF: the [rise of stablecoins](https://blogs.imf.org/2019/09/19/digital-currencies-the-rise-of-stablecoins/)
- Spencer Dinwiddie wants to tokenize a portion of the next [3 years of his NBA contract](https://fortune.com/2019/09/26/nba-spencer-dinwiddie-recession-tokenizing-contract). Minimum $150k investment though.
- Kik to [shut down Kik](https://medium.com/@tedlivingston/moving-forward-boldly-with-kin-ec6290a6453). Bit of a headscratcher to me.
- [Miners are accumulating ETH](https://www.reddit.com/r/ethfinance/comments/d98chg/ethereum_miner_balances_continue_to_increase/)
- [Nonfungible ERC20 tokens](https://medium.com/@iamdefinitelyahuman/nftoken-the-non-fungible-erc20-cacc6c2826e6)

**General**

- Chiesa, Ojha, Spooner: [Fractal](https://eprint.iacr.org/2019/1076) efficient recursive composition of post-quantum SNARKs
- Vitalik: [understanding PLONK](https://vitalik.ca/general/2019/09/22/plonk.html)
- Understanding [gas accounting and the fee market](https://medium.com/@eric.conner/understanding-ethereum-gas-blocks-and-the-fee-market-d5e268bf0a0e)
- Filecoin hopes to launch [mainnet in March 2020](https://filecoin.io/blog/update-2019-q2-q3/)
- Major [Lightning Network vulnerability](https://lists.linuxfoundation.org/pipermail/lightning-dev/2019-September/002174.html) allowed BTC to be stolen
- Your [TV is tracking you](https://twitter.com/random_walker/status/1177570679232876544).

* * *

## **🎂 3 year anniversary 🎂**

I did another annotated version for the folks who bought the NFT. They can read [the limited edition](https://weekinethereumnews.com/three-year-anniversary-edition/). This will very likely be the last annotated edition.

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Sep 30 - [Gitcoin CLR matching](https://gitcoin.co/blog/gitcoins-q3-match-100k-to-oss-projects/) ends
- **Oct 2 - Istanbul fork on Ropsten testnet at block #6485846**
- Oct 4 - [Enterprise Ethereum in Banking Summit](https://www.meetup.com/Seoul-Ethereum-Meetup/events/264911728/) (Seoul)
- Oct 5-6 - [Cryptoeconomics System Summit](https://cryptoresearch.pubpub.org/) (Boston)
- Oct 7 - [ENS workshop](https://medium.com/the-ethereum-name-service/ens-workshop-applications-are-now-open-f46db6c63384) (Osaka)
- Oct 8-11 - [Devcon](https://devcon.org/agenda) (Osaka). **Link to agenda.  Social events: [OffDevcon](https://www.offdevcon.com/) and [Kickback](http://osaka.kickback.events/events/)**
- Oct 19-20 - [Crosslink](https://crosslink.taipei/) (Taipei)
- **Oct 26 - [Zero Knowledge Summit](https://www.zeroknowledge.fm/summit) (SF)**
- Nov 1 - [Ledger EU](https://ledgerproject.eu/) apply for 200k euro startup funding
- Nov 5-6 - [Decentralized insurance D1Conf](https://blog.etherisc.com/d1conf-2019-to-focus-on-blockchain-adoption-november-5-6th-in-malta-3b8b582ac7b4) (Malta)
- Nov 8-10 - [ETHWaterloo](https://ethwaterloo.com/)
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

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/week-in-ethereum-news-september-29-2019/](https://weekinethereumnews.com/week-in-ethereum-news-september-29-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

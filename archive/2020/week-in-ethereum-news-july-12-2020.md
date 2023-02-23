---
title: "Week in Ethereum News <BR> July 12, 2020"
date: "2020-07-12"
---

## **Eth News and Links**

**Eth1**

- Piper Merriam argues that an [Eth client needs to be easier to build](https://snakecharmers.ethereum.org/applying-the-five-whys-to-the-client-diversity-problem/)
- [Deploying Nethermind](https://medium.com/nethermind-eth/deploying-nethermind-ethereum-client-with-monitoring-stack-55ce1622edbd) with Grafana/Prometheus/Seq monitoring stack
- Latest [core devs call](https://youtu.be/RUZ3eJ81c0k). Notes from [Beiko](https://twitter.com/TimBeiko/status/1281584671206211585) and [Ranjan](https://github.com/ethereum/pm/blob/cd5e46d86909e034568ef01b0022def006248e0a/All%20Core%20Devs%20Meetings/Meeting%2091.md), quick discussion of some EIP progress and then much discussion of Piper’s article above
- [Simpler sync: state snapshots and blockchain and receipt files](https://ethresear.ch/t/simpler-ethereum-sync-major-minor-state-snapshots-blockchain-files-receipt-files/7672)
- [DHT-based state network](https://notes.ethereum.org/EYRD1-NZQ5aVRCsM4fg92Q) sketch
- Vitalik’s [stateless client witnesses](https://vitalik.ca/files/misc_files/stateless_client_witnesses.pdf) deck
- Quilt’s [account abstraction playground](https://github.com/quilt/account-abstraction-playground)

**Eth2**

- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200710)
- [EF’s Eth2 research team AMA](https://www.reddit.com/r/ethereum/comments/ho2zpt/ama_we_are_the_efs_eth_20_research_team_pt_4_10/) - on track to [ship phase0 genesis in 2020](https://www.reddit.com/r/ethereum/comments/ho2zpt/ama_we_are_the_efs_eth_20_research_team_pt_4_10/fxj2r7p/) with [phase1 hopefully close behind](https://www.reddit.com/r/ethereum/comments/ho2zpt/ama_we_are_the_efs_eth_20_research_team_pt_4_10/fxizpkf/). Also a [VDF update](https://www.reddit.com/r/ethereum/comments/ho2zpt/ama_we_are_the_efs_eth_20_research_team_pt_4_10/fxj4gsh/), among other nuggets.
- Latest [eth2 call](https://youtu.be/4IooxDX_GfU?t=49). Notes from [Ben](https://hackmd.io/@benjaminion/B1WexiV1P) and [Mamy](https://gist.github.com/mratsim/9fe87f650cde05c5da8c3c49da2f3b06)
- [Beacon fuzz](https://blog.sigmaprime.io/beacon-fuzz-06.html) - eth2 client differential fuzzer is now dockerized so anyone can run it and try to find eth2 client bugs. The fuzzer has found bugs in Nimbus and Lodestar in last month
- [Lighthouse client](https://lighthouse.sigmaprime.io/update-27.html) update - Altona testnet review, new BLS library doubles sync speed, better peer management
- Nimbus wants you to be able to run an [eth2 validator on an old phone](https://our.status.im/the-importance-of-an-easy-to-use-mobile-friendly-client/)
- [BeaconScan](https://medium.com/etherscan-blog/beaconscan-the-validators-explorer-66c5aa2d4229) will have dashboard and email alerts for validators
- IPFS’s [GossipSub v1.1](https://blog.ipfs.io/gossipsubv1.1-eval-report-and-security-audit/) full evaluation (used in eth2)

**Layer2**

- A pithy [explanation of how zk rollups work](https://ethresear.ch/t/validating-transactions-with-zk-methods/7654/3)

* * *

### **This newsletter is made possible thanks to [Trail of Bits](https://www.trailofbits.com/)!**

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fa28d33ed-ff02-4179-b90f-1d1545069584_1876x1128.png)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fa28d33ed-ff02-4179-b90f-1d1545069584_1876x1128.png)

[Easily verify your contracts with manticore-verifier](https://blog.trailofbits.com/2020/07/12/new-manticore-verifier-for-smart-contracts/). Express security properties in Solidity and have them extensively tested with fuzzing and symbolic execution. Get started with this short tutorial from Trail of Bits.

* * *

**Stuff for developers**

- Solidity [v0.6.11](https://solidity.ethereum.org/2020/07/07/solidity-0611-release-announcement/) - inheritance for NatSpec comments, better debugging data output
- Truffle [v5.1.34](https://github.com/trufflesuite/truffle/releases/tag/v5.1.34) - lots of dependency updates (eg, Node >=10.12)
- A 4 part series on [web3.go](https://medium.com/coinmonks/web3-go-part-1-31c68c68e20e), using go-ethereum as a library
- 5 year [anniversary of the first Solidity release](https://solidity.ethereum.org/2020/07/08/solidity-turns-5/)
- [Transthereum](https://medium.com/unibrightio/transthereum-unibrights-open-source-blockchain-explorer-for-developers-2894d0bac293), simple block explorer for local environments like Ganache
- Alchemys’s [Build tool suite](https://blog.alchemyapi.io/blog/alchemy-build-the-most-powerful-tools-for-blockchain-developers) - block explorer, tx pool visualizer, RPC call composer
- Torus now supports [Eth wallets for accounts](https://medium.com/toruslabs/login-to-torus-with-appleid-github-linkedin-twitter-line-and-passwordless-accounts-50c591725de2) from Google, Facebook, Reddit, Twitch, Discord, AppleID, Github, LinkedIn, Twitter, Line & Passwordless
- [Legions](https://media.consensys.net/legions-a-tool-for-ethereum-security-researchers-e526cb84c505) - ConsenSysDiligence tool to query common node endpoints
- [Verify invariants of your contracts using Manticore](https://blog.trailofbits.com/2020/07/12/new-manticore-verifier-for-smart-contracts/) tutorial
- Austin Griffith’s [scaffold-eth with IPFS](https://medium.com/@austin_48503/tl-dr-scaffold-eth-ipfs-20fa35b11c35) tutorial
- Epheph video on avoiding [honey pots](https://twitter.com/epheph/status/1281340414105014272) with Tenderly
- Understanding the [diamond proxy standard](https://dev.to/mudgen/understanding-diamonds-on-ethereum-1fb), contracts that share storage variables and Eth address.

**Ecosystem**

- [TheGraph processed one billion queries](https://thegraph.com/blog/one-billion-monthly-queries) in June 2020
- DeFi hits [2 billion dollars locked up](https://twitter.com/defipulse/status/1280864007029583873)

**Enterprise**

- Nethermind and Provide offer [enterprise-focused privacy, messaging and key management](https://medium.com/nethermind-eth/nethermind-partners-with-provide-to-offer-advanced-key-management-enterprise-support-a5d4c065b920)
- EEA picks [Daniel Burnett as executive director](https://entethalliance.org/enterprise-ethereum-alliance-appoints-dr-daniel-burnett-as-executive-director/)

**Standards**

- [ERC2774](https://github.com/ethereum/EIPs/blob/de0b77485de2de96ce7b94b0b7a7131e18be19bf/EIPS/eip-2774.md): price-sensitive challenge process
- [ERC2770](https://github.com/ethereum/EIPs/blob/c2417ea6c2aed914279429b5e90b685671a695c2/EIPS/eip-2770.md): Meta-Transactions Forwarder Contract

**Application layer**

- [Cryptograph](https://medium.com/cryptograph/introducing-cryptograph-a01fc53399e1) art NFT auction where previous bidder gets ~10% of the diffential of the higher bid, with creator profits to charity. My [NFT auction](https://cryptograph.co/Cryptograph/Evan-Van-Ness-Web3-Is-Coming) (I “drew” the Eth logo) ends in ~18 hours
- [Aave adds credit delegation](https://twitter.com/StaniKulechov/status/1280500969986498561), so one address can delegate its credit to another
- Unstoppable Domains released [dchat messaging using GunDB](https://medium.com/@AlexMasmej/introducing-dchat-an-open-source-chat-protocol-linked-to-your-crypto-address-f657de73a62a), which got some [criticism from the folks at Status researching messaging](https://twitter.com/DeanEigenmann/status/1280643845219377153)
- [Kyber’s Katalyst upgrade is live](https://blog.kyber.network/katalyst-and-kyberdao-are-now-live-19ee6a6eb77e) with KyberDAO staking/governance, custom fee/spread & lots more
- SEC approves [tokenized (live on Eth mainnet) shares of Arca’s US Treasury debt fund](https://arcoin.arcalabs.com/)

**Tokens/Business/Regulation**

- TheBlock broke the story that [USDC blacklisted 100k](https://www.theblockcrypto.com/linked/70850/centre-appears-to-have-blacklisted-an-address-holding-usdc-for-the-first-time)
- [Censorable assets are toxic collateral](https://www.tonysheng.com/p/censorable-assets-are-toxic-collateral)
- [Aggregation theory applied to DeFi](https://insights.deribit.com/market-research/aggregation-theory-applied-to-defi/)
- The [Protocol Sink Thesis](https://bankless.substack.com/p/global-public-goods-and-the-protocol)
- [Experimental land rights in VR](https://blog.simondlr.com/posts/experimental-land-rights-in-vr)
- A list of [yield farming opportunities](https://tokenbrice.xyz/posts/2020/yield-farmer-tier-list/)

**General**

- Crypto companies taking US federal bailouts: differing lists from [Coindesk](https://www.coindesk.com/consensys-polychain-tron-ciphertrace-blockchain-startups-got-18m-in-us-ppp-bailout-loans) and [TheBlock](https://www.theblockcrypto.com/post/70511/ledgerx-consensys-tendermint-crypto-ppp-trump)
- Coinbase is talking to [bankers about an IPO](https://www.reuters.com/article/us-coinbase-ipo-exclusive/exclusive-crypto-exchange-coinbase-readies-landmark-stock-market-listing-sources-idUSKBN24A21W)
- [Brave Ads have a ~10% CTR](https://brave.com/nyiax-partnership/)

* * *

## **Job Listings**

- Sigma Prime is hiring [Blockchain Security Engineers](https://github.com/sigp/positions-vacant/blob/master/security-engineer.md) and an [Executive Assistant](https://github.com/sigp/positions-vacant/blob/master/ea.md)
- [0x is hiring](https://0x.org/about/jobs) a Periscope tech lead & full-stack, back-end, and front-end engineers
- Trail of Bits is looking for an elite [blockchain security engineer](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf)
- Celer Network: [Android developer](https://www.celer.network/career.html)
- Lead the Chainlink technical community as the [Head of Community](https://careers.smartcontract.com/o/head-of-community)! 

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH/DAI/USDC to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **Housekeeping**

Follow me on Twitter [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get the **annotated edition of this newsletter** on Monday or Tuesday. Plus I tweet most of what makes it into the newsletter.

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-july-12-2020/](https://weekinethereumnews.com/week-in-ethereum-news-july-12-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **Jul9 - Aug30 - [EthPlanet’s Summer Camp](https://www.ethplanet.org/ethereum-summer-camp-2020/) virtual event series**
- July 20 - [Fork the World](https://metagame.substack.com/p/fork-the-world-hackathon) MetaCartel hackathon
- July 28 - [Augur v2 launch](https://www.augur.net/blog/v2-launch/)
- July 30 - EEA’s [Ethereum in the Enterprise 2020](https://www.conference.entethalliance.org/) virtual conference
- Aug 2 - [ENS grace period](https://medium.com/the-ethereum-name-service/the-great-renewal-its-time-to-renew-your-eth-names-or-else-lose-them-afccea4852cb) begins to end
- **Aug 28-29 - Chainlink’s [Smart Contract Virtual Summit](https://www.smartcontractsummit.io/)**
- Oct 2-Oct 30 - [EthOnline hackathon](https://www.ethonline.org/)
- **Nov 6-Nov 7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)**

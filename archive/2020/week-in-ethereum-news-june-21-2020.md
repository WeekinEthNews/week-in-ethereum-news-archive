---
title: "Week in Ethereum News <BR> June 21, 2020"
date: "2020-06-21"
---

## **Eth News and Links**

**Eth1**

- Trinity [v0.1.0-alpha.36](https://github.com/ethereum/trinity/releases/tag/v0.1.0-alpha.36) (Python client) - BeamSync improvements, metrics tracking (influxDB/Grafana), partial eth/65 support
- Updated [Eth on ARM images](https://www.reddit.com/r/ethereum/comments/hbxrq0/ethereum_on_arm_new_eth10_image_for_the_raspberry/). Geth fast syncs a full node in 40 hours on 8GB Raspberry Pi4
- Miners began [bumping up the gas limit](https://twitter.com/etherchain_org/status/1273912037274537984) (12m now), which sparked some [polemics](https://twitter.com/peter_szilagyi/status/1273921434700730369) about the tradeoff between state growth versus user fees. Higher gas limit resulted in safelow gas fees in the teens for the first time in weeks.

**Eth2**

- Prysmatic [(Go) client update](https://medium.com/prysmatic-labs/eth-2-0-dev-update-52-onyx-testnet-launched-a87a937f292e) - stable Onyx testnet, 80% validators community run, RAM usage optimizations
- Nimbus [(Nim) client update](https://our.status.im/nimbus-june-update/) - up to spec, 10-50x processing speedup, splitting node and validator clients
- SigmaPrime’s update on their [Eth2 fuzzer](https://blog.sigmaprime.io/beacon-fuzz-05.html) - found some Prysmatic bugs, fuzzing Lodestar (Javascript client), Lighthouse ENR crate bug, dockerizing the fuzzer so the community can run it
- Jonny Rhea’s Packetology posts ([one](https://ethresear.ch/t/packetology-validator-privacy/7547/) and [two](https://ethresear.ch/t/packetology-eth2-testnet-block-propagation-analysis/7561)) on identifying validators
- [Attack nets](https://notes.ethereum.org/@djrtwo/Hkth99G3I) - a testnet specifically for attacks

**Layer2**

- Matter Labs’ [ZK Sync rollup is live](https://medium.com/matter-labs/zksync-is-live-bringing-trustless-scalable-payments-to-ethereum-9c634b3e6823) - tiny transaction fees, withdrawals to Eth mainnet in 15 mins, 300 transactions per second (with 2000 tps coming)
- [Minimally viable rollback](https://ethresear.ch/t/mvr-minimally-viable-rollback/7538) in Validium/Volition

**Crypto**

- a [GKR inside a snark](https://ethresear.ch/t/using-gkr-inside-a-snark-to-reduce-the-cost-of-hash-verification-down-to-3-constraints/7550) to speed up SNARK proving 200x
- Attacking the [Diogenes setup ceremony for Eth2's VDF](https://medium.com/zengo/diogenes-octopus-playing-red-team-for-eth2-0-vdf-part-1-dac3f2e3cc7b)
- [Isogenies VDFs: delay encryption](https://ethresear.ch/t/vdfs-delay-encryption/7542)
- [Kate polynomial commitments](https://dankradfeist.de/ethereum/2020/06/16/kate-polynomial-commitments.html) explainer from Dankrad Feist
- [Reputable List Curation from Decentralized Voting](http://eprint.iacr.org/2020/709) Crites, Maller, Meiklejohn and Mercer paper for construction of private TCR voting

* * *

### This newsletter is made possible thanks to [Matcha by 0x](https://matcha.xyz/?id=weekinethereum1)!

![](https://weekinethereumnews.com/wp-content/uploads/2020/06/matcha-avatar.png)

0x is excited to sponsor Week in Ethereum News and invite readers to try out [our new DEX](https://matcha.xyz/?id=weekinethereum1)!

Sign up here to get early access to [Matcha](https://matcha.xyz/?id=weekinethereum1), your new home for fast, secure token trading.

* * *

**Stuff for developers**

- [Waffle v3](https://medium.com/ethworks/waffle-3-0-released-with-ethers-js-5-0-and-more-fc76d5232ae4) with ethers v5 support
- [WalletConnect v1 release](https://medium.com/walletconnect/walletconnect-beta-is-over-2644efd372aa), now with mobile linking
- [ethers-rs](https://docs.rs/ethers/0.1.3/ethers/), a port of ethers to Rust
- Solidity [v0.6.10](https://solidity.ethereum.org/2020/06/11/solidity-0610-release-announcement/). error codes and bugfix for externally calling a function that returns variables with calldata location.
- [Inheritance in Solidity v0.6](https://solidity.ethereum.org/2020/06/18/solidity-0.6-inheritance/)
- [Sorting without comparison](https://medium.com/coinmonks/sorting-in-solidity-without-comparison-4eb47e04ff0d) in Solidity
- Create [dynamic NFTs using oracles](https://blog.chain.link/create-dynamic-nfts-using-chainlink-oracles/)
- [Deploying with libraries on Remix IDE](https://medium.com/remix-ide/deploying-with-libraries-on-remix-ide-24f5f7423b60)
- Wyre’s [WalletPasses](https://blog.sendwyre.com/native-apple-and-google-wallet-integration-for-teams-protocols-b3ebe674bf0c) allow push notifications for dapps

**Code security**

- OpenZeppelin found a [bug that affected 61 Argent](https://blog.openzeppelin.com/argent-vulnerability-report/) wallets
- Bancor bug: public method allowed anyone to drain user balances. Amusingly, the [white hat draining got frontrun](https://medium.com/@1inch.exchange/bancor-network-hack-2020-3c71444fd59d)
- [DeFiSaver exchange vulnerability](https://medium.com/defi-saver/disclosing-a-recently-discovered-exchange-vulnerability-fcd0b61edffe). They white hat drained it and also got frontrun.
- [Database of audit reports](https://consensys.github.io/blockchainSecurityDB/)
- Check out this **newsletter’s weekly job listings** below the general section

**Ecosystem**

- [Reddit announces scaling competition](https://www.reddit.com/r/ethereum/comments/hbjx25/the_great_reddit_scaling_bakeoff/) to move Reddit’s community points to mainnet
- It seems the mysterious and [massive transaction fees were from a hacked korean ponzi called GoodCycle](https://twitter.com/peckshield/status/1272924046091358209). Various miners have handled differently: [Ethermine](https://twitter.com/etherchain_org/status/1272425639673462784) (already paid out). [Sparkpool](https://twitter.com/sparkpool_eth/status/1272809999392071680) (said it would pay out but then victim identified, unclear to me if yet resolved). [f2pool](https://blog.f2pool.com/en/announcement-en/handling-of-abnormal-eth-tx-en) (said they’d return to new address)
- By default, Geth will no longer [accept transaction fees over 1 eth](https://twitter.com/peter_szilagyi/status/1273163343562510340)
- 3box on [demystifying the many facets of digital identity](https://medium.com/3box/demystifying-digital-id-6ec413b129ac)
- The [death (and web3 rebirth?) of privacy](https://blog.usejournal.com/the-death-and-rebirth-of-privacy-bb7d06e90653)
- Ethereum Foundation [invests in Unicef's CryptoFund startups](https://www.unicef.org/innovation/CryptoFundInvestments)

**Enterprise**

- WEF, IADB and Colombian government project to [reduce corruption in procurement](https://www.weforum.org/reports/exploring-blockchain-technology-for-government-transparency-to-reduce-corruption)
- EY launches [crypto tax reporting app](https://www.ey.com/en_us/news/2020/06/ey-launches-first-of-its-kind-cryptocurrency-reporting-app)

**DAOs and Standards**

- [EIP2733](https://github.com/lightclient/EIPs/blob/transaction-package/EIPS/eip-2733.md): Transaction package
- [Anonymous voting using MACI and BrightID](https://medium.com/brightid/anonymous-participation-e-g-voting-using-brightid-42a13b4d1c94)

**Application layer**

- [$COMP was distributed](https://medium.com/compound-finance/compound-community-ownership-ee0ed1252cc3) and liquidity mining (“yield farming”) blew up. Compound passed Maker for #1 on DeFiPulse, and $COMP has had a fully diluted market cap over $3.5 billion
- [Uniswap v2 passes v1](https://migrate.uniswap.info/home) in liquidity
- Streamr’s [data unions framework](https://www.reddit.com/r/ethereum/comments/hberts/news_the_streamr_data_unions_framework_is_live_in/) is live for anyone to create their own
- [5m KNC burned](https://twitter.com/loi_luu/status/1273640515573968899) milestone
- [Yield farming on steroids](https://medium.com/renproject/introducing-an-incentivized-btc-liquidity-pool-by-ren-synthetix-and-curve-213d21691d9a) from Synthetix, Ren, and Curve
- A [yield farming for normies](https://twitter.com/tonysheng/status/1274393189231689728) (and the [risks](https://twitter.com/tonysheng/status/1274780457729617920)!) tweetstorms from Tony Sheng
- [this artwork is always on sale, v2](https://blog.simondlr.com/posts/this-artwork-is-always-on-sale-v2) with 100% per year tax instead of 5%

**Tokens/Business/Regulation**

- ETH disrupting SWIFT: [why fintech VCs are missing DeFi](https://bankless.substack.com/p/why-the-vcs-are-missing-defi)
- Nick Tomaino on the [economics of Eth2](https://thecontrol.co/the-economics-of-eth2-dbcc78a2f48)
- [Personal token vote on Alex Masmej’s life decisons](https://medium.com/@AlexMasmej/introducing-control-my-life-use-my-cryptocurrency-alex-to-vote-on-my-life-choices-8d62471963cd)
- Liechtenstein company [tokenizes 1.1m USD collectable Ferrari](https://curioinvest.com/car/4)
- Opyn: [hedging with calls](https://medium.com/opyn/hedging-with-calls-6a1a8f77eb66)

* * *

## **Job Listings**

- Synthetix: Deep [Solidity engineer](https://docs.google.com/document/d/1xtEyu2pBszNRYjWyzNxndFipIORr5RnyhzJQNprBMm8/edit#heading=h.pdeo1jdmjhxc), 2+ years exp & US/EU friendly timezone
- Chainlink: [Product Manager for Blockchain Integrations](https://careers.smartcontract.com/o/product-manager-blockchain-integrations) and [Lead Test Engineer](https://careers.smartcontract.com/o/lead-test-engineer-on-chainlink)
- [0x is hiring](https://0x.org/about/jobs) full-stack, back-end, front-end engineers + 1 data scientist
- Celer Network: [Android developer](https://www.celer.network/career.html)
- Trail of Bits is looking for masters of low-level security. [Apply here](https://jobs.lever.co/trailofbits/8b7f7fc1-efb0-4e89-b406-784c3a2d77e4).

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH/DAI/USDC to evan.ethereum.eth. Questions? thecryptonewspodcast -at-gmail

* * *

## **Housekeeping**

Follow me on Twitter [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get the **annotated edition of this newsletter** on Monday or Tuesday. Plus I tweet most of what makes it into the newsletter.

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-june-21-2020/](https://weekinethereumnews.com/week-in-ethereum-news-june-21-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- June 24 - [EIP1559 call](https://github.com/ethereum/pm/issues/184)
- June 25 - Eth2 call
- June 26 - [Core devs call](https://github.com/ethereum/pm/issues/180)
- June 29 - [Swarm first public event](https://swarm-gateways.net/bzz:/alpha.swarm.eth/)
- **July 3 - [Gitcoin matching grants](https://gitcoin.co/grants) ends (here’s [my grant](https://gitcoin.co/grants/237/week-in-ethereum-news))**
- **July 6-Aug 6 - [HackFS](https://hackfs.com/) Filecoin/IPFS and Ethereum hackathon**
- **July 20 - [Fork the World](https://metagame.substack.com/p/fork-the-world-hackathon) MetaCartel hackathon**
- Aug 2 - [ENS grace period](https://medium.com/the-ethereum-name-service/the-great-renewal-its-time-to-renew-your-eth-names-or-else-lose-them-afccea4852cb) begins to end
- Oct 2-Oct 30 - [EthOnline hackathon](https://www.ethonline.org/)

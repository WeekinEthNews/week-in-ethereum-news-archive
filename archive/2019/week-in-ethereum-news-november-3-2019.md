---
title: "Week in Ethereum News <BR> November 3, 2019"
date: "2019-11-04"
---

## **Eth News and Links**

**Eth1**

- [Skinny eip1559](https://ethereum-magicians.org/t/skinny-eip-1559/3738), an easier to implement gas fee market change
- Latest [core devs call](https://www.youtube.com/watch?v=aZ0S_oLSwhE). Beiko’s [notes](https://twitter.com/TimBeiko/status/1190269448621633536). To reiterate: Istanbul scheduled for Dec 4. Next fork scheduled in 6 months (~June).
- Academic paper [profiling Parity](https://arxiv.org/pdf/1910.11143.pdf) says SLOAD, SSTORE, and CALLCODE costs are increasing with block height

**Eth2**

- Danny Ryan’s [eth2 update](https://blog.ethereum.org/2019/10/31/eth2-quick-update-no-2/) has a simple explanation of new phase1 plan
- [phase 0 spec v0.9](https://github.com/ethereum/eth2.0-specs/releases/tag/v0.9.0), some changes given phase 1 shift
- [Implementing cross shard transactions](https://ethresear.ch/t/implementing-cross-shard-transactions/6382) by sequentially processing receipts
- [Prysmatic client update](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-38-prysmatic-labs-a3293ca9280d) - better caching, getting up to spec v0.9
- [Lodestar client update](https://medium.com/chainsafe-systems/lodestar-post-devcon-update-78886344c1e1) - optimizing state transition/caching, light client research
- Updated Eth2 [devs handbook and FAQs](https://notes.ethereum.org/@serenity/handbook)

**EIPs**

- EIP2330: [EXTSLOAD opcode](https://github.com/dominicletz/EIPs/blob/343818c1206f5649bdbdfba12792e9abf3727533/EIPS/eip-2330.md)
- EIP2327: [BEGINDATA opcode](https://github.com/ethereum/EIPs/blob/279b1cd2ddf022cde00d1bf2b8007004be9fa3b5/EIPS/eip-2327.md)
- EIP2333: [BLS12-381 Key Generation](https://github.com/ethereum/EIPs/blob/2d1f68ab42da3e6ee06f735e0543c2291480a1a2/EIPS/eip-2333.md) and [call for spec for public key checksums](https://github.com/CarlBeek/EIPs/blob/840af2fa4e6cbf6c26668d022982a54ab06787f8/EIPS/eip-draft_bls_pubkey_encoding.md)
- EIP2334: [BLS12-381 Deterministic Account Hierarchy](https://github.com/ethereum/EIPs/blob/de52c7ef2e44f2ab95d6aa4b90245c3c969aaf9f/EIPS/eip-2334.md)
- EIP2335: [BLS12-381 Keystore](https://github.com/ethereum/EIPs/blob/376f2988fb735a96e213ebf97f349e40b4ce05ca/EIPS/eip-2335.md)

**Stuff for developers**

- [Starter kit repo for Typescript environment](https://hackernoon.com/the-new-solidity-dev-stack-buidler-ethers-waffle-typescript-706830w0) with Buidler, ethers.js and Waffle
- Embark [v5 alpha](https://github.com/embark-framework/embark/blob/master/CHANGELOG.md#500-alpha0-2019-10-28)
- Truffle [v5.0.43](https://github.com/trufflesuite/truffle/releases/tag/v5.0.43) all contract objects return transaction hash
- [Subspace v1.1](https://github.com/embark-framework/subspace/releases/tag/1.1.0) event tracking
- [dfuse](https://medium.com/coinmonks/whats-wrong-with-dapps-on-ethereum-68d666645848): indexing APIs to abstract away dealing with nodes
- MetaMask is [deprecating synchronous provider methods](https://medium.com/metamask/deprecating-synchronous-provider-methods-82f0edbc874b)
- [How to integrate ENS multicoin support](https://medium.com/the-ethereum-name-service/how-to-integrate-ens-multi-coin-support-into-your-wallet-for-developers-8d3a8a37d1eb) into your wallet
- [OpenZeppelin Contracts v2.4](https://forum.openzeppelin.com/t/openzeppelin-contracts-v2-4/1665)
- Using [Rimble’s React components to create a new Burner Wallet](https://medium.com/@MakingRimble/prototyping-a-new-burner-at-devcon-with-maker-rimble-64af185727eb)
- [ETHcode v0.0.6](https://medium.com/quanta-network/ethcode-update-v0-0-6-unit-testing-solidity-with-remix-tests-b51dddb06c41). unit testing with remix-tests
- Loopring [opensources its snark circuits](https://medium.com/loopring-protocol/loopring-open-sources-its-zksnark-circuit-code-53c934b67ce5) (and will do a trusted setup ceremony soon)
- Universal Login [developer beta is live on mainnet](https://medium.com/universal-ethereum/universal-login-beta-is-live-heres-how-you-can-apply-7386890c2e0d)
- ConsenSys Diligence [reviewed Vyper](https://diligence.consensys.net/blog/2019/10/vyper-preliminary-security-review/), found bugs, says it is not ready for production
- [Samsung unveils its Ethereum SDK](https://news.samsung.com/global/developers-and-users-get-more-out-of-blockchain-with-samsung-blockchain-platform-sdk)

**Ecosystem**

- [30 days of ETH shipping](https://concourseopen.com/blog/30-days-of-eth-october-2019/), an October retrospective
- [Sync across Metamask devices with 3Box](https://medium.com/3box/how-metamask-backs-up-wallet-data-using-3box-storage-c90a34f9e56f).
- Infura’s [open architecture initiative](https://blog.infura.io/building-better-ethereum-infrastructure-48e76c94724b)
- Hayden Adams’ [Uniswap inception story](https://medium.com/@hayden_41532/uniswap-birthday-blog-v0-7a91f3f6a1ba)
- [Has DeFi made Eth unforkable](https://medium.com/dragonfly-research/ethereum-is-now-unforkable-thanks-to-defi-9818b967738f)? Apps certainly complicate contentious forks.

**Enterprise**

- A [technical analysis of Ethereum vs Fabric vs Corda](https://kaleido.io/a-technical-analysis-of-ethereum-vs-fabric-vs-corda/?utm_campaign=Newsletter&utm_medium=email&_hsenc=p2ANqtz--Z9rgow-603BNKIlxpij4IiFwYEk2tsUle0-HmQAp_THJEun0GgAXFtiTTw0vOq7CnzHP9_j4QxnYeaWYcKhPgXN8ZJUi5-Pj_43s9WHnx5bjgPRQ&_hsmi=78794657&utm_content=78794657&utm_source=hs_email&hsCtaTracking=e3622fc6-256b-4c01-a1b3-ecc937eba194%7Cb42a5916-2e8d-4282-ba4f-1699c9c9f698)
- [Ensure uptime with PegasysPlus](https://pegasys.tech/how-to-ensure-uptime-with-advanced-monitoring-in-pegasys-plus/)

**Application layer**

- bZx’s [Torque is live](https://medium.com/bzxnetwork/torque-is-live-a-step-by-step-guide-to-the-most-powerful-decentralized-borrowing-platform-on-21139dc6abce). Fixed rate, indefinite term loans, as long as you stay collateralized.
- Dharma’s [smart wallet live](https://www.reddit.com/r/ethfinance/comments/dm3h23/dharma_is_live_to_the_public/) on top of Compound
- Codefi’s [DeFi scoreboard](https://defiscore.io/) getting live updates
- [Maple](https://medium.com/maple-finance/introducing-maple-1e160ab0bcef): use cDai as collateral for tranched CDOs, so you can lock in fixed rates.
- Livepeer’s [Streamflow is on testnet](https://medium.com/livepeer-blog/livepeers-public-streamflow-testnet-is-now-live-45b8fb500932). Miners can test how little getting paid to transcode video will affect their hashrate. It also has probabilistic micropayments, for those looking for a layer2 alternative.
- [Details on The LAO](https://medium.com/@thelaoofficial/the-lao-an-early-sneak-peek-a0c9be66a3ae): TheDAO returns wrapped in a Delaware LLC with 10 founding members + 90 from public sale, using an extended MolochDAO
- Decentralized [note taking app using your Eth address and 3Box](https://medium.com/@KamesCG/esence-dbb3a6ced578)
- [Overview of 0x v3](https://blog.0xproject.com/0x-the-community-owned-liquidity-api-26da5732447e) ahead of the weeklong vote that starts Nov 4th
- [With MCD, some Maker terms change](https://blog.makerdao.com/say-goodbye-to-cdps-and-hello-to-maker-vaults/). CDP -> Vault. Dai-> Sai. MCD -> Dai (what we’ve been calling Dai was always Sai).
- Dai Stability Fee is [now 5.5%](https://twitter.com/nanexcool/status/1188812875013459969)

**Tokens / Business / Regulation**

- The [Tether Flippening](https://twitter.com/AlexanderFisher/status/1189209147117576200) occurred this week.
- Raining on that parade: Stripe’s Patrick McKenzie says “[Tether is the internal accounting system for the largest fraud since Madoff](https://www.kalzumeus.com/2019/10/28/tether-and-bitfinex/)”
- Seeking [uniform valuation for crypto](https://medium.com/@HASHCIB/seeking-uniform-valuation-for-crypto-34df2f106e60)
- [Aditya Asgaonkar’s game theory evaluation of TCRs](https://arxiv.org/pdf/1809.01756.pdf). Or [slides](https://docs.google.com/presentation/d/1bN4a80wlWDYxOczmxgJck3rQSdNEfQJGb2lMI15Z__w/edit), if you prefer those to academic papers.

**General**

- Coinmetrics finds the [ASICs in nonce distributions](https://coinmetrics.substack.com/p/coin-metrics-state-of-the-network-04a). ASICs were mining ETH before they shipped
- Binance charged [Blockstack $250k for a listing](https://www.theblockcrypto.com/post/44837/binance-accepted-250000-to-list-blockstacks-token-despite-claiming-there-was-no-listing-fee)
- EPIC FAIL: [BitMEX leaks majority of user emails](https://www.theblockcrypto.com/post/45487/bitmex-exposes-some-users-email-ids-to-other-users-affecting-their-privacy) by putting them in the “to” field
- Data analytics firm Splunk used [Burner Wallet/xDai for a 10k person popup economy](https://www.splunk.com/blog/2019/11/01/splunk-unveils-buttercup-bucks-at-conf19.html) at their conference

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Nov 5-6 - [Decentralized insurance D1Conf](https://blog.etherisc.com/d1conf-2019-to-focus-on-blockchain-adoption-november-5-6th-in-malta-3b8b582ac7b4) (Malta)
- Nov 7 - [web3 UX unconference](http://ux.conflux.network/#/) (Toronto)
- Nov 8-10 - [ETHWaterloo](https://ethwaterloo.com/)
- **Nov 18 - [Multi-collateral Dai](https://blog.makerdao.com/breaking-launch-date-of-multi-collateral-dai-announced-at-devcon-5/)**
- **Dec 4 - Istanbul network upgrade**
- Jan 1 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff-update/)
- Feb 9-15 - [EthLagos](https://ethlagos.io/)
- Feb 14-16 - [ETHDenver](https://www.ethdenver.com/)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

It’s amazing to me how many people email me when every issue has a link at the bottom saying not to email me to get in the newsletter.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **I want your links: [weekinethereumnews.com](https://weekinethereumnews.com/)**

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/week-in-ethereum-news-november-3-2019/](https://weekinethereumnews.com/week-in-ethereum-news-november-3-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

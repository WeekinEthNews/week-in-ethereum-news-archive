---
title: "Week in Ethereum News <BR> March 14, 2021"
date: "2021-03-14"
---

## **Eth News and Links**

**Mainnet**

- [Berlin upgrade fork is happening](https://blog.ethereum.org/2021/03/08/ethereum-berlin-upgrade-announcement/): Ropsten forked this week relatively uneventfully (found a small Besu issue). Reminder: EIPs are 2565 (lowers cost of ModExp precompile), 2718 (typed transaction envelope), 2929 (anti-DOS measure to increase gas costs for state access), and 2930 (optional access lists, mitigates some 2929 gas increases)
- Update your clients! Latest Berlin-ready client releases: Besu [v21.1.1](https://github.com/hyperledger/besu/releases/tag/21.1.1), Geth [v1.10.1](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.1), Nethermind [v1.10.41](https://github.com/NethermindEth/nethermind/releases/tag/1.10.41), OpenEthereum [v3.2](https://github.com/openethereum/openethereum/releases/tag/v3.2.0)
- Restesteth (test generator) [v0.1](https://github.com/ethereum/retesteth/releases/tag/v0.1.0-accesslist) with access lists
- Why we should do [verkle trees and per-epoch state expiry](https://hackmd.io/@HWeNw8hNRimMm2m2GH56Cw/state_expiry_paths) together
- EVM [object format](https://notes.ethereum.org/@axic/evm-object-format), alternative to EVM versioning and BEGINDATA
- [Account abstraction](https://github.com/flashbots/pm/issues/24) via flashbots?
- Vitalik’s [history of ideas that never made it in](https://www.reddit.com/r/ethereum/comments/m4ftnv/some_technical_proposals_that_were_considered_for/): async only, automated load balancing shards, SSTORE big objects in one slot, parallel execution

**EIPs/Standards**

- [ERC3345](https://github.com/ethereum/EIPs/blob/ab47267999dab7aaf09580ca7d18a415bacb9879/EIPS/eip-3345.md): Call chaining standard
- [ERC3361](https://github.com/ethereum/EIPs/blob/75733a015350518c622484d20e0fc2dcd5a94598/EIPS/eip-3361.md): JSON-RPC method to sign Ethereum messages
- [EIP3369](https://github.com/ethereum/EIPs/blob/f4c510a3d657e77b42fd8afe11f7731ff03532e9/EIPS/eip-3369.md): Brick current ASICs with minor Ethash mod
- [EIP3368](https://eips.ethereum.org/EIPS/eip-3368): increase block rewards

**Proof of Stake (stakers: update your Ethereum mainnet clients for Berlin)**

- Latest [proof of stake](https://youtu.be/s017DQlsCCw?t=302) call. Notes from [Alex Stokes](https://twitter.com/ralexstokes/status/1370027668960284677) and [Ben Edgington](https://hackmd.io/@benjaminion/HkIXJsDmd): lots of client updates, first upgrade named Altair, new Prater devnet, improving fork choice discussion, and talk about going full proof of stake for Ethereum
- Mikhail Kalinin’s [spec to end proof of work](https://github.com/ethereum/eth2.0-specs/pull/2229) in pull release form
- A quick and dirty method to [end PoW on an accelerated timeframe](https://notes.ethereum.org/@vbuterin/B1mUf6DXO) by running mainnet nodes and PoS nodes and modifying fork choice on the mainnet nodes
- How [exchanges get much better security than PoW chains](https://ethresear.ch/t/high-confidence-single-block-confirmations-in-casper-ffg/8909) even without finality in Casper FFG.
- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210313): the rush to turn off PoW?

**Layer2**

- Explaining StarkEx’s [conditional transactions](https://medium.com/starkware/conditional-transfers-the-key-to-interoperability-2e1de044fb65) for fast withdrawals from l2 to l1
- A practical example of the [difference between l2 and sidechains](https://gourmetcrypto.substack.com/p/layer-2-for-beginners)

* * *

### **This newsletter is made possible thanks to Celer!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

[Celer](http://celer.network/) is a coherent layer-2 scaling platform on Ethereum powered by [Generalized State Channel Network](https://www.celer.network/docs/celercore/index.html) and [Rollup](https://medium.com/celer-network/adding-hybrid-pos-rollup-sidechain-to-celers-coherent-layer-2-platform-d1d3067fe593) technology.

Celer recently announced [Layer2.finance](https://layer2.finance/), a layer-2 rollup-based DeFi aggregator that acts as a low-cost and trust-free gateway for the users to explore and benefit from the existing DeFi ecosystem with 100X lower-cost. Layer2.finance achieves scalability “in-place” with no protocol migration needed and therefore, does not cause liquidity fragmentation or break composability. Layer2.finance is launching in March.

Follow Celer on [twitter](https://twitter.com/CelerNetwork), [blog](https://blog.celer.network/), [discord](https://discord.com/invite/Trhab5w) and [telegram](https://t.me/celernetwork).

* * *

**Stuff for developers**

- OpenZeppelin [Sentinel monitoring](https://blog.openzeppelin.com/introducing-sentinels/) and alerting
- Reimplementing Nexus Mutual’s [bonding curve implementation](https://medium.com/nexus-mutual/our-bonding-curve-has-been-improved-e6d9d0cec7d1) to prevent high MCR vulnerability
- [Scaffold-eth and optimism](https://azfuller20.medium.com/optimism-scaffold-eth-draft-b76d3e6849e8) starter pack
- [Harmony](https://github.com/itzmeanjan/harmony): open source transaction pool explorer
- [Ape Safe](https://twitter.com/bantg/status/1368650716076769281): preview GnosisSafe transactions from local mainnet fork
- wighawag updates boilerplate for [Solidity contract development](https://twitter.com/wighawag/status/1369019735896186889)

**Security/incidents**

- Dodo [hacked for 2.1m](https://www.rekt.news/au-dodo-rekt/) from an unprotected init
- One Zerion user gets hit for $30k due to [fake Balancer pool in interface](https://blog.zerion.io/post-mortem-on-zerions-asset-phishing-attack-4fa9516414a3), so now Zerion checks pools against Balancer code on chain
- The [private key got compromised to Roll’s hotwallet](https://twitter.com/tryrollhq/status/1371179318496354304), with the hacker selling Roll’s portion (~$6m) of personal tokens

**Ecosystem**

- GPUs can transcode video on Livepeer with nearly zero loss in hashpower ([2 old GPUs made almost $1000 in a month](https://hackernoon.com/i-earn-dollar1000-a-month-using-my-old-nvidia-gpus-a-how-to-guide-vj7833be)?)
- Vitalik: making the [ecosystem more friendly to light clients](https://www.reddit.com/r/ethereum/comments/m0tqz5/making_the_ecosystem_more_lightclient_friendly/)
- You can now [backup your TornadoCash deposits onchain](https://tornado-cash.medium.com/tornado-cash-adds-on-chain-deposit-backups-dbef9ac9e61d) (but not with hardware wallets)

**Enterprise**

- Quorum [v21.1](https://consensys.net/blog/quorum/consensys-quorum-21-1-0-features-enhanced-ethereum-mainnet-compatibility/) - makes it easier to launch mainnet, new db format with lower storage and better performance

**Application layer**

- Beeple everyday collage [sells for $69.3m at Christie’s](https://twitter.com/ChristiesInc/status/1370436536626511879) to MetaKovan
- Dylan Field’s [statement on selling Cryptopunk 7804](https://www.youtube.com/watch?v=hb5LapixLbk&t=3236s) for ~$7.5m
- [TacoBell selling NFTs](https://twitter.com/tacobell/status/1368807880434982912) on Rarible
- [Aphex Twin selling NFTs](https://foundation.app/AphexTwin) on Foundation
- Digging up old cryptocollectibles from a few years ago was a thing this week: Cryptocats, Mooncats, Etheria (no links)
- Golem is back with a new version of [Golem running on zkSync](https://blog.golemproject.net/mainnet-release-beta-i/)
- Democracy Earth’s [universal basic income](https://blog.kleros.io/proof-of-humanity-an-explainer/) for proof of humanity
- [Etherplay to return](https://etherplay.medium.com/etherplay-is-back-de0d848d2859) on a rollup

**Regulation/business/tokens**

- Binance is being [investigated by the CFTC](https://www.bloomberg.com/news/articles/2021-03-12/crypto-exchange-binance-investigated-by-u-s-over-who-s-trading), per Bloomberg
- JP Morgan designing a [basket of public equities with indirect crypto exposure](https://www.theblockcrypto.com/linked/97815/jpmorgan-crypto-public-companies-basket-document-sec)
- Lucius Fang’s [deep dive into decentralized insurance](https://www.coingecko.com/buzz/decentralized-insurance-deep-dive)
- A protocol merger? [Keep and NuCypher in discussions](https://twitter.com/mhluongo/status/1368963503663513606)
- Linda Xie: A [beginner’s guide to DAOs](https://linda.mirror.xyz/Vh8K4leCGEO06_qSGx-vS5lvgUqhqkCz9ut81WwCP2o)

**General**

- What your [browser sends home to centralized servers about you](https://brave.com/popular-browsers-first-run/) when you first startup the browser
- [Malware delivered via URL due to website and adtech syncs](https://mediatrust.com/blog/march-2021-digital-trends-user-sync-hijackings) (ahem: why you should block ads with Brave)
- [CVE-2021-21300](https://lwn.net/Articles/848893/): Update your git release

* * *

## **Job Listings**

- Nomic Labs is hiring a [senior dev and an engineering manager](https://www.notion.so/Nomic-Labs-jobs-991b37c547554f75b89a95f437fd5056)
- [Powerloom Protocol](https://powerloom.io/) is looking for [Distributed Systems Engineers](https://angel.co/company/powerloom/jobs) in Bangalore
- Build the future with [ChainSafe](https://chainsafe.io/careers/openpositions). [Rust](https://chainsafe.io/careers/openpositions/rust-developer), [Golang](https://chainsafe.io/careers/openpositions/lead-golang-developer), [Solidity](https://chainsafe.io/careers/openpositions/solidity-engineer), [TS Devs](https://chainsafe.io/careers/openpositions/ethereum-typescript-developer) needed!
- [Props](https://www.propsproject.com/): [Senior Marketing Manager](https://www.propsproject.com/careers?gh_jid=2954767), [Director of Finance](https://www.propsproject.com/careers?gh_jid=2933297) and [Marketing Intern](https://www.propsproject.com/careers?gh_jid=2954773).
- DeFi hub of Polkadot - [Acala](https://acala.network/jobs) is hiring [Solidity](https://jobs.lever.co/acala/e21fa149-101d-4f94-997e-f1f9414cbd56), [Rust](https://jobs.lever.co/acala/3c16081e-b40c-473c-aaaa-a761aac07a70) and [Fullstack](https://jobs.lever.co/acala/c5ff6bb8-79db-4373-b3c4-4ec369a29799) devs.
- Week in Ethereum News is [looking for an editor](https://twitter.com/evan_van_ness/status/1370826680420417536).

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-march-14-2021/](https://weekinethereumnews.com/week-in-ethereum-news-march-14-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Mar 19-21 - ETHGlobal’s [NFT Hack](https://nft.ethglobal.co/)
- Mar 25 - [Gitcoin CLR matching grants](https://gitcoin.co/grants/) round **ends** (ahem: [Week in Eth News](https://gitcoin.co/grants/237/week-in-ethereum-news))
- Apr 9 - May 14 - ETHGlobal’s [Scaling Ethereum](https://scaling.ethglobal.co/) hackathon
- April 14 - [Berlin upgrade fork](https://github.com/ethereum/pm/issues/248#issuecomment-782069875) (testnets: Ropsten Mar 10, Goerli Mar 17, Rinkeby Mar 24)
- April 16 - [Rollup community grant](https://esp.ethereum.foundation/en/rollup-grants/) applications due
- April 22 - [Ethereum in the Enterprise 2021](https://www.conference2021.entethalliance.org/)
- May 14 - papers due for [WoSCA 2021](https://trailofbits.github.io/WoSCA/)
- Jul 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

---
title: "Week in Ethereum News <BR> Jan 18, 2021"
date: "2021-01-18"
---

## **Eth News and Links**

**Eth1**

- All the cool [protocol changes happening in 2021](https://twitter.com/lightclients/status/1349169327769931776)
- Latest [1559 implementer call](https://www.youtube.com/watch?v=KllIW2hqw2I). Beiko’s [notes](https://twitter.com/TimBeiko/status/1349788674334945282)
- [Transaction pool sorting](https://hackmd.io/@adietrichs/1559-transaction-sorting-part2) with 1559
- [Block variance in 1559](https://notes.ethereum.org/@vbuterin/eip_1559_spikes) is fine
- Barnabé’s [notebook simulating the transition to 1559](https://github.com/barnabemonnot/abm1559/blob/master/notebooks/transition1559.ipynb)
- [Basefee manipulation](https://medium.com/nethermind-eth/the-manipulation-of-the-basefee-in-the-context-of-eip-1559-4b082898271c) simulations in 1559
- A [list of 1559 resources](https://hackmd.io/@timbeiko/1559-resources)
- Piper: how to get [functional light clients](https://snakecharmers.ethereum.org/the-winding-road-to-functional-light-clients/), [part 2](https://snakecharmers.ethereum.org/the-winding-road-to-functional-light-clients-part-2/), [part 3](https://snakecharmers.ethereum.org/the-winding-road-to-functional-light-clients-part-3/)
- Alexandra [state network update](https://snakecharmers.ethereum.org/alexandria-dev-update-4/): successful 20 node testnet serving 1m block headers

**Eth2**

- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news). The chain “could hardly be running better.” Upgrade in ~6 months to fine-tune and reset slashing penalties.
- Latest [eth2 implementer call](https://youtu.be/xNt6MmEV3JI?t=131). Ben Edgington’s [notes](https://hackmd.io/@benjaminion/BJ2TO360v). Discussion of what goes into the first eth2 upgrade.
- [Ethstaker video with Danny Ryan](https://www.youtube.com/watch?v=mRn-nxq8yF4): turning off PoW is closer than expected and probably the priority before sharding
- [eth2 issuance](https://www.attestant.io/posts/exploring-net-issuance/): it’s quite low overall and about 95% of the theoretical maximum
- Why is my [attestation reward negative if the attestation was immediately included](https://www.symphonious.net/2021/01/10/exploring-eth2-attestation-rewards-and-validator-performance/)?

**Layer2**

- [Optimism soft launches](https://medium.com/ethereum-optimism/mainnet-soft-launch-7cacc0143cd5) with [Synthetix, who is rolling out their optimistic rollup transition](https://blog.synthetix.io/the-optimistic-ethereum-transition/) in five phases
- You can [now transfer to any Eth address on Loopring](https://twitter.com/loopringorg/status/1349427566319456264) even if they haven’t yet enabled the zk-rollup
- [Connext Vector](https://medium.com/connext/vector-0-1-0-mainnet-release-9496ae52c422) launches cross-layer2 routing network

* * *

### **This newsletter is made possible thanks to Celer!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

[Celer](http://celer.network/) is a coherent layer-2 scaling platform on Ethereum powered by [Generalized State Channel Network](https://www.celer.network/docs/celercore/index.html) and [Hybrid Rollup](https://medium.com/celer-network/adding-hybrid-pos-rollup-sidechain-to-celers-coherent-layer-2-platform-d1d3067fe593) technology. Celer has just published [a review](https://blog.celer.network/2021/01/17/celer-network-2021-update-to-a-better-future/) on the technology and adoption achievements in 2020 and the roadmap update in 2021. Follow Celer on [twitter](https://twitter.com/CelerNetwork), [blog](https://blog.celer.network/), [discord](https://discord.com/invite/Trhab5w) and [telegram](https://t.me/celernetwork).

* * *

**Stuff for developers**

- [Metamask provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-are-here-7b11c9388be9) are live
- [ethers-rs v2](https://github.com/gakonst/ethers-rs/)
- [Restless](https://medium.com/ethworks/introducing-restless-validations-for-ts-ethereum-and-express-js-ec2ef55b0005), simple validation library for express.js and Ethereum
- [Using Smock](https://soliditydeveloper.com/smock) to mock contracts in Hardhat
- Tutorial on [deploying governance with Hardhat](https://github.com/withtally/Tutorial-Deploy-Governance)

**Security/incidents**

- EthGlobal’s [DeFi exploits panel](https://youtu.be/Df2zzfoTfMc) video
- Maurelian finds a bzx-style [batchTransfer vulnerability in the Sandbox](https://medium.com/sandbox-game/the-sandbox-asset-smart-contract-security-update-a465fd6345e8)

**Ecosystem**

- [Cloudflare to run the eth.link resolver](https://blog.cloudflare.com/cloudflare-distributed-web-resolver/)

**Application layer**

- [Notional finance](https://medium.com/notional-finance/notional-launches-out-of-beta-beeec5d69fe0) fixed-rate loaning launches on mainnet
- Yield has [fixed-rate, fixed-term loans for Maker](https://medium.com/yield-protocol/fixed-rate-loans-for-makerdao-users-c652b4186caa) using flash loans
- Personal tokens this week from techno DJ [Carl Cox](https://twitter.com/Carl_Cox/status/1349325324706664453), Rick and Morty creator [Justin Roiland](https://twitter.com/niftygateway/status/1349506514030108672), indie rockers [Portugal the man](https://twitter.com/portugaltheman/status/1349763357994192897), and DJ [3LAU](https://twitter.com/3LAU/status/1350893555397509120)
- Cream’s [Ironbank](https://medium.com/@CreamdotFinance/introducing-the-iron-bank-bab9417c9a) - protocols get whitelisted and then can borrow up to credit limit without collateral
- 1559 will allow Oiler to create [native gas price derivatives](https://medium.com/oiler-network/oiler-research-eip-1559-basefee-manipulations-6de2d177bd66)
- Stablecoin designs: [Fei](https://medium.com/fei-protocol/introducing-fei-protocol-2db79bd7a82b), a dollarcoin collateralized by ETH on a bonding curve
- [Coinbase, Kraken, Binance and Gemini users can buy cover](https://twitter.com/roxdanila/status/1348957143240732689) for custody risk on Nexus Mutual

**Regulation/business/tokens**

- Mnuchin gives up and [punts proposed wallet regulations to Biden administration](https://www.fincen.gov/news/news-releases/fincen-extends-comment-period-rule-aimed-closing-anti-money-laundering)
- OCC allows [Anchorage to become a bank](https://www.occ.gov/news-issuances/news-releases/2021/nr-occ-2021-6.html)
- OCC head Brian Bondy: [get ready for selfdriving banks](https://archive.is/wvInk)
- Must be a bull market: [GoldmanSachs crypto custody is back](https://www.coindesk.com/goldman-sachs-to-enter-crypto-market-soon-with-custody-play-source)
- Andre Cronje’s [defi sucks rant](https://andrecronje.medium.com/building-in-defi-sucks-part-2-75df9ee7871b) about community and value

**General**

- Be careful what [apps you download in an app store](https://medium.com/mycrypto/malicious-crypto-apps-are-ramping-up-on-google-play-7bd60ebcb8d1), fake apps on rise again. Remember: [phone numbers in crypto considered harmful](https://twitter.com/evan_van_ness/status/1350126333209272333).
- [Readable Eth transactions](https://blog.gridplus.io/readable-ethereum-transactions-a-new-standard-945c5e9ef2c7) on a hardware wallet with the GridPlus Lattice
- [Ledger has another data leak](https://twitter.com/Ledger/status/1349375083891011591) via Shopify
- [Censorship resistance and responsibility](https://petkanics.medium.com/live-video-censorship-resistance-and-responsibility-c6bc772db6d3), viewed from the Livepeer lens

* * *

## **Job Listings**

- Trail of Bits is looking for a [technical editor/writer](https://jobs.lever.co/trailofbits/8bf936ff-b86c-462e-80b2-4d58004bc68d) & [security engineer](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf)
- Nexus Mutual: [experienced Solidity dev](https://angel.co/company/nexus-mutual-1/jobs/967538-smart-contract-engineer) in Euro timezones
- 0x looking for [devs of all types](https://0x.org/about/jobs) and a [Matcha marketing manager](https://boards.greenhouse.io/0x/jobs/4923909002)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) on Twitter.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-jan-18-2021/](https://weekinethereumnews.com/week-in-ethereum-news-jan-18-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Jan 22 - Feb 21 - EthIndia’s [EtherPunk](https://etherpunk.devfolio.co/) hackathon
- Feb 5-12 - [EthDenver](https://www.ethdenver.com/) (virtual)
- Mar 5 - Financial Cryptography [DeFi academic workshop](https://fc21.ifca.ai/defi/)
- Apr 6-8 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

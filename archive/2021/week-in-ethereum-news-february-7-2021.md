---
title: "Week in Ethereum News <BR> Feb 7, 2021"
date: "2021-02-07"
---

## **Eth News and Links**

**Eth1**

- Latest [core devs call](https://youtu.be/ju92hAKzKcg?t=217). Beiko’s [notes](https://twitter.com/TimBeiko/status/1357685104416460803): ephemeral yolov3 testnet launched, Berlin testnet tentatively Feb 24, aiming at Berlin fork in late q1/early q2, eth/66 discussion, EVM384/precompile discussion
- A call for [devs interested in light clients and stateless Ethereum](https://snakecharmers.ethereum.org/wanted-monkey-trainer-pedestal-builders-need-not-apply/)

**Eth2**

- [Workshop](https://youtu.be/uGeIDNEwHjs?t=512) video for merging mainnet with proof of stake as well as data shards
- Afri [benchmarks the eth2 clients](https://dev.to/q9/ethereum-2-0-mainnet-clients-3and). Headline: “I would consider all of them production-ready”
- Staked got [slashed from running redundancies](https://blog.staked.us/blog/eth2-post-mortem). Never run two machines with same staking key and never disable slashing protection!
- [Spectroscope](https://github.com/neukind/spectroscope): eth2 node monitoring tool

* * *

### **This newsletter is made possible thanks to [Chainlink](https://chain.link/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/05/FE39n5_g.png)

Chainlink Labs is hiring! [Explore our open roles](http://chn.lk/careers) and come join us in accelerating the adoption of Chainlink's decentralized oracle network and universally connected smart contracts.

**Stuff for developers**

- OpenZeppelin Contracts [v3.4](https://blog.openzeppelin.com/openzeppelin-contracts-3-4): erc777 security fix, virtual view functions, erc20 permit, beacon proxy, minimal proxy
- Latest [Truffle releases add lots of Vyper support/](https://github.com/trufflesuite/truffle/releases/tag/v5.1.65)features
- Vertigo [v1.3](https://github.com/JoranHonig/vertigo/releases/tag/v1.3.0), mutation testing framework now works with Hardhat
- Latest [vscode solidity adds "import" autocomplete](https://twitter.com/juanfranblanco/status/1357267332712775680) support
- [App storage pattern for state variables](https://dev.to/mudgen/appstorage-pattern-for-state-variables-in-solidity-3lki) in Solidity
- Austin Griffith’s [flash loans intro](https://github.com/austintgriffith/scaffold-eth/tree/flash-loans-intro)

**Security/incidents**

- [yearn got hacked](https://github.com/iearn-finance/yearn-security/blob/master/disclosures/2021-02-04.md) via flashloans depegging oracle for 11m DAI, yearn stopped it while in progress and saved ~70% of the DAI. Some safeguard shields had been lowered to encourage moving to v2. A [walkthrough of the attack](https://twitter.com/FrankResearcher/status/1357464851531116544)
- [Dedaub finds a DeFlast vulnerability](https://medium.com/dedaub/look-ma-no-source-hacking-a-defi-service-with-no-source-code-available-c40a6583f28f) by decompiling the closed source code and finding it lacked safeguards
- [Artifact minting exploit](https://blog.zkga.me/artifact-minting-exploit) via randomness in Dark Forest game
- Petty: [what is a security audit and how should you prep for it](https://our.status.im/what-is-a-security-audit-when-you-should-get-one-and-how-to-prepare/)?
- [Writing your code properties](https://consensys.net/diligence/blog/2021/02/4-effective-strategies-to-come-up-with-scribble-annotations) with Scribble
- ArmorFi massive bug bounty pays off as [Alexander Schlindwein found a vulnerability](https://twitter.com/ArmorFi/status/1356784271923503108) and got a (mostly vested) 7 figure payout
- Echidna [v1.6.1](https://github.com/crytic/echidna/releases/tag/v1.6.1), Eth code fuzzer now allows using compiler metadata to detect which contracts are deployed and performance optimizations for reverts

**Ecosystem**

- Ethereum crossed [1 billion transactions](https://twitter.com/etherscan/status/1357750257795297281) this week
- [Gasnow.org](https://www.gasnow.org/) adds historical data on gas price for the last week by hour/day
- Micah Zoltu: [how Eth governance functions](https://medium.com/coinmonks/how-ethereum-governance-works-71856426b63a)
- Noyes: what is [MEV](https://research.paradigm.xyz/MEV), how much is there, where are we now and tomorrow, and 1559 helps mitigate it
- epheph’s [MEV of the week](https://twitter.com/epheph/status/1357089176898969600). Another [example of the Flashbots tools](https://twitter.com/andrekorol1/status/1358252320207876104)
- [Umbra stealth payments](https://twitter.com/UmbraCash/status/1356677825005240324) aiming to be on mainnet in a couple months

**Enterprise**

- In early 2022, [Visa to issue a card](https://www.forbes.com/sites/michaeldelcastillo/2020/12/02/visa-partners-with-ethereum-digital-dollar-startup-that-raised-271-million/?sh=fc8988a4b1f5) for businesses to transact directly in USDC. I checked: ~99% of USDC is on Ethereum.
- EY and BSN partnering to deliver its [Ethereum OpsChain product in China](https://twitter.com/pbrody/status/1356780086590984193)
- EEA’s [dev tool survey results](https://entethalliance.org/eea-ethereum-developer-tool-survey-results/)
- Setup a [Clique POA network with Nethermind](https://medium.com/nethermind-eth/clique-poa-private-network-with-nethermind-6cfa21e43a51)
- [IBM Blockchain cut to zero](https://www.coindesk.com/ibm-blockchain-revenue-misses-job-cuts-sources). Never bet against Ethereum.

**Application layer**

- Linkin Park’s Mike Shinoda is selling a [crypto art NFT on Zora](https://twitter.com/mikeshinoda/status/1358090976414236674)
- Gas fees are high, Uniswap still at [record number of traders](https://twitter.com/teo_leibowitz/status/1357768977536147459)
- Short Bitcoin without having to short Bitcoin: [short Bitcoin dominance on UMA](https://medium.com/uma-project/bitcoin-dominance-on-uma-announcing-the-domination-finance-team-e2d8501a1f82)
- Balancer [v2](https://medium.com/balancer-protocol/balancer-v2-generalizing-amms-16343c4563ff) in next few months, currently being audited: uses less gas, customizable AMM logic, better capital efficiency. Single vault holds all assets in Balancer
- Balancer is [partially reimbursing gas costs in select pools](https://medium.com/balancer-protocol/exchange-gas-reimbursements-8326db66cab2) for users of its UI
- [How to short using Synthetix](https://blog.synthetix.io/how-to-short-using-synthetix/)
- Nexus Mutual can now [invest the mutual’s funds](https://medium.com/nexus-mutual/upgrade-investment-earnings-reduced-gas-fees-and-streamlined-architecture-724e1ced3af)
- [APwine](https://apwine.medium.com/our-beta-is-live-on-the-ethereum-mainnet-3860491a365c), tokenized future yield for Aave and Curve
- [Long dated options](https://primitivefinance.medium.com/the-longest-dated-options-in-defi-8b1605a275f0): Primitive says their September dated options are longest in Defi
- [ever.eth](https://medium.com/the-ethereum-name-service/everest-creates-on-chain-directory-of-kyc-and-humanness-with-ens-name-ever-eth-c22a94edacdb): Everest’s onchain directory of individual and entity KYC/data, where each record gets a subdomain
- [autem.eth](https://medium.com/@agusx1211/introducing-autem-eth-b76d2e08c761): a minimal wills and trusts app via dead man switch

**Regulation/business/tokens**

- Grayscale’s [Ethereum valuation thesis](https://grayscale.co/wp-content/uploads/2021/02/VALUING_ETHEREUM.pdf): ETH as money, ETH as consumable commodity, ETH as interest bearing asset
- CME’s ETH futures goes [live today at 6pm EST](https://www.cmegroup.com/trading/ether-futures.html)

**General**

- Status [compares what messengers can really see](https://our.status.im/private-messengers-what-can-they-really-see/). All the “private” messengers aren’t private.
- Attacking [OSS using abandoned resources](https://evilpacket.net/2021/attacking-oss-using-abandoned-resources/)
- Brave at [25m MAUs](https://brave.com/25m-mau/), more than doubling in a year
- [Chrome/Chromium 0day found](https://threatpost.com/google-chrome-zero-day-windows-mac/163688/). Immediately update your browser

* * *

## **Job Listing**

- [Showtime](https://twitter.com/tryshowtime), the NFT social network, is hiring for a [founding engineer](https://www.notion.so/showtimeinc/Showtime-Founding-Engineer-8b7d7053fd1a4418968bd3706ecbb6c2)
- [Pocket](http://pokt.network) is hiring a [developer growth lead](http://bit.ly/POKTEcosystemDev_GrowthLead) to supercharge dev adoption**←apply**
- Trail of Bits is looking for a [technical editor/writer](https://jobs.lever.co/trailofbits/8bf936ff-b86c-462e-80b2-4d58004bc68d) & [security engineer](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf)
- 0x looking for [devs of all types](https://0x.org/about/jobs) and a [data analyst](https://boards.greenhouse.io/0x/jobs/4220949002)
- Reddit: [Senior backend/Ethereum engineer](https://boards.greenhouse.io/reddit/jobs/2419120)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-feb-7-2021/](https://weekinethereumnews.com/week-in-ethereum-news-feb-7-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Feb **7** - [CME launches ETH futures](https://www.cmegroup.com/trading/ether-futures.html)
- **Feb 9 - [Stateless Ethereum call](https://snakecharmers.ethereum.org/wanted-monkey-trainer-pedestal-builders-need-not-apply/)**
- Mar 5 - Financial Cryptography [DeFi academic workshop](https://fc21.ifca.ai/defi/)
- **May 14 - papers due for [WoSCA 2021](https://trailofbits.github.io/WoSCA/)**
- Jul 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

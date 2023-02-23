---
title: "Week in Eth News <BR> October 4, 2020"
date: "2020-10-04"
---

## **Eth News and Links**

**Eth1**

- Geth [v1.9.22](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.22), bug fixes and a flag to override max gas price
- Weekly Turbogeth [alpha](https://github.com/ledgerwatch/turbo-geth/releases/tag/v2020.10.01). Much faster logs using roaring bitmaps.
    - Using the Turbogeth API, a UI to find [eth supply at any block](http://mandrigin.ru/eth-supply.html)
- Latest [core devs call](https://youtu.be/v5Q5WPdN1jk?t=71). Tim Beiko’s [notes](https://twitter.com/TimBeiko/status/1312021038130106370)
- [Transactions overhaul](https://notes.ethereum.org/@axic/Hyrc1i7ED) overview doc
- [block header sync in light clients](https://ethresear.ch/t/state-of-block-header-sync-in-light-clients/8047)

**EIPs/Standards**

- [3009](https://eips.ethereum.org/EIPS/eip-3009): Transfer With Authorization
- [3014](https://eips.ethereum.org/EIPS/eip-3014): Create `eth_symbol` method for JSON-RPC

**Proof of Stake launch**

- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_201002), the 2 year anniversary issue
    - “I believe the deposit contract deployment to be days, not weeks, away.”
- eth2 [quick update](https://blog.ethereum.org/2020/10/01/eth2-quick-update-no-18/)
    - Spadina showed we **need better client diversity**, so another dress rehearsal named Zinken
- [Eth2 client benchmarks](https://github.com/q9f/eth2-bench-2020-10)
- [SigmaPrime fuzzing](https://blog.sigmaprime.io/beacon-fuzz-08.html) found some slashing vulnerabilities and 2 bugs in blst library
- Latest [eth2 call](https://youtu.be/IRWQUQfq7yQ?t=103). Notes from [Ben](https://hackmd.io/@benjaminion/rkRaLS7Lv) and [Mamy](https://gist.github.com/mratsim/c5bc1d0e6ad11888d27d5db981f63a39)
- [Attack via time servers](https://ethresear.ch/t/eth2-attack-via-time-servers/8049) and mitigation
- Attestant wrote their own [validator client so they can switch](https://www.attestant.io/posts/introducing-vouch/) between eth2 nodes
- [secret shared validator PoC](https://github.com/dankrad/python-ssv)
- If you’re running in the cloud (not advised!), check out [Kotal](https://medium.com/coinmonks/multi-client-ethereum-networks-dcebb34d41f7) (switch clients and/or cloud providers easily) or 1 line helm/kubernetes cluster [command to switch between Nimbus/Lighthouse](https://github.com/eth2-clients/multinet)
- Pintail has the [first entry I’ve seen](https://github.com/bluepintail/medalla_analysis/blob/master/medalla_analysis.ipynb) to the Medalla data challenge

**Layer2**

- Rollups as “[fast pipes and smart VMs](https://www.lakshmansankar.com/#/fast-pipes-smart-vms)”
- Barry Whitehat on [sidechains vs layer2](https://ethresear.ch/t/understanding-sidechains/8045). Echos of [Georgios’ “sidechains are not layer2” tweetstorm](https://twitter.com/gakonst/status/1146793685545304064)
- Easy way to [run a Raiden node](https://medium.com/@raiden_network/the-easiest-way-to-try-out-a-full-raiden-node-16e54d32d6ca)
- The story of how [Geohot helped fix Optimism’s transpiler](https://twitter.com/jinglanW/status/1310718738417811459)

* * *

### **This newsletter is made possible thanks to Trail of Bits!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/05/2314423.jpeg)

Get immediate security help by booking an [office hours session](https://calendly.com/dan-trailofbits/office-hours) with Trail of Bits. In a 1 hour, 1-on-1 working session with an engineer from Trail of Bits, get help with your top security challenges and expert guidance to inform your approach.

* * *

**Stuff for developers**

- Solidity [v0.7.2](https://solidity.ethereum.org/2020/09/28/solidity-0.7.2-release-announcement/) - bugfix for free functions; adds compiler-generated utility file export. Expanded SMTChecker.
- [Jolly Roger](https://jolly-roger.eth.link/): wighawag’s Eth app with PWA frontend template
- [Damnvulnerabledefi.xyz](https://www.damnvulnerabledefi.xyz/): practice finding security holes
- [Solidity bytes library](https://github.com/GNSPS/solidity-bytes-utils/tree/0.1.0#important-fixes-changelog) had a bug in the slice method, please update
- [Testing with waffle v3](https://soliditydeveloper.com/waffle)
- [Solidity railroad grammar](https://sambacha.github.io/solidity-grammar-rrd/)
- abi to sol: generate [Solidity interface from ABI](https://github.com/gnidan/abi-to-sol)
- ethers-rs now has [rust implementation of secp256k1](https://twitter.com/gakonst/status/1311694465267126279)
- [NPM package to deploy to same address on EVM chains](https://twitter.com/PhABCD/status/1310652740331339778)
- [Coding a leaderboard](https://medium.com/coinmonks/create-and-deploy-an-ethereum-leaderboard-1ba60dba1495) tutorial in Solidity
- Breaking [Eth nodes with TeaTime](https://diligence.consensys.net/blog/2020/09/breaking-ethereum-nodes-with-teatime/); 34 RPC scans
- How [EMN got hacked](https://twitter.com/bkiepuszewski/status/1310901151311835136) this week using a flashloan
- Sam Sun finds [bug on Incognito’s bridge](https://we.incognito.org/t/how-a-smart-contract-vulnerability-was-discovered-and-fixed/6416)

**Ecosystem**

- A [rollup-centric Ethereum roadmap](https://ethereum-magicians.org/t/a-rollup-centric-ethereum-roadmap/4698). Vitalik argues that we should make some rollup-friendly changes to mainnet; launch sharding for data availability for rollups (phase 1), then swap out proof of work for proof of stake. This is all happening soon™, whereas phase2 is not close (and maybe not necessary?)
- It’s been clear for awhile that this was Eth’s roadmap: [eth2 is a rollup](https://lightclient.io/blog/eth2-is-a-rollup/)
- In September, [miners made more from fees than block rewards](https://www.theblockcrypto.com/linked/79452/ethereum-miner-revenue-september-gas-fees)
- An update on [Waku v2 messaging](https://vac.dev/waku-v2-update), moving to libp2p, better routing, more nodes
- Devcon Bogotá: [August 10-13, 2021](https://twitter.com/EFDevcon/status/1312074718002982912)

**Enterprise**

- [EY Opschain Network Procurement](https://www.prnewswire.com/news-releases/new-blockchain-based-ey-opschain-network-procurement-solution-helps-complex-enterprises-manage-spend-globally-301138679.html): e2e private enterprise procurement on mainnet using Baseline Protocol
- SEC Chairman Clayton says [all stocks could become tokenized](https://ledgerinsights.com/sec-chair-stocks-become-blockchain-tokens/)

**Application layer**

- [Uniswap’s volume exceeds Coinbase](https://www.theblockcrypto.com/linked/79775/uniswap-coinbase-monthly-volume-september) for the month of September
- Andre Cronje deployed some [test code for a game](https://mobile.twitter.com/AndreCronjeTech/status/1310763506170499072) from an address known to be his, and 15 million flooded in before a hacker found a bug and sent half back. Link in devs section for hack details.
- Augur: [foundry.finance](https://medium.com/sunrise-over-the-merkle-trees/how-to-use-augur-foundry-315f408c0d57) to easily provide liquidity to whether Trump will win, and a [Uniswap-like interface for end users](https://catnip.exchange/) to predict Trump or Biden
- Aggregator wars: [Matcha claims it has the best prices](https://blog.0xproject.com/a-comprehensive-analysis-on-dex-liquidity-aggregators-performance-dfb9654b0723), adjusted for transaction fees
- RAC’s $TAPE is the [most expensive cassette of all time](https://twitter.com/RAC/status/1311403650057527296). He’s also [giving out $RAC to his supporters](https://blog.ourzora.com/introducing-rac).
- DefiSaver adds [Aave liquidation protection](https://medium.com/defi-saver/aavetomation-is-now-live-with-automatic-liquidation-protection-and-leveraging-available-c5c293f3f16e)
- A new round of [Dark Forest is live](https://blog.zkga.me/dark-forest-v04). Now spawn to safe spaces; uses burner wallets.
- [Shield mining](https://medium.com/nexus-mutual/shield-mining-is-here-85067a30ab06): any token can incentivize Nexus Mutual staking so that there is more Nexus Mutual coverage for their project

**Regulation (“end of agency fiscal year” issue)**

- SDNY judge rules against [Kin in summary judgment](https://www.courtlistener.com/recap/gov.uscourts.nysd.516941/gov.uscourts.nysd.516941.88.0_2.pdf) (legal term for “Kin loses; not even close”)
- SEC forces Salt to [repay investors from q2 2017](https://www.sec.gov/litigation/admin/2020/33-10865.pdf) sale
- Bitmex charged by DOJ and CFTC for [money laundering and unlawful operation of an exchange](https://www.cftc.gov/PressRoom/PressReleases/8270-20)
- Americans are _de facto_ [no longer allowed to pay ransomware](https://home.treasury.gov/policy-issues/financial-sanctions/recent-actions/20201001)
- Venezuelan dictatorship attempts [Eth-based dex to circumvent US sanctions](https://www.coindesk.com/venezuela-rolls-out-ethereum-based-stock-exchange-to-help-skirt-us-sanctions)

**Business/tokens**

- Wax announces Eth bridge: “[Ethereum is best positioned to become the monetary system for all blockchains](https://medium.com/wax-io/coming-to-wax-a-new-wax-tokenomic-model-cd0616a069e9)”
- Arjun Balaji: [crypto market structure 3.0](https://arjun.af/crypto-market-structure)
- [Moats in crypto](https://www.varunsrinivasan.com/2020/09/29/crypto-moats)
- The [bull case for social tokens](https://bankless.substack.com/p/the-bull-case-for-social-tokens)
- Danger Zhang: [defi forks have been value acretive](https://thedefiant.substack.com/p/defi-forks-are-moving-beyond-copy)
- A [liquidity mining taxonomy](https://medium.com/bollinger-investment-group/liquidity-mining-a-user-centric-token-distribution-strategy-1d05c5174641)

**General**

- [Stark-based VDFs](https://ethresear.ch/t/stark-based-vdfs/8052)
- Brave is at [20m monthly active users](https://twitter.com/BrendanEich/status/1311829887011840000)
- [Life after losing crypto](https://medium.com/mycrypto/life-after-losing-crypto-737d1c17001f), a practical guide
- To help avoid losing crypto, learn [how to read audit reports](https://twitter.com/evan_van_ness/status/1312486580041392128)

* * *

## **Job Listings**

- Livepeer is hiring a [Blockchain Community Marketing + Ops Lead](https://angel.co/company/livepeer/jobs/874811-blockchain-public-network-community-marketing-associate)
- BnkToTheFuture is hiring a high performance dev team! Come [create the future](https://app.bnktothefuture.com/careers)!
- Collaborate with Chainlink’s incredible ecosystem as a [Marketing Director](https://chainlinklabs.com/careers#job-492239)
- Trail of Bits hiring elite [blockchain security engineers](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & [app security](https://jobs.lever.co/trailofbits/8b7f7fc1-efb0-4e89-b406-784c3a2d77e4)
- DeFi devs! Yield is hiring for Solidity and front-end – contact@yield.is
- 0x is hiring devs! [Full-stack, back-end, front-end or Solidity](https://0x.org/about/jobs)
- Celer Network: hiring Solidity and Go devs. Email: hiring@celer.network
- Nexus Mutual: [experienced Solidity dev](https://angel.co/company/nexus-mutual-1/jobs/967538-smart-contract-engineer); prefer European timezones

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **🥩 Staking pool questionnaire: October 15 🥩** 

My [questionnaire for staking pools](https://docs.google.com/document/d/1wrzKXff2XwY4Bu5ynVqvlPXI4xqM4-Hwx7Jh7_-1IGg/edit) will be due October 15th.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow the newsletter on twitter: [@WeekinEthNews](https://twitter.com/WeekInEthNews)

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-eth-news-october-4-2020/](https://weekinethereumnews.com/week-in-eth-news-october-4-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **Oct 12 - [Zinken eth2 dress rehearsal](https://github.com/goerli/medalla/blob/master/zinken/README.md) (deposits due by Oct 8)**
- Oct 19-26 - [EthLagos energy hackathon](https://ethlagos.io/)
- Oct 20 - [submission deadline for Medalla data challenge](https://ethereum.org/en/eth2/get-involved/medalla-data-challenge/)
- Oct 31 - [submission deadline for Underhanded Solidity Contest](https://underhanded.soliditylang.org/)
- Nov 6-7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)
- Nov 16 - [MetaMask Provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about)_ _**to receive it weekly**_

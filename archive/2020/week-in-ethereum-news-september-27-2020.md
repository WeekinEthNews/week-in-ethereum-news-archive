---
title: "Week in Eth News <BR> September 27, 2020"
date: "2020-09-27"
---

## **Eth News and Links**

**Eth1**

- OpenEthereum [release candidate for v3.1](https://github.com/openethereum/backport-3.1/tree/v3.1.0-rc.1). They have backtracked and will [continue to support Kovan](https://twitter.com/OpenEthereumOrg/status/1308388284519849984).
- [Snap sync in Geth benchmarking](https://twitter.com/peter_szilagyi/status/1309095486188670978) on Rinkeby
- Turbogeth [weekly alpha release](https://github.com/ledgerwatch/turbo-geth/releases/tag/v2020.09.04). They’re moving to a [modular architecture](https://github.com/AlexeyAkhunov/papers/blob/master/Turbo-Geth-Silkworm-architecture-plans.pdf), with the first [example of using Turbogeth as a library](https://github.com/mandrigin/turbo-api-examples/tree/master/cmd/mint)
- Tim Beiko’s [eip1559 fee market with burn update](https://hackmd.io/@timbeiko/1559-update-001): implementation, simulations, formal analysis, community input
- More [eip1559 agent based simulations](https://github.com/barnabemonnot/abm1559/blob/master/notebooks/strategicUser.ipynb) under various strategies in Jupyter notebook
- [Fuzzing the eip2537 BLS precompiles](https://medium.com/coinmonks/fuzzing-the-bls-precompiles-ba3728dec622)

**EIPs/Standards**

- [EIP2997](https://github.com/ethereum/EIPs/blob/ea8f361754f332562676f979e23ab35ba5af2898/EIPS/eip-IMPERSONATECALL.md): `IMPERSONATECALL` opcode
- [EIP3005](https://github.com/ethereum/EIPs/blob/7d443c72cc41c20948224a584534325323741281/EIPS/eip-3005.md): viability of batched meta transactions

**Eth2**

- [eth2 quick update](https://blog.ethereum.org/2020/09/22/eth2-quick-update-no-17/): deposit contract live for Sept 29 dress rehearsal testnet launch. “…everyone involved is making their final preparations for \[mainnet\] launch🚀”
- [Prysm client](https://medium.com/prysmatic-labs/eth-2-0-dev-update-56-getting-ready-for-spadina-ca79da0befd1) update. Implementing weak subjectivity, planning for forks

**Layer2**

- Optimism launches [optimistic rollup testnet](https://medium.com/@optimismPBC/light-at-the-end-of-the-tunnel-c390a05bbcb8) [incentivized by Synthetix](https://blog.synthetix.io/optimistic-ethereum-l2-testnet/)
- DxDAO is deploying a payment network [frontend to Loopring’s zkrollup](https://medium.com/rails-ethereums-layer-2/rails-a-new-l2-product-from-loopring-and-dxdao-enables-gas-free-ethereum-transfers-3975789a706d)

* * *

### **This newsletter is made possible thanks to [Celer](http://celer.network/)!**

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F0028ff3e-48a7-4fae-b912-f848e8908768_950x400.png)](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F0028ff3e-48a7-4fae-b912-f848e8908768_950x400.png)

[Celer](http://celer.network/) is a coherent layer-2 scaling platform on Ethereum powered by [Generalized State Channel Network](https://www.celer.network/docs/celercore/index.html) and [Hybrid Rollup](https://medium.com/celer-network/adding-hybrid-pos-rollup-sidechain-to-celers-coherent-layer-2-platform-d1d3067fe593) technology. Real money games, such as [Arcade Win](https://apps.apple.com/us/app/arcade-win/id1459895768) and [Daub Cash](https://apps.apple.com/us/app/daub-cash/id1513396754), built using [Celer's gaming-focused SDK](http://developer.celerx.app/) just reached top #10 ranking in App Store.We have also just launched [State Guardian Network beta testnet.](https://blog.celer.network/2020/08/10/state-guardian-network-beta-testnet-launches/) Follow us on [twitter](https://twitter.com/CelerNetwork), [blog](https://blog.celer.network/), [discord](https://discord.com/invite/Trhab5w) and [telegram](https://t.me/celernetwork).

* * *

**Stuff for developers**

- How to set up [Sentry and Pagerduty with Tenderly alerts](https://blog.tenderly.co/how-to-set-up-sentry-and-pagerduty-for-your-ethereum-dapp/) for your Eth app
- [NestJS Truffle box](https://github.com/ikhvost/truffle-nest-box)
- Create [time-locked functions](https://medium.com/cryptexglobal/how-to-create-time-locked-functions-523424def80) in Solidity with Builder
- Dealing with [“stack too deep” errors](https://soliditydeveloper.com/stacktoodeep)
- First level of a [game to learn Vyper](https://vyper.fun/#/1/introduction)
- Several [yearn vaults affected by bug](https://github.com/iearn-finance/yearn-security/blob/master/disclosures/2020-09-25.md) this week

**Frontrunning**

- A tale of Sam Sun, Scott Bigelow, Tina Zhen, SparkPool, and friends saving [10m in ETH from frontrunners](https://samczsun.com/escaping-the-dark-forest/). More [technical details of the bug from Lien](https://medium.com/lien-finance/interruption-of-service-incident-analysis-32077389c13)
- BlockNative releases a [transaction pool explorer](https://blog.blocknative.com/blog/explorer)
- ZenGo analyzes [generalized frontrunning attacks](https://medium.com/zengo/into-the-monsters-eye-analyzing-a-generalized-front-running-arbitrage-bot-attack-a4754145de0e)
- A closeup [examination of Uniswap frontrunning bots](https://medium.com/@mierzwik/how-to-munch-on-pickles-from-a-whale-dinner-edb5628cc769) in a large transaction

**Enterprise**

- Visa’s Plaid is [integrating with Dharma and Teller](https://www.coindesk.com/visa-owned-plaid-has-a-hidden-passion-for-defi)
- HongKong central bank’s [digitized international payments](https://consensys.net/blog/press-release/consensys-selected-by-hong-kong-monetary-authority-for-phase-two-of-project-inthanon-lionrock/) led by ConsenSys, whereas a prior version had used Corda.

**Application layer**

- [DeFi passed 10 billion](https://twitter.com/TrustlessState/status/1309273933217058816) with Maker and Uniswap nearly tied for #1. (Though data got backfilled putting TVL over 10b on Sept 12.)
- ICL arXiv paper studying [DeFi interest rates](https://arxiv.org/pdf/2006.13922.pdf) finds uncovered interest parity does not generally hold
- Vocdoni’s [voting as a service](https://blog.vocdoni.io/introducing-voting-as-a-service/)
- Aave is about to pass a [proposal to migrate LEND to AAVE](https://medium.com/aave/the-governance-is-in-your-hands-vote-on-the-first-aip-7037af6fcae1)
- [State of ENS 2020](https://medium.com/the-ethereum-name-service/state-of-the-ens-2020-cd8afa19f59d)

**Tokens/Business/Regulation**

- Proposed EU [framework for cryptoasset regulation](https://ec.europa.eu/finance/docs/law/200924-crypto-assets-proposal_en.pdf)
- OCC says [banks/thrifts can hold stablecoins](https://www.occ.gov/news-issuances/news-releases/2020/nr-occ-2020-125.html)
- SEC staff: [security tokens can trade on exchanges](https://www.sec.gov/divisions/marketreg/mr-noaction/2020/finra-ats-role-in-settlement-of-digital-asset-security-trades-09252020.pdf)
- For the memecoiners: Liquality’s [browser extension](https://twitter.com/Liquality_io/status/1309167433349881856) for cross-chain ETH/BTC swaps and [tBtc launches with increasing supply caps](https://blog.keep.network/tbtc-the-safe-way-to-use-bitcoin-in-defi-is-live-on-tbtc-network-de2bb8b6eaf7)
- Fairmint releases the SAFE-like [Continuous Agreement for Equity](https://medium.com/fairmint/introducing-the-cafe-ae12d6c34cc0) (CAFE)

**General**

- Kucoin [hacked for at least 150m USD](https://www.kucoin.com/news/en-kucoin-security-incident-update). Tether [froze 33m USDT in response](https://twitter.com/paoloardoino/status/1309771801581494272) and Ocean Protocol [paused their token contract to migrate it](https://blog.oceanprotocol.com/ocean-protocol-foundation-statement-regarding-kucoin-hack-c1af0aa0c36b)
- China state TV runs [positive news about Ethereum and DeFi](https://twitter.com/MariaShen/status/1309886115688542210)
- Ex-employee of Loom Network [opines on how the demise occurred](https://www.kickstarter.com/projects/328862817/zombie-battleground-the-new-generation-of-ccg-tcg/posts/2906929)
- OpenBazaar to [shut down if no funding found](https://medium.com/@therealopenbazaar/openbazaar-needs-your-support-75fe7e117ad1) by [2021](https://twitter.com/openbazaar/status/1310252576848437248)
- “[websites secretly track you by drawing random junk offscreen and measuring small variations in how different browsers/computers render it](https://twitter.com/kcimc/status/1308367355693600768)”

* * *

## **Job Listings**

- DeFi devs! Yield is hiring for Solidity and front-end – contact@yield.is
- Mainframe is hiring a [Senior Front End Engineer](https://cryptocurrencyjobs.co/engineering/mainframe-senior-front-end-engineer/)
- Live for DeFi? [mStable](https://twitter.com/mstable_) is looking for a [Smart Contract/Protocol Developer](https://cryptocurrencyjobs.co/engineering/mstable-protocol-developer-defi)
- Integrate new blockchains into Chainlink as an [Integrations Engineer](https://jobs.lever.co/chainlink/475db2e1-32dc-4c17-bc09-f9421fa633ac)
- Trail of Bits hiring elite [blockchain security engineers](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & [app security](https://jobs.lever.co/trailofbits/8b7f7fc1-efb0-4e89-b406-784c3a2d77e4)
- 0x is hiring devs! [Full-stack, back-end, front-end or Solidity](https://0x.org/about/jobs)
- Celer Network: hiring Solidity and Go devs. Email: hiring@celer.network
- Nexus Mutual: [experienced Solidity dev](https://angel.co/company/nexus-mutual-1/jobs/967538-smart-contract-engineer); prefer European timezones

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## 🥩 **Staking pool questionnaire: October 15** 🥩 

My [questionnaire for staking pools](https://docs.google.com/document/d/1wrzKXff2XwY4Bu5ynVqvlPXI4xqM4-Hwx7Jh7_-1IGg/edit) will be due October 15th.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow me on twitter: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-27-2020/](https://weekinethereumnews.com/week-in-ethereum-news-september-27-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Sep 29 - Spadina [eth2 deposit contract/genesis dress rehearsal](https://github.com/goerli/medalla/blob/master/spadina/README.md). **[viewing party](https://www.youtube.com/watch?v=8YJuAmJqSLU)**
- Sep 29 - [ENS online workshop](https://medium.com/the-ethereum-name-service/ens-online-workshop-2020-date-announced-47b8deb69877)
- Sep30 - Oct25 - [EthPlanet hackathon](https://ethplanet-hackathon.devfolio.co/)
- Oct 2-30 - [EthOnline hackathon](https://www.ethonline.org/) and summits
- Oct 2 - [Gitcoin grants matching ends](https://gitcoin.co/grants/). Here’s my [Week in Eth News grant](https://gitcoin.co/grants/237/week-in-ethereum-news)
- **Oct 19-26 - [EthLagos energy hackathon](https://ethlagos.io/)**
- Oct 20 - [submission deadline for Medalla data challenge](https://ethereum.org/en/eth2/get-involved/medalla-data-challenge/)
- Oct 31 - [submission deadline for Underhanded Solidity Contest](https://underhanded.soliditylang.org/)
- Nov 6-7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)
- Nov 16 - [MetaMask Provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

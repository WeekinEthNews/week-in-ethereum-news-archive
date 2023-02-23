---
title: "Week in Ethereum News <BR> Jan 24, 2021"
date: "2021-01-24"
---

## **Eth News and Links**

**Eth1**

- Latest [core devs call](https://youtu.be/3xNfGNnQ5Vs?t=150). Beiko’s [notes](https://twitter.com/TimBeiko/status/1352615824859648001): Berlin testnet coming soon, Ice Age delay probably goes in the next 1559 fork.
- [Criteria for Turbogeth beta release](https://github.com/ledgerwatch/turbo-geth/wiki/Criteria-for-transitioning-from-Alpha-to-Beta): usable for mining, simplify block header/body downloading, Clique/POA switching, switching from LMDB database to MDBX
- Latest [Turbogeth weekly release](https://github.com/ledgerwatch/turbo-geth/releases/tag/v2021.01.02) adds `debug_traceCall`
- Gas cost [estimates of EVM384](https://notes.ethereum.org/@poemm/evm384-update5)
- [Why 1559](https://hackmd.io/@timbeiko/why-1559)? Better UX, better economics, better security.
- Beiko’s [state of 1559 update](https://hackmd.io/@timbeiko/1559-updates/https%3A%2F%2Fhackmd.io%2F%40timbeiko%2F1559-update-006)
- Alex Stokes: [1559 is good for miners](https://ralexstokes.medium.com/miners-favor-1559-b91e003b63eb)

**Eth2**

- Danny Ryan’s [state of Eth2 in Jan 2021](https://blog.ethereum.org/2021/01/20/the-state-of-eth2-january-2021/): eth2 is Eth’s future consensus layer, next up is either turning off PoW or sharded data for rollups
- Latest [Lighthouse update](https://lighthouse.sigmaprime.io/update-33.html): in-depth discussion of sharded data or turning off PoW. Leans toward turning off PoW with (an obviously tentative) goal of shipping in 12 months.
- [Prysm’s short-term work](https://medium.com/prysmatic-labs/prysmatic-labs-2021-update-494def64f0b5): more performant slasher and production ready UI
- [Nimbus Grafana dashboard challenge](https://our.status.im/nimbus-grafana-challenge/) (prizes up to $5k)
- Supranational’s [blst library](https://medium.com/supranational/introducing-blst-2b6a988d68ee) first public release, fast sigs for BLS12-381

**Layer2**

- [Fast withdrawals to mainnet](https://twitter.com/daniel_loopring/status/1351467899274240000?) on Loopring’s zk rollup
- Celer has [1 million users on its state channel](https://blog.celer.network/2021/01/17/celer-network-2021-update-to-a-better-future/) games
- [DeFi Pooling](https://medium.com/starkware/defi-pooling-1332ddebff21) from StarkWare, a yearn-style vault on layer2 to save gas

* * *

### **This newsletter is made possible thanks to [Trail of Bits](https://www.trailofbits.com/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/05/2314423.jpeg)

[Rajeev G](https://twitter.com/0xRajeev), a security engineer with the Status project, has started providing audit report breakdowns for the benefit of less security-savvy users. [His first report breakdown](https://secureum.substack.com/p/making-defi-safu-secureum-3) covers the Trail of Bits report for the Origin Dollar, which was launched without a security review and then exploited before the scheduled audit was completed. One takeaway: 7 security issues, including 3 of the highest severity, could have been found automatically with [Slither](https://github.com/crytic/slither).

* * *

**Stuff for developers**

- web3js [v1.3.3](https://github.com/ChainSafe/web3.js/releases/tag/v1.3.3) - fix Metamask provider change
- Fe [v0.1 alpha release](https://github.com/ethereum/fe/releases/tag/v0.1.0-alpha) python-like language
- [Truffle-token-test-utils](https://www.npmjs.com/package/truffle-token-test-utils) token transfer viz
- [SMTChecker and the synthesis of external functions](https://fv.ethereum.org/2021/01/18/smtchecker-and-synthesis-of-external-functions/), coming in next Solidity release
- A [dev’s intro to Ethereum](https://snakecharmers.ethereum.org/a-developers-guide-to-ethereum-pt-2/), part 2

**Security/incidents**

- Livepeer finds and [patches logic bug](https://forum.livepeer.org/t/security-vulnerability-disclosure-fixed-delegators-can-increase-stake-and-fees-by-delegating-to-transcoders-under-certain-conditions/1202)
- Secureum’s [guide to reading audits](https://secureum.substack.com/p/making-defi-safu-secureum-3)

**Ecosystem**

- Josh Stark: [Year in Ethereum 2020](https://jjmstark.medium.com/the-year-in-ethereum-2020-98123e5f160d)
- ENS’s [DNS Namespace integration](https://medium.com/the-ethereum-name-service/dns-namespace-integration-on-testnet-ethereum-classic-labs-sponsors-with-grant-19d57bf16a8b) is live on testnet. Use your .com domain as your ENS name.

**Application layer**

- [Gasless NFT minting](https://mintable.medium.com/gas-fees-suck-mint-nfts-without-a-transaction-on-mintable-8d54b85a471c) with Mintable
- [Enzyme (eg, Melon v2) live](https://medium.com/enzymefinance/introducing-enzyme-7100201a56b5). 150 assets, lending enabled, provide liquidity, synthetics. v1 UI stays live for 3 months.
- Metastable [SAVE v2 is live](https://medium.com/mstable/mstable-launches-new-composable-version-of-musd-save-982a814e17d0), with tokenized stablecoin LPs
- [Saddle is live](https://medium.com/saddle/introducing-saddle-a-specialized-amm-for-pegged-value-crypto-assets-e607d2747345), a Curve fork aimed at BTC on Ethereum using virtual synths
- In the tokenized BTC realm, BadgerDAO does BTC yieldfarming and this week launched a [rebase BTC game called Digg](https://badgerdao.medium.com/digg-at-a-glance-complete-guide-d0dc2c29d303)
- [Charm options](https://medium.com/charmfinance/charm-is-live-on-mainnet-a6e5af542456) is live. No oracles, 100k cap per market right now
- [ArmorFinance is live](https://medium.com/armorfi/introducing-armor-14cccb5d1699): buy Nexus Mutual coverage without having to doxx yourself (KYC), plus token rewards for users
- We’re over [$25b total value locked](https://twitter.com/defipulse/status/1351520589039738880) per DefiPulse

**Regulation/business/tokens**

- [Defi will eat corporate debt](https://newsletter.banklesshq.com/p/defi-will-eat-corporate-debt)
- Coindesk: [ETH to 2k](https://www.coindesk.com/ethereum-price-to-2k-3-reasons)
- Fundstrat issues [$10.5k price target for ETH](https://twitter.com/David_Grid/status/1351766444829253632)
- [Coinbase buys BisonTrails](https://blog.coinbase.com/coinbase-to-acquire-leading-blockchain-infrastructure-platform-bison-trails-f879654421d6)
- Chainalysis says the only crime on blockchains is [payments for ransomware and darknet markets](https://blog.chainalysis.com/reports/2021-crypto-crime-report-intro-ransomware-scams-darknet-markets). Disproportionately on Bitcoin, of course

**General**

- MyCrypto’s review of 2020’s [major blockchain security incidents](https://medium.com/mycrypto/2020-in-review-major-blockchain-crypto-security-incidents-6c5ced8dc81e)
- Billy Rennekamp on the [future (and unbundling?) of crypto wallets](https://billyrennekamp.medium.com/account-coordinator-a-proposal-for-the-future-of-wallets-9fc54032a202)
- Brave adds [IPFS support](https://brave.com/ipfs-support/) with go-ipfs running a local node
- Qin, Zhou, Gervais paper: Quantifying [miner extractable value](https://arxiv.org/pdf/2101.05511.pdf)
- Werner, Perez, et al, paper: [DeFi Systemization of Knowledge](https://arxiv.org/abs/2101.08778)

* * *

## **Job Listings**

- MetaMask is hiring engineers for a variety of positions. Apply [here](https://consensys.net/open-roles/2572388/).
- Trail of Bits is looking for a [technical editor/writer](https://jobs.lever.co/trailofbits/8bf936ff-b86c-462e-80b2-4d58004bc68d) & [security engineer](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf)
- 0x looking for [devs of all types](https://0x.org/about/jobs) and a [data analyst](https://boards.greenhouse.io/0x/jobs/4220949002)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-jan-24-2021/](https://weekinethereumnews.com/week-in-ethereum-news-jan-24-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **Jan 27 - [ETH JSON RPC API Standard](https://github.com/ethereum-oasis/eth1.x-JSON-RPC-API-standard) call**
- **Feb 5 - [Nimbus Grafana challenge](https://our.status.im/nimbus-grafana-challenge/) submissions deadline (prizes up to $5k)**
- Feb 5-12 - [EthDenver](https://www.ethdenver.com/) (virtual)
- **Feb 8 - [CME launches ETH futures](https://www.cmegroup.com/trading/ether-futures.html)**
- Mar 5 - Financial Cryptography [DeFi academic workshop](https://fc21.ifca.ai/defi/)
- Apr 6-8 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

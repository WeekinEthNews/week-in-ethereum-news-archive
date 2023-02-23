---
title: "Week in Ethereum News <BR> May 9, 2021"
date: "2021-05-09"
---

## **Eth News and Links**

**Mainnet execution layer**

- Geth [v1.10.3](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.3): new Grafana dashboard, next release likely to have snap sync as default, eth/65 now the minimum
- [FuzzyVM](https://mariusvanderwijden.github.io/blog/2021/05/02/FuzzyVM/): an EVM differential fuzzing framework
- A proposed [design for witness gas costs](https://notes.ethereum.org/@vbuterin/witness_gas_cost_2) after switching to Verkle trees
- Notes from the [London coordination call](https://twitter.com/TimBeiko/status/1390703192153808899)
- [Baikal](https://github.com/ethereum/eth1.0-specs/blob/master/network-upgrades/client-integration-testnets/baikal.md), the latest London devnet, will launch this week

**EIPs/Standards**

- [EIP3554](https://github.com/ethereum/EIPs/blob/909863b2938b5f8ae38d42c8b6442e599d7605a4/EIPS/eip-3554.md): difficulty bomb delay

**Proof of stake consensus layer**

- Latest [consensus layer call](https://youtu.be/qhcMxBh0GEc?t=117). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/B1wRBDWdd) and [Alex Stokes](https://twitter.com/ralexstokes/status/1390370217524568064): Altair upgrade aggressively aimed at August
- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210508) reviews last week’s “very encouraging” ephemeral multi-client testnet to turn off PoW
- For (somewhat technical) stakers: [track your relative performance](https://www.reddit.com/r/ethstaker/comments/n692yp/granular_validator_performance_tracking/)
- New Ledger [Nano S firmware supports Eth staking](https://www.ledger.com/blog/ledger-nano-s-new-firmware-version-200-now-available) deposits
- [Secret shared validators (MPC for distributed control of a staker), phase 1 testing summary](https://medium.com/bloxstaking/secret-shared-validator-ssv-phase-1-testing-summary-5e3f5ab06083): several shared validators successfully staked on Pyrmont testnet
- How [Eth staking incentives promote decentralization and client diversity](https://phil-eth.medium.com/diversity-for-a-healthy-beaconchain-645ee1cea7ec)

**Layer2**

- [OKEx to support deposits/withdrawals to Arbitrum](https://www.okex.com/support/hc/en-us/articles/360060706511)
- StarkEx [crosses $1b traded](https://twitter.com/ukolodny/status/1390601561173381125) across dydx, Deversifi, and Immutable
- Two standardization efforts for layer2 and sidechains: [standard arbitrary message bridge](https://ethereum-magicians.org/t/a-standard-interface-for-arbitrary-message-bridges-between-chains-layers/6163) and an outline for a [standard interface token transfers](https://ethereum-magicians.org/t/outlining-a-standard-interface-for-cross-domain-erc20-transfers/6151)

* * *

### **This newsletter is made possible thanks to [1inch Network](https://1inch.io/?utm_source=evan_van_ness&utm_medium=newsletter&utm_campaign=letter_02)!**

![](https://weekinethereumnews.com/wp-content/uploads/2021/04/1inchbanner-1024x402.png)

The [1inch Network](https://1inch.io/?utm_source=evan_van_ness&utm_medium=newsletter&utm_campaign=letter_02) brings together the best decentralized protocols whose synergies enable the fastest, most lucrative, and most protected operations in the DeFi space. The 1inch Aggregation Protocol facilitates cost-efficient and secure swap transactions across multiple liquidity sources and the 1inch Liquidity Protocol is a next-generation automated market maker that protects users from front-running attacks and offers attractive opportunities to liquidity providers.

In late April, the team at 1inch Network released the [1inch Wallet for iOS](https://1inch.io/wallet/?utm_source=evan_van_ness&utm_medium=newsletter&utm_campaign=letter_02), a highly protected and innovative solution for storing, receiving, sending, and swapping crypto assets on Ethereum and Binance Smart Chain.

Download the [1inch Wallet for iOS](https://apps.apple.com/app/apple-store/id1546049391?pt=122481420&ct=evan_van_ness&mt=8) now and start swapping at the best market rates.

For more info check [1inch.io](https://1inch.io/?utm_source=evan_van_ness&utm_medium=newsletter&utm_campaign=letter_02) and follow the [1inch Network's official Twitter](https://twitter.com/1inchNetwork)!

* * *

**Stuff for developers**

- [Typechain v5](https://twitter.com/krzKaczor/status/1391473971531587584) (TypeScript bindings for Eth code)
- [ETK](https://quilt.github.io/etk/): EVM bytecode assembler and disassembler
- Tool to [simulate transactions with mainnet state](https://oko.palkeo.com/txview/)
- Full documentation of [Solidity’s optimizer](https://docs.soliditylang.org/en/latest/internals/optimizer.html) - the old one using opcodes and the new one on Yul
- Tutorial on [new upgradable UUPS (EIP1822) proxy](https://forum.openzeppelin.com/t/uups-proxies-tutorial-solidity-javascript/7786) pattern in OpenZeppelin
- [Building graphQL APIs](https://dev.to/dabit3/building-graphql-apis-on-ethereum-4poa) on Ethereum
- [New transaction types](https://blog.mycrypto.com/new-transaction-types-on-ethereum/), understanding Berlin’s EIP2718 Typed Transaction Envelope
- [tally](https://www.reddit.com/r/ethereum/comments/n7n1mq/tally_arbitraryprecision_arithmetic_library_for/): arbitrary-precision arithmetic library for JavaScript and EVM
- Pinata now offers [dedicated IPFS gateways](https://medium.com/pinata/announcing-dedicated-ipfs-gateways-60f599949ce)
- Some [best JavaScript security practices](https://twitter.com/brunobar79/status/1389724665338269701) for your Eth app
- Dabit and Austin Griffith [video discussion of how web2 devs can learn to build web3 apps with Ethereum](https://www.youtube.com/watch?v=ogjOjUjCVLk&t=780s)

**Security**

- Rari [hacked for ~4k ETH (~$15m)](https://nipunp.medium.com/5-8-21-rari-capital-exploit-timeline-analysis-8beda31cbc1a) across both Ethereum and BinanceSmartChain using fake tokens similar to the Pickle attack
- Binance’s ValueDefi hacked twice this week for a total of ~$21m, once by [reintializing a function](https://www.rekt.news/value-rekt2/) and once by [improperly calculating exponents](https://www.rekt.news/value-rekt3/)
- Insecure RNG in Meebits minting [exploited for a rare Meebit](https://twitter.com/sillytuna/status/1391013965170454540). The unverified source code allowed for LarvaLabs to pause the minting.

**Ecosystem**

- Guido Vranken [finds Golang bug](https://groups.google.com/g/golang-announce/c/cu9SP4eSXMc) as part of Eth bounty program
- [EF Fellowship](https://blog.ethereum.org/2021/05/07/ethereum-for-the-next-billion/)’s first cohort, an pilot program to nurture public sector adoption in emerging economies

**Application layer**

- Uniswap [v3 launches](https://uniswap.org/blog/launch-uniswap-v3/) and quickly becomes [#2 dex behind v2](https://twitter.com/haydenzadams/status/1391063276507836417) with some of the NFT LP positions containing rare sparkles
    - Neat v3 [LP strategy simulator](https://defi-lab.xyz/) tool
- Synthetix’s [Kwenta crosses $1b](https://twitter.com/kwenta_io/status/1390038926006624257) trading mark
- What’s in a [Commons Stack token hatch](https://medium.com/commonsstack/whats-in-a-hatch-3799a398243a)?
- Gary Vaynerchuk announces [Veefriends](https://www.veefriends.com/): NFT series with accompanying real world rights from mentoring to Veecon to gift boxes

**Regulation/business/tokens**

- VanEck files for [ETH ETF](https://www.sec.gov/Archives/edgar/data/1860788/000093041321001047/c101690_s1.htm)
- [The road to Eth 150k](https://draecomino.substack.com/p/the-road-to-150000-ethereum-with) with Nikhil Shamapant
- S&P releases three crypto indexes: [ETH, BTC, and a combo of both](https://www.coindesk.com/sp-goes-live-with-bitcoin-ethereum-crypto-indexes)

**General**

- [Cryptofees.info v2](https://dmihal.medium.com/cryptofees-info-grows-up-eaf64557f6f4) adds ability to go back in time to specific date, a PS ratio, and extra details on each project
- Coinbase committing to decentralization by [closing its former San Fran HQ](https://twitter.com/CoinbaseNews/status/1390065013071781889)
- Twitter adds tipping features with accompanying major privacy fails: [your email address](https://twitter.com/ashk4n/status/1390502576194392069) and [your address](https://twitter.com/amyhoy/status/1390419731564269568)
- Apple ends opaque [cross-app iPhone tracking](https://www.eff.org/deeplinks/2021/04/apples-apptrackingtransparency-upending-mobile-phone-tracking). Android is worse, of course.

* * *

## **Job Listings**

- The Raiden team is hiring a [Growth and Marketing Lead](https://angel.co/company/brainbot-group/jobs/1350874-growth-marketing-lead-for-the-raiden-network) in Berlin
- Devs + researchers; build fixed-income, leverage & P2P markets w/[Prometheus](https://www.prl.one/jobs/)
- DeFi coverage protocol [Solace](https://solace.fi/), launching May, seeks [Solidity and Frontend devs](https://angel.co/company/solace-fi/jobs/1310318-full-stack-ethereum-developer)
- ENS is hiring all kinds of [devs, plus Community, Integration & Governance leads](https://medium.com/the-ethereum-name-service/ens-is-hiring-come-build-a-new-decentralized-internet-with-us-24398dea3ac)
- [Join Zerion as Product Manager](https://jobs.lever.co/zerion/02a3d561-3367-48c0-9e50-eef8db11d5dc?lever-origin=applied&lever-source%5B%5D=WeekInEthereum) and take DeFi to the next level
- Giveth is [hiring experienced Solidity Devs](https://cryptojobslist.com/jobs/lead-solidity-smart-contract-developer-at-giveth-remote) interested in #Defi4good
- Join our team to help [bring Ethereum into governments as a dApp developer](https://www.notion.so/symfoni/Symfoni-jobs-0c2bdc029d2a4cf7b91864a5e68ed00f)
- BitGo's WBTC team is hiring [Blockchain Engineers](https://boards.greenhouse.io/bitgo/jobs/5191525002), [Sr. Blockchain Engineers](https://boards.greenhouse.io/bitgo/jobs/5089951002) and [Lead Blockchain Engineers](https://boards.greenhouse.io/bitgo/jobs/5197342002). (You can check out the rest of our jobs [here](https://boards.greenhouse.io/bitgo)!)

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-may-9-2021/](https://weekinethereumnews.com/week-in-ethereum-news-may-9-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- May 14 - papers due for [WoSCA 2021](https://trailofbits.github.io/WoSCA/)
- May 14 - Jun 2 - [0xHack](https://0xhack.dev/)
- May 18-21 - [EY Global Blockchain Summit](https://pub.ey.com/public/2021/2101/2101-3679331/blockchain-summit-2021/index.html)
- **May 21 - [Linda Xie and Austin Griffith talk Eth dev tooling](https://twitter.com/ljxie/status/1390772688193560581)**
- **Jul 14 - [tentative date for London hard fork](https://docs.google.com/spreadsheets/d/1Y3yyTqeqRO1O2UFVkNkHK_V5oRulZd6y-JJbSnKYrb4/edit#gid=0) (Ropsten June 9, Goerli June 16, Rinkeby June 23)**
- Jul 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

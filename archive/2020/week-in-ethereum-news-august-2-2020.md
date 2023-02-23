---
title: "Week in Ethereum News <BR> August 2, 2020"
date: "2020-08-03"
---

## **Eth News and Links**

**Eth1**

- [Turbogeth public alpha](https://github.com/ledgerwatch/turbo-geth/releases/tag/2020.07.01-alpha) - full sync in 2 days, 650 gigs disk space
- Geth [v1.9.18](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.18) bugfix release
- A [backrunning patch has been merged](https://github.com/ethereum/go-ethereum/pull/21358) and is scheduled for Geth v1.9.19
- [Stationary behavior of EIP 1559 agent-based model](https://github.com/barnabemonnot/abm1559/blob/master/notebooks/stationary1559.ipynb)

**Eth2**

- [Validator launchpad](https://blog.ethereum.org/2020/07/27/eth2-validator-launchpad/) released - the interface for eth2 stakers which is being tested now for the Aug 4 Medalla testnet launch
- Ben Edgington’s writeup of the [genesis process of Eth2’s Beacon Chain](https://hackmd.io/@benjaminion/genesis)
- Strategies for [protecting validator keys](https://www.attestant.io/posts/protecting-validator-keys/)
- If you’re looking for help with validating on Medalla, join the [eth2 staker discord](https://invite.gg/ethstaker)

**EIPs/Standards**

- [EIP2844](https://github.com/oed/EIPs/blob/5b9bdaebe3743f083e0a06f315db1b9c70b60bce/EIPS/eip-2844.md): Add DID related methods to the JSON-RPC
- [EIP2831](https://github.com/GregTheGreek/EIPs/blob/fb7ae6c84549da34f5080143e826ce8cccf66485/EIPS/eip-2831.md): Transaction Replacement Message Type

**Crypto**

- Microsoft’s [Spartan](https://github.com/microsoft/Spartan): fast SNARKs without trusted setup
- [IBM completes successful field trials on Fully Homomorphic Encryption](https://arstechnica.com/gadgets/2020/07/ibm-completes-successful-field-trials-on-fully-homomorphic-encryption/)

**Layer2**

- Wow! Some impressive [Reddit Scaling Bakeoff submissions](https://www.reddit.com/r/ethereum/comments/hbjx25/the_great_reddit_scaling_bakeoff/fznuqn2/) from layer2 (in order of submission): [Starkware](https://www.reddit.com/r/ethereum/comments/i01sjk/starkwares_submission_to_reddits_scaling_bakeoff/), [Matic](https://www.reddit.com/r/ethereum/comments/i07h1g/matic_networks_great_reddit_scaling_bakeoff/), [OMG Network](https://www.reddit.com/r/ethereum/comments/i19us9/omg_networks_great_reddit_scaling_bakeoff_proposal/), [Fuel Labs](https://www.reddit.com/r/ethereum/comments/i1cimc/the_great_reddit_scaling_bakeoff_submission_by/), [Raiden](https://www.reddit.com/r/ethereum/comments/i1dulf/raiddit_raiden_network_submission_to_the_great/), [Arbitrum](https://www.reddit.com/r/ethereum/comments/i1g5cc/scaling_reddit_community_points_with_arbitrum/), [Aztec](https://www.reddit.com/r/ethereum/comments/i1j6ck/the_reddit_bakeoff_zkreddit_by_aztec/), [MatterLabs](https://www.reddit.com/r/ethereum/comments/i1rsan/zksync_v11_reddit_edition_recursion_up_to_3000/?), [Abridged/Kchannels](https://www.reddit.com/r/ethereum/comments/i1jjjv/reddit_scaling_bakeoff_submission_abridged/), [Hubble Project](https://www.reddit.com/r/ethereum/comments/i1qmod/the_reddit_bakeoff_submission_by_hubble_project/), [Celer](https://www.reddit.com/r/ethereum/comments/i2hx80/celer_joins_reddit_great_scaling_bakeoff_exactly/)
- Also check out [Connext’s submission](https://www.reddit.com/r/ethereum/comments/i1eooc/spacefold_connexts_submission_to_the_great_reddit/) on using channels between rollups
- [Rollup exits with efficient witness generation](https://ethresear.ch/t/efficient-unassisted-exit-witness-generation-from-rollups/7776)
- [Pessimistic rollup](https://ethresear.ch/t/pessimistic-rollup-scalable-batched-smart-contract-interactions/7765)

* * *

### **This newsletter is made possible thanks to [Celer Network](https://www.celer.network/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/05/Screenshot-from-2020-05-10-16-13-18.jpg)

[Celer](http://celer.network/) is a coherent layer-2 scaling platform on Ethereum. [Their submission to Reddit Great Scaling Bakeoff](https://www.reddit.com/r/ethereum/comments/i2hx80/celer_joins_reddit_great_scaling_bakeoff_exactly/) talks about their in-production matching uses cases, why they believe state channel offers the right tradeoffs for the use cases and performance benchmarks. They also propose the concept of Layer-2 LEGO to have multiple different layer-2 techniques working together to address all current and future use cases in a coherent way. 

* * *

**Stuff for developers**

- Solidity [v0.7](https://solidity.ethereum.org/2020/07/28/solidity-v0.7.0-release-announcement/) breaking release with lots of backwards-incompatible syntax and semantics changes
- Truffle [v5.1.37](https://github.com/trufflesuite/truffle/releases/tag/v5.1.37) adds syntax highlighting for Solidity v0.7
- hevm adds [symbolic execution features](https://fv.ethereum.org/2020/07/28/symbolic-hevm-release/) and a tutorial for using them
- Academic paper [benchmarking Eth security analysis tools](https://dl.acm.org/doi/pdf/10.1145/3395363.3397385)
- [EthCode](https://marketplace.visualstudio.com/items?itemName=ethential.ethcode) plugin for VSCode had a new release
- [Building an encrypted to-do list](https://medium.com/3box/building-an-encrypted-todo-list-with-3box-part-1-2-d1619cd02e5b) with 3Box tutorial
- Fairmint [opensources its linear bonding curve](https://blog.fairmint.co/continuous-financing-bonding-curve-contract/) code
- [any.sender](https://medium.com/anydot/any-sender-first-publicly-accessible-relayer-with-0-gas-overhead-and-2-fee-f2efe1f44e09) fast and cheap transaction relayer API now has zero gas overhead and a library for unit testing
- Loredana’s [decentralized spreadsheets demo](https://www.youtube.com/watch?v=PoA6zqBiApg&feature=youtu.be) in her lisp-like language, Taylor
- How to [create a Defi dashboard with TheGraph and GoogleSheets](https://towardsdatascience.com/how-to-create-a-ethereum-defi-realtime-dashboard-a60c23b527f7)
- Paul Berg’s [Solidity template for his favorite toolstack](https://github.com/PaulRBerg/solidity-template): Buidler + Typechain + Ethers + Waffle + Solhint + Solcover

**Ecosystem**

- This week we celebrated [5 years since the mainnet genesis block](https://blog.ethereum.org/2020/07/30/ethereum-turns-5/)
- Miners pushed the [block gas limit to 12.5m](https://etherscan.io/chart/gaslimit), so Eth’s max throughput is now 45 transactions per second. Barnabé’s analysis is that the [gaslimit increase did not lower gas prices](https://ethereum.github.io/rig/ethdata/notebooks/gas_weather_reports/exploreJuly21.html)
- Ethereum has a [54 day streak of more transaction fees than Bitcoin](https://twitter.com/Delphi_Digital/status/1289232632471883779)
- Check out this very cool [txstreet transaction visualizer](https://txstreet.com/v/eth-btc)
- A simple and [easy interface to cancel pending transactions](https://cancel-ethereum-transactions.web.app/)
- Ethereum.org is now [available in 30 languages](https://blog.ethereum.org/2020/07/29/ethdotorg-translation-milestone/)
- [Dex volumes are threatening to pass centralized exchanges](https://explore.duneanalytics.com/public/dashboards/c87JEtVi2GlyIZHQOR02NsfyJV48eaKEQSiKplJ7)

**Enterprise**

- Videos from the EEA’s [Ethereum in the Enterprise](https://www.youtube.com/watch?v=pw6OzjkkXcU) conference
- Securing [enterprise chains with Luna HSMs and PegaSysPlus v1.2](https://pegasys.tech/thales-luna-hsms-and-pegasys-plus-1-2/)
- Hyperledger Besu [v1.5.1](https://github.com/hyperledger/besu/releases/1.5.1?)

**Application layer**

- Augur v2 launched and [then relaunched](https://www.augur.net/blog/augur-v2-redo/) with no more GSN/new account fee. If you want to support this newsletter, [this is an affiliate link](https://augurapp.eth.link?r=0x663d3947f03eF5B387992b880aC85940057c13e3)
- Synthetix [decommissions its foundation in favor of 3 DAOs](https://blog.synthetix.io/synthetix-foundation-decommissioned/)
- [Aave revamping its token model](https://medium.com/aave/aavenomics-eeab650cccc2); migrating LEND to AAVE to govern the protocol; adding stakers for safety
- [How to protect yourself against hacks](https://bankless.substack.com/p/how-to-protect-against-hacks-with) with Nexus Mutual
- YFI and forks [had quite a week](https://medium.com/hakkafinance/analysis-of-yearn-and-mstable-frenzy-cd381d8e069): a [fork called YFII](https://medium.com/@WhiteNoise1984/yfii-innovative-decentralized-defi-mining-pool-d745c032dfc0) catching fire in China before getting removed from the Balancer UI, [YFI started farming YFII and dumping it](https://twitter.com/oli_vdb/status/1288970901237661700), and then a different [fork (YYFI) was a scam](https://twitter.com/nanexcool/status/1289280976267419648) where the owner drained the Balancer pool
- [dForce is back](https://medium.com/dforcenet/dforce-yield-markets-dtoken-a397eebdbd96) doing a similar yield aggregation
- [MakerDAO hit 1 billion USD](https://twitter.com/nanexcool/status/1287578466477641734) in value locked up

**Tokens/Business/Regulation**

- What if [Eth had EIP1559](https://bankless.substack.com/p/what-if-eth-had-a-fee-burn-5-years) when the network launched?
- Coinbase is adding [2% a year rewards to holding DAI](https://blog.coinbase.com/coinbase-launches-dai-rewards-for-customers-in-the-us-uk-netherlands-spain-france-and-1519113f8d2f) with them
- How ArCoin got [SEC permission to do a treasury fund on Eth](https://www.coindesk.com/arcoins-blockchain-traded-fund-arca-tokensoft)
- 1inch’s [Chi gastoken](https://medium.com/@1inch.exchange/everything-you-wanted-to-know-about-chi-gastoken-a1ba0ea55bf3): how to hedge against gas prices
- [ResearchCoin is live to be earned](https://medium.com/researchhub/announcing-researchcoin-bc075d4a3235) (minted in future) where you earn tokens for uploading, summarizing and discussing scientific research
- Sign of the times: [flippening.watch returns](http://www.flippening.watch/)

**General**

- [Identity index](https://medium.com/@msena/what-is-identity-index-d3594b59633e): standard for creating a unified, decentralized identity-centric resource index
- TheGraph [launches incentivized testnet](https://thegraph.com/blog/testnet-announcement)
- [Ledger data breach](https://www.reddit.com/r/ethfinance/comments/hzwvn2/ledger_got_hacked_misled_people_dragged_their/): 1 million emails and 9500 physical addresses
- 3 kids [arrested for hacking Twitter](https://www.tampabay.com/news/crime/2020/07/31/17-year-old-in-tampa-arrested-for-hack-of-prominent-twitter-accounts/) and taking over accounts a couple weeks ago
- [ETC got 51% attacked](https://blog.bitquery.io/ethereum-classic-51-chain-attack-july-31-2020) again and the price went up

* * *

## **Job Listings**

- Trail of Bits is looking for: [blockchain security engineer](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & [cryptography analyst](https://jobs.lever.co/trailofbits/56af8506-3205-4c7b-b28d-ba8292bd1a47)
- 0x is looking for all kinds of devs: [full-stack, back-end, and front-end](https://0x.org/about/jobs)
- Celer Network: [Android developer](https://www.celer.network/career.html)
- Join one of the fastest-growing teams in blockchain: [19+ open roles](https://careers.smartcontract.com/) at Chainlink

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH/DAI/USDC to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **Watch this space**

If you want to follow me on Twitter, I got [@evan\_van\_ness](https://twitter.com/evan_van_ness) back after being suspended for a week for no reason, but after 3 weeks [@WeekInEthNews is still suspended for the crime of (checks notes) trying to upload a profile picture](https://www.evanvanness.com/post/624463633751195648/twitter-incompetence-in-one-small-image). Twitter is truly the most shamelessly incompetent company.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-2-2020/](https://weekinethereumnews.com/week-in-ethereum-news-august-2-2020/)

Did you get **forwarded** this newsletter? **[Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Aug 2 - [ENS grace period](https://medium.com/the-ethereum-name-service/the-great-renewal-its-time-to-renew-your-eth-names-or-else-lose-them-afccea4852cb) begins to end
- **Aug 4 - Medalla Eth2 testnet launch [viewing party](https://www.reddit.com/r/ethstaker/comments/i18ju5/announcing_the_ethereum_2_phase_0_multiclient/)**
- Aug 9-11 - [EDCON](https://edcon.io/)
- Aug 28-29 - Chainlink’s [Smart Contract Virtual Summit](https://www.smartcontractsummit.io/)
- Oct 2-30 - [EthOnline hackathon](https://www.ethonline.org/)
- Nov 6-7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)

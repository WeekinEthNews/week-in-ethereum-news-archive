---
title: "Week in Ethereum News <BR> Feb 22, 2021"
date: "2021-02-22"
---

## **Eth News and Links**

**Mainnet**

- Latest [core devs call](https://youtu.be/anrbnroO3dc?t=249). Beiko’s [notes](https://twitter.com/TimBeiko/status/1362787905433866245), discussion of what is needed to turn off PoW, mainnet Berlin fork set for April 14
- List of [EVM features possibly worth deleting](https://hackmd.io/@HWeNw8hNRimMm2m2GH56Cw/evm_feature_removing). Let’s rip the bandaids off, turning off PoW (“the merge”) is the opportunity
- Anyone want to [become an EIP editor](https://medium.com/ethereum-cat-herders/become-an-eip-editor-337f4376bf29)?
- EthereumJS’s [Typescript EVM release](https://github.com/ethereumjs/ethereumjs-monorepo/releases) with critical bugfixes
- Micah Zoltu’s argument for adding [BLS precompile in London](https://notes.ethereum.org/@GW1ZUbNKR5iRjjKYx6_dJQ/Skxf3tNcg_) fork
- [London fork with EIP1559 scheduled for July](https://github.com/ethereum/pm/issues/245), when the difficulty bomb starts to go off
- Understanding how [EIP1559 helps congestion control](https://barnabe.substack.com/p/congestion-control-and-eip1559)

**Proof of Stake**

- eth proof of stake [date to slot converter](https://play.rust-lang.org/?version=stable&mode=debug&edition=2018&gist=a211036e42c9726bfbbbcdf5a58ad086)
- New Lighthouse [release will help head/target attestations for whole network](https://github.com/sigp/lighthouse/releases/tag/v1.1.1), so if you’re running Lighthouse, please upgrade!
- [Withdrawal credentials merged](https://github.com/ethereum/eth2.0-specs/pull/2149), should enable trustless staking pools

**Layer2**

- Celer’s [cBridge](https://blog.celer.network/2021/02/15/celer-cbridge-fast-and-low-cost-value-transfer-network-for-an-interconnected-layer2-and-layer1-future), a cross-layer2 network for cheap, instant value transfers on EVM chains. Production ready, UI coming.
- [layer2.finance](https://blog.celer.network/2021/02/18/layer2-finance-get-defi-mass-adoption-today-scaling-layer-1-defi-in-place-with-zero-migration/): pool layer2 transactions from many users into a single transaction using Celer’s State Guardian Network for the rollup, coming in a month or two.
- Loopring’s rollup dex hasn’t been around long, has already done [500m USD](https://twitter.com/loopringorg/status/1363195374723284992), and is now doing $30m a day

* * *

### **This newsletter is made possible thanks to [Trail of Bits](https://www.trailofbits.com/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/05/2314423.jpeg)

Trail of Bits wants YOU to [apply for a position](https://www.trailofbits.com/careers) on their team! Positions are open for blockchain security engineers, project managers, product managers, financial controllers, and more. Make a career-defining contribution and help direct the future of blockchain security at Trail of Bits.

* * *

**Stuff for developers**

- [Defi Simulation](https://twitter.com/TenderlyApp/status/1361401631934414848) with Tenderly, spin up instant forks and manipulate the state/blockheight to simulate transactions
- How to [stream pending transactions with ethersjs](https://www.quiknode.io/guides/defi/how-to-stream-pending-transactions-with-ethers-js)
- Prysmatic: [finding an elusive bug](https://rauljordan.com/2021/02/18/when-a-solution-is-right-in-front-of-your-eyes.html) where database calls were inperformant on startup
- Infura: why use [Infura Transactions instead of your own in-house relayer](https://blog.infura.io/why-you-should-use-infura-transactions-instead-of-building-your-own-in-house-relayer)

**Security/incidents**

- Samsun found [bug in hashmasks sale](https://thehashmasks.medium.com/hashmask-art-sale-bug-report-13ccd66b55d7), could have re-entrancy minted thousands of hashmasks
- Primitive Finance found a [bug related to infinite approvals](https://primitivefinance.medium.com/whitehack-by-primitive-finance-most-funds-are-safe-user-action-required-4dd31c387b8) and rescued most funds
- Immunefi advocates for a [scaling bug bounty](https://medium.com/immunefi/a-defi-security-standard-the-scaling-bug-bounty-9b83dfdc1ba7)
- Malicious [Hardhat npm package](https://twitter.com/HardhatHQ/status/1362866790695641094) on hardhat-waffle instead of @nomiclabs/hardhat-waffle. Hardhat has now squatted relevant package names. Beware of trusted code!
- Use [strong Fiat-Shamir transformation and be careful](https://blog.trailofbits.com/2021/02/19/serving-up-zero-knowledge-proofs/) when implementing snarks
- [Reviews DAO](https://twitter.com/emilianobonassi/status/1361371101419421700): peer audits via barter
- An [Eth code security checklist](https://secureum.substack.com/p/smart-contract-security-101-secureum)

**Ecosystem**

- Nvidia is introducing an [Ethereum ASIC miner](https://blogs.nvidia.com/blog/2021/02/18/geforce-cmp/)
- Why miners can be [simultaneously paid too much and yet struggling to survive:](https://www.symphonious.net/2021/02/15/why-miners-can-be-simultaneously-paid-too-much-and-struggling-to-survive/) miners as a group are overpaid yet individual miners are barely breaking even

**Enterprise**

- Christie’s to auction a [Beeple NFT](https://twitter.com/ChristiesInc/status/1361670588608176128), it’s first purely digital art auction. It will also [accept ETH for payment](https://www.bloomberg.com/news/articles/2021-02-18/christie-s-beeple-auction-will-accept-ether-cryptocurrency-payment).
- Dubai government [free trade zone will now accept ETH](https://www.coindesk.com/dubai-free-zone-becomes-first-uae-government-entity-to-accept-bitcoin), BTC, and Tether
- [Expo IDE puts some of its treasury into ETH](https://twitter.com/JI/status/1362976438383636481). The devs know.

**Application layer**

- NyanCat creator sells NyanCat [NFT for 300 ETH](https://twitter.com/Lindsay_Howard/status/1362840312067031046) (~$600k) on Foundation
- [Rai is live](https://ameensol.medium.com/a-money-god-raises-rai-is-live-on-ethereum-mainnet-f9aff2b1d331) on mainnet. An Eth-collateralized asset with a reflexive self-peg set by interest rates
- [Ideamarket](https://ideamarket.io/) on mainnet: bonding curves for Twitter accounts.
- [uniswap over 100b](https://twitter.com/haydenzadams/status/1361356927226310668) lifetime volume
- PoolTogether [incentivizes deposits to their no-loss lottery](https://medium.com/pooltogether/introducing-pool-23b09f36db48) with the POOL governance token. Deposits have skyrocketed ~100x
- Ribbon finance is on [mainnet with a strangle option strategy](https://ribbonfinance.medium.com/yield-hacking-for-fun-and-profit-b50cf47fca35) - an aggregator of Hegic and Opyn

**Regulation/business/tokens**

- Vitalik reflects on his [post-election nTrump stacking](https://vitalik.ca/general/2021/02/18/election.html)
- Rekt.news says [cryptoart is art](https://www.rekt.news/nft-digital-art-enthusiast/): lots of money laundering
- NFTs as [“port of entry” for internet media](https://variant.mirror.xyz/T8kdtZRIgy_srXB5B06L8vBqFHYlEBcv6ae2zR6Y_eo)

**General**

- RFP for a full verification of the [Pickles SNARK on Ethereum](https://hackmd.io/u_2Ygx8XS5Ss1aObgOFjkA)
- [Consensus for async distributed key gen](https://arxiv.org/abs/2102.09041)
- Apple takes steps to thwart [M1 Mac “Silver Sparrow” malware](https://www.macrumors.com/2021/02/22/apple-revokes-silver-sparrow-certificates/)
- [Robinhood announces it will enable deposits and withdrawals for crypto](https://twitter.com/RobinhoodApp/status/1362143073510121472)

* * *

## **Job Listings**

- [DeversiFi](https://www.deversifi.com/careers) is hiring senior developers and marketing champions
- Are you a front-end dev? [Join Balancer!](https://angel.co/company/balancer-labs-1/jobs/1146637-front-end-engineer) Email: career \[at\] balancer.finance
- NEAR is looking for a [React Engineer](https://boards.greenhouse.io/near/jobs/4938418002)
- Trail of Bits is looking for a [blockchain security engineer](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf)
- 0x: [devs of all types](https://0x.org/about/jobs) and a [data analyst](https://boards.greenhouse.io/0x/jobs/4220949002)
- [HOPR](https://hoprnet.org/) is looking for a [privacy protocol engineer](https://hoprnet.jobbase.io/).

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-feb-22-2021/](https://weekinethereumnews.com/week-in-ethereum-news-feb-22-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Feb 28 - [Nimbus Grafana dashboard](https://twitter.com/ethnimbus/status/1360273972944920582) submissions due
- **Mar 1-5 - Ethereum Foundation’s [Ecosystem Support Program](https://twitter.com/EF_ESP/status/1362817256774893568) office hours**
- Mar 5 - Financial Cryptography [DeFi academic workshop](https://fc21.ifca.ai/defi/)
- **Mar 19-21 - ETHGlobal’s [NFT Hack](https://nft.ethglobal.co/)**
- Apr 9 - May 14 - ETHGlobal’s [Scaling Ethereum](https://scaling.ethglobal.co/) hackathon
- **April 14 - [Berlin upgrade fork](https://github.com/ethereum/pm/issues/248#issuecomment-782069875) (testnets: Ropsten Mar 10, Goerli Mar 17, Rinkeby Mar 24)**
- May 14 - papers due for [WoSCA 2021](https://trailofbits.github.io/WoSCA/)
- Jul 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

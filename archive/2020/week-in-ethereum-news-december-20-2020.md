---
title: "Week in Ethereum News <BR> Dec 20, 2020"
date: "2020-12-20"
---

## **Eth News and Links**

**Eth1**

- [1559 update](https://hackmd.io/@timbeiko/1559-updates/https%3A%2F%2Fhackmd.io%2F%40timbeiko%2F1559-update-005): more testing, tx pool management fine. [1559 Mainnet checklist](https://github.com/ethereum/pm/blob/master/Fee%20Market%20Meetings/mainnet-readiness.md)
- Latest [1559 implementation call](https://www.youtube.com/watch?v=mCOfz50Wcmo). Beiko’s [notes](https://twitter.com/TimBeiko/status/1339635848128544770)
- Alexandria [state network update](https://snakecharmers.ethereum.org/alexandria-dev-update-3/) - full header chain available in Jan

**Proof of Stake**

- Latest [eth2 call](https://youtu.be/Eo7H8fZA23E?t=150). Notes from [Mamy](https://gist.github.com/mratsim/86323a501154d581e67a1de9aa2149dc) and [Ben](https://hackmd.io/@benjaminion/ryC4cCunv). Early planning for q1/q2 2021 fork, to shift some accounting to mid-epoch and add light clients
- This week, we crossed 1 billion USD worth of ETH in the deposit contract (no link)

**Layer 2**

- Optimism [testnet adds fraud proofs](https://medium.com/ethereum-optimism/fraud-proof-security-drill-will-you-be-my-1-of-n-654e78c5ee1c), with a 3.2 eth bounty for anyone who finds their fraudulent transaction

* * *

### **This newsletter is made possible thanks to [Celer](https://www.celer.network/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

We are excited to announce that [Phase One of the Celer State Guardian Network (SGN) mainnet](https://blog.celer.network/2020/11/09/celer-state-guardian-network-launches-on-mainnet/) is now up and running! You can stake $CELR and [earn state guarding rewards](https://sgn.celer.network/explorer/) now with more than 35% block and fee annual reward. Real money games, such as [Arcade Win](https://apps.apple.com/us/app/arcade-win/id1459895768) and [Daub Cash](https://apps.apple.com/us/app/daub-cash/id1513396754), built using [Celer](http://developer.celerx.app/) as the foundational technology, have hosted more than 12 million games in the last year and processed 30million transactions using Celer's layer-2 infrastructure. 

Follow us on [twitter](https://twitter.com/CelerNetwork), [blog](https://blog.celer.network/), [discord](https://discord.com/invite/Trhab5w) and [telegram](https://t.me/celernetwork).

* * *

**Stuff for developers**

- Solidity [v0.8](https://blog.soliditylang.org/2020/12/16/solidity-v0.8.0-release-announcement/), say goodbye to SafeMath, internal errors will revert instead of invalid
- Solidity [0.7.6](https://blog.soliditylang.org/2020/12/16/solidity-0.7.6-release-announcement/), better support for calldata types, fallback function can return data
- [ethersjs is now equally as used as web3js](https://twitter.com/pedrouid/status/1340663949252063232)
- MyCrypto’s [testnet faucet](https://app.mycrypto.com/faucet) - Kovan, Rinkeby, Ropsten, Goerli
- [TheGraph](https://thegraph.com/blog/the-graph-network-launches-mainnet) launches on mainnet for decentralized indexing, subgraphs will begin migrating to decentralized in 2021

**Security and incidents**

- Slither [v0.7](https://github.com/crytic/slither/releases/tag/0.7.0), adds 26 detectors including what would have caught last week’s [Aave bug](https://blog.trailofbits.com/2020/12/16/breaking-aave-upgradeability/), plus support for Solidity top level objects
    - Neat: run the [Aave exploit in a Hardhat repo](https://github.com/Dan-Nolan/Delegatecall-Proxy-Bug)
- Warp Finance (something I’d never heard of until it got attacked) got [attacked for 6.8m in DAI/USDC](https://www.rekt.news/warp-finance-rekt/) (plus 1400 ETH) by swapping nearly 200m on Uniswap and 50m on dydx which depegged the price of WETH. Warp managed to get [~75% back of the DAI/USDC](https://warpfinance.medium.com/warp-finance-exploit-summary-recovery-of-funds-5b8fe4a11898)

**Ecosystem**

- [OpenGrants](https://jamesfickel.ghost.io/towards-long-term-incentives-on-ethereum/): long-term incentives for open source through streaming payments. First grant is [3600 ETH for Eth2 development](https://opengrants.com/grant/0x53e7daa8e3aa23cd30c75b2f599c303bada17064)
- [Money movers](https://money-movers.info/): compare value moved by ETH vs other blockchains
- Sassal’s [Eth now vs eth then](https://twitter.com/sassal0x/status/1339192917735292928). Comparing stats of when ETH first crossed $500 and where it is now.

**Enterprise**

- Microsoft [DRAM/SSD orders, shipments, and assets track and trace](https://cloudblogs.microsoft.com/industry-blog/manufacturing/2020/12/17/improve-supply-chain-resiliency-traceability-and-predictability-with-blockchain/) for Azure using private chain built on Quorum
- EY and Microsoft expand [XBox’s royalty management to be end-to-end](https://www.businesswire.com/news/home/20201214005125/en/EY-and-Microsoft-Expand-Xbox-Enterprise-Blockchain-Platform-for-Rights-and-Royalties-Management). Also on a private Quorum chain

**Application layer**

- Tornado.cash now [incentivizing deposits to increase privacy](https://tornado-cash.medium.com/tornado-cash-governance-proposal-a55c5c7d0703) (“the anonymity set”) through a token. Plus airdrop for early users
- [USM “minimalist stablecoin](https://twitter.com/JaEsf/status/1339324385988108299)” on mainnet, though in size-limited “baby form”
- Beeple [makes 3.5m](https://loopifyyy.medium.com/the-proof-of-nfts-3-5m-beeple-drop-37955867d789) USD in last weekend’s cryptoart sale
- Sorare signs up [Real Madrid](https://medium.com/sorare/real-madrid-joins-sorare-26e9271af3f0) and [Gerard Piqué](https://medium.com/sorare/gerard-piqu%C3%A9-joins-the-sorare-team-as-strategic-advisor-c467f82d57ac) in the same week
- [Defi777](https://dmihal.medium.com/defi777-v1-launch-c92f03ee40a1) is on mainnet. Wrap your erc20 tokens so you don’t have to approve and then you can interact with protocols by sending to an ENS name
- Treum’s [Swether](https://swether.io/) - design your Christmas sweater NFT (plus free sweatshirt with that logo if in US)

**Regulation/business/tokens**

- [CME announced ETH futures](https://www.cmegroup.com/trading/ether-futures.html) to launch Feb 8. Cash settled, 1 contract = 50 ETH
- CFTC releases [Digital Assets Primer](https://www.cftc.gov/PressRoom/PressReleases/8336-20)
- Germany legalizes [securities on chain](https://uk.reuters.com/article/germany-bonds-crypto-currency/germany-paves-way-for-electronic-securities-to-reap-blockchain-fruits-idUKKBN28Q1A0)
- Mnuchin’s ill-considered [midnight rulemaking](https://public-inspection.federalregister.gov/2020-28437.pdf) proposal on crypto addresses
- Coinbase [submits S-1 to begin IPO process](https://blog.coinbase.com/coinbase-announces-confidential-submission-of-draft-registration-statement-b140a9dfc9f5)

**General**

- [Halo Infinite](https://twitter.com/drakefjustin/status/1338626938999599116), any additive polynomial commitment scheme
- [Prover time comparison of GKR+Groth16 vs. Groth16 for proving MiMC hashes](https://ethresear.ch/t/prover-time-comparison-of-gkr-groth16-vs-groth16-for-proving-mimc-hashes/8373)
- Compound [announces PoA appchain](https://compound.cash/) plans; governed by COMP, with a collateralized stablecoin as the unit for paying fees.
- Multiple US federal agencies [compromised in attack on SolarWind](https://www.solarwinds.com/securityadvisory). The feds are [blaming Russian state action](https://abcnews.go.com/Politics/pretty-clear-russia-solarwinds-hack-pompeo-1st-us/story?id=74818788)
- Deleting [Google’s malware to 10x your machine’s performance](https://chromeisbad.com/): Chrome (and Keystone)

* * *

## **Job Listings**

- Passionate about DeFi? [Join us and drive BD at mStable](https://angel.co/company/mstable/jobs/1096364-business-development-manager)
- SigmaPrime is hiring a [blockchain security engineer](https://blog.sigmaprime.io/blockchain-security-engineer.html)
- 0x looking for [devs of all types](https://0x.org/about/jobs) and a [Matcha marketing manager](https://boards.greenhouse.io/0x/jobs/4923909002)
- Chainlink Labs is looking for a [DevOps Engineer (Monitoring)](https://jobs.lever.co/chainlink/41ffd762-bbf3-4254-80c5-d14243e39dfc?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Nexus Mutual: [experienced Solidity dev](https://angel.co/company/nexus-mutual-1/jobs/967538-smart-contract-engineer) in Euro timezones

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow the newsletter on twitter: [@WeekinEthNews](https://twitter.com/WeekInEthNews)

Permalink for this week’s issue:  [https://weekinethereumnews.com/week-in-ethereum-news-dec-20-2020/](https://weekinethereumnews.com/week-in-ethereum-news-dec-20-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Dec 22 - Deadline to apply for [proof of stake community grants](https://ethereum.org/en/eth2/get-involved/staking-community-grants/)
- **Jan 15 - Feb 7 - ETHGlobal’s [Market Make](https://marketmake.ethglobal.co/) hackathon**
- Feb 5-12 - [ETHDenver](https://twitter.com/EthereumDenver/status/1328367230707396609) (virtual)
- **[Apr 6-8](https://medium.com/ethcc/ethcc-4-6-7-8-april-2021-a9f6d306a941)** - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

---
title: "Week in Ethereum News <BR> Dec 13, 2020"
date: "2020-12-13"
---

## **Eth News and Links**

**Eth1**

- Geth [v1.9.25](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.25), last in 1.9 series. Working on snapshot db and sync for next major release
- Latest [core devs call](https://youtu.be/EPbZ4tU4P5A?t=172). Beiko’s [notes](https://twitter.com/TimBeiko/status/1337395528837996547), final steps for Berlin fork testnet
- Tim Beiko’s [1559 update](https://hackmd.io/@timbeiko/1559-updates/https%3A%2F%2Fhackmd.io%2F%40timbeiko%2F1559-update-004), mainnet-sized testnets coming
- Wang, Zheng, et al, paper: [ewasm slower than EVM in 256 bit](https://arxiv.org/pdf/2012.01032.pdf) and most 64 bit benchmarks

**EIPs/Standards**

- [EIP3155](https://eips.ethereum.org/EIPS/eip-3155): EVM trace specification
- [ERC3156](https://eips.ethereum.org/EIPS/eip-3156): flash loans

**Proof of Stake**

- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_201212)
- Latest [eth2 call](https://youtu.be/8mE--yxMZtk?t=42). Notes from [Ben](https://hackmd.io/@benjaminion/SJphODIiv) and [Mamy](https://gist.github.com/mratsim/d35a5171c52d3b998b492e9512f6cee7); everyone happy at how the chain is beating expectations
- A notebook on [performance of the first 1000 epochs](https://ethereum.github.io/rig/eth2data/notebooks/mainnet_explore.html)
- Understanding the [minimum needed slashing protection](https://alonmuroch-65570.medium.com/minimal-slashing-protection-45e679af235a)
- [Perfect is the enemy of the good](https://blog.ethereum.org/2020/12/10/validated-perfect-is-the-enemy-of-the-good/): most stakers don’t need to worry about going down; the design is very forgiving of going offline for days
- [Dangers of redundancy](https://www.adiasg.me/2020/12/11/eth2-staking-failover-redundancy.html): running multiple validators on same key will likely eventually lead to slashing
- Lakshman explains how [withdrawals will allow decentralized staking pools](https://www.lakshmansankar.com/#/staking-pools)
- Creating [eth2 withdrawal keys with ethdo](https://medium.com/coinmonks/creating-ethereum-2-withdrawal-keys-using-ethdo-6e41b14ddd7b)
- A guide to [staking on Mac with Lighthouse](https://lighthouse.sigmaprime.io/macos-guide.html) for those who don’t normally use terminal
- Etherchain’s [mobile app for validator monitoring](https://twitter.com/etherchain_org/status/1336949569498853377)

* * *

### **This newsletter is made possible thanks to [Chainlink](https://chain.link/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/12/FE39n5_g.png)

Chainlink oracles protect DeFi dApps against flash loan exploits and other market manipulation. Learn more about the importance of tamper-proof price oracles in Chainlink’s deep dive on [data quality for DeFi smart contracts](https://chn.lk/data-quality-for-defi)_._

* * *

**Stuff for developers**

- [Solidity Developer Survey 2020](https://blog.soliditylang.org/2020/12/09/solidity-developer-survey-2020/): tell Solidity what you want to see
- [Remix over the last 6 months](https://medium.com/remix-ide/remix-project-the-last-6-months-4a7ad00ff536). (Studio is being [deprecated](https://blog.ethereum.org/2020/12/07/we-are-sunsetting-studio/))
- [Scribble](https://github.com/ConsenSys/scribble) specification language and runtime verification tool
- [web3api](https://web3api.dev/#/) wasm standard for integrating eth into apps
- [web3j now has solidity dependency management](https://blog.web3labs.com/solidity-dependency-management-comes-to-web3j) for npm importing
- [Unity plugin to create NFTs](https://medium.com/arkane-network/our-unity-plugin-is-live-allowing-game-developers-to-create-nfts-on-matic-ethereum-43a0d6f03971) on Eth and Matic

**Security and incidents**

- [Symbolic execution with ds-test](https://fv.ethereum.org/2020/12/11/symbolic-execution-with-ds-test/) in hevm tutorial
- Trail of Bits’ Josselin Feist found an [unintialized proxy in Aave v1 and v2](https://medium.com/aave/aave-security-newsletter-546bf964689d) which could get self-destructed
- [Immunefi](https://immunefi.com/explore/): list of Ethereum bug bounties

**Ecosystem**

- Ethereum Foundation [comprehensive update](https://blog.ethereum.org/2020/12/09/ef-supported-teams-research-and-development-update-2020-pt-2/) on what every EF team is doing
- [Unlimited erc20 allowances considered harmful](https://kalis.me/unlimited-erc20-allowances/)

**Enterprise**

- JPMorgan: first [intraday repo market](https://www.businesswire.com/news/home/20201210005155/en/J.P.-Morgan-Executes-Intraday-Repo-Transaction-Using-Blockchain) transaction using JPMCoin and digitized Treasuries. Built on Ethereum/Quorum.
- [Two Japanese cities exploring online voting](https://www.coindesk.com/japan-city-kaga-blockchain-voting-id) on Ethereum
- International standards body OASIS names [Baseline Protocol their Outstanding New Initiative for 2020](https://www.oasis-open.org/2020/12/08/baseline-protocol-and-saml-win-2020-open-cup-awards-oasis-open-honors-jim-cabral-jane-ginn-and-bret-jordan/)
- Hyperledger Besu releases [Baseline Commitment Manager](https://www.oasis-open.org/2020/12/09/baseline-protocol-commitment-manager-brings-hyperledger-besu-infura-public-blockchain-clients-to-enterprise-workflows/)

**Application layer**

- Artist Beeple (1.7m instagram followers) [auctioning 2020 collection on Niftygateway](https://niftygateway.com/collections/beepletwo)
- [Rari is moving to Melon](https://medium.com/enzymefinance/rari-capital-moving-to-the-melon-protocol-84a10933228f); it appears Melon is rebranding as Enzyme
- Cent is going to allowed verified [Twitter accounts to sell NFTs of their tweet](https://beta.cent.co/cent/+usqwzk)

**Regulation/business/tokens**

- [Securities law and social tokens](https://medium.com/seedclub/securities-law-social-community-tokens-3bb0ffaae62)
- DeFi reveals that [Bitcoin’s supply cap is the emperor with no clothes](https://cointelegraph.com/news/the-butterfly-effect-why-defi-will-force-btc-to-break-its-21m-supply-ceiling)
- As [Brian Armstrong warned us](https://twitter.com/brian_armstrong/status/1331744884856741888), rumors flying that Trump administration will issue ill-thought regulations requiring KYC on self-hosted wallets. [Circle’s letter to Mnuchin](https://www.circle.com/hubfs/AllaireLetterUSTreasurySecretary.pdf) points out that the regulations would benefit China at America’s expense. [Four Republican representatives tell Mnuchin](https://twitter.com/WarrenDavidson/status/1336804544320327683) it’s a bad idea

**General**

- GridPlus’s [Lattice hardware wallet store](https://gridplus.io/lattice) is open for North America, Europe, and Singapore
- [Rogue Key attack](https://blog.sigmaprime.io/dkg-rogue-key.html) on Joint-Feldman and DKG
- [Brave Today](https://brave.com/announcing-brave-today/): a privacy-first RSS reader. Neat architecture (private CDN)
- [Electric Capital’s 2020 developer report](https://medium.com/electric-capital/electric-capital-developer-report-2020-9417165c6444) highlights Ethereum’s dominance

* * *

## **Job Listings**

- SigmaPrime is hiring a [blockchain security engineer](https://blog.sigmaprime.io/blockchain-security-engineer.html)
- 0x looking for [devs of all types](https://0x.org/about/jobs) and a [Matcha marketing manager](https://boards.greenhouse.io/0x/jobs/4923909002)
- Nexus Mutual: [experienced Solidity dev](https://angel.co/company/nexus-mutual-1/jobs/967538-smart-contract-engineer) in Euro timezones

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow the newsletter on twitter: [@WeekinEthNews](https://twitter.com/WeekInEthNews)

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-dec-13-2020/](https://weekinethereumnews.com/week-in-ethereum-news-dec-13-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Dec 17 - [Gitcoin grants matching](https://gitcoin.co/grants) ends (here’s [Week in Eth News](https://gitcoin.co/grants/237/week-in-ethereum-news))
- **Dec 19 - SiliconValleyEth: [Tim Roughgarden presentation](https://www.meetup.com/EthereumSiliconValley/events/275008164/)**
- **Dec 19-20 - [EthConKorea2020](https://ethcon.kr/)**
- Dec 22 - Deadline to apply for [proof of stake community grants](https://ethereum.org/en/eth2/get-involved/staking-community-grants/)
- Feb 5-12 - [ETHDenver](https://twitter.com/EthereumDenver/status/1328367230707396609) (virtual)
- Mar 2-4 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

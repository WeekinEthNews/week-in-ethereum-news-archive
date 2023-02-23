---
title: "Week in Ethereum News <BR> June 26, 2021"
date: "2021-06-26"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest [core devs call](https://www.youtube.com/watch?v=uhvhfxiC-NA&t=718s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1408459851349467136): 
    - Ropsten testnet upgraded to London, then stress tested
    - London upgrade block for mainnet ~ August 4, to be chosen after upgrading Goerli testnet
    - EIP3074 discussion
- Tim Beiko’s [All Core Devs Update](https://hackmd.io/@timbeiko/acd/https%3A%2F%2Fhackmd.io%2F%40timbeiko%2Facd-update-004): spec to turn off proof of work is finished on the staking side, working on the spec for mainnet clients, next upgrade in December to delay difficulty bomb will either be Shanghai or PoW turn off depending on which is ready
- Evan’s [benefits of EIP1559](https://twitter.com/evan_van_ness/status/1407784691718148100) tweet storm: UX, rollups, security, incentivize layer2 adoption and disincentivize short-term re-orgs
- [Fluffy](https://our.status.im/nimbus-fluffly/): ultra-light client mode of Nimbus client on portal network
- [Account abstraction](https://notes.ethereum.org/@axic/rybPKSz2_) using EVM Object Format
- State expiry depends on address periods, using a [prefix for address periods](https://ethereum-magicians.org/t/simple-non-address-length-extending-address-periods/6536) is an alternative to extending addresses from 20 to 32 bytes

**Proof of stake consensus layer**

- [EF Research Team AMA](https://www.reddit.com/r/ethereum/comments/o4unlp/ama_we_are_the_efs_research_team_pt_6_23_june_2021/); questions included: staking reward withdrawal (transfers), staking minimum < 32ETH, EIP1559 impact, exciting cryptographic techniques, economic inspiration, post-quantum cryptography and the difficulty bomb
- Beacon chain has > 170k active validators with [5% of ETH supply staked](https://twitter.com/eth2validators/status/1407848405435617286)
- [Data visualization of staking effectiveness](https://pintail.xyz/posts/validator-rewards-in-practice/): median efficiency > 98% for first 4 months
- [Nimbus v1.4.0](https://github.com/status-im/nimbus-eth2/releases/tag/v1.4.0): improved attestation effectiveness and CPU usage; [runs on Raspberry Pi3](https://twitter.com/jcksie/status/1407281364433571841), 2GB memory, SD card, full history ~13GB
- [SimpleSerialize (SSZ) visualizer](https://medium.com/@iaskeddiego/ssz-visualizer-online-83007de68ca2): input SSZ data and get visual representation of serialized and merkelized forms

* * *

### **This newsletter is made possible thanks to NEAR’s [Aurora](https://aurora.dev/) EVM and Bridge!**

![Aurora](https://weekinethereumnews.com/wp-content/uploads/2021/05/aurora-1024x341.jpeg)

Aurora is an Ethereum Layer-2 protocol that provides developers and users a seamless experience of Ethereum on top of [NEAR Protocol](https://near.org/): a scalable, developer-friendly blockchain platform for decentralized applications. Aurora’s design allows base fees to be paid in ETH or other ERC-20s and enables all existing ETH wallets and other tools to work out of the box. Users don’t even need to leave their MetaMask wallet while using Aurora. 

The Aurora environment consists of the Aurora Engine, a high performance EVM, and the Aurora Bridge, facilitating trustless transfer of ETH and ERC20 tokens between Ethereum and Aurora, within a seamless, familiar user experience. Join top ETH projects such as 1inch & DODO in building the multi-chain future. Start using [Aurora](https://aurora.dev/about) to scale your Ethereum project now. 

Don’t forget to follow Aurora on [Twitter](https://twitter.com/auroraisnear) and join our [Telegram](https://t.me/auroraisnear).

* * *

**Stuff for developers**

- Solidity [v0.8.6](https://blog.soliditylang.org/2021/06/22/solidity-0.8.6-release-announcement/): fixes unreachable code warning and optimizer setting
- Remix IDE [v0.13.0](https://medium.com/remix-ide/remix-ide-v0-13-0-is-released-e7117894ddb0): London version of JavaScript VM
- Coinbase [Solidify](https://blog.coinbase.com/introducing-solidify-a-tool-to-automatically-detect-and-classify-smart-contract-security-risks-73a1338fdbbe): detects contract features using a signature database, score risks and suggests mitigation strategies
- [Front end](https://twitter.com/dennisonbertram/status/1406701589289738241) for Gov Alpha deployer: create a token, governor, and timelock in one transaction
- [Custom error](https://medium.com/coinmonks/solidity-revert-with-custom-error-explained-with-example-d9dff8937ef4) (introduced in Solidity v0.8.4) tutorial using Remix or Hardhat
- [Ecrecover](https://soliditydeveloper.com/ecrecover) tutorial
- Opyn’s [Developer Toolkit](https://medium.com/opyn/introducing-opyn-developer-toolkit-2bfd5bcc7a92) for building options projects on top of Opyn

**Security**

- [38k ETH staked using Stakehound](https://stakehound.com/blog-post/fireblocks-eth-2-key-management-incident/) inaccessible due to loss of part of the withdrawal key
- [SharedStake](https://medium.com/immunefi/sharedstake-insider-exploit-postmortem-17fa93d5c90e) $500k alleged insider timelock exploit
- [Zapper Polygon Bridge post mortem](https://medium.com/zapper-protocol/post-mortem-polygon-bridge-vulnerability-cb8029275622): part of the rescue was front run by arbitrage bot, bot operator returned the intercepted funds to Zapper for distribution
- [Mushrooms Finance post mortem](https://medium.com/immunefi/mushrooms-finance-logic-error-bug-fix-postmortem-780122821621): logic error
- [Visor Finance beta incident report](https://medium.com/visorfinance/visor-beta-incident-report-1b2521b9266): $500k withdrawn via admin account

**Ecosystem**

- Flashbot searchers [gamed pricing and merging of bundles](https://twitter.com/bertcmiller/status/1407305924600029189)
- MyCrypto’s [common NFT scams](https://blog.mycrypto.com/common-nft-scams-to-avoid/): artist impersonation, brand impersonation, fake storefronts and deceitful bidding

**Enterprise**

- [Goldman Sachs swapped a US Treasury bond for digital dollars](https://www.bloomberg.com/news/articles/2021-06-22/goldman-sachs-begins-trading-on-jpmorgan-repo-blockchain-network) on JPMorgan’s blockchain network
- [Bank of Israel](https://en.globes.co.il/en/article-bank-of-israel-adopts-ethereum-for-digital-shekel-trial-1001375607) piloted digital shekel

**Application layer**

- [Reddit auctioning 3 CryptoSnoos NFTs](https://www.reddit.com/r/CryptoCurrency/comments/o6ms0b/introducing_cryptosnoosa_very_reddit_take_on_nfts/) on OpenSea that can be used as Reddit avatars
- [Sotheby’s auctioning Picasso](https://mashable.com/article/picasso-nft) with NFT signature of physical painting properties
- Jay-Z changes Twitter profile pic to a [Cryptopunk](https://www.theblockcrypto.com/post/109655/jay-z-puts-a-cryptopunk-nft-as-his-twitter-profile-picture) in advance of selling NFT through Sotheby’s
- [Risk Harbor](https://medium.com/riskharbor/risk-harbor-debuts-on-mainnet-with-a-new-round-of-funding-b18064dbd5dc) marketplace for DeFi risk management: mainnet launch with protection for Harvest and BarnBridge users

**Regulation/business/tokens**

- [UK regulator lists crypto asset businesses](https://register.fca.org.uk/s/search?predefined=U) that are not registered for AML
- [Model law for DAOs](https://coala.global/wp-content/uploads/2021/06/DAO-Model-Law.pdf): model set of rules that could be implemented internationally to provide legal certainty for DAOs
- Coopahtroopa’s [DAO Landscape](https://coopahtroopa.mirror.xyz/_EDyn4cs9tDoOxNGZLfKL7JjLo5rGkkEfRa_a-6VEWw): DAOs for grants, protocols, investments, service, social, collector and media

**General**

- Andreessen Horowitz [$2.2 billion fund](https://a16z.com/2021/06/24/crypto-fund-iii/) to invest in crypto
- [Private Signaling](https://eprint.iacr.org/2021/853.pdf): server-aided solution to the private signaling problem that guarantees full privacy for all recipients
- [Brave search](https://brave.com/brave-search-beta/) beta: no tracking or profiling of users, plans for paid ad-free search and free ad-supported search

* * *

## **Job Listings**

- NFT innovator SuperRare seeks [Director of Eng](https://superrare.breezy.hr/p/f1919c5bb07b-director-of-engineering) following Series-A fundraise
- [Garnet](https://careers.garnet.app/) is hiring web3 engineers to build better crypto community spaces
- [Anyblock is hiring](https://www.anyblockanalytics.com/careers/) an experienced Technical Writer, DevOps Engineer & more
- Unstoppable Domains is hiring for [Business Development, Crypto - Remote](https://grnh.se/e73546e24us)

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please post your news to an Ethereum subreddit; emails/DMs are not part of our workflow.

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-june-26-2021/](https://weekinethereumnews.com/week-in-ethereum-news-june-26-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- **June 30 - [DAO Summit](https://www.daocoop.org/) (virtual)**
- July 2 - [Gitcoin Grants Round 10](https://gitcoin.co/grants/explorer/) ends (support [Week in Eth News](https://gitcoin.co/grants/2785/week-in-ethereum-news))
- July 10 - Road to Devcon Quest: [Devcon Trivia Game](https://ethstaker.cc/road-to-devcon/)
- July 20-22 – [EthCC4](https://ethcc.io/) (Paris)
- **August 4** – [tentative date for London hard fork](https://docs.google.com/spreadsheets/d/1Y3yyTqeqRO1O2UFVkNkHK_V5oRulZd6y-JJbSnKYrb4) (Goerli June 30, Rinkeby July 7)
- **Aug 27-29** – [Edcon](https://www.edcon.io/) (Shenzhen/online)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

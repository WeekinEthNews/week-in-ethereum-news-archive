---
title: "Week in Ethereum News <BR> July 3, 2021"
date: "2021-07-03"
---

## **Eth News and Links**

**Mainnet execution layer**

- Goerli testnet [upgraded to London](https://twitter.com/nethermindeth/status/1410884599274692609), upgrade block for mainnet to be chosen next week
- Vitalik’s [statelessness, Verkle trees and state expiry AMA](https://www.reddit.com/r/ethereum/comments/o9s15i/impromptu_technical_ama_on_statelessness_and/): devs should start taking state expiry into account in contract design
- Piper’s [Core Dev apprenticeship program](https://snakecharmers.ethereum.org/the-core-developer-apprenticeship-program/) update: the process of finding and funding more people to work on state expiry and Verkle tries

**Proof of stake consensus layer**

- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210702): Ben is embracing the Eth2 nomenclature
- Prysmatic Labs [dropping Eth2 terminology](https://twitter.com/rauljordaneth/status/1409527165138391043) to reduce user confusion
- PoS [implementers call](https://www.youtube.com/watch?v=FNXk4ScqHn0&t=168s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/BJSvvGs2O): Altair devnet end of next week, upgrade Pyrmont testnet to Altair targeted for end of month
- Merge [implementers call](https://www.youtube.com/watch?v=6d944TCNpqc&t=24s). Notes from [Protolambda](https://notes.ethereum.org/@protolambda/BJdsuHjnO)
- [Teku v21.6.1](https://github.com/ConsenSys/teku/releases/tag/21.6.1): reduced CPU usage, improved peer ENR tracking and improved execution client tracking/metrics
- [Grandine](https://github.com/sifraitech/grandine): new Rust based client, currently closed source

**Layer2**

- [EY Nightfall 3](https://www.ey.com/en_gl/news/2021/07/ey-contributes-a-zero-knowledge-proof-layer-2-protocol-into-the-public-domain-to-help-address-increasing-transaction-costs-on-ethereum-blockchain): optimistic rollup with zero-knowledge private transfers, uses ~8200 gas per transaction
- [Rollup diff compression](https://ethresear.ch/t/rollup-diff-compression-application-level-compression-strategies-to-reduce-the-l2-data-footprint-on-l1/9975) to reduce the amount of mainnet gas used by rollups

* * *

### **This newsletter is made possible thanks to [Element Finance](https://www.element.fi/)!**

![Element Finance](https://weekinethereumnews.com/wp-content/uploads/2021/07/IMG_20210702_182909_267-1024x538.jpg)

[Element has officially launched](https://medium.com/element-finance/element-is-live-on-ethereum-mainnet-ae7c58cf2e57) on Ethereum Mainnet with crvLUSD as their first asset. 

You can now earn a fixed rate of 9.5% on your crvLUSD. 

Or go further by becoming an LP in Element Pools and earn additional APY! 

Next week, Element will be adding a new term for crvTriCrypto (currently ~30% APY), followed by DAI and USDC as they pursue their mission of bringing new fixed rate primitives to the DeFi ecosystem. 

* * *

**Stuff for developers**

- OpenZeppelin Contracts [v4.2](https://blog.openzeppelin.com/openzeppelin-contracts-4-2/): ERC20 voting extensions for governance, ERC20Wrapper and ERC1155 extension tracking total supply of each token id
- Understanding Compound’s [Governor Bravo](https://medium.com/tally-blog/understanding-governor-bravo-69b06f1875da)
- Ethers [v5.4.0](https://github.com/ethers-io/ethers.js/releases/tag/v5.4.0): EIP1559 support, TransactionResponse.gasPrice can now be null
- Web3.js [v1.4.0](https://github.com/ChainSafe/web3.js/releases/tag/v1.4.0): Berlin transaction support, defaults to Berlin when signing
- dapptools [v0.33.0](https://github.com/dapphub/dapptools/releases/tag/dapp%2F0.33.0): invariant tests and a FFI cheatcode
- Web3.py [London branch](https://snakecharmers.ethereum.org/web3-py-goes-to-london/): EIP1559 transaction support
- [Cairo playground](https://www.cairo-lang.org/playground/) adds deploying StarkNet contracts directly
- Hardhat [weekly downloads](https://twitter.com/gitpusha/status/1409572555611115525) overtakes Truffle for the first time
- [Hardhat-interface-generator](https://github.com/dmihal/hardhat-interface-generator): generate an interface from a Solidity contract
- Learn from [liquidation bot in Go](https://github.com/fxfactorial/liquidation-bot-fall-2020), circa Q3 2020
- [Burn Ether permanently](https://github.com/amanusk/burn4ever) proof of concept, burner gets 0.1% fee
- ERC20 token in a [tweet](https://twitter.com/wadealexc/status/1409861913119428610): 224 bytes of bytecode, base85 encoded, don’t use in production

**Security**

- NFTX v2 Punk token minting [exploit](https://blog.nftx.org/nftx-v2-punk-incident-post-mortem/)
- [SafeDollar](https://twitter.com/mudit__gupta/status/1409463917290557440) ~$250k infinite mint exploit on Polygon
- Researcher paid $200k for [Yearn vulnerability disclosure](https://github.com/yearn/yearn-security/blob/master/disclosures/2021-06-29.md) of a logic bug allowing bypass of the safety checks

**Ecosystem**

- ETHGlobal MEV summit [video](https://www.youtube.com/watch?v=s3nACF7uVZw&t=270s), [agenda and slides](https://hackmd.io/ivUzk3piQEG8ALzCGbxlag)
- [Etherscan](https://goerli.etherscan.io/blocks) shows total EIP1559 burn and % of fees burnt/tx fees earned
- [Otterscan](https://github.com/wmitsuda/otterscan): fast local block explorer using Erigon (formerly Turbogeth) archive node
- EF $5m in [Q1 grants](https://blog.ethereum.org/2021/07/01/esp-allocation-update-q1-2021/)

**Enterprise**

- [Compound Treasury](https://medium.com/compound-finance/announcing-compound-treasury-for-businesses-institutions-83d4484fb82e): enterprises send USD to Compound Labs and get paid fixed 4% interest

**Application layer**

- Twitter creates [140 NFTs](https://rarible.com/twitter?tab=created), 7 designs with 20 each, as an ERC1155 on Ethereum using Rarible
- [Element Finance](https://medium.com/element-finance/element-is-live-on-ethereum-mainnet-ae7c58cf2e57) live on mainnet: earn fixed 9.5% on your crvLUSD on 3 and 6 month terms; DAI and USDC pools coming
- Opyn [partially collateralized options](https://medium.com/opyn/opyn-partial-collateralization-how-to-trade-partially-collateralized-defi-options-3e23e8a201e)
- [one1INCH](https://medium.com/ichifarm/introducing-one1inch-a-stablecoin-for-better-payments-incentives-and-rewards-in-defi-2fc4d1331252): 1inch stable coin
- Andre Cronje [Fixed Forex](https://andrecronje.medium.com/introducing-fixed-forex-usd-eur-zar-ypy-cny-etc-e668b931a884): stable coin framework, no token, unaudited, unverified, experimental contract
- [An Old Dictator Appears](https://blog.synthetix.io/an-old-dictator-appears/): Kain runs for Spartan Council, will also return to coordinating Synthetix core contributors
- [MakerDAO fires back](https://forum.makerdao.com/t/response-to-chainlinkgod-accusations/9112) at Chainlink after community accusations
- Uniswap [v3 liquidity mining contracts](https://twitter.com/Uniswap/status/1410675488172003330) deployed to mainnet
- Simon de la Rouviere’s [story NFT memorabilia](https://untitledfrontier.substack.com/p/the-line-to-anchor-city-nft-memorabilia): SVG artwork and JSON metadata generated in the contract (Disclosure: I bought one of each)

**Regulation/business/tokens**

- [Wyoming DAO law](https://wyoleg.gov/2021/Introduced/SF0038.pdf) went into effect yesterday, recognizing DAOs as business formations
- Kain Warwick: forget Valley VC term sheets, go [DAO first for fundraising](https://blog.synthetix.io/dao-first-capital-formation/)
- [US Fed Vice Chair for Supervision](https://www.federalreserve.gov/newsevents/speech/quarles20210628a.htm): non-US CBDCs not a threat, no need to fear stablecoins but wants regulation for stability
- Dragonfly Research: [understanding ETH as an investment](https://medium.com/dragonfly-research/a-guide-to-understanding-eth-as-an-investment-6f0f393db591); valuation target implies ETH ~$50k

**General**

- [Bandersnatch](https://ethresear.ch/t/introducing-bandersnatch-a-fast-elliptic-curve-built-over-the-bls12-381-scalar-field/9957): fast elliptic curve built over the BLS12-381 scalar field
- [GitHub Copilot](https://copilot.github.com/): AI pair programmer (trained using public repositories)
- Vitalik [r/buttcoin](https://www.reddit.com/r/Buttcoin/comments/oac9lc/the_charles_ponzi_of_the_modern_era_answers/h3ldo00) reply: [what blockchain technology has done (better)](https://www.reddit.com/r/Buttcoin/comments/oac9lc/the_charles_ponzi_of_the_modern_era_answers/h3lf9g1)

* * *

## **Job Listings**

- NFT innovator SuperRare seeks [Director of Eng](https://superrare.breezy.hr/p/f1919c5bb07b-director-of-engineering) following Series-A fundraise
- EF seeking [Formal Verification Researcher](https://hackmd.io/@leoalt/fv-zk) for Zero Knowledge apps
- [WalletConnect](https://angel.co/company/walletconnect/jobs): Swift Engineer and Kotlin Engineer
- OpenZeppelin hiring a [Technical Recruiter](https://openzeppelin.com/jobs/opening/?gh_jid=4548720003) to drive the hiring process

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please post your news to an Ethereum subreddit; emails/DMs are not part of our workflow.

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-3-2021/](https://weekinethereumnews.com/week-in-ethereum-news-july-3-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- July 10 - Road to Devcon Quest: [Devcon Trivia Game](https://ethstaker.cc/road-to-devcon/)
- July 20-22 - [EthCC4](https://ethcc.io/) (Paris)
- **July 21 - [ETHécole Conference](https://medium.com/ethereum-magicians/ethecol%C3%A9-conference-all-you-need-to-know-7867dec7eaf6) (Paris)**
- **July 25-31 - [IC3 Blockchain Camp](https://www.initc3.org/events/2021-07-25-ic3-blockchain-summer-camp) (virtual)**
- August 4 - [tentative date for London hard fork](https://docs.google.com/spreadsheets/d/1Y3yyTqeqRO1O2UFVkNkHK_V5oRulZd6y-JJbSnKYrb4) (Rinkeby July 7)
- Aug 27-29 - [Edcon](https://www.edcon.io/) (Shenzhen/online)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

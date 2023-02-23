---
title: "Week in Ethereum News <BR> June 6, 2021"
date: "2021-06-05"
---

## **Eth News and Links**

**Mainnet execution layer**

- [OpenEthereum are sunsetting the legacy Parity codebase](https://medium.com/openethereum/gnosis-joins-erigon-formerly-turbo-geth-to-release-next-gen-ethereum-client-c6708dd06dd) and are instead [working on Akula](https://twitter.com/StefanDGeorge/status/1400925451887972354) (Rust version of Erigon - formerly Turbogeth). OpenEthereum v3 functionality including tracing being added to Erigon  
- Geth changing [default to snap sync from fast sync](https://github.com/ethereum/go-ethereum/pull/22973) ([~2hrs vs ~11hrs](https://blog.ethereum.org/2021/03/03/geth-v1-10-0/))
- London devnet named [Calaveras](https://github.com/ethereum/eth1.0-specs/blob/master/network-upgrades/client-integration-testnets/calaveras.md) fixes constraint issues that Martin Swende found
- [Python-based game](https://github.com/perama-v/gidget-gadget) to play with EIP1559 base fee mechanics
- [Analysis](https://notes.ethereum.org/@ipsilon/code-chunk-cost-analysis) on charging 350 gas for accessing code chunks
- Proof of concept [Geth devnet with verkle trees](https://twitter.com/gballet/status/1400815481569923075)

**EIPs/Standards**

- [EIP3601](https://github.com/ethereum/EIPs/issues/3601): Fractional NFT with Royalty Distribution system

**Proof of stake consensus layer**

- Latest [what’s new in PoS](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210605): 6 months of Beacon Chain - one major incident, >150k validators staking ~5m ETH
- [PoS implementers call](https://www.youtube.com/watch?v=cgH8OsCg9tY&t=86s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/HkCsML89u): close to finalizing the spec for the Altair upgrade
- [Merge implementers call](https://www.youtube.com/watch?v=j61FqoQwEHo&t=16s). Notes from [Protolambda](https://notes.ethereum.org/@protolambda/Hkg21v8qu), ironing out details for a production spec 
- Protolambda’s update on [sharding prototype](https://twitter.com/protolambda/status/1399436703669051394), to come after we turn off proof of work
- [Stop worrying about your validator uptime](https://www.reddit.com/r/ethstaker/comments/nnwfx1/why_you_should_stop_worrying_about_your/)

**Layer2**

- [Uniswap V3 live on Arbitrum](https://twitter.com/Uniswap/status/1400847744596598792) after community vote. Currently only for Arbitrum listed devs, no changes required once open to the public
- Interact and deploy to [Arbitrum mainnet via Alchemy](https://blog.alchemy.com/blog/arbitrum-is-live)
- Deep dive into [zkSync 2.0 architecture](https://twitter.com/zksync/status/1399469062539952128): includes zkEVM which supports most opcodes
- Non-technical [intro to rollups](https://www.mechanism.capital/rollups-introduction/)

* * *

### **This newsletter is made possible thanks to [Hardhat](https://hardhat.org/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2021/06/hardhat-rectangle-1024x325.png)

Hardhat is the Ethereum development environment for professionals. It’s flexible, it’s extensible, and it’s _fast_.

Easily deploy your contracts, run tests and debug Solidity code without dealing with live environments. Hardhat Network is a local Ethereum network designed for development. You get Solidity stack traces, console.log, and explicit error messages when transactions fail.

Check out the [documentation](https://hardhat.org/getting-started/), [plugin list](https://hardhat.org/plugins/) and [tutorial](https://hardhat.org/tutorial/) to get started. 

We’re also hiring for [senior systems engineers](https://nomiclabs.io/hiring) to expand our product offering.

* * *

**Stuff for developers**

- Update to [ethers v5.3.0+ to prevent a DoS issue in earlier versions of ws](https://twitter.com/ethersproject/status/1399565829650456576) if you’re using WebSockets in node and allow users to enter their own URL
- [JS-Waku](https://vac.dev/presenting-js-waku): library to use Waku v2 in the browser, dapps can send/receive p2p messages, query for missed messages and send with confirmations
- [NFT.Storage](https://nft.storage): free decentralized storage and bandwidth via IPFS and Filecoin
- [Approve and transfer ERC20 tokens atomically](https://twitter.com/thegostep/status/1399312917342785537) using Flashbots
- Solidity library to [read and write to a storage slot](https://docs.openzeppelin.com/contracts/4.x/api/utils#StorageSlot)
- Go-ethereum [transaction signer for AWS Key Management Service managed private keys](https://github.com/welthee/go-ethereum-aws-kms-tx-signer)
- [Circom and snarkJS library](https://blog.iden3.io/circom-snarkjs-plonk.html) now support PLONK
- [Open Source Insights](https://opensource.googleblog.com/2021/06/introducing-open-source-insights-project.html): interactive view of open source dependencies
- Ethereum Stackexchange [moderator elections](https://ethereum.stackexchange.com/election)

**Security**

- Tincho from OpenZeppelin: [make your auditors love you](https://twitter.com/tinchoabbate/status/1400170232904400897) tweet storm
- Due to the number of [projects on Binance Smart Chain being hacked](https://twitter.com/binancechain/status/1398838655481913346), we'll only mention them going forward if they are truly massive or technically interesting

**Ecosystem**

- MEV:
    - Vitalik: [Proposer/block builder separation](https://ethresear.ch/t/proposer-block-builder-separation-friendly-fee-market-designs/9725) friendly fee market designs
    - [MEV-SGX](https://twitter.com/bertcmiller/status/1399737488151830538): using secure enclaves to provide a private mempool and a sealed bid MEV auction
- ETHGlobal [Web3 Weekend finalists](https://twitter.com/ethglobal/status/1399107405665951747)
- [Uniswap V3 efficiencies causing CEX to reduce prices for stable swaps](https://twitter.com/haydenzadams/status/1399573590467567620)
- [Core devs apprentice program receives 400 applicants](https://twitter.com/trent_vanepps/status/1399817600486494209) for funding.  

**Enterprise**

- ConsenSys private transaction manager [Tessera integrated with Hyperledger Besu](https://consensys.net/blog/quorum/tessera-the-privacy-manager-of-choice-for-consensys-quorum-networks/). Orion being sunset
- [Norton 360 adding Ethereum mining](https://investor.nortonlifelock.com/About/Investors/press-releases/press-release-details/2021/NortonLifeLock-Unveils-Norton-Crypto/default.aspx) (reminder: PoW turning off in ~6-9 months)
- [Ethereum node to be installed on International Space Station](https://medium.com/blogspacechain/spacechain-empowers-customers-with-highly-secure-on-orbit-ethereum-multisignature-transaction-f9d2035cf834)

**Application layer**

- [Umbra](https://www.scopelift.co/blog/umbra-is-live): stealth address payment protocol beta live. Payer sends funds to a new address, controlled by the receiver and known only to both parties
- Uniswap [V3 fee calculator](https://uniswapv3.flipsidecrypto.com/)
- [Nexus Mutual yield token cover](https://nexusmutual.gitbook.io/docs/users/types-of-cover#yield-token-cover) for up to 90% of loss if yield bearing token de-pegs in value >10%, currently available for yEarn and Curve
- 1inch adds [flashbot transactions](https://help.1inch.io/en/articles/5300755-what-are-flashbot-transactions-and-how-do-they-work-on-1inch)
- [Matcha v2](https://matcha.xyz/blog/matcha-v2): fiat on-ramp via MoonPay and OTC trades avoid front-running or sandwich attacks
- [ETH flipped BTC in several metrics in May](https://twitter.com/lars0x/status/1399734913218355201) including [settling more value](https://money-movers.info/)

**Regulation/business/tokens**

- [Reserve Bank of India](https://rbi.org.in/Scripts/NotificationUser.aspx?Id=12103&Mode=0) advises banks not to use its repealed anti-crypto order from 2018
- [Google to allow US advertising for exchanges and wallets](https://support.google.com/adspolicy/answer/10688110#) (only banks and registered money transmitters)
- [Fee volume > PoS issuance](https://twitter.com/drakefjustin/status/1399326516199239680) even at 6 month low

**General**

- Mark Cuban: [all the things that crypto does better than its competitors](https://twitter.com/mcuban/status/1400459822080819204)
- [Public goods problems are coordination problems](https://s.mirror.xyz/djByMntM2rQF4tqUISYS2MAO3oCfSWoOZSOpZjsYwaw)
- Proposed design to [aggregate votes off-chain and validate on-chain](https://nikeshnazareth.github.io/vote-aggregation/) using polynomial commitments
- [Amazon devices will join wireless mesh network Sidewalk](https://arstechnica.com/gadgets/2021/05/amazon-devices-will-soon-automatically-share-your-internet-with-neighbors/) unless users opt out
- [Google according to court documents](https://www.businessinsider.com/unredacted-google-lawsuit-docs-detail-efforts-to-collect-user-location-2021-5) made it hard for users to find location privacy settings

* * *

## **Job Listings**

- [Argent is hiring](https://apply.workable.com/argenthq/) Layer 2 Solidity Engineers, JS Full Stack, iOS & Android
- Quant (DeFi Options): [Solidity Eng](https://jobs.lever.co/QuantLabs/e5178731-3101-477b-b1b0-73b455f149fa?lever-origin=applied&lever-source%5B%5D=week%20in%20ethereum), [Designer](https://jobs.lever.co/QuantLabs/e9b98ca2-c37c-41ff-938c-93f8a6a4c5cc?lever-origin=applied&lever-source%5B%5D=week%20in%20ethereum), [Marketing Lead](https://jobs.lever.co/QuantLabs/9730189f-65ec-4f91-86db-b92a5c5be29d?lever-origin=applied&lever-source%5B%5D=week%20in%20ethereum), [DevOps](https://jobs.lever.co/QuantLabs/ef7fd355-cc6b-4921-b2f6-1ed6664d86e0?lever-origin=applied&lever-source%5B%5D=week%20in%20ethereum)
- A leader in the NFT ecosystem, Immutable, are hiring a [Head of Blockchain](https://jobs.lever.co/immutable/9c796e83-3d62-4c2a-818b-9e3a136782d1?lever-origin=applied&lever-source%5B%5D=Ethereum%20news)
- Livepeer is hiring a [Protocol Engineer](https://livepeer.org/jobs/protocol-engineer)
- Kumavis from MetaMask is looking for a [JavaScript Security Engineer](https://twitter.com/kumavis_/status/1400640634789105666)
- [Nomic Labs are hiring](https://www.notion.so/Nomic-Labs-jobs-991b37c547554f75b89a95f437fd5056): Snr Software Engineer and Lead Software Architect

**Want to reach experienced Ethereum devs? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please post your news to an Ethereum subreddit; emails/DMs are not part of our workflow.

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-june-6-2021/](https://weekinethereumnews.com/week-in-ethereum-news-june-6-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- **June 16 - July 1 - proposed dates for [Gitcoin Grants Round 10](https://gitcoin.co/grants/explorer/)**
- **June 16 - July 7 - [Gitcoin Grants Round 10 Hackathon](https://gitcoin.co/hackathon/gr10/onboard)**
- June 18 – July 9 – [ETHGlobal – Hack Money 2021](https://hackmoney.ethglobal.co/)
- **June 23 - [Ethereum Foundation PoS team AMA](https://twitter.com/drakefjustin/status/1398375498342977544)**
- June 25-27 – [Edcon](https://www.edcon.io/) (Shenzhen/online)
- July 10 - Road to Devcon Quest: [Devcon Trivia Game](https://ethstaker.cc/road-to-devcon/)
- July 28 – [tentative date for London hard fork](https://docs.google.com/spreadsheets/d/1Y3yyTqeqRO1O2UFVkNkHK_V5oRulZd6y-JJbSnKYrb4) (Ropsten June 23, Goerli June 30, Rinkeby July 7)
- July 20-22 – [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

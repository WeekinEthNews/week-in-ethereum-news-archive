---
title: "Week in Ethereum News <BR> July 10, 2021"
date: "2021-07-10"
---

## **Eth News and Links**

**Mainnet execution layer**

- Mainnet upgrades to London at [block 12965000](https://github.com/ethereum/eth1.0-specs/pull/223), 1-5pm UTC [4 August](https://etherscan.io/block/countdown/12965000)
- Latest core devs [call](https://www.youtube.com/watch?v=OLCumSVoc0o&t=770s). Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1413532890747441158):
    - Rinkeby testnet upgraded to London
    - gasPrice field will use effective gas price for mined EIP1559 transactions but [field will eventually be removed](https://twitter.com/TimBeiko/status/1413536062429794304); instead use effectivegasprice from the transaction receipt
    - London-ready mainnet clients due to be released next week
    - For average 15m gas in a block London miners would need to target 30m, as EIP1559 aims for 50% full blocks 
    - [Geth](https://gist.github.com/zsfelfoldi/9607ad248707a925b701f49787904fd6) and [Erigon](https://github.com/ledgerwatch/erigon/wiki/Transaction-Pool-Design#design-proposal) EIP1559 transaction pool sorting approaches
    - Walkthrough of PoW switch off readiness checklist
    - Planning approach discussion for PoW turn off, Shanghai upgrade and client maintenance
- [Erigon receipt repair utility](https://twitter.com/mandrigin/status/1413094261537624065) for receipt users who upgraded from 2021.06.04 to 2021.06.05
- Initial analysis of [SELFDESTRUCT](https://hackmd.io/@albus/HJ6EBiTn_) usage for Verkle Tree proposal which includes removing most of the self destruct functionality
- Migrate EOAs to [validation focused smart contract wallets](https://ethereum-magicians.org/t/validation-focused-smart-contract-wallets/6603) with EIP3074
- Address Space Extension [working group call](https://www.youtube.com/watch?v=HSEEjoljb6g)
- Piper’s notes on the [header accumulator](https://notes.ethereum.org/KaMqlqxiQLCWyDoXCUCC4Q) to use in the Portal Network

**Proof of stake consensus layer**

- [Turning off Proof of Work](https://github.com/ethereum/pm/blob/master/Merge/mainnet-readiness.md): checklist of tasks before we can get rid of PoW forever
- First Beacon chain [upgrade to Altair on a devnet has finalized](https://twitter.com/terencechain/status/1413137159234543630)
- [Prototype of validator withdrawals](https://twitter.com/mkalinin2/status/1413434573208252420): demo and tutorial using local testnet
- Proposal for [smart contract triggered validator withdrawals](https://ethresear.ch/t/0x03-withdrawal-credentials-simple-eth1-triggerable-withdrawals/10021)
- [Data shard block format](https://ethresear.ch/t/suggested-format-for-shard-blob-header/9996) proposal to allow several application data bundles to coexist in one blob
- [Beacon Book](https://stateful.mirror.xyz/Y1ED9RorG9OvEUXD8NBmXgYhSVhjj8H537-I2SZJkYA): perspectives from Beacon chain researchers and implementers (Disclosure: bought an NFT)

**Layer2**

- [Synthetix enabling exchanges on Optimism](https://blog.synthetix.io/optimism-launch-announcement/) week of July 26
- Optimism stops [subsidizing L2 gas fees](https://blog.synthetix.io/oks-gas-update-weth-distribution/) and relaying user withdrawals, Synthetix giving WETH to existing users to cover several transactions
- [Arbitrum Update](https://offchain.medium.com/arbitrum-updates-standing-up-an-ecosystem-7666260a734b): a few infrastructure projects that are dependencies for dApps are not yet live, single ERC20 bridge being used
- Concern that users [won’t care about rollups](https://medium.com/dragonfly-research/im-worried--will-care-about-rollups-554bc743d4f1) when they launch
- [Dispute resolution](https://insights.deribit.com/market-research/making-sense-of-rollups-part-2-dispute-resolution-on-arbitrum-and-optimism/) comparison of Optimism and Arbitrum

* * *

### **This newsletter is made possible thanks to Synthetix’s [Kwenta](https://kwenta.io/)!**

![Kwenta](https://weekinethereumnews.com/wp-content/uploads/2021/04/IMG_20210418_190328_618-1024x512.jpg)

[Kwenta](https://kwenta.io/) enables traders to access real-world and derivative assets on-chain with zero slippage using the power of the [Synthetix](https://synthetix.io/) protocol.

Trade popular synthetic cryptocurrencies, commodities, forex, and equities, such as TSLA, COIN, and FAANG stocks, without the limits or compromises of a centralized exchange.

Try [Kwenta](https://kwenta.io/) today!

* * *

**Stuff for developers**

- EthereumJS [releases](https://twitter.com/EFJavaScript/status/1413090893389828096) with finalized support for London upgrade
- Andre Cronje released [5 prototypes](https://twitter.com/AndreCronjeTech/status/1411244286146977792) for learning and to inspire teams to form around them
- [Local ERC20 balance manipulation](https://kndrck.co/posts/local_erc20_bal_mani_w_hh/) using Hardhat, useful for testing with DeFi tokens
- EVM opcodes reference [updated for London](https://github.com/wolflo/evm-opcodes/pull/13/files)
- [EthernautDAO](https://twitter.com/the_ethernaut/status/1412576783178813441) aims to convert senior developers to Ethereum devs
- [Build an NFT marketplace](https://dev.to/dabit3/building-scalable-full-stack-apps-on-ethereum-with-polygon-2cfb), using Next.js, Tailwind, Hardhat and Ethers.js on EVM testnet
- [x \* y = k AMM](https://monokh.com/posts/uniswap-from-scratch) line by line explainer

**Ecosystem**

- Philip Daian: no official Flashbot software or materials for extracting [MEV from reorgs](https://twitter.com/phildaian/status/1413480058677731330)
- Sandwich bots increasing in complexity, [4 transactions sandwiched](https://twitter.com/bertcmiller/status/1412740149155352578)
- ETH Global [Hack Money 2021 finalists](https://twitter.com/ethglobal/status/1413577852520484883)
- Etherscan displays [EIP1559 savings](https://twitter.com/TimBeiko/status/1412995748665298944) per transaction
- Modeling [Governance Extractable Value](https://twitter.com/aklamun/status/1412757593097916419): DAOs have billion $ treasuries at stake

**Enterprise**

- Singapore and France central banks test [cross border payment](https://www.mas.gov.sg/news/media-releases/2021/monetary-authority-of-singapore-and-banque-de-france-break-new-ground-in-cbdc-experimentation) using simulated Singapore Dollar and Euro CDBCs on J.P. Morgan’s Onyx

**Application layer**

- [Maker activates flash minting](https://twitter.com/brianmcmichael/status/1413264238710333440): 0.05% fee to flash mint up to 500 million DAI
- [daistats.com](https://twitter.com/sgmacpherson/status/1412802352210493452) shows total amount of collateral backing DAI and DAI minted by collateral type, < 35% of collateral backing DAI is USDC
- Reflexer Labs [pilots self repaying RAI loans](https://medium.com/reflexer-labs/rai-times-the-inaugural-issue-3db62e3df99d) using reserves
- [Leasing a Tesla](https://aaron.ng/posts/defi-tesla-lease/) with DeFi yield (Liquity and Curve staking)
- [Andre Cronje launches bridge to Goerli testnet](https://thedefiant.io/cronjes-goerli-move-triggers-confusion-and-dreams-of-instant-wealth/) which would make it value-bearing and not a testnet
- [Axie Infinity made >$1million](https://twitter.com/phabcd/status/1413133873077125126) in revenue in a single day, comparable with biggest AAA games
- [OpenSea permissive approach](https://twitter.com/natechastain/status/1411442112462266371) to derivatives/homages, DMCAs still apply
- [NFTX v2 creates liquidity](https://mobile.twitter.com/dareal_sisyphe/status/1412812020991266825) for NFTs at the floor price
- Mooncat adds designer and boutique for [accessories](https://mooncat.community/blog/accessories-launch)

**Regulation/business/tokens**

- USDC issuer [Circle going public](https://www.circle.com/blog/circle-to-become-a-public-company) on NYSE, [forecasts USDC in circulation](https://www.circle.com/hubfs/investors/Circle-Investor-Presentation-July2021.pdf) of $35billion for 2021 and $194billion for 2023
- German regulator allows funds for institutions to [allocate 20% of assets to cryptocurrencies](https://www.ft.com/content/c523fa52-25da-4d7e-8378-cc58bd1e6c89)
- [Token Terminal](https://twitter.com/tokenterminal/status/1412774591894855684?s=20) adds price to earnings (P/E) ratio for protocols
- [ETH liquidity crunch](https://twitter.com/SquishChaos/status/1413345944116940810) coming from staked Ether and EIP1559
- Tweetstorm of [24 reasons why](https://twitter.com/CroissantEth/status/1412574228973563909?s=20) ETH is undervalued

**General**

- China’s crackdown on mining: [BTC difficulty adjusts down ~28%](https://insights.glassnode.com/the-week-on-chain-week-27-2021/)
- [JPMorgan analysts](https://twitter.com/santiagoroel/status/1411345440793038849) expect blockchain staking rewards to reach $40 billion by 2025
- [Kaspersky Password Manager](https://donjon.ledger.com/kaspersky-password-manager/) previously used a PRNG not suited for cryptography, with current time single source of entropy
- Opsec vulnerability: [online dating wrench attack](https://blog.keys.casa/casa-client-case-study-the-tinder-trap/)

* * *

## **Job Listings**

- NFT innovator SuperRare seeks [Director of Eng](https://superrare.breezy.hr/p/f1919c5bb07b-director-of-engineering) following Series-A fundraise
- Sourcify looking for an [experienced TypeScript developer](https://ethereum.bamboohr.com/jobs/view.php?id=38)
- Kwenta Open Position: [Solidity Engineer](https://blog.kwenta.io/kwenta-open-position-solidity-engineer/)

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-10-2021/](https://weekinethereumnews.com/week-in-ethereum-news-july-10-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- **July 15 - [OpenZeppelin secure development series](https://zpl.in/security_series) 1st of 6**
- **July 16 - applications close for [ETH Summer](https://summer.ethuniversity.org/) undergrad program (virtual)**
- July 20-22 - [EthCC4](https://ethcc.io/) (Paris)
- July 21 - [ETHécole Conference](https://medium.com/ethereum-magicians/ethecol%C3%A9-conference-all-you-need-to-know-7867dec7eaf6) (Paris)
- July 25-31 - [IC3 Blockchain Camp](https://www.initc3.org/events/2021-07-25-ic3-blockchain-summer-camp) (virtual)
- **July 26+30 - [OpenZeppelin/ITBA free course](https://twitter.com/marquitos_eth/status/1411868494115786752) for devs in Spanish**
- **July 30 - Aug 20 - ETHGlobal & Protocol Labs [HackFS](https://fs.ethglobal.co/) hackathon**
- **August 4 - [London hard fork](https://docs.google.com/spreadsheets/d/1Y3yyTqeqRO1O2UFVkNkHK_V5oRulZd6y-JJbSnKYrb4)**
- Aug 27-29 - [Edcon](https://www.edcon.io/) (Shenzhen/online)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

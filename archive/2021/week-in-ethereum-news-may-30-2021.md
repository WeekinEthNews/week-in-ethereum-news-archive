---
title: "Week in Ethereum News <BR> May 30, 2021"
date: "2021-05-30"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest [core devs call](https://www.youtube.com/watch?v=7MSYLbn-Xro&t=508s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1398329483434741762): 
    - EIP1559 - adding explicit constraints to prevent attacks using arbitrarily large transactions, new devnet Calaveras
    - Unofficial London mainnet date now July 28 due to EIP1559 changes
    - Gas DoS protection discussion - separate transaction pool to guard against execution attacks
    - EIP3584 - add access lists to blocks
- EIP1559
    - [Setting expectations](https://twitter.com/trent_vanepps/status/1397959686247301123): legacy transactions are still valid, mechanism may need tweaking based on mainnet learning, wallets and gas APIs may need time to set optimal values
    - [Addressing community concerns](https://twitter.com/gakonst/status/1397855965429612547)
    - Beiko’s [list of EIP1559 resources](https://hackmd.io/@timbeiko/1559-resources)
- [EthereumJS releases](https://twitter.com/EFJavaScript/status/1397859663295746048) (VM, Tx, Block and others) for London/EIP1559
- Erigon (formerly TurboGeth) adds [pruning node options](https://twitter.com/vorot93/status/1397900505834266626): <500GB with block history, ~100GB without block history
- Samczsun found a way for an attacker to make [fast-synced Geth nodes fork off mainnet](https://www.paradigm.xyz/2021/05/booby-trapping-the-ethereum-blockchain/)

**EIPs/Standards**

- [EIP3589](https://github.com/ethereum/EIPs/pull/3589): Assembly NFT

**Proof of stake consensus layer**

- Danny Ryan’s [Finalized](https://blog.ethereum.org/2021/05/25/finalized-no-26/) PoS update: Altair upgrade specs stabilized, client teams focused on London/Altair upgrades, researchers are refining and testing merge spec
- Vitalik’s [annotated spec for the Altair upgrade](https://github.com/ethereum/annotated-spec/blob/master/altair/beacon-chain.md)
- [Lodestar (TypeScript client) update](https://medium.com/chainsafe-systems/lodestars-recent-progress-metrics-and-other-oddities-49c6e646e421): light client prototype, out-of-memory resolved, 50–75% profitability compared to network average
- A guide to Ethereum PoS’s [Simple Serialize (SSZ)](https://www.ssz.dev/)
- Data visualization of [staker behavior](https://crypto.omnianalytics.io/2021/05/14/tiering-and-dashboarding-eth-2-0-validator-behavior/)
- [Kate commitments](https://hackmd.io/yqfI6OPlRZizv9yPaD-8IQ), an implementation perspective

**Layer2**

- [Arbitrum mainnet beta](https://offchain.medium.com/introducing-arbitrum-one-our-mainet-beta-ed0e9b63b435) is live, onboarding developers now, open access at least two weeks away, fees paid in ETH, [Etherscan support in July](https://offchain.medium.com/etherscan-is-coming-to-arbitrum-4f41edaff100)
- Uniswap community support for [Arbitrum deployment of Uniswap v3](https://twitter.com/haydenzadams/status/1397675094001045508)
- [Nitro virtual channels](https://blog.statechannels.org/virtual-channels/) to create a channel network
- [Adamantium protocol](https://ethresear.ch/t/adamantium-power-users/9600) from StarkWare is a flavor of Validium where a user can keep their own offchain data
- [Faster finality in zkrollups](https://ethresear.ch/t/checkpoints-for-faster-finality-in-starknet/9633) using validity proof checkpoints
- [zkSync upgrade](https://medium.com/matter-labs/zksync-1-x-swaps-nfts-event-system-and-permissionless-token-listing-e126fcc04d61): NFTs and swaps on testnet in advance of going live 2 weeks after upgrade (time locked)

* * *

### **This newsletter is made possible thanks to NEAR’s [Aurora](https://aurora.dev/) EVM and Bridge!**

![Aurora](https://weekinethereumnews.com/wp-content/uploads/2021/05/aurora-1024x341.jpeg)

Aurora is an Ethereum Layer-2 protocol that provides developers and users a seamless experience of Ethereum on top of [NEAR Protocol](https://near.org/): a scalable, developer-friendly blockchain platform for decentralized applications. Aurora’s design allows base fees to be paid in ETH or other ERC-20s and enables all existing ETH wallets and other tools to work out of the box. Users don’t even need to leave their MetaMask wallet while using Aurora. 

The Aurora environment consists of the Aurora Engine, a high performance EVM, and the Aurora Bridge, facilitating trustless transfer of ETH and ERC20 tokens between Ethereum and Aurora, within a seamless, familiar user experience. Join top ETH projects such as 1inch & DODO in building the multi-chain future. Start using [Aurora](https://aurora.dev/about) to scale your Ethereum project now. 

Don’t forget to follow Aurora on [Twitter](https://twitter.com/auroraisnear) and join our [Telegram](https://t.me/auroraisnear).

* * *

**Stuff for developers**

- Remix supports [decoding custom errors](https://twitter.com/ethchris/status/1397189633235161093)
- [WalletConnect Remix plugin](https://medium.com/remix-ide/remix-ide-now-has-a-walletconnect-plugin-cd6c5f9d70f5): allows Remix Desktop to deploy on public networks and devs can mimic users paying on mobile
- [Ape](https://github.com/ApeWorX/ape): framework for Web3 Python apps and smart contracts, alpha release
- [JollyRoger dapp template](https://jolly-roger.eth.link/) with hot contract replacement: now uses svelte-kit with IPFS adaptor
- [ERC20 tokens and modifiers](https://github.com/ZeframLou/mev-token) to allow use for only MEV and no MEV
- Mariano Conti: [live coding to create an ERC20 using Dapp tools](https://nanexcool.medium.com/creating-your-own-erc20-token-in-more-than-2-hours-f0846bc34c9c)
- Using [Uniswap V3 in your contracts](https://soliditydeveloper.com/uniswap3)
- [Transaction tracing with Ethernal](https://blog.tryethernal.com/transaction-tracing-with-ethernal/): block explorer for private/local chains including Hardhat Network and Ganache
- [Ethcode](https://medium.com/ethential/ethcode-and-other-ethereum-devtools-f789d2373ed9) updates: load Solidity JSON, JSON tree view, Remix VS Code extension
- [TrueBlocks dynamic traversers](https://tjayrush.medium.com/dynamic-traversers-in-trueblocks-7e2215cb1af9): account transaction history in 10 lines of C++

**Security**

- Mushrooms Finance [theft of yield frontrunning vulnerability fix](https://medium.com/immunefi/mushrooms-finance-theft-of-yield-bug-fix-postmortem-16bd6961388f) postmortem
- WildCredit [unprotected initialize](https://twitter.com/Mudit__Gupta/status/1397888546686398470) exploited for $600k - funds returned by front runner
- Binance Smart Chain attacks:
    - [~$7m Burgerswap exploit](https://twitter.com/haydenzadams/status/1398132414199873537): UniswapV2 fork with x\*y=k check removed, could be trivially drained
    - [~$6m Belt Finance exploit](https://twitter.com/FrankResearcher/status/1398772580602060804): price manipulation using bug in the strategy balance calculations
    - Bunny forks attacked: [AutoShark](https://watchpug.medium.com/sharkfinance-performance-fee-minting-incident-analysis-4b2e3bd03923) & [Merlin](https://watchpug.medium.com/merlin-lab-performance-fee-minting-incident-analysis-12571b591eb3)
- [Post-hack playbook](https://medium.com/immunefi/what-to-do-after-youve-been-hacked-8d2e838a2d65): war rooms and crisis management

**Ecosystem**

- [Flashbots v0.2](https://twitter.com/bertcmiller/status/1396961882121121799): bundle merging allows miners to include multiple bundles per block
- ENS keyholders removed their [ability to replace the .eth registrar](https://twitter.com/nicksdjohnson/status/1398060124720091136)
- [History of apps gas usage](https://www.nansen.ai/research/through-the-looking-gas-a-history-of-ethereum-protocols) data visualization
- Justin Drake: [ETH deserves a Unicode character](https://twitter.com/drakefjustin/status/1397930556763955200)

**Enterprise**

- [Gamestop creating blockchain division](https://twitter.com/finestonematt/status/1397309790964047872), announced with [1/1 NFT](https://etherscan.io/address/0x13374200c29c757fdcc72f15da98fb94f286d71e#code)

**Application layer**

- [mistX](https://alchemistcoin.medium.com/introducing-mistx-78066e140e13): gasless dex built on FlashBots; transaction fee charged as part of swap
- [BackRunMe](https://medium.com/bloxroute/there-is-light-in-the-dark-forest-2d7b77f4ca2d): use Bloxroute to send transactions privately and if the transaction creates a backrunning opportunity, then you get 25% share of the backrunning profit
- [Gitcoin’s DAO](https://gitcoin.co/blog/introducing-gtc-gitcoins-governance-token/) for fund allocation, matching pools, and grant collusion; airdrop claimers select delegate prior to receiving tokens
- Non-transferrable (initially) governance token by [Ribbon Finance](https://ribbonfinance.medium.com/decentralizing-ribbon-governance-395950da7a6) to ensure only used for governance
- [Selling music](https://twitter.com/JackSpallone/status/1398334164160729093) in the streaming era: (pre release) canon - 1/1, collectible - 1/n, streaming - 1/∞
- [NFT multisender](https://twitter.com/rstormsf/status/1396853563494600713): send multiple ERC721/ERC1155 tokens in a transaction
- [Pilot of weather index insurance](https://medium.com/finx-vc/finx-pilot-smart-contract-based-weather-index-insurance-in-kenya-part-1-d7a59eba644e) with 10k smallholder farmers in Kenya

**Regulation/business/tokens**

- Packy McCormick's Ethereum bull case: [like owning a piece of the internet](https://www.notboring.co/p/own-the-internet)
- [Carl Icahn on Bloomberg TV](https://cryptobriefing.com/carl-icahn-bullish-ethereum-may-invest-1-5b-crypto/): “Ethereum has two things: you can use it as a payment system and you can use it as a store of value.” 
- Goldman Sachs report: “[Ether beats bitcoin as a store of value](https://www.goldmansachs.com/insights/pages/crypto-a-new-asset-class-f/report.pdf)”
- Bankless: [the Flippening is inevitable](https://newsletter.banklesshq.com/p/the-flippening-is-inevitable)
- Second ETH [ETF application](https://www.sec.gov/Archives/edgar/data/0001864519/000119312521175426/d153307ds1.htm) with SEC from WisdomTree
- [SEC sues Bitconnect promoters](https://www.sec.gov/litigation/complaints/2021/comp-pr2021-90.pdf) for selling unregistered securities
- UNI proposal to [fund crypto policy/lobbying](https://gov.uniswap.org/t/temperature-check-funding-a-political-defense-of-defi/12557)

**General**

- WSJ [profile of Uniswap](https://www.wsj.com/articles/upstart-peer-to-peer-crypto-exchanges-take-aim-at-coinbase-11621848601)
- [Paypal & Venmo](https://www.coindesk.com/paypal-will-let-customers-withdraw-crypto-exec-says) to allow transfer to third party wallets
- [$2 trillion volume](https://twitter.com/fintechfrank/status/1398112145288712193) for crypto exchanges in May
- Vitalik is in favor of real world [elections on blockchains](https://vitalik.ca/general/2021/05/25/voting2.html); confine to small experiments short term
- [M1RACLES](https://m1racles.com/) covert channel vulnerability in the Apple M1 chip
- [Half-Double (Rowhammer variation) attack on RAM](https://therecord.media/google-says-rowhammer-attacks-are-gaining-range-as-ram-is-getting-smaller/), that can bypass Target Row Refresh mitigation
- [Cryptanalysis of an oblivious PRF from supersingular isogenies](https://eprint.iacr.org/2021/706) paper

* * *

## **Job Listings**

- A leader in the NFT ecosystem, Immutable, are hiring a [Head of Blockchain](https://jobs.lever.co/immutable/9c796e83-3d62-4c2a-818b-9e3a136782d1?lever-origin=applied&lever-source%5B%5D=Ethereum%20news)
- Livepeer is hiring a [Protocol Engineer](https://livepeer.org/jobs/protocol-engineer)
- Ethereum.org are seeking a [Community & Ecosystem Lead](https://ethereum.org/en/about/community-lead/)
- Nethermind: Hiring [interns, software engineers, researchers & devops](https://twitter.com/nethermindeth/status/1397109477334261762)

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of the workflow.

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-may-30-2021/](https://weekinethereumnews.com/week-in-ethereum-news-may-30-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- May 31 – deadline to apply for [Eth core dev apprenticeship](https://blog.ethereum.org/2021/05/13/core-dev-apprenticeship/)
- **June 3 – OpenZeppelin [automate smart contract workflows](https://openzeppelin.zoom.us/webinar/register/4316221282507/WN_s9cUl_XASYm6fOSS7DlO0g) workshop**
- June 18 – July 9 – [ETHGlobal – Hack Money 2021](https://hackmoney.ethglobal.co/)
- June 25-27 – [Edcon](https://www.edcon.io/) (Shenzhen/online)
- July 10 - Road to Devcon Quest: [Devcon Trivia Game](https://ethstaker.cc/road-to-devcon/)
- **July 28 – [tentative date for London hard fork](https://docs.google.com/spreadsheets/d/1Y3yyTqeqRO1O2UFVkNkHK_V5oRulZd6y-JJbSnKYrb4) (Ropsten June 23, Goerli June 30, Rinkeby July 7)**
- July 20-22 – [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

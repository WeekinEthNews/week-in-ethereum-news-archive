---
title: "Week in Ethereum News <BR> June 19, 2021"
date: "2021-06-19"
---

## **Eth News and Links**

**Mainnet execution layer**

- Tim Beiko’s [London announcement](https://blog.ethereum.org/2021/06/18/london-testnets-announcement/): testnet blocks, client versions and upgrade FAQ
- [Geth v1.10.4](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.4): snap sync now default, ~7 hours to sync a Geth node
- [State expiry call](https://consensysmesh.zoom.us/rec/play/VoftjeRO0xNFHObLZpot-r0hTj0U6ZG0fUKORwQzy2qoh-JlweRgL6hj5UxqC8WsdYW3IOVBc6l_912R.ND8fJB672c-EpG1T?_x_zm_rhtaid=872&_x_zm_rtaid=Jhbf_Q6fTx-tPJB7vFllMg.1623863913448.e6b0045131eec8ea5666c579c3b613b7&autoplay=true&continueMode=true&startTime=1623848674000) going through Vitalik’s [state expiry and statelessness roadmap](https://notes.ethereum.org/@vbuterin/verkle_and_state_expiry_proposal): annual expiry of state, only require block producers to store state and other nodes can be stateless
- Vitalik’s [Verkle tree explainer](https://vitalik.ca/general/2021/06/18/verkle.html): Verkle trees allow proofs < 150 bytes making stateless clients viable
- [Trin (Rust portal network client) update](https://snakecharmers.ethereum.org/trin-development-update/): fully functional JSON RPC light client, talking with other clients, next step transmit data
- Alternative to [EIP3074](https://ethereum-magicians.org/t/a-case-for-a-simpler-alternative-to-eip-3074/6493) and a critique
- [EVM Object Format](https://notes.ethereum.org/@ipsilon/evm-object-format-overview) (EOF) explainer
- [Analysis of memory copying in contracts](https://notes.ethereum.org/@ipsilon/evm-mcopy-analysis) and potential savings using the proposed MCOPY opcode

**EIPs/Standards**

- [Proto-EIP](https://notes.ethereum.org/@vbuterin/verkle_tree_eip): verkle trees

**Proof of stake consensus layer**

- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210618): Pyrmont and Prater testnet validators need to update their Goerli nodes prior to London upgrade
- [PoS implementers call](https://www.youtube.com/watch?v=ZSMrxG1LAck&t=12s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/SJoLSp_s_): upgrade a testnet to Altair in ~4 weeks, mainnet Altair upgrade early August
- [Merge implementers call](https://www.youtube.com/watch?v=b5gh0Mw2oPU&t=3s). Notes from [Protolambda](https://notes.ethereum.org/@protolambda/Sy54x0_iO): EIP needed for setting DIFFICULTY opcode value, merge research near-completion, coming up - rebase merge work on Altair

**Layer2**

- [Starknet zkrollup alpha](https://medium.com/starkware/starknet-planets-alpha-on-ropsten-e7494929cb95): Ropsten testnet, smart contracts written in Cairo
- [Raiden Light Client](https://raiden-network.medium.com/announcing-the-raiden-light-client-ashvini-release-60d2a66b0d4): Typescript implementation that runs in an Ethereum enabled browser

* * *

### **This newsletter is made possible thanks to [Celer](https://www.celer.network/)’s [layer2.finance](https://layer2.finance/)!**

![Celer](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

[Celer](http://celer.network/) is a coherent layer-2 scaling platform on Ethereum powered by [Generalized State Channel Network](https://www.celer.network/docs/celercore/index.html) and [Rollup](https://medium.com/celer-network/adding-hybrid-pos-rollup-sidechain-to-celers-coherent-layer-2-platform-d1d3067fe593) technology. 

Celer recently launched [Layer2.finance](https://layer2.finance/), a layer-2 rollup-based DeFi aggregator that acts as a low-cost and trust-free gateway for the users to explore and benefit from the existing DeFi ecosystem with 100X lower cost. Layer2.finance achieves scalability “in-place” with no protocol migration needed and therefore, does not cause liquidity fragmentation or break composability. You can use the app here: [app.l2.finance](https://app.l2.finance/). 

Follow Celer on [twitter](https://twitter.com/CelerNetwork), [blog](https://blog.celer.network/), [discord](https://discord.com/invite/Trhab5w) and [telegram](https://t.me/celernetwork).

* * *

**Stuff for developers**

- [Hardhat v2.4.0](https://github.com/nomiclabs/hardhat/releases/tag/hardhat-core-v2.4.0): Solidity 0.8: custom errors and panic codes; Hardhat Network: minimum gas price to simulate network conditions, transaction replacement and new RPC methods
- Solidity team seeking feedback on requested feature: [user-defined value types](https://forum.soliditylang.org/t/user-defined-value-types/314)
- [App template](https://github.com/ScopeLift/vue-tailwind-ethereum-template) with Vue 3, Tailwind CSS, Ethers, Multicall2, Blocknative onboarding, dark mode and Vite
- [PRBMath v2](https://github.com/hifi-finance/prb-math/releases/tag/v2.0.0): adds type safety
- [Weiroll](https://twitter.com/nicksdjohnson/status/1405644379067351043): chain contract operations (early stage, don’t use on mainnet yet)
- [ChainSafe Gaming SDK](https://medium.com/chainsafe-systems/announcing-chainsafe-gaming-an-sdk-to-bridge-your-gaming-engines-to-the-web-3-0-ecosystem-f33aa27c7a98): beta for Unity
- [Eauth](https://github.com/pelith/node-eauth-server): OAuth2-compatible service using Ethereum credentials to authenticate users on websites

**Security**

- [Alchemix alETH incident report](https://forum.alchemix.fi/public/d/137-incident-report-06162021): users could withdraw collateral due to incorrect indexing of vaults in array
- Zapper: [Sushiswap/Uniswap v2 Zap out exploit](https://medium.com/zapper-protocol/post-mortem-sushiswap-uniswap-v2-zap-out-exploit-84e5d34603f0) post mortem and [Polygon bridge](https://twitter.com/zapper_fi/status/1405287845971914757) vulnerability
- Tincho (OpenZeppelin) [guidelines for projects doing a fast mainnet launch](https://twitter.com/tinchoabbate/status/1405873466365128712)

**Ecosystem**

- [Watch how much ETH gets burnt with EIP1559](http://watchtheburn.com/): live on Calaveras devnet
- [MEV payments](https://twitter.com/bertcmiller/status/1405234475680862210) from Flashbots as a % of transaction fees increasing 
- [Sandwiched.wtf](https://sandwiched.wtf/): amount of MEV made by sandwiching your trades
- 5 years since [The DAO](https://blog.slock.it/the-history-of-the-dao-and-lessons-learned-d06740f8cfa5) hack on June 17
- [23% of ETH in smart contracts](https://thedailygwei.substack.com/p/dude-wheres-my-eth-the-daily-gwei), same percentage as at time of The DAO

**Enterprise**

- [Medoxie digital health passport](https://consensys.net/blog/quorum/the-chinese-university-of-hong-kong-and-consensys-announce-the-medoxie-covid-19-digital-health-passport) in Hong Kong uses Quorum to record COVID-19 events: test results, temperature checks, vaccinations, and immunity

**Application layer**

- [Instadapp governance](https://blog.instadapp.io/inst) live with airdrop for Maker, Aave and Compound users, includes liquidity mining for managing your DeFi position in InstaDapp
- [Volmex Finance](https://blog.volmex.finance/volmex-v1-mainnet/) live on mainnet: tokenized 30-day implied volatility, currently available for ETH and BTC 
- Element’s [de-collateralize](https://medium.com/element-finance/de-collateralize-an-alternative-to-collateral-backed-loans-b4a7eb49f00): split principal and yield into separate tokens
- [Pendle](https://medium.com/pendle/pendle-is-live-23589c8b14dc) live on mainnet: trade and hedge future aUSDC or cDAI yield
- UMA’s [Range Token](https://medium.com/uma-project/treasury-diversification-with-range-tokens-145d4b12614e): DAOs can borrow using their native token, via convertible debt-like instrument constructed using put and call options 
- [EthSign](https://twitter.com/ethsign/status/1405556735520083970) live on mainnet: onchain document signing with various decentralized storage option
- Sorare: [France is first national team to issue football NFT cards](https://medium.com/sorare/introducing-sorare-national-team-cards-24c3b605581)
- Sotheby’s auctioning [Tim Berners-Lee’s source code as NFT](https://sothebys-com.brightspotcdn.com/94/a2/742444404b45ae855523a58edcd2/www-pr-en.pdf)

**Regulation/business/tokens**

- [Goldman Sachs](https://www.bloomberg.com/news/articles/2021-06-14/goldman-expands-in-crypto-trading-with-plans-for-ether-options?srnd=cryptocurrencies) plans to offer options and futures trading in Ether
- [Sygnum Bank (Switzerland)](https://www.insights.sygnum.com/post/sygnum-launches-first-phase-of-institutional-grade-access-to-decentralised-finance) adds institutional custody and regulated trading of DeFi tokens
- Partially collateralized stablecoin from [Iron Finance had a bank run](https://thedefiant.io/iron-finance-implodes-after-bank-run/) and collapsed from a TVL peak of $3billion
- Lots of discussion this week about Curve competing or collaborating
    - [Yearn and Convex competing](https://newsletter.banklesshq.com/p/is-convex-the-yfi-killer) in the Curve yield farming wars
    - Two [Curve proposals](https://thedefiant.io/curve-drama-intensifies-as-new-proposals-target-alusd-and-saddle-finance/): remove incentives for Alchemix and a lawsuit against Saddle for alleged IP infringement

**General**

- Scammers sending [fake replacement Ledgers](https://www.bleepingcomputer.com/news/cryptocurrency/criminals-are-mailing-altered-ledger-devices-to-steal-cryptocurrency/) to customers in the Ledger data breach
- Bobby Ong: [security best practices for users](https://twitter.com/bobbyong/status/1403881080902471680)
- [RAC in RollingStone’s Future 25](https://www.rollingstone.com/pro/features/rac-future-25-1179443/) for work in crypto
- [Fully Homomorphic Encryption](https://github.com/google/fully-homomorphic-encryption) (FHE) transpiler from Google: transpile C++ to FHE-ready C++

* * *

## **Job Listings**

- NFT innovator SuperRare seeks [Director of Eng](https://superrare.breezy.hr/p/f1919c5bb07b-director-of-engineering) following Series-A fundraise
- Celer are hiring [software engineers](https://www.celer.network/career.html)
- Ethereum.org are seeking a [Community & Ecosystem Lead](https://ethereum.org/en/about/community-lead/)
- bp’s Digital Science and Engineering team are hiring a [Blockchain Developer](https://docs.google.com/document/d/1vNvgHmpE7C_kkjecJAG2gF2odF0oSyxhRlnxO-_8jQo/edit)
- Nethermind [internship program](https://www.notion.so/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please post your news to an Ethereum subreddit; emails/DMs are not part of our workflow.

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-june-19-2021/](https://weekinethereumnews.com/week-in-ethereum-news-june-19-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- July 1 - [Gitcoin Grants Round 10](https://gitcoin.co/grants/explorer/) ends (support [Week in Eth News](https://gitcoin.co/grants/2785/week-in-ethereum-news))
- June 23 - [Ethereum Foundation Research team AMA](https://twitter.com/drakefjustin/status/1398375498342977544)
- June 25-27 – [Edcon](https://www.edcon.io/) (Shenzhen/online)
- July 10 - Road to Devcon Quest: [Devcon Trivia Game](https://ethstaker.cc/road-to-devcon/)
- July 28 – [tentative date for London hard fork](https://docs.google.com/spreadsheets/d/1Y3yyTqeqRO1O2UFVkNkHK_V5oRulZd6y-JJbSnKYrb4) (Ropsten June 24, Goerli June 30, Rinkeby July 7)
- July 20-22 – [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

---
title: "Week in Ethereum News <br> April 16, 2022"
date: "2022-04-16"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest core devs [call video](https://www.youtube.com/watch?v=JXbOeiPN_uE&t=109s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1515067269147111424) & [Christine Kim](https://twitter.com/christine_dkim/status/1515013002105442312):
    - Keep shadow forking until no client issues, then upgrade Ropsten, followed by shorter timeframe for Goerli & Sepolia
    - Rinkeby won’t be upgraded; Ropsten & Rinkeby will be deprecated
    - [latestValidHash analysis](https://hackmd.io/GDc0maGsQeKfP8o2C7L52w?view) with potential attack scenarios
    - EOF, SELFDESTRUCT and Verkle tries discussion
    - Not accepting more EIPs for Shanghai until post merge
- ethereumjs/client [v0.4.1](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs/client%400.4.1): merge/Kiln fixes
- Erigon [merge support & v2](https://erigon.substack.com/p/erigon-2-three-upgrades): Alpha version will support the merge, v2 aims to solve snapshot sync & transaction level granularity for history
- Erigon [v2022.04.02](https://github.com/ledgerwatch/erigon/releases/tag/v2022.04.02): using mirror for MDBX after [removal from GitHub](https://twitter.com/realledgerwatch/status/1514898348100231171)
- [Condrieu Verkle testnet](http://condrieu.ethdevops.io) now public 
- The future of accounts: [options for migrating EOAs to contract wallets](https://ethresear.ch/t/a-brief-note-on-the-future-of-accounts/12395)

**Proof of Stake consensus layer**

- Nimbus [v22.4.0](https://github.com/status-im/nimbus-eth2/releases/tag/v22.4.0): 750MB to run a node after 250MB memory use reduction
- Lighthouse [v2.2.1](https://github.com/sigp/lighthouse/releases/tag/v2.2.1): fix sync from genesis/pre-Altair checkpoint
- Ben Edgington’s Upgrading Ethereum book [Randomness](https://eth2book.info/altair/part2/building_blocks/randomness) chapter
- [Lido plans for decentralization](https://blog.lido.fi/the-next-chapter-for-lido/): gradual adoption of Distributed Validator Technology 

**PoW switch off (the merge)**

- The merge likely [won’t be June](https://twitter.com/TimBeiko/status/1514010098145759232)
- Pari’s [shadow fork explainer](https://twitter.com/parithosh_j/status/1513129881927884801)
- mainnet-shadow-fork-1 [successful](https://twitter.com/parithosh_j/status/1513494565529001984) but several clients found issues
- [Goerli-shadow-fork-4](https://github.com/eth-clients/merge-testnets/tree/main/goerli-shadow-fork-4#readme) on April 19, next mainnet shadow fork April 23

**EIPs/Standards**

- [ERC721R](https://twitter.com/CryptoFighters/status/1513183463851003904): minters can return NFT for a refund
- [EIP5008](https://github.com/ethereum/EIPs/pull/5008/files): ERC721 Nonce and Metadata Update Extension
- [EIP5007](https://github.com/ethereum/EIPs/pull/5007/files): ERC721 Time Extension
- [EIP5005](https://github.com/ethereum/EIPs/pull/5005/files): Zodiac
- [EIP5003](https://github.com/ethereum/EIPs/pull/5003/files): Replace EOAs with AUTHUSURP
- [EIP4985](https://github.com/ethereum/EIPs/pull/4985/files): NFT for GameFi
- [EIP4897](https://github.com/ethereum/EIPs/pull/4987/files): Held token standard
- [EIP4804](https://github.com/ethereum/EIPs/pull/4995/files): Web3 URL to EVM Call Message Translation

**Layer2**

- [KuCoin](https://www.kucoin.com/news/en-arb-withdrawal-service-for-eth-usdt-usdc-is-now-supported-on-kucoin-20220412) supports withdrawals on Arbitrum
- [Worldcoin open sources protocol](https://worldcoin.org/open-sourcing-worldcoin) including optimistic rollup based on the Hubble Project and Semaphore

* * *

### **This newsletter is made possible thanks to the** [**Uniswap Grants Program**](https://unigrants.org/)**!**

![](https://weekinethereumnews.com/wp-content/uploads/2022/03/Uniswap-Grants-Program-1024x274.png)

[](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F1e3c4313-4d62-4db0-b13b-37522fc694a1_1600x429.png)

[Uniswap Grants Program](https://unigrants.org/) - If you’ve ever wanted to work on TWAP oracles, better DeFi devtools, had ideas on optimizing LP strategies, or just wanting to improve the Uniswap protocol, [apply for a grant from UGP today](https://airtable.com/shrWrSFRs6t1q1s9v)!

For more grant ideas, check out our [list of RFPs](https://www.notion.so/RFPs-Challenges-3be614ba4e504b5caeee7b0159e64a42)!

* * *

**Stuff for developers**

- Underhanded Solidity Contest [winners](https://blog.soliditylang.org/2022/04/09/announcing-the-underhanded-contest-winners-2022/)
- Remix [v0.23.0](https://twitter.com/EthereumRemix/status/1514595790479454218): improved caching, run a script after compiling via natspec
- ethereumjs/vm [v5.9.0](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs%2Fvm%405.9.0): EIP3651 (warm coinbase), EIP1153 (transient storage opcodes) and custom pre-compiles
- [Foundry key repos](https://twitter.com/gakonst/status/1514733433188073473) consolidated in one GitHub organization
- [Unimock](https://twitter.com/maurelian_/status/1514819077939757059): mock contract for Foundry testing
- [Hot-chain-svg](https://github.com/w1nt3r-eth/hot-chain-svg#readme): on-chain SVG toolkit, hot reloading, visual testing and library
- [NFT gas optimization](https://medium.com/@WallStFam/the-ultimate-guide-to-nft-gas-optimization-7e9289e2d88f) guide
- Nethereum (.Net library) [v4.3.0](https://github.com/Nethereum/Nethereum/releases/tag/4.3.0): improved support for Sign-In with Ethereum, contracts for ERC tokens & ENS and log processing
- useDapp [v1.0](https://medium.com/truefieng/usedapp-1-0-released-4ee60a94fb06) (dapp development framework): multi-chain support, WalletConnect integration and custom chain configuration
- Uniswap Labs [Swap Widget](https://uniswap.org/blog/widget): React component for token swaps
- Center [NFT React components](https://twitter.com/centerapp/status/1513939345996062722): embed NFTs in React apps
- [Auth0 guide](https://auth0.com/blog/sign-in-with-ethereum-siwe-now-available-on-auth0/) for adding Sign-in with Ethereum
- Otterscan [v2022.04.01](https://github.com/wmitsuda/otterscan/releases/tag/v2022.04.01-otterscan): USD prices for token transfers and testnet faucets

**Security**

- EF Security research team [update](https://blog.ethereum.org/2022/04/14/secured-no-3/) on consensus layer & the merge

**Ecosystem**

- Josh Stark: [atoms, institutions & blockchains](https://stark.mirror.xyz/n2UpRqwdf7yjuiPKVICPpGoUNeDhlWxGqjulrlpyYi0)
- Post merge [deflationary ETH minimum gas price](https://twitter.com/domothy/status/1512817907130114059): 14.1 gwei at 350k validators, 16.9 gwei at 500k validators and 23.9 gwei at 1M validators
- [Malicious SVG NFTs can contain JavaScript](https://research.checkpoint.com/2022/check-point-research-detects-vulnerability-in-the-rarible-nft-marketplace-preventing-risk-of-account-take-over-and-cryptocurrency-theft/) to steal NFTs by requesting holders approve an allowance
- Etherscan [token ignore list](https://twitter.com/etherscan/status/1512785670418628609): hide transactions for spam tokens
- ETHGlobal DAOHacks [finalists](https://twitter.com/ethglobal/status/1513302525696516101)
- A [simple guide](https://mirror.xyz/brunny.eth/upIPESej7MjO2rFijwQyx8NBel845fIPV9J5G0Vn4cE) to Ethereum

**Enterprise**

- EEA business readiness & use case [survey](https://docs.google.com/forms/d/e/1FAIpQLSdqwKJa-ZOvBNuRoMjJPQ3w_VF9MqOgZ88rEUczofzzHvHK_A/viewform)

**Application layer**

- Alchemix [Elixir](https://alchemixfi.medium.com/elixir-the-alchemix-algorithmic-market-operator-2e4c8ad04569): Algorithmic Market Operator (AMO)
- ICHI [pool 136 postmortem](https://medium.com/ichifarm/postmortem-of-pool-136-3cb22102065a), price decline after $10M sale resulted in a cascading liquidation event
- 0x [analysis on impact of slippage](https://blog.0x.org/measuring-the-impact-of-hidden-dex-costs/)
- Coinbase [casting call for Bored Apes](https://degentrilogy.com/) to appear in three part short film 
- Lit [Token Access](https://twitter.com/LitProtocol/status/1514276972242903042): token gated access to products/discounts on Shopify, beta
- [Spice](https://blog.spice.ai/announcing-spice-xyz-94323159cd2b): data & AI infrastructure for apps & ML, preview

* * *

### **Job Listings**

- EF seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- [Internship program](https://nethermind.notion.site/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1) at Nethermind (1-3 month) 
- OpenZeppelin are hiring a [Director of Development - Contracts](https://openzeppelin.com/jobs/opening/?gh_jid=5078928003)
- EF’s Privacy & Scaling Explorations team: [Web3 Engineer](https://jobs.lever.co/ethereumfoundation/ece6534a-b946-4996-b7e7-713bd1ec0353?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Devcon needs a [front-end web developer](https://ethereum.bamboohr.com/jobs/view.php?id=61&source=weekinethnews)
- EF ecosystem support hiring for [Communications](https://jobs.lever.co/ethereumfoundation/4b0c3305-cf03-4e33-9bfb-63e4ec6f3a68?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum), [Analyst](https://jobs.lever.co/ethereumfoundation/64361391-9a74-49ed-b37c-8ff35931430e?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) & [Admin Assistant](https://jobs.lever.co/ethereumfoundation/5684f7ea-c3ad-4703-b86c-462964f49392?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- EF hiring [Test Engineer](https://jobs.lever.co/ethereumfoundation/e6d303e5-168d-447e-a596-e3c2b105ca3f?lever-source%5B%5D=Week%20in%20Ethereum%20) to improve testing infrastructure & coverage

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US Treasury allege North Korean Lazarus group](https://www.coindesk.com/policy/2022/04/14/us-officials-tie-north-korean-hacker-group-to-axies-ronin-exploit/) behind Axie Infinity/Ronin hack
- [Tornado Cash front end](https://twitter.com/tornadocash/status/1514904975037669386) blocks sanctioned addresses using Chainalysis oracle
- [Challenges for strongly on-chain games](https://dialectic.ch/editorial/thoughts-on-chain-gaming): UI/UX, backrunning & gaMEV, information hiding and latency

**General**

- Virgil Griffith [sentenced to 63 months with a $100k fine](https://twitter.com/innercitypress/status/1513915104500367363). A first hand account of Virgil’s [North Korea trip](https://cointelegraph.com/magazine/2022/04/12/bizarre-the-fbis-takedown-of-an-eth-dev-who-went-to-north-korea)
- Another [Chrome zero day](https://twitter.com/shanehuntley/status/1514719656619114506).  Update your Chrome/Brave browsers ASAP
- [Frozen Heart](https://blog.trailofbits.com/2022/04/13/part-1-coordinated-disclosure-of-vulnerabilities-affecting-girault-bulletproofs-and-plonk/) zk proof vulnerability disclosed: Fiat-Shamir transformation implementations allow users to forge proofs for random statements 

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-april-16-2022](https://weekinethereumnews.com/week-in-ethereum-news-april-16-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in_ **_bold_**_)_**:**

- Apr 18-25 – [Devconnect](https://devconnect.org/schedule) (Amsterdam)
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- **May 1 – application deadline for** [**yAcademy’s auditor fellowship**](https://yacademy.dev/fellowship-program/)
- May 3-5 – [Spaghett ETH](https://spaghett-eth.com/) (Milan)
- May 6-27 – ETHGlobal [Hack Money](https://defi.ethglobal.com/)
- **May 8 – deadline for** [**EF academic grants round**](https://esp.ethereum.foundation/academic-grants)
- May 17-20 – [EY Global blockchain summit](https://pub.ey.com/public/2021/2112/2112-3933703/blockchain-summit-2022/index.html)
- May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETH NYC](https://nyc.ethglobal.co/)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev) (hackathon & conference)
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** [_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive it weekly_**

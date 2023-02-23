---
title: "Week in Ethereum News <br> January 15, 2022"
date: "2022-01-15"
---

## **Eth News and Links**

**Mainnet execution layer**

- Kintsugi testnet [returns to finality](https://twitter.com/parithosh_j/status/1481394021566193668) after issues found from fuzz testing [changing expected blockhash](https://twitter.com/vdwijden/status/1479945793893277698) and [setting block number to 1](https://twitter.com/vdwijden/status/1480969541928816644)
- Erigon [v2022.01.01](https://github.com/ledgerwatch/erigon/releases/tag/v2022.01.01): bug fixes
- Nethermind [v1.12.4](https://github.com/NethermindEth/nethermind/releases/tag/1.12.4): JSON RPC support improvements
- Besu [v21.10.7](https://github.com/hyperledger/besu/releases/tag/21.10.7): bug fixes
- Why and how clients will [stop serving chain history older than a year](https://twitter.com/nonveumann/status/1481657327283359749)

**EIPs/Standards**

- [EIP4671](https://github.com/ethereum/EIPs/blob/3fba38040b8b7fcc7ba44b85373f1e66462e3394/EIPS/eip-4671.md): Non-Tradable Tokens
- [EIP4636](https://github.com/ethereum/EIPs/blob/4795fe491894f49e812885e99d059938a6a397c6/EIPS/eip-4636.md): Licensing Token Standard
- [EIP4341](https://eips.ethereum.org/EIPS/eip-4341): Ordered NFT Batch Standard

**Proof of Stake consensus layer**

- [Client diversity stats](https://twitter.com/sproulM_/status/1481109509544513539): we have a super-majority client; Institutions, pools & stakers **are negligent** if they run a super-majority client (more than 66% share), as a super-majority [endangers both their stake and the network](https://upgrading-ethereum.info/altair/part2/incentives/diversity)
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220114)
- PoS implementers [call](https://www.youtube.com/watch?v=izyYW9-HbNk&t=121s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/ryBR2ip3Y): 
    - Spec to be updated for call semantics, keep Kintsugi until this happens
    - One more testnet before upgrade public testnets to switch off PoW
- Nimbus [v1.6.0](https://github.com/status-im/nimbus-eth2/releases/tag/v1.6.0): Key manager API support (beta), validator performance metrics, speed improvements, [uses just 1 gig of RAM](https://twitter.com/dannyryan/status/1481641164952379410) on mainnet
- [Key manager UI](https://twitter.com/sproulM_/status/1481859790557319168) with Lighthouse demo, uses Key manager API, work in progress
- Proposal for [Whisk](https://ethresear.ch/t/whisk-a-practical-shuffle-based-ssle-protocol-for-ethereum/11763), privacy-preserving protocol for electing beacon chain block proposers, modified version of Single Secret Leader Election
- Vitalik’s [Serenity design rationale](https://notes.ethereum.org/@vbuterin/serenity_design_rationale) updated (old but relevant) 

**Layer2**

- Optimism [transaction fees reduced](https://twitter.com/optimismpbc/status/1479840872954875905), transactions ~30% cheaper on average
- Arbitrum [Sequencer downtime](https://offchain.medium.com/todays-arbitrum-sequencer-downtime-what-happened-6382a3066fbc) due to hardware failure, backup had software upgrade in progress, Arbitrum still in beta, plans to decentralize Sequencer
- [Binance](https://twitter.com/dmihal/status/1481709263932342275) enables Arbitrum withdrawals
- Polygon Zero (formerly Mir) [Plonky2](https://blog.polygon.technology/introducing-plonky2/): recursive SNARK based on PLONK and FRI, recursive proofs generated in ~170ms on Macbook Pro
- Fuel proposes Layer 2 token model: [tokenizing right to collect fees](https://fuel-labs.ghost.io/token-model-layer-2-block-production/) as a Layer 2 block producer; suggests models to avoid: PoS, fee paying & governance
- Celer [inter-chain message framework](https://blog.celer.network/2022/01/12/celer-inter-chain-message-framework-the-paradigm-shift-for-building-and-using-multi-blockchain-dapps/) live on testnet, single click UX to send arbitrary messages and execution instructions
- [Adoption curves](https://twitter.com/ethdreamer/status/1480676820026597377) of Optimism and Arbitrum vs sidechains (linear & log scale)

* * *

### **This newsletter is made possible thanks to Starbloom Ventures!**

![Starbloom Ventures](https://weekinethereumnews.com/wp-content/uploads/2021/11/Screenshot-from-2021-11-19-15-25-51.png)

Starbloom Ventures is a new early-stage venture fund by Evan Van Ness and James Fickel to invest in the future of web3. 

What does it mean to invest in the future of web3?  Check out our [request for startups](https://twitter.com/evan_van_ness/status/1471593545085734922).

We’re pledging [10% of profits to support Ethereum public goods](https://twitter.com/evan_van_ness/status/1461840784819425288).  Why hasn’t your favorite VC taken the pledge?

* * *

**Stuff for developers**

- Foundry: [debugger](https://github.com/gakonst/foundry/pull/356): step through a transaction and view opcodes, stack, memory & source code highlighting
- Foundry [parallel EVM tests](https://github.com/gakonst/foundry/pull/444): speed up unit and fuzz tests
- Getting started with [Forge](https://mirror.xyz/crisgarner.eth/BhQzl33tthkJJ3Oh2ehAD_2FXGGlMupKlrUUcDk0ALA) (Foundry testing framework)
- OpenZeppelin Contracts [v4.5 release candidate](https://forum.openzeppelin.com/t/release-candidate-for-contracts-4-5-open-review-period/22700) open review
- [Hardhat-marmite](https://github.com/primitivefinance/hardhat-marmite): Hardhat plugin to compare gas costs of Solidity snippets
- xdeployer [v1.1.0](https://github.com/pcaversaccio/xdeployer/releases/tag/v1.1.0): Hardhat plugin to deploy contracts with deterministic address (uses CREATE2), supports mainnet, Arbitrum, Optimism & testnets
- [Seatbelt](https://uniswap.org/blog/governance-seatbelt): test suite for Governor Bravo proposals, lists referenced addresses, confirms referenced contracts are verified and lists state changes
- [PaymentSplitter](https://twitter.com/divergencearran/status/1481641622861324304): factory to create low cost splitters using EIP1167 minimal proxies, fixed cost <200k gas
- [evm-codes](https://www.evm.codes/precompiled): adds precompiled contracts reference
- [evm-puzzles](https://github.com/fvictorio/evm-puzzles): new levels, set transaction data/value so won’t revert
- [starknet-cairo-101](https://github.com/l-henri/starknet-cairo-101): set of exercises to learn StarkNet
- Blocknative [Transaction Preview API](https://www.blocknative.com/blog/ethereum-transaction-preview-api): simulate transactions to see effects before authorizing
- Matthew Green’s casual review of [MetaMask crypto](https://blog.cryptographyengineering.com/2022/01/14/an-extremely-casual-code-review-of-metamasks-crypto/)
- [Ethereum Data Warehouse](https://tokenflow.live/blog/edw): queryable full history, based on Snowflake cloud, relation between events and emitting call, limited beta

**Security**

- Stobox [STBU deployer private key compromised](https://twitter.com/StoboxCompany/status/1479263023772672004), reserve funds stolen
- OpenZeppelin Contracts [security advisory](https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-m6w8-fq7v-ph4m) for GovernorBravo compatibility layer, proposals executing function calls could have incorrect arguments due to bad ABI encoding

**Ecosystem**

- Galaxy Digital’s [MEV report](https://docsend.com/view/vr6seimd2bfx8iei): $730+ million in MEV in 2021, most common strategy is arbitrage, Flashbots transactions are less than 1.5% of block space
- [Cryptopunk](https://twitter.com/bertcmiller/status/1482086447775580161) sandwiched: 26.25 ETH bid placed, bot makes a higher bid, bot withdraws bid, bot adds new highest bid at 1 wei and wins
- [Etherscan features](https://medium.com/etherscan-blog/21-etherscan-features-in-2021-6adbaedc39b5) in 2021 \[in case you missed any\]
- [Bot drained 58 ETH](https://twitter.com/cat5749/status/1481813755914711042) from WETH <> WTF liquidity pool, beware of tokens with high slippage; reminder to be mindful of [low effort airdrops](https://twitter.com/lefterisjp/status/1481928978680188928)
- Moxie (Signal founder): [first impressions of web3](https://moxie.org/2022/01/07/web3-first-impressions.html); responses from [Vitalik](https://www.reddit.com/r/ethereum/comments/ryk3it/my_first_impressions_of_web3/hrrz15r/) and [Dan Finlay](https://medium.com/@danfinlay/what-moxie-missed-on-web3-wallets-8dc572e7f39b)
- Analysis of [Ethereum PoW emissions](https://kylemcdonald.github.io/ethereum-emissions/), bottom up estimate, 20 ktCO2/day, ~ 2-3 coal power plants; roll on switching off PoW forever

**Application layer**

- Opyn [Squeeth](https://medium.com/opyn/squeeth-primer-a-guide-to-understanding-opyns-implementation-of-squeeth-a0f5e8b95684) live on mainnet, tracks index of ETH squared, options like exposure without need for strikes or expiries, no liquidations on long side 
- [EPNS](https://medium.com/ethereum-push-notification-service/the-epns-mainnet-is-here-470faec0c01) (push notification service) live, subscribe to channels for notifications
- Olympus [v2 Bonds](https://olympusdao.medium.com/introducing-v2-bonds-a17c7da298a2): adds auto-staking and flexible vesting
- Live on Optimism
    - [0x API](https://blog.0x.org/0x-api-is-now-available-on-optimism/), [Matcha](https://blog.matcha.xyz/optimism-is-now-live-on-matcha/) and [Set Protocol](https://medium.com/set-protocol/set-protocol-live-on-optimism-enabling-structured-products-on-layer-2-78361a0c86a1)
    - [Tornado Cash](https://tornado-cash.medium.com/tornado-cash-has-been-deployed-on-optimism-68351443bbc)
- [Euler Finance](https://lambert-guillaume.medium.com/how-to-deploy-delta-neutral-liquidity-in-uniswap-or-why-euler-finance-is-a-game-changer-for-lps-1d91efe1e8ac) guide to hedging in Uniswap
- ENS [eth.link](https://twitter.com/nicksdjohnson/status/1481748889409822720): DNS servers being switched to CloudFlare to avoid breaking ENS subdomain SSLs, older IPFS versions need upgrading
- [LooksRare](https://docs.looksrare.org/blog/launch-post) NFT marketplace, fees paid to token stakers, offer on any NFT in a collection, floor prices of traits, [apparent wash trading](https://twitter.com/dingalingts/status/1481135479940874241) for rewards
- [MoonCats](https://mooncat.community/blog/onchain): traits, colors and SVGs now on-chain
- [FancyLoogies](https://twitter.com/damianmarti/status/1480520597381783556): composable on-chain SVG NFT on Optimism
- [Doomsday NFT](https://anallergytoanalogy.medium.com/the-doomsday-nft-adb113a986ec): on-chain survival game, NFTs randomly destroyed

* * *

### **Job Listings**

- Geth team seeks [Senior Technical Writer](https://ethereum.bamboohr.com/jobs/view.php?id=51&source=weekinethnews) to take ownership & redo docs
- The VAC team at Status.im are looking for a [blockchain engineer](https://jobs.status.im/?gh_jid=3706505)
- Are you a p2p networking whiz? EF research hiring [Networking Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=54&source=weekinethnews)
- Kwenta seeks [Frontend Engineer](https://blog.kwenta.io/kwenta-open-position-front-end-developer/), [Solidity Engineer](https://blog.kwenta.io/kwenta-open-position-solidity-engineer/) & [Marketing Lead](https://blog.kwenta.io/kwenta-open-position-marketing-manager/)
- Certora seeks [SR SW Eng](https://www.certora.com/#careers), [Security Res](https://www.certora.com/#careers), [Security Eng](https://www.certora.com/#careers) & [Community Manager](https://www.certora.com/#careers)

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Ethereum Q4 financial results](https://newsletter.banklesshq.com/p/state-of-ethereum-q4-report) by Bankless, ETH annualized net issuance at 0.46%, $154 billion TVL in DeFi, $5.6 billion TVL in Layer 2
- [USDC supply on Ethereum](https://www.theblockcrypto.com/post/130342/usdc-supply-on-ethereum-surpasses-usdt-first-time) surpasses USDT
- [Neufund](https://blog.neufund.org/why-were-shutting-down-neufund-e553d990e8b1) shutting down due to lack of support from European regulators
- [Pudgy Penguins](https://thedefiant.io/fire-on-the-iceberg-pudgy-penguin-holders-eye-coup-amid-acquisition-talks/) community vs founders, potential acquisition, community wrapping NFTs to avoid royalties going to founders
- [Coinbase acquiring FairX](https://blog.coinbase.com/coinbases-path-to-creating-a-robust-and-regulated-crypto-derivatives-market-a1dc71577337) (US regulated derivatives exchange), plans to offer crypto derivatives in US
- [Proposed bill](https://twitter.com/RepTomEmmer/status/1481283945492852743) to prohibit US Fed from issuing CBDC directly to individuals
- [Class-action lawsuit filed against PoolTogether](https://www.wsj.com/articles/crypto-savings-lawsuit-puts-principles-of-defi-to-the-test-11642069806) by ex-staff of US Senator Warren for allegedly allowing purchase of illegal lottery ticket
- [Fees paid](https://twitter.com/0xstark/status/1481381321058385922) to use Ethereum in 2021 10x fees paid to use Bitcoin

**General**

- [Don’t use antipattern of raw secrets on the web](https://twitter.com/sniko_/status/1480542426519543812), data is vulnerable and normalizes users entering secrets
- The Onion’s [guide to web3](https://www.theonion.com/the-onion-guide-to-web3-1848356077)
- Wikipedia editors for most expensive artworks list [discuss whether NFTs should be classified as art](https://en.wikipedia.org/w/index.php?title=Talk:List_of_most_expensive_artworks_by_living_artists#Separation_of_NFT_sales_and_artwork_sales)
- Decentralization matters: Dapper Labs’ [NBA Top Shot](https://www.coindesk.com/business/2022/01/12/nba-top-shot-bans-user-freehongkong/) froze user account FreeHongKong
- Marak, [developer of colors.js and faker.js added infinite loop](https://www.bleepingcomputer.com/news/security/dev-corrupts-npm-libs-colors-and-faker-breaking-thousands-of-apps/) in apparent protest for corporations not giving back to the open source community

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-january-15-2022](https://weekinethereumnews.com/week-in-ethereum-news-january-15-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Feb 15 - Apr 5 – [Cryptocurrency Class](https://mirror.xyz/0xaFaBa30769374EA0F971300dE79c62Bf94B464d5/oGqGP2NOK9g7QPl1sMKkzql_Fh0P6hKbpYLZ-EkQTXU) (virtual) 
- Feb 17 – [Schelling Point](https://schellingpoint.gitcoin.co/) (Denver) 
- Feb 18-20 – [ETHDenver](https://www.ethdenver.com/)
- Mar 14-17 – [Eth Rio](https://www.ethrio.org/)
- Mar 17-18 – [ETH Austin](https://2022.ethaustin.org/) summit
- Mar 29-31 – [ETHDubai](https://www.ethdubaiconf.org/)
- Apr 7-9 – [ETH Portland](https://2022.ethportland.com/) hackathon 
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- May 3-8 – [spaghettETH](http://spaghett-eth.com/) (Milan)
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 16-19 – [ETH Miami](https://2022.eth-miami.com/) summit & hackathon
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26  – [ETHNewYork](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

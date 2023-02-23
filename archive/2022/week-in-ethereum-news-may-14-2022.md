---
title: "Week in Ethereum News <br> May 14, 2022"
date: "2022-05-14"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- [Ropsten testnet upgrade to PoS](https://twitter.com/trent_vanepps/status/1525138148879220742) estimated for June 8 (Terminal Total Difficulty 43531756765713534)
- [Mainnet-shadow-fork-4](https://twitter.com/parithosh_j/status/1524767841773363200) merge looked perfect, Erigon had unrelated sync issues
- [Mainnet-shadow-fork-5](https://twitter.com/abcoathup/status/1525252459383656448) merge on May 19, equal validator split across execution & consensus layer clients
- Staking safely post-Merge [requires client diversity](https://twitter.com/TimBeiko/status/1524136595862941696) for both consensus & execution layers
    - Geth currently over 80% at the execution layer

**Mainnet execution layer**

- Latest core devs [call video](https://www.youtube.com/watch?v=BFxkGdPv4F8&t=188s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1525232290321690624) & [Christine Kim](https://twitter.com/christine_dkim/status/1525178255002677248):
    - Mainnet-shadow-fork-4: empty blocks due to consensus clients asking for the candidate block too quickly
    - Ropsten to be upgraded to PoS early June with permissionless beacon chain, not using Fork ID; Sepolia beacon chain to be permissioned
    - Agreed on latest, finalized & safe JSON RPC block tags
    - EIP discussions: EIP4938 (eth/67: removal of GetNodeData) and EIP5081 (expirable transaction)
- Nethermind [v1.13.0](https://github.com/NethermindEth/nethermind/releases/tag/1.13.0): beta snap sync support, sync reduced from 24+ hours to 2 hours & download size cut from ~90GB to ~30GB
- Erigon [v2022.05.03-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.05.03): more fixes to improve snapshot download speed

**Proof of Stake consensus layer**

- Updated [consensus client diversity](https://twitter.com/sproulM_/status/1525026588428890112) estimates: Prysm 48%, Lighthouse 23%, Teku 15% and Nimbus 8%
- Somer’s staker migration guides: [migrate from Prysm to Nimbus](https://someresat.medium.com/ethereum-staker-migration-guide-migrating-from-prysm-to-nimbus-b802a7dcb31e)
- Teku [v22.5.0](https://github.com/ConsenSys/teku/releases/tag/22.5.0): epoch processing optimisations & fixes issue loading optimized BLST library on Windows
- Lodestar [v0.36.0](https://github.com/ChainSafe/lodestar/releases/tag/v0.36.0): security fix and proposer boost enabled by default
- [Danksharding panel](https://www.youtube.com/watch?v=N5p0TB77flM) with Dankrad, Protolambda & Vitalik, moderated by Tim Beiko
- Danny Ryan: [Lido over 1/3 of stakers](https://twitter.com/dannyryan/status/1524044527828303872) is a centralization risk

**EIPs/Standards**

- Proposal for [NFT sale of unused EIP numbers](https://github.com/ethereum/EIPs/issues/5082)
- [EIP5089](https://github.com/ethereum/EIPs/pull/5089/files): Principal token
- [EIP5083](https://github.com/ethereum/EIPs/pull/5083/files): NFT token acceptance
- [EIP5081](https://eips.ethereum.org/EIPS/eip-5081): Expirable transaction

**Layer2**

- [KuCoin](https://www.kucoin.com/news/en-opt-deposit-service-for-usdt-usdc-is-now-supported-on-kucoin-20220511) supports USDC & USDT deposits on Optimism
- Censorship resistant [bridges](https://twitter.com/bkiepuszewski/status/1524666863858425856)
- Polygon Hermez v2 [deep dive](https://blog.polygon.technology/zkverse-deep-dive-into-polygon-hermez-2-0/)

* * *

### **This newsletter is made possible thanks to clr.fund’s** [**staking public goods round**](https://qf.ethstaker.cc/#/projects)**!**

![clr.fund](https://weekinethereumnews.com/wp-content/uploads/2022/05/1500x500-1024x341.jpeg)

[](https://substackcdn.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F94cb536b-bea8-4114-829a-ede51d3afc18_1500x500.jpeg)

[clr.fund](https://clr.fund/) and [ETHStaker](https://ethstaker.cc/) are running a 350k DAI (funded by the Ethereum Foundation) quadratic funding round dedicated to open source public goods for our staking ecosystem.

Under the hood, clr.fund uses zk-SNARKs using [MACI to prevent collusion and bribery](https://blog.clr.fund/clr-fund-explained-pt-1/) attacks as well as [BrightID](https://www.brightid.org/) for Sybil-attack resistance.

You can register to [get funded](https://qf.ethstaker.cc/#/join) or go [donate](https://qf.ethstaker.cc/#/projects) DAI to allocate the 350k+ DAI matching pool.

Round ends May 24th.  [Donate now](https://qf.ethstaker.cc/#/)!

* * *

**Stuff for developers**

- samczsun’s [Signature Database](https://sig.eth.samczsun.com/): search function, error, event & name signatures
- [Use optional access list](https://twitter.com/libevm/status/1523141360076812288) to reduce gas costs reading multiple storage slots
- [Thirdweb-deploy](https://blog.thirdweb.com/thirdweb-deploy): deploy contracts using MetaMask or Gnosis Safe, dashboard to view deployments
- Blocknative [Transaction Preview API](https://www.blocknative.com/blog/simulate-multiple-transactions-with-bundle-preview) simulate bundled transactions
- Sepolia testnet [faucet](https://faucet.sepolia.dev/)
- OxPARC [Ecne](https://0xparc.org/blog/ecne): verify ZK circuits
- 1inch’s [cumulative merkle drop tool](https://blog.1inch.io/1inchs-cumulative-merkle-drop-tool-an-overview-55542c9addca) 

**Security**

- [Chainlink minimal value circuit breaker](https://twitter.com/sniko_/status/1524943313706565639) triggered for LUNA/USD, oracle reported LUNA at $0.107, [Blizz Finance](https://twitter.com/BlizzFinance/status/1524911400992243761) (Avalanche) drained, [Venus Protocol](https://blog.venus.io/venus-protocol-official-statement-regarding-luna-6eb45c3cb058) (BNB chain) $13.5 million lost from borrowing at outdated price
- Balancer [DoS vulnerability disclosed](https://forum.balancer.fi/t/medium-severity-bug-found/3161), double entry-point ERC20 tokens

**Ecosystem**

- [Decentralized Society](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4105763) (DeSoc): ecosystem of accounts (Souls) holding revocable soulbound (non-transferrable) tokens for social identity, with community recovery
- Wallet devs call [notes](https://twitter.com/_samwilsn_/status/1524453665536417794): discussions on batch/bundled transactions endpoint, support multiple wallet extensions and cross-wallet testing
- [Ads on crypto websites](https://twitter.com/frankresearcher/status/1525242200816222210) such as Etherscan & Coingecko used in token approval attack

**Enterprise**

- [Instagram](https://about.instagram.com/blog/announcements/instagram-digital-collectibles) testing sharing NFTs with selected creators & collectors
- [Amazon Managed Blockchain](https://aws.amazon.com/about-aws/whats-new/2022/05/amazon-managed-blockchain-goerli-testnet-ethereum/) supports running Goerli testnet nodes
- [KFC Malaysia sending promo codes](https://twitter.com/etherscan/status/1524377578370650112) via Etherscan’s Blockscan Chat
- EY Blockchain Analyzer [Reconciler](https://www.prnewswire.com/news-releases/ey-announces-general-availability-of-ey-blockchain-analyzer-reconciler-301544701.html): import enterprise records, reconcile off-chain records with on-chain transactions and track wallet balances
- [S&P Global](https://medium.com/compound-finance/compound-treasury-sp-credit-rating-897aff3a6f8c) gave Compound Treasury B- credit rating

**Application layer**

- [Maker vault](https://forum.makerdao.com/t/consolfreight-update-may-2022-consolfreight-helps-mastercard-to-test-defi/15081) used to finance Australian beef shipment
- Bancor [v3](https://blog.bancor.network/bancor-3-the-ultimate-defi-liquidity-solution-is-live-a19aa3ba7314): single-sided staking, impermanent loss protection, dual rewards, auto-compounding rewards, and composable single-sided pool tokens
- [Sushi](https://sushichef.medium.com/sushis-rolling-up-to-optimism-a325d2c585c7) live on Optimism
- Element Finance [open sourced research](https://mirror.xyz/0x3fcAf7DDf64E6e109B1e2A5CC17875D4a5993F39/xYvoTmOzunnxhndOxjeOZagiRm9U0w7o1x3SS9BpQ-Q) \[Disclosure: Evan is advisor\]
- [Backed](https://twitter.com/backed_xyz/status/1524839160909025322) (NFT-backed loans) live on Optimism
- Gnosis Safe [Transaction Simulation](https://twitter.com/gnosisSafe/status/1524443825933983745) in transaction builder
- [Karma](https://twitter.com/showkarma_xyz/status/1524057027143733248?s=20&t=zDY6t5f0iqmVlUVn_5H0gg): delegate from DAO contributor reputation leaderboard; \[Disclosure: Starbloom portfolio\]
- [Hop using Sybil hunters](https://twitter.com/whinfreychris/status/1525178626563420160) to find Sybil airdrop attackers
- Reminder to [check ENS expiry dates](https://twitter.com/nicksdjohnson/status/1524532524671639552)
- [ETHPass](https://twitter.com/ethpass/status/1523701219226652673): token gated events with tickets in Apple Wallet/Google Pay, scanning tickets can autoclaim POAPs
- [Huddle01](https://twitter.com/huddle01com/status/1524772270115225601): token gated video calls live; beta
- [Headline](https://viaheadline.xyz/): decentralized publishing & newsletter platform
- [OpenSea](https://opensea.io/blog/safety-security/were-improving-the-opensea-verification-process/) updated account verification and collection badging system

* * *

### **Job Listings**

- Status Waku is hiring: [Software & DevRel Engineer (Web)](https://jobs.status.im/?gh_jid=4143735&gh_src=55c532491us)
- Ethereum Foundation need a [People Operations Lead](https://jobs.lever.co/ethereumfoundation/8046bbe5-6343-4ecf-8296-37dc2a5bf915?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Trail of Bits [Security Apprenticeship](https://jobs.lever.co/trailofbits/b2d6ce87-6b01-462f-965a-597a273ce26f) (3 months)
- Vac @ status are looking for [protocol engineers](https://jobs.status.im/?gh_jid=3693623) 
- Status are hiring [engineers who focus on incentive design](https://jobs.status.im/?gh_jid=3706505)

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US Treasury Secretary current scale of stablecoin market](https://www.theblockcrypto.com/linked/146583/yellen-says-the-stablecoin-market-is-still-too-small-to-pose-systemic-risk) not a threat to US financial stability
- [Germany's tax guidance](https://decrypt.co/100086/germany-wont-tax-bitcoin-ethereum-sold-after-one-year-of-possession): sale of purchased Ether tax free after one year
- Polynya: [sustainable blockchain checklist](https://mirror.xyz/polynya.eth/UL8_QVNtB-nQoPYyoGyTteJoFNf9jEubzdRqO_5Ez58)
- [Azuki](https://mirror.xyz/0x1Cb8332607fba6A780DdE78584AD3BFD1eEB1E40/yG8rI1lpQGLPhZch0kjxYRjKTtA9rAL51zg-ZrURyAc) co-creator behind abandoned CryptoPhunks, Tendies and CryptoZunks NFT projects

**General**

- [UST](https://rekt.news/luna-rekt/) algorithmic stablecoin fell from peg, [over 6 trillion Luna printed](https://twitter.com/nanexcool/status/1524963716344815627)
- [Coindesk names Do Kwon](https://www.coindesk.com/tech/2022/05/11/usts-do-kwon-was-behind-earlier-failed-stablecoin-ex-terra-colleagues-say/) as co-founder of failed algorithmic stablecoin Basis Cash
- Meta scoping [single wallet experience](https://medium.com/@skasriel/where-the-metaverse-can-take-fintech-a936e6bd6987)
- [Discord API leaks private channel metadata](https://twitter.com/joshfraser/status/1524093110116130816): name, description, members list & activity data

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-may-14-2022](https://weekinethereumnews.com/week-in-ethereum-news-may-14-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in_ **_bold_**_)_**:**

- May 17-20 – [EY Global blockchain summit](https://pub.ey.com/public/2021/2112/2112-3933703/blockchain-summit-2022/index.html)
- May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline
- **May 24 –** [**ETH Staking QF Round**](https://blog.clr.fund/350k-eth-staking-qf-round/) **ends**
- **Jun 8 –** [**Ropsten testnet upgrades to PoS**](https://twitter.com/trent_vanepps/status/1525138148879220742)
- Jun 10 – [Austin DeFi](https://2022.austindefi.org/) summit
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETH NYC](https://nyc.ethglobal.co/)
- Jul 6-8 – [ETHBarcelona](https://twitter.com/eth_barcelona/status/1516773782538448896)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 5-7 – [ETH Seoul](https://2022.ethseoul.org/)
- **Aug 8-10 –** [**ETHToronto**](https://www.ethtoronto.ca/)
- **Aug 11-14 –** [**ETH LATAM (Buenos Aires)**](https://twitter.com/ethlatam/status/1524146640474587137)
- Aug 18-19 – [Ethereum SP](https://twitter.com/EthereumRio/status/1520490449009528832) (São Paulo)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 28 – [DeFi San Francisco](https://2022.defi-sf.com/) summit
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev) (hackathon & conference)
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** [_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive it weekly_**

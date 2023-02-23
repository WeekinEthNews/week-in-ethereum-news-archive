---
title: "Week in Ethereum News <br> December 31, 2021"
date: "2021-12-30"
---

## **Eth News and Links**

**Mainnet execution layer**

- [Akula](https://medium.com/@vorot93/meet-akula-the-fastest-ethereum-implementation-ever-built-58eaca244c39) client preview, written in Rust, can currently run alongside Erigon to sync, full validation from genesis in < 24 hours, enterprise-friendly Apache 2.0 license
- History of [account abstraction](https://medium.com/nethermind-eth/the-history-and-future-of-account-abstraction-10cb097ebdc8) and EIP4337 proposal
- [Archive node](https://twitter.com/EthereumOnARM/status/1476110668789125120) running on Raspberry Pi 4, using Erigon. Also running a Nimbus staking client on same device

**EIPs/Standards**

- [EIP4610](https://github.com/ethereum/EIPs/blob/6676c5710e2e64942f12ba1f5c28b390bde138d5/EIPS/eip-4610.md): ERC721 Delegator Extension 

**Proof of Stake consensus layer**

- Dankrad’s proposed new [sharding design](https://notes.ethereum.org/@dankrad/new_sharding): adds a transaction type with sharded data as call data, allows tight integration between Layer 1 & 2, higher computing requirements for block builders
- Consensus specs [v1.1.8](https://github.com/ethereum/consensus-specs/releases/tag/v1.1.8): sets Bellatrix as upgrade name & new test vectors
- StakeWise [Metro](https://stakewise.medium.com/a-new-era-for-stakewise-decentralizing-the-architecture-e598fde75ea8): allows external node operators

**Layer2**

- [Huobi Global](https://www.huobi.ma/support/en-us/detail/84894749060248) adds ETH deposit and withdrawals on Arbitrum
- [Argent zksync wallet](https://www.argent.xyz/blog/trading-is-now-live-on-l2/) integrates ZigZag exchange, flat $1 trade & network fee
- [#L222](https://twitter.com/kaiynne/status/1475623704147099651) is the “official” hashtag for Layer 2 adoption in 2022 🦆
- Proposal for efficient [zk-EVM](https://ethresear.ch/t/a-zk-evm-specification/11549) arithmetization from ConsenSys Applied R&D

* * *

### **This newsletter is made possible thanks to [NEAR](https://near.org/)!**

![NEAR](https://weekinethereumnews.com/wp-content/uploads/2021/10/near_logo_stack.jpg)

NEAR has [launched Simple Nightshade sharding](https://near.org/blog/near-launches-nightshade-sharding-paving-the-way-for-mass-adoption/) to pave the way for greater throughput!

Simple Nightshade has four different state shards.  For devs and users, it’s important to note that NEAR treats cross-contract calls the same regardless of whether two contracts are on the same shard.

Early in 2022, [phase 1 will introduce chunk-only producers](https://near.org/decentralize/), who only validate one shard and allow for further decentralization via more validators.  Full Nightshade is scheduled for q3 2022 and will feature full sharding of both state and processing.

Learn more about what’s going on in NEAR in the community-driven [NEARweek](https://nearweek.com/) newsletter.

* * *

**Stuff for developers**

- Solidity Language Server [explainer](https://twitter.com/solidity_lang/status/1476212072623005702?s=20): every IDE with Language Server support can support Solidity out of the box
- Foundry [forge run](https://github.com/gakonst/foundry/pull/324) command, runs single file contract as a script, supports cheatcodes, mainnet forking and debug logs
- [Fuzzing](https://ventral.digital/posts/2021/12/21/fuzzing-complex-projects-with-echidna-sushi-bentobox) complex projects with Echidna, example uses Sushi's BentoBox
- Advanced [optimization tips](https://hackmd.io/@gn56kcRBQc6mOi7LCgbv1g/rJez8O8st) for Yul & Solidity 
- OpenZeppelin Nile [v0.3.0](https://github.com/OpenZeppelin/nile/releases/tag/v0.3.0) (StarkNet projects in Cairo): deploy accounts and send transactions, mainnet & Görli compatible
- [ShortString](https://twitter.com/frangio_/status/1476305797449670660): immutable bytes32 can be used for short strings (Solidity doesn’t support immutable strings), convert back to string in a view function
- [erc721-drop](https://github.com/m1guelpf/erc721-drop): NFT drop template with constants for supply cap and price, uses Solmate, Solidity test with Foundry, AGPL v3 license
- [Captcha-protected NFT distribution](https://forum.openzeppelin.com/t/human-first-nft-mints/21921) using an off-chain signing service
- [merkle-airdrop-starter](https://github.com/Anish-Agnihotri/merkle-airdrop-starter): scripts, contracts and frontend, for an airdrop

**Security**

- Polygon lack of balance/allowance check [postmortem](https://medium.com/immunefi/polygon-lack-of-balance-check-bugfix-postmortem-2-2m-bounty-64ec66c24c7d), 9 billion MATIC was at risk, 800k MATIC stolen, $2.2 million + 500k MATIC bounties paid
- Bent Finance [postmortem](https://bentfi.medium.com/we-got-bent-how-we-got-exploited-and-recovered-stronger-1ebdeb44c5d7), rogue dev upgraded to contract with hard coded balances, funds returned

**Ecosystem**

- Fishing for an [ECDSA nonce reuse bot](https://www.bertcmiller.com/2021/12/28/glimpse_nonce_reuse.html) with Ether as bait
- Flashbots MEV Roast & research workshop [videos](https://www.youtube.com/channel/UCclbTgsnYUy3vmrptIqCmqQ)
- [Tutela](https://medium.com/@wmctighe_4577/tutela-tornado-cash-pool-anonymity-set-auditor-3c196d0cdf06): check anonymity of an address on Tornado Cash

**Enterprise**

- [Gamestop NFT marketplace](https://nft.gamestop.com/) opens applications for creators

**Application layer**

- [Aelin](https://mirror.xyz/seldon.eth/iwUxGuwCSe7uHPTBJyNAcF1XOsX-cYAFga860EYlLTw) deal coordination protocol live on Optimism
- [Real World Asset](https://medium.com/centrifuge/rwa-market-the-aave-market-for-real-world-assets-goes-live-48976b984dde) market live, built on Centrifuge and AAVE
- [Sperax](https://twitter.com/SperaxUSD/status/1474242087839096832) algorithmic USD stablecoin beta live on Arbitrum
- [Tokenized Time](https://mirror.xyz/0xB297faf8C856699F5A2163F8682Dbe4D5dc892fd/HeruNhvXhxXkYznRQ-evbhvQRzN-ufTDg4tmsGOzpZA): buy, sell and trade time, proof of concept
- [briq](https://twitter.com/briqs_/status/1475508112857698310) composable blocks to construct NFTs, alpha on StarkNet
- [Cryptopunks](https://www.larvalabs.com/blog/2021-11-11-18-0/open-sourcing-a-new-interface-for-the-cryptopunks-market) decentralized market beta, MIT license
- [Movement](https://twitter.com/cinematic_dev/status/1476261848890626053): 3D browser based gallery for an address/ENS
- Gnosis Guild’s [Zodiac bridge module](https://twitter.com/gnosisguild/status/1475499147348295680) allows a DAO on one network to control assets and interact with systems on another network
- [Paris Hilton](https://twitter.com/ethleaderboard/status/1476647213044416512) adds ENS to Twitter

* * *

### **Job Listings**

- Certora seeks [SR SW Eng](https://www.certora.com/#careers), [Security Res](https://www.certora.com/#careers), [Security Eng](https://www.certora.com/#careers) & [Community Manager](https://www.certora.com/#careers)
- The VAC team at Status.im are looking for a [blockchain engineer](https://jobs.status.im/?gh_jid=3712494)
- Geth team is looking for a [Senior Technical Writer](https://ethereum.bamboohr.com/jobs/view.php?id=51&source=weekinethnews)
- Kwenta seeks [Frontend Engineer](https://blog.kwenta.io/kwenta-open-position-front-end-developer/), [Solidity Engineer](https://blog.kwenta.io/kwenta-open-position-solidity-engineer/) & [Marketing Lead](https://blog.kwenta.io/kwenta-open-position-marketing-manager/)
- Are you a p2p networking whiz? EF research hiring [Networking Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=54&source=weekinethnews)
- [Textile](https://textile.io/) is hiring! [Blockchain Eng](https://grnh.se/f093ec154us), [Backend Eng](https://grnh.se/526aef8d4us), and [Partner Manager](https://grnh.se/06c1dfdf4us)

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Be mindful of [low effort airdrops](https://twitter.com/AndreCronjeTech/status/1476162044927819781): [OpenDAO](https://www.theopendao.com/)’s SOS based on amount spent on OpenSea; [Gas DAO](https://mirror.xyz/gasdao.eth/AwZGIpiVuIOkcwUaKqn4ZdcI4MetmYmvVdnuZsNZlaQ)’s GAS based on gas spent; [visualizations](https://twitter.com/takenstheorem/status/1476089648694931460) of SOS airdrop claim and [analysis](https://twitter.com/asvanevik/status/1476165444549726210) of top 25 recipients, 68% dumped their tokens
- [Mirrortable](https://balajis.com/mirrortable/): concept of a capitalization table mirrored on-chain to streamline angel investing
- Proposal to [port Aave v3 to StarkNet](https://governance.aave.com/t/arc-deploying-aave-on-starknet/6726) Layer 2
- [Bored Ape token](https://twitter.com/boredapeyc/status/1446569318540615681) expected Q1 2022 (beware of scams)
- [South Korean centralized exchanges](https://cointelegraph.com/news/south-korea-crypto-exchanges-to-follow-coinone-in-verifying-private-wallets) to block transfers to non-verified addresses
- [Bank of Mexico](https://twitter.com/GobiernoMX/status/1476376240873517061) plans for CBDC by 2024

**General**

- [Web3 is self certifying](https://jaygraber.medium.com/web3-is-self-certifying-9dad77fd8d81): authorship of content is proven with cryptographic user identifiers & content-addressed data
- [LastPass](https://blog.lastpass.com/2021/12/unusual-attempted-login-activity-how-lastpass-protects-you/) warns some users of unusual login attempt, due to credential stuffing, some alerts triggered in error
- [T-mobile](https://www.bleepingcomputer.com/news/security/t-mobile-says-new-data-breach-caused-by-sim-swap-attacks/) notifies small number of customers their SIMs were swapped
- [Halo2-franchise-proof](https://github.com/vocdoni/halo2-franchise-proof): experimental port of Vocdoni voting anonymizer zk circuit to the ZCash Halo2 proving system which doesn’t have a trusted setup

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-31-2021](https://weekinethereumnews.com/week-in-ethereum-news-december-31-2021)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- **Jan 13 – [MEV in 2021](https://github.com/flashbots/mev-research/issues/68) (virtual)**
- ****Jan 14-16 – ETHGlobal**’s [NFTHack](https://nft.ethglobal.com/) (virtual)**
- **Feb 15 - Apr 5 – [Cryptocurrency Class](https://mirror.xyz/0xaFaBa30769374EA0F971300dE79c62Bf94B464d5/oGqGP2NOK9g7QPl1sMKkzql_Fh0P6hKbpYLZ-EkQTXU) (virtual)** 
- Feb 17 – [Schelling Point](https://schellingpoint.gitcoin.co/) (Denver) 
- Feb 18-20 – [ETHDenver](https://www.ethdenver.com/)
- Mar 14-17 – [Eth Rio](https://www.ethrio.org/)
- Mar 29-31 – [ETHDubai](https://www.ethdubaiconf.org/)
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- May 3-8 – [spaghettETH](http://spaghett-eth.com/) (Milan)
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- **Jun 21-23 – [NFT.NYC](https://www.nft.nyc/)** 
- Jun 24-26  – [ETHNewYork](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4) 
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

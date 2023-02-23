---
title: "Week in Ethereum News <BR> July 24, 2021"
date: "2021-07-24"
---

## **Eth News and Links**

**Mainnet execution layer**

- Clients need to update after [consensus issue](https://github.com/ethereum/eth1.0-specs/blob/master/network-upgrades/retrospectives/london.md) found on Ropsten testnet, Geth included a transaction which OpenEthereum and Besu rejected; updated client versions:
    - Geth [v1.10.6](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.6)
    - Erigon [2021.07.04-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2021.07.04)
    - Nethermind [v1.10.79](https://github.com/NethermindEth/nethermind/releases/tag/1.10.79)
- Latest core devs [call](https://www.youtube.com/watch?v=tjvviOLy0hw&t=419s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1418618923172261892):
    - London upgrade date unchanged after consensus issue
    - gasPrice field will be set to maxFeePerGas and changes to effectiveGasPrice once mined, field to be removed next upgrade
    - Focus on Proof of Stake testnets post London
- [Naming upgrades](https://ethereum-magicians.org/t/ethereum-roadmapping-improvements/6653/12) discussion with polls
- [Access list transactions since Berlin upgrade](https://gist.github.com/perama-v/b9b8c5595f4ce9e3651b816da32d6841): ~270k transactions, ~5% of potential gas space
- [Chain history storage network](https://hackmd.io/ctTNH9xsSu2ci9DeGidUsQ?view) first draft: provides on-demand availability of historical block headers and block bodies
- [Storage layout](https://notes.ethereum.org/h58LZcqqRRuarxx4etOnGQ) proposal for state network
- Proposal for [EEICALL opcode](https://ethresear.ch/t/eeicall-opcode-to-execute-bytecode-over-given-eei/10161) to execute bytecode over given Execution Environment Interface

**EIPs/Standards**

- [EIP3664](https://github.com/ethereum/EIPs/pull/3664): next generation game NFT
- [EIP3670](https://eips.ethereum.org/EIPS/eip-3670): EOF - Code Validation

**Proof of stake consensus layer**

- Draft [EIP3675](https://github.com/ethereum/EIPs/pull/3675): Upgrade consensus to Proof-of-Stake
- Validators need to [update their execution clients](https://twitter.com/rauljordaneth/status/1418441045331808258) for the London consensus issue, validators running Prysm need to update Prysm
- [Lighthouse client](https://lighthouse.sigmaprime.io/update-37.html) update: focusing on Altair upgrade, doppelganger support and networking overhaul

**Layer2**

- [Reddit scaling Community Points](https://www.reddit.com/r/ethereum/comments/opi5rg/scaling_reddits_community_points_with_arbitrum/) using an Arbitrum rollup: starting with Rinkeby testnet then migrating to mainnet
- Celer [cBridge v1.0](https://blog.celer.network/2021/07/22/celer-cbridge-launches-seamlessly-bridging-cross-chain-and-cross-layer-liquidity-2/): instant token transfer between Ethereum, Arbitrum and selected sidechains
- StarkNet [Alpha 1](https://medium.com/starkware/starknet-alpha-1-90c3348cca4f): Layer1<>Layer2 messaging protocol and onchain data availability via state diff published to Ethereum

* * *

### **This newsletter is made possible thanks to [Celer](https://www.celer.network/)!**

![Celer](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

[Celer cBridge](http://cbridge.celer.network/) v1.0 is now live on mainnet! Users are now able to use cBridge to instantly transfer tokens across Ethereum, Arbitrum, Polygon and Binance Smart Chain, with many more side chain and layer-2 chain integrations planned for in the near future. Anyone can [run a cBridge node](https://github.com/celer-network/cbridge-node) to join the cBridge Network and provide cross-chain and cross-layer liquidity while generating yields through transaction fees.

* * *

**Stuff for developers**

- Hardhat [v2.5.0](https://github.com/nomiclabs/hardhat/releases/tag/hardhat-core-v2.5.0): Hardhat Network support for London
- Brownie [v1.15.0](https://github.com/eth-brownie/brownie/releases/tag/v1.15.0): Multicall context manager, Solidity 0.8 typed errors, EIP712 message signing, hardware wallet support, and Vyper v0.2.14
- [Permit Singleton](https://github.com/amxx/permit): meta transaction transfers for already deployed ERC20/721/1155 tokens via a singleton contract per network
- [micro-eth-signer](https://github.com/paulmillr/micro-eth-signer) updated for London and Berlin
- abi-to-sol [v0.3.0](https://github.com/gnidan/abi-to-sol/releases/tag/v0.3.0): adds a web UI and improved support for older Solidity versions
- Ledger [plugins](https://blog.ledger.com/ethereum-plugins/) to parse transaction fields and build custom displays for smart contracts
- Don’t use [spot price as an oracle](https://shouldiusespotpriceasmyoracle.com/)
- Beginner tutorial: [send transactions in React via useDapp](https://dev.to/jacobedawson/send-react-web3-dapp-transactions-via-metamask-2b8n)

**Security**

- Thorchain [exploit](https://twitter.com/THORChain/status/1418360743523618825) ~$8million; [call to malicious contract](https://twitter.com/bantg/status/1418586485725532165) can drain holders RUNE
- Array Finance [exploit](https://blocksecteam.medium.com/the-analysis-of-the-array-finance-security-incident-bcab555326c1) ~$500k, price manipulation drained the pool
- Alex’s rescuer perspective of saving funds from a [phishing scammer](https://amanusk.medium.com/frontrunning-a-scammer-95f34dd33cf8) using an Ethereum burner and Flashbots
- SupDucks [unrevealed on-chain metadata not private](https://medium.com/@hype-eth/how-we-bought-an-nft-before-reveal-for-an-18-eth-profit-e684c1cbfda9)
- 3 month [Secureum bootcamp](https://hackmd.io/@secureum/bootcamp-epoch0-announcement) for smart contract auditing

**Ecosystem**

- Georgios & Vitalik: [Reorgs in Ethereum](https://www.paradigm.xyz/2021/07/ethereum-reorgs-after-the-merge/), prevention measure is to speed up Proof of Work switch off, less of an issue with Proof of Stake as attack would require large portion of validators
- Flashbots Research on [MEV post EIP1559](https://hackmd.io/@flashbots/MEV-1559)
- Optimism experimenting with public goods funding using sequencing profits, first experiment is [retroactive public goods funding](https://medium.com/ethereum-optimism/retroactive-public-goods-funding-33c9b7d00f0c)
- [NFT series](https://stateful.mirror.xyz/rsUhYxXARr7j2iDjqJeelY7nc6CN_Y-MilVDP1S5voA) retroactively supporting EIP1559 contributors (Disclosure: I supported)
- [Ashton Kutcher asks Mila Kunis](https://twitter.com/aplusk/status/1417959228157878273) about Ethereum with special guest
- [#ETH gains the Ethiopian flag](https://twitter.com/Olympics/status/1418356081131130885) as Twitter adds flags to 3 letter country code hashtags for the Olympics
- Ethereum.org [Q3 roadmap](https://github.com/ethereum/ethereum-org-website/issues/3446)
- EthCC [mainstage videos](https://www.youtube.com/playlist?list=PLhM7rBgpVV-K3Dko5_PUhwy0DnwzR1lgN)

**Enterprise**

- [Bank of Korea selects GroundX for CBDC pilot](https://consensys.net/blog/press-release/groundx-partners-with-consensys-wins-bank-of-korea-central-bank-digital-currency-project/) with ConsenSys as technical partner

**Application layer**

- [Maker Foundation shutting down](https://blog.makerdao.com/makerdao-has-come-full-circle/) as MakerDAO is decentralized
- [DAppNode governance token](https://medium.com/dappnode/welcome-to-the-node-economy-3c6ea2ffa043): airdrop with 3 year claimable stream
- Tweet storm [list of DAOs](https://twitter.com/shegenerates/status/1417482201294311438) & strategies for picking them
- [PartyBid](https://github.com/PartyDAO/partybid): protocol to pool funds for bidding in NFT auctions
- Intro to [Axie Infinity](https://notboring.mirror.xyz/rPk2Ozej8JHZZ_qayaekCfc1OUUHkmzLtZF3axlfmok) and play to earn gaming model
- [AutographNFT](https://medium.com/alphawallet/how-autographnft-is-bringing-authenticity-to-nfts-aa711c86297e): use web2 IDs such as Twitter to autograph NFTs
- ZKNFT [alpha](https://blog.0xmons.xyz/83014466310): proof of concept NFT marketplace on zkSync
- [PawNFT](https://github.com/anish-agnihotri/PawNFT) on Rinkeby: NFT-collateralized lending using active auction
- Run a [local game](https://github.com/projectsophon/darkforest-local) of the Dark Forest
- Aave planning to build [Twitter alternative on Ethereum](https://decrypt.co/76278/defi-project-aave-to-release-ethereum-based-twitter-alternative-this-year)

**Regulation/business/tokens**

- EU proposal to [extend AML/CFT rules to entire crypto sector](https://ec.europa.eu/commission/presscorner/detail/en/ip_21_3690): service providers to conduct due diligence on their customers, anonymous crypto asset wallets will be prohibited
- US Working Group on Financial Markets [discussed stablecoins](https://home.treasury.gov/news/press-releases/jy0281): act quickly on regulatory framework, recommendations expected in coming months
- [Taming wildcat stablecoins](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3888752) paper - Gorton (Yale) and Zhang (US Fed)
- [USDC reserves](https://www.centre.io/hubfs/pdfs/attestation/Grant-Thorton_circle_usdc_reserves_07162021.pdf): 61% cash and equivalents
- [ETH, the world’s most valuable asset](https://static1.squarespace.com/static/5acc19529772aea736648f44/t/60f8320f0a353f345fc42d17/1626878483121/ETH%2C+The+World%27s+Most+Valuable+Asset.pdf)

**General**

- Detect NSO Group’s [Pegasus phone malware](https://www.amnesty.org/en/latest/research/2021/07/forensic-methodology-report-how-to-catch-nso-groups-pegasus/), used to target activists, politicians and journalists
- [Security analysis](https://mtpsym.github.io/) of Telegram, vulnerabilities disclosed in message reordering, encrypted message detection, plaintext recovery of encrypted messages and attacker in the middle
- Chrome patches 8th [zero day vulnerability](https://www.bleepingcomputer.com/news/security/google-patches-8th-chrome-zero-day-exploited-in-the-wild-this-year/) this year, reports of exploit in the wild
- DuckDuckGo [Email Protection beta](https://www.spreadprivacy.com/introducing-email-protection-beta/): removes email trackers from @duck.com and unique private email addresses

* * *

## **Job Listings**

- 🧙 [Defi marketing wizard](https://docs.float.capital/docs/marketing-lead?enl), Float.Capital seeks 🧙
- [Props](https://www.props.xyz/) is hiring a [Front End Blockchain Engineer](https://jobs.gohire.io/props-0ds2x7xe/front-end-blockchain-engineer-40634/)
- Alejandro from Synthetix: [smart contract engineer trainee](https://forum.ethernautdao.io/t/alejandro-from-synthetix-is-looking-for-a-smart-contract-engineer-trainee/22) via EthernautDAO
- Nethermind [internship program](https://www.notion.so/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-24-2021/](https://weekinethereumnews.com/week-in-ethereum-news-july-24-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- July 25-31 - [IC3 Blockchain Camp](https://www.initc3.org/events/2021-07-25-ic3-blockchain-summer-camp) (virtual)
- July 26+30 - [OpenZeppelin/ITBA free course](https://twitter.com/marquitos_eth/status/1411868494115786752) for devs in Spanish
- July 30 - [Sign in with Ethereum RFP](https://notes.ethereum.org/@djrtwo/sign-in-with-ethereum-RFP) deadline
- **August 1 - applications close for [Secureum auditing bootcamp](https://hackmd.io/@secureum/bootcamp-epoch0-announcement)**
- August 4 - [London hard fork](https://blog.ethereum.org/2021/07/15/london-mainnet-announcement/)
- August 12 - applications close for [EF small grants for events](https://esp.ethereum.foundation/en/devcon-grants/)
- Aug 27-29 - [Edcon](https://www.edcon.io/) (Shenzhen/online)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

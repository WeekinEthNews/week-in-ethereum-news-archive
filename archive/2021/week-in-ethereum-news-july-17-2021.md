---
title: "Week in Ethereum News <BR> July 17, 2021"
date: "2021-07-17"
---

## **Eth News and Links**

**Mainnet execution layer**

- [London upgrade](https://blog.ethereum.org/2021/07/15/london-mainnet-announcement/) goes live on block 12,965,000 ~August 4
- London ready client versions:
    - Geth [v1.10.5](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.5)
    - OpenEthereum [v3.3.0-rc.4](https://github.com/openethereum/openethereum/releases/tag/v3.3.0-rc.4)
    - Erigon [2021.07.03-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2021.07.03)
    - Nethermind [v1.10.77](https://github.com/NethermindEth/nethermind/releases/tag/1.10.77)
    - Besu [v21.7.1](https://github.com/hyperledger/besu/releases/tag/21.7.1)
- Dashboard of [clients synced for London](https://ethernodes.org/london)
- London upgrade EIPs in [visual format](https://analyticali.substack.com/p/ethereum-london-hark-fork)
- [Spreadsheet](https://docs.google.com/spreadsheets/d/1Ld4JSyaz-gvTx-4xIaxe4qU2wlaG1XAQfMiKl9CKCY0/edit#gid=0) showing how quickly EIP1559 baseFeePerGas rises/falls
- [Difficulty bomb explainer](https://twitter.com/nethermindeth/status/1414622903274905600) tweetstorm: prevents do nothing as an option, London may have been 1-6 months later without the bomb
- Tim Beiko’s proposal for Ethereum [long term planning](https://ethereum-magicians.org/t/ethereum-roadmapping-improvements/6653):
    - Stop considering EIPs for specific upgrades ~6 months in advance
    - ~2 upgrades per year
    - Agree roadmap of large initiatives for future upgrades
- [evmodin](https://github.com/vorot93/evmodin): Rust EVM implementation, port of evmone (C++)
- [Address Space Extension (ASE) with bridge-contracts](https://notes.ethereum.org/@axic/B1BUs526u) alternative proposal building on ASE with translation map
- Proposal for [overlay protocol](https://notes.ethereum.org/tPzmxQD_S3S3uvtpUSA0-g) for establishing and managing an overlay network for any number of sub-protocols

**EIPs/Standards**

- [EIP3651](https://eips.ethereum.org/EIPS/eip-3651): Warm COINBASE

**Proof of stake consensus layer**

- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210716): stakers need to update their execution clients before the London upgrade 
- PoS implementers [call](https://www.youtube.com/watch?v=-Bzq4s8Lr5E&t=338s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/SJT4An66O)
- [Altair devnet 1 upgraded](https://twitter.com/protolambda/status/1415665659665522697) from Phase 0 to Altair with 5 clients
- Altair [beta prerelease spec](https://github.com/ethereum/eth2.0-specs/releases/tag/v1.1.0-beta.1): no breaking changes unless critical issue
- Nimbus [v1.4.1](https://github.com/status-im/nimbus-eth2/releases/tag/v1.4.1): increase block attestation wait time to fix attestations being dropped by other nodes
- [VDF proving](https://ethresear.ch/t/vdf-proving-with-snarkpack/10096) with SnarkPack

**Layer2**

- [Optimism live with Uniswap V3](https://optimismpbc.medium.com/announcing-uniswap-v3-on-optimism-6fb033398a11): alpha, 50k transactions/day cap using congestion pricing, unplanned/planned downtime, 7 day withdrawal to mainnet, token bridge for DAI, WBTC, USDT, EURT, ETH, and SNX
- [Uniswap’s Optimism documentation](https://help.uniswap.org/en/collections/3033942-layer-2) on how to deposit, connect, swap and withdraw
- [Single permissioned sequencers](https://twitter.com/krzKaczor/status/1415326134552641536) in rollups
- [StarDrop](https://kobi.one/2021/07/14/stardrop.html): experimental project to distribute rewards in a privacy-preserving manner on StarkNet

* * *

### **This newsletter is made possible thanks to NEAR’s [Aurora](https://aurora.dev/) EVM and Bridge!**

![Aurora](https://weekinethereumnews.com/wp-content/uploads/2021/05/aurora-1024x341.jpeg)

Aurora is an Ethereum Layer-2 protocol that provides developers and users a seamless experience of Ethereum on top of [NEAR Protocol](https://near.org/): a scalable, developer-friendly blockchain platform for decentralized applications. Aurora’s design allows base fees to be paid in ETH or other ERC-20s and enables all existing ETH wallets and other tools to work out of the box. Users don’t even need to leave their MetaMask wallet while using Aurora. 

The Aurora environment consists of the Aurora Engine, a high performance EVM, and the Aurora Bridge, facilitating trustless transfer of ETH and ERC20 tokens between Ethereum and Aurora, within a seamless, familiar user experience. Join top ETH projects such as 1inch & DODO in building the multi-chain future. Start using [Aurora](https://aurora.dev/about) to scale your Ethereum project now. 

Check out our [EthCC talk on the Rainbow Bridge](https://ethcc.io/agenda)! “The First Fully Trustless Bridge to Ethereum” on July 20th at 5:05pm in the Monge room.

* * *

**Stuff for developers**

- Remix IDE [v0.14.0](https://medium.com/remix-ide/remix-ide-v0-14-0-is-released-3f6bdde42740): next opcode shown in debugger, multi-select files to delete
- [MetaMask JSON-RPC API](https://metamask.github.io/api-playground/api-documentation) playground for debugging
- [Preparing for EIP1559](https://blog.alchemy.com/blog/eip-1559): remove gasPrice, add maxPriorityFeePerGas and maxFeePerGas to your send transaction code
- [EIP1559 fee estimator](https://github.com/zsfelfoldi/ethereum-docs/blob/master/eip1559/feeHistory_example.js) using the eth\_feeHistory API
- [Upgradeable smart contracts with Brownie](https://github.com/brownie-mix/upgrades-mix): based on OpenZeppelin transparent proxy
- [Scribble generator](https://consensys.net/diligence/blog/2021/07/introducing-scribble-generator/): add Scribble annotations to Echidna and Dapptools fuzz test cases
- Fe compiler [JavaScript bindings](https://github.com/mjobuda/vscode-fe/tree/tokenprovider/fejs)
- [OpenZeppelin subgraphs](https://blog.openzeppelin.com/subgraphs-announcement/) library to build subgraphs of commonly used contracts from OpenZeppelin Contracts including ERC20 and ERC721
- Otterscan [v2021.07.03](https://twitter.com/wmitsuda/status/1415772224255053825): Erigon connection checks, Chainlink integration, focus highlighting and smaller binary distribution
- [Web3 login for MetaMask](https://dev.to/jacobedawson/build-a-web3-dapp-in-react-login-with-metamask-4chp) using React
- [Rarepress](https://rarepress.org/): 2 lines of JavaScript to lazy mint NFTs on Rarible with metadata on IPFS

**Security**

- Anyswap V3 bridge [exploit](https://www.rekt.news/anyswap-rekt/) ~$8million, two transactions with the same R value enabled hacker to deduce private key
- ChainSwap bridge [logic error](https://chain-swap.medium.com/chainswap-exploit-11-july-2021-post-mortem-6e4e346e5a32) ~$4million, unauthorized addresses increased quota
- Thorchain bridge [exploit](https://twitter.com/mudit__gupta/status/1415894999049261056) ~$5million, attackers wrapper contract deposited zero value from transaction sent value
- Bondly finance [minting exploit](https://www.rekt.news/bondly-rekt/) ~$6million, using admin account
- DefiPlaza [exploit](https://twitter.com/mudit__gupta/status/1414838405569994754), overflow allowing pool to be drained
- Victims perspective of [$117k rescue](https://www.reddit.com/r/CryptoCurrency/comments/oip4mi/if_you_want_to_join_me_in_watching_metamask/) using Flashbots and an Ether burner for phished secret phrase

**Ecosystem**

- Trent’s [Ethereum upgrade path](https://twitter.com/trent_vanepps/status/1415741658067517441) infographic
- [Flashbots on incentivized reorg clients](https://medium.com/flashbots/flashbots-on-reorgs-914e397b78d8), negative-sum, unstable game for everyone
- [Back running the MEV crisis](https://medium.com/dragonfly-research/we-live-in-a-mempool-backrunning-the-mev-crisis-a4ea0b493b05): embrace MEV, hide MEV, unionize and evolve
- [Ethernaut DAO](https://ethernautdao.medium.com/introducing-the-ethernautdao-21bfca20ee80): 2 month mentoring program to convert senior developers to senior Solidity developers
- [Ethereum: The Infinite Garden](https://ethereumfilm.mirror.xyz/3SV8gLXHIW8Ot45h3RL7aOgDINxN2hjLfFVOvyatB2A) documentary film, fundraised ~1000ETH using Mirror and NFTs by pplpleasr

**Enterprise**

- [ConsenSys Quorum update](https://consensys.net/blog/quorum/consensys-quorum-21-7-0-product-update-london-hard-fork-qbft-and-more/): QBFT consensus algorithm, Tessera private transaction manager support; web3js-quorum JavaScript web3 library

**Application layer**

- [Unique addresses per DeFi project](https://duneanalytics.com/k06a/DeFi-Project-Users): Uniswap ~2.4million, 1inch ~0.5million
- [Hop](https://medium.com/hop-protocol/hop-is-live-2dbd4721b1bc) is live: almost immediate token bridge between Ethereum and scaling networks, starting with USDC and sidechains
- [Ribbon Finance yvUSDC ETH Put Selling Vault](https://ribbonfinance.medium.com/stacking-ribbon-x-yearn-yield-b585e6bc2d70), allows stacking Ribbon and Yearn yield at the same time, $10 million deposit cap 
- [SuperRare collector royalties](https://medium.com/superrare/the-art-royalty-revolution-6c0d13a6912a): 12 month pilot of 1% transaction royalty for collectors decaying by 50%
- [DAO-to-DAO loan](https://medium.com/cream-finance/c-r-e-a-m-finance-facilitates-first-dao-to-dao-loan-with-iron-bank-and-pleasrdao-ed001f3b391): $3.5million credit line for PleasrDAO from Iron Bank collateralized by NFTs with a purchase price of ~$10million
- [Tribute DAO framework](https://medium.com/@OpenLawOfficial/introducing-the-tribute-dao-framework-3f2f0ed50d62): customizable, upgradeable, Snapshot integration for gasless voting and uses an optimistic rollup
- [Radicle Orgs](https://radicle.xyz/blog/radicle-orgs.html) decentralized code management for DAOs built on Gnosis Safe
- [Holly+ DAO](https://holly.mirror.xyz/54ds2IiOnvthjGFkokFCoaI4EabytH9xjAYy1irHy94) to govern Holly Herndon’s voice model rights
- [Giveth TRACE](https://medium.com/giveth/giveth-trace-is-live-e91b0be1e1f6): donations disbursed on mainnet, Rinkeby testnet used for donation management

**Regulation/business/tokens**

- [Ultrasound.money](https://ultrasound.money/): estimate peak ETH supply, as EIP1559 and Proof of Stake reduce ETH issuance
- Python based [Ethereum economic model](https://twitter.com/CADLabs_org/status/1415986905485910023)
- European Central Bank preparing for [possible digital euro](https://www.ecb.europa.eu/press/blog/date/2021/html/ecb.blog210714~6bfc156386.en.html)
- [SEC charged Coinschedule](https://www.sec.gov/news/press-release/2021-125) for failing to disclose compensation from ICOs it profiled, [Commissioner Peirce dissent](https://www.sec.gov/news/public-statement/peirce-roisman-coinschedule) as didn’t specify which tokens were securities and the reasons why
- [ShapeShift becoming a DAO](https://erikvoorhees.medium.com/shapeshift-is-decentralizing-639bb4c82fc8): dissolving corporate entities, dropped tokens for ~1 million users of ShapeShift and DeFi

**General**

- Matthew Ball: [Metaverse Primer](https://www.matthewball.vc/the-metaverse-primer)
- Vitalik: [M-of-N secret sharing](https://ethresear.ch/t/m-of-n-secret-sharing-with-pre-known-shares/10074) with pre-known shares
- [Publicly auditable MPC as a service](https://arxiv.org/abs/2107.04248) with succinct verification and universal setup
- Revised [cryptanalysis of an oblivious PRF from supersingular isogenies](https://eprint.iacr.org/2021/706) paper, adding the result of the 67 bits attack which took 1.89days

* * *

## **Job Listings**

- Prysmatic labs: [Software Development Engineer in Test (SDET)](https://prysmaticlabs.com/careers/sdet)
- [Synthetix](https://twitter.com/kaiynne/status/1415573456146501634): 2 Solidity engineers to work direct with Kain Warwick in Sydney
- Sourcify looking for an [experienced TypeScript developer](https://ethereum.bamboohr.com/jobs/view.php?id=38)

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-17-2021/](https://weekinethereumnews.com/week-in-ethereum-news-july-17-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- July 20-22 - [EthCC4](https://ethcc.io/) (Paris)
- July 21 - [ETHécole Conference](https://medium.com/ethereum-magicians/ethecol%C3%A9-conference-all-you-need-to-know-7867dec7eaf6) (Paris)
- July 25-31 - [IC3 Blockchain Camp](https://www.initc3.org/events/2021-07-25-ic3-blockchain-summer-camp) (virtual)
- July 26+30 - [OpenZeppelin/ITBA free course](https://twitter.com/marquitos_eth/status/1411868494115786752) for devs in Spanish
- **July 30 - [Sign in with Ethereum RFP](https://notes.ethereum.org/@djrtwo/sign-in-with-ethereum-RFP) deadline**
- August 4 - [London hard fork](https://docs.google.com/spreadsheets/d/1Y3yyTqeqRO1O2UFVkNkHK_V5oRulZd6y-JJbSnKYrb4)
- **August 12 - applications close for [EF small grants for events](https://esp.ethereum.foundation/en/devcon-grants/)**
- Aug 27-29 - [Edcon](https://www.edcon.io/) (Shenzhen/online)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

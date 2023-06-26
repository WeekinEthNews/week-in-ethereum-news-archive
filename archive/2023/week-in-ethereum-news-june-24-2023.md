---
title: "Week in Ethereum News <br> June 24, 2023"
date: "2023-06-24"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=09Kzi2x06UM&t=105s). Summary by [Tim Beiko](https://twitter.com/abcoathup/status/1672007424033816577).  Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1671927373749686272) and [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-execution-call-164/):
    - [Overview of execution spec tests](https://notes.ethereum.org/@danceratopz/execution-spec-tests-overview-202306), Python suite of state & blockchain tests
    
    - Dencun upgrade discussions: EIP4844 precompile address moved to 0xA, EIP4788 storage size bounded, EIP5656 (MCOPY) tests added and Engine API spec changes
    
    - EIP4844 devnet 6 had issues, restart as devnet 7 once stable client releases & pass hive tests
    
    - EIP repo to split out app layer ERCs

- Consensus specs [v1.4.0-beta.0](https://github.com/ethereum/consensus-specs/releases/tag/v1.4.0-beta.0): Deneb feature complete, stable unless issues found

- EIP4844:
    - Kelvin: [Mr. Moloch's ephemeral album party](https://kelvinfichter.com/pages/thoughts/moloch/) contribution to KZG ceremony

**Layer 1**

- [Reth v0.1.0-alpha](https://www.paradigm.xyz/2023/06/reth-alpha): execution layer client in Rust, syncs archive node in 50 hours with 2TB database using NVMe SSD, also SDK for building EVM infrastructure, Apache/MIT license

- EthereumJS [v6](https://twitter.com/efjavascript/status/1671137022478540802) (final release before v7): updates ethereum-cryptography, adds allowUnlimitedInitcodeSize option and removes non-finalized state code (EIP4844)

- [Verkle tries](https://verkle.info) info website

**Client releases**

- Consensus layer:
    - Lodestar [v1.9.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.9.0): fix reduced slashing DB size by 97%, slashing protection export format compatible with other clients and flag to disable peer scoring for testing
    
    - Nimbus [v23.6.0](https://github.com/status-im/nimbus-eth2/releases/tag/v23.6.0): history prune enabled by default, processes untimely attestations without expensive state replays and use Keymanager API for voluntary exits

- Execution layer:
    - Erigon [v2.47.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.47.0): fix for v2.45.0, no resync required

**For Stakers**

- [Execution Layer client diversity improved](https://clientdiversity.org/#distribution), Geth around 50%

**Research**

- [Fast amortized KZG proofs](https://eprint.iacr.org/2023/033)

- [Speculative execution DoS attacks](https://www.researchgate.net/publication/371641235_Speculative_Denial-of-Service_Attacks_in_Ethereum) using conditional transactions to exhaust resources and/or transaction pool spamming

**Layer 2**

- [Zora Network](https://docs.zora.co/docs/zora-network/intro) for NFTs, optimistic rollup built on OP stack, live

- [Arbitrum Orbit chains](https://developer.arbitrum.io/launch-orbit-chain/orbit-gentle-introduction) (layer 3): guide to launch a devnet

- L2Beat [Stages](https://medium.com/l2beat/introducing-stages-a-framework-to-evaluate-rollups-maturity-d290bb22befe): rollup maturity framework from stage 0 (run by the operators) to stage 2 (fully managed by contracts)

- [Shared validity sequencing](https://www.umbraresearch.xyz/writings/shared-validity-sequencing) proposal to enable cross-rollup interoperability

- Vitalik: [L2 to L1 & cross-L2 reading](https://vitalik.ca/general/2023/06/20/deeperdive.html) to implement cross-chain social recovery wallets with a keystore in one location & wallets in many locations

**EIPs/Standards**

- EIPs:
    - Meta [EIP7199](https://eips.ethereum.org/EIPS/eip-7199): Linter scope 
    
    - [EIP7212](https://github.com/ethereum/EIPs/pull/7212/files): Precompile for secp256r1 curve support

- ERCs (app layer):
    - [ERC838](https://github.com/ethereum/EIPs/pull/7186/files): ABI specification for REVERT reason string
    
    - [ERC7196](https://github.com/ethereum/EIPs/pull/7197/files): Simple token
    
    - [ERC7201](https://eips.ethereum.org/EIPS/eip-7201): Namespaced storage layout 
    
    - [ERC7202](https://github.com/ethereum/EIPs/pull/7202/files): Offchain checks (for low cost ERC1155 distribution)
    
    - [ERC7204](https://github.com/ethereum/EIPs/pull/7204/files): Contract wallet management asset
    
    - [ERC7208](https://github.com/ethereum/EIPs/pull/7210/files): MetaNFT keystore contracts 

**Stuff for developers**

- Hardhat:
    - [v2.16.0](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.16.0): adds extendable providers, wrap network provider with custom logic
    
    - [Hardhat-ledger plugin](https://github.com/NomicFoundation/hardhat/releases/tag/%40nomicfoundation/hardhat-ledger%401.0.0): send transactions & sign messages

- [Alloy](https://www.paradigm.xyz/2023/06/alloy): rewrite of ethers-rs, includes Solidity's type system in Rust

- Guide to [Solidity data locations](https://blog.smlxl.io/solc-internals-part-2-data-locations-2f6517aeb154) (memory, calldata & storage)

- Cookbook [ChefGPT](https://twitter.com/cookbook_dev/status/1670866221066235904) Remix plugin to answer Solidity questions including on current contract

- [Intro to Ape](https://snakecharmers.ethereum.org/intro-to-ape/) (contract development framework for Python devs) using WETH as an example

- Uniswap v4 [flash loan template](https://github.com/jtriley-eth/uni-v4-core-flashloans#readme) 

- Seaport [Validator & Navigator](https://twitter.com/z0age/status/1671531066287353858): helper contracts to scan orders for errors and fulfill respectively

- Simon de la Rouviere: [Daisychains NFT onchain SVG animation](https://www.untitledfrontier.studio/blog/behind-the-scenes-crafting-the-onchain-daisychains) \[Andrew had one free mint\]

- [Smoldata](https://www.smoldata.xyz/): zero-ETL indexing for contracts

**Security**

- Astaria (NFT lending) [vulnerability disclosed](https://twitter.com/AstariaXYZ/status/1671215491069927429), protocol paused with tokens rescued, beacon proxy could be manipulated to load rogue implementation allowing self destruct

- Foundation NFT contracts [vulnerability disclosed](https://twitter.com/0xngmi/status/1671344096441499648), contract owner can self destruct implementation, destroying minted NFTs

- Tincho: [questions auditors should ask devs](https://blog.theredguild.org/auditors-what-do-you-ask-developers/) before a secure code review.

**Ecosystem**

- Etherscan [code reader](https://etherscan.io/code-reader), answers questions about a specific contract address, OpenAI API key required, beta

**Enterprise**

- Paul Brody: [Ethereum for Business](https://www.uapress.com/product/ethereum-for-business/) book

- [SAP demoing cross border payments with USDC](https://blogs.sap.com/2023/06/15/cross-border-payments-made-easy-with-digital-money-experience-the-future-today/): customers can pay a sample invoice on testnet

**Notable at app layer**

- Maker [sDAI](https://twitter.com/makerdao/status/1671220727322906624) (savings DAI): tokenized DSR-enabled DAI, ERC4626

- Utopia [transaction templates](https://twitter.com/utopialabs_/status/1671276761013690373) for Safe multisig on mainnet

- PartyDAO [Party](https://twitter.com/prtydao/status/1671926165395718205): create groups with lightweight voting to take onchain actions

- Mirror [collectable embeds](https://dev.mirror.xyz/3gA4vAjijdwueXtmZ9WIkqh3my6R8jbLmZwPr37dQ2U): mint or buy on secondary NFTs embedded in posts

- [Noun Nyms](https://twitter.com/personae_labs/status/1671557431552544768): persistent pseudonyms for Noun holders with reddit-like interface

- [Ethscriptions](https://twitter.com/dumbnamenumbers/status/1669822912579223552): create/transfer digital artifacts using data URI in calldata, similar to Bitcoin Ordinals

- [BND](https://twitter.com/niftynaut/status/1671643671073005569) (German foreign intelligence) released dog NFTs

- Sudo v2 [gradual dutch auction bonding curves](https://twitter.com/0xmons/status/1670723757118480386)

- [Gitcoin grants stack](https://twitter.com/grantsstack/status/1670836700392595456): create & manage a grants program

* * *

### Job Listings

- Devconnect Istanbul: [Production Assistant](https://jobs.lever.co/ethereumfoundation/db6e2775-39d3-4eb9-9313-dfb15dfab9bc) and [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/401e0af5-f4a2-4e66-a724-4accb003113e)

- Solidity team need a highly skilled [Developer Advocate](https://jobs.lever.co/ethereumfoundation/b9e33c9e-48ee-464f-a672-d51eece2b99d)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- FT: [Crypto.com internal trading teams](https://archive.is/qBF6W) potential conflict of interest

**General/crypto**

- [Polygon PoS proposal](https://forum.polygon.technology/t/pre-pip-discussion-upgrading-polygon-pos-to-a-zkevm-validium/12187) to upgrade to a zkEVM validium in 2024

- [BSC adding layer 2](https://www.bnbchain.org/en/blog/introducing-opbnb-unleashing-a-new-era-of-scalability/) (Optimism fork) on testnet

- [Security proof of Nova](https://eprint.iacr.org/2023/969) on a cycle of curves  

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-june-24-2023](https://weekinethereumnews.com/week-in-ethereum-news-june-24-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jun 26 – Jul 17 – [CLRFund round 9](https://blog.clr.fund/clrfund-round-9-is-coming/)

- Jul 5-9 – [ETHBarcelona](https://ethbarcelona.com/) conference & hackathon

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- **Jul 20–23 –** [**Pragma Paris**](https://ethglobal.com/events/pragma-paris) & [ETHGlobal Paris](https://ethglobal.com/events/paris2023) hackathon

- Aug 11-13 – [ETHMunich](https://ethmunich.de/) hackathon

- Aug 15-16 – [ETHToronto](https://www.ethtoronto.ca/) & [ETHWomen](https://www.ethwomen.com/)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org/) (Buenos Aires)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 30 – Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- **Sep 15-17 –** [**ETHChicago**](https://www.ethchicago.xyz/) **conference & hackathon**

- Sep 18-21 – [ETH Montréal](https://ethmontreal.xyz/) conference & hackathon

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 6–27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- **Oct 13–15 –** [**Ethereum Kuala Lumpur**](https://twitter.com/ethkl1/status/1670761473348624384) **conference & hackathon**

- Oct 27–29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://twitter.com/ethbrno/status/1652198745902137344)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 17-19 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

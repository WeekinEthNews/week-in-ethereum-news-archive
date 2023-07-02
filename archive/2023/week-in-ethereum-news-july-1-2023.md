---
title: "Week in Ethereum News <br> July 1, 2023"
date: "2023-07-01"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=zdqtl9x_UjA&t=310s). Notes from [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-consensus-call-112/):
    - Deneb upgrade Engine API changes: deprecate Merge config exchange and proposed flag for EL to suggest local block building
    
    - EIP7251 (increase max effective balance) discussion
    
    - E-star name upgrade candidate for inclusion: EIP7002 (EL triggerable exits)

- EIP4844:
    - [EIP4844 devnet 7](https://4844-devnet-7.ethpandaops.io/) launched (same spec as devnet 6)
    
    - Latest EIP4844 implementer [call video](https://www.youtube.com/watch?v=WFwXitiwv-Q). Notes from [Terence](https://twitter.com/terencechain/status/1673366026313162752). Devnet 8 should include Dencun EIPs

- Execution-spec-tests [v1.0.0](https://github.com/ethereum/execution-spec-tests/releases/tag/v1.0.0): upgraded to PyTest, EIP4844 tests

**Layer 1**

- Holešky testnet (Goerli successor) [coordination call notes](https://github.com/ethereum/pm/issues/814#issuecomment-1613224057): 1.7M validators planned, with 800k run by client teams, genesis planned for September 15 (Merge day)

- MEV-Boost [v1.6](https://github.com/flashbots/mev-boost/releases/tag/v1.6): additional data availability and logging improvements

- Proposal to [remove RIPEMD-160 & blake2f precompiles](https://ethereum-magicians.org/t/discussion-removal-of-ripemd-160-and-blake2f-precompiles/14857)

- [Understanding enshrined PBS](https://mirror.xyz/0x55a0c204c6fDd0DCf238430cb4BF79D45e8D9Bc3/kw_7qbkOl4NV1pmpRgVwtsS-7TZff_zTmmNEOm2BbmU)

**Client releases**

- Consensus layer:
    - Lodestar [v1.9.1](https://github.com/ChainSafe/lodestar/releases/tag/v1.9.1): patch for peering/attestation issues & logging UX
    
    - Nimbus [v23.6.1](https://github.com/status-im/nimbus-eth2/releases/tag/v23.6.1): database pruning performance improvement for history prior to April 2021

- Execution layer:
    - Besu [v23.4.4](https://github.com/hyperledger/besu/releases/tag/23.4.4): new flat database improves block processing time & attestation performance, BlobDB for non-state blockchain data improves sync time & disk IO

**Research**

- [BaseSAP](https://arxiv.org/abs/2306.14272): stealth address protocol, extendable for particular cryptographic schemes

**EIPs/Standards**

- EIPs:
    - [EIP7251](https://github.com/ethereum/EIPs/pull/7251/files): Increase the MAX\_EFFECTIVE\_BALANCE

- ERCs (application layer):
    - [ERC7229](https://github.com/ethereum/EIPs/pull/7229/files): Minimal upgradable proxy contract
    
    - [ERC7231](https://github.com/ethereum/EIPs/pull/7231/files): Identity aggregated NFT
    
    - [ERC7246](https://github.com/ethereum/EIPs/pull/7246/files): Encumber (ERC20 extension)
    
    - [ERC7253](https://github.com/ethereum/EIPs/pull/7253/files): Universal wallet uplink
    
    - [ERC7254](https://github.com/ethereum/EIPs/pull/7254/files): Token revenue sharing

**Stuff for developers**

- Remix [v0.34.0](https://medium.com/remix-ide/remix-release-v0-34-0-f40d90c197e2): EVM version label, adds SolHint linter to Solidity analyzers, Etherscan contract verification adds L2 support, constructor arguments & proxy support

- Foundry:
    - [ForGePT](https://forgept.apoorv.xyz/): trained on Foundry book & Telegram support channel, OpenAI API key required

- [Solidity events](https://mirror.xyz/spacesailor.eth/LEe2yoLoqy97BWHyO6J65XhnG8t33Nmvz_Vsa3ve7rY): guide to logging and using web3.js to retrieve/listen 

- [Function Requirements-Effects-Interactions + Protocol Invariants](https://www.nascent.xyz/idea/youre-writing-require-statements-wrong) (FREI-PI) pattern

- Viem [v1.2](https://twitter.com/wagmi_sh/status/1673832563931238400): extend a client with custom actions

- [Raw transaction signing script](https://github.com/pcaversaccio/raw-tx/tree/main#readme) using ethers.js

- Overview of [Python ecosystem](https://snakecharmers.ethereum.org/python-ecosystem/): web3.py, py-evm, eth-tester, Ape, Woke, Vyper & Titanoboa

- [Noble-ciphers](https://github.com/paulmillr/noble-ciphers#readme): Salsa20, ChaCha, Poly1305 & AES-SIV in JavaScript, no dependencies

- Slither [v0.9.4](https://github.com/crytic/slither/releases/tag/0.9.4) & [v0.9.5](https://github.com/crytic/slither/releases/tag/0.9.5) patch: new detectors: cache-array-length, encode-packed-collision & incorrect-using-for; new printer: lines of code; adds interface generator and support for custom storage layouts

- RareSkills: [Tornado Cash code base explainer](https://www.rareskills.io/post/how-does-tornado-cash-work)

- CTF: [Decently Safe DeFi](https://decentlysafedefi.xyz/me/), 4 challenges, uses Foundry

- [E2PG](https://github.com/orgs/indexsupply/discussions/122): Ethereum to Postgres indexer

**Security**

- Themis (lending) on Arbitrum [$370k exploit](https://twitter.com/BlockSecTeam/status/1673897088617426946) via oracle manipulation

**Ecosystem**

- EF [academic grant recipients](https://blog.ethereum.org/2023/06/28/academic-grants-round-23): 43 projects share $2 million in funding

- ETHGlobal Waterloo [hackathon finalists](https://twitter.com/ethglobal/status/1673069276805099520) & [videos](https://www.youtube.com/playlist?list=PLXzKMXK2aHh7ZShjCVqztXMbdm9xTSqIR)

**Notable at app layer**

- USDC [Cross-Chain Transfer Protocol](https://www.circle.com/en/cross-chain-transfer-protocol) (CCTP) live on mainnet & Arbitrum

- [The Graph](https://twitter.com/graphprotocol/status/1674143754725277697) served 1 trillion queries

- Mirror [Writing NFTs v2](https://dev.mirror.xyz/8MThiFhn391cfgffQtiRoSpS-Op93IR71rYgf6YEzBc): read post in NFT and open editions

- Diva (DVT liquid staking) [DAO airdrop](https://divastaking.medium.com/announcing-the-diva-dao-270bb0d188e8) claimable by stakers, non-transferable so presumably no taxes incurred, frontend blocks US/Canada

- [CLRFund round 9](https://blog.clr.fund/round-9-is-underway/) live on Arbitrum, contribute to public goods

* * *

### Job Listings

- Devconnect Istanbul: [Production Assistant](https://jobs.lever.co/ethereumfoundation/db6e2775-39d3-4eb9-9313-dfb15dfab9bc) and [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/401e0af5-f4a2-4e66-a724-4accb003113e)

- Solidity team need a highly skilled [Developer Advocate](https://jobs.lever.co/ethereumfoundation/b9e33c9e-48ee-464f-a672-d51eece2b99d)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- UK [Financial Services & Markets act](https://www.coindesk.com/policy/2023/06/29/uk-crypto-stablecoin-rules-receive-royal-assent-passing-into-law/) enables regulation of crypto

- [HSBC Hong Kong](https://twitter.com/WuBlockchain/status/1673263927780859904) allows customers to buy/sell Ether ETF

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-1-2023](https://weekinethereumnews.com/week-in-ethereum-news-july-1-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jul 5-9 – [ETHBarcelona](https://ethbarcelona.com/) conference & hackathon

- **Jul 17 –** [**CLRFund round 9**](https://blog.clr.fund/round-9-is-underway/) **ends**

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 20–23 – [Pragma Paris](https://ethglobal.com/events/pragma-paris) & [ETHGlobal Paris](https://ethglobal.com/events/paris2023) hackathon

- Aug 11-13 – [ETHMunich](https://ethmunich.de/) hackathon

- Aug 15-16 – [ETHToronto](https://www.ethtoronto.ca/) & [ETHWomen](https://www.ethwomen.com/)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org/) (Buenos Aires)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 31 – Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 15-17 – [ETHChicago](https://www.ethchicago.xyz/) conference & hackathon

- Sep 18-21 – [ETH Montréal](https://ethmontreal.xyz/) conference & hackathon

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 6–27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 13–15 – [Ethereum Kuala Lumpur](https://hack.ethkl.org/) conference & hackathon

- Oct 27–29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- **Oct 31 –** [**Road to Devcon grants**](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) **application deadline**

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://twitter.com/ethbrno/status/1652198745902137344)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 17-19 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

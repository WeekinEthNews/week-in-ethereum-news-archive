---
title: "Week in Ethereum News <br> June 3, 2023"
date: "2023-06-03"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs - consensus (ACDC) [call video](https://www.youtube.com/watch?v=050Jq9lO838&t=242s). Notes from [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-consensus-call-110/):
    - Discussions on bounding EIP4788 (beacon root in EVM), implementation complexity of EIP6988 (prevent slashed validator being elected block proposer) and Engine API versioning
    
    - Dankrad tested big blocks on mainnet to size safe blobs per block, recommends increasing blobs per block target to 3 with a maximum of 6, up from 2 & 4 respectively

- EIP4844:
    - Latest EIP4844 implementer [call video](https://www.youtube.com/watch?v=lZiotV3nNIU&t=4s). Notes from [Terence](https://twitter.com/terencechain/status/1663232693566586880): Engine API versioning, add data\_gas\_used to execution header and devnet 6 scope
    
    - Terence: [validator & builder interaction with blob transactions](https://hackmd.io/zRO9lv-hS1-RX6yvbLK9oA?view) in Dencun
    
    - [KZG ceremony](https://ceremony.ethereum.org/) hit [100k contributions](https://twitter.com/CarlBeek/status/1662456925374521344), available to anyone with 16 mainnet transactions

- Consensus-specs [v1.4.0-alpha.1](https://github.com/ethereum/consensus-specs/releases/tag/v1.4.0-alpha.1): adds data\_gas\_used and changes excess\_data\_gas & data\_gas\_used type from uint256 to uint64

**Layer 1**

- EthStaker: [node operators should use minority execution clients](https://paragraph.xyz/@ethstaker/execution-client-diversity) (not Geth)

- Guide to [beacon chain networking components](https://hackmd.io/@dmarz/ethereum_overlays): p2p overlays & GossipSub

- [Intents in account abstraction](https://www.paradigm.xyz/2023/06/intents), they are great but come with risks of block production centralization, trust-based barriers to entry and lack of transparency

- [Ethereum halving proposal](https://twitter.com/phabcd/status/1664629884101046273): reduce staking requirement from 32 ETH to 1 ETH over 8 years, thanks to hardware & client improvements

**Client releases**

- Execution layer:
    - Besu [v23.4.1](https://github.com/hyperledger/besu/releases/tag/23.4.1): experimental transaction pool for more profitable local block production
    
    - Erigon [v2.44.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.44.0): Caplin (embedded CL) improvements, added new Sepolia testnet bootnodes
    
    - Nethermind [v1.19.0](https://github.com/NethermindEth/nethermind/releases/tag/1.19.0): faster sync and reduced database size (fresh sync required for full benefits of disk space optimization)

**For Stakers**

- [Validator queue dashboard](https://www.validatorqueue.com/) with historical charts

**Research**

- Longitudinal study of [block construction market](https://arxiv.org/abs/2305.16468): measures MEV-Boost & money flows and introduces a MEV-time law

**Layer 2**

- [RFP](https://github.com/ethereum-optimism/ecosystem-contributions/issues/61) to build zk validity prover for OP Stack

- [Kinto](https://mirror.xyz/0xc1f4D15C16A1f3555E0a5F7AeFD1e17AD4aaf40B/jUsuqznqrfUCpmWod5PiiKGm4S8eTl7dnO1B4CaD21Y) (optimistic rollup, KYC users only) live on testnet

- Norswap: [rollup definition debate is noise](https://twitter.com/norswap/status/1664462934360092674), focus on the specific security assumptions

- Polygon zkEVM [vulnerability disclosed](https://twitter.com/0xiczc/status/1662090451493740545), could DoS sequencer & prover

**EIPs/Standards**

- ERCs:
    - [ERC7085](https://github.com/ethereum/EIPs/pull/7085/files): NFT relationship enhancement
    
    - [ERC7087](https://github.com/ethereum/EIPs/pull/7087/files): MIME type for web3 URL in auto mode
    
    - [ERC7092](https://github.com/ethereum/EIPs/pull/7092/files): Financial bonds
    
    - [ERC7093](https://github.com/ethereum/EIPs/pull/7093/files): Social recovery interface
    
    - [ERC7099](https://github.com/ethereum/EIPs/pull/7099/files): Offchain checks (for low cost ERC20 distribution)
    
    - [ERC7108](https://github.com/ethereum/EIPs/pull/7108/files): Clustered ERC721
    
    - [ERC7110](https://github.com/ethereum/EIPs/pull/7115/files): NFT dynamic ownership
    
    - [ERC7121](https://github.com/ethereum/EIPs/pull/7121/files): SoulBounds Interface (soulbound assets ERC1155 extension)

**Stuff for developers**

- [Rinkeby testnet](https://twitter.com/peter_szilagyi/status/1664298102277251075) was shutdown

- Foundry:
    - [Iron wallet](https://mirror.xyz/iron-wallet.eth/OnCNvwKBs6ZpJrOVQQqsqHFW1RkqEK7MAsbPSIQNRFo): dev focused browser extension wallet, Anvil aware
    
    - Tip: [print colorful logs](https://twitter.com/paulrberg/status/1663498994503368704) using console2 & StdStyle
    
    - Tip: [fuzz private keys](https://twitter.com/paulrberg/status/1664207399744421890) using boundPrivateKey

- [Zipped contracts](https://github.com/merklejerk/zipped-contracts#readme): low cost deployment for contracts called offchain, self-extracts when called

- [Pack structs manually](https://twitter.com/real_philogy/status/1663882285811212290) for ~200-300 gas saving per struct change

- [N-per-epoch](https://github.com/rsproule/n-per-epoch#readme): modifier to rate limit a contract function call by humans

- [Cookbook VS Code extension](https://twitter.com/cookbook_dev/status/1663562176697864192): find contracts from Cookbook registry

- Ape [v0.6.10](https://twitter.com/ApeFramework/status/1664058070128033793): event log comparison, historical log optimization, account option flag for test accounts

- [EVM CFG](https://github.com/plotchy/evm-cfg#readme): control flow graph generator for unverified contracts using symbolic stack analysis

- Hardhat-ethers [v3](https://github.com/NomicFoundation/hardhat/releases/tag/%40nomicfoundation%2Fhardhat-ethers%403.0.0): Ethers.js v6 support

- Ethers-rs [v2.0.6](https://github.com/gakonst/ethers-rs/releases/tag/ethers-v2.0.6): support Optimism deposited transactions

- [GuardianTest](https://github.com/GuardianUI/GuardianTest/#readme): end to end testing, uses Playwright, injects a wallet connected to Anvil network fork

- [Armchair](https://github.com/m1guelpf/armchair#readme) (app starter kit): Next.js app router & server actions, Sign in with Ethereum

- CTFs:
    - Curta CTF [Labyrinth solution](https://twitter.com/0xkaden/status/1664026474813489153)
    
    - Secureum RACE #18: [8 question Solidity quiz & answers](https://ventral.digital/posts/2023/5/29/race-18-of-the-secureum-bootcamp-epoch-infinity)
    
    - [GPT-4 plays Ethernaut](https://blog.openzeppelin.com/chatgpt-4-vs-ethernaut-using-ai-to-hack-solidity-smart-contracts): 19/23 for older levels in the training data, 1/5 for new levels

**Security**

- Jimbo v2 (semi-stablecoin) [$7.5 million exploit](https://rekt.news/jimbo-rekt/) on Arbitrum via lack of slippage control

- El Dorado Exchange (EDE) [$680k exploit](https://lunaray.medium.com/analysis-of-the-ede-finance-attack-event-8edb5d5cfc50) on Arbitrum via oracle manipulation

- unshETH [$375k taken](https://twitter.com/unshethintern/status/1664386251162783745) after deployer private key shared on GitHub

- [Open Standard Web3 Attack Reference](https://oswar.org/) (OSWAR): framework to identify, categorize & mitigate attacks & vulnerabilities

**Ecosystem**

- [Lido is over 36% of staked ETH](https://www.reddit.com/r/ethfinance/comments/13wcu4w/comment/jmbhv0z/)
    - Reminder: [don’t allocate capital to LSDs exceeding 25% of staked ETH](https://github.com/djrtwo/writing/blob/main/docs/2022-05-30_the-risks-of-lsd.md)

- Ethereum Protocol Fellowship [cohort four applications](https://blog.ethereum.org/2023/06/01/ethereum-protocol-fellowship-fourth-apps-open) are open

- [Etherscan adds advanced filters](https://twitter.com/etherscan/status/1664589458652667906) for transaction searches, beta

- ETHDublin [hackathon projects](https://twitter.com/EthIreland/status/1663860034487349250)

**Notable at app layer**

- [Circle launching native USDC on Arbitrum](https://arbitrumfoundation.medium.com/usdc-to-come-natively-to-arbitrum-f751a30e3d83) on June 8, bridged token renamed to USDC.e

- Curve [Tricrypto-ng](https://twitter.com/CurveFinance/status/1663673455215013893) (next generation of pools) deployed, swap gas costs halved

* * *

### Job Listings

- Devconnect Istanbul: [Production Assistant](https://jobs.lever.co/ethereumfoundation/db6e2775-39d3-4eb9-9313-dfb15dfab9bc) and [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/401e0af5-f4a2-4e66-a724-4accb003113e)

- [Protocol Engineer](https://github.com/tvl-labs/job-board/blob/main/engineering/protocol_engineer.md) (DeFi) sought by [Tunnel Vision Labs](https://tunnelvisionlabs.xyz/)

- Solidity team need a highly skilled [Developer Advocate](https://jobs.lever.co/ethereumfoundation/b9e33c9e-48ee-464f-a672-d51eece2b99d)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US SEC settled with former Coinbase staffer](https://www.sec.gov/news/press-release/2023-98) on insider trading charges to [avoid having to prove that any of the tokens were securities](https://twitter.com/RSSH273/status/1663582576983040000)

**General/crypto**

- [Blockchain censorship](https://arxiv.org/abs/2305.18545): effect of OFAC sanctions on Ethereum & Bitcoin

- [iMessage](https://securelist.com/operation-triangulation/109842/) zero-click exploit

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-june-3-2023](https://weekinethereumnews.com/week-in-ethereum-news-june-3-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jun 9-11 – [ETHPrague](https://ethprague.com/) conference & hackathon

- **Jun 16 –** [**Ethereum Protocol Fellowship cohort four**](https://blog.ethereum.org/2023/06/01/ethereum-protocol-fellowship-fourth-apps-open) **application deadline**

- Jun 22–25 – [Pragma Waterloo](https://ethglobal.com/events/pragma-waterloo) & [ETHGlobal Waterloo](https://ethglobal.com/events/waterloo2023) hackathon

- Jul 5-9 – [ETHBarcelona](https://ethbarcelona.com/) conference & hackathon

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Aug 15-16 – [ETHToronto](https://www.ethtoronto.ca/) & [ETHWomen](https://www.ethwomen.com/)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org/) (Buenos Aires)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 30 – Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 18-21 – [ETH Montréal](https://ethmontreal.xyz/) hackathon & conference

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 6–27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 27–29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://twitter.com/ethbrno/status/1652198745902137344)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 17-19 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

---
title: "Week in Ethereum News <br> March 25, 2023"
date: "2023-03-25"
---

## **Eth News and Links**

**Shapella (Shanghai + Capella) upgrade**

- Update your nodes ready for [mainnet Shapella upgrade on April 12](https://github.com/ethereum/execution-specs/blob/master/network-upgrades/mainnet-upgrades/shanghai.md#upgrade-schedule), ensure to update both your beacon node & validator client

- Consensus layer mainnet releases:
    - Lighthouse [v4.0.1-rc.0](https://github.com/sigp/lighthouse/releases/tag/v4.0.1-rc.0) (hotfix for v4.0.0)
    
    - Lodestar [expected next week](https://github.com/ChainSafe/lodestar/releases)
    
    - Nimbus [v23.3.2](https://github.com/status-im/nimbus-eth2/releases/tag/v23.3.2)
    
    - Prysm [expected next week](https://github.com/prysmaticlabs/prysm/releases)
    
    - Teku [v23.3.1](https://github.com/ConsenSys/teku/releases/tag/23.3.1)

- Execution layer mainnet releases:
    - Besu [v23.1.2](https://github.com/hyperledger/besu/releases/tag/23.1.2)
    
    - Erigon [expected next week](https://github.com/ledgerwatch/erigon/releases)
    
    - Geth [v1.11.5](https://github.com/ethereum/go-ethereum/releases/tag/v1.11.5)
    
    - Nethermind [v1.17.3](https://github.com/NethermindEth/nethermind/releases/tag/1.17.3)

- Consensus specs [v1.3.0-rc.5](https://github.com/ethereum/consensus-specs/releases/tag/v1.3.0-rc.5): sets Capella upgrade epoch

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=Xc6Ss-m_nlE&t=488s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/HkfYv0tgn) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-consensus-call-105/):
    - [bug bounty doubled for Shapella specific issues](https://ethereum.org/en/bug-bounty/) up to $500k, until April 5
    
    - final Shapella mainnet shadow fork planned once all client releases are out
    
    - Deneb discussions: add proofs to blobs bundle in Engine API, KZG library startup times for testing and SSZ scope
    
    - [post-Deneb upgrade naming](https://ethereum-magicians.org/t/e-star-name-for-consensus-layer-upgrade-after-deneb/13248) & using a merged name (CL star + EL city)

**Dencun (Cancun + Deneb) upgrade**

- Latest EIP4844 implementers [call video](https://www.youtube.com/watch?v=gdy5svsnFrM&t=4s). Notes from [Terence](https://twitter.com/terencechain/status/1637913237198082048): split EIP4844 SSZ effort from SSZ overhaul and fee market discussions but no immediate changes

- [KZG Ceremony](https://twitter.com/trent_vanepps/status/1637559648076087296): 83k+ contributors from first general contribution period (now closed)

**Layer 1**

- [EOF mega spec](https://notes.ethereum.org/@ipsilon/B1nnZ1fl3): merged from v1.1 & v2 discussions

- [692 ETH proposer payment](https://twitter.com/bertcmiller/status/1637768534016024576), MEV bot lost $1 million

**Client releases**

- Consensus layer:
    - Lodestar [v1.6.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.6.0): client monitoring using remote services, fixes for issues preventing Rocket Pool & Dappnode integration

**Research**

- RIG Open Problem: [monitor supply chain health](https://efdn.notion.site/ROP-5-Ethereum-Supply-Network-Health-Framework-66b81aa8b486496aa3b95cb5b619137b)
    - [Inclusion time delay](https://ethresear.ch/t/estimating-inclusion-delays-for-censored-transactions/15115) for censored transactions is median of 11 seconds

- [Origami verifiable delay function](https://eprint.iacr.org/2023/384): folding Plonk proofs

**For Stakers**

- [Lodestar $20k incentive program](https://blog.chainsafe.io/introducing-the-lodestar-user-incentive-program-bbaeaa3246eb) to try their client & propose a block

**Layer 2**

- zkSync Era (zkEVM) [mainnet alpha](https://blog.matter-labs.io/gm-zkevm-171b12a26b36) open to all, native account abstraction, publishes state diffs rather than transaction inputs, initially with a [24 hour execution delay](https://blog.matter-labs.io/securing-zksync-era-execution-delay-ee32b11d6f9)

- Taiko (zkEVM) [alpha-2 testnet](https://mirror.xyz/labs.taiko.eth/A6G6TNN-CXDAhl42k_bNHg_20fyGcT0xH-LBBSOPNzU): uses Sepolia testnet

- [Immutable zkEVM](https://www.immutable.com/blog/immutable-and-polygon) announced, using Polygon zkEVM, gas to be paid in $IMX

- Optimism [two step withdrawals](https://dev.optimism.io/two-step-withdrawals/) in Bedrock upgrade, improves bridge security

- [ARB token reverse-bridging](https://twitter.com/DZack23/status/1639354219206434829): layer 2 token can be bridged to mainnet

**EIPs/Standards**

- EIPs:
    - [EIP6733](https://github.com/ethereum/EIPs/pull/6733/files): Revert creation in case of collision

- ERCs:
    - [ERC6732](https://github.com/ethereum/EIPs/pull/6732/files): Redeemable tokens
    
    - [ERC6734](https://github.com/ethereum/EIPs/pull/6734/files): L2 token list
    
    - [ERC6735](https://github.com/ethereum/EIPs/pull/6735/files): L2 aliasing of EVM-based addresses
    
    - [ERC6774](https://github.com/ethereum/EIPs/pull/6774/files): Non-sellable tokens

**Stuff for developers**

- [Update NFT metadata on OpenSea](https://twitter.com/nnnnicholas/status/1637960142284115970) using ERC4906 events & ERC1155 uri event

- [Re-export interfaces & types](https://twitter.com/paulrberg/status/1638643601650651136) so users don’t need to install additional dependencies

- [Reentrancy guard proxy](https://medium.com/spherex-technologies/reentrancy-guard-2-0-cbbc0be41634): prevents reentrant external calls & read only reentrancy

- Intro to [gas optimization](https://medium.com/@ayomilk1/maximizing-efficiency-how-gas-optimization-can-streamline-your-smart-contracts-4bafcc6bf321)

- [Foundry x Fe](https://github.com/cburgdorf/Foundry-Fe#readme): template to compile & test Fe contracts

- Slither [v0.9.3](https://github.com/crytic/slither/releases/tag/0.9.3): adds detector for high complexity functions

- Curta CTF TinySig challenge [solution](https://twitter.com/rileyholterhus/status/1637905710095933441)

- [slither-docs-action](https://github.com/crytic/slither-docs-action#readme): GitHub Action to generate documentation for Solidity pull requests

- [Symbolic execution tools](https://hackmd.io/@SaferMaker/EVM-Sym-Exec): comparison of Mythril, Manticore, hevm & EthBMC

- noble secp256k1 & noble ed25519 [v2](https://twitter.com/paulmillr/status/1639217783727697920): single feature modules in 4KB gzipped

- Semaphore [v3.4.0](https://github.com/semaphore-protocol/semaphore/releases/tag/v3.4.0): HeyAuthn library to create & manage identities

- [Circomspect v0.8.0](https://blog.trailofbits.com/2023/03/21/circomspect-static-analyzer-circom-more-passes/) (static analyzer for Circom): added five new analysis passes

**Security**

- Cloudflare users: [rotate Global API key for all accounts](https://twitter.com/tayvano_/status/1639029010687721474)

- [Transaction simulation vulnerabilities](https://zengo.com/zengo-uncovers-security-vulnerabilities-in-popular-web3-transaction-simulation-solutions-the-red-pill-attack/) disclosed using basefee, coinbase & gasprice variables

- Tincho’s [audit process](https://mirror.xyz/patrickalphac.eth/KSls5PVxzzvrtcR9dxNguXqgyUh7T3V74dBPt77m8Zk)

**Ecosystem**

- At least [636k ETH supply lost/frozen so far](https://twitter.com/jconorgrogan/status/1637944295746412549): Parity wallet bug, contract bugs, burnt, typos & trapped in WETH

**Enterprise**

- [Coinbase Wallet as a Service](https://twitter.com/yugacohler/status/1638559696230440962) public preview on testnet

- [Xapo Bank integrated USDC](https://www.xapobank.com/blog/xapo-bank-is-the-first-bank-to-fully-integrate-with-usdc), send & receive USDC from USD accounts, non-US only

**Notable at app layer**

- [ERC4361 (Sign In with Ethereum) integrated with MetaMask](https://blog.spruceid.com/spruce-integrates-sign-in-with-ethereum-into-metamask-for-better-user-experience-and-safety/): sign in request display & domain binding

- [Maker DAO voted to maintain USDC](https://vote.makerdao.com/polling/QmQ1fYm3#poll-detail) as primary reserve

- [Uniswap mini portfolio](https://twitter.com/Uniswap/status/1638579346351824911): view tokens, NFTs & LP pools

- [SpankPay](https://twitter.com/SpankPay/status/1637895544373739520) closing down due to no willing fiat rails

* * *

### Job Listings

- L2BEAT 💗 is hiring a Senior Software Engineer & Product Owner. [Apply here!](https://l2beat.notion.site/We-are-hiring-Work-at-L2BEAT-e4e637265ae94c5db7dfa2de336b940f)

- [Nimbus](https://nimbus.team/#about) is hiring a [Site Reliability Engineer](https://jobs.status.im/?gh_jid=4797968)

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US SEC:
    - [Coinbase received Wells notice](https://www.coinbase.com//blog/we-asked-the-sec-for-reasonable-crypto-rules-for-americans-we-got-legal) for potential violations of securities law but SEC declines to specify which assets are securities
    
    - Paradigm: [“just come in and register” is a fabrication](https://policy.paradigm.xyz/writing/secs-path-to-registration-part-i)
    
    - [SushiSwap & Head Chef served](https://forum.sushi.com/t/establish-sushi-legal-defense-fund/11813) with subpoena
    
    - [Justin Sun charged](https://www.sec.gov/news/press-release/2023-59) with unregistered sale of securities and 8 celebrities charged for promotion without disclosing payment

- Whitehouse [2023 economic report](https://www.whitehouse.gov/wp-content/uploads/2023/03/ERP-2023.pdf) \[PDF\]: “crypto assets currently do not offer widespread economic benefits”

- [Do Kwon arrested](https://www.coindesk.com/business/2023/03/23/do-kwon-arrested-in-montenegro-interior-minister/) in Montenegro

- [IRS proposed NFT guidance](https://www.irs.gov/pub/irs-drop/n-23-27.pdf) \[PDF\] on treatment of certain NFTs as collectibles, feedback requested

**General/crypto**

- [Ronin exploiter apparently tried to trick the Euler exploiter](https://twitter.com/hudsonjameson/status/1638240083496038409) into using a vulnerable library

- [aCropalypse](https://www.da.vidbuchanan.co.uk/blog/exploiting-acropalypse.html): cropped/redacted images from Google Pixel’s screenshot editor can be partially recovered

- [Goblin Plonk](https://hackmd.io/@aztec-network/BkGNaHUJn/%2FGfNR5SE5ShyXXmLxNCsg3g): lazy recursive proof composition

- [cqlin](https://eprint.iacr.org/2023/393): efficient linear operations on KZG commitments with cached quotients

- [Proactive refresh](https://github.com/lyronctk/proactive-refresh#readme) (every 30 seconds) for BLS threshold signatures

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-march-25-2023](https://weekinethereumnews.com/week-in-ethereum-news-march-25-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Mar 27-30 – [Ethereum Rio](https://www.ethereumbrasil.com/ethereumrio)

- Mar 31 - Apr 2 – [ETHSamba](https://www.ethsamba.org/) (Rio) hackathon & conference

- Mar 31 – deadline for [EF account abstraction grants round](https://esp.ethereum.foundation/account-abstraction-grants)

- Apr 5-8 – [ETH Beijing](https://www.ethbeijing.xyz/) hackathon

- Apr 12 – [Mainnet upgrades to Shapella](https://github.com/ethereum/execution-specs/blob/master/network-upgrades/mainnet-upgrades/shanghai.md#upgrade-schedule)

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- Apr 13-16 – [Pragma Tokyo](https://ethglobal.com/events/pragma-tokyo) & [ETHGlobal Tokyo](https://tokyo.ethglobal.com/) hackathon

- Apr 14-16 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference & hackathon

- Apr 21-25 – [EthTaipei](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) hackathon & conference

- Apr 27-30 – [Istanbul ETH Privacy](https://www.leadingprivacy.com/istanbul) conference & hackathon

- Apr 28 – deadline for EF’s [Next Billion fellowship cohort 3](https://blog.ethereum.org/2023/03/16/fellowship-cohort-3-applications)

- May 5-10 – [ETHTallinn](https://ethtallinn.org/) hackathon & [NFT Tallinn](https://nfttallinn.com/) conference

- May 9-12 – [EY blockchain summit](https://web.cvent.com/event/c066d44d-4e50-4d7e-b6fb-3cc0abdae7ff/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7)

- May 12-14 – [ETHGlobal Lisbon](https://ethglobal.com/events/lisbon)

- May 19-23 – [EDCON](https://edcon.io/) Montenegro (changed from Vienna)

- May 20-21 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 24-26 – [Spaghett ETH](https://naples.spaghett-eth.com/) (Naples) conference

- May 26-28 – [ETHDublin](https://www.ethdublin.io/) hackathon

- Jun 2-4 – [ETH Seoul](https://2023.ethseoul.org/)

- Jun 2-6 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 9-11 – [ETHPrague](https://ethprague.com/) conference & hackathon

- Jun 23–25 – [ETHGlobal Waterloo](https://ethglobal.com/events/waterloo2023) (changed from Toronto)

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Aug 16-19 – [Ethereum Argentina](https://twitter.com/EtherArgentina/status/1625857633260552200) (Buenos Aires)

- Aug 30 - Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–25 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 28–30 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

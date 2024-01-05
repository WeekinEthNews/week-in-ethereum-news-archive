---
title: "Week in Ethereum News <br> October 28, 2023"
date: "2023-10-27"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=P_a3s6zNFEk&t=282s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1717540482270818497) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-173/):
    - **Mainnet**: upgrade likely to be 2024 (minimum 2 week gap between each testnet upgrade)
    
    - **Goerli testnet**: upgrade late November (at the earliest), CL clients not ready yet
    
    - **Devnet 10**: [normal](https://notes.ethereum.org/@ethpandaops/dencun-devnet-10-analysis) & [stress](https://notes.ethereum.org/@ethpandaops/devnet-10-stress-analsysis) testing analysis, tested EIP7514 (max churn limit)
    
    - [**Devnet 11**](https://notes.ethereum.org/@ethpandaops/dencun-devnet-11): launch early next week, test all clients with MEV pipeline
    
    - **Goerli shadow fork**: launch early next week
    
    - Discussed [EIP7523](https://eips.ethereum.org/EIPS/eip-7523) (empty accounts deprecation) 

- [Proposed Deneb simplification](https://github.com/ethereum/consensus-specs/pull/3531) to attach the block header & an inclusion proof on each blob sidecar

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.51%**](https://dune.com/hildobby/eth2-staking) **has reduced again but still far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~84% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm at 45%, any client bug over 33.3% could mean loss of finality

- [Geographic diversity needed for stakers & nodes](https://nodewatch.io/), particularly outside of US/Canada/EU

**Layer 1**

- Verkle [Kaustinen testnet](https://twitter.com/gballet/status/1716743548442132895) back online, upgraded to Shapella, proof witnesses include post state and adds Lodestar CL client

**Client releases**

- Consensus layer:
    - Prysm [v4.1.1](https://github.com/prysmaticlabs/prysm/releases/tag/v4.1.1): patch to fix using REST API with external builder and experimental state deadlock

- Execution layer:
    - Besu [v23.10.1](https://github.com/hyperledger/besu/releases/tag/23.10.1): UX, memory and RPC performance improvements
    
    - Erigon [v2.53.2](https://github.com/ledgerwatch/erigon/releases/tag/v2.53.2): fixes
    
    - Nethermind [v1.21.1](https://github.com/NethermindEth/nethermind/releases/tag/1.21.1): hotfix for invalid block production

**Research**

- [SubnetDAS](https://ethresear.ch/t/subnetdas-an-intermediate-das-approach/17169): proposal for intermediate DAS approach with linkability of queries tradeoff

- Family of [embedded curves for BLS](https://eprint.iacr.org/2023/1662)

**Layer 2**

- First monthly RollCall (Layer 2 protocol & EVM standardization) [call video](https://www.youtube.com/watch?v=aPvMoVI6rFE):
    - intros, Rollup Improvement Proposals (RIPs), EIP7212 (secp256r1 precompile) as first RIP, Devconnect discussion topics and EIP7530 (EVM profiles)

**EIPs/Standards**

- [ERCs split](https://twitter.com/lightclients/status/1717295084532551881) from EIPs

- EIPs
    - [EIP7542](https://eips.ethereum.org/EIPS/eip-7542): eth/69 - available-blocks-extended protocol
    
    - [EIP7543](https://github.com/ethereum/EIPs/pull/7904/files): EVM decimal math (opcodes)
    
    - [EIP7545](https://github.com/ethereum/EIPs/pull/7926/files): Verkle proof verification precompile

- ERCs (application layer):
    - (Informational) [ERC7544](https://github.com/ethereum/EIPs/pull/7915/files): Security flaws in ERC20 transfer patterns (tokens sent to contracts can be lost)
    
    - [ERC7546](https://github.com/ethereum/ERCs/pull/39/files): Upgradeable clone (proxy pattern)

**Stuff for developers**

- Solidity [v0.8.22](https://soliditylang.org/blog/2023/10/25/solidity-0.8.22-release-announcement):
    - Adds unchecked loop increments, Yul optimizer rematerializes zero literals, experimental support to import EVM Assembly JSON and event definition at file level
    
    - EVM versions before Constantinople deprecated

- Hardhat:
    - [Ignition](https://medium.com/nomic-foundation-blog/introducing-hardhat-ignition-a-refreshed-deployments-experience-9580d2946e10): declarative contract deployment with support for recovery
    
    - [Hardhat-verify v2](https://github.com/NomicFoundation/hardhat/releases/tag/%40nomicfoundation/hardhat-verify%402.0.0): adds Sourcify verification, enable via config

- OpenSea [Shipyard](https://github.com/ProjectOpenSea/shipyard-core#readme): NFT libraries & implementations

- Fe (language) [v0.25.0](https://github.com/ethereum/fe/releases/tag/v0.25.0): fe test adds print logs and filter to only run specific tests 

- [evm.storage](https://blog.smlxl.io/announcing-bytecode-generated-storage-layouts-on-evm-storage-96761758d397): supports unverified contracts using bytecode-generated layouts

- [EVM Glue](https://github.com/Philogy/evm-glue#readme): EVM assembler in Rust

- [Uniswap universal router decoder & encoder](https://github.com/Elnaril/uniswap-universal-router-decoder#readme) in Python

- [halo2-repl](https://blog.axiom.xyz/halo2-repl/): write zk circuits using JavaScript in browser-based REPL for Halo 2

**Security**

- Maestro [280 ETH exploit](https://twitter.com/ProdigalWiz/status/1717002922246950925) via arbitrary call, users refunded

- Aztec Connect [vulnerability postmortem](https://hackmd.io/@aztec-network/claim-proof-bug), $450k bounty paid, withdraw funds from zk.money

- UniPass account abstraction (ERC4337) module [vulnerability disclosed](https://www.fireblocks.com/blog/fireblocks-researchers-uncover-first-account-abstraction-wallet-vulnerability/)

- [SEAL drills](https://twitter.com/samczsun/status/1717243519243636755): protocol incident response testing via simulated attack, drills run with Compound & Yearn

**Ecosystem**

- [Etherscan](https://twitter.com/etherscan/status/1717516814933217326) account abstraction (ERC4337) transaction display

- ETH Hong Kong [hackathon winners](https://build.bewater.xyz/en/campaigns/mUwy-2023ETH-HongKong-Hackathon/result)

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 5.3 to 97.5 gwei, with 18.8 gwei average
    - Zero net issuance currently at 21.6 gwei 
    
    - 2.1k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $1,595 - $1,845, currently $1,777

- [ETHBTC](https://ratiogang.com/): currently 0.053 (Flippening at ~0.16)

**Notable at app layer**

- Call for [open bridge standards](https://twitter.com/connextnetwork/status/1717953446475620379)

- Polygon [POL token](https://polygon.technology/blog/polygon-2-0-milestone-pol-contracts-are-live-on-ethereum-mainnet) live on mainnet

- Gitcoin [direct grants](https://www.gitcoin.co/blog/intro-to-direct-grants-how-do-they-work): award funds to projects/individuals for deliverables

- Karma [grantee accountability protocol](https://twitter.com/karmahq_/status/1717530274593161640) for public goods projects; \[[Starbloom](https://twitter.com/starbloomvent) portfolio\]

- Hats [modules](https://hats.mirror.xyz/xAk_yb7dDL1OLBx8nq47Ni7V1SuiC6L6B-49u7vz520): automatic granting/revocation of roles based on conditions

- [Slugs](https://s.box/) (onchain URL shortener) live on Optimism

* * *

### Job Listings

- eBay Web3 team seeking [Lead Solidity Engineer](https://jobs.ebayinc.com/us/en/job/R0060412/Lead-Solidity-Engineer)

- Gnosis seek a [VP Technology](https://gnosis.jobs.personio.com/job/1267892?_pc=1517287), [Senior Web Devs (Wallet)](https://gnosis.jobs.personio.com/job/1239306?_pc=1517287&display=en) & [Backend Devs](https://gnosis.jobs.personio.com/job/1284509?_pc=1517287)

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

- [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db) wanted by EF

**Job listings: $600 for four issues** (75 character limit).  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Elliptic: [correcting WSJ](https://www.elliptic.co/blog/setting-the-record-straight-on-crypto-crowdfunding-by-hamas), no evidence Hamas received significant volumes of crypto donations

- SEC Commissioner Peirce: [dissent on LBRY](https://www.sec.gov/news/statement/peirce-statement-lbry-102723), SEC’s misguided enforcement-driven approach to crypto

- [BlockFi](https://blockfi.com/blockfi-emerges-from-bankruptcy/) emerged from bankruptcy

- [Yuga Labs vs Ryder Ripps trademark lawsuit](https://twitter.com/NeerMcD/status/1717634980002582902): Yuga awarded $1.5M & RR/BAYC NFT contract

- Proposal for [Internet Native Company](https://inc.mirror.xyz/5w00mPQzwba24mVZu1mm53VTDTCsISFADu2JCgM2EGs) (INC): for-profit org operated & governed onchain

**General**

- [Okta support system breached](https://sec.okta.com/harfiles), detected by customers [BeyondTrust](https://www.beyondtrust.com/blog/entry/okta-support-unit-breach), [Cloudflare](https://blog.cloudflare.com/how-cloudflare-mitigated-yet-another-okta-compromise/) & [1Password](https://blog.1password.com/okta-incident/)

- [iLeakage](https://ileakage.com/): transient execution side channel targeting Safari browser

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-october-28-2023](https://weekinethereumnews.com/week-in-ethereum-news-october-28-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) deadline (max $1k for local meetups)

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul), [**travel advisory**](https://blog.ethereum.org/2023/10/23/devconnect-ist-advisory-update)

- Nov 15-29 – [Gitcoin Grants 19](https://twitter.com/gitcoin/status/1715026016924737800)

- Nov 16-19 – [Pragma](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Nov 18 – [Ethereum Costa Rica](https://www.meetup.com/ethereumcr/events/295894129/)

- **Dec 4** – [ETHVenice](https://ethvenice.com/)

- Dec 6-7 – [Columbia CryptoEconomics workshop](http://columbiacryptoeconomics.org/) (New York)

- Dec 8-10 – ETHGlobal [ETHIndia](https://ethindia.co/) (Bangalore) 

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

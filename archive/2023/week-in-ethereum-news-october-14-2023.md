---
title: "Week in Ethereum News <br> October 14, 2023"
date: "2023-10-13"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=t25IIQWfCnY&t=167s). Recap by [Tim Beiko](https://mirror.xyz/abcoathup.eth/eU0ggEdbNvIiOT0xMoqVbk2Ow0KBU5Qw04Hw6PruRBo).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1712534201042612514) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-172/):
    - Devnet 9 testing continues, MEV-Boost testing started (need to test with blobs)
    
    - Devnet 10 ideally launches next week, once KZG setup in CL specs/clients and devnet 9 testing complete
    
    - [EVM Object Format (EOF) status update](https://docs.google.com/presentation/d/10mxZK5hzLeaTLGAVo83qrPybk0Y8fUN5prAffGhKV6o/edit#slide=id.p)
    
    - Discussions on priorities/timeline for EOF & Verkle, whether to ever include EOF and L1/L2 EVM divergence

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.89%**](https://dune.com/hildobby/eth2-staking) **has reduced again but still far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)
    - [Arbitrum delegates](https://thedefiant.io/lido-misses-out-as-arbitrum-grants-vote-closes) voted against incentives for Lido

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~84% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm at 45%, any client bug over 33.3% could mean loss of finality
        - [Blockprint](https://blog.sigmaprime.io/blockprint-ui.html) (CL client diversity analysis) updated to include accuracy data

- [Geographic diversity needed for stakers & nodes](https://nodewatch.io/), particularly outside of US/Can/EU

**Layer 1**

- Péter Szilágyi (Geth): proposal for [eth/69](https://gist.github.com/karalabe/28aab3a5296d80cf7616a8b8b859131b) to improve transaction propagation, no hard fork required

- Proposal for [time restricted transaction execution](https://ethresear.ch/t/time-restricted-transaction-execution/17024), add a minStartTime field to transactions

- [Verkle Tree cryptography](https://github.com/jsign/verkle-crypto#readme) implemented in Zig

**For Stakers**

- Beacon chain [churn limit increased to 13](https://twitter.com/irina_everstake/status/1711645101812809940) per epoch (Dencun EIP7514 reduces to 8 for deposits)

- [~9k solo stakers](https://mirror.xyz/0xf3bF9DDbA413825E5DdF92D15b09C2AbD8d190dd/CzCNFznCveDlKnlVaSU5-MzUtbn9gW0KlgPe5FVrQME): estimate based on deposit addresses interacting with smart contracts

**Client releases**

- Consensus layer:
    - Teku [v23.10.0](https://github.com/Consensys/teku/releases/tag/23.10.0): attestation duty calculation performance improvements

- Execution layer:
    - Besu [v23.10.0](https://github.com/hyperledger/besu/releases/tag/23.10.0): Layered transaction pool now default
    
    - Erigon [v2.52.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.52.0): fixes
        - Otterscan [v2.1.0 alpha](https://github.com/otterscan/otterscan/releases/tag/v2.1.0): adds indexer for withdrawals per address
    
    - Geth [v1.13.3](https://github.com/ethereum/go-ethereum/releases/tag/v1.13.3): updates Pebble to fix occasional IO/CPU runaway

**Research**

- Vitalik’s [proposed staking design changes](https://notes.ethereum.org/@vbuterin/staking_2023_10) to give delegators power to choose nodes & participate in consensus, improving decentralization & reducing consensus overhead

- [Minimum viable issuance](https://notes.ethereum.org/@anderselowsson/MinimumViableIssuance) (only issue ETH that is strictly needed for security): benefits & drawbacks

- [PEPC-Boost](https://hackmd.io/@bchain/BJkarrEWp): out of protocol relay design which auctions top-of-block & rest-of-block separately

- [Commitment-Satisfaction Committees](https://ethresear.ch/t/commitment-satisfaction-committees-an-in-protocol-solution-to-pepc/17055): leverage attesters to enforce commitments for PEPC

- Proposal for optional [validator identification metadata](https://ethresear.ch/t/how-optional-non-kyc-validator-metadata-can-improve-staking-decentralization/17032)

**Layer 2**

- L2BEAT [Build Your Own Rollup](https://medium.com/l2beat/build-your-own-rollup-72423f4255e7): simplified sovereign rollup for education purposes

**EIPs/Standards**

- EIPs
    - (Informational) [EIP7532](https://github.com/ethereum/EIPs/pull/7827/files): Generation unit (64 epochs)
    
    - [EIP7534](https://github.com/ethereum/EIPs/pull/7837/files): Theorem-carrying-transaction

- ERCs (application layer):
    - [ERC7533](https://github.com/ethereum/EIPs/pull/7833/files): Public cross port (connect EVM networks)
    
    - [ERC7535](https://github.com/ethereum/EIPs/pull/7846/files): ETH (native asset) tokenized vault (ERC4626)

* * *

### **Optimism’s** [**RetroPGF Round 3 applications**](https://optimism.mirror.xyz/wiHMKqsbAQnK51Se3MraSnvf0blwRzS9jguojEmKKVc) **are open**

![Optimism RetroPGF Round 3 applications](https://weekinethereumnews.com/wp-content/uploads/2023/10/Optimism-RetroPGF3-applications-1024x512.png)

Applications for Optimism’s RetroPGF Round 3 are open!

In this round 30 million OP will be allocated to the builders, artists, creators, and educators who have demonstrated their impact in building the Optimism Collective.

[Apply now](https://app.optimism.io/retropgf-signup), applications close October 23

* * *

**Stuff for developers**

- [Hardhat-viem](https://medium.com/nomic-foundation-blog/hardhat-viem-808a536dcfe6) (plugin): use Viem library in new & existing Hardhat projects

- Foundry [test summary](https://twitter.com/0xasp_/status/1711366727895048327): use summary flag for concise table of test results

- [P256Verifier](https://daimo.xyz/blog/p256verifier): Solidity contract for P256 signature verification, deployed on mainnet

- Vyper:
    - titanoboa [v0.1.8](https://twitter.com/big_tech_sux/status/1712612490419245157) (Vyper interpreter): adds Vyper v0.3.10 support, network mode to deploy contracts, jupyter integration and coverage
    
    - Snekmate [v0.0.3](https://github.com/pcaversaccio/snekmate/releases/tag/v0.0.3) (Vyper contracts): updated to Vyper v0.3.10, adds ERC2981 (NFT royalties)

- Huff:
    - [Huff playground](https://oguimbal.github.io/huff/): Huff equivalent of evm.codes
    
    - [Tstore huff template](https://github.com/AmadiMichael/tstore-huff-template#readme): use tload & tstore opcodes (in Dencun upgrade) via verbatim helper

- Ethers.js [v6.8.0](https://github.com/ethers-io/ethers.js/releases/tag/v6.8.0): updated to latest noble crypto libraries

- Alchemy [account kit](https://alchemy.com/blog/introducing-account-kit): toolkit for ERC4337 account abstraction

- Swiss Knife [send tx](https://transact.swiss-knife.xyz/send-tx): UI to deploy contract bytecode

- [Call this](https://github.com/shazow/callthis#readme): transaction builder UI with shareable link, uses WhatsABI

- [ZK Hunt](https://0xparc.org/blog/zk-hunt): RTS-like onchain PvP game built using MUD and circom

**Security**

- Wise Lending [exploit](https://twitter.com/blocksecteam/status/1712871304993689709) front run by MEV searcher c0ffeebabe

- [Threshold tBTC vulnerabilities disclosed](https://blog.threshold.network/a-tale-of-two-bugs/), DoS vector and redemption mechanism design flaw

**Ecosystem**

- ETHRome [hackathon winners](https://twitter.com/ethrome/status/1711423469043216665)

**Enterprise**

- [BlackRock used tokenized money market fund](https://archive.is/QhVY4) as collateral in OTC derivatives trade on JPMorgan’s Onyx

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 4.3 to 47.7 gwei, with 7.4 gwei average
    - Negative issuance currently at 21.3 gwei 
    
    - 10.5k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $1,529 - $1,646, currently $1,549

- [ETHBTC](https://ratiogang.com/): currently 0.058 (Flippening at ~0.16)

**Notable at app layer**

- [Farcaster](https://twitter.com/dwr/status/1712185006037283031) (social network) now permissionless on Optimism
    - [Warpcast cryptoless signups](https://twitter.com/dwr/status/1712185006037283031) on iOS

* * *

### Job Listings

- eBay Web3 team seeking [Lead Solidity Engineer](https://jobs.ebayinc.com/us/en/job/R0060412/Lead-Solidity-Engineer)

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

- [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db) wanted by EF

- EF Privacy & Scaling Explorations team seek a [Technical Project Coordinator](https://jobs.lever.co/ethereumfoundation/c826b9a1-ede0-465e-9639-f34029304374)

- Aave seek a [UX Engineer](https://jobs.eu.lever.co/aave/2ce6fc26-729f-4cbf-a8f0-070321663262?lever-origin=applied&lever-source%5B%5D=WeekinEthereumNews) and a [Staff Rust Engineer](https://jobs.eu.lever.co/aave/46c3f25c-2c74-4b31-903e-bfbdfbd63d66?lever-origin=applied&lever-source%5B%5D=WeekinEthereumNews)

**Job listings: $600 for four issues** (75 character limit).  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [CFTC](https://www.cftc.gov/PressRoom/PressReleases/8805-23) and [FTC](https://www.ftc.gov/news-events/news/press-releases/2023/10/ftc-reaches-settlement-crypto-company-voyager-digital-charges-former-executive-falsely-claiming) charge former Voyager CEO Stephen Ehrlich

- [SEC not appealing](https://www.reuters.com/markets/us/us-sec-does-not-plan-appeal-court-decision-grayscale-bitcoin-etf-source-2023-10-13/) Grayscale ruling for spot Bitcoin ETF

**General**

- [Tornado Cash compliance tool users please help](https://twitter.com/CryptoCanal/status/1672208748192976897) the defense of Alex Pertsev in the Netherlands

- [HTX (formerly Huobi)](https://twitter.com/justinsuntron/status/1710687566792675553) stolen funds returned

- Contribute to Unirep (private & non-repudiable reputation system) [ceremony](https://ceremony.unirep.io)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-october-14-2023](https://weekinethereumnews.com/week-in-ethereum-news-october-14-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Oct 21 – [Ethereum México](https://twitter.com/ethereum_mexico/status/1684649652639924224)

- **Oct 23 – Optimism’s** [**RetroPGF Round 3 application**](https://app.optimism.io/retropgf-signup) **deadline**

- Oct 22-24 – [ETH Hong Kong](https://www.ethhongkong.co/)

- Oct 27-29 – [ETH London](https://www.encode.club/eth-london) hackathon

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Oct 28-30 – [Paradigm CTF](https://ctf.paradigm.xyz/)

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) deadline (max $1k for local meetups)

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 16-19 – [Pragma](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Nov 18 – [Ethereum Costa Rica](https://www.meetup.com/ethereumcr/events/295894129/)

- Dec 4-5 – [ETHVenice](https://ethvenice.com/)

- Dec 8-10 – ETHGlobal [ETHIndia](https://ethindia.co/) (Bangalore) 

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

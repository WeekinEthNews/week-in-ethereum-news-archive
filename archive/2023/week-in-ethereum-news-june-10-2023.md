---
title: "Week in Ethereum News <br> June 10, 2023"
date: "2023-06-10"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=LqaR-kdnOoU&t=195s). [Summary](https://twitter.com/abcoathup/status/1666931922436771842) & [notes](https://twitter.com/TimBeiko/status/1666905821723373568) from Tim Beiko:
    - Cancun upgrade scope finalized: adds bounded EIP4788 (beacon root in EVM) & tentatively EIP5656 (MCOPY) if implementation/testing not a bottleneck
    
    - Cancun will not include EIP2537 (BLS), EIP5920 (PAY) & EIP7069 (revamped CALL instructions)
    
    - EIP4844 blobs per block set to 3 & 6 (target & limit) for devnets, may change for mainnet
    
    - Devnet 6 for EIP4844 to be launched next week
    
    - [Holešky testnet](https://github.com/ethereum/pm/issues/803) (Goerli successor) first launch coordination call June 15, targeting September genesis (potentially too late for Dencun testing)

- Consensus-specs [v1.4.0-alpha.2](https://github.com/ethereum/consensus-specs/releases/tag/v1.4.0-alpha.2): increases MAX\_BLOBS\_PER\_BLOCK to 6 for EIP4844

**Layer 1**

- [Flood](https://github.com/paradigmxyz/flood/#readme): benchmarking RPC endpoints for the EVM

- Terence: [reducing Prysm validator's slot 0 propose time](https://hackmd.io/lWq6jEVhThy72CnAkpTvig) by precomputing the shuffling

**Client releases**

- Execution layer:
    - Erigon [v2.45.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.45.0): Caplin (embedded CL) bug fixes & DB layout changed for block bodies
    
    - Nethermind [v1.19.2](https://github.com/NethermindEth/nethermind/releases/tag/1.19.2): support for upcoming Teku v23.6

**For Stakers**

- [EL sync driver](https://github.com/tbenr/el-sync-driver#readme): sync a new EL client using an existing CL client, no CL config changes required

**Research**

- Proposal to [increase MAX\_EFFECTIVE\_BALANCE](https://ethresear.ch/t/increase-the-max-effective-balance-a-modest-proposal/15801), allows validator consolidation to lighten networking load

- [Verkle Tree proof generation & verification](https://hackmd.io/@jsign/vkt-proofs-implementation-notes) implementation optimization notes

**Layer 2**

- Optimism [Bedrock upgrade](https://twitter.com/optimismFND/status/1666850591669202965) live, gas fees over 40% lower via data compression and [ETH native representation](https://twitter.com/maurelian_/status/1667205092959830016)

- Arbitrum [batch-poster bug](https://twitter.com/ArbitrumDevs/status/1666549893001887744) caused a temporary pause in posting transactions onchain, no loss of service from a user perspective

- Arbitrum [time boost transaction ordering](https://arxiv.org/abs/2306.02179) economic analysis

**EIPs/Standards**

- ERCs:
    - [ERC7144](https://github.com/ethereum/EIPs/pull/7144/files): ERC20 with transaction validation step
    
    - [ERC7160](https://github.com/ethereum/EIPs/pull/7160/files): ERC721 multi-metadata extension

**Stuff for developers**

- Web3 interface libraries:
    - web3.js [v4](https://blog.chainsafe.io/announcing-the-full-release-of-web3-js-v4-e9e26275a3dc): rewritten in TypeScript, reduced build size, modular & extensible via plugins
    
    - viem [v1](https://twitter.com/wagmi_sh/status/1666189876910501888): includes opt-in batch JSON-RPC 

- [evm.storage](https://evm.storage/): view storage & state for verified contracts at a specific block, alpha version

- OpenZeppelin Contracts [v4.9.1](https://github.com/OpenZeppelin/openzeppelin-contracts/releases/tag/v4.9.1): fixes DoS vulnerability in Governor & GovernorCompatibilityBravo where proposal creation could be blocked by frontrunning

- Foundry:
    - Patrick Collins: [Solidity development course - Foundry edition](https://github.com/Cyfrin/foundry-full-course-f23#readme), 27 hours of video
    
    - Tip: [invoke commands with custom profiles](https://twitter.com/drakeevansv1/status/1666468515795140611)

- NatSpec [best practices](https://twitter.com/spearbitdao/status/1665800702122250241)

- abi-to-sol [v0.8.0](https://github.com/gnidan/abi-to-sol/releases/tag/v0.8.0): adds user-defined value types support

- [Titanoboa](https://twitter.com/big_tech_sux/status/1664856295474712579) (Vyper interpreter) adds node interaction allowing deployment

- snekmate [v0.0.2](https://github.com/pcaversaccio/snekmate/releases/tag/v0.0.2) (Vyper contracts): adds wad\_ln & wad\_exp and EIP5267 support

- [EVM diff](https://github.com/mds1/evm-diff#readme): diff execution-level specs of EVM-compatible chains

- Tenderly [precise gas estimates](https://blog.tenderly.co/how-tenderly-enables-most-accurate-ethereum-gas-estimation/) in a single run

- [Noble cryptography updated](https://twitter.com/paulmillr/status/1664984693790457858): npm provenance used for transparent builds and ed25519 & ed448 provide non-repudiation

- [Merklefy](https://github.com/martriay/merklefy#readme): web app to generate merkle trees from a csv

- [Create first zk contract](https://betterprogramming.pub/how-to-create-a-zk-smart-contract-cd948a673749) using Circom & Hardhat

**Ecosystem**

- EF [run a node grants](https://esp.ethereum.foundation/run-a-node-grants) to encourage diversification, receive a Dappnode or a grant for hardware

- Vitalik: [transitions](https://vitalik.eth.limo/general/2023/06/09/three_transitions.html) to rollups, contract wallets and privacy

- ETH Seoul hackathon [winners](https://ethseoul2023.devfolio.co/projects?show_winners=true)

- ETH Belgrade hackathon [winners](https://twitter.com/ethbelgrade/status/1667099119351914497) & [list of projects](https://taikai.network/ethbelgrade/hackathons/hackathon-2023/projects)

**Enterprise**

- Norwegian government tests putting their [central bank issued Krone on Arbitrum](https://medium.com/blockchangers/traditional-finance-meets-blockchain-92c74f0991e9)

**Notable at app layer**

- [Maker DAO deployed 500M DAI with Coinbase](https://twitter.com/MakerDAO/status/1665770361265459202) for 2.6% annual rewards

- [FLAIR](https://blog.uniswap.org/metric-evaluate-lp-competitiveness-amm) metric to measure intra-pool LP competitiveness in AMM

- [Forkable stablecoin design](https://ethresear.ch/t/forkable-stablecoin/15820) to manage contentious chain forks

- 0xSplits [Swapper](https://0xsplits.mirror.xyz/eZ1uAL3bIOd75LGcBXQEzOYE51wTHtCjNGsAD70rocg): received tokens swapped into an output token, stackable e.g. create tax wallet

- sudoswap [v2](https://blog.sudoswap.xyz/introducing-sudoswap-v2.html) (NFT marketplace): onchain royalties, creator settings, ERC1155 support, conditional orders and fee streaming

- [Usernames.club](https://launch.mirror.xyz/oyJ1CLHinWc-NqJ5QYpNGgzsbQO5M-813apMWQcZhO0): community namespaces for username NFTs, under usr.id, via Nouns auctions

- [Summa](https://github.com/summa-dev): zk proof of solvency for CEX, beta

* * *

### Job Listings

- Solidity team need a highly skilled [Developer Advocate](https://jobs.lever.co/ethereumfoundation/b9e33c9e-48ee-464f-a672-d51eece2b99d)

- Devconnect Istanbul: [Production Assistant](https://jobs.lever.co/ethereumfoundation/db6e2775-39d3-4eb9-9313-dfb15dfab9bc) and [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/401e0af5-f4a2-4e66-a724-4accb003113e)

- [Protocol Engineer](https://github.com/tvl-labs/job-board/blob/main/engineering/protocol_engineer.md) (DeFi) sought by [Tunnel Vision Labs](https://tunnelvisionlabs.xyz/)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US SEC regulation by enforcement:
    - [Coinbase](https://www.sec.gov/news/press-release/2023-102) charged for operating as unregistered securities exchange, broker & clearing agency and offer of securities for staking program
    
    - Coinbase issued [show cause order](https://cointelegraph.com/news/coinbase-targeted-by-state-security-regulators-concurrent-to-sec-lawsuit) from multiple state regulators for staking rewards
    
    - [Binance & CZ](https://www.sec.gov/news/press-release/2023-101) charged with securities violations and misleading investors over Binance US controls

- [CFTC won Ooki DAO case](https://twitter.com/z0r0zzz/status/1667272302294360064), members of unincorporated association may have to pay the fine

- [PoolTogether federal case dismissed](https://twitter.com/lay2000lbs/status/1666532463428943875) as plaintiff failed to show they suffered harm

- [ConsenSys forced to hold shareholder vote](https://www.coindesk.com/consensus-magazine/2023/06/08/consensys-faces-shareholder-vote-over-controversial-transfer-of-company-assets/) over intra-company transfer of MetaMask, Infura, etc

**General/crypto**

- Atomic wallet [$35 million stolen](https://www.bleepingcomputer.com/news/security/atomic-wallet-hacks-lead-to-over-35-million-in-crypto-stolen/)

- KeePass [v2.54](https://www.bleepingcomputer.com/news/security/keepass-v254-fixes-bug-that-leaked-cleartext-master-password/) fixes master password leak

- [SnarkJS](https://medium.com/@Beosin_com/beosin-security-researchers-discovered-snarkjs-library-vulnerability-cve-2023-33252-7e64f487c73c) library vulnerability

- [Hypernova implementation](https://github.com/privacy-scaling-explorations/multifolding-poc#readme), proof of concept

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-june-10-2023](https://weekinethereumnews.com/week-in-ethereum-news-june-10-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jun 16 – [Ethereum Protocol Fellowship cohort four](https://blog.ethereum.org/2023/06/01/ethereum-protocol-fellowship-fourth-apps-open) application deadline

- **Jun 20 – EF** [**run a node grant**](https://esp.ethereum.foundation/run-a-node-grants) **deadline**

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

- Sep 18-21 – [ETH Montréal](https://ethmontreal.xyz/) conference & hackathon

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

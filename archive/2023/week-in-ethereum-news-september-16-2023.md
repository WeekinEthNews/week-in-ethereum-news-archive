---
title: "Week in Ethereum News <br> September 16, 2023"
date: "2023-09-16"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=aobFWu7NANc&t=214s). Recap by [Tim Beiko](https://twitter.com/abcoathup/status/1702413867618640191).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1702423601037873449) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-170/):
    - Testing continues on devnet-8 and MEV-Boost workflows on kurtosis
    
    - Max epoch churn limit (EIP7514) added to Dencun, the maximum new stakers per epoch will be set to 8;  
        Dankrad: EIP7514 [gives time to deal with economic/tech consequences of Lido attack](https://notes.ethereum.org/@dankrad/churn-limit)
    
    - BLOBBASEFEE opcode (EIP7516) for L2 fee calculations added to Dencun
    
    - EIP4788 (beacon block root in EVM) being updated with changes from audits
    
    - Devnet-9 to include EIP7514, EIP7516 & EIP4788 changes, ACDC to set launch date
    
    - [Reth intro](https://docs.google.com/presentation/d/1alcw5tbqQ4NRkjoGE5YfBWKy3qFc_55CabbeyPI6IP0): EL client in Rust, hoping to join devnet-9

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 32.3%**](https://dune.com/hildobby/eth2-staking) **has reduced slightly but still very close to breaching risky** [**33% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm over 33%, a bug could mean loss of finality

- Need more [geographic diversity for both stakers and nodes](https://nodewatch.io/), particularly outside of US/Can/EU

**Layer 1**

- [Epoch churn limit](https://twitter.com/christine_dkim/status/1701302000107782559) increased from 11 to 12 (EIP7514 in Dencun sets to 8 for deposits)

- MEV-build-rs [alpha](https://mev-rs.pbs.dev/mev-build-rs.html): MEV-Boost builder in Rust, extends Reth (EL client)

**For Stakers**

- [Lodestar incentive program](https://blog.chainsafe.io/the-lodestar-user-incentive-program-list-of-winners-dispute-period-9a3d66d98b7d) results, 86 validators to share $25k

- [Geth node](https://twitter.com/ethereumonarm/status/1701891496645956028) running on NanoPC-T6 ($129 board), synced in 13 hours

- [Secure-signer](https://mirror.xyz/ladislaus.eth/joTqwZ1sBLxlJayV4pIYxCkwl4RWheM_xipU_OCp9MM) (alpha): remote-signing inside hardware enclave

- [Tor Push](https://twitter.com/vacp2p/status/1702289509252026467): proof of concept for validator privacy, push messages into gossipsub via Tor

**Client releases**

- Consensus layer:
    - Nimbus [v23.9.0](https://github.com/status-im/nimbus-eth2/releases/tag/v23.9.0): Holešky testnet support and simplified config for remote signers

- Execution layer:
    - Geth [v1.13.0](https://blog.ethereum.org/2023/09/12/geth-v1-13-0): pruning reimplemented using path based storage (needs a resync)

**Research**

- [Streamlining fast finality](https://ethresear.ch/t/streamlining-fast-finality/16591): single proposal and voting phase per slot using strong confirmation

- [Two-tiered staking](https://notes.ethereum.org/@mikeneuder/goldilocks): native liquid staking design

**EIPs/Standards**

- EIPs
    - [EIP7516](https://eips.ethereum.org/EIPS/eip-7516): BLOBBASEFEE opcode

- ERCs (application layer):
    - [ERC7515](https://github.com/ethereum/EIPs/pull/7678/files): NFT alternative text in metadata
    
    - [ERC7517](https://github.com/ethereum/EIPs/pull/7682/files): Content consent for AI/ML data mining
    
    - [ERC7518](https://github.com/ethereum/EIPs/pull/7719/files): Global compliant STO & interoperable asset lifecycle (ERC1155 extension)

**Stuff for developers**

- [Holešky testnet didn’t launch](https://twitter.com/parithosh_j/status/1702816780542984504) due to misconfiguration, relaunch expected in two weeks

- Hardhat [v2.17.3](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.17.3): default EVM set to Paris for solc v0.8.20+ (for L2s that don’t support Shanghai)

- [Invariant check in modifier skipped](https://twitter.com/zachobront/status/1699954240058277928) if an assembly block directly returns

- Overview of [minimal proxies](https://banteg.xyz/posts/minimal-proxies/): ERC1167 variants and Clones with immutable arguments

- [ERC4626 conformance](https://medium.com/@vikram.arun/multichain-erc-4626-conformance-f34b682b273b): 20% of vaults don’t conform

- [MinimalAccount](https://github.com/kopy-kat/MinimalAccount#readme) (ERC4337): gas-optimized implementation in Huff for benchmarking

- [ERC deployments](https://dune.com/ilemi/erc-and-eip-starter-kit): Dune dashboard showing number of deployments for common ERCs

- [Huff-stack-generator](https://github.com/shafu0x/huff-stack-generator#readme): generate stack comments

- [Geas](https://github.com/fjl/geas#readme) (Good Ethereum Assembler): macro assembler for the EVM

- Slitherin (custom Slither detectors) [v0.3](https://github.com/pessimistic-io/slitherin/releases/tag/v0.3.0): adds arbitrary call detector 

- [Vyper compiler](https://x.com/CodeHawks/status/1702200846941823371) audit competition

- CTFs:
    - [ONLYPWNER](https://onlypwner.xyz/documentation): CTF platform with 9 challenges
    
    - Curta CTF [Murder Mystery writeup](https://github.com/hrkrshnn/notes/blob/main/2023/curta.md) and a [solution](https://twitter.com/zigtur/status/1700945573166149830)
    
    - Secureum RACE #21: [8 question Solidity quiz & answers](https://ventral.digital/posts/2023/9/5/race-21-of-the-secureum-bootcamp-epoch-infinity)

- Paradigm’s [Rust x Ethereum slides & videos](https://twitter.com/gakonst/status/1701631039008084126): Reth, Foundry, Alloy, Ruint and wagmi/viem & Rivet

- [ZK Face ID wallet](https://hackmd.io/@knownothing/zk-face-id) (ERC4337) demo, uses WebAuthn and Halo2 proof 

**Security**

- Balancer [postmortem of two Linear Pools vulnerabilities](https://medium.com/balancer-protocol/rate-manipulation-in-balancer-boosted-pools-technical-postmortem-53db4b642492): $1M bounty paid for first vulnerability and second vulnerability exploited for $1.2M on mainnet & Optimism

- [Browsing for bugs](https://www.zellic.io/blog/browsing-for-bugs-3m-bug-in-premia-finance): finding a Premia vulnerability with $3M at risk, fixed with bounty paid

**Ecosystem**

- [1 year mergeversary](https://twitter.com/ultrasoundmoney/status/1702599071398277183) 🐼, supply reduced by 300k ETH
    - [MEV-Boost](https://collective.flashbots.net/t/merge-anniversary-a-year-in-review/2400): first year of out-of-protocol PBS

- [ETHAccra](https://taikai.network/ethaccra/hackathons/hackathon/projects) hackathon projects

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 7 to 411 gwei, with 15.6 gwei average
    - Negative issuance currently at 20.6 gwei 
    
    - 3.9k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $1,541 - 1,653, currently $1642

- [ETHBTC](https://ratiogang.com/): currently 0.0616 (Flippening at ~0.16)

**Notable at app layer**

- MetaMask [Snaps beta](https://metamask.io/news/latest/snaps-in-metamask-stable-and-where-we-go-from-here/): wallet plugins for transaction security, chat & non-EVM networks

- [Uniswap UI](https://x.com/Uniswap/status/1701229817411342396) auto detects fee on transfer tokens

- [Gaslite](https://drop.gaslite.org/): airdrop ETH, ERC20 & ERC721 tokens, including ETH to Friend Tech key holders

- [Optimism](https://twitter.com/optimismgov/status/1702748223847170261) directly distributing unclaimed OP for Airdrop 1

* * *

### Job Listings

- [Product Manager - L2 Blockchain Effort](https://grnh.se/48614a711us) @ Status: [All jobs](https://grnh.se/9fc6e6fc1us)

- EF Privacy & Scaling Explorations team seek a [Technical Project Coordinator](https://jobs.lever.co/ethereumfoundation/c826b9a1-ede0-465e-9639-f34029304374)

- [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db) wanted by EF

**Job listings: $600 for four issues** (75 character limit).  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [SEC claims Stoner Cats NFTs are securities](https://www.sec.gov/news/press-release/2023-178): $1 million fine, return sale proceeds & destroy NFTs held by the team
    - [Unanimous Republican dissent](https://www.sec.gov/news/statement/peirce-uyeda-statement-stonercats-091323) from Commissioners Peirce & Uyeda
    
    - Jonathan Mann’s [this song is a security](https://songaday.world/auction/5369) NFT sold for 6 ETH

- [DeFi Education Fund](https://twitter.com/amandatums/status/1701237935536796087) attempts to cancel a US patent claiming to invent oracles

- [Three PayPal dollars](https://jpkoning.blogspot.com/2023/09/there-are-now-two-types-of-paypal.html): centralized, crypto & savings, with crypto offering better protections than centralized but savings offers deposit insurance & interest

- [FTX allowed to sell](https://www.coindesk.com/policy/2023/09/13/judge-allows-bankrupt-ftx-to-sell-its-crypto-holdings-including-btc-and-sol/) its crypto assets

**General**

- [Remove your phone number](https://twitter.com/timbeiko/status/1700659107764785336) from Twitter (X) to prevent account recovery by sim swap

- [Pink Drainer](https://twitter.com/boringsecdao/status/1700724667391307863) targets users with most profitable attack: Seaport bulk listing signature, setApprovalForAll, upgradeTo, transfer ETH and transferPunk

- [ZachXBT refund](https://x.com/zachxbt/status/1701232146159931730) for legal fee donations

- Centralized exchange hot wallet thefts: $54M from [CoinEx](https://rekt.news/coinex-rekt/) & $2.7M from [Remitano](https://rekt.news/remitano-rekt/)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-16-2023](https://weekinethereumnews.com/week-in-ethereum-news-september-16-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Sep 18-24 – [ETHSafari](https://ethsafari.xyz/) (Kilifi Kenya)

- Sep 21–24 – [Pragma](https://ethglobal.com/events/pragma-newyork) & [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 13-15 – [Ethereum Kuala Lumpur](https://hack.ethkl.org/) conference & hackathon

- Oct 21 – [Ethereum México](https://twitter.com/ethereum_mexico/status/1684649652639924224)

- Oct 22-24 – [ETH Hong Kong](https://www.ethhongkong.co/)

- Oct 27-29 – [ETH London](https://www.encode.club/eth-london) hackathon

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Oct 27-29 – [ETH Vietnam](https://www.eth-vietnam.com/)

- Oct 28-30 – [Paradigm CTF](https://ctf.paradigm.xyz/)

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) deadline (max $1k for local meetups)

- Nov 3-5 – [ETHBrno](https://ethbrno.cz)

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 16-19 – [Pragma](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Dec 4-5 – [ETHVenice](https://ethvenice.com/)

- Dec 8-10 – ETHGlobal [ETHIndia](https://ethindia.co/) (Bangalore) 

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

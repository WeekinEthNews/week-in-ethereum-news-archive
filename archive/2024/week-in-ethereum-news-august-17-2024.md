---
title: "Week in Ethereum News <br> August 17, 2024"
date: "2024-08-17"
---

## Eth News and Links

**All core devs**

- [All Core Devs - Execution (ACDE) #194](https://ethereum-magicians.org/t/all-core-devs-execution-acde-194-august-15-2024/20703):
    - **Pectra (Prague + Electra) upgrade**:
        - **Pectra-devnet-3**: launch in 2 weeks with EIP7702 (set EOA account code)
        
        - **EOF**: targeting Pectra-devnet-4 in ~4 weeks
        
        - **EIP2537 BLS precompile**: reprice gas costs based on benchmarks
        
        - **PeerDAS**: plan to rebase code from Dencun to Pectra but avoid testing other Pectra EIPs on PeerDAS devnets
    
    - **EIP7732 ePBS**: no execution layer changes required other than builder API, provides delayed execution validation, spec is stable & implementations have started
    
    - **Post-merge cleanup proposals:**
        - Remove totalDifficulty from Execution API
        
        - EIP7642 eth/69: drop pre-merge fields to reduce bandwidth

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade, likely targeting Q1 2025**

- PeerDAS:
    - [PeerDAS breakout #7](https://ethereum-magicians.org/t/epbs-breakout-7-august-16-2024/20797): discussed moving to slot auctions to address free data availability problem in block auctions

[**Osaka + F starname**](https://eips.ethereum.org/EIPS/eip-7607) **upgrade**

- [F-starname](https://github.com/ethereum/pm/issues/1129#issuecomment-2286790680) last call: suggestion to name consensus layer upgrade Fulu (current favorite) and combined upgrade Fosaka (Osaka + Fulu)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.7%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~55% majority 
    
    - Consensus layer: Prysm 36%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Layer 1**

- Toni Wahrstätter: [evolution of timing games](https://ethresear.ch/t/on-attestations-block-propagation-and-timing-games/20272), Kiln causes biggest problems

- Lighthouse [tree-states](https://lighthouse-blog.sigmaprime.io/tree-states-part1.html) explainer, reduce RAM while keeping more beacon states in memory

- [Dora](https://x.com/parithosh_j/status/1823348169180082668) (explorer): add views of execution & consensus layer clients peer mesh

**Research**

- [Censorship insurance markets for BRAID](https://ethresear.ch/t/censorship-insurance-markets-for-braid/20288): proposal to improve user experience issue of liquidity requirements

**Client Releases**

- Execution layer:
    - EthereumJS [v0.10.2](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs/client%400.10.2): RPC improvements
    
    - Erigon [v2.60.6](https://github.com/erigontech/erigon/releases/tag/v2.60.6): improvements to stateDiff encoding, callTracer & diagnostics
    
    - Geth [v1.14.8](https://github.com/ethereum/go-ethereum/releases/tag/v1.14.8): bug fixes
    
    - Nethermind [v1.28.0](https://github.com/NethermindEth/nethermind/releases/tag/1.28.0): adds eth\_simulate, enhances OP Stack support & tune Pruning.CacheMb
    
    - Reth [v1.0.5](https://github.com/paradigmxyz/reth/releases/tag/v1.0.5): OP Granite upgrade support

**Layer 2**

- Optimism [activated permissioned fallback](https://gov.optimism.io/t/upgrade-proposal-10-granite-network-upgrade/8733) until vulnerabilities from fault proof audits are fixed by Granite upgrade

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7756](https://github.com/ethereum/EIPs/pull/8799/files): EOF/EVM trace specification (adds EOF support to EIP3155 tracing)

- RIPs (Rollup improvement proposals):
    - [RIP7755](https://github.com/ethereum/RIPs/pull/31/files): Cross-L2-calls

**Stuff for developers**

- Brock: [intervals of memory/heap allocated values](https://brocke.xyz/interval-expanded) in Solidity

- [Bulloak toolchain](https://github.com/smol-ninja/bulloak-toolchain#readme) (GitHub Action): check Solidity tests conform to Branching Tree Technique spec

- Halmos [v0.1.14](https://github.com/a16z/halmos/releases/tag/v0.1.14) (symbolic testing): adds toml config, Docker image & forge-std assert cheatcode support

- MACI [v2](https://maci.pse.dev/blog/2024-v2): adds concurrent polls and custom gatekeepers: Hats Protocol, Gitcoin Passport, Zupass & Semaphore
    - Contribute to [MACI v2 trusted setup ceremony](https://ceremony.pse.dev/projects/MACI%20v2%20Trusted%20Setup%20Ceremony)

**Ecosystem**

- Eth Magicians [call for contributions](https://ethereum-magicians.org/t/call-for-contributions-fellowship-of-ethereum-magicians/20814): new ideas, logo & moderators wanted

- EF [data collection grant recipients](https://blog.ethereum.org/2024/08/14/data-collection-round) share $560k

* * *

### Job Listings

- [Sablier](https://sablier.notion.site/Careers-at-Sablier-d3771d8eefbf44a8a8428436fb950a1d) are hiring a Business Development Lead and Frontend Engineer

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 0.6 to 23.5 gwei, 2.5 gwei average; zero net issuance at 23.9 gwei 
    
    - 16k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,534 - $2,752, currently $2,593, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.044 (Flippening at ~0.164)

**Notable at app layer**

- [Maker voted to offboard WBTC](https://vote.makerdao.com/executive/template-executive-vote-wbtc-vault-debt-ceiling-reductions-stability-scope-parameter-changes-bug-bounty-payments-clippermomjob-update-july-2024-aligned-delegate-compensation-6s-capital-stability-fee-increase-monetalis-clydesdale-and-coinbase-custody-dao-resolutions-spark-proxy-spell-august-12-2024) after BitGo announced plans for [BiT Global](https://blog.bitgo.com/bitgo-to-move-wbtc-to-multi-jurisdictional-custody-to-accelerate-global-expansion-plan-2ea0623fa2c8) (Justin Sun) to hold 2 of 3 multisig keys, due to the backlash [BitGo Singapore will now hold 3rd key](https://x.com/BitGo/status/1823751918575095854)
    - Coinbase hinted at a future [cbBTC](https://x.com/coinbase/status/1823501582006411614)

- [Accept USDC](https://acceptusdc.com/): campaign for small retailers to accept USDC payments 

**Regulation/business/tokens**

- Thai SEC [digital asset regulatory sandbox](https://www.sec.or.th/EN/Pages/News_Detail.aspx?SECID=11004) open for applications

- CoinDesk: [Eigen Labs sent employee addresses to EigenLayer projects](https://www.coindesk.com/tech/2024/08/15/top-crypto-startup-drove-other-projects-airdrops-to-its-employees/) for token airdrops

**General**

- Alex Pertsev [fundraiser for appeal](https://x.com/alex_pertsev/status/1822184616620339397) to 5 year sentence

- ZachXBT: [DPRK IT workers uncovered at 25+ projects](https://x.com/zachxbt/status/1824047425822310580)

- [NIST post quantum encryption algorithms](https://www.nist.gov/news-events/news/2024/08/nist-releases-first-3-finalized-post-quantum-encryption-standards): ML-KEM, ML-DSA & SLH-DSA

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-august-17-2024](https://weekinethereumnews.com/week-in-ethereum-news-august-17-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 23-26 – [ETHTokyo](https://www.ethtokyo.com/) hackathon & conference

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- Aug 31 – [Underhanded Solidity contest](https://soliditylang.org/blog/2024/07/31/underhanded-solidity-contest-2024-announcement/) deadline

- Sep 5-8 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 9-15 – [ETHSafari](https://ethsafari.xyz/) (Kenya)

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 13-14 – [Ethereum México](https://ethmexico.org/)

- Sep 20-22 – [ETHCapeTown](https://www.ethcapetown.com/) hackathon

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Sep 26-27 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 4-6 – [Ethereum Kuala Lumpur](https://www.2024.ethkl.org/) conference & hackathon

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 17-20 – [ETHLisbon](https://ethlisbon.org/) hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

- **Dec 6-8 –** [**ETHIndia**](https://ethindia.co/) **hackathon**

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

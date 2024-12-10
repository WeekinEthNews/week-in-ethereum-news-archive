---
title: "Week in Ethereum News <br> December 7, 2024"
date: "2024-12-07"
---

## Eth News and Links

**Eth R&D protocol call (All Core Devs)**

- [Execution layer focused protocol call](https://ethereum-magicians.org/t/all-core-devs-execution-acde-201-december-5-2024/21760) (ACDE #201):
    - **Pectra upgrade:**
        - [**Mekong testnet**](https://mekong.ethpandaops.io/): 97% participation, client teams fixing issues
        
        - [**Pectra-devnet-5 spec**](https://notes.ethereum.org/@ethpandaops/pectra-devnet-5): ideally launch devnet before the holidays
        
        - **EIP2537 BLS precompile:** 2-3x gas cost increase proposed, agree async
        
        - **EIP7623 increase calldata cost:** scheduled for inclusion in Pectra, discuss on testing call which devnet to add to
        
        - **EIP7762 increase min blob base fee**: not included for now, discuss at RollCall (L2 standards) & consensus layer call (ACDC) next week
    
    - **EIP4803 limit transaction gas**: proposed to retroactively include
    
    - [**History expiry plan**](https://hackmd.io/Dobc38YVQ1qmbbyI6LcFqA): pre-merge expiry set for May 1, discussed if new eth/70 protocol needed (EIP7639)
    
    - [**All Core Devs process improvements**](https://ethereum-magicians.org/t/allcoredevs-network-upgrade-ethmagicians-process-improvements/20157/51): added Declined for Inclusion EIP status and non-consensus changing EIPs can be included in upgrade Meta EIPs

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- [Client testing call #15](https://ethereum-magicians.org/t/client-testing-call-15-december-2-2024/21929): Mekong testnet deposit processing fixed and Pectra-devnet-5 spec discussions

- [Pectra system contracts](https://x.com/parithosh_j/status/1863543767233368324) for consolidations, withdrawals & block hash lookup; used instead of precompiles, implemented in Assembly

[**Amsterdam**](https://eips.ethereum.org/EIPS/eip-7773) **upgrade**

- [Stateless implementers call #28](https://ethereum-magicians.org/t/stateless-implementers-call-28-december-2-2024/21939) (formerly Verkle): file based approach for preimage distribution and implementation in progress of EIP7736 leaf-level state expiry

**Layer 1**

- [Bandwidth availability](https://ethresear.ch/t/bandwidth-availability-in-ethereum-regional-differences-and-network-impacts/21138) shows reasonable to increase blob count

- [EVMMAX implementers call #1](https://ethereum-magicians.org/t/evmmax-implementers-call-1-december-5-2024/21976): Poseidon planned as first use case

**For stakers**

- [Slashing event](https://x.com/nixorokish/status/1864679505425486123): 21 validators slashed for attestation violation

- [SOLO](https://ethresear.ch/t/solo-liquid-staking-for-solo-validators/21157): proposal for liquid staking using portion of stake unlikely to be lost, without needing governance, trusted hardware or permissioned operator sets

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.1%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~43% & Nethermind ~36% (estimate based on 74% self reported data)
    
    - Consensus layer: Prysm 35%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Client Releases**

- Consensus layer:
    - Lighthouse [v6.0.0](https://github.com/sigp/lighthouse/releases/tag/v6.0.0): hierarchical state diffs (on-disk tree states) for more compact archive nodes, downgrading requires resync
    
    - Nimbus [v24.11.0](https://github.com/status-im/nimbus-eth2/releases/tag/v24.11.0): faster forward sync, experimental light client-based sync (testing only) and fixes config mismatch errors for unscheduled upgrades

**Layer 2**

- [Arbitrum Connect](https://arbitrumconnect.wakeuplabs.io/): interface for users to force include transactions during sequencer downtime

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7830](https://eips.ethereum.org/EIPS/eip-7830): Contract size limit increase for EOF
    
    - [EIP7833](https://github.com/ethereum/EIPs/pull/9096/files): Scheduled function calls
    
    - [EIP7834](https://github.com/ethereum/EIPs/pull/9100/files): Separate metadata section for EOF

- ERCs (application layer):
    - [ERC7831](https://github.com/ethereum/ERCs/pull/749/files): Multi-chain addressing
    
    - [ERC7832](https://github.com/ethereum/ERCs/pull/752/files): Sustainable NFT collections
    
    - [ERC7835](https://github.com/ethereum/ERCs/pull/755/files): wallet\_transmitCrossChainIntents method
    
    - [ERC7836](https://github.com/ethereum/ERCs/pull/758/files): Wallet call preparation API

**Stuff for developers**

- Foundry: [forge build](https://github.com/foundry-rs/compilers/pull/231) 10-36% faster compilation, [forge coverage](https://github.com/foundry-rs/foundry/pull/9456) 2x faster

- Hardhat [v2.22.17](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.22.17): adds Solidity v0.8.28 support

- Ape [v0.8.21](https://github.com/ApeWorX/ape/releases/tag/v0.8.21) (Python contract framework): faster console launch & auto fork chains

- Frangio: [Solidity learnings](https://frang.io/blog/the-next-700-evm-languages/) & working on EVML (EVM language)

- [Tornado Cash reference manual](https://zk.bearblog.dev/tornado-cash-manual/): architecture, Circom circuit, Solidity contracts and client side proof generation & verification

- [eth\_simulateV1 explainer](https://mirror.xyz/killaridev.eth/eQhG3pw-P-iqdLWaEFJ_nKzr5SdaoY00ECZYcQuymAM): standardized approach for multicall via JSON-RPC

- Rotki [balance scanner](https://github.com/rotki/balanceScanner#readme) (Vyper): query ETH/token balances, deployed on mainnet & L2s

- [Drift](https://x.com/ryegoree/status/1864345044364206464) (create cached contract calls): adds hooks

- [Safe owner manager](https://github.com/GNSPS/safe-owner-manager#readme): manage Safe multisig owners & thresholds in bulk

**Security**

- Vestra [$500k exploit](https://x.com/Vestra_DAO/status/1864677381459390781) on mainnet

- Clipper (DEX) [$460k exploit](https://blog.clipper.exchange/clipper-dec-24-exploit-post-mortem/) on Optimism & Base

- Spectral Syntax v2 [$200k exploit](https://spectral-labs.notion.site/Post-Mortem-14fed21b975880f681ecd85c76c9536f) on Base via infinite approval

- [ETH Rangers](https://blog.ethereum.org/2024/12/02/ethrangers-public-goods), $25k stipend from EF for public goods security work, December 20 deadline

* * *

### Job Listings

- Mimic: [Tech Lead Engineer](https://mimic-fi.notion.site/Tech-Lead-Engineer-14b9958dbf4d80d88dadf252126e6375)

- Vyper (Pythonic EVM language) seek a [DevRel](https://e63fu2j2ew4.typeform.com/to/Rt6A2juT)

- Nethermind: [AI Agent](https://job-boards.eu.greenhouse.io/nethermind/jobs/4465865101), [Infra](https://job-boards.eu.greenhouse.io/nethermind/jobs/4467282101), [Blockchain](https://job-boards.eu.greenhouse.io/nethermind/jobs/4467974101), [Full Stack](https://job-boards.eu.greenhouse.io/nethermind/jobs/4467217101), [BizDev](https://job-boards.eu.greenhouse.io/nethermind/jobs/4471319101) & [Researcher](https://job-boards.eu.greenhouse.io/nethermind/jobs/4466531101)

**Job listings: $600 for 4 issues** (75 char limit). [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.** Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 4.5 to 202.4 gwei, 20.2 gwei average; zero net issuance at 24.1 gwei
    
    - 2.7k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,543 - $4,089, currently $4,022, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.04 (Flippening at ~0.164)

**Ecosystem**

- [EF Q3 grantees](https://blog.ethereum.org/2024/12/03/esp-allocation-q324) share $12.8 million in funding

- [Public goods dashboards](https://x.com/EFDevcon/status/1863672042186551733) share $250k via quadratic voting at Devcon

**Enterprise**

- Wyoming stable token commission: [request for qualifications](https://stabletoken.notion.site/Request-For-Qualification-Info-Center-141c90ef13ad80ddbf23c017fca789bc) to support state issued USD backed stablecoin, deadline December 12

**Notable at app layer**

- [Vitalik’s ideal wallet](https://vitalik.eth.limo/general/2024/12/03/wallets.html): cross-L2, secure from users & wallet devs, private transfers, store private data, secure chain access & keystores

- [ENS DAO grants](https://docs.ensdaogrants.xyz/main#list-of-large-grants-recepients): $12-50k for public goods projects

**Regulation/business/tokens**

- [Paul Atkins](https://truthsocial.com/@realDonaldTrump/113595807734621827) to be nominated as SEC Chair; [David Sacks](https://truthsocial.com/@realDonaldTrump/113603133222686186) to be White House AI & crypto czar

- Coinbase obtained [FDIC’s requests for banks to pause crypto activities](https://downloads.ctfassets.net/c5bd0wqjc7v0/6y0GZ2y2LzOZi1gUnCTtxh/55bf6ae9665ca12b9fe7bdfb3ebe746b/-26-1-_Exhibit_A_-_Redacted_Pause_Letters.pdf)

- [Alex Mashinsky](https://www.reuters.com/technology/celsius-founder-alex-mashinsky-intends-plead-guilty-two-fraud-counts-2024-12-03/) (former Celsius CEO) pleaded guilty to fraud

**General**

- XT exchange [$1M stolen](https://xtsupport.zendesk.com/hc/en-us/articles/40528847749657-XT-COM-Statement-on-Abnormal-Transfer-of-Platform-Wallet-Assets)

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-december-7-2024](https://weekinethereumnews.com/week-in-ethereum-news-december-7-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Dec 9 – [EF internships 2025](https://blog.ethereum.org/2024/11/16/announcing-ef-internship-program) application deadline

- **Dec 20 –** [**ETH Rangers**](https://blog.ethereum.org/2024/12/02/ethrangers-public-goods) **application deadline**

- Jan 20 – [Ethereum protocol attackathon](https://blog.ethereum.org/2024/11/25/ethereum-protocol-attackathon) ends

- Jan 30-31 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Feb 23 - Mar 2 – [ETHDenver](https://www.ethdenver.com/)

- Apr 4-6 – [ETHGlobal Taipei](https://ethglobal.com/events/taipei) hackathon

- May 9-11 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 27-29 – [ETHPrague](https://ethprague.com/) conference

- May 30 - Jun 1 – [ETHGlobal Prague](https://ethglobal.com/events/prague) hackathon

- Jun 3-8 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 12-13 – [Protocol Berg](https://protocol.berlin/) (Berlin) conference

- Jun 16-18 – [DappCon](https://dappcon.io/) (Berlin)

- Jun 26-28 – [ETHCluj](https://www.ethcluj.org/) (Romania) conference

- Jun 30 - Jul 3 – [EthCC](https://ethcc.io/) (Cannes) conference

- Jul 4-6 – [ETHGlobal Cannes](https://ethglobal.com/events/cannes) hackathon

- Aug 15-17 – [ETHGlobal New York](https://ethglobal.com/events/newyork2025) hackathon

- Sep 26-28 – [ETHGlobal New Delhi](https://ethglobal.com/events/newdelhi) hackathon

- Nov – [ETHGlobal Devconnect](https://ethglobal.com/events/ethglobal-devconnect) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

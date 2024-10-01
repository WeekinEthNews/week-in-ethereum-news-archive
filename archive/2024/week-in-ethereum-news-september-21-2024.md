---
title: "Week in Ethereum News <br> September 21, 2024"
date: "2024-09-21"
---

## Eth News and Links

Pectra split into two upgrades with PectrA capped at devnet-3 EIPs & USDS stablecoin live

**All core devs**

- [All Core Devs – Consensus (ACDC) #142](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-142-september-19-2024/21086):
    - **Pectra (Prague + Electra) upgrade:**
        - [**Pectra-devnet-3**](https://pectra-devnet-3.ethpandaops.io/): issues found by bad block fuzzer being debugged
        
        - **Pectra split discussion**:
            - Pectra scope (PectrA) capped at EIPs in devnet-3
            
            - Second upgrade scope (PectrB) yet to be decided, concerns on scope creep if not frozen, candidates include PeerDAS & EOF, discussion on including Verkle ahead of EOF and proposal to add EIP7688 SSZ stable container
            
            - Client team perspectives: [Erigon](https://hackmd.io/@somnergy/rJYyPoK6C) & [Prysm](https://hackmd.io/@potuz/rk9_ETt60)
            
            - Base proposed [Pectra blob increase](https://docs.google.com/document/d/1mkxfhDNvbT6jFEjH3e6LADsGGh3jEvL_WOt2glFbFfA/edit#heading=h.v2qm0jqcd4bj): client teams generally support increase of blob target but not max count without PeerDAS, needs more analysis, IDONTWANT messages should reduce bandwidth
        
        - **PectrA EIP improvements**: changes to validator consolidation in EIP7251, deposit flow in EIP6110, attestation refactoring in EIP7549 and opaque requests in EIP7685

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- [Pectra testing call #5](https://ethereum-magicians.org/t/pectra-testing-call-5-16-september-2024/21111):
    - Builder specs & remote signer API need updating and more clients ready for EOF devnet

- Consensus-specs [v1.5.0-alpha.6](https://github.com/ethereum/consensus-specs/releases/tag/v1.5.0-alpha.6): minor fixes for Electra, PeerDAS & ePBS

- [EOF implementers call #58](https://ethereum-magicians.org/t/eof-implementers-call-58-september-18-2024/21147):
    - Discussions on EIP7761 HASCONTRACT for ERC721/1155 NFTs, EXTCALL return codes and allowing EXTDELEGATECALL to legacy 

- [PeerDAS breakout #8](https://ethereum-magicians.org/t/peerdas-breakout-8-september-17-2024/20985):
    - Debugging local devnet forking issues before launching peerdas-devnet-2
    
    - Validity custody is main remaining spec change before shipping

- Distributed block building call #0 [video](https://www.youtube.com/watch?v=fnmZCMWk6xY): discussed Dankrad’s proposal to gossip sample proofs

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.1%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~52% majority
    
    - Consensus layer: Prysm 37%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Layer 1**

- [ePBS slot auctions](https://ethresear.ch/t/trusted-advantage-in-slot-auction-epbs/20456) don’t satisfy No Trusted Advantage

- Terence: [FOCIL resource considerations](https://ethresear.ch/t/focil-resource-design-considerations/20457)

- Potuz: proposal to [decouple execution & consensus layer syncing](https://hackmd.io/@potuz/HkZ5ZWv6A)

- Péter Szilágyi: SSZ [v0.3.0](https://github.com/karalabe/ssz/releases/tag/v0.3.0) (library in Go): adds monolithic type support, fixes decoding zero-length dynamic arrays and adds SizeSSZ

- [SSZ deserialization differences disclosed](https://www.asymmetric.re/blog/ghost-in-the-block-ethereum-consensus-vulnerability) between Prysm & Lighthouse

**Research**

- [Variable orbit single slot finality with circular & spiral finality](https://ethresear.ch/t/vorbit-ssf-with-circular-and-spiral-finality-validator-selection-and-distribution/20464): review of cumulative committee-based finality under fast-rotating validator committees and avenues to reduce aggregate finality gap

**Client Releases**

- Consensus layer:
    - Lodestar [v1.22.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.22.0): minor performance optimizations including shortening startup time

- Execution layer:
    - Besu [v24.9.1](https://github.com/hyperledger/besu/releases/tag/24.9.1): adds client version info for consensus layer graffiti
    
    - Geth [v1.14.9](https://github.com/ethereum/go-ethereum/releases/tag/v1.14.9): adds multicall (eth\_simulateV1) support
    
    - Reth [v1.0.7](https://github.com/paradigmxyz/reth/releases/tag/v1.0.7): adds multicall (eth\_simulateV1) support

**Layer 2**

- Hildobby: [L2 blob usage](https://x.com/hildobby_/status/1836359358843883843), pruned blobs ~30GB & full history 275GB

- Norswap: [cross-chain interoperability overview](https://github.com/0xFableOrg/xchain/blob/master/README.md) & applicability to Optimism Superchain

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7768](https://github.com/ethereum/EIPs/pull/8888/files): No-Ether transactions with free-for-all tips

- ERCs (application layer):
    - [ERC7769](https://github.com/ethereum/ERCs/pull/628/files): JSON-RPC API for ERC4337 (account abstraction)
    
    - [ERC7770](https://github.com/ethereum/ERCs/pull/644/files): Fractional reserve token
    
    - [ERC7771](https://github.com/ethereum/ERCs/pull/647/files): Router proxy
    
    - [ERC7772](https://github.com/ethereum/ERCs/pull/649/files): Partial gas sponsorship

**Stuff for developers**

- Foundry [decode internal](https://github.com/foundry-rs/foundry/pull/8222): trace internal function calls & generate flamegraph/chart

- [Tevm cast](https://github.com/evmts/tevm-cast#readme): browser based CLI similar to Foundry cast

- Hardhat:
    - Hardhat [v2.22.11](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.22.11): adds support for latest Solidity versions (v0.8.25/26/27)
    
    - Hardhat-verify [v2.0.11](https://github.com/NomicFoundation/hardhat/releases/tag/%40nomicfoundation/hardhat-verify%402.0.11): adds Blockscout verification

- Remix [v0.54.0](https://medium.com/remix-ide/remix-release-v0-54-0-021575d54849): adds Cookbook templates & GitHub login from file explorer

- [ERC7726 common quote oracle](https://hackernoon.com/erc-7726-never-code-an-oracle-in-ethereum-again) explainer

- [Huff](https://github.com/huff-language/) (language) sunset, repos archived

- [Sourcify](https://x.com/sourcifyeth/status/1836042721972359399): 5M verified contracts available to download in Parquet format or zip

- [EthereumJS EVM code & dependencies](https://gist.github.com/holgerd77/2c032488196b4afee5d976dc85ee70eb) published as un-minified bundle to gist

- Google Cloud [blockchain RPC](https://cloud.google.com/blog/topics/financial-services/introducing-blockchain-rpc-service-for-web3-builders): mainnet & testnets, free tier up to 100 requests/second

- Semaphore [v4](https://github.com/semaphore-protocol/semaphore/releases/tag/v4.0.0): changed to Lean Incremental Merkle Tree and EdDSA identity schema

**Security**

- DeltaPrime [$6M exploit](https://rekt.news/deltaprime-rekt/) on Arbitrum via compromised admin private key

- [Liquid restaking](https://blog.sigmaprime.io/liquid-restaking.html) common vulnerabilities & security risks

**Ecosystem**

- [Privacy and Scaling Explorations](https://pse-team.notion.site/A-new-era-for-PSE-f4cde2e1a20d49ed92071a93ad8ba7df) (PSE): Barry Whitehat leaving, Sam Richards taking over & some projects sunsetting

- [Vitalik: An Ethereum Story](https://ethereumfilm.xyz/streaming) (movie): token gated stream via $20 mint, available for 1 month

**Enterprise**

- WisdomTree [Connect](https://ir.wisdomtree.com/news-events/press-releases/detail/704/wisdomtree-launches-new-platform---wisdomtree-connect): tokenized real world assets on mainnet

- Enterprise Ethereum Alliance: [DLT interoperability specification v1](https://entethalliance.org/eea-releases-dlt-interoperability-specification/)

* * *

### Job Listings

- Nethermind: [ZK Engineer](https://job-boards.eu.greenhouse.io/nethermind/jobs/4382980101), [Sr Dev](https://job-boards.eu.greenhouse.io/nethermind/jobs/4387067101), [SRE Lead](https://job-boards.eu.greenhouse.io/nethermind/jobs/4390680101) & [Sr Embedded Software Dev](https://job-boards.eu.greenhouse.io/nethermind/jobs/4391152101)

- Gnosis seek [CoreDevs](https://gnosis.jobs.personio.com/job/893408?_pc=1517287), [Sr Algorithm Engineer](https://gnosis.jobs.personio.com/job/1698369?_pc=1517287), [Sr Smart Contract Engineer](https://gnosis.jobs.personio.com/job/1698390?_pc=1517287)

- [Nomos](https://free.technology/nomos) is hiring [Ecosystem Developer](https://grnh.se/6a2297081us), [Rust Engineer](https://grnh.se/bd96340e1us) & [Applied Researcher](https://grnh.se/03fe75801us)!

- [Status](https://status.app/) [free.technology](https://free.technology/) is hiring a [Business Developer](https://grnh.se/63f67b381us). More [jobs](https://free.technology/jobs) at IFT!

- Join [Witnet](https://witnet.io/) as a [Community Builder](https://wellfound.com/l/2Akjg4)! Full-time, remote opportunity.

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 0.7 to 85.6 gwei, 6.7 gwei average; zero net issuance at 24.2 gwei 
    
    - 12k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,268 - $2,577, currently $2,556, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.041 (Flippening at ~0.164)

**Notable at app layer**

- Sky (formerly Maker) [USDS stablecoin & SKY governance token](https://x.com/SkyEcosystem/status/1836401027664281972) live on mainnet

- 1inch [Fusion+](https://blog.1inch.io/1inch-introduces-fusion-plus/): atomic cross-chain swaps, beta

- [eth.link](https://x.com/eth_limo/status/1836830294101610650): ENS gateway now powered by eth.limo

**Regulation/business/tokens**

- US SEC [end of fiscal year](https://x.com/jchervinsky/status/1831404691215077757) actions:
    - [FlyfishClub settled](https://www.sec.gov/files/litigation/admin/2024/33-11305.pdf) for selling NFT restaurant memberships prior to opening
        - [Commissioners Peirce & Uyeda](https://www.sec.gov/newsroom/speeches-statements/peirce-uyeda-statement-flyfish-091624): “securities laws are not needed here, and their application is harmful both in the present case and as future precedent”
    
    - [Rari Capital charged](https://www.sec.gov/newsroom/press-releases/2024-138) with misleading investors & acting as unregistered brokers
    
    - [Prager Metis (auditors) settled](https://www.sec.gov/newsroom/press-releases/2024-133) for negligence in FTX audits

**General**

- BingX (centralized exchange) [hot wallet compromised](https://rekt.news/bingx-rekt/)

- ZackXBT: [$243M in BTC stolen](https://x.com/zachxbt/status/1836752923830702392) from one person via social engineering, two suspects arrested

- Discord [audio & video end-to-end encryption](https://discord.com/blog/meet-dave-e2ee-for-audio-video) rolling out, doesn’t include group chats & DMs

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-september-21-2024](https://weekinethereumnews.com/week-in-ethereum-news-september-21-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Sep 26-27 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 4-6 – [Ethereum Kuala Lumpur](https://www.2024.ethkl.org/) conference & hackathon

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 17-20 – [ETHLisbon](https://ethlisbon.org/) hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

- Dec 6-8 – [ETHIndia](https://ethindia.co/) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

---
title: "Week in Ethereum News <br> August 31, 2024"
date: "2024-08-31"
---

## Eth News and Links

OpenSea received Wells notice, Maker rebrands to Sky

**All core devs**

- [All Core Devs – Execution (ACDE) #195](https://ethereum-magicians.org/t/all-core-devs-execution-acde-195-august-29-2024/20910):
    - **Pectra (Prague + Electra) upgrade**:
        - **Pectra-devnet-3**: launch once client teams pass spec tests
        
        - **EIP7702**: SELFDESTRUCT behavior clarification and proposals to change signing domain constant from 0x05 to 0x1a & check chain ID
        
        - **EOF**: discussion on ERC721/1155 needs for ISCONTRACT & impact on proxies of DELEGATECALL restriction.  Scope to remain as is for Pectra-devnet-4
        
        - **Proposed Pectra additions**:
            - **EIP7623 increase calldata cost** to reduce max block size by disincentivizing using mainnet for data availability, already candidate for inclusion
            
            - **EIP7742 uncouple blob count between CL & EL**, moved to candidate for inclusion
            
            - **Increase blob reserve price** for faster price discovery, EIP to be created & proposed for inclusion
            
            - [List of EIPs proposed for inclusion](https://github.com/ethereum/EIPs/pull/8846), to be considered on next ACDE

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- [Pectra testing call #2](https://ethereum-magicians.org/t/pectra-testing-call-2-26-august-2024/20899): Pectra-devnet-2 being left in unhealthy state for debugging

- [PeerDAS cryptography](https://eprint.iacr.org/2024/1362) proved secure

[**Fusaka**](https://eips.ethereum.org/EIPS/eip-7607) **(Osaka + Fulu) upgrade**

- [Verkle implementers call #23](https://ethereum-magicians.org/t/verkle-implementers-call-23-august-26-2024/20704): test framework progressing, 3 clients ready for next testnet and [exploration of binary trees](https://notes.ethereum.org/@gballet/verkle-and-binary) as alternative to Verkle with last minute swap fairly easy

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.4%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~52% majority
    
    - Consensus layer: Prysm 36%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Layer 1**

- ePBS:
    - [ePBS breakout #8](https://ethereum-magicians.org/t/epbs-breakout-8-august-30-2024/20839): client teams working on implementations, support for moving from block auctions to slot auctions due to free data availability issue
    
    - Terence: [block proposal in ePBS block auctions](https://hackmd.io/@ttsao/epbs-block-proposal) is slower than today, less severe in a slot auction

- [Multi-block MEV analysis](https://ethresear.ch/t/does-multi-block-mev-exist-analysis-of-2-years-of-mev-data/20345): less sequences than statistically expected, payments increase with sequence length and no indication of deliberate strategies

- [Portal Network](https://blog.nimbus.team/fluffy-and-the-portal-network-enhancing-ethereums-decentralization/) explainer, distributed storage network for Ethereum data

**Research**

- EF Research team AMA on r/Ethereum September 5, [submit your questions](https://docs.google.com/forms/d/e/1FAIpQLSc4iT1bjp_wM85l3YQAWeOWC4pNz3VZUv5JGhD9IF5zcGhC0w/viewform)

- [Execution Tickets economic modeling](https://arxiv.org/abs/2408.11255): captures some but not all MEV, reduces validator set centralization pressure but doesn’t alleviate builder centralization

- [FOCIL & BRAID compared](https://hackmd.io/xz1UyksETR-pCsazePMAjw): FOCIL is add-on to existing protocol to improve censorship resistance, BRAID is new protocol to improve censorship resistance & solve MEV

**Client Releases**

- Consensus layer:
    - Nimbus [v24.8.0](https://github.com/status-im/nimbus-eth2/releases/tag/v24.8.0): 25% speed increase for processing blocks with deposits and avoid running light client sync in background when node is synced

- Execution layer:
    - Reth [v1.0.6](https://github.com/paradigmxyz/reth/releases/tag/v1.0.6): adds experimental EngineAPI implementation with 100x improvement on fork choice update message handling and bug fixes for OP-Reth & RPC

**For Stakers**

- [Vero](https://serenita.io/blog/2024/improving-client-diversity-with-vero): multi-node validator client, uses remote signer

**EIPs/Standards**

- EIPs (Ethereum improvement proposals)::
    - [EIP7761](https://github.com/ethereum/EIPs/pull/8838/files): IS\_CONTRACT instruction (EOF)

**Stuff for developers**

- [Evm.codes](https://www.evm.codes/?fork=EOF): adds EOF opcodes proposed for Pectra (select EOF fork to view)

- RareSkills:
    - [ERC1822 universal upgradeable proxy](https://www.rareskills.io/post/uups-proxy) (UUPS) explainer
    
    - Guide to [OpenZeppelin upgrades plugin for Foundry](https://www.rareskills.io/post/openzeppelin-foundry-upgrades)

- Kontrol [v1](https://x.com/rv_inc/status/1828106093756915723) (formal verification): faster & more stable

- Revm [v14](https://github.com/bluealloy/revm/releases/tag/v42): adds latest spec of EIP7702 (set EOA account code)

- [PyXatu](https://github.com/nerolation/pyxatu#readme) (Python package): query Xatu database for execution & consensus layer data

- Lattice MUD [v2.2](https://x.com/mud_dev/status/1829555428164043187) (game framework): adds world explorer to view/modify state

- Guide to [create basic zero knowledge proofs](https://zkintro.com/articles/programming-zkps-from-zero-to-hero) (ZKPs) using Circom & Groth16

**Security**

- [Onchain hack impact estimate](https://x.com/MitchellAmador/status/1828110931718758690): $16M loss, 52% market cap decline, depressed token price for 6+ months, 3 months recovery effort & platforms (chain or primitive) are wiped out

- [Optimization bug found in LLVM](https://governance.aave.com/t/bgd-aave-v3-zksync-activation-issue-report/18819) (used by ZKsync compiler) while testing Aave deployment, doesn’t affect 64 bit machines but impacted 256 bit EVM

**Ecosystem**

- Josh Stark: [EF spending](https://x.com/0xstark/status/1828416178194104342), ~38% internal (EF teams) & ~62% external (grants) in 2022/23

- [EF Q2 grantees](https://blog.ethereum.org/2024/08/30/esp-allocation-q224) share $8M in funding

- [ETHTokyo](https://app.akindo.io/hackathons/3dXM7ZO2WsxvlkXp?tab=products) hackathon projects

- [Suggest a city](https://docs.google.com/forms/d/e/1FAIpQLSfSvVV-q5SbU_USO_vrqy7icPGgbsfLzXcQ4hbrGQaQvirJtQ/viewform) for ETHGlobal 2025 

- [ETHGas](https://www.ethgas.com/market/): gas explorer, beta

* * *

### Job Listings

- Gnosis seek [CoreDevs](https://gnosis.jobs.personio.com/job/893408?_pc=1517287), [Sr Algorithm Engineer](https://gnosis.jobs.personio.com/job/1698369?_pc=1517287), [Sr Smart Contract Engineer](https://gnosis.jobs.personio.com/job/1698390?_pc=1517287)

- Join [Witnet](https://witnet.io/) as a [Community Builder](https://wellfound.com/l/2Akjg4)! Full-time, remote opportunity.

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 0.5 to 18.7 gwei, 1.5 gwei average; zero net issuance at 23.9 gwei 
    
    - 17k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,409 - $2,809, currently $2,528, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.043 (Flippening at ~0.164)

**Notable at app layer**

- [Maker rebranded to Sky](https://forum.makerdao.com/t/sky-has-arrived/24959): USDS stablecoin ([freezable in future upgrade](https://forum.makerdao.com/t/usds-and-puredai-the-two-paths-for-decentralized-stablecoins/24987#p-98658-future-freeze-function-3)) & SKY governance token launch September 18, rewards exclude US, UK & VPN users
    - [MakerDAO Twitter handle](https://x.com/ForesightNewsEN/status/1829080229622808850) snatched

- Polygon [MATIC migration to POL](https://x.com/0xPolygon/status/1828490520340865472), manual on Ethereum, automatic on Polygon PoS

- 100x [prediction markets](https://medium.com/100xfinance/prediction-markets-on-100x-a6490d52b755) \[[Starbloom](https://twitter.com/starbloomvent) portfolio\]

- Linkdrop [Soulbounds](https://blog.linkdrop.io/linkdrop-soulbounds-onchain-badges-on-base-157192ce2a7a): create/claim non-transferrable NFTs on Base

**Regulation/business/tokens**

- [OpenSea](https://x.com/dfinzer/status/1828791832009953706) received Wells notice from SEC, NFTs on the platform alleged to be securities

**General**

- Telegram CEO [Pavel Durov arrested in France](https://www.tribunal-de-paris.justice.fr/sites/default/files/2024-08/2024-08-26%20-%20CP%20TELEGRAM%20.pdf) \[French & English\], released on [€5M bail & ban on leaving France](https://www.tribunal-de-paris.justice.fr/sites/default/files/2024-08/2024-08-28%20-%20CP%20TELEGRAM%20mise%20en%20examen.pdf) \[French\]
    - Reminder: [Telegram chats are probably visible on their servers](https://blog.cryptographyengineering.com/2024/08/25/telegram-is-not-really-an-encrypted-messaging-app/) as not end to end encrypted unless secret chats enabled

- [North Korean hackers](https://www.microsoft.com/en-us/security/blog/2024/08/30/north-korean-threat-actor-citrine-sleet-exploiting-chromium-zero-day/) targeting crypto exploited Chrome zero-day to deploy rootkit

- [Intel SGX](https://x.com/_markel___/status/1828112469010596347) encrypted root provisioning key extracted

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-august-31-2024](https://weekinethereumnews.com/week-in-ethereum-news-august-31-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Sep 2 – Scaffold-ETH 2 [extensions hackathon](https://extensions.buidlguidl.com/) deadline

- **Sep 5 – EF Research AMA on r/Ethereum,** [**submit your questions**](https://docs.google.com/forms/d/e/1FAIpQLSc4iT1bjp_wM85l3YQAWeOWC4pNz3VZUv5JGhD9IF5zcGhC0w/viewform)

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

- Dec 6-8 – [ETHIndia](https://ethindia.co/) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

---
title: "Week in Ethereum News <br> October 5, 2024"
date: "2024-10-05"
---

## Eth News and Links

**Eth R&D protocol calls (All Core Devs)**

- [Eth R&D protocol call focused on consensus layer](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-144-october-3-2024/21155) (ACDC #143):
    - **Pectra upgrade:**
        - **Pectra-devnet-3**: minor bugs being resolved
        
        - **Pectra-devnet-4**: open issue for EIP7685 execution layer requests on whether to send requests or hashes
        
        - **Public testnet**: planned for Devcon, Pectra-devnet-4 spec, [name suggestions wanted](https://ethereum-magicians.org/t/naming-the-public-pectra-testnet/21263)
    
    - **Blob increase**: more data needed, engine\_getBlobsV1 being implemented by client teams to help stakers with low bandwidth

- [Eth R&D protocol call focused on execution layer](https://ethereum-magicians.org/t/all-core-devs-execution-acde-197-september-26-2024/21085) (ACDE) #197:
    - **Pectra upgrade scope:** 
        - **Included EIPs (pectra-devnet-3 spec)**: **EIP2537** BLS precompile, **EIP2935** historical block hashes in state, **EIP6110** validator deposits onchain, **EIP7002** execution layer triggerable exits, **EIP7251** increase max effective balance, **EIP7549** committee index outside attestation, **EIP7685** general purpose execution layer requests & **EIP7702** EOA account code for one transaction
        
        - **Considered for inclusion**: **EIP7623** increase calldata cost, **EIP7742** decouple blob count, **EIP7762** increase min blob fee and a **blob increase** (needs more analysis & concerns about stakers with low bandwidth)
    
    - **Fusaka upgrade scope**: included **EIP7594** PeerDAS & **EIP7692** EOF.  No other EIPs will be scheduled for inclusion until there is a working Fusaka devnet
    
    - **Amsterdam upgrade scope**: Verkle EIPs considered for inclusion

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- Blob increase proposal:
    - Nixo: [blob increase & solo staking](https://x.com/nixorokish/status/1841189515798724665)
    
    - Toni Wahrstätter: [impact of blobs on reorgs](https://ethresear.ch/t/steelmanning-a-blob-throughput-increase-for-pectra/20499) and [analysis of solo staking & local block building](https://ethresear.ch/t/on-solo-staking-local-block-building-and-blobs/20540)
    
    - [Client optimizations to support blob increases](https://hackmd.io/@jimmygchen/H1EskpDRA), engine\_getBlobsV1 & IDONTWANT, followed by PeerDAS & ePBS

- Data Always: [case for increasing minimum blob base fee](https://ethresear.ch/t/understanding-minimum-blob-base-fees/20489) (EIP7762), makes blobspace market more responsive to demand

- Consensus-specs [v1.5.0-alpha.7](https://github.com/ethereum/consensus-specs/releases/tag/v1.5.0-alpha.7)

- [Weekly testing call #7](https://ethereum-magicians.org/t/pectra-testing-call-7-30-september-2024/21240)

[**Fusaka**](https://eips.ethereum.org/EIPS/eip-7607) **(Osaka + Fulu) upgrade**

- PeerDAS:
    - peerdas-devnet-2: launched but will need to be relaunched due to missing invalid sidecar check
    
    - [PeerDAS breakout #9](https://ethereum-magicians.org/t/peerdas-breakout-9-october-1-2024/21134): rebase on Pectra after pectra-devnet-4
    
    - [PeerDAS & distributed blob building](https://blog.sigmaprime.io/peerdas-distributed-blob-building.html): bottlenecks, optimizations, testing and impact on solo stakers

- [EOF implementers call #59](https://ethereum-magicians.org/t/eof-implementers-call-59-october-2-2024/21264): release tests on top of Prague broken, discussed migration to Osaka

[**Amsterdam**](https://eips.ethereum.org/EIPS/eip-7773) **upgrade**

- [Stateless implementers call #25](https://ethereum-magicians.org/t/stateless-implementers-call-24-september-23-2024/21154) (formerly Verkle): refining gas costs to support EIP7702, partial witness charging and devnet-7 coming soon starting with local testing

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.1%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~52% majority
    
    - Consensus layer: Prysm 37%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Layer 1**

- EIP7732 ePBS:
    - Potuz: [ePBS benefits](https://hackmd.io/@potuz/r1U45HEAR), lower CPU & bandwidth requirements, less missed attestations, less reorgs and no trusted intermediaries
    
    - [ePBS breakout #10](https://ethereum-magicians.org/t/epbs-breakout-10-september-27-2024/21156): steady progress by client teams, aiming for devnet before Devcon

- [IPv6 support by clients](https://ipv6eth.info/) dashboard: most clients can use dual stack, IPv6 not enabled by default

- Flashbots: [MEV searcher running in Intel TDX](https://collective.flashbots.net/t/searching-in-tdx/3902)

- Aestus Relay: [MEV-Boost timing games as a service](https://hackmd.io/@austonst-aestus/BJsvEoia6)

**For stakers**

- EthStaker: [solo staker bandwidth survey](https://poap-feedback.deform.cc/Solo-Staker-Bandwidth-Survey)

- [Contribute to Xatu data](https://ethpandaops.io/posts/contribute-to-xatu-data/) by running a xatu sentry sidecar on beacon node

**Research**

- [Fork-Choice enforced Inclusion Lists (FOCIL) workflow](https://ethresear.ch/t/focil-cl-el-workflow/20526): roles & duties of inclusion list committee members, nodes, proposers & attesters and edge case mitigations for equivocation, invalidation & inclusion list stuffing 

- Terence: [inclusion list out of protocol market risks](https://hackmd.io/@ttsao/il-market-risks)

- Proposal to [move state root to start of next block](https://ethresear.ch/t/proposal-delay-stateroot-reference-to-increase-throughput-and-reduce-latency/20490) to reduce latency & increase throughput

- [Tuyen optimization](https://ethresear.ch/t/attestation-verification-optimization/20516) to aggregate multiple attestations over the same message

**Client Releases**

- Consensus layer:
    - Nimbus [v24.9.0](https://github.com/status-im/nimbus-eth2/releases/tag/v24.9.0): adds support for additional beacon API endpoints and stability fixes

- Execution layer:
    - Erigon [v3.0.0-alpha4](https://github.com/erigontech/erigon/releases/tag/v3.0.0-alpha4): resync for better performance on chain-tip
    
    - Geth [v1.14.11](https://github.com/ethereum/go-ethereum/releases/tag/v1.14.11): new docker images; [v1.14.10](https://github.com/ethereum/go-ethereum/releases/tag/v1.14.10): hot fix for v1.14.9 blob pool regression
    
    - Reth [v1.0.8](https://github.com/paradigmxyz/reth/releases/tag/v1.0.8): ExEx support for experimental Engine API, RPC bug fixes & performance improvements

**Layer 2**

- Base [17 minute block building outage](https://base.mirror.xyz/TpAyBWKURrmafsXjANR1Gjn9Xqs_K2nV69xVT-XvLdA) on September 21 due to sequencer cluster misconfiguration

- Growthepie [L2 economics](https://www.growthepie.xyz/economics) dashboard: revenue, costs, profit/loss, margin & blob data used

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - Meta [EIP7773](https://eips.ethereum.org/EIPS/eip-7773): Hardfork Meta - Amsterdam
    
    - [EIP7775](https://github.com/ethereum/EIPs/pull/8914/files): BURN opcode
    
    - [EIP7778](https://eips.ethereum.org/EIPS/eip-7778): Prevent block gas smuggling

- ERCs (application layer):
    - [ERC7774](https://github.com/ethereum/ERCs/pull/652/files): Cache invalidation in ERC5219 mode web3 URL
    
    - [ERC7776](https://github.com/ethereum/ERCs/pull/659/files): Transparent financial statements
    
    - [ERC7777](https://github.com/ethereum/ERCs/pull/660/files): Governance for human robot societies
    
    - [ERC7779](https://github.com/ethereum/ERCs/pull/663/files): Interoperable delegated accounts
    
    - [ERC7780](https://github.com/ethereum/ERCs/pull/666/files): Validation module extension for ERC7579

**Stuff for developers**

- Foundry:
    - Forge-std [v1.9.3](https://github.com/foundry-rs/forge-std/releases/tag/v1.9.3): adds cheatcodes publicKeyP256, pause/resumeTracing, resetGasMetering, expectPartialRevert, setArbitraryStorage, copyStorage, mockFunction, assumeNoRevert, keyExists, getArtifactPathByCode/DeployedCode, parseTomlType, skip with reason and random bool/bytes/int/uint

- Hardhat [v2.22.12](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.22.12): ~10% performance improvement from internal Solidity tracing refactor

- [Solidity bugs viewer](https://00xsev.github.io/solidityBugsByVersion/) organized by version

- OpenZeppelin Contracts [v5.1.0-rc.0](https://github.com/OpenZeppelin/openzeppelin-contracts/releases/tag/v5.1.0-rc.0): reentrancy guard & ERC20 approval using transient storage, adds Errors, Hashes, Packing, Panic & SlotDerivation utilities, adds P256 & RSA cryptographic primitives and adds CircularBuffer, Heap & MerkleTree data structures

- Multiproof [v1](https://github.com/sigp/multiproof/releases/tag/v1.0.0) (Solidity library): generate Merkle proofs for testing in Foundry

- [Solgauss](https://github.com/cairoeth/solgauss#readme) (Solidity library): statistical functions rationally approximated, includes erfc, erfinv, erfcinv, ppf & and cdf

- [Viem-deal](https://github.com/Rubilmax/viem-deal#readme): deal ERC20 tokens by manipulating account balance with setStorageAt

- Halmos [v0.2](https://github.com/a16z/halmos/releases/tag/v0.2.0): expands focus to finding bugs & exploits, adds cheatcode to [generate calldata](https://x.com/daejunpark/status/1839053256175292713) and adds branching over symbolic call addresses

- Runtime Verification: [formal verification of loops](https://runtimeverification.com/blog/formally-verifying-loops-part-1)

- Patrick Collins: [flash loans guide](https://www.cyfrin.io/blog/flash-loans-everything-you-need-to-know)

- RareSkills: [common Solidity mistakes](https://www.rareskills.io/post/solidity-beginner-mistakes) by beginners

- CTFs:
    - Secureum RACE #33: [answers to 8 question Solidity quiz](https://ventral.digital/posts/2024/10/1/race-33-of-the-secureum-bootcamp-epoch-infinity/)

- Micro-eth-signer [v0.12.0](https://github.com/paulmillr/micro-eth-signer/releases/tag/0.12.0): adds EIP7702 and EIP7495 SSZ stable container support

- [Bashquiat](https://github.com/jrhea/bashquiat#readme) Discv5 in Bash

**Security**

- EF RFP: [Pectra system contracts audit wanted](https://github.com/ethereum/requests-for-proposals/blob/master/open-rfps/pectra-system-contracts-audit.md) for EIP2935, EIP7002 & EIP7251 

- Bedrock uniBTC [$2M exploit](https://mirror.xyz/0xF3c0C25090ae1458FC152947Aab57253cB8E0F0F/7dqKrAfS20rr3m_zuCwN80lChYTB0Cniie5IrdiC9ZQ) on 8 chains via minting using native tokens

- Onyx Protocol (Compound v2 fork) [$3.8M exploit](https://rekt.news/onyx-protocol-rekt2/) via unverified user input

- Shezmu [$4.9M exploit](https://rekt.news/shezmu-rekt/), funds recovered minus 20% bounty

- Banana Gun (Telegram trading bot) [$3M exploit](https://x.com/BananaGunBot/status/1838660010387116484)

- [Malicious VSCode Solidity extension](https://x.com/lehmannlorenz/status/1841545179825942991)

**Ecosystem**

- Vitalik: [legible Ethereum alignment](https://vitalik.eth.limo/general/2024/09/28/alignment.html) using metrics of open source, open standards, decentralization & security and positive sum

- [ETHGlobal Singapore](https://x.com/ETHGlobal/status/1837771164116263146) finalists

**Enterprise**

- [Visa tokenized asset platform](https://investor.visa.com/news/news-details/2024/Visa-Introduces-the-Visa-Tokenized-Asset-Platform/default.aspx): banks can issue fiat-backed stablecoins on public Ethereum, testing only this year, BBVA expected to have live pilots in 2025

- [PayPal paid EY invoice](https://archive.is/LuVIA) using PYUSD stablecoin via SAP’s digital currency hub

- [PayPal](https://newsroom.paypal-corp.com/2024-09-25-PayPal-Enables-Business-Accounts-to-Buy,-Hold-and-Sell-Cryptocurrency) enabled US business accounts to buy, hold, sell & transfer crypto

* * *

### Job Listings

- Sigma Prime is hiring Rust developers and security engineers. [Remote roles](https://github.com/sigp/positions-vacant)!

- [Status](https://status.app/) [free.technology](https://free.technology/) is hiring a [Business Developer](https://grnh.se/63f67b381us). More [jobs](https://free.technology/jobs) at IFT!

- Nethermind [InfoSec Head](https://job-boards.eu.greenhouse.io/nethermind/jobs/4371138101), [Sr Dev](https://job-boards.eu.greenhouse.io/nethermind/jobs/4387067101), [SRE Lead](https://job-boards.eu.greenhouse.io/nethermind/jobs/4390680101), [Sr Embedded Dev](https://job-boards.eu.greenhouse.io/nethermind/jobs/4391152101) & [UX UI designer](https://job-boards.eu.greenhouse.io/nethermind/jobs/4418511101)

- [Nomos](https://free.technology/nomos) is hiring [Ecosystem Developer](https://grnh.se/6a2297081us), [Rust Engineer](https://grnh.se/bd96340e1us) & [Applied Researcher](https://grnh.se/03fe75801us)!

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 2.5 to 76.7 gwei, 10.2 gwei average; zero net issuance at 24.3 gwei 
    
    - 11k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,316 - $2,701, currently $2,418, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.039 (Flippening at ~0.164)

**Notable at app layer**

- [Ethereum follow protocol](https://x.com/brantlymillegan/status/1838641601981329876) (onchain social graph) live: follow & tag accounts

- [Drakula](https://x.com/Drakulaapp/status/1841479778412462528) (iOS app): scrollable video feed, mint videos & trade memecoins on Base

- [ZKP2P Domains](https://domains.zkp2p.xyz/how-it-works): trade web2 domains registered with Namecheap

- [Azuki x Flashbots](https://x.com/hasufl/status/1841918806945681602): tokenized delegation to make single tweet using [Teleport](https://github.com/Account-Link/teleport-gramine-rs#readme)

- [Jelly Beans](https://jellybeans.wtf/): guess the number (or lower) for future onchain events to win OP

**Regulation/business/tokens**

- [Roman Storm motion to dismiss denied](https://x.com/valkenburgh/status/1841841346157359278), trial scheduled for December

- Inside [Biden destroying crypto-friendly banks](https://www.piratewires.com/p/inside-biden-admin-plot-to-destroy-silvergate-and-debank-crypto-for-good-nic-carter)

- US SEC [end of fiscal year](https://x.com/jchervinsky/status/1831404691215077757) actions:
    - [TrustToken & TrueCoin settled](https://www.sec.gov/newsroom/press-releases/2024-145) for sale of TUSD
    
    - [Mango settled](https://www.sec.gov/newsroom/press-releases/2024-154) for sale of MNGO tokens

- [UK Gambling Commission](https://www.gamblingcommission.gov.uk/news/article/consumer-information-notice-sorare-com-prosecution) prosecuting Sorare

**General**

- [Ethereum obituaries](https://ethereumobituaries.com/): all the times Eth declared dead since 2014

- KrebsOnSecurity: [Adam Iza allegedly bribed cops & stole from cybercriminals](https://krebsonsecurity.com/2024/09/crooked-cops-stolen-laptops-the-ghost-of-ugnazi/)

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-october-5-2024](https://weekinethereumnews.com/week-in-ethereum-news-october-5-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- **Oct 16 –** [**Gitcoin Grants 22**](https://grants.gitcoin.co/)**, OSS application deadline**

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- **Oct 25-27 –** [**ETHSydney**](https://2024.ethsydney.net/) **hackathon**

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

- Dec 6-8 – [ETHIndia](https://ethindia.co/) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

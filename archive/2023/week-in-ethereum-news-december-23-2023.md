---
title: "Week in Ethereum News <br> December 23, 2023"
date: "2023-12-22"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=7amkZxKobX4&t=312s). Recap by [Tim Beiko](https://mirror.xyz/abcoathup.eth/ERd6HNtS68D_zph_5nfkc9K5hsPW9e1KOqkpG60FosY).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1737834960881680800) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-177/):
    - **Testnet upgrade dates**: Goerli Jan 17 (epoch 231680), then assuming no issues, single client releases for Sepolia Jan 30 (epoch 132608) & Holešky Feb 7 (epoch 29696)
    
    - **Goerli shadow fork 1** [analysis](https://notes.ethereum.org/@ethpandaops/dencun-gsf-1-analysis): 290 nodes across 4 continents with all clients except Erigon; blobs increased network usage by ~200kbps & block latency by ~300ms
    
    - **Precompile address ranges:** upper half of range reserved for L2s
    
    - [**Prague/Electra planning**](https://ethereum-magicians.org/t/prague-electra-network-upgrade-meta-thread/16809): discussed potential small upgrade then Verkle-only upgrade

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.67%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~84% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm 41% & Lighthouse 34%, any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- EIP3074 (AUTH & AUTHCALL) [nonce proposal](https://github.com/ethereum/EIPs/pull/8050) to allow revocation

- Verkle implementers [call notes](https://twitter.com/rudolf6_/status/1737534896158253180)

- evmone [v0.11.0](https://github.com/ethereum/evmone/releases/tag/v0.11.0): full Cancun support

- Blocknative [transaction pool data archive](https://www.ethernow.xyz/mempool-data-archive), > 8TB of data, since November 2019

**MEV**

- PBS Foundation [pilot grants](https://pbsfoundation.notion.site/Launching-the-PBS-Foundation-Working-Together-to-Keep-Ethereum-s-Consensus-Layer-Decentralized-4cd7cb83907248b5ae8962d10eef0b70): infrastructure, research, data transparency & community education 

- [bloXroute MEV-Boost relays](https://twitter.com/bloxroutelabs/status/1736819783520092357) rejecting blocks with OFAC transactions

- MEV-Boost community [call notes](https://dataalways.mirror.xyz/-m0-bp3aZpcqa15_QbMX3MD1v9xg7VCcfGtZBR7I9Bg)

**For Stakers**

- [L1 & L2 (Base) node](https://twitter.com/ethereumonarm/status/1737409687358718304) on $189 ARM64 board, proof of concept

**Client releases**

- Consensus layer:
    - Lodestar [v1.13.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.13.0): logs info on connected service URLs, supports voluntary exits by remote signers and performance improvements
    
    - Teku [v23.12.1](https://github.com/Consensys/teku/releases/tag/23.12.1): fixes minor bugs in v23.12.0, validator client not compatible with Lighthouse beacon nodes

- Execution layer
    - Geth [v1.13.8](https://github.com/ethereum/go-ethereum/releases/tag/v1.13.8): hotfix for refusing to start after shutdown during sync; [v1.13.7](https://github.com/ethereum/go-ethereum/releases/tag/v1.13.7): eth\_sendTransaction RPC improved for low-fee txs; [v1.13.6](https://github.com/ethereum/go-ethereum/releases/tag/v1.13.6): faster gas estimation with 1.5% error ratio & non-deterministic and logging changed to slog (Go logging framework)

**Research**

- Timing games: [impact of intentional vs unintentional delays](https://ethresear.ch/t/empirical-analysis-of-the-impact-of-block-delays-on-the-consensus-layer/17888), validators needing longer signature times (e.g. DVT) won’t be able to play timing games as efficiently

**Layer 2**

- Arbitrum One [Sequencer downtime & L1 gas pricing issue](https://github.com/ArbitrumFoundation/docs/blob/50ee88b406e6e5f3866b32d147d05a6adb0ab50e/postmortems/15_Dec_2023.md) post-mortem

- L2Beat’s risk analysis [exit window](https://twitter.com/l2beat/status/1737823646108799250): available time to exit L2 before an upgrade is executed

- Gelato [rollup deployment platform](https://twitter.com/gelatonetwork/status/1737914982510023041): choose OP Stack or Polygon CDK

- Once an OG “ETH killer”: [Lisk](https://lisk.com/blog/posts/announcing-lisk-move-to-ethereum-ecosystem) plans migration to OP Stack rollup

- [Manta Pacific](https://mantanetwork.medium.com/manta-pacific-becomes-first-ethereum-l2-using-celestia-as-modular-da-d29cafc37cdd) stops publishing calldata to Ethereum; sidechain DA but done [with minimal security](https://twitter.com/donnoh_eth/status/1736792589741736290)

- [20% of mainnet gas](https://twitter.com/k06a/status/1736795024178733407) is now used for L2 data

**Stuff for developers**

- Hardhat [v2.19.3](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.19.3): Solidity v0.8.23 support

- Tip: [Solidity v0.8.13-21 via-IR code generator](https://twitter.com/paulrberg/status/1737169159052468479) can result in different but equivalent bytecode when using dependencies via symlinks, causing verification issues, fixed in v0.8.22

- [CreateX](https://twitter.com/pcaversaccio/status/1738153235678998855): contract deployer using CREATE/2/3, factory live on mainnet & L2s 

- [Vyper LSP](https://twitter.com/apeframework/status/1737609795148898647) (Language Server Protocol): errors/warnings, auto-complete, code navigation & hover-over info

- Ape [v0.7.0](https://twitter.com/ApeFramework/status/1737227442870251935): test account key pairs same HD path as Anvil/Hardhat and upgraded to Pydantic v2

- Guide to [decoding raw EVM calldata](https://jbecker.dev/research/decoding-raw-calldata)

- [Curta Golf](https://twitter.com/curta_ctf/status/1736167863000453270): gas optimization competition, Par NFT for valid entry, King NFT for most optimized

- Secureum
    - RACE #24: [12 question Solidity quiz & answers](https://docs.google.com/document/d/1PswXg-sc4Hy4YCGuTrwgZnXSEsfNZ_-rkiABw2ggOKc/edit)
    
    - RACE #0: [Solidity quiz explainers](https://www.youtube.com/playlist?list=PLq4UK_ZsMGQet4TwVQhL6UfwWtY86IWUD) \[videos\]

- [Stealth address (ERC5564) library](https://github.com/jsign/zig-stealth-addresses) implemented in Zig

- [Quint](https://github.com/informalsystems/quint): specification language based on TLA

- Kumavis: [LavaMoat (JavaScript supply chain security)](https://metamask.io/news/security/lavamoat-and-the-ledger-software-supply-chain-attack/) and the Ledger supply chain attack

**Security**

- NFT exploits:
    - NFT Trader (p2p trading) [exploit](https://twitter.com/0xCygaar/status/1736056050816876626) via reentrancy of older contracts, [some NFTs recovered](https://twitter.com/0xquit/status/1736268685579608142)
    
    - Flooring protocol (fractionalize NFTs) [exploit](https://twitter.com/FLC_FlooringLab/status/1736233859350667479) via external multicall

- [Audit Wizard](https://www.auditwizard.io/blog/auditing-with-poc-tests-in-audit-wizard) adds support to create/run Foundry tests for Proof of Concepts

**Ecosystem**

- [EF Q3 grantees](https://blog.ethereum.org/2023/12/19/esp-allocation-q323) share $9M in funding

- Etherscan [refresh NFT image & metadata](https://twitter.com/etherscan/status/1738147084153553342)

- [Inscriptions explainer](https://twitter.com/0xcygaar/status/1736581628259107314): tokens stored in low cost calldata with offchain indexers
    - Hildobby: [inscriptions dashboard](http://dune.com/hildobby/inscriptions), 90% of Goerli testnet gas this week

**Enterprise**

- EEA [Ethereum business readiness report](https://entethalliance.org/eea-ethereum-business-readiness-report-2023/)

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 20.1 to 289.8 gwei, with 47.7 gwei average
    - Zero net issuance currently at 21.9 gwei 
    
    - 19k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,131 - $2,342, currently $2,314

- [ETHBTC](https://ratiogang.com/): currently 0.053 (Flippening at ~0.16)

**Notable at app layer**

- Sablier [Airstreams](https://blog.sablier.com/introducing-airstreams/): vesting airdrops via token streams, supports up to 50k recipients

- 3cities [pay pages](https://twitter.com/3cities_xyz/status/1736157363667910780): payment to an address or ENS using mainnet & L2s 

- Protocol rewards: [Mirror](https://support.mirror.xyz/hc/en-us/articles/21917161046804-Mirror-s-Protocol-Rewards) & [Sound](https://sound.mirror.xyz/MegFCY1uOgDHMs3boM2y9udcbmMdmGPCr9LC2rMIS28) split fixed fees between creator, referrer & protocol

- Coordinape [CoLinks](https://twitter.com/coordinape/status/1736843220292612202) (Friend Tech fork) live on Optimism, professional social network

* * *

### Job Listings

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

**Job listings: $600 for four issues** (75 character limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [$78M raised for Fairshake super PAC in Q4](https://www.coinbase.com/blog/crypto-industry-donates-over-usd78-million-to-elect-pro-innovation) to support pro-crypto leaders in 2024 US elections

- [Congress of Mexico approves decentralized justice](https://twitter.com/Kleros_io/status/1736863867874017602) as alternative dispute resolution mechanism

**General**

- Rekt: [return of ape season](https://rekt.news/ape-season-returns/)

- [Ledger](https://twitter.com/Ledger/status/1737457365526470665) replacing blind signing by June 2024 with Clear Signing (centralized registry)

- [Fake Calendly site](https://twitter.com/BrantlyMillegan/status/1736925973507965021) asks to connect Twitter for account takeover

- Privacy & Scaling Explorations: [applied Fully Homomorphic Encryption](https://mirror.xyz/privacy-scaling-explorations.eth/D8UHFW1t48x2liWb5wuP6LDdCRbgUH_8vOFvA0tNDJA) (FHE)

- Trail of Bits: [Forbidden attack on AES-GCM in secure enclaves](https://blog.trailofbits.com/2023/12/18/a-trail-of-flipping-bits/) to extract ECDSA private key

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-23-2023](https://weekinethereumnews.com/week-in-ethereum-news-december-23-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jan 15 – EF’s [Next Billion fellowship cohort 4](https://fellowship.ethereum.foundation/) deadline

- **Jan 17 –** [**Goerli testnet**](https://github.com/ethereum/EIPs/pull/8051) **Dencun upgrade epoch 231680**

- **Jan 30 –** [**Sepolia testnet**](https://github.com/ethereum/EIPs/pull/8051) **Dencun upgrade epoch 132608 (assuming no issues)**

- Feb 2-4 – [ETH Cinco de Mayo](https://ethcincodemayo.com/) hackathon (Cholula, Puebla)

- Feb 3 – [Ethereum Lima Day](https://ethlimaday.org/)

- **Feb 7 –** [**Holešky testnet**](https://github.com/ethereum/EIPs/pull/8051) **Dencun upgrade epoch 29696 (assuming no issues)**

- Feb 23-Mar 3 – [ETHDenver](https://www.ethdenver.com/) BUIDLWeek & hackathon

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024)

- Mar 19-21 – [ETH Canal](http://ethcanal.xyz) (Panama City, Panamá) conference & hackathon

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) conference & hackathon

- Mar 29-31 – [ETH Seoul](https://www.ethseoul.org/)

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) (virtual)

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference & hackathon

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney)

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/)

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels)

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels)

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) (virtual)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024)

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024)

- Nov – [ETHGlobal DevCon](https://ethglobal.com/events/devcon2024)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

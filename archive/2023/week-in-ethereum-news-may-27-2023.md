---
title: "Week in Ethereum News <br> May 27, 2023"
date: "2023-05-27"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=jJvS6QjhPlM&t=7s). Summary by [Tim Beiko](https://twitter.com/abcoathup/status/1661875930376339456).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1661829680100691968) and [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-execution-call-162/):
    - [SELFDESTRUCT removal impact analysis](https://docs.google.com/document/d/1HDbym5YOoYj63xswMAwvt5Psh4JaI0biY06b6ZvYV2s/edit): EIP6780 (SELFDESTRUCT only in same tx) is low impact and will be in Cancun; EIP6913 SETCODE not in Cancun for now
    
    - EIP4844 discussions: excess\_data\_gas, use big endian for precompile, remove SSZ EIPs, draft devnet 6 spec (last EIP4844 specific devnet before Dencun devnets)
    
    - Proposed ordering of Cancun & Prague opcodes being added to execution specs
    
    - Final candidates for inclusion in Cancun: EIP4788 (beacon block root in EVM), EIP2537 (BLS precompile), EIP5656 (MCOPY), EIP5920 (PAY) & EIP7069 (revamped CALL instructions); no more EIPs to be considered for Cancun

- Consensus-specs [v1.4.0-alpha.0](https://github.com/ethereum/consensus-specs/releases/tag/v1.4.0-alpha.0): Deneb updates & attnets revamp

- [KZG ceremony](https://ceremony.ethereum.org/) nears 100k contributions, now available to accounts with [16 mainnet transactions](https://twitter.com/carlbeek/status/1661795909875924992)

**Layer 1**

- Ben Edgington: [deposits & withdrawals](https://eth2book.info/capella/part2/deposits-withdrawals/), new chapter from Upgrading Ethereum book

- Geth team: [what happens if a supermajority EL client has a bug](https://gist.github.com/holiman/4f6601018a8f559d7ce4cfe4e861cf73)?

- [Verkle overlay tree conversion method](https://twitter.com/gballet/status/1662046913259085824) implemented

**Client releases**

- Consensus layer:
    - Lighthouse [v4.2.0](https://github.com/sigp/lighthouse/releases/tag/v4.2.0): validator client faster to detect & avoid beacon nodes with offline execution layer
    
    - Prysm [v4.0.5](https://github.com/prysmaticlabs/prysm/releases/tag/v4.0.5): attestation aggregation improvements

- Execution layer:
    - Geth [v1.12.0](https://github.com/ethereum/go-ethereum/releases/tag/v1.12.0): PoW removed, GraphQL numeric values encoded as hex strings
    
    - Nethermind [v1.18.2](https://github.com/NethermindEth/nethermind/releases/tag/1.18.2): sync process accelerated

**For Stakers**

- Eth-wizard [v0.9.7](https://github.com/stake-house/eth-wizard/releases/tag/v0.9.7): validator setup on Ubuntu/Windows with MEV-Boost

**Research**

- [Path to enshrined Proposer-Builder Separation](https://ethresear.ch/t/why-enshrine-proposer-builder-separation-a-viable-path-to-epbs/15710): top-down via Two-Block HeadLock (variant of two-slot PBS) and bottom-up via optimistic relay

- [Timing games](https://arxiv.org/abs/2305.09032): proposer may delay block proposal to maximize MEV but still be early enough to be included

**Layer 2**

- [Distributed Sequencer Technology](https://figmentcapital.medium.com/distributed-sequencer-technology-a-path-to-decentralized-sequencing-549662cc9912): proposal for progressive decentralization of L2 sequencers using Distributed Validator Technology

- Layer N [zk fraud proofs](https://www.layern.com/blog/zkfp): hybrid approach only requires a proof to be generated when there is possibility of fraud

**EIPs/Standards**

- EIPs:
    - [EIP7069](https://github.com/ethereum/EIPs/pull/7069/files): Revamped CALL instructions

- ERCs:
    - [ERC7050](https://github.com/ethereum/EIPs/pull/7050/files): NFT creator provenance
    
    - [ERC7053](https://github.com/ethereum/EIPs/pull/7053/files): Interoperable digital media indexing
    
    - [ERC7066](https://github.com/ethereum/EIPs/pull/7066/files): ERC721 lockable

**Stuff for developers**

- OpenZeppelin Contracts [v4.9.0](https://blog.openzeppelin.com/introducing-openzeppelin-contracts-v4.9): Governor with Timestamps support for Optimism & Base, ERC4626 inflation attack protection, default admin rules for AccessControl, improved EIP712 signature interoperability via EIP-5267 and ERC777 deprecated

- [Solc contract metadata](https://www.rareskills.io/post/solidity-metadata) explainer: IPFS hash of JSON metadata + Solidity version

- Foundry:
    - Foundry [pre v1 update highlights](https://twitter.com/hievalir/status/1662171773973204993)
    
    - Forge-std [v1.5.6](https://github.com/foundry-rs/forge-std/releases/tag/v1.5.6): new cheatcodes and pure console log
    
    - tip: [console logging supports format specifiers](https://twitter.com/paulrberg/status/1660598958454865926) e.g. %s and %d

- abi-to-sol [v0.7](https://github.com/gnidan/abi-to-sol/releases/tag/v0.7.0): generate embeddable output (e.g. no pragma, no license identifier)

- Guide to [finding precision loss vulnerabilities](https://dacian.me/exploiting-precision-loss-via-fuzz-testing) using fuzz testing

- [Cicada](https://github.com/a16z/cicada#readme): private on-chain voting using homomorphic time-lock puzzles

- Vyper [v0.3.8](https://github.com/vyperlang/vyper/releases/tag/v0.3.8): transient storage keyword, ternary operators, raw\_revert builtin, shift operators, configurable send() gas stipend and use PUSH0

- Ape [v0.6.9](https://github.com/ApeWorX/ape/releases/tag/v0.6.9): easier testing via Pytest fixtures, Python v3.11 support and use\_network marker

- [Uniswap](https://twitter.com/uniswap/status/1661362297632088066) live on Sepolia testnet

- [enstate.rs](https://github.com/v3xlabs/enstate#readme): simultaneous ENS queries with caching, in Rust

- [Safer](https://github.com/morpho-labs/safer#readme): sign & submit transactions to a Safe multisig using Foundry scripts

- Curta CTF [Baby it’s me solution](https://twitter.com/popular_12345/status/1662174518696366080)

- [Code specification overview](https://twitter.com/SpearbitDAO/status/1661786772072804361): focus on plain english, state machines, diagramming, interfaces, placeholder tests and optionally formal definitions

- Echidna [v2.2.0](https://github.com/crytic/echidna/releases/tag/v2.2.0): multicore fuzzing & optimized coverage collection, up to 20x faster fuzzing

**Security**

- Tornado Cash [governance captured by attacker](https://github.com/coinspect/learn-evm-attacks/tree/master/test/Business_Logic/TornadoCash_Governance) using SELFDESTRUCT + CREATE2

**Ecosystem**

- Vitalik: [overloading Ethereum’s social consensus is high-risk](https://vitalik.ca/general/2023/05/21/dont_overload.html), app devs & Layer 2s need to find alternatives to achieve their security goals, there will be no bailouts

- Nick Fett: [restaking is overhyped](https://medium.com/@nfett/eigenlayer-crypto-rehypothecation-and-the-infinite-trust-machine-4e8164845b59) 

- Optimism’s [RetroPGF round 2 learnings](https://optimism.mirror.xyz/7v1DehEY3dpRcYFhqWrVNc9Qj94H2L976LKlWH1FX-8) 

- ETHDam [hackathon projects](https://taikai.network/cryptocanal/hackathons/ethdam/projects?filter_by=finalists)

- ETHGlobal [autonomous worlds hackathon finalists](https://twitter.com/ethglobal/status/1662142905048350724)

**Notable at app layer**

- Maker voting to [raise DSR to 3.33%](https://forum.makerdao.com/t/stability-scope-parameter-changes-2-non-scope-defined-parameter-changes-may-2023/20981)

- [Levon](https://medium.com/block-analitica/introducing-project-levon-e1444bd888d1): get a credit score for a Maker vault, beta

- Kain: [state of Synthetix](https://mirror.xyz/kain.eth/EB9DQldVEb0F74-LmrVau6YbjEtr8dsj1qVn6muYuXw)

- [TAI](https://mirror.xyz/0x01393d9b6dFFce134b6765e9bdd626b258357C37/7tghsnpqiCRKxS-5xbwPC7CPs2drbxWCR4GEZFhNWBY) (controlled peg stablecoin) live on mainnet

- [Astaria](https://astaria.xyz/) (NFT-backed lending) live on mainnet, beta

- [Safe multisig](https://twitter.com/safe/status/1660677975669633024) adds ERC1271 message signing support (used for OpenSea signing)

- [Utopia](https://twitter.com/utopialabs_/status/1661784971676381185): Safe multisig gasless swaps, beta

- [Flashbots Bundler](https://github.com/lcfr-eth/FlashbotsBundlerUI#readme): UI for token rescues from compromised addresses

* * *

### Job Listings

- [Protocol Engineer](https://github.com/tvl-labs/job-board/blob/main/engineering/protocol_engineer.md) (DeFi) sought by [Tunnel Vision Labs](https://tunnelvisionlabs.xyz/)

- Solidity team need a highly skilled [Developer Advocate](https://jobs.lever.co/ethereumfoundation/b9e33c9e-48ee-464f-a672-d51eece2b99d)

- Devconnect Istanbul: [Production Assistant](https://jobs.lever.co/ethereumfoundation/db6e2775-39d3-4eb9-9313-dfb15dfab9bc) and [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/401e0af5-f4a2-4e66-a724-4accb003113e)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US Fed](https://twitter.com/sebventures/status/1661063483369177108): 10% of adults used crypto in 2022

- Dan Elitzer: [DeFi primitives](https://www.nascent.xyz/idea/why-defi-is-broken-and-how-to-fix-it-pt-1-oracle-free-protocols) should have no governance, no upgradeability and no oracles

**General/crypto**

- Taylor warns of [targeted spearphishing](https://twitter.com/tayvano_/status/1661473965825740800)

- [KeePass vulnerability](https://github.com/vdohney/keepass-password-dumper#readme), master password can be retrieved from memory

- [Poseidon hash Merkle Trees](https://www.ulvetanna.io/news/poseidon-merkle-trees-in-hardware) implemented in FPGA hardware

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-may-27-2023](https://weekinethereumnews.com/week-in-ethereum-news-may-27-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jun 2-4 – [ETH Seoul](https://2023.ethseoul.org/)

- Jun 2-7 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 9-11 – [ETHPrague](https://ethprague.com/) conference & hackathon

- **Jun 22**–25 – [**Pragma Waterloo**](https://ethglobal.com/events/pragma-waterloo) & [ETHGlobal Waterloo](https://ethglobal.com/events/waterloo2023) hackathon

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

- Sep 18-21 – [ETH Montréal](https://ethmontreal.xyz/) hackathon & conference

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 6–27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 27–29 – [ETH Miami](https://ethmiami.net/) festival + hackathon

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://twitter.com/ethbrno/status/1652198745902137344)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 17-19 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

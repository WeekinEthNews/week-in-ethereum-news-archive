---
title: "Week in Ethereum News <br> May 13, 2023"
date: "2023-05-13"
---

## Eth News and Links

**Brief loss of finalization and first inactivity leak** 

- [Beacon chain stopped finalizing twice](https://ethstaker.notion.site/Finality-issue-updates-May-2023-3cb4d74e67c04d1f9ed31659e48c314b) over the past 36 hours and [had first inactivity leak](https://twitter.com/benjaminion_xyz/status/1657103592799588357)
    - [Consensus clients on lower spec hardware](https://twitter.com/potuz1/status/1657031082749861891) struggled to follow the chain after valid but untimely attestations were broadcast
    
    - Bottom line: blocks & transactions continued
    
    - For a short time, Ethereum devolved into the same probabilistic finality as PoW
    
    - Consensus client teams are working on patches
    
    - [Lighthouse overtook Prysm as majority consensus client](https://twitter.com/benjaminion_xyz/status/1656302859518869504), reminder: no client should have more than a 33% share, switch to a minority client

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=s6q5z53SICE&t=183s). [Summary](https://twitter.com/abcoathup/status/1656815791545933824) by Tim Beiko.  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1656693404808667138) and [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-execution-call-161/):
    - EIP4844: agreed to use big-endian for EL inputs/outputs and use RLP on EL & SSZ on CL via Engine API and discussion on state of KZG libraries
    
    - Meta discussion if Layer 2 focused EIPs need to go through core devs e.g. EIP6968
    
    - Cancun upgrade EIP candidates for inclusion to be discussed on next ACDE

- [KZG ceremony](https://ceremony.ethereum.org/) available to anyone with [32 mainnet transactions](https://twitter.com/CarlBeek/status/1655991868390539264). Wait time is generally zero.

**Layer 1**

- [MEV unbundling attack variant disclosed](https://lighthouse-blog.sigmaprime.io/mev-unbundling-rpc.html) with temporary mitigation

- Evmone [v0.10.0](https://github.com/ethereum/evmone/releases/tag/v0.10.0): Shanghai upgrade & EOF v1 support and performance improvements

- List of projects from the [third Ethereum Protocol Fellowship cohort](https://blog.ethereum.org/2023/05/10/ethereum-protocol-fellowship-third-recap)

**Client releases**

- Consensus layer:
    - Nimbus [v23.5.0](https://github.com/status-im/nimbus-eth2/releases/tag/v23.5.0): fixes missed block proposals when using an external builder in v23.4, experimental Web3Signer extension to verify block properties

**Research**

- Proposal to [consolidate large stakes into fewer validators](https://ethresear.ch/t/removing-unnecessary-stress-from-ethereums-p2p-network/15547) to reduce p2p messages

- [zkCasper](https://research.polytope.technology/zkcasper): verify Casper FFG consensus proofs using SNARKs, increases security of light clients

- [ArbiNet](https://ethresear.ch/t/a-research-on-mev-transaction-detection-using-graph-neural-networks/15553): MEV transaction detection using Graph Neural Networks

**Layer 2**

- Optimism [transaction delays postmortem](https://github.com/ethereum-optimism/optimism/blob/develop/technical-documents/postmortems/2023-04-26-transaction-delays.md)

**EIPs/Standards**

- EIPs:
    - [EIP6992](https://github.com/ethereum/EIPs/pull/6992/files): HTTP requests
    
    - [EIP7002](https://github.com/ethereum/EIPs/pull/7002/files): Execution layer triggerable exits

- ERCs:
    - [ERC6997](https://github.com/ethereum/EIPs/pull/6997/files): ERC721 with transaction validation step
    
    - [ERC7007](https://github.com/ethereum/EIPs/pull/7007/files): zkML AIGC-NFTs
    
    - [ERC7015](https://github.com/ethereum/EIPs/pull/7015/files): NFT authorship attribution
    
    - [ERC7017](https://github.com/ethereum/EIPs/pull/7017/files): Notification interface
    
    - [ERC7023](https://github.com/ethereum/EIPs/pull/7023/files): Automatic transaction representation

**Stuff for developers**

- Solidity [v0.8.20](https://blog.soliditylang.org/2023/05/10/solidity-0.8.20-release-announcement/): adds Shanghai support & sets Shanghai as default EVM version, experimental AST import via Standard JSON
    - [Change EVM version](https://twitter.com/msolomon44/status/1656411871635972096) when deploying Solidity v0.8.20+ to Layer 2 or other networks if they don’t support Shanghai

- Nomic Foundation [Slang](https://medium.com/nomic-foundation-blog/slang-alpha-release-6d322cf986a3) (Solidity compiler) alpha release, testers wanted

- Foundry:
    - [Pre v1.0 changes](https://github.com/foundry-rs/foundry/blob/master/CHANGELOG.md#pre-10)
    
    - [Etch cheat](https://twitter.com/bytes032/status/1656110114279915521) to debug deployed contract, add console.log & replace the code in a fork
    
    - Vulcan [v0.1](https://twitter.com/nomoixyz/status/1655670523269881872): dev framework for Foundry projects, aims for improved vm naming & test readability

- [pureConsole](https://twitter.com/devtooligan/status/1654945451584667648): Solidity library for console logging from pure functions

- [Protomerkle](https://github.com/hananbeer/protomerkle#readme): Solidity library to build onchain merkle trees

- [YulExp2Huff](https://github.com/PraneshASP/yul2huff#readme): convert Yul arithmetic expressions to Huff equivalent

- Wagmi [v1](https://twitter.com/wagmi_sh/status/1655993650621317149): uses viem (rather than ethers), reduced bundle size, prepare hooks not mandatory and deterministic errors; 

- RainbowKit [v1](https://github.com/rainbow-me/rainbowkit/releases/tag/%40rainbow-me%2Frainbowkit%401.0.0): supports wagmi v1 & viem, improved browser extension support

- [OpenZeppelin Contracts Wizard + Remix](https://twitter.com/loopifyyy/status/1654874026815225859) used to deploy a testnet memecoin in 27 seconds

- Coherent [mainnet dataset](https://coherent.xyz/blog/introducing-free-and-open-source-95-decoded-ethereum-datashares-and-sql-api-by-coherent): CC0, 95% decoded logs/txs/traces, via Snowflake or API

- [PGP onchain keyserver](https://ethereum-magicians.org/t/pretty-good-privacy-pgp-gpg-on-chain-keyserver/14158), concept

- [Dappnet](https://github.com/dappnetbby/dappnet#readme): portal for decentralized front ends, Chrome/Firefox/Brave on macOS, alpha

**Security**

- Immunefi: [unauthorized whitehat hacking is unethical](https://medium.com/immunefi/why-unauthorized-whitehacking-is-unethical-eb83347126ec)

**Ecosystem**

- [Validator exit queue](https://twitter.com/marceaueth/status/1655395351350657028) was emptied of everyone wanting to withdraw

- [Ether supply is down 100k ETH](https://twitter.com/ultrasoundmoney/status/1655254118779297793) in 30 days

- [Google search](https://twitter.com/nalin/status/1656753830862942208) for an address shows Ether balance, doesn’t support ENS yet  
    

**Enterprise**

- [EY OpsChain ESG](https://www.prnewswire.com/news-releases/ey-launches-ey-opschain-esg-to-provide-a-trusted-platform-for-emissions-and-carbon-credit-traceability-through-tokenization-301818831.html): tokenized CO2 emissions & carbon credits, beta

**Notable at app layer**

- Rune’s [Maker endgame roadmap](https://forum.makerdao.com/t/the-5-phases-of-endgame/20830): rebranding, new stablecoin & governance token (1:1200 ratio)

- Maker [Spark Protocol](https://twitter.com/makerdao/status/1655575088547127311): lend & borrow ETH, stETH, DAI & sDAI

- [Aragon Association](https://www.coindesk.com/business/2023/05/09/aragon-cancels-planned-community-control-of-200m-treasury-amid-battle-with-activist-investors/) refusing to transfer treasury to Aragon DAO

- [Cozy v2](https://mirror.xyz/cozy.eth/w24TU4ksefu7-jF1AGBrIbfeNKuZAH9v41aJw_VAr4g) (protection marketplace) live on Optimism, non-US, limited to $5M per protection set

- [Ethereum Attestation Service](https://twitter.com/eas_eth/status/1654957376473272322?s=20): attest & verify a file

- [Tessera](https://twitter.com/andy8052/status/1657031015066394630) (formerly Fractional) winding down

- Karma [delegate activity tracker](https://twitter.com/karmahq_/status/1656322134439002114) to check DAO delegate performance

* * *

### Job Listings

- [Snr React Native UI Dev](https://grnh.se/2fada6031us) at Status: [All jobs](https://grnh.se/9fc6e6fc1us)

- Solidity team need a highly skilled [Developer Advocate](https://jobs.lever.co/ethereumfoundation/b9e33c9e-48ee-464f-a672-d51eece2b99d)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US Chamber of Commerce amicus brief](https://twitter.com/MetaLawMan/status/1656737447756038177) in Coinbase SEC case

- [Biden gaslights](https://twitter.com/POTUS/status/1655988502079602690) that there is a special tax loophole for crypto

- [Former Coinbase product manager sentenced](https://www.justice.gov/usao-sdny/pr/former-coinbase-insider-sentenced-first-ever-cryptocurrency-insider-trading-case) to 2 years jail in insider trading case

- [IRS $44 billion claims](https://www.coindesk.com/business/2023/05/10/us-internal-revenue-service-files-claims-worth-44-billion-against-ftx-bankruptcy/) on FTX entities

**General/crypto**

- [Pseudorandom functions & permutations](https://blog.cryptographyengineering.com/2023/05/08/prfs-prps-and-other-fantastic-things/) explainer

- [MSI private keys published by hackers](https://www.techspot.com/news/98612-hackers-publish-msi-private-keys-enabling-signed-malware.html), could be used to to sign malware

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-may-13-2023](https://weekinethereumnews.com/week-in-ethereum-news-may-13-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- May 19-23 – [EDCON](https://edcon.io/) Montenegro

- May 20-21 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 24-26 – [Spaghett ETH](https://naples.spaghett-eth.com/) (Naples) conference

- May 26-28 – [ETHDublin](https://www.ethdublin.io/) hackathon

- Jun 2-4 – [ETH Seoul](https://2023.ethseoul.org/)

- Jun 2-7 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 9-11 – [ETHPrague](https://ethprague.com/) conference & hackathon

- Jun 23–25 – [ETHGlobal Waterloo](https://ethglobal.com/events/waterloo2023) (changed from Toronto)

- **Jul 5-9 –** [**ETHBarcelona**](https://ethbarcelona.com/) **conference & hackathon**

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- **Aug 15-16** – [ETHToronto](https://www.ethtoronto.ca/) & [ETHWomen](https://www.ethwomen.com/)

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

- Oct 6–27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 27–29 – [ETH Miami](https://ethmiami.net/) festival + hackathon

- **Nov 3-5** – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://twitter.com/ethbrno/status/1652198745902137344)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 17-19 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

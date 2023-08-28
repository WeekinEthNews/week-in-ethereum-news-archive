---
title: "Week in Ethereum News <br> August 26, 2023"
date: "2023-08-26"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=RysjOBGRDDg&t=52s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-116/):
    - Dencun [testing overview](https://notes.ethereum.org/@ethpandaops/dencun-testing-overview)
    
    - Timelines for a short lived devnet 9 & upgrading public testnets to be discussed on next ACDE call

- [KZG Ceremony](https://twitter.com/CarlBeek/status/1694566774375698789) finished with 141,416 contributions, largest ceremony ever

**Layer 1**

- Holešky testnet (Goerli replacement)
    - [Genesis file generated](https://twitter.com/parithosh_j/status/1694041437300535399), launches September 15 with 1.46M validators
    
    - ACDC agreed to change Shapella upgrade to epoch 256, validator ejection balance to 28 hETH and support compressed genesis state

- Dapplion: [Whisk (SSLE) expensive duty discovery](https://hackmd.io/@dapplion/expensive_duty_discovery) can be solved using a validator’s public key

**For stakers**

- [Geth still supermajority EL client](https://twitter.com/hanni_abu/status/1694300131598680292) based on self-reported data from large pools & entities

- [Siren v1](https://lighthouse-blog.sigmaprime.io/Siren.html) (Lighthouse's validator management UI): monitor node & validator health 

**Client releases**

- Consensus layer:
    - Nimbus [v23.8.0](https://github.com/status-im/nimbus-eth2/releases/tag/v23.8.0): performance & stability improvements
    
    - Prysm [v4.0.8](https://github.com/prysmaticlabs/prysm/releases/tag/v4.0.8): reduce memory usage

- Execution layer:
    - Besu [v23.7.1](https://github.com/hyperledger/besu/releases/tag/23.7.1): performance & stability improvements, updated dependencies and extended functionality of EVM tool & RPC trace modules
    
    - Reth [v0.1.0-alpha.7](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.7): fixes for crawlers reaching nodes, RPC & txpool and rudimentary eth\_getProof support for accounts

**Research**

- [Super-finality](https://ethresear.ch/t/super-finality-high-safety-confirmation-for-casper/16429) confirmation rule for Casper, can implement client-side/wallets using Beacon API

- [Proof of Validator](https://ethresear.ch/t/proof-of-validator-a-simple-anonymous-credential-scheme-for-ethereums-dht/16454): anonymous credential scheme for Distributed Hash Table participants

**Layer 2**

- RISC Zero [Zeth](https://www.risczero.com/news/zeth-release): zk block prover based on revm

- [Base](https://base.mirror.xyz/aBwt4flT1WAKJGQTj2AXBpH_8Qd3umQ-ZECLAJoO_nE) uses 2/2 upgrade multisig (Optimism Foundation & Base)
    - Coinbase will contribute minimum 2.5% of Base sequencer revenue to Optimism Collective for RetroPGF & ecosystem projects 
    
    - [Optimism](https://optimism.mirror.xyz/Luegue9qIbTO_NZlNVOsj25O1k4NBNKkNadp2d0MsTI?a) granting up to ~118M OP tokens (2.7% of supply) over 6 years to Coinbase

**EIPs/Standards**

- Updated [EIP editor handbook](https://eips.ethereum.org/EIPS/eip-5069) (EIP5069)

- ERCs (application layer):
    - [ERC7502](https://github.com/ethereum/EIPs/pull/7502/files): Self tradable NFT
    
    - [ERC7503](https://github.com/ethereum/EIPs/pull/7522/files): Zero-knowledge wormholes
    
    - [ERC7504](https://github.com/ethereum/EIPs/pull/7523/files): Dynamic contracts (one-to-many proxy contracts)

* * *

### **The Tornado Cash devs helped bring privacy to Ethereum. In return, the US federal government is trying to put them in jail**

![Web3 Builders](https://weekinethereumnews.com/wp-content/uploads/2023/08/Web3-Builders.webp)

Watch [Ameen Soleimani discuss the injustice of the US federal charges brought against Roman Storm and Roman Semenov](https://www.youtube.com/watch?v=GsMpdDzCNnM) for writing open source code.  (Or [listen](https://open.spotify.com/show/6eV2i8BgtnL002ZO7fUzp5))

Donate to the [legal defense fund](https://donate.peppersec.com/). (KYC required)

* * *

**Stuff for developers**

- Foundry:
    - Vulcan [v0.2.0](https://twitter.com/nomoixyz/status/1694421244798460067) (dev framework): adds gas estimation and deployment address calculation
    
    - [Cast rpc with jwt secret](https://twitter.com/rjected/status/1694072110971248666) allows Engine API calls to EL

- [Full Stack dapp workshop](https://github.com/kmjones1979/full-stack-dapp-workshop#readme) using ScaffoldETH-2 and The Graph

- Ape Framework [code coverage](https://mirror.xyz/apeworx.eth/gCGyXvzzwbTOLnr7rUzXPWFWkCVDjMs1haOcIj0Q2Hc) guide

- [Ape-hackathon-kit](https://github.com/wolovim/ape-hackathon-kit#readme): develop contracts in Ape framework and web apps in Next.js, Tailwind, RainbowKit & wagmi

- WhatsABI [v0.8.0](https://github.com/shazow/whatsabi/releases/tag/v0.8.0) (guesses ABI from bytecode): tested with ethers.js v5/6 & viem, bundle size reduced to 12KB

- TrueBlocks [v1](https://github.com/TrueBlocks/trueblocks-core/releases/tag/v1.0.0-release) and [EF grant report](https://tjayrush.medium.com/trueblocks-final-report-for-ef-grant-d784653c830d)

- tx2uml [v1.1.23](https://twitter.com/naddison/status/1693512699249086702): adds options to hide parameter names/values in trace; [v1.1.24](https://github.com/naddison36/tx2uml/releases/tag/v1.1.24) supports Base

- wagmi [mipd](https://github.com/wagmi-dev/mipd#readme): TypeScript utilities for ERC6963 (Multi Injected Provider Discovery)

- CTFs:
    - Curta CTF: [devtooligan’s Elohim solution](https://twitter.com/devtooligan/status/1694746398326128777)
    
    - [Paradigm CTF](https://ctf.paradigm.xyz/) October 28-30

- [Cryogen](https://github.com/banteg/cryogen#readme): consolidate parquets into larger chunks for smaller datasets & faster queries

**Security**

- [Balancer v2 pools vulnerability disclosed](https://twitter.com/balancer/status/1694014645378724280), withdraw affected LPs

**Ecosystem**

- [Danny Ryan](https://twitter.com/dannyryan/status/1694709761412087989) rebuts [Lido’s claim that dual governance](https://hackmd.io/@sacha/on-the-risks-of-lsd) mitigates risks to Ethereum as Lido nears 33% of stake

- Hackathon projects: [ETHToronto](https://dorahacks.io/hackathon/ethtoronto2023/buidl), [ETHWomen](https://dorahacks.io/hackathon/ethwomen/buidl) and [Ethereum Argentina](https://taikai.network/ethargentina/hackathons/buildathon-2023/projects)

- Etherscan [search bar shortcut](https://twitter.com/etherscan/status/1695031093043626181): press “/”

**Notable at app layer**

- Privacy & Scaling Explorations [Bandada v1](https://mirror.xyz/privacy-scaling-explorations.eth/p3Mtft28FG1ctgeUARVEKLTK_KexnWC6T4CUHaQark4): create/manage privacy-preserving groups of anons

- ScopeLift: [DAO voting from Layer 2 with flexible voting](https://www.scopelift.co/blog/dao-voting-from-layer-2-with-flexible-voting), proof of concept

- Base apps:
    - [Friend Tech](https://twitter.com/friendtech/status/1694880415318954358) adds photo sharing with key holders
    
    - [StoryBase](https://www.storybase.xyz/): fee per character collaborative writing, snippets minted as NFTs
    
    - Parody [bike race](https://citibike.xyz/frequently-asked-questions.html): mint/steal NFTs of NYC Citi Bikes in 10 day race

* * *

### Job Listings

- EF Privacy & Scaling Explorations team seek [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4)

**Job listings: $600 for four issues** (75 character limit).  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Roman Semenov & Roman Storm (Tornado Cash co-founders) unjustly charged](https://www.justice.gov/usao-sdny/pr/tornado-cash-founders-charged-money-laundering-and-sanctions-violations) with conspiracy to launder money because they wrote open source code:
    - Roman Storm arrested and [out on bail](https://twitter.com/brianeklein/status/1694779420731658700).
    
    - [OFAC](https://home.treasury.gov/news/press-releases/jy1702) sanctioned Roman Semenov
    
    - Donate to [legal defense fund](https://donate.peppersec.com/). (KYC required)
    
    - web3 Builders: [interview with Ameen Soleimani](https://www.youtube.com/watch?v=GsMpdDzCNnM) about the charges

- [Nate Chastain](https://www.justice.gov/usao-sdny/pr/former-employee-nft-marketplace-sentenced-prison-first-ever-digital-asset-insider) sentenced to 3 months jail, $50k fine + proceeds for OpenSea insider trading

- [Bitstamp ending Ethereum staking](https://www.coindesk.com/policy/2023/08/24/bitstamp-to-stop-ether-staking-in-us-amid-regulatory-scrutiny/) for US customers

- [USDC changes](https://www.coinbase.com/blog/ushering-in-the-next-chapter-for-usdc): Circle to control issuance & Coinbase taking equity stake in Circle

- [Proposed draconian US tax rules](https://home.treasury.gov/news/press-releases/jy1705) would require KYC for most blockchain transfers and blocking US citizens from nearly everything, comments open until October 30

**General**

- BlockFi, FTX & Genesis [bankruptcy claimants data stolen from Kroll](https://www.kroll.com/en/about-us/news/security-incident) via T-Mobile SIM swap

- MACI v1 [trusted setup ceremony](https://ceremony.pse.dev/projects/Maci%20v1%20Trusted%20Setup%20Ceremony)

- Arnaucube: [intuition for ProtoGalaxy](https://arnaucube.com/blog/protogalaxy.html) folding scheme

- [Soundness notions for Interactive Oracle Proofs](https://eprint.iacr.org/2023/1256) (IOPs)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-26-2023](https://weekinethereumnews.com/week-in-ethereum-news-august-26-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 29 – [Gitcoin Grants 18](https://grants.gitcoin.co/) ends (support [Week in Ethereum News](https://explorer.gitcoin.co/#/round/10/0x2871742b184633f8dc8546c6301cbc209945033e/0x2871742b184633f8dc8546c6301cbc209945033e-122))

- Aug 31 - Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 7-9 – [ETHAccra](https://www.ethaccra.xyz/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 15-17 – [ETHChicago](https://www.ethchicago.xyz/) conference & hackathon

- **Sep 15 –** [**Holešky testnet**](https://github.com/eth-clients/holesky#readme) **genesis**

- Sep 18-24 – [ETHSafari](https://ethsafari.xyz/) (Kilifi Kenya)

- Sep 21–24 – [Pragma](https://ethglobal.com/events/pragma-newyork) & [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 6-27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- **Oct 28-30 –** [**Paradigm CTF**](https://ctf.paradigm.xyz/)

- Oct 13-15 – [Ethereum Kuala Lumpur](https://hack.ethkl.org/) conference & hackathon

- Oct 21 – [Ethereum México](https://twitter.com/ethereum_mexico/status/1684649652639924224)

- Oct 22-24 – [ETH Hong Kong](https://www.ethhongkong.co/)

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Oct 27-29 – [ETH Vietnam](https://www.eth-vietnam.com/)

- Oct 27-29 – [ETH London](https://www.encode.club/eth-london) hackathon

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) deadline (max $1k for local meetups)

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://lu.ma/ethbrno3)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 16-19 – [Pragma](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- **Dec 4-5 –** [**ETHVenice**](https://ethvenice.com/)

- **Dec 8-10 – ETHGlobal** [**ETHIndia**](https://ethindia.co/) **(Bangalore)** 

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

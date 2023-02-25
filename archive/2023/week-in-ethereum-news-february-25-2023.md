---
title: "Week in Ethereum News <br> February 25, 2023"
date: "2023-02-25"
---

## **Eth News and Links**

**Shapella (Shanghai + Capella) upgrade**

- Sepolia testnet [upgrades to Shapella February 28](https://github.com/ethereum/execution-specs/blob/master/network-upgrades/mainnet-upgrades/shanghai.md#upgrade-schedule)

- Consensus layer Sepolia releases:
    - Lighthouse [v3.5.0](https://github.com/sigp/lighthouse/releases/tag/v3.5.0)
    
    - Lodestar [v1.5.0-rc.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.5.0-rc.0)
    
    - Nimbus [v23.2.0](https://github.com/status-im/nimbus-eth2/releases/tag/v23.2.0)
    
    - Prysm [v3.2.1](https://github.com/prysmaticlabs/prysm/releases/tag/v3.2.1)
    
    - Teku [v23.2.0](https://github.com/ConsenSys/teku/releases/tag/23.2.0)

- Execution layer Sepolia releases:
    - Besu [v23.1.1-RC1](https://github.com/hyperledger/besu/releases/tag/23.1.1-RC1)
    
    - Ethereum JS [v0.7](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs%2Fclient%400.7.0)
    
    - Erigon [v2.39.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.39.0)
    
    - Geth [v1.11.2](https://github.com/ethereum/go-ethereum/releases/tag/v1.11.2)
    
    - Nethermind [v1.17.0](https://github.com/NethermindEth/nethermind/releases/tag/1.17.0)

- EF blog post for [Sepolia upgrade to Shapella](https://blog.ethereum.org/2023/02/21/sepolia-shapella-announcement)

- consensus-specs [v1.3.0-rc.3](https://github.com/ethereum/consensus-specs/releases/tag/v1.3.0-rc.3): adds test for validator deposit & BLS change in one block, frees EIP4844 blobs from blocks and adds KZG API

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=io7ALEfxJsE&t=722s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/r1ucJgrCo) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-consensus-call-103/):
    - circuit breaker (fallback to local building) tested using mock builder in Hive tests
    
    - MEV-Boost running successfully on Zhejiang testnet
    
    - SSE discussion so any client (rather than just Prysm fork) can trigger block building

- Flashbots: [MEV-Boost stack changes for Capella](https://flashbots.notion.site/MEV-Boost-Capella-Upgrades-00cea01704794f6eb4f792c55b69c441)

**Dencun (Cancun + Deneb) upgrade**

- KZG Ceremony:
    - [54,000+ contributors](https://ceremony.ethereum.org/), 4000+ in the lobby, 16 days left in _first_ general contribution period

- Latest EIP4844 implementers [call video](https://www.youtube.com/watch?v=hWcpSlwNTBU&t=3s). Notes from [Terence](https://twitter.com/terencechain/status/1628095926127702017): client teams freeing blobs from blocks, devnet expected in a few weeks once decoupled

**Layer 1**

- [Visualization of withdrawal credentials](https://twitter.com/Data_Always/status/1629210968025714690) (0x00 vs 0x01) over time

- [Beverly Hills](https://twitter.com/jasoriatanishq/status/1627692040015478785) (Verkle tree) testnet is now multi-client, Nethermind synced along with Geth

- Reth (execution client) [modular p2p architecture](https://fiber.chainbound.io/blog/reth-p2p/) can be used as standalone component

**Research**

- [Recent Latest Message Driven GHOST](https://twitter.com/luca_zanolini/status/1628702750392344577): synchronous dynamically available & resilient to bounded asynchronous periods, proposed replacement for Gasper’s LMD-GHOST

**For Stakers**

- Superphiz: [best practices to avoid getting slashed](https://twitter.com/superphiz/status/1628403796442329088) (only 226 validators have been slashed)

- [Stake Local dashboard](https://docs.stakelocal.io/): multi-client Grafana dashboard

- [Beaconcha.in explorer](https://twitter.com/butta_eth/status/1628117713523511296) adds BLS change signature & broadcast of voluntary exits for Zhejiang testnet

- [Obol running distributed validator on mainnet](https://blog.obol.tech/road-to-mainnet-and-beyond-for-distributed-validators/) with 98.6% average effectiveness

**Layer 2**

- [Arbitrum One](https://twitter.com/l2beat/status/1628356180769636353) tops Ethereum mainnet in transactions, first rollup to achieve more transactions in a day than mainnet

- [Base](https://base.mirror.xyz/jjQnUq_UNTQOk7psnGBFOsShi7FlrRp8xevQUipG_Gk): Coinbase layer 2 built on Optimism’s OP Stack, live on testnet, transaction fees paid in ETH with a portion of sequencer revenue going to funding public goods

- Optimism’s [Superchain concept](https://stack.optimism.io/docs/understand/explainer/): network of OP Chains with shared bridge & communication layer

- Patrick McCorry: [rollup transaction finality](https://stonecoldpat.substack.com/p/tiers-of-transaction-finality-for): sequencer’s promise, order finality and execution settlement 

**EIPs/Standards**

- New [EIP core & ERC editors](https://twitter.com/EthCatHerders/status/1628380724406456326)

- ERCs:
    - [ERC6538](https://eips.ethereum.org/EIPS/eip-6538): Stealth meta-address registry
    
    - [ERC6551](https://eips.ethereum.org/EIPS/eip-6551): NFT bound accounts

* * *

### **This newsletter is made possible thanks to** [**Mimic**](https://mimic.fi/)**!**

![mimic](https://weekinethereumnews.com/wp-content/uploads/2022/10/mimic-banner-1024x427.png)

Does your _app_ or _DAO_ want to automate your DeFi operations?  With Mimic, you can **automate swapping, bridging and treasury management**.

Check out our [Smart Vaults](https://medium.com/mimicfi/introducing-smart-vaults-3438bacc843d) to automate DeFi operations in a secure, trustless, and non-custodial way.

We’ll be at EthDenver if you want to [request a demo](https://airtable.com/shrSvH8fTJcbHq0xl) IRL. _Backed by Starbloom Ventures_.

* * *

**Stuff for developers**

- Solidity [v0.8.19](https://blog.soliditylang.org/2023/02/22/solidity-0.8.19-release-announcement/): adds [operators for user-defined value types](https://blog.soliditylang.org/2023/02/22/user-defined-operators/) and fix for deployment bloat (code only used in creation code was included in runtime bytecode) 

- Solidity proposals for [improving try/catch](https://forum.soliditylang.org/t/call-for-feedback-the-future-of-try-catch-in-solidity/1497), feedback wanted

- Foundry:
    - [configure SMTChecker](https://twitter.com/paulrberg/status/1627654614811115520)
    
    - [Testnet.fyi](https://twitter.com/emilianobonassi/status/1629133975091572743): short lived serverless testnet as a service using Anvil & AWS, proof of concept

- [Statistical approximation](https://www.primitive.xyz/posts/solstat) in Solidity

- [AztecConnectAuction](https://a16zcrypto.com/through-the-looking-glass-a-cross-chain-sealed-bid-auction-using-aztec-connect/): cross-chain sealed-bid auction using Aztec Connect

- [Solidity external library](https://twitter.com/real_philogy/status/1625649928901992451) cost Blur airdrop claimers $34k, internal would have saved ~2600 gas each

- Huffmate [v1.1](https://github.com/pentagonxyz/huffmate/pull/72) (contract library in Huff): SendEthers utility, ECDSA & BytesLib implementation

- [EVM disassembly guide](https://karmacoma.notion.site/Building-reliable-EVM-disassemblers-ecf689d965cc4ffc9c3b2e34f4227b46): navigating metadata & why bytecode 6142 breaks most disassemblers

- sol2uml [v2.5.0](https://twitter.com/naddison/status/1627551722150432768): storage variables are parsed in contract storage diagrams

- [ContractReader.io](https://twitter.com/backseats_eth/status/1629203031584800768) adds live inline values

- Seaport [v1.4](https://twitter.com/z0age/status/1627848957396422656): fix for v1.3 so zone & contract offerer checks applied after transfers

- Alchemy [Create Web3 Dapp](https://www.alchemy.com/create-web3-dapp): NextJs based starter kit with components & templates

- [Emojimon](https://mud.dev/tutorials/emojimon/): guide to create Pokémon-inspired on-chain game using MUD stack

- EKO2022 CTF [Phoenixtto solution](https://stermi.xyz/blog/eko2022-ctf-phoenixtto-solution)

- Ethernaut CTF [solutions in Huff](https://github.com/0xJCN/Ethernaut-CTF#readme) (added to solutions in Vyper)

- Gitcoin Passport [Scorer API](https://twitter.com/gitcoinpassport/status/1627716829446832128): gate apps based on passport score

- [SuperNova](https://github.com/jules/supernova#readme) implementation in Rust, experimental

**Security**

- [Oasis multisig upgraded a contract](https://www.blockworksresearch.com/research/we-do-a-little-counter-exploit) to recover funds from Wormhole exploiter [based on UK court order](https://blog.oasis.app/statement-regarding-the-transactions-from-the-oasis-multisig-on-21st-feb-2023/)

**Ecosystem**

- Danny Ryan’s [reflections on the state of Ethereum](https://github.com/djrtwo/writing/blob/main/docs/2023-02-23_2023-Reflections.md): technological concerns, execution layer client diversity, core dev incentives, capture, ossification and L2 alignment

- Tim Beiko: [testnet past, present & future](https://twitter.com/timbeiko/status/1628819200696516608):
    - Goerli: test validator setups, [EthStaker](https://goerli.launchpad.ethstaker.cc/en/) offer low Goerli ETH deposits, deprecated
    
    - Holešovice: planned for later this year as replacement for Goerli
    
    - Sepolia: test apps, no supply issues as [Sepolia ETH supply can be inflated](https://github.com/eth-clients/merge-testnets/pull/14#issuecomment-1152570001)
    
    - [Ephemery](https://ephemery.pk910.de/): test validator setups on ephemeral testnet

- [EF Q4 grantees](https://blog.ethereum.org/2023/02/22/allocation-update-q4-22) share $4.4million in funding

- [MetaMask](https://docs.metamask.io/guide/signing-data.html#signing-data) disabling eth\_sign RPC signature method by default

**Enterprise**

- [Spotify pilots NFT gated playlists](https://www.coindesk.com/web3/2023/02/23/spotify-is-testing-token-enabled-music-playlists/) on Android in selected countries

**Application layer**

- [Synthetix v3](https://blog.synthetix.io/synthetix-v3-is-on-mainnet/) deployed on mainnet & Optimism

- [Aave voted](https://snapshot.org/#/aave.eth/proposal/0x7fe7d372601aa2864cbe21071bd2fda10bf22aa8f66076db276818a2d6808bef) to freeze BUSD reserve on v2

- [ENS ETHDenver custom sticker pack](https://twitter.com/ensdomains/status/1627714810568912897) pre-register and set your avatar

- NFT marketplace wars:
    - [Blur NFT trading volume](https://twitter.com/poof_eth/status/1628452399315550208): 20% from 15 wallets, 50% from ~300 wallets
    
    - [125k ETH NFT wash trade](https://old.reddit.com/r/ethfinance/comments/117w2io/daily_general_discussion_february_21_2023/j9egih2/) (0% marketplace fee) via flash loan
    
    - [Uniswap](https://twitter.com/uniswap/status/1628396162423160839): use any ERC20 token to buy NFTs
    
    - Dankrad Feist’s explainer for creators: [NFT contracts can’t enforce royalties](https://twitter.com/dankrad/status/1627312777600593923)

- [Ethereum Postal Service](https://github.com/EthereumPostalService/eps-core#readme): send physical letters via a contract call (but don’t dox anyone)

- Backed [bCOIN](https://twitter.com/BackedFi/status/1629134151658905600) tokenized tracker of Coinbase COIN, non-US qualified investors only 

* * *

### Job Listings

- Frax Finance is expanding their official core developer team. [Apply here!](https://docs.google.com/forms/d/e/1FAIpQLSem7KL-FFgsuxaUMww4OXMxdJ-qXfyWJ_IvGdqVteBSM5FgxA/viewform)

- Immutable is hiring a [Protocol Blockchain Engineer](https://jobs.lever.co/immutable/03e6848f-6cc7-4295-a162-7910b0368c4d).

- [Cyfrin.io](https://www.cyfrin.io/) is hiring [senior security engineers](https://github.com/ChainAccelOrg/SecurityEngineerReq) $190k-$300k.

- [Request Network](https://request.network/en/) is hiring a [Community & Communication Manager](https://jobs.lever.co/request/76d0db8a-06bc-42c9-9816-69317c5f8c99)

- Shell Protocol team is hiring [senior Solidity devs & more](https://shellprotocol.io/posts/now-hiring-for-shell-protocol/), remote or Hawaii

- Certora is hiring a [Senior Enterprise Sales Rep](https://www.certora.com/#careers).

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US regulators guidance for banks](https://www.federalreserve.gov/newsevents/pressreleases/bcreg20230223a.htm) on liquidity risks from crypto entities

- [FTX Japan](https://help-jp.ftx.com/hc/ja/articles/15765489546393) reopens withdrawals

- [Forsage founders charged with fraud](https://www.justice.gov/opa/pr/forsage-founders-indicted-340m-defi-crypto-scheme) in Ponzi scheme

- Jon Charbonneau: [how value flows through Ethereum and why issuance is misunderstood](https://joncharbonneau.substack.com/p/eth-is-not-ultrasound-money-part)

**General/crypto**

- Coinbase: [lessons to learn from social engineering attack](https://www.coinbase.com/blog/social-engineering-a-coinbase-case-study)

- Trail of Bits: [VSCode extensions](https://blog.trailofbits.com/2023/02/21/vscode-extension-escape-vulnerability/) & [VSCode](https://blog.trailofbits.com/) vulnerabilities disclosed

- [Static analysis detectors](https://eprint.iacr.org/2023/190) for common vulnerabilities in Circom programs

- [wienr](https://github.com/zach-is-my-name/wiener#readme): CLI reader for Week in Ethereum News

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-february-25-2023](https://weekinethereumnews.com/week-in-ethereum-news-february-25-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Feb 27 – deadline for [EF academic grants round](https://esp.ethereum.foundation/academic-grants-2023)

- Feb 28 – [Sepolia testnet](https://blog.ethereum.org/2023/02/21/sepolia-shapella-announcement) upgrades to Shapella

- Mar 2-5 – [ETHDenver Hackathon](https://www.ethdenver.com/)

- Mar 10-29 – [Scaling Ethereum](https://ethglobal.com/events/scaling2023) (ETHGlobal) virtual

- **Mar 11  –**  [**Ethereum Guatemala**](https://www.eventbrite.com/e/ethereum-guatemala-11-de-marzo-tickets-531104466757)

- Mar 15-16 – [ETHDubai](https://www.ethdubaiconf.org/)

- Mar 16-18 – [ETH Porto](https://ethporto.org/)

- Mar 28-30 – [Ethereum Rio](https://www.ethereumbrasil.com/ethereumrio)

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- Apr 14-16 – [ETHGlobal Tokyo](https://tokyo.ethglobal.com/)

- **Apr 14-16 –** [**EthereumZuri.ch**](https://ethereumzuri.ch/) **conference & hackathon**

- Apr 21-25 – [EthTaipei](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) hackathon & conference

- Apr 27-30 – [Istanbul ETH Privacy](https://www.leadingprivacy.com/istanbul) conference & hackathon

- May 5-7 – [ETHMalaysia](https://ethmalaysia.com/) conference & hackathon

- May 5-7 – [ETHTallinn](https://ethtallinn.org/) hackathon

- May 9-10 – [NFT Tallinn](https://nfttallinn.com/) conference

- May 19-23 – [EDCON](https://edcon.io/) Montenegro (changed from Vienna)

- May 20-21 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 24-26 – [Spaghett ETH](https://naples.spaghett-eth.com/) (Naples) conference

- May 26–28 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Jun 2-4 – [ETH Seoul](https://2023.ethseoul.org/)

- **Jun 9-11 –** [**ETHPrague**](https://ethprague.com/) **conference & hackathon**

- Jun 23–25 – [ETHGlobal Toronto](https://ethglobal.com/events/toronto)

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Aug 16-19 – [Ethereum Argentina](https://twitter.com/EtherArgentina/status/1625857633260552200) (Buenos Aires)

- **Sep 10-12 –** [**Ethereum Singapore**](https://www.ethereumsingapore.com/) **hackathon & conference**

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–25 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

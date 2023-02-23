---
title: "Week in Ethereum News <br> December 17, 2022"
date: "2022-12-17"
---

## Eth News and Links

**Shapella (Shanghai + Capella) upgrade**

- Tim Beiko’s [core devs update](https://tim.mirror.xyz/zLdl8bEiDmobHZ5RlvG2LrlZLWV9c2XvkuKQ-vpljSU): details of Shanghai EIPs and planning for the subsequent Cancun upgrade

- Latest consensus devs call [video](https://www.youtube.com/watch?v=UazJO0fQ3Ho&t=111s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/Bk9cIjuus) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-consensus-layer-call-100/): Shapella testnet planned for next week, D-starname needed for next CL upgrade

- Consensus-specs [v1.3.0-alpha.2](https://github.com/ethereum/consensus-specs/releases/tag/v1.3.0-alpha.2): adds withdrawals sweep bounding, config changes, clarifications & minor fixes

**Cancun + D-starname upgrade**

- EIP4844 implementers call [video](https://www.youtube.com/watch?v=MQGJgdWOTpI&t=9s) and [notes](https://twitter.com/terencechain/status/1602708792051138560): devnet 3 planned for next week

- [Run EIP4844 local devnet](https://hackmd.io/q1SLCaubTIWw_1zsEjW_Vg?view) using Geth + Prysm

- EIP1153 [transient storage explainer](https://etherworld.co/2022/12/13/transient-storage-for-beginners/)

**Layer 1**

- [Lido plans to delegate listing of MEV-Boost relays](https://research.lido.fi/t/lido-on-ethereum-identify-and-constitute-relay-maintenance-committee/3386) to a committee

- [Reconnaissance](https://github.com/Will-Smith11/reconnaissance#readme): proxy node using Reth client

- Vitalik’s [EOF proposal to ban code introspection](https://ethereum-magicians.org/t/eof-proposal-ban-code-introspection-of-eof-accounts/12113): automate code conversion to the latest EVM version and make adding EVM features easier

**Research**

- [Block vs slot auction](https://mirror.xyz/0x03c29504CEcCa30B93FF5774183a1358D41fbeB1/CPYI91s98cp9zKFkanKs_qotYzw09kWvouaAa9GXBrQ) Proposer-Builder Separation

**Client releases**

- Consensus Layer:
    - Nimbus [v22.11.1](https://github.com/status-im/nimbus-eth2/releases/tag/v22.11.1): hotfix for missed block proposals when using remote signers
    
    - Prysm [v3.2.0](https://github.com/prysmaticlabs/prysm/releases/tag/v3.2.0): adds randao json & liveness endpoints and bug fixes 

- Execution Layer:
    - Besu [v22.10.3](https://github.com/hyperledger/besu/releases/tag/22.10.3): implement Eth/68, speed up modexp, Graalvm no longer supported
    
    - EthereumJS [v0.6.6](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs/client%400.6.6): optimizations & fixes from Shandong (pre-Shanghai) testnet
    
    - Erigon [v2.32.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.32.0): bug fixes

**Layer 2**

- Arbitrum [griefing attack of bridge deemed unrealistic](https://twitter.com/hkalodner/status/1601788042431397889) as no plans for third party relayers

- Scroll: [bottlenecks in proof generation](https://scroll.io/blog/proofGeneration) with options to accelerate

- Polygon [zkEVM](https://twitter.com/jbaylina/status/1603144831978831872) proving time 2.5 min on a $7 per hour AWS instance

- Consensys [Vortex zk prover](https://ethresear.ch/t/vortex-building-a-prover-for-the-zk-evm/14427): 30 million gas block in 5 minutes on AWS hpc6a.48xlarge

- zkSync [v2 alpha delayed](https://twitter.com/zksync/status/1602687972108664832) until Q2 2023

**EIPs/Standards**

- [EIP6120](https://github.com/ethereum/EIPs/pull/6120/files): Universal token router

- [EIP6122](https://github.com/ethereum/EIPs/pull/6122/files): Forkid checks based on timestamps

- [EIP6123](https://github.com/ethereum/EIPs/pull/6123/files): Smart derivative contract

- [EIP6145](https://github.com/ethereum/EIPs/pull/6145/files): Hashtag NFT collective royalty treasury

- [EIP6147](https://github.com/ethereum/EIPs/pull/6147/files): Guard of NFT/SBT, an extension of ERC721

- [EIP6150](https://github.com/ethereum/EIPs/pull/6150/files): Hierarchical NFTs

* * *

### **This newsletter is made possible thanks to** [**SpeedRunEthereum**](https://speedrunethereum.com/)**!**

![Speed Run Ethereum](https://weekinethereumnews.com/wp-content/uploads/2022/10/Speed-Run-Ethereum-banner.png)

Test your skills and learn how to build apps on Ethereum at [SpeedRunEthereum.com](https://speedrunethereum.com/).

* * *

**Stuff for developers**

- [Sepolia testnet](https://sepolia.ethpandaops.io/) landing page: RPC, checkpoint sync, explorers & spec

- Forge-std [v1.2.0](https://github.com/foundry-rs/forge-std/releases/tag/v1.2.0) (Foundry): speed up via-ir compilation, bound integers and cheat codes for environment variable defaults, get file/folder metadata & to pause gas metering

- Foundry [fork testing using a specific block number](https://twitter.com/PaulRBerg/status/1603057723985301507) in GitHub Actions can cache RPC responses

- Remix [v0.29.0](https://medium.com/remix-ide/remix-ide-v0-29-0-release-9cd5718b7021): debugger shows gas usage in editor & variable value on hover, multisig workspace template, UI in Simplified Chinese characters, formatting config and remixd updated

- Otterscan [v1.29.0](https://github.com/wmitsuda/otterscan/releases/tag/v2022.12.01-otterscan): optional beacon chain integration

- [Contract honeypots](https://mplankton.substack.com/p/rediscovering-smart-contract-honeypots): review of common traps with examples

- [Auditing heuristics](https://github.com/OpenCoreCH/smart-contract-auditing-heuristics#readme) for common pitfalls

- Sol2uml [v2.4.0](https://github.com/naddison36/sol2uml/releases/tag/v2.4.0) adds flattened diff of verified contracts

- Create an [NFT balance checker React hook](https://blog.0x3.studio/a-very-simple-to-offer-a-connect-wallet-option-for-your-website-thanks-to-rainbowkit/) using RainbowKit & wagmi

**Security**

- Lodestar Finance on Arbitrum [$5.8 million exploit](https://blog.lodestarfinance.io/post-mortem-summary-13f5fe0bb336) via price oracle manipulation

- SushiSwap [Kashi vulnerability disclosed](https://blocksecteam.medium.com/beyond-the-market-risk-a-logic-bug-identified-in-sushiswaps-kashipairmediumriskv1-contract-80ead49d8d6d), pools could be drained via outdated exchange rate

**Ecosystem**

- [KZG ceremony grants round](https://blog.ethereum.org/2022/12/15/kzg-ceremony-grants-round) (for EIP4844) to develop an implementation or perform weird entropy generation & destruction

- ETHIndia (ETHGlobal) [finalists](https://twitter.com/ETHGlobal/status/1603833092346609700)

**Enterprise**

- VMware [Blockchain for Ethereum](https://octo.vmware.com/vmware-blockchain-v1-8/) Beta 1 release

- [PayPal integrated with MetaMask mobile app](https://consensys.net/blog/press-release/consensys-teams-with-paypal-for-a-new-way-to-buy-crypto-in-metamask/) to allow US users to buy ETH

**Application layer**

- [PartyBid](https://party.mirror.xyz/zgdSE6qsaa_su8rqFJq-HsoKtTvdnubIzElG0J2TOiQ) (crowdfund NFT purchases) adds membership NFTs for group actions on purchases

- [KnifeGame](https://medium.com/@knifegame/knife-game-round-1-the-complete-guide-ffe1f4b2ff23) PvP game, spy & knife prices determined by a VRGDA curve

- [Santa.fm](https://twitter.com/JordanLyall/status/1603794030420447232): on-chain white elephant NFT gift exchange

- Optimism’s [AttestationStation](https://community.optimism.io/docs/governance/attestation-station): reputation contract live

* * *

### Job Listings

- [Backend Engineers](https://grnh.se/d933f3635us) wanted by Alchemy to bring web3 to 1 billion people.

- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- SBF & FTX:
    - SBF [arrested](https://twitter.com/sdnynews/status/1602451395910803457) with fraud charges by [US Attorney](https://www.justice.gov/usao-sdny/pr/united-states-attorney-announces-charges-against-ftx-founder-samuel-bankman-fried), [CFTC](https://www.cftc.gov/PressRoom/PressReleases/8638-22) & [SEC](https://www.sec.gov/news/press-release/2022-219)
    
    - [Bloomberg, Dow Jones, NYT & FT](https://twitter.com/AutismCapital/status/1601371985514139648) objected to redaction of customer info from bankruptcy filing

- Reuters: [US Justice Department split over charging Binance](https://www.reuters.com/markets/us/us-justice-dept-is-split-over-charging-binance-crypto-world-falters-sources-2022-12-12/).  \[Binance [denies](https://www.binance.com/en/blog/leadership/inside-binances-fight-against-crypto-crime-5422427314690193337)\]

- [Coinbase ERC20 recovery tool](https://www.coinbase.com/blog/coinbase-announces-new-asset-recovery-tool-for-erc-20-tokens) for deposited unsupported tokens

- Compound [DAO sued as general partnership](https://twitter.com/z0r0zzz/status/1602775520609177601) in frivolous lawsuit

- Donald Trump sells [$4.5m of NFTs](https://www.bbc.com/news/business-63995563) on Polygon

- Polynya: [Total Addressable Market for decentralized apps](https://polynya.mirror.xyz/gm6bUvvDF-sQAt7HuU6kRKCLIT9tAuaSCxHeNFdDVHk) isn’t that high in terms of blockspace

**General**

- Proposal for [SNARKed Merkle Sum Tree](https://ethresear.ch/t/snarked-merkle-sum-tree-a-practical-proof-of-solvency-protocol-based-on-vitaliks-proposal/14405), a Proof-of-Solvency protocol

- [Gemini vendor data leak](https://www.gemini.com/blog/protecting-our-customers-from-phishing-campaigns) of email addresses and partial phone numbers 

- [COVID-bit](https://arxiv.org/abs/2212.03520): electromagnetic waves transmit data over 2 meters from an air-gapped computer

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-17-2022](https://weekinethereumnews.com/week-in-ethereum-news-december-17-2022)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Dec 20 – [Attitudes to staking survey](https://stakingsurvey.paperform.co/) deadline

- Jan 8 – [Solidity developer survey](https://blog.soliditylang.org/2022/12/07/solidity-developer-survey-2022-announcement/) deadline

- Jan 17-31 – [Gitcoin grants round](https://go.gitcoin.co/blog/announcing-the-gitcoin-alpha-tests)

- **Jan 31 –** [**KZG ceremony grants round**](https://blog.ethereum.org/2022/12/15/kzg-ceremony-grants-round) **deadline**

- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

- Mar 15-16 – [ETHDubai](https://www.ethdubaiconf.org/)

- Apr 3-6 – [Edcon](https://edcon.io/) Vienna

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

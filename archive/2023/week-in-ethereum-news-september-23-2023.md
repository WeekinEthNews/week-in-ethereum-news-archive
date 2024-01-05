---
title: "Week in Ethereum News <br> September 23, 2023"
date: "2023-09-23"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=7ob1JFbcwZo&t=500s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-118/):
    - Devnet-9 planned for September 27, will include KZG ceremony values if ready
    
    - Public testnet upgrade order changed: Goerli to be first as it’s deprecated, allows testing 3/6 (target/max) EIP4844 blobs, ideally before Devconnect

- Dencun testing [call video](https://www.youtube.com/watch?v=DRkAEbE-V4g&t=137s).  Notes from [Terence](https://hackmd.io/@oiYljOkuS1KY6mgjjbfQww/BJwFNsc1a)

- Consensus-specs [v1.4.0-beta.2](https://github.com/ethereum/consensus-specs/releases/tag/v1.4.0-beta.2): adds EIP7514 (max churn limit) and fork-choice rule proposer boost adjustment

**Prague + Electra upgrade**

- Terence: [Electra focus should be improving consensus layer stability](https://terencechain.substack.com/p/navigating-ethereums-2024-consensus), inclusion list, increasing max effective balance (EIP7251) and improving fork choice

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 32.23%**](https://dune.com/hildobby/eth2-staking) **still far too close to risky** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm over 33%, a bug could mean loss of finality

- Need more [geographic diversity for both stakers and nodes](https://nodewatch.io/), particularly outside of US/Can/EU

**Layer 1**

- ERC4337 (account abstraction) meeting [notes](https://twitter.com/johnrising_/status/1704883350408950189)

- State of [verifying p256 curve onchain](https://hackmd.io/@1ofB8klpQky-YoR5pmPXFQ/SJ0nuzD1T)

- Guide to [adding a precompile into Revm](https://alessandromazza.notion.site/P256VERIFY-Precompile-in-Revm-ca2f782a91214b7d99f130cba8ceaed5) (and Reth), example adds P256VERIFY

- [MEV-Boost integrated builders](https://twitter.com/MaxResnick1/status/1705320727162077235) dominate CEX/DEX arbitrage due to advantages from latency

**For Stakers**

- [Using retirement funds](https://www.yamlike.com/archive/fund-solo-ethereum-validator-node-with-ira) (IRA in US) to fund solo staking

**Client releases**

- Execution layer:
    - Geth [v1.13.1](https://github.com/ethereum/go-ethereum/releases/tag/v1.13.1): hotfix for v1.13.0 block production, adds env vars for configs & colored help screen
    
    - Nethermind [v1.20.4](https://github.com/NethermindEth/nethermind/releases/tag/1.20.4): Holešky testnet new genesis

**Research**

- [EF Cryptographers](https://ethresear.ch/t/statement-regarding-the-public-report-on-the-analysis-of-minroot/16670): VDFs are dead…for now?

- Single Secret Leader Election (SSLE): [addressing Whisk bootstrapping problem](https://ethresear.ch/t/the-return-of-torus-based-cryptography-whisk-and-curdleproof-in-the-target-group/16678) using the target group and XTR & CEILIDH

- Mike Neuder: [ePBS](https://notes.ethereum.org/@mikeneuder/infinite-buffet) in-protocol designs, out-of-protocol proposals and open questions

- [Private PEPC-DVT](https://ethresear.ch/t/making-pepc-dvt-private-with-bls-blinded-multi-signatures/16692) using BLS blinded multi-signatures

**Layer 2**

- [Pessimism](https://base.mirror.xyz/qQAChAdkfZDG_8Ik7FgrMIpjE-si3TdF1E5W6c8ruFQ) by Base: monitoring system for OP Stack

- [Canto](https://polygon.technology/blog/canto-to-migrate-to-a-zk-l2-powered-by-polygon-chain-development-kit) and [Palm](https://www.infura.io/blog/post/palm-network-scales-up-for-enhanced-operations-and-broader-use-cases) plan migrations to zk rollups using Polygon Chain Development Kit (CDK)

- Optimism [RetroPGF Round 3 applications](https://optimism.mirror.xyz/wiHMKqsbAQnK51Se3MraSnvf0blwRzS9jguojEmKKVc) are open, 30 million OP will be distributed

**EIPs/Standards**

- EIPs
    - [EIP7519](https://eips.ethereum.org/EIPS/eip-7519): Atomic storage operations SCREDIT and SDEBIT
    
    - [EIP7523](https://eips.ethereum.org/EIPS/eip-7523): Empty accounts deprecation (prohibit empty accounts on post-merge networks)

- ERCs (application layer):
    - [ERC7520](https://github.com/ethereum/EIPs/pull/7733/files): zk-SNARK public inputs overflow protection
    
    - [ERC7521](https://github.com/ethereum/EIPs/pull/7739/files): General intents for contract wallets
    
    - [ERC7522](https://github.com/ethereum/EIPs/pull/7743/files): OIDC (OpenID Connect) zk verifier for Account Abstraction (ERC4337)

* * *

### **Lido is a systemic threat to ETH:** [**interview with Danny Ryan**](https://podcasters.spotify.com/pod/show/web3builderspodcast)

![Danny Ryan interview](https://weekinethereumnews.com/wp-content/uploads/2023/09/web3-Builders-Danny-Ryan-interview-1024x576.jpg)

Lido is a systemic threat to Ethereum.  You won't want to miss this [episode with Danny Ryan.](https://podcasters.spotify.com/pod/show/web3builderspodcast/episodes/Lido-Is-A-Systemic-Risk-W-Danny-Ryan-e29hpv8) (Watch on [YouTube](https://www.youtube.com/watch?v=Y0ddkSa1ZuI))

Danny also covers the death of VDFs, EIP7514 (max epoch churn limit) and EIP7251 (increase max effective balance).

* * *

**Stuff for developers**

- [Holešky testnet](https://github.com/eth-clients/holesky#readme) genesis rescheduled for September 28

- [Truffle & Ganache are being sunset](https://consensys.io/blog/consensys-announces-the-sunset-of-truffle-and-ganache-and-new-hardhat), devs can migrate to Hardhat

- Foundry:
    - [Rivet](https://twitter.com/_jxom/status/1704004731415511079) (developer wallet) adds log & calldata decoding
    
    - [Tstore-template](https://github.com/hrkrshnn/tstore-template#readme): Foundry template with custom solc binaries that support transient storage opcodes in inline assembly

- [Emily](https://github.com/0xfuturistic/emily#readme): Solidity library for credible commitments

- [Speed Run Ethereum](https://twitter.com/austingriffith/status/1703828935346454924) updated to Scaffold-ETH-2, can use Hardhat or Foundry

- Alchemy University [Learn Solidity](https://www.alchemy.com/university/courses/solidity): 11 browser based lessons

- [OP Viem](https://github.com/base-org/op-viem#readme): viem extension for OP Stack networks

- [TLSNotary](https://mirror.xyz/privacy-scaling-explorations.eth/T4MR2PgBzBmN2I3dhDJpILXkQsqZp1Bp8GSm_Oo3Vnw) (alpha release) enables privacy-preserving data provenance & portability

**Security**

- [Balancer frontend attacked](https://twitter.com/balancer/status/1704552285395894422) via social engineering of .fi domain registrar

- Proposed [onchain representation for audits](https://mirror.xyz/anichohan.eth/QoLKhNHUqkycVPV8Ku2KnjbcBlG-Wwj5Sz_bfmemgbg) (ERC7512)

**Ecosystem**

- [Rainbow browser extension](https://twitter.com/rainbowdotme/status/1704900402427166858): includes watch mode with impersonation

- Patrick McCorry: [enablement of MEV and morality of extracting](https://www.cryptofrens.info/p/enablement-of-mev-and-the-morals)

- ETHChicago [hackathon projects](https://taikai.network/ethchicago/hackathons/ETHChicagoHackathon2023/projects)

**Enterprise**

- [PayPal USD stablecoin](https://newsroom.paypal-corp.com/2023-09-20-PayPal-USD-is-now-available-on-Venmo) available on Venmo

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 6.3 to 329.3 gwei, with 12.9 gwei average
    - Negative issuance currently at 20.7 gwei 
    
    - 6k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $1,577 - $1,666, currently $1595

- [ETHBTC](https://ratiogang.com/): currently 0.06 (Flippening at ~0.16)

**Notable at app layer**

- [Cacti-chat](https://twitter.com/wearecacti/status/1704605245353918541) (web3 chatbot) live, beta

- [Anon Aadhaar](https://mirror.xyz/privacy-scaling-explorations.eth/6R8kACTYp9mF3eIpLZMXs8JAQmTyb6Uy8KnZqzmDFZI): anonymously prove Aadhaar (Indian) identity

- [DeFiSaver automates using Liquity](https://twitter.com/DeFiSaver/status/1703773252936708340) to earn Maker DSR interest

- [GammaSwap](https://medium.com/gammaswap-labs/gammaswap-is-officially-live-on-arbitrum-mainnet-e8a89e43ddb8): onchain options of Sushi pools, live on Arbitrum. Market makers can hedge AMM LP positions

- Vampire attacking CEX: [Infinex to allow traders](https://mirror.xyz/infinex.eth/YA3Z3PTktUEwKPZjrrwi86urUWHqYd86zlq0dzry5n8) to earn an airdrop from derivative CEX trading history

- [Optimism Airdrop 3](https://community.optimism.io/docs/governance/airdrop-3/#) directly distributed to users who delegated

* * *

### Job Listings

- [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db) wanted by EF

- EF Privacy & Scaling Explorations team seek a [Technical Project Coordinator](https://jobs.lever.co/ethereumfoundation/c826b9a1-ede0-465e-9639-f34029304374)

- [Logos Nomos](https://logos.co/nomos) is hiring a [Distributed Systems Applied Researcher](https://grnh.se/9fb1a68e1us)

**Job listings: $600 for four issues** (75 character limit).  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Coinbase campaign](https://www.coinbase.com/blog/a-call-to-action-mobilizing-52-million-crypto-owners-into-an-army-of-1) to get the 52 million Americans owning crypto to ask Congress to pass clear & sensible legislation

- [FTX sues SBF’s parents](https://storage.courtlistener.com/recap/gov.uscourts.deb.188450/gov.uscourts.deb.188450.2642.0.pdf) to recover alleged fraudulently transferred & misappropriated funds

**General**

- [Virgil Griffith moved prisons](https://twitter.com/brantlymillegan/status/1704478744130273363), new address to write to him

- [Nansen data breach](https://twitter.com/nansen_ai/status/1705137387838574904) via a vendor, some email addresses, password hashes and blockchain addresses exposed

- [More Apple zero-days](https://www.bleepingcomputer.com/news/apple/apple-emergency-updates-fix-3-new-zero-days-exploited-in-attacks/), update your devices

- Revisiting [hardware acceleration for zk proofs](https://medium.com/@omershlomovits/revisiting-paradigm-hardware-acceleration-for-zero-knowledge-proofs-16f717a49555)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-23-2023](https://weekinethereumnews.com/week-in-ethereum-news-september-23-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- **Sep 28 –** [**Holešky testnet**](https://github.com/eth-clients/holesky#readme) **genesis (rescheduled)**

- **Sep 28 - Oct 3 –** [**Huffathon**](https://huff.sh/hackathon) **challenges & hackathon (virtual)**

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 13-15 – [Ethereum Kuala Lumpur](https://hack.ethkl.org/) conference & hackathon

- Oct 21 – [Ethereum México](https://twitter.com/ethereum_mexico/status/1684649652639924224)

- Oct 22-24 – [ETH Hong Kong](https://www.ethhongkong.co/)

- Oct 27-29 – [ETH London](https://www.encode.club/eth-london) hackathon

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Oct 27-29 – [ETH Vietnam](https://www.eth-vietnam.com/)

- Oct 28-30 – [Paradigm CTF](https://ctf.paradigm.xyz/)

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) deadline (max $1k for local meetups)

- Nov 3-5 – [ETHBrno](https://ethbrno.cz)

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 16-19 – [Pragma](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Dec 4-5 – [ETHVenice](https://ethvenice.com/)

- Dec 8-10 – ETHGlobal [ETHIndia](https://ethindia.co/) (Bangalore) 

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

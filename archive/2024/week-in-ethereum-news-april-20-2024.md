---
title: "Week in Ethereum News <br> April 20, 2024"
date: "2024-04-20"
---

## Eth News and Links

**Pectra (Prague + Electra) upgrade (meta** [**EIP7600**](https://eips.ethereum.org/EIPS/eip-7600)**)**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=srOu8TqFYYM&t=550s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-132/):
    - **Electra included EIPs**:
        - **EIP7251 maxEB**: changing to execution layer triggered consolidations after pectra-devnet-0 and proposal to apply deposit to state when epoch finalized
        
        - **EIP7549 move committee index outside attestation**: discussion on handling Deneb attestations at fork boundary and proposal to replace committee bits with indices
    
    - **Electra proposed additions:**
        - **EIP7685 general purpose execution layer requests:** consolidate request types, decide Monday on including
        
        - **EIP7691 blob throughput increase:** short term scaling before PeerDAS, exact values to be based on testing, alternative to EIP7659 stepped increase
    
    - **Electra candidates for inclusion**:
        - **EIP7547 inclusion lists**: issues with EIP3074 can’t be resolved for Electra
    
    - Node-id mapping to attestation subnets: clarification for mainnet & PeerDAS

- consensus-specs [v1.5.0-alpha.0](https://github.com/ethereum/consensus-specs/releases/tag/v1.5.0-alpha.0): initial Electra spec for pectra-devnet-0 

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=FWvi_z1_gB0&t=242s).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1778489895587360814) & [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-185/):
    - **Pectra upgrade (small fork targeting late 2024)**
        - **EIPs added to Pectra & will be part of** [**pectra-devnet-0**](https://notes.ethereum.org/@ethpandaops/pectra-devnet-0):
            - EIP3074 AUTH/AUTHCALL opcodes
            
            - EIP2935 save historical block hashes in state
        
        - **EIPs considered for inclusion**:
            - EOF: need to assess cross client testing complexity & any potential issues with Verkle
            
            - EIP7623 increase call data cost: need to consider best mechanism to cap block size
        
        - **EIP7547 IL (inclusion lists)**: some opposition to including
    
    - **Osaka upgrade**
        - **EIPs considered for inclusion:**
            - EIP7667 raise gas costs of hash functions

- EIP3074 AUTH/AUTHCALL opcodes
    - Lightclient: [addressing EIP3074 concerns](https://twitter.com/lightclients/status/1778823652584120497)

- EIP7251 maxEB (increase max effective balance)
    - Breakout [call video](https://www.youtube.com/watch?v=J1i3WtLE-6o) & [notes](https://hackmd.io/@philknows/Hywht12eR): staking providers prefer execution layer triggered consolidations (consolidations not in pectra-devnet-0) and don’t need custom ceilings

**Osaka + F starname upgrade (meta** [**EIP7607**](https://eips.ethereum.org/EIPS/eip-7607)**)**

- Verkle:
    - Implementers [call video](https://www.youtube.com/watch?v=R-Jo2Lci0zc&t=6s) & [notes](https://twitter.com/rudolf6_/status/1778087343611884011)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.7%**](https://dune.com/hildobby/eth2-staking) **still too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~63% majority
    
    - Consensus layer: Prysm 38%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- ePBS
    - Potuz: [ePBS spec notes](https://hackmd.io/@potuz/rJ9GCnT1C) and [ePBS forkchoice annotated spec](https://hackmd.io/@potuz/SJdXM43x0)
    
    - Terence: [with ePBS you may choose to trust relayers](https://hackmd.io/@ttsao/bypassing-relayer) instead of having to trust them

- Vitalik: a concrete [proposal for correlated attester penalties](https://ethresear.ch/t/a-concrete-proposal-for-correlated-attester-penalties/19341)
    - Vitalik’s proposal builds on Toni Wahrstätter’s [correlated attestation penalties analysis](https://ethresear.ch/t/analysis-on-correlated-attestation-penalties/19244)

- Issuance change proposals:
    - [Minimum viable issuance](https://notes.ethereum.org/@anderselowsson/Foundations-of-MVI) creates value by reducing total costs for users
    
    - [Reward curve with capped issuance](https://notes.ethereum.org/@anderselowsson/Reward-curve-with-capped-issuance), alternative to tempered issuance
    
    - Why [exogenous rewards must be considered](https://mirror.xyz/themandalore.eth/y4wDpXtVv-3rNf_zVjkXsXuThvrF32NdpNRJH_rtHiY) in the issuance debate 

- ethPandaOps:
    - [Assertoor](https://ethpandaops.io/posts/assertoor-introduction/): cross-client integration testing tool, higher abstraction level than Hive
    
    - [Tracoor](https://ethpandaops.io/posts/tracoor-debug-tool/): beacon data & execution trace explorer to identify & address network problems
    
    - [Guide to using Kurtosis](https://ethpandaops.io/posts/kurtosis-deep-dive/) & ethereum-package to launch local devnets

- bloXroute & Lighthouse: [post mortem of March issue with 13% missed slots](https://gist.github.com/benhenryhunter/7b7d9c9e3218aad52f75e3647b83a6cc)

**Client Releases**

- Execution layer:
    - Geth [v1.13.15](https://github.com/ethereum/go-ethereum/releases/tag/v1.13.15): fixes to avoid snapsync-related data-corruption

**For Stakers**

- EthStaker [staking survey](https://stakinglandscape.limesurvey.net/748278)

**Layer 2**

- Arbitrum [BOLD](https://medium.com/offchainlabs/arbitrum-bold-testnet-live-the-next-step-in-decentralization-2a6cd39e9bba) (dispute resolution protocol) live on dedicated testnet

- L2BEAT [Costs](https://l2beat.com/scaling/costs): breakdown of L2 transaction costs

- [XEN spam](https://twitter.com/notnotstorm/status/1778803270750023813) is 68% of Base state

- Steven Goldfeder: [technical & financial benefits end at L3](https://twitter.com/sgoldfed/status/1778173218496401807)

- ZeroPool: [zk native sharded storage protocol](https://zeropool.network/pdf/WriteupZeroPoolShardedStorage.pdf)

- [Prooφ](https://arxiv.org/abs/2404.06495): SNARK prover market mechanism

- RollCall (L2 standards) [call video](https://www.youtube.com/watch?v=M2v6Rv2XE_o)

**EIPs/Standards**

- EIPs:
    - [EIP7684](https://eips.ethereum.org/EIPS/eip-7684): Return deposits for distinct credentials
    
    - [EIP7685](https://eips.ethereum.org/EIPS/eip-7685): General purpose execution layer requests
    
    - [EIP7686](https://eips.ethereum.org/EIPS/eip-7686): Linear EVM memory limits
    
    - [EIP7688](https://github.com/ethereum/EIPs/pull/8439/files): Forward compatible consensus data structures
    
    - [EIP7691](https://github.com/ethereum/EIPs/pull/8452/files): Blob throughput increase 
    
    - Meta [EIP7692](https://github.com/ethereum/EIPs/pull/8448/files): EVM Object Format (EOF) Meta
    
    - [EIP7693](https://github.com/ethereum/EIPs/pull/8454/files): Backward-compatible post-quantum migration 

- RIPs (Rollup Improvement Proposals):
    - [RIP7696](https://github.com/ethereum/RIPs/pull/18/files): Precompile for generic DSM (double scalar multiplication)

- ERCs (application layer):
    - [ERC7680](https://github.com/ethereum/ERCs/pull/368/files): Valued tokens with layered liquidity
    
    - [ERC7681](https://github.com/ethereum/ERCs/pull/369/files): Dual nature multi-token protocol (ERC20 & ERC1155)
    
    - [ERC7682](https://github.com/ethereum/ERCs/pull/372/files): Auxiliary funds capability
    
    - [ERC7683](https://eips.ethereum.org/EIPS/eip-7683): Cross chain intents ([proposed by Uniswap & Across Protocol](https://blog.uniswap.org/uniswap-labs-and-across-propose-standard-for-cross-chain-intents))
    
    - [ERC7687](https://github.com/ethereum/ERCs/pull/378/files): AUTHCALL ERC4626 deposit/withdraw extension
    
    - [ERC7689](https://github.com/ethereum/ERCs/pull/380/files): Smart blobs (state machine on top of blobs)
    
    - [ERC7690](https://github.com/ethereum/ERCs/pull/382/files): Union lock (based on TSTORE/TLOAD)
    
    - [ERC7694](https://github.com/ethereum/ERCs/pull/390/files): Solana storage handler for CCIP-Write
    
    - [ERC7695](https://github.com/ethereum/ERCs/pull/391/files): Ownership delegation and context for NFTs

**Stuff for developers**

- Remix [v0.47.0](https://medium.com/remix-ide/remix-release-v0-47-0-d52f3dc21886): adds Solidity Copilot using SolCoder LLM, pin contracts deployed to Remix VM and DappDraft plugin to generate a front end

- Foundry:
    - [Forge clone](https://twitter.com/troublor/status/1780984367931695256): create Foundry project from a verified contract
    
    - [Forge verify-bytecode](https://twitter.com/lucasmanuel_eth/status/1778806293190316393): verify code at a commit hash matches deployed contract
    
    - [OpenZeppelin Foundry Upgrades](https://github.com/OpenZeppelin/openzeppelin-foundry-upgrades#readme): deploy/manage upgradeable contracts with safety checks

- [Token types](https://github.com/jtriley-eth/token-types#readme) (Solidity): drop-in replacements for interfaces; ERC20, ERC721, ERC721Receiver, ERC4626 & ERC6909

- Solhint community [v4](https://github.com/solhint-community/solhint-community/blob/master/CHANGELOG.md): config files per subdirectory, improved exit code handling, saner defaults, single rule for casing & redefined recommended ruleset

- [Inline Yul](https://twitter.com/jtriley_eth/status/1781399788556337524) style guide

- [FUCK](https://brainfucktoken.eth.link/): ERC20 token implemented in Brainfuck

- Slither [v0.10.2](https://github.com/crytic/slither/releases/tag/0.10.2): slither-mutate support for Foundry projects, unused imports detector and supports aliases

- Cyfrin [Aderyn](https://github.com/Cyfrin/aderyn#readme): Solidity static analyzer, in Rust

- [Vyper interface scanner](https://blog.yacademy.dev/2024-04-19-small-steps-in-automating-security/): detecting incorrect interface definitions

- Halmos [v0.1.11](https://twitter.com/0xkarmacoma/status/1778904133820616867) (symbolic testing): adds support for ecrecover precompile, addr(key) & sign(key, digest) cheats and makeAddr functions from forge-std

- [Sub Zero](https://github.com/Philogy/sub-zero-contracts#readme): mine vanity addresses using CREATE2, tokenized as ERC721 NFTs

- Viem [experimental](https://viem.sh/experimental): adds EIP3074 sign & verify auth message and recover signing address from auth message

- Guide to [writing efficient DuneSQL queries](https://docs.dune.com/query-engine/writing-efficient-queries)

- [Sonobe](https://github.com/privacy-scaling-explorations/sonobe#readme) experimental folding schemes library, implements Nova & CycleFold

**Security**

- Hedgey Finance [$44M exploit](https://cryptocsec.substack.com/p/hack-alert-hedgy-finance-exploit) on Arbitrum & mainnet via missing input validation

- Grand Base [$2M exploit](https://rekt.news/grand-base/) on Base via deployer private key compromise

- [SEAL-ISAC](https://twitter.com/samczsun/status/1780586104506531948) (database of blackhat info): free membership for whitehats via application

- [Analysis of Angel drainer](https://muellerberndt.medium.com/a-brief-analysis-of-angel-drainer-1660d15c9248) used in web3 phishing

**Ecosystem**

- [Decline of public transaction pool](https://paragraph.xyz/@chaskin/private-transactions-where-mev-and-the-public-mempool-go-to-die): private RPCs & order flow auctions used to reduce impact of MEV

- [ETHDam](https://taikai.network/cryptocanal/hackathons/ethdam2024/projects) hackathon projects

- [Eth.limo](https://twitter.com/eth_limo/status/1778783099897168236) architecture explainer

* * *

### Job Listings

- ChainSafe: [Head of Protocol Engineering](https://grnh.se/c6e27e794us) and [Senior Product Manager](https://grnh.se/8736d15d4us)

- EF: [People Operations Support](https://jobs.lever.co/ethereumfoundation/8054f5c5-ac89-4da8-98cc-738797837446)

- Devcon: [Community Supporter](https://jobs.lever.co/ethereumfoundation/6ad3d8e7-17cb-4d5c-820d-c279e8002551), [Production Magician](https://jobs.lever.co/ethereumfoundation/aa4c69f8-f564-4036-9c5e-3e09f0eb27df) & [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/e93dae67-65a6-495c-8638-46e3db28cb64)

- Nethermind [Mechanism Designer](https://grnh.se/e78eb182teu), [Protocol Research Manager](https://grnh.se/8f2a6c32teu), [Research Engineer](https://grnh.se/887df932teu)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 5.0 to 586.3 gwei, with 17.5 gwei average
    - Zero net issuance currently at 23.0 gwei 
    
    - 4.1k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,876 - $3,282, currently $3,029

- [ETHBTC](https://ratiogang.com/): currently 0.048 (Flippening at ~0.16)

**Notable at app layer**

- [PoolTogether](https://pooltogether.mirror.xyz/ASC44Qnx2rgDMM2mAcdBs-EvuiBurMe-d5_1rBdC2q8) v5 live on Optimism, ETH prizes automatically sent, no parameter governance & no admin controls
    - [Target Period Dutch Auction](https://twitter.com/b_asselstine/status/1781090260727771362) liquidation algorithm

- [ethOS phone](https://twitter.com/ethereumphone/status/1780295152168317391): mint & burn NFT on Base to redeem for Pixel 7a with ethOS v3

- [Ouragan](https://www.leku.blog/ouragan/): Tornado Cash offramp

- [71.8 ETH donated to Roman Storm & Alex Pertsev legal defense fund](https://twitter.com/freealexeyroman/status/1780694076578238905) after coordinated jury vote for Crypto: The Game Season 2

**Regulation/business/tokens**

- [Uniswap Labs](https://blog.uniswap.org/fighting-for-defi) received Wells notice from SEC

- [IRS draft form 1099-DA](https://twitter.com/TheCryptoCPA/status/1781403340045197813) includes unhosted wallet provider checkbox

- Mango Markets attacker [Avraham Eisenberg convicted](https://www.justice.gov/opa/pr/man-convicted-110m-cryptocurrency-scheme) for commodities fraud & market manipulation, sentencing scheduled for July 29

- [Ethereum generated $369M profit](https://twitter.com/tokenterminal/status/1780911733613167072) in Q1 (daily USD value of burned ETH minus issuance)

**General**

- Telegram users: [disable automatic media download](https://twitter.com/ChainLight_io/status/1778722009687720325) to prevent attacks via media files

- [World-Check](https://techcrunch.com/2024/04/18/world-check-database-leaked-sanctions-financial-crimes-watchlist/) KYC screening database illegally obtained via third party system

- [Jolt](https://a16zcrypto.com/posts/article/a-new-era-in-snark-design-releasing-jolt/): zkVM using sumcheck protocol

- [Blendy](https://gfenzi.io/papers/blendy-sumcheck/): sumcheck prover

- [Greco](https://eprint.iacr.org/2024/594): fast zk proofs for valid FHE RLWE ciphertexts formation

- [Rapidsnark GPU acceleration](https://orbiter-finance.medium.com/gpu-acceleration-of-rapidsnark-46b64d99f00d) 4x CPU

- [Families of prime-order endomorphism-equipped](https://eprint.iacr.org/2023/1662) embedded curves on pairing-friendly curves

- [Mopro](https://github.com/zkmopro/mopro#readme): simple client-side proving on mobile

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-april-20-2024](https://weekinethereumnews.com/week-in-ethereum-news-april-20-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Apr 23-May 7 – [Gitcoin Grants 20](https://www.gitcoin.co/blog/announcing-gg20)

- Apr 26-28 – [ETHBoston](https://ethboston.xyz/) hackathon & conference

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- May 10-11 – [ETH Bratislava](https://www.ethbratislava.com/) conference & hackathon

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/) hackathon

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- May 31-Jun 5 – [ETH Belgrade](https://ethbelgrade.rs/) hackathon & conference

- Jun 14 – [EF EIP4844 data challenge](https://esp.ethereum.foundation/data-challenge-4844) deadline

- Jun 21-23 – [ETHKyiv](https://www.ethkyiv.org/) hackathon & conference

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 26-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 23-26 – [ETHTokyo](https://www.ethtokyo.com/) hackathon & conference

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- Sep 5-8 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 9-15 – [ETHSafari](https://ethsafari.xyz/) (Kenya)

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

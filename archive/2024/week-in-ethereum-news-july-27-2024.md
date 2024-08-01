---
title: "Week in Ethereum News <br> July 27, 2024"
date: "2024-07-27"
---

## Eth News and Links

Spot ETH ETFs launched in US and support Roman Storm legal defense

**All core devs**

- [All core devs – consensus (ACDC) #138](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-138-july-25-2024/20630):
    - **Pectra (Prague + Electra) upgrade**:
        - [**Pectra-devnet-1**](https://pectra-devnet-1.ethpandaops.io/) launched, multiple issues being debugged
        
        - **Request types**:
            - [ExecutionPayloadEnvelope](https://github.com/ethereum/consensus-specs/issues/3856) proposal: broad support to move request data needed for state transition outside structure that CL clients prune
            
            - [Unify request objects](https://github.com/ethereum/execution-apis/pull/565) proposal: intend to move forward
        
        - **SSZ StableContainer**: no strong push for inclusion, focus on existing Pectra EIPs before considering increasing scope
        
        - **EIP7594 PeerDAS**:
            - Simplification proposal to drop peer sampling phase from Pectra
            
            - Discussion on when to activate (currently separate epoch to Pectra)
        
        - [BeaconBlocksByRange v3](https://github.com/ethereum/consensus-specs/pull/3845) proposal

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade, likely targeting Q1 2025**

- [PeerDAS breakout #4](https://ethereum-magicians.org/t/peerdas-breakout-4-july-23-2024/20629):
    - Teams focused on client stability, optimization & refactoring before launching peerdas-devnet-2

- [EOF taxonomy](https://rakita.github.io/blog/EVM%20(EOF)%20Taxonomy.png) diagram

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 29.05%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~55% majority 
    
    - Consensus layer: Prysm 35%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Layer 1**

- EIP7732 ePBS:
    - Terence: [builder bidding strategies under ePBS market space rules](https://ethresear.ch/t/builder-bidding-behaviors-in-epbs/20129)

**Research**

- Toni Wahrstätter: [EIP7716 anti-correlation penalties](https://ethresear.ch/t/diseconomies-of-scale-anti-correlation-penalties-eip-7716/20114) for diseconomies of scale

- [Block builder concentration](https://arxiv.org/abs/2407.13931) analysis

**Client Releases**

- Execution layer:
    - Erigon:
        - [v2.60.5](https://github.com/erigontech/erigon/releases/tag/v2.60.5): improvements & fixes
        
        - [v3.0.0-alpha1](https://erigon.tech/erigon-3-alpha-1-the-first-all-in-one-evm-node-on-the-efficient-software-frontier-is-live/): all-in-one (execution layer + Caplin consensus layer) node
    
    - Nethermind [v1.27.1](https://github.com/NethermindEth/nethermind/releases/tag/1.27.1): fix improperly enabled pre-warming blocks on OP Stack chains

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7747](https://github.com/ethereum/EIPs/pull/8743/files): EVM modular arithmetic extensions
    
    - [EIP7748](https://github.com/ethereum/EIPs/pull/8752/files): State conversion to Verkle Tree

**Stuff for developers**

- Foundry [Anvil](https://github.com/foundry-rs/foundry/pull/8476) adds EIP7702 support

- [Eclair](https://x.com/danhper/status/1816897006423445550): Solidity interpreter, focused on contract interactions

- [Guide to improving Foundry testing](https://blog.sigmaprime.io/forge-testing-leveling.html) using fuzzing & invariant testing

- RareSkills:
    - [Solidity try/catch](https://www.rareskills.io/post/try-catch-solidity) guide, handling low-level call failure
    
    - [Beacon proxy pattern](https://www.rareskills.io/post/beacon-proxy) explainer

- Tips:
    - [Solidity arrays & memory](https://x.com/optimizoor/status/1815633095347085506)
    
    - [Solady LibString](https://x.com/optimizoor/status/1815889772046651745) for string concatenation

- [Sandwich-resistant AMM](https://www.umbraresearch.xyz/writings/sandwich-resistant-amm): application-layer approach to mitigate atomic sandwich attacks

- [Trevm](https://x.com/init4tech/status/1816504559440900561): typestate interface to revm

- Viem [v2.18](https://x.com/wevm_dev/status/1816196241329643640): adds ERC-4337 Account Abstraction extension

**Security**

- MonoSwap [$1.3M stolen](https://x.com/monoswapio/status/1816151998267547851) on Blast via phishing of developer

- Spectra [$550k exploit](https://x.com/shoucccc/status/1815981585637990899) via arbitrary call to any address

**Enterprise**

- Toyota research into [mobility accounts](https://www.toyota-blockchain-lab.org/library/how-to-introduce-mobility-into-the-public-blockchain) based on ERC4337 account abstraction

* * *

### Job Listings

- Aragon: [Senior Smart Contract Developer](https://jobs.lever.co/aragon/fba68080-9e98-49d7-8ed7-ac05d047d4b0)

- [EF Protocol Support](https://jobs.lever.co/ethereumfoundation/60a70892-cea9-461e-9db2-199cb95f7d43): generalist to help with ACD, EPF, SoP & more

- EF seek a [European/Civil Law qualified Legal Counsel](https://jobs.lever.co/ethereumfoundation/204e2031-e60b-4c43-835a-e6837cef00b2)

- Nethermind: [Senior Device Security Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4336487101), Senior DevOps Engineer [AMER](https://boards.eu.greenhouse.io/nethermind/jobs/4363348101) & [APAC](https://boards.eu.greenhouse.io/nethermind/jobs/4363281101), [Full Stack Lead](https://boards.eu.greenhouse.io/nethermind/jobs/4356246101) APAC, [Post-Grad Internship](https://boards.eu.greenhouse.io/nethermind/jobs/4364252101) & [App Security Engineer](https://boards.eu.greenhouse.io/nethermind/jobs/4363291101)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 1.1 to 46.7 gwei, 4.5 gwei average; zero net issuance at 23.6 gwei 
    
    - 15k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,099 - $3,538, currently $3,265, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.048 (Flippening at ~0.164)

**Notable at app layer**

- [Coinbase](https://x.com/coinbasewallet/status/1816518451651051986): free conversion from USDT on Tron to USDC on Base for parts of Latin America, Africa & Asia

- Atari X [Asteroids](https://www.arcade.fun/asteroids) live on Base, mint to play

- Zora [Sparks](https://zora.co/writings/sparks): changing display units to 1/1000000 ETH (Szabo)

**Regulation/business/tokens**

- Spot ETH ETFs launched in US:
    - [ETF flow](https://farside.co.uk/?p=1518) dashboard

- [UK Financial Conduct Authority](https://www.fca.org.uk/news/press-releases/fca-first-enforcement-action-against-firm-enabling-cryptoasset-trading) fined Coinbase £3.5M for user onboarding with restrictions in place

**General**

- [Support Roman Storm legal defense](https://x.com/freealexeyroman/status/1815466170948219153) via Juicebox fundraiser

- Vitalik: [circle STARKs](https://vitalik.eth.limo/general/2024/07/23/circlestarks.html) (implemented in Stwo & Plonky3)

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-july-27-2024](https://weekinethereumnews.com/week-in-ethereum-news-july-27-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jul 29-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 2-4 – [Ethereum Argentina](https://ethereumargentina.org/) conference & hackathon

- Aug 7-9 – [Science of Blockchain Conference](https://www.sbc-conference.com/) (New York)

- Aug 15-17 – [Ethereum Uruguay](https://www.ethereumuruguay.org/) hackathon & conference

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

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

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

---
title: "Week in Ethereum News <br> July 6, 2024"
date: "2024-07-06"
---

## Eth News and Links

Pectra upgrade size discussion (potentially cap scope)

**All core devs**

- [All core devs – execution (ACDE) #191](https://ethereum-magicians.org/t/all-core-devs-execution-acde-call-191-july-4-2024/20427):
    - Pectra (Prague + Electra) upgrade:
        - **pectra-devnet-1**: now expect to launch in 1-2 weeks, locally tested with 2 execution layer + 3 consensus layer clients
        
        - **EIP7702**: delegation designation proposal to be merged & included in pectra-devnet-2
        
        - **RIP7212 secp256r1 precompile**: discussion on including in Pectra, whether to use RIP precompile address & what return value to use; review inclusion at next ACDE
        
        - **EIP7002 EL triggered withdrawals & EIP7251 maxEB**: agreed to add events
        
        - **Pectra size discussion**: potentially capping (strong support) or reducing (some support) scope
    
    - Discussions: history expiry and improving blob transaction propagation
        - To progress non-upgrade specific features need to target specific devnets, provide updates at all core devs & more breakouts

[**Osaka + F starname**](https://eips.ethereum.org/EIPS/eip-7607) **upgrade**

- [Verkle implementers call #20](https://ethereum-magicians.org/t/verkle-implementers-call-20-july-1-2024/20428): blockhash handling to use EIP4788 behavior, sync during transition needs to be combination of snap & full sync and avoiding extra EOF extcodesize/hash costs

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 29.2%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~55% majority 
    
    - Consensus layer: **Prysm 37%**
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Layer 1**

- Vitalik: [faster transaction confirmation times](https://vitalik.eth.limo/general/2024/06/30/epochslot.html) via Single Slot Finality & rollup/based preconfirmations

- EIP7732 ePBS:
    - [ePBS breakout #4](https://ethereum-magicians.org/t/epbs-breakout-4-july-5-2024/20429): EIP created, pull request for consensus specs, withdrawal processing complications and bid gossip p2p DoS vulnerability
    
    - Terence: [fork choice attacks in ePBS](https://ethresear.ch/t/fork-choice-attacks-and-protections-in-epbs/19951)
    
    - Potuz: [benefits of ePBS](https://x.com/potuz_eth/status/1808569058045931523)

- Dapplion: [fetch blobs from execution layer pool](https://hackmd.io/@dapplion/blob_fetch) proposal, rather than wait for blobs over gossipsub

- Flashbots [rbuilder](https://github.com/flashbots/rbuilder#readme): MEV-Boost block builder in Rust

- Gossipsub performance: [bandwidth consumption](https://ethresear.ch/t/ethereum-node-message-propagation-bandwidth-consumption/19952) and [message propagation latency](https://ethresear.ch/t/gossipsub-message-propagation-latency/19982)

**Client Releases**

- Execution layer:
    - Geth [v1.14.6](https://github.com/ethereum/go-ethereum/releases/tag/v1.14.6): adds experimental stateless witness builder & (self) cross validator

**For Stakers**

- Obol Charon [v1](https://blog.obol.org/releasing-charon-1-0/): distributed validator middleware

- EthStaker [staking survey results](https://paragraph.xyz/@ethstaker/staking-survey-2024): 32% genesis stakers, 74% don’t work in crypto & 95% male

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7732](https://eips.ethereum.org/EIPS/eip-7732): Enshrined proposer-builder separation (ePBS)
    
    - [EIP7735](https://github.com/ethereum/EIPs/pull/8723/files): Gas fee sponsorship
    
    - [EIP7736](https://github.com/ethereum/EIPs/pull/8724/files): Leaf-level state expiry in verkle trees 

- ERCs (application layer standards):
    - [ERC7731](https://github.com/ethereum/ERCs/pull/513/files): Vulnerability and exposure identifier
    
    - [ERC7734](https://github.com/ethereum/ERCs/pull/517/files): Decentralized identity verification (DID)

**Stuff for developers**

- Foundry forge-std [v1.9.0](https://github.com/foundry-rs/forge-std/releases/tag/v1.9.0): adds cheatcodes for a uint prompt, generate a random address/uint, invariant excludeSelector helper and deprecates console2; [v1.9.1](https://github.com/foundry-rs/forge-std/releases/tag/v1.9.1): adds missing console logs

- [EVMRepl](https://www.evmrepl.com/) (formerly Gas Playground): adds Solidity compilation errors

- Wevm [webauthn-p256](https://github.com/wevm/webauthn-p256#readme) (TypeScript): P256 signature utilities for WebAuthn

- [Stealth Address SDK](https://github.com/ScopeLift/stealth-address-sdk/#readme) v1 beta (TypeScript): work with EIP5564 & EIP6538 stealth addresses

**Security**

- [Immunefi Safe Harbor](https://mitchellamador.com/p/safe-harbor-the-making-of-a-new-security): implementation of Security Alliance (SEAL) whitehat safe harbor framework

**Enterprise**

- [Societe Generale-FORGE](https://www.sgforge.com/stablecoin-elevation/) EURCV stablecoin no longer permissioned to use

* * *

### Job Listings

- Aragon: [Senior Smart Contract Developer](https://jobs.lever.co/aragon/fba68080-9e98-49d7-8ed7-ac05d047d4b0)

- Privacy and Scaling Explorations: [ZK Circuits Engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 1.1 to 73.4 gwei, 5.5 gwei average; zero net issuance at 23.8 gwei 
    
    - 14k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,831 - $3,512, currently $2,990, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.053 (Flippening at ~0.16)

**Notable at app layer**

- Element DAO’s [Hyperdrive](https://blog.delv.tech/element-daos-hyperdrive-deployment-is-officially-live-on-mainnet/) (fixed/variable rate 6 month yields) live on mainnet

- [Moshicam](https://x.com/moshicamera/status/1807831995646726303) (onchain Instagram): mint photos with custom borders on Base

- [WannaBet](https://x.com/limes_eth/article/1808114375133413501): peer-to-peer betting, onchain escrow, designated judge

**Regulation/business/tokens**

- [Judge dismissed SEC claim](https://x.com/EleanorTerrett/status/1806896212173328850) that secondary BNB sales are securities, in case against Binance

- [Circle](https://x.com/jerallaire/status/1807791418489889279) USDC/EURC stablecoins EU MiCA compliant with reserves held in Europe

- [Logan Paul sues Coffeezilla](https://www.courtlistener.com/docket/68891856/1/paul-v-findeisen/) for defamation over CryptoZoo reporting

- [German government](https://x.com/ArkhamIntel/status/1809194916842512894) moved 2k BTC & [Mt Gox](https://x.com/ArkhamIntel/status/1809157408280772958) moved 47k BTC

**General**

- [EF updates mailing list](https://blog.ethereum.org/2024/07/02/blog-incident) compromised to email link to crypto drainer

- Twilio: [Authy account data](https://www.twilio.com/en-us/changelog/Security_Alert_Authy_App_Android_iOS) (including phone numbers) identified via unauthenticated endpoint

- [regreSSHion](https://blog.qualys.com/vulnerabilities-threat-research/2024/07/01/regresshion-remote-unauthenticated-code-execution-vulnerability-in-openssh-server): OpenSSH server remote code execution vulnerability

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-july-6-2024](https://weekinethereumnews.com/week-in-ethereum-news-july-6-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jul 7 – [Devcon scholars program](https://blog.ethereum.org/2024/06/07/devcon7-scholars) deadline

- Jul 9– [Devcon ticket raffle & auction](https://raffle.devcon.org/) deadline

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 29-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 2-4 – [Ethereum Argentina](https://ethereumargentina.org/) conference & hackathon

- Aug 7-9 – [Science of Blockchain Conference](https://www.sbc-conference.com/) (New York)

- Aug 15-17 – [Ethereum Uruguay](https://www.ethereumuruguay.org/) hackathon & conference

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Aug 23-26 – [ETHTokyo](https://www.ethtokyo.com/) hackathon & conference

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- Sep 5-8 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 9-15 – [ETHSafari](https://ethsafari.xyz/) (Kenya)

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 13-14 – [Ethereum México](https://ethmexico.org/)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Sep 26-27 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 4-6 – [Ethereum Kuala Lumpur](https://www.2024.ethkl.org/) conference & hackathon

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

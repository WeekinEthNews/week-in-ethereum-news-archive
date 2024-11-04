---
title: "Week in Ethereum News <br> November 2, 2024"
date: "2024-11-02"
---

## Eth News and Links

**Eth R&D protocol call (All Core Devs)**

- [Consensus layer focused protocol call](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-145-october-31-2024/21456) (ACDC #145):
    - **Pectra upgrade:**
        - [**Pectra-devnet-4**](https://pectra-devnet-4.ethpandaops.io/): testing going well
        
        - [**Mekong testnet**](https://mekong.ethpandaops.io/): Pectra public testnet live with devnet-4 spec
        
        - **Pectra-devnet-5**: minor spec changes merged, still finalizing spec
        
        - **EIP7742 uncouple blob count between CL/EL**: agreed simple change to blob base fee calculation but would be asymmetric if target increased to 4 with max 6 blobs per block
            - [Symmetric blob base fee adjustments](https://hackmd.io/@Nerolation/HJSGsd1Wkl) could be made in Fusaka upgrade with PeerDAS 

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- [Weekly testing call #11](https://ethereum-magicians.org/t/pectra-testing-call-11-october-28-2024/21494): fusaka-devnet-0 with EOF still ~1 week away

[**Fusaka**](https://eips.ethereum.org/EIPS/eip-7607) **(Osaka + Fulu) upgrade**

- [PeerDAS breakout #11](https://ethereum-magicians.org/t/peerdas-breakout-11-october-29-2024/21383): peerdas-devnet-3 died after a 100k slot reorg, peerdas-devnet-4 planned for end of November, will rebase on Pectra

- [EOF implementers call #61](https://ethereum-magicians.org/t/eof-implementers-call-61-october-30-2024/21388): spec change discussions

[**Amsterdam**](https://eips.ethereum.org/EIPS/eip-7773) **upgrade**

- [Kaustinen-7](https://verkle-gen-devnet-7.ethpandaops.io/) (Verkle testnet) live, use [lodestar-quickstart](https://github.com/ChainSafe/lodestar-quickstart/pull/55) to sync locally

**Layer 1**

- Terence: [blob transactions in FOCIL](https://hackmd.io/@ttsao/blob-focil) (Fork-Choice enforced Inclusion Lists) using execution layer blob pool

- [GossipSub potential improvements](https://vac.dev/rlog/gsub-largemsg-improvements/) for large message handling

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 27.8%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~52% majority
    
    - Consensus layer: Prysm 37% & Lighthouse 33.3%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Client Releases**

- Consensus layer:
    - Nimbus [v24.10.0](https://github.com/status-im/nimbus-eth2/releases/tag/v24.10.0): improvements to sync & validator client scalability
    
    - Teku [v24.10.3](https://github.com/Consensys/teku/releases/tag/24.10.3): improvements to GossipSub publishing & IDONTWANT usage

**For stakers**

- [Validator penalty simulator](https://portal.llamarisk.com/penalty/slashing): visualize slashing & inactivity penalties on a single validator

- Rocket Pool [Saturn 0 upgrade](https://docs.rocketpool.net/guides/saturn-0/whats-new#the-saturn-0-upgrade): 8 ETH mini pools with no RPL required

**Layer 2**

- Base [fault proofs](https://base.mirror.xyz/eOsedW4tm8MU5OhdGK107A9wsn-aU7MAb8f3edgX5Tk) live, to become a stage 1 rollup final step is using a security council for upgrades

- [Blob burn simulator](https://ethereum-blob-simulator.netlify.app/): visualize the impact of blob usage on ETH burn

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7799](https://eips.ethereum.org/EIPS/eip-7799): System logs
    
    - [EIP7801](https://github.com/ethereum/EIPs/pull/9004/files): eth/70 - sharded blocks protocol
    
    - [EIP7804](https://github.com/ethereum/EIPs/pull/9005/files): Withdrawal credential update request
    
    - [EIP7805](https://github.com/ethereum/EIPs/pull/9010/files): Committee-based Fork-Choice enforced Inclusion Lists (FOCIL)

- ERCs (application layer):
    - [ERC7798](https://github.com/ethereum/ERCs/pull/686/files): Tap to pay
    
    - [ERC7802](https://github.com/ethereum/ERCs/pull/692/files): Crosschain token interface
    
    - [ERC7803](https://github.com/ethereum/ERCs/pull/693/files): EIP712 extensions for account abstraction

**Stuff for developers**

- [Argot collective](https://argot.org/blog/hello-world): dev tools including Solidity & Sourcify spinning out of EF as a non-profit with 5-10 years of funding

- [Vyper (language) security](https://blog.vyperlang.org/posts/vyper-security/): audit coverage for key parts of codebase & ABI decoder fuzzer

- [Tornado Cash (rebuilt)](https://github.com/nkrishang/tornado-cash-rebuilt#readme): Foundry project with latest versions of Circom & snarkJS, for educational purposes

- Swiss knife [contract diff](https://contract-diff.swiss-knife.xyz/): compare verified contracts across chains using Etherscan API v2

- [Based agent](https://github.com/murrlincoln/Based-Agent/tree/main/Based-Agent#readme): create AI agent using Coinbase developer platform & OpenAI

- CTF:
    - [Bank challenge](https://github.com/Al-Qa-qa/bank-web3-security-tutorial#readme): sequence of 5 Solidity challenges using Foundry

**Security**

- Security Alliance (SEAL) [wargames drill scenario template](https://github.com/security-alliance/drill-template#readme)

**Ecosystem**

- More Vitalik explainers on Ethereum roadmap:
    - [Reduce storage & complexity (the Purge)](https://vitalik.eth.limo/general/2024/10/26/futures5.html): history expiry, state expiry and feature cleanup
    
    - [Fix everything else (the Splurge)](https://vitalik.eth.limo/general/2024/10/29/futures6.html): EVM improvements, account abstraction, EIP1559 improvements, verifiable delay functions (VDFs) and obfuscation + one-shot signatures

- Evan’s dumbing down of Vitalik’s roadmap explainers: [the Merge](https://x.com/evan_van_ness/status/1851499710835748939) & [the Surge](https://x.com/evan_van_ness/status/1851699900909502617)

- [ETHSydney](https://ethsydney-hackathon.devfolio.co/projects) hackathon projects 

**Enterprise**

- [Shift4 enabling merchants to accept crypto](https://www.shift4.com/blog/why-shift4-is-offering-crypto-payments), converted & settled in fiat, pilot Q4, rollout 2025

- [UBS asset management](https://www.ubs.com/global/tc/media/display-page-ndp/en-20241101-first-tokenized-investment-fund.html) launches tokenized investment fund

* * *

### Job Listings

- [Executive Director](https://docs.google.com/document/d/16qSjXRk2r9v6EnRRVSCoQjrPyJB6icoWgBkCxAme8Nc/edit) for Enterprise Ethereum Alliance

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 2.4 to 39.2 gwei, 8.8 gwei average; zero net issuance at 24.3 gwei 
    
    - 11.6k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,434 - $2,720, currently $2,514, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.036 (Flippening at ~0.164)

**Notable at app layer**

- [Synthetix proposal to acquire Kwenta](https://blog.synthetix.io/proposal-to-acquire-kwenta-and-relaunch-synthetix-exchange/) after spinning it out in 2020

- Limit Break [wrapped native](https://medium.com/limit-break/introducing-wrapped-native-a-modern-replacement-for-wrapped-ether-cc0431c8a964): updated WETH deployable on EVM chains with same address 

- [Tee\_hee\_he](https://x.com/sxysun1/status/1851581478683238637): AI agent on X run in TEE

- [Wallet security ranking](https://www.coinspect.com/wallets/): mobile & browser wallets evaluated against a checklist

**Regulation/business/tokens**

- [Immutable](https://x.com/Immutable/status/1852093814112161932) received Wells notice from SEC

- US Treasury: [crypto & Treasury markets presentation](https://home.treasury.gov/system/files/221/CombinedChargesforArchivesQ42024.pdf#page=107), benefits/risks of tokenizing Treasuries 

- [Roman Storm trial](https://www.coindesk.com/policy/2024/11/01/tornado-cash-developer-roman-storms-trial-pushed-to-april) moved to April

- [Temporary restraining order](https://x.com/diogenescasares/status/1852087198704898260) filed against Aragon for ANT redemption \[Update: TRO application withdrawn\]

- [Panama foundation vs Cayman-BVI explainer](https://x.com/wassielawyer/status/1850551931393151123) for token launches

- Layoffs: [Consensys](https://consensys.io/blog/consensys-path-to-long-term-sustainability-and-decentralization) 20%, [Kraken](https://www.nytimes.com/2024/10/30/technology/kraken-cryptocurrency-layoff-ceo.html) 15% & [dYdX](https://dydx.exchange/blog/letting-go) 35%

**General**

- [Lottie player](https://www.bleepingcomputer.com/news/security/lottiefiles-hacked-in-supply-chain-attack-to-steal-users-crypto/) (JavaScript animation) supply chain attack injected wallet drainer
    - [1inch](https://x.com/1inch/status/1851832307746742686) amongst impacted projects

- [MrBeast onchain activity](https://www.loock.io/blog/mrbeast-investigation) analyzed

- M2 (UAE exchange) [$13.7M stolen](https://rekt.news/m2-exchange-rekt/) from hot wallets

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-november-2-2024](https://weekinethereumnews.com/week-in-ethereum-news-november-2-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- **Nov 6 –** [**Gitcoin Grants 22**](https://www.gitcoin.co/blog/announcing-gitcoin-grants-22) **ends**

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

- **Dec 4-5 –** [**Columbia CryptoEconomics workshop**](http://columbiacryptoeconomics.org/) **(New York)**

- Dec 6-8 – [ETHIndia](https://ethindia.co/) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

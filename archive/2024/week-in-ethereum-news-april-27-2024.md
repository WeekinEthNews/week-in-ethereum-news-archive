---
title: "Week in Ethereum News <br> April 27, 2024"
date: "2024-04-27"
---

## Eth News and Links

**Pectra (Prague + Electra) upgrade (meta** [**EIP7600**](https://eips.ethereum.org/EIPS/eip-7600)**)**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=iLnBFPH-1Gc&t=191s).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1783544172894646675) & [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-186/):
    - **Pectra upgrade (small fork targeting late 2024)**
        - [**Pectra-devnet-0**](https://notes.ethereum.org/@ethpandaops/pectra-devnet-0#Client-implementation-tracker): added EIP7685 general purpose execution layer requests; client team implementations progressing though Erigon may be delayed as implementing on Erigon v3
        
        - **EIP3074**: discussions on DELEGATECALL, nonce, revocation, chain ID and some late account abstraction opposition; no changes for devnet-0, breakout planned
        
        - **EIPs added to Pectra considered for inclusion**:
            - EIP7212 secp256r1 precompile
        
        - **SSZ**: [async update](https://github.com/ethereum/pm/issues/1016#issuecomment-2077790649)
        
        - **EOF**: discussion on potentially reducing scope
        
        - **L1/L2 governance discussion**

**Osaka + F starname upgrade (meta** [**EIP7607**](https://eips.ethereum.org/EIPS/eip-7607)**)**

- Verkle:
    - Implementers [call video](https://www.youtube.com/watch?v=dbz6UPOT01U&t=6s) & [notes](https://twitter.com/rudolf6_/status/1783449448590541016): Kaustinen testnet v6 launched, presentations on [potentially storing Verkle state in Portal Network](https://ethresear.ch/t/portal-network-verkle/19339) and [Verkle + EOF](https://hackmd.io/@jsign/slides-eof-verkle#/)
    
    - [Are Verkle proofs more ZK friendly](https://hackmd.io/@dlubarov/B1rVbPgb0)? Daniel Lubarov says it depends

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.69%**](https://dune.com/hildobby/eth2-staking) **still too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~63% majority
    
    - Consensus layer: Prysm 38%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- ePBS:
    - Terence: [ePBS annotated validator spec](https://hackmd.io/@ttsao/epbs-annotated-validator)
    
    - Barnabe: [APS-Burn](https://mirror.xyz/barnabe.eth/QJ6W0mmyOwjec-2zuH6lZb0iEI2aYFB9gE-LHWIMzjQ), alternative to execution tickets for attester-proposer separation

- [Uncrowdable Inclusion Lists](https://ethresear.ch/t/uncrowdable-inclusion-lists-the-tension-between-chain-neutrality-preconfirmations-and-proposer-commitments/19372) to uphold chain neutrality

- [EIP7657 sync committee slashings](https://twitter.com/eawosikaa/status/1781659545846136876) explainer, improves security for light client bridges

- Ethereum Protocol Fellowship: [EPF.wiki](https://epf.wiki/) & [recap of cohort 4 projects](https://blog.ethereum.org/2024/04/22/epf-4-recap)

**Client Releases**

- Consensus layer:
    - Lodestar [v1.18.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.18.0): fixes cross-client, DVT & remote signer compatibility issues and defaults to local block if external builder less than 10% additional value
    
    - Teku [v24.4.0](https://github.com/Consensys/teku/releases/tag/24.4.0): performance improvements

- Execution layer:
    - Geth [v1.14.0](https://github.com/ethereum/go-ethereum/releases/tag/v1.14.0): defaults to pathdb, adds live tracing, drops support for pre-merge networks, pending block only constructed on demand and adds beacon chain light client
    
    - Nethermind [v1.26.0](https://github.com/NethermindEth/nethermind/releases/tag/1.26.0): adds snap server support and HalfPath state database upgrade
    
    - Reth [v0.2.0-beta.6](https://github.com/paradigmxyz/reth/releases/tag/v0.2.0-beta.6): fixes critical bug that would lead to invalid trie state and adds Discv5 support

**Layer 2**

- Optimism disclosed [two issues in FaultDisputeGame contract](https://blog.oplabs.co/sherlock-audit-roundup/) found by Offchain Labs

- [Blob market analysis](https://mirror.xyz/preconf.eth/6lZYL62DR9U14KC7wCC4RHReVdHcBeMy5PKeHVbPq5k): Base & Optimism use a blob-maximization strategy

**EIPs/Standards**

- EIPs:
    - [EIP7697](https://github.com/ethereum/EIPs/pull/8493/files): AUTHCREATE opcode
    
    - [EIP7698](https://github.com/ethereum/EIPs/pull/8498/files): EOF - creation transaction

- ERCs (application layer):
    - [ERC7699](https://github.com/ethereum/ERCs/pull/399/files): ERC20 payment reference extension

**Stuff for developers**

- Remix [v0.48](https://medium.com/remix-ide/remix-release-v0-48-0-0f256b049ff6): supports using multiple browser wallets (EIP6963), added PLONK scripts to zk proof templates and added CREATE2 factory for deploying

- Guide to [Hardhat Ignition contract verification on Etherscan](https://blog.nomic.foundation/how-to-verify-your-deployment-on-etherscan-with-hardhat-ignition-5cbb7ee6c7be)

- [Safe singleton factory deployer](https://github.com/wilsoncusack/safe-singleton-deployer-sol#readme) (Solidity): for using the factory with Foundry deployment scripts

- [Forge AlphaNet](https://github.com/paradigmxyz/forge-alphanet#readme) (Solidity): libraries for AlphaNet, EIP2537 BLS precompiles, RIP7212 Secp256r1 precompile and EIP3074 invokers

- Snekmate (Vyper contracts): [added Echidna-based property tests](https://github.com/pcaversaccio/snekmate/pull/239) for ERC20/721 contracts

- Guide to [integrate Permit2 into Vyper contracts](https://banteg.xyz/posts/vyper-permit2/)

- [Dpack-py](https://github.com/banteg/dpack#readme) (EVM packaging format): share addresses & artifacts to interact with contracts

- web3.py: [guide to Bloom filters](https://snakecharmers.ethereum.org/bloom-filters/)

- Tenderly [virtual testnets](https://blog.tenderly.co/how-virtual-testnets-replace-public-testnets/) for dapp developers, uses mainnet state, with a faucet, RPC, explorer & debugging tools  

- Privacy and Scaling Explorations [core program](https://pse-team.notion.site/PSE-Core-Program-2024-64ae61c3d7e74bf4bf9c15914ef22460): 8 week hybrid course for students in Japan, South Korea, Taiwan, Costa Rica, Ecuador & Argentina, apply by April 30

**Security**

- Magpie (cross-chain swaps) [$129k exploit](https://medium.com/@Magpieprotocol/magpie-protocol-smart-contract-vulnerability-post-mortem-f6400db0a25e) via position of function selector not being checked

- Rico [$36k exploit](https://twitter.com/ricocreditsys/status/1782172744362172681) on Arbitrum via flash loan entry point

**Ecosystem**

- [Reth (execution layer client) scaling roadmap](https://www.paradigm.xyz/2024/04/reth-perf) to 1 gigagas per second for L2
    - Péter Szilágyi (Geth): [would need heavy tradeoffs](https://twitter.com/peter_szilagyi/status/1783192981836603793)

- ETHGlobal [Scaling Ethereum finalists](https://twitter.com/ETHGlobal/status/1783907083487674737)

- Dan Finlay: [history of eth\_sign in MetaMask](https://blog.danfinlay.com/a-history-of-eth_sign-in-metamask/)

**Enterprise**

- [Stripe to support accepting stablecoin payments](https://techcrunch.com/2024/04/25/after-6-year-hiatus-stripe-to-start-taking-crypto-payments-starting-with-usdc-stablecoin/) mid-year

- Visa: [stablecoin dashboard](https://visaonchainanalytics.com/)

- EEA: [Week in Enterprise Ethereum News](https://twitter.com/EntEthAlliance/status/1782326155871207649) weekly newsletter

* * *

### Job Listings

- Nethermind: [Mechanism Designer](https://grnh.se/e78eb182teu) and [Research Engineer](https://grnh.se/887df932teu)

- Devcon: [Production Magician](https://jobs.lever.co/ethereumfoundation/aa4c69f8-f564-4036-9c5e-3e09f0eb27df) & [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/e93dae67-65a6-495c-8638-46e3db28cb64)

- EF: [People Operations Support](https://jobs.lever.co/ethereumfoundation/8054f5c5-ac89-4da8-98cc-738797837446)

- ChainSafe: [Developer Relations - Sygma](https://grnh.se/6627a6284us) and [Senior Product Manager](https://grnh.se/8736d15d4us)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 4.0 to 52.9 gwei, with 9.9 gwei average
    - Zero net issuance currently at 23.1 gwei 
    
    - 10k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,039 - $3,281, currently $3,089

- [ETHBTC](https://ratiogang.com/): currently 0.049 (Flippening at ~0.16)

**Notable at app layer**

- [ENS .box integration](https://blog.ens.domains/post/ens-integrates-dot-box): tokenized top level domain

- [Safe{Pass}](https://safe.global/blog/safe-pass-activity-program): points campaign announced to incentivize moving away from EOA

- Renzo [ezETH depegged](https://unchainedcrypto.com/renzos-ezeth-depeg-amid-criticism-of-airdrop-underlines-broader-risks-in-restaking/), airdrop criticized

- [Gitcoin Grants 20](https://grants.gitcoin.co/) live on Arbitrum; open source software rounds: infrastructure, dev tooling, apps and hackathon alumni

**Regulation/business/tokens**

- [Consensys received Wells notice](https://assets.ctfassets.net/gjyjx7gst9lo/2kfQoAKoQyQD1cw0HbVF3I/9c52c1e8754583c8f9b090e4b610de65/Consensys_v._Gensler_et_al.__Complaint_for_Declaratory_and_Injunctive_Relief__as-filed_.pdf) from SEC for allegedly violating securities laws with MetaMask Swaps & MetaMask Staking

- [Samourai wallet founders charged](https://www.justice.gov/usao-sdny/pr/founders-and-ceo-cryptocurrency-mixing-service-arrested-and-charged-money-laundering) in US for operating non-custodial Bitcoin coinjoiner

- [UK National Crime Agency & police](https://www.gov.uk/government/news/new-powers-to-seize-cryptoassets-used-by-criminals-go-live) gain power to seize crypto without an arrest

**General**

- Rekt: [ZKasino rugpull](https://rekt.news/zkasino-rekt/)

- Manuel Araoz: [tools to defend your attention](https://maraoz.com/2024/04/25/light-tech/)

- [Android TVs](https://twitter.com/matthew_d_green/status/1783493988881748157) can expose email inbox

- [Polygon zkEVM integrated optimal Ate pairing over BLS](https://twitter.com/EllipticHector/status/1783519685461299606) by taking the 381 bit field and overloading onto 256 bit registers

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-april-27-2024](https://weekinethereumnews.com/week-in-ethereum-news-april-27-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- May 7 – [Gitcoin Grants 20](https://grants.gitcoin.co/) ends

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

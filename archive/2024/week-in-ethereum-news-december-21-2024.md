---
title: "Week in Ethereum News <br> December 21, 2024"
date: "2024-12-21"
---

## Eth News and Links

**Eth R&D protocol call (All Core Devs)**

- [Execution layer focused protocol call](https://ethereum-magicians.org/t/all-core-devs-execution-acde-202-december-19-2024/21974) (ACDE #202):
    - **Pectra upgrade:**
        - [**Pectra-devnet-5 spec**](https://notes.ethereum.org/@ethpandaops/pectra-devnet-5):
            - Launch when enough clients are ready, testing locally with Teku & Besu
            
            - **EIP7840 blob schedule in EL config:** added to devnet
            
            - **EIP7702**: chain id changed to u256
            
            - **EIP2537 BLS precompile:** gas repricing finalized & redundant MUL precompiles removed
            
            - **System contracts:** audited, recommended minor changes for EIP2935, audits to be shared in January
    
    - **History expiry**: discussed [need for eth/70 protocol](https://notes.ethereum.org/JdRsfhU5Qz27THubjkstcA) to drop pre-merge data
    
    - **Gossip limit**: discussed decoupling gas limit & payload size
    
    - **eth/69**: agreed to not remove new block hashes as used by non-merged chains
    
    - **EIP7808 reserve tx-type range for RIPs**: approved
    
    - **Resource pricing**: working group starting to coordinate repricing efforts
        - [Hardware specs](https://hackmd.io/@kevaundray/S1hUQuV4Jx): feedback wanted on commodity node hardware

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- Reminder: [Mekong testnet](https://mekong.ethpandaops.io/) live for testing (pectra-devnet-4 spec)

- [Client testing call #17](https://ethereum-magicians.org/t/client-testing-call-17-december-16-2024/22247): tested increasing gas limit to 40M & didn’t hit 10MiB gossip limit

- Consensus layer specs [v1.5.0-alpha.10](https://github.com/ethereum/consensus-specs/releases/tag/v1.5.0-alpha.10)

**Layer 1**

- Gas limit increase:
    - [Gas limit signaling](https://gaslimit.pics/) dashboard, 20% of validators signalling to increase
    
    - [Coinbase validators signaling](https://x.com/samcmau/status/1869657320378253792) for an increase to 36M

- Data Always: [role of MEV-Boost relays in reorgs](https://collective.flashbots.net/t/the-role-of-relays-in-reorgs/4247)

- EIP7732 [ePBS breakout #14](https://ethereum-magicians.org/t/epbs-breakout-14-december-20-2024/22249): rebasing to Pectra, targeting interop for end of January

- Terence: [inclusion list committee](https://hackmd.io/@ttsao/il-committee-selection) selection approaches compared

**Research**

- Post-Quantum:
    - [Upgrade tasks for quantum resistance](https://ethresear.ch/t/tidbits-of-post-quantum-eth/21296): bip32, transaction signing, sender address recovery, precompiles & node discovery
    
    - [Upgrading to a post-quantum signature scheme](https://ethresear.ch/t/so-you-wanna-post-quantum-ethereum-transaction-signature/21291) such as Falcon via account abstraction, network upgrade or a hybrid

- [Attester-includer separation](https://ethresear.ch/t/towards-attester-includer-separation/21306): includers (inclusion list creators) rewarded with inclusion fees and have minimal hardware/capital requirements

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.4%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~43% & Nethermind ~36% (estimate based on 74% self reported data)
    
    - Consensus layer: **Prysm 34%**
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Client Releases**

- Consensus layer:
    - Lighthouse [v6.0.1](https://github.com/sigp/lighthouse/releases/tag/v6.0.1): patch for minor issues in v6
    
    - Lodestar [v1.24.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.24.0): adds engine\_getBlobsV1 support to get blobs from execution layer and adds experimental keymanager endpoint
    
    - Prysm [v5.2.0](https://github.com/prysmaticlabs/prysm/releases/tag/v5.2.0): QUIC enabled by default, adds engine\_getBlobsV1 support and fix for using MEV-Boost with a gas limit increase
    
    - Teku [v24.12.1](https://github.com/Consensys/teku/releases/tag/24.12.1): bug fixes

- Execution layer:
    - Besu [v24.12.2](https://github.com/hyperledger/besu/releases/tag/24.12.2): hotfix for users of account state overrides in eth\_call
    
    - Erigon [v3.0.0-alpha7](https://github.com/erigontech/erigon/releases/tag/v3.0.0-alpha7): faster eth\_getTransactionReceipt and return PrunedError when reading unavailable historical data

**For stakers**

- Ethstaker-deposit-cli [v1](https://github.com/eth-educators/ethstaker-deposit-cli/releases/tag/v1.0.0): generate validator keys, voluntary exit and add a withdrawal address to an existing validator

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7843](https://github.com/ethereum/EIPs/pull/9141/files): SLOT precompile

- ERCs (application layer):
    - [ERC7842](https://github.com/ethereum/ERCs/pull/728/files): State channel data types & interfaces
    
    - [ERC7844](https://github.com/ethereum/ERCs/pull/774/files): Consolidated dynamic storage
    
    - [ERC7845](https://github.com/ethereum/ERCs/pull/778/files): Minimal orchestrator RPC
    
    - [ERC7846](https://github.com/ethereum/ERCs/pull/779/files): Wallet connection API
    
    - [ERC7847](https://github.com/ethereum/ERCs/pull/782/files): Social media NFTs

**Stuff for developers**

- Foundry:
    - Forge-std [v1.9.5](https://github.com/foundry-rs/forge-std/releases/tag/v1.9.5): adds get broadcast cheat codes, mock call overloads and count for expect emit/revert

**Security**

- GemPad (launch pad) [~$2M exploit](https://rekt.news/gempad-rekt/) on mainnet, Base & BSC via reentrancy

- Security Alliance (SEAL): [LastPass users who stored private keys or seed phrases](https://x.com/_seal_org/status/1868805837311074576) prior to 2023, funds might be at risk

* * *

### Job Listings

- Nethermind: [Agentic Internship](https://job-boards.eu.greenhouse.io/nethermind/jobs/4490627101), [Snr Engineer](https://job-boards.eu.greenhouse.io/nethermind/jobs/4491847101), [Fullstack Lead](https://job-boards.eu.greenhouse.io/nethermind/jobs/4493512101) & [Fullstack](https://job-boards.eu.greenhouse.io/nethermind/jobs/4493501101) Go

- Vyper (Pythonic EVM language) seek a [DevRel](https://e63fu2j2ew4.typeform.com/to/Rt6A2juT)

- Mimic: [Tech Lead Engineer](https://mimic-fi.notion.site/Tech-Lead-Engineer-14b9958dbf4d80d88dadf252126e6375)

**Job listings: $600 for 4 issues** (75 char limit). [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.** Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 4.7 to 113.8 gwei, 15.2 gwei average; zero net issuance at 24 gwei
    
    - 6.3k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $3,113 - $4,078, currently $3,458 all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.035 (Flippening at ~0.164)

**Ecosystem**

- [Deep funding](https://deepfunding.org/) (retroactive grants for open source dependencies):
    - Models assign relative weights for the value that each dependency provides, spot checked by a human jury
    
    - $170k for 40k Ethereum dependencies assigned by models, $40k for best models & $40k for open source models

- Etherscan adds [account abstraction transactions](https://x.com/etherscan/status/1869347003123236986) support (ERC4337 user ops)

- [r/ethfinance subreddit merging](https://www.reddit.com/r/ethfinance/comments/1hhucz3/merge_make_ethereum_reddit_genuinely_excellent/) with r/ethereum

**Enterprise**

- Kraken [Ink](https://blog.kraken.com/news/ink-mainnet-launch) live using OP Stack

- [Deutsche Bank](https://archive.is/dY9Ym) building L2 using ZKsync tech

**Regulation/business/tokens**

- SEC:
    - [CyberKongz](https://x.com/cyberkongz/status/1868746903053127941) received Wells notice
    
    - (Gensler favorite) [Prometheum sued Matt Blumberg](https://x.com/matt_blumberg/status/1868787339226759422) for defamation

**General**

- [Polygon proposal to generate yield from bridged assets](https://rekt.news/burning-bridges/) abandoned after backlash

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-december-21-2024](https://weekinethereumnews.com/week-in-ethereum-news-december-21-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jan 20 – [Ethereum protocol attackathon](https://blog.ethereum.org/2024/11/25/ethereum-protocol-attackathon) ends

- **Jan 24-26 –** [**ETH Pondy**](https://www.ethpondy.xyz/) **(Puducherry) hackathon**

- Jan 30-31 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- **Feb 7-9 –** [**ETH Oxford**](https://ethoxford.io/) **hackathon**

- **Feb 10-16 –** [**ETHiopia**](https://eth-iopia.xyz/) **conference & hackathon**

- Feb 23 - Mar 2 – [ETHDenver](https://www.ethdenver.com/)

- **Apr 2-5 –** [**ETH Bucharest**](https://ethbucharest.ro/) **hackathon & conference**

- Apr 4-6 – [ETHGlobal Taipei](https://ethglobal.com/events/taipei) hackathon

- **May 9-10 –** [**ETHBratislava**](https://ethbratislava.com/) **conference & hackathon**

- May 9-11 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- **May 9-11 –** [**ETHLisbon**](https://ethlisbon.org/) **hackathon**

- May 27-29 – [ETHPrague](https://ethprague.com/) conference

- May 30 - Jun 1 – [ETHGlobal Prague](https://ethglobal.com/events/prague) hackathon

- Jun 3-8 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 12-13 – [Protocol Berg](https://protocol.berlin/) (Berlin) conference

- Jun 16-18 – [DappCon](https://dappcon.io/) (Berlin)

- Jun 26-28 – [ETHCluj](https://www.ethcluj.org/) (Romania) conference

- Jun 30 - Jul 3 – [EthCC](https://ethcc.io/) (Cannes) conference

- Jul 4-6 – [ETHGlobal Cannes](https://ethglobal.com/events/cannes) hackathon

- **Jul 16-19 –** [**NapulETH**](https://www.napuleth.org/) **(Napoli) conference**

- Aug 15-17 – [ETHGlobal New York](https://ethglobal.com/events/newyork2025) hackathon

- Sep 26-28 – [ETHGlobal New Delhi](https://ethglobal.com/events/newdelhi) hackathon

- Nov – [ETHGlobal Devconnect](https://ethglobal.com/events/ethglobal-devconnect) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

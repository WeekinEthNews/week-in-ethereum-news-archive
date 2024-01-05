---
title: "Week in Ethereum News <br> December 30, 2023"
date: "2023-12-29"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- No core devs call this week, next [all core devs - execution (ACDE) call](https://github.com/ethereum/pm/issues/931) January 4

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.62%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~84% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm 41%, any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Research**

- Vitalik’s [Proof of Stake simplification](https://ethresear.ch/t/sticking-to-8192-signatures-per-slot-post-ssf-how-and-why/17989) proposal, 3 approaches to cap signatures to 8192 per slot:
    - **DVT**: 4096 validators with minimum 4096 ETH deposit, solo stakers join DVT pools
    
    - **Two-tiered staking**: heavy layer (4096 ETH min deposit) finalizes and light layer (no min deposit) attests, heavy layer + 50% or more of online light layer to finalize a block
    
    - **Rotating participation**: randomly choose 4096 active validators, incentive weight decoupled from consensus weight

- [Execution tickets](https://ethresear.ch/t/execution-tickets/17944) (previously Attester-Proposer Separation): in-protocol ticket market, lottery to select beacon block proposer & attesters and lottery to select execution block proposer & attesters

- [Blob DA scaling overview](https://ethresear.ch/t/from-4844-to-danksharding-a-path-to-scaling-ethereum-da/18046): up to 128 blobs via 1D PeerDAS, then increase up to 256 blobs via 2D PeerDAS or full Danksharding

**MEV**

- [MEV-Boost auction model and bidding strategies](https://arxiv.org/abs/2312.14510) (naive, adaptive, last-minute & bluff bidding) show reducing latency optimizes builders performance 

- Rekt: [$1.3M paid to solo validator by searcher](https://rekt.news/moneyfornothing/) after user error adding liquidity

**Layer 2**

- zkSync Era [network issues](https://twitter.com/zkSyncDevs/status/1739395228233335154) post-mortem: safety procedure caused sequencer to wait for computed state update mismatch to be resolved

**EIPs/Standards**

- EIPs
    - [EIP7581](https://github.com/ethereum/EIPs/pull/8058/files): Increase block gas target and gaslimit

- ERCs (application layer):
    - [ERC7582](https://github.com/ethereum/ERCs/pull/170/files): Modular accounts with delegated validation (ERC4337 extension)
    
    - [ERC7583](https://github.com/ethereum/ERCs/pull/173/files): Inscription in smart contract
    
    - [ERC7584](https://github.com/ethereum/ERCs/pull/176/files): Linagee Name Registrar and Ethereum Content Delivery Network
    
    - [ERC7585](https://github.com/ethereum/ERCs/pull/177/files): MixHash and public data storage proofs

**Stuff for developers**

- Hardhat-chai-matchers [v2.0.3](https://github.com/NomicFoundation/hardhat/releases/tag/%40nomicfoundation/hardhat-chai-matchers%402.0.3): adds Addressable support in withArgs & equals

- Solidity memory safety: [avoid scratch space between assembly blocks](https://twitter.com/AmadiMichaels/status/1738538907258515710)

- xdeployer [v3.0.0](https://github.com/pcaversaccio/xdeployer/releases/tag/v3.0.0) (Hardhat plugin for deterministic address deployment): uses CreateX

- Halmos [v0.1.10](https://github.com/a16z/halmos/releases/tag/v0.1.10) (symbolic testing): reduces memory footprint, adds match-test & match-contract options and adds timeout & error failure modes

- EVMole [v0.3.1](https://github.com/cdump/evmole/releases/tag/0.3.1) (function selector extractor): adds Rust implementation

- [Ethernaut CTF solutions](https://github.com/Al-Qa-qa/ethernaut-solutions-foundry/) in Foundry

- [Sourcify](https://twitter.com/sourcifyeth/status/1740009724412936614) updates: containerized components, run components with custom configs and removes create2 verification

**Security**

- Trail of Bits: [ABI zero-sized types (ZSTs) DoS attack](https://blog.trailofbits.com/2023/12/29/billion-times-emptiness/) on ABI parsers

- [Solidity contract with view function verified on Etherscan](https://twitter.com/pcaversaccio/status/1739724912175059104) without view function declared

**Ecosystem**

- Vitalik: [make Ethereum cypherpunk again](https://vitalik.eth.limo/general/2023/12/28/cypherpunk.html)

- Etherscan: [multichain portfolio](https://twitter.com/etherscan/status/1738515605547049218) and advanced filter [time series chart](https://twitter.com/etherscan/status/1740707984928649230)

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 10.0 to 177.0 gwei, with 23.4 gwei average
    - Zero net issuance currently at 21.9 gwei 
    
    - 1k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,194 - $2,431, currently $2,279

- [ETHBTC](https://ratiogang.com/): currently 0.055 (Flippening at ~0.16)

**Notable at app layer**

- [Infinex](https://twitter.com/infinex_app/status/1738371497763447069) (perp trading) live on Base, web2 style UX, self-custody accounts, waitlist

- [Aave governance v3](https://twitter.com/aave/status/1739673359296999907) live, low cost voting on L2s & other chains, delegations reset

* * *

### Job Listings

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [BarnBridge](https://www.sec.gov/news/press-release/2023-258) $1.7M settlement with SEC for selling SMART yield bonds

- [India block 9 overseas centralized exchanges](https://www.coindesk.com/policy/2023/12/29/indias-local-crypto-and-web3-advocacy-body-asked-for-action-against-offshore-entities-source/) & issue show cause notices

**General**

- [Redditors report](https://www.reddit.com/r/mtgoxinsolvency/comments/18t7vv5/current_status_of_repayments/) Mt Gox fiat repayments to PayPal accounts

- [Thunder 87k ETH exploit](https://twitter.com/ThunderTerminal/status/1739843737860374845), wallet withdrawals via session tokens from MongoDB connection URL

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-30-2023](https://weekinethereumnews.com/week-in-ethereum-news-december-30-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jan 15 – EF’s [Next Billion fellowship cohort 4](https://fellowship.ethereum.foundation/) deadline

- Jan 17 – [Goerli testnet](https://github.com/ethereum/EIPs/pull/8051) Dencun upgrade epoch 231680

- Jan 30 – [Sepolia testnet](https://github.com/ethereum/EIPs/pull/8051) Dencun upgrade epoch 132608 (assuming no issues)

- Feb 2-4 – [ETH Cinco de Mayo](https://ethcincodemayo.com/) hackathon (Cholula, Puebla)

- Feb 3 – [Ethereum Lima Day](https://ethlimaday.org/)

- Feb 7 – [Holešky testnet](https://github.com/ethereum/EIPs/pull/8051) Dencun upgrade epoch 29696 (assuming no issues)

- Feb 23-Mar 3 – [ETHDenver](https://www.ethdenver.com/) BUIDLWeek & hackathon

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024) hackathon

- Mar 19-21 – [ETH Canal](http://ethcanal.xyz) (Panama City, Panamá) conference & hackathon

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) hackathon & conference 

- Mar 29-31 – [ETH Seoul](https://www.ethseoul.org/) conference

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) virtual hackathon

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- **Apr 12-14 –** [**ETHDam**](https://www.ethdam.com/) **(Amsterdam) conference & hackathon**

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/)

- **May 31-Jun 2 –** [**ETHDublin**](https://ethdublin.io/) **hackathon & conference**

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- **Jun 3-5 –** [**ETH Belgrade**](https://ethbelgrade.rs/) **conference**

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- **Jul 26-30 –** [**EDCON Tokyo**](https://www.edcon.io/) **conference** 

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov – [ETHGlobal DevCon](https://ethglobal.com/events/devcon2024) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

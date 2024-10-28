---
title: "Week in Ethereum News <br> October 26, 2024"
date: "2024-10-26"
---

## Eth News and Links

**Eth R&D protocol call (All Core Devs)**

- [Execution layer focused protocol call](https://ethereum-magicians.org/t/all-core-devs-execution-acde-199-october-24-2024/21355) (ACDE #199):
    - **Pectra upgrade:**
        - [**Pectra-devnet-4**](https://pectra-devnet-4.ethpandaops.io/): issues being debugged & fixed
        
        - **EIP2537 BLS precompile**: keeping subgroup checks, STARK projects unlikely to switch to using due to lack of infrastructure support
        
        - **EIP7742 uncouple blob count between CL/EL**: scheduled for inclusion in Pectra
    
    - **Gas limit (set by validators):** discussion on whether to increase validator defaults and what mechanism to use
    
    - **Engine API revert error codes**: proposal to standardize on Geth error codes

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- [Weekly testing call #10](https://ethereum-magicians.org/t/pectra-testing-call-10-october-21-2024/21441): peerdas-devnet-3 still unfinalized, fusaka-devnet-0 ~1 week away

[**Amsterdam**](https://eips.ethereum.org/EIPS/eip-7773) **upgrade**

- [Stateless implementers call #26](https://ethereum-magicians.org/t/stateless-implementers-call-26-october-21-2024/21442): upcoming Circle SNARK weekly seminars, [Verkle measurements](https://efdn.notion.site/Verkle-measurements-123d9895554180e6ac17eddf76c692b6) from replaying ~200k historical blocks and gas cost spec discussion

**Layer 1**

- EIP7732 ePBS:
    - [ePBS breakout #12](https://ethereum-magicians.org/t/epbs-breakout-12-october-25-2024/21455): support for [all-in-one fork choice](https://hackmd.io/UX7Vhsv8RTy8I49Uxez3Ng) proposal, devnet proceeding as planned, consensus specs can then be updated with fork choice proposal

- Xatu dataset adds [execution layer data](https://ethpandaops.io/posts/xatu-execution-layer/) in Parquet format from genesis

**Research**

- Anders Elowsson: [practical endgame on issuance policy](https://ethresear.ch/t/practical-endgame-on-issuance-policy/20747), proposes curves to temper growth or alternatively set a 0.5% issuance rate for now

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 27.9%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~52% majority
    
    - Consensus layer: Prysm 37% & Lighthouse 33.3%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Client Releases**

- Execution layer:
    - Erigon [v3.0.0-alpha5](https://github.com/erigontech/erigon/releases/tag/v3.0.0-alpha5): faster time on tip of chain, less time needed to download blobs, fix for v3.0.0-alpha4 crashes; resync required

**For stakers**

- [Update consensus layer clients](https://x.com/0xFrancisLi/status/1849469356410839462) so the network bandwidth changes of IDONTWANT messages can be observed

**Layer 2**

- [Helios](https://a16zcrypto.com/posts/article/scaling-ethereum-rollups-with-helios/) (light client): adds OP Stack support; [demo](https://helios.a16zcrypto.com/demo) syncing mainnet, OP Mainnet & Base

- Arbitrum One [time lock extended](https://www.tally.xyz/gov/arbitrum/proposal/27888300053486667232765715922683646778055572080881341292116987136155397805421) to 8 days (up from 3 days)

- [ApeChain](https://twitter.com/apecoin/status/1847731593437155673) (Arbitrum Orbit L3) live

- Arbitrum Orbit [fast withdrawals for AnyTrust chains](https://docs.arbitrum.io/launch-orbit-chain/how-tos/fast-withdrawals): up to 15 minute frequency, trust assumption on fast withdrawals committee

- L2 Standards [EVM equivalence breakout](https://ethereum-magicians.org/t/rollcall-8-1-breakout-future-of-the-evm-on-l2-october-23-2024/21312) (RollCall #8.1)

**EIPs/Standards**

- EIPs (Ethereum improvement proposals):
    - [EIP7791](https://github.com/ethereum/EIPs/pull/8980/files): GAS2ETH opcode
    
    - [EIP7792](https://eips.ethereum.org/EIPS/eip-7792): Verifiable logs
    
    - [EIP7793](https://github.com/ethereum/EIPs/pull/8981/files): TXINDEX opcode
    
    - [EIP7797](https://github.com/ethereum/EIPs/pull/8995/files): Double speed for hash\_tree\_root

- ERCs (application layer):
    - [ERC7794](https://github.com/ethereum/ERCs/pull/680/files): Grant registry
    
    - [ERC7795](https://github.com/ethereum/ERCs/pull/681/files): Wallet transaction intents
    
    - [ERC7796](https://github.com/ethereum/ERCs/pull/682/files): Conditional send transaction RPC

**Stuff for developers**

- Foundry forge-std [v1.9.4](https://github.com/foundry-rs/forge-std/releases/tag/v1.9.4): adds cheatcodes for gas snapshots, random bytes, mock calls, debug trace recording, remember keys & get wallets

- Remix [contract verification plugin](https://x.com/SourcifyEth/status/1849450860600021229): verify on Etherscan, Sourcify & Blockscout at the same time

- PRBMath [v4.1.0](https://github.com/PaulRBerg/prb-math/releases/tag/v4.1.0) (Solidity library): adds UD21x18 alias for uint128 & SD21x18 alias for int128

- [Etherscan API v2](https://info.etherscan.com/etherscan-api-v2-multichain/): multichain with single API key for all supported chains, beta

- Coinbase OnchainKit [Checkout](https://onchainkit.xyz/checkout/checkout) (React component): accepts USDC payments

- [Safe multisig transaction hashes](https://github.com/pcaversaccio/safe-tx-hashes-util#readme): Bash script to generate Safe transaction hashes to cross-check with Ledger; [Safe hash preview](https://www.safehashpreview.com/): hosted UI with additional trust assumptions

- [Veritas](https://github.com/0xbow-io/Veritas#readme): Circom circuit testing using Go

**Security**

- Tapioca DAO [$4.7M exploit](https://mirror.xyz/tapiocada0.eth/RVcRuKmJAavD05ObYsyYOHLDJ4gkEZKwyY_Y0Gx6gNc) via private key compromise starting with fake job offer on LinkedIn

- [DAO governance](https://blog.sigmaprime.io/governance-dao.html) common vulnerabilities

**Ecosystem**

- More Vitalik explainers on Ethereum roadmap:
    - [Minimize staking centralization risks (the Scourge)](https://vitalik.eth.limo/general/2024/10/20/futures3.html): fix block construction pipeline and staking economics 
    
    - [Easy block verification (the Verge)](https://vitalik.eth.limo/general/2024/10/23/futures4.html): stateless verification (Verkle or STARKs) and validity proofs of EVM execution & consensus

- Hackathon projects: [ETHGlobal San Francisco finalists](https://x.com/ethglobal/status/1848130391124656541) & [ETHSofia](https://dorahacks.io/hackathon/ethsofia/buidl)

**Enterprise**

- [Stripe acquiring Bridge](https://x.com/Stablecoin/status/1848390039975469094) (stablecoin payments) for a reported $1.1B

* * *

### Job Listings

- Sigma Prime is hiring Rust developers and security engineers. [Remote roles](https://github.com/sigp/positions-vacant)!

- [Executive Director](https://docs.google.com/document/d/16qSjXRk2r9v6EnRRVSCoQjrPyJB6icoWgBkCxAme8Nc/edit) for Enterprise Ethereum Alliance

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 3.4 to 96 gwei, 11.3 gwei average; zero net issuance at 24.2 gwei 
    
    - 11k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,399 - $2,747, currently $2,440, all time high $4,878

- [ETHBTC](https://ratiogang.com/): currently 0.037 (Flippening at ~0.164)

**Notable at app layer**

- Rune: [proposals to recenter Maker brand](https://forum.sky.money/t/success-of-the-usds-launch-and-the-opportunity-to-recenter-the-maker-brand/25383)

- Kain Warwick: retrospective of [Infinex patron sale](https://mirror.xyz/kain.eth/AfqSUcrBR6Y2Ylqrp9DK5zHe5N5sBoVPnH_Mit_Vuus) rather than a VC seed round

- Safe [multichain deployment](https://help.safe.global/en/articles/222612-deploying-a-multi-chain-safe): deploy at same address, no gas fees on major L2s

- [Gitcoin Grants 22](https://www.gitcoin.co/blog/announcing-gitcoin-grants-22): open source software rounds on Arbitrum; [mint attestations](https://www.gitcoin.co/blog/mint-attestations-capturing-your-impact) of donations

- **AD**: Buy an NFT to [tweet once as @evan\_van\_ness](https://opensea.io/assets/base/0xaa875a983746f2a5e9f7eccdc1bc988ca7ce4035/234). Auction ends Monday morning, some restrictions apply

**Regulation/business/tokens**

- Binance employee [Tigran Gambaryan released](https://www.wired.com/story/tigran-gambaryan-charges-dropped-nigeria/) from Nigeria

- WSJ reports that [Tether is under investigation by SDNY](https://archive.is/bCRd3); CEO [denies](https://x.com/paoloardoino/status/1849930663278833822)

**General**

- [Transak third party KYC vendor data breach](https://transak.com/blog/transak-security-incident-oct-2024) via compromised employee credentials

- [Secp256k1-node vulnerability](https://github.com/advisories/GHSA-584q-6j8j-r5pm) allows private key extraction over ECDH

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-october-26-2024](https://weekinethereumnews.com/week-in-ethereum-news-october-26-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

- Dec 6-8 – [ETHIndia](https://ethindia.co/) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

---
title: "Week in Ethereum News <br> October 21, 2023"
date: "2023-10-21"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=KD07crJXN9U&t=431s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-120/):
    - Devnet 9: testing found issue with conflicting blobs, to be [clarified in the spec](https://github.com/ethereum/consensus-specs/pull/3526)
    
    - Devnet 10: launch expected next week, waiting on KZG in clients (Go-KZG dependencies)

- Consensus-specs [v1.4.0-beta.3](https://github.com/ethereum/consensus-specs/releases/tag/v1.4.0-beta.3): mainnet KZG config and adds blob gossip condition

- Dencun interop testing [call video](https://www.youtube.com/watch?v=Pw5vl5wfqDQ&t=83s)

- Blob testing:
    - [Blobber](https://github.com/marioevz/blobber#readme): proxy between beacon & validator clients to modify blobs
    
    - Nethermind [send blobs](https://github.com/NethermindEth/nethermind/tree/master/tools/SendBlobs#readme): tool to send valid/invalid blobs

- KZG Ceremony: [verify transcript](https://hackmd.io/w7kvxwIhTlShzutKRKmRfA) & [buy a POAP](https://checkout.poap.xyz/151249) (~$0.25 for contributions that used Sign-in with Ethereum, currently no POAP for GitHub contributors)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.74%**](https://dune.com/hildobby/eth2-staking) **has reduced again but still far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~84% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm at 45%, any client bug over 33.3% could mean loss of finality

- [Geographic diversity needed for stakers & nodes](https://nodewatch.io/), particularly outside of US/Can/EU

**For Stakers**

- Validator [entry & exit queues reached zero](https://twitter.com/Wenmerge2022/status/1713441979655454928)

- [Lighthouse trialing QUIC support](https://lighthouse-blog.sigmaprime.io/Quic.html) for improved throughput & latency

**Client releases**

- Consensus layer:
    - Lighthouse [v4.5.444-exp](https://github.com/sigp/lighthouse/releases/tag/v4.5.444-exp): experimental tree-states to improve disk usage & state management, not recommended for mainnet, supports Deneb on devnets 
    
    - Nimbus [v23.10.0](https://github.com/status-im/nimbus-eth2/releases/tag/v23.10.0): performance improvements (mostly for large validator networks e.g. Holešky testnet)
    
    - Prysm [v4.1.0](https://github.com/prysmaticlabs/prysm/releases/tag/v4.1.0): Deneb foundations, reduced memory via multi-value slices, EIP4881 (deposit tree) for improved block processing, BLST v0.3.11 for improved portable build performance and multiarch containers preview

- Execution layer:
    - Geth [v1.13.4](https://github.com/ethereum/go-ethereum/releases/tag/v1.13.4): hotfix lowers warning log triggered by Erigon

**Research**

- Terence: [forward inclusion-list](https://ethresear.ch/t/specing-out-forward-inclusion-list-w-dedicated-gas-limits/17115) with dedicated gas limits

- [MEV-Burn](https://ethresear.ch/t/in-a-post-mev-burn-world-some-simulations-and-stats/17092) simulated stats

- [Total-Order Broadcast protocol](https://arxiv.org/abs/2310.11331) with single vote decisions in the Sleepy Model

**Layer 2**

- [Scroll](https://scroll.io/blog/founderLetter) (zk rollup) mainnet live 

**EIPs/Standards**

- EIPs
    - Meta [EIP7539](https://github.com/ethereum/EIPs/pull/7875/files): ERC extensions (naming conventions, metadata & procedures)
    
    - [EIP7541](https://github.com/ethereum/EIPs/pull/7880/files): Apply coinbase rewards at the end of block

- ERCs (application layer):
    - [ERC7536](https://github.com/ethereum/EIPs/pull/7853/files): Multi-edition NFT distribution
    
    - [ERC7537](https://github.com/ethereum/EIPs/pull/7855/files): Soulbound tokens
    
    - [ERC7538](https://github.com/ethereum/EIPs/pull/7873/files): Multiplicative tokens
    
    - [ERC7540](https://github.com/ethereum/EIPs/pull/7876/files): Asynchronous ERC4626 tokenized vaults

**Stuff for developers**

- Reminder: [Goerli testnet](https://github.com/eth-clients/goerli#readme) is deprecated, [Base](https://base.mirror.xyz/kkz1-KFdUwl0n23PdyBRtnFewvO48_m-fZNzPMJehM4) & [Arbitrum](https://twitter.com/arbitrumdevs/status/1714713920072557032) are migrating testnets to Sepolia

- Remix [Cookbook plugin](https://twitter.com/cookbook_dev/status/1714734999373803969) updated, one click code import

- [P256Verifier Vyper](https://github.com/pcaversaccio/p256-verifier-vyper#readme): contract for P256 signature verification rewritten in Vyper

- Slither [v0.10.0](https://github.com/crytic/slither/releases/tag/0.10.0): adds Vyper support, new detectors (incorrect-return, return-leave, incorrect-exp, tautological-compare & return-bomb), new printers (ck, halstead & martin) and improved Foundry support

- [Guide to multicall in dapps](https://coinsbench.com/optimizing-smart-contract-interactions-a-guide-to-multi-call-integration-in-web3-front-end-dapp-936331156b57) using wagmi

- noble-ciphers [v0.4](https://github.com/paulmillr/noble-ciphers/releases/tag/0.4.0): AES in pure JavaScript, useful for platforms such as React Native

- Personae [Sapir](https://github.com/personaelabs/sapir/tree/main#readme): client-side zk proving library, experimental, based on Spartan

**Security**

- HopeLend protocol [528 ETH exploit](https://twitter.com/blocksecteam/status/1714701696189034664) via precision loss, attack was frontrun with [assets later returned](https://twitter.com/Hope_money_/status/1715329752205312043)

**Ecosystem**

- Hackathons:
    - [Ethereum Kuala Lumpur](https://twitter.com/ETHKL1/status/1714237204942430613) finalists
    
    - [Huffathon](https://twitter.com/huff_language/status/1713961581212807369) winners

**Enterprise**

- [Reddit community points](https://www.reddit.com/r/CryptoCurrency/comments/17a33ql/serious_sunsetting_community_points_beta_and/) being sunset, due to scalability & regulatory environment

- [Ferrari accepting ETH & USDC payments](https://www.reuters.com/business/autos-transportation/ferrari-accept-crypto-payment-its-cars-us-2023-10-14/) for cars in US

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 4.0 to 123.6 gwei, with 9.1 gwei average
    - Zero net issuance currently at 21.5 gwei 
    
    - 9.4k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $1,546 - $1,627, currently $1,605

- [ETHBTC](https://ratiogang.com/): currently 0.054 (Flippening at ~0.16)

**Notable at app layer**

- PoolTogether [v5](https://pooltogether.mirror.xyz/CBvKNusRaaLJUSFH9ZQHureadrOF7eE7r6QsgqP2Oc8) live on Optimism, permissionless, enter via deposit in app or swap, prizes automatically sent

- Kain: [Synthetix experiments](https://mirror.xyz/kain.eth/lVhI3TWwpzPHSsFwUvcRFTz_8IBhdrOYC0ojtkvLbNY), deploy to Base, Optimism & Arbitrum with non-SNX collateral, deploy an optimized version of perps to mainnet and create a SNX chain using OP Stack

- Yearn [veYFI](https://twitter.com/yearnfi/status/1714971027980087603): ve-style tokenomics

- Rysk finance [atomic credit spreads](https://medium.rysk.finance/announcing-atomic-credit-spreads-ff2cca5c1472); \[[Starbloom](https://twitter.com/starbloomvent) portfolio\]

- [Uniswap Labs adds 0.15% fee](https://twitter.com/haydenzadams/status/1713987105666265113) for major token swaps via their UI, no fee for using protocol

* * *

### Job Listings

- Gnosis seek a [VP Technology](https://gnosis.jobs.personio.com/job/1267892?_pc=1517287), [Senior Web Devs (Wallet)](https://gnosis.jobs.personio.com/job/1239306?_pc=1517287&display=en) & [Backend Devs](https://gnosis.jobs.personio.com/job/1284509?_pc=1517287)

- EF Privacy & Scaling Explorations team seek a [Technical Project Coordinator](https://jobs.lever.co/ethereumfoundation/c826b9a1-ede0-465e-9639-f34029304374)

- [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db) wanted by EF

- eBay Web3 team seeking [Lead Solidity Engineer](https://jobs.ebayinc.com/us/en/job/R0060412/Lead-Solidity-Engineer)

- Aave seek a [UX Engineer](https://jobs.eu.lever.co/aave/2ce6fc26-729f-4cbf-a8f0-070321663262?lever-origin=applied&lever-source%5B%5D=WeekinEthereumNews) and a [Staff Rust Engineer](https://jobs.eu.lever.co/aave/46c3f25c-2c74-4b31-903e-bfbdfbd63d66?lever-origin=applied&lever-source%5B%5D=WeekinEthereumNews)

**Job listings: $600 for four issues** (75 character limit).  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [FinCEN propose adding mixing](https://www.fincen.gov/news/news-releases/fincen-proposes-new-regulation-enhance-transparency-convertible-virtual-currency) to list of primary money laundering concerns
    - Chainalysis: [role of crypto in terrorism financing vastly overestimated](https://www.chainalysis.com/blog/cryptocurrency-terrorism-financing-accuracy-check/)

- [NY Attorney General sues Gemini, Genesis & DCG](https://ag.ny.gov/press-release/2023/attorney-general-james-sues-cryptocurrency-companies-gemini-genesis-and-dcg) for allegedly defrauding investors

- [California Governor](https://twitter.com/milesjennings/status/1713993525245919299) signed web3 licensing regime into law

- European Central Bank: [digital euro](https://www.ecb.europa.eu/press/pr/date/2023/html/ecb.pr231018~111a014ae7.en.html) (CBDC) proceeding to 2 year preparation phase

- [Australian Treasury](https://treasury.gov.au/sites/default/files/2023-10/c2023-427004-proposal-paper-final.pdf) crypto regulation consultation paper

- Dozens of [ConsenSys early employees sue Joe Lubin](https://iapps.courts.state.ny.us/nyscef/ViewDocument?docIndex=o_PLUS_Rl1RtTIENwlGHZo2yB1g==) in US over alleged fraudulent transfer of MetaMask & Infura

**General**

- JP Kroning: [lower estimate of Americans owning crypto](https://jpkoning.blogspot.com/2023/10/crypto-adoption-in-america.html)

- Help [find the hash-seeds for the NIST curves](https://hackmd.io/@merkleplant/seeds-bounty) (P-192, P-224, P-256, P-384 & P-521)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-october-21-2023](https://weekinethereumnews.com/week-in-ethereum-news-october-21-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Oct 23 – Optimism’s [RetroPGF Round 3 application](https://app.optimism.io/retropgf-signup) deadline

- Oct 22-24 – [ETH Hong Kong](https://www.ethhongkong.co/)

- Oct 27-29 – [ETH London](https://www.encode.club/eth-london) hackathon

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Oct 28-30 – [Paradigm CTF](https://ctf.paradigm.xyz/)

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) deadline (max $1k for local meetups)

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- **Nov 15-29 –** [**Gitcoin Grants 19**](https://twitter.com/gitcoin/status/1715026016924737800)

- Nov 16-19 – [Pragma](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Nov 18 – [Ethereum Costa Rica](https://www.meetup.com/ethereumcr/events/295894129/)

- Dec 4-5 – [ETHVenice](https://ethvenice.com/)

- **Dec 6-7 –** [**Columbia CryptoEconomics workshop**](http://columbiacryptoeconomics.org/) **(New York)**

- Dec 8-10 – ETHGlobal [ETHIndia](https://ethindia.co/) (Bangalore) 

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

---
title: "Week in Ethereum News <br> October 15, 2022"
date: "2022-10-15"
---

## **Eth News and Links**

**Execution layer**

- Tim Beiko’s [core devs update](https://tim.mirror.xyz/zxOfNlTUO1MOhSrVP1rWGSywxlugdAc9fOUURW09zgE): Shanghai candidate EIPs, calls resume October 27
- Besu [v22.7.6](https://github.com/hyperledger/besu/releases/tag/22.7.6): hotfix for v22.7.x failed block proposals
- Erigon [v2.28.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.28.0): stability fixes & optimizations
- [Shandong](https://twitter.com/EFJavaScript/status/1581003267152412672): pre-Shanghai upgrade testnet, Lodestar + Ethereum JS EL client

**Consensus layer**

- Prysm developer [Prysmatic Labs acquired by Offchain Labs](https://offchain.medium.com/the-merge-2-0-offchain-labs-acquires-prysmatic-labs-the-leading-ethereum-consensus-client-team-9eab169c5fb6) (Arbitrum developer)
- Proposed [MEV-Boost development philosophy](https://collective.flashbots.net/t/mev-boost-development-philosophy/505)
- [MEV Watch](https://www.mevwatch.info/) of US OFAC censorship adds visualization of last 100 blocks
- Light client proxies; connect wallet to local RPC, calls are verified using proofs against latest block header:
    - [Nimbus](https://twitter.com/jcksie/status/1580201162846146565) light proxy
    - [Kevlar](https://github.com/shresthagrawal/kevlar#readme) CLI tool to run a light client-based RPC proxy, uses Lodestar API
- Nimbus [v22.10.1](https://github.com/status-im/nimbus-eth2/releases/tag/v22.10.1): light client REST API support and stability improvement when using an external block builder
- Teku [v22.10.1](https://github.com/ConsenSys/teku/releases/tag/22.10.1): bug fixes, optimizations and voluntary-exit command improvements
- Ben Edgington’s Upgrading Ethereum book & annotated spec [Bellatrix edition](https://eth2book.info/bellatrix/)
- Barnabe: [protocol-enforced proposer commitments](https://ethresear.ch/t/unbundling-pbs-towards-protocol-enforced-proposer-commitments-pepc/13879?u=barnabe) (PEPC) as possible alternative to opinionated in-protocol PBS

**EIPs/Standards**

- Ethereum Cat Herders [Learn-2-Earn](https://medium.com/ethereum-cat-herders/ech-introduces-learn2earn-43928a7cdd94): complete quizzes on EIPs to receive POAPs
- [ERCRef](https://ethereum-magicians.org/t/ercref-a-place-to-share-erc-implementations/11318): repository for ERC implementations
- [EIP5773](https://github.com/ethereum/EIPs/pull/5773/files): Multi-resource token

**Layer 2**

- Polygon zkEVM [public testnet](https://blog.polygon.technology/polygon-zkevm-public-testnet-the-next-chapter-for-ethereum/), open-source zk proving system

* * *

### **This newsletter is made possible thanks to** [**SpeedRunEthereum**](https://speedrunethereum.com/)**!**

![Speed Run Ethereum](https://weekinethereumnews.com/wp-content/uploads/2022/10/Speed-Run-Ethereum-banner.png)

Test your skills and learn how to build apps on Ethereum at [SpeedRunEthereum.com](https://SpeedRunEthereum.com).

* * *

**Stuff for developers**

- Foundry [inspect ir-optimized](https://twitter.com/w1nt3r_eth/status/1579486967963693057): view optimized Yul assembly generated from Solidity
- tincho’s intro pill to [fuzzing with Foundry](https://www.notonlyowner.com/learn/how-to-test-a-smart-contract-function-a-million-times/)
- [Auction Zoo](https://github.com/a16z/auction-zoo#readme): overcollateralized sealed-bid second-price (Vickery) auction in Solidity
- Simon de la Rouviere: [creating on-chain SVG capsule art NFTs](https://www.untitledfrontier.studio/blog/behind-the-scenes-crafting-the-on-chain-svg-capsules)
- [Bytepeep](https://github.com/kadenzipfel/bytepeep#readme): minimal bytecode peephole optimizer
- I am the chad v1: gas optimizor challenge [current winner](https://twitter.com/NoahCitron/status/1580359718341484544) & [second place](https://www.rileyholterhus.com/writing/optimizor)
- BlockSec [Phalcon transaction explorer](https://twitter.com/blocksecteam/status/1580937962652475396) adds simulation for specified block & position
- [ABI parser](https://abi-parser-nvk.vercel.app/): generates BigQuery SQL for events & functions of a verified contract
- wagmi [v0.7](https://twitter.com/wagmi_sh/status/1580591788611338240) (React hooks): infer types based on ABI & EIP712 Typed Data definitions
- [ReCap](https://blog.spruceid.com/extending-sign-in-with-ethereum-to-authorizations-recap/): Sign-In with Ethereum extended to add authorizations
- Guide to [building a Uniswap v3 clone](https://uniswapv3book.com/) using Foundry with a React front end
- [UniStark](https://medium.com/nethermind-eth/introducing-unistark-uniswap-only-warped-to-starknet-6b62d3a96690): Uniswap v3 transpiled to Cairo using Warp with manual modifications, [passes test suite](https://twitter.com/0xgreg_/status/1580291490655350784)
- [Maze](https://github.com/privacy-scaling-explorations/maze#readme): cli to aggregate Circom-PLONK proofs
- [nplate](https://github.com/whitenois3/nplate#readme): template for Noir (Aztec’s Rust-based language) projects

**Security**

- TempleDAO’s STAX [$2.3 million exploit](https://rekt.news/templedao-rekt/), missing access control
- QANX Bridge deployer [$1.2 million exploit](https://medium.com/qanplatform/qanx-bridge-wallet-disclosure-analysis-continuously-updated-724121bbbf9a), address generated using derivative of Profanity
- EFLeverVault [748 ETH exploit](https://twitter.com/danielvf/status/1580936010556661761), missing checks in flash loan callback, [MEV bot front run first transaction](https://twitter.com/MevRefund/status/1580917351217627136) for 480 ETH
- Rabby Swap [$200k exploit](https://twitter.com/Rabby_io/status/1579819525494960128), arbitrary external call, revoke approvals
- Curve LP oracle [vulnerability disclosed](https://chainsecurity.com/heartbreaks-curve-lp-oracles/), read-only reentrancy, $100 million was at risk

**Ecosystem**

- Devcon Bogotá [opening ceremonies](https://archive.devcon.org/archive/playlists/devcon-6-opening/)
- ETHBogotá [finalists](https://twitter.com/ethglobal/status/1579249265557192704)
- Infinite Hackathon Bogotá [winner](https://twitter.com/InfiniteHackETH/status/1579462128871710720)
- EF [fellows cohort 2](https://blog.ethereum.org/2022/10/10/ef-fellowship-cohort-2)

**Application layer**

- Uniswap [web app](https://uniswap.org/blog/refreshed-web-app): adds token data, discovery and search
- Polynomial [Portal](https://mirror.xyz/0xf3897707d8Fa5dC27b2A6575319e409a464eB8D8/E030dcsEQEEHWlUa7EhPei3A56FdqbHQr9OPjMp16nE) one-click deposit on any chain bridges to Optimism, converts to Synths & deposits into vault
- [Dolomite](https://medium.com/dolomite-official/dolomite-launches-margin-protocol-and-dex-our-journey-begins-862777432414) margin protocol & DEX live on Arbitrum
- Timeless [Bunni](https://twitter.com/Timeless_Fi/status/1580713579971366913): represents LP positions as ERC20 tokens instead of NFTs
- 0xSplits [Waterfall](https://0xsplits.mirror.xyz/TQTsLgiRZ76-r3C_OvP7FyYaN3JIS1RanIrqTHrZ1EA): tiered payouts using fixed amounts, live on mainnet & Optimism
- [Google search](https://twitter.com/hhua_/status/1579700083314282496) displays Ether balance from Etherscan when searching an address
- [NFT Embed](https://medium.com/graviton-xyz/nft-embed-new-features-alert-643bec22ec0b) adds embedding in Medium, WordPress & Webflow and aggregates listings
- Quix [Optimism NFT bridge](https://mirror.xyz/0xB1EA5a3E5EA7fA1834d48058EcDa26d8c59e8251/wlHiInzN5noCQKwRmNcdNMiTS8vfW2a68iI5NSmMGnk) from mainnet
- [Gitcoin propose to delay Grants Round 16](https://gov.gitcoin.co/t/request-for-feedback-proposed-future-for-the-grant-programs-and-gr16-as-we-transition-to-the-protocol/11624) until 2023 to focus on decentralized protocol

* * *

### **Job Listings**

- [Research scientist](https://jobs.lever.co/ethereumfoundation/cd2382ec-abbd-493b-b942-b5e2a61a6c0a) wanted for EF Robust Incentives Group
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- [Join Llama](https://zenith-caboc-8a4.notion.site/Join-Llama-ad66be1cb28541f5b5346aa37d192b79) to help build the future of protocol DAOs: [Solidity](https://zenith-caboc-8a4.notion.site/Smart-Contract-Engineer-ef9426f7cfef4f0d90b596aaeff216e0) and [Backend](https://zenith-caboc-8a4.notion.site/Senior-Backend-Engineer-6a096e7937c248f4a90fba08c3bf14ae)

**Job listings: $600** for four issues (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Coin Center suing US OFAC](https://www.coincenter.org/coin-center-is-suing-ofac-over-its-tornado-cash-sanction/) over Tornado Cash sanction
- BNY Mellon [crypto custody platform](https://www.bnymellon.com/us/en/about-us/newsroom/press-release/bny-mellon-launches-new-digital-asset-custody-platform-130305.html) live in US
- [Bittrex settles with US Treasury](https://home.treasury.gov/news/press-releases/jy1006) OFAC for $25 million & FinCEN for $29 million
- [Financial accounting standards board](https://taxbit.com/blog/fasb-allows-fair-value-treatment-for-crypto-assets) (FASB) voted to account for crypto at fair value
- Searchable [Celsius data](https://celsiusnetworth.com/) of losses by user
- [Tether](https://tether.to/en/tether-slashes-commercial-paper-to-zero/) replaced commercial paper reserves with US Treasury Bills

**General**

- [L2BEAT bridges](https://l2beat.com/bridges/tvl/) dashboard, displays TVL & risk analysis
- DeFiLlama dashboard of [project hacks](https://defillama.com/hacks)
- [Microsoft Windows RPC vulnerabilities disclosed](https://www.akamai.com/blog/security-research/cold-hard-cache-bypassing-rpc-with-cache-abuse), security callback mechanism bypassed by caching

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-october-15-2022](https://weekinethereumnews.com/week-in-ethereum-news-october-15-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Oct 18-23 – [Eth Medellin](https://www.ethmedellin.co/) (Colombia)
- Oct 26-28 – [Eth Panama](https://www.ethpanama.com/)
- Oct 28-30 – [ETH Lisbon](https://www.ethlisbon.org/)
- Oct 31 – [Merge data challenge](https://esp.ethereum.foundation/merge-data-challenge) deadline
- Oct 31-Nov 10 – Clr.fund [LatAm round](https://ethcolombia.clr.fund/)
- Nov 3 – US Treasury [digital assets RFC](https://public-inspection.federalregister.gov/2022-20279.pdf) \[PDF\] deadline
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 11-13 – [ETHBrno](https://mirror.xyz/ethbrno.eth/6BH9cUVuD85hy5O0L5cOOOE7niSA9Yo5eWsXVzKOlO4) (Czech Republic)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Nov 25-27 – [ETH Vietnam](https://www.eth-vietnam.com/)
- Nov 26-30 – [ETH Miami](https://ethmiami.net/)
- **Dec 1 –** [**Columbia cryptoeconomics workshop**](https://bit.ly/columbiacryptoeconomics) **(New York)**
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

---
title: "Week in Ethereum News <br> December 10, 2022"
date: "2022-12-10"
---

## **Eth News and Links**

**Shapella (Shanghai + Capella) upgrade**

- Latest core devs [call video](https://www.youtube.com/watch?v=y8jZ11_CQGo&t=323s).  Summary by [Tim Beiko](https://twitter.com/abcoathup/status/1601052402274033664).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1600936500832899072) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-call-151/):
    - Shanghai confirmed to target March prioritizing withdrawals plus warm COINBASE, PUSH0 & limit/meter initcode
    
    - EOF EIPs (3540, 3670, 4200, 4750, 5450) will be included in Shanghai only if implementations tested by January 5 _and_ devnets successful by January 19
    
    - EIP4844 agreed as main feature for next upgrade quickly after Shanghai ([Cancun](https://github.com/ethereum/execution-specs/pull/663)), with EIP1153 (transient storage) & EIP2537 (BLS precompile) as candidates for inclusion

- [Withdrawals impact](https://twitter.com/terencechain/status/1599781623687700482) on builder layer: relays & builders just need to run correct client versions

- Unified [EOF specification](https://notes.ethereum.org/@ipsilon/eof1-unified-specification)

- [EOF benefits](https://twitter.com/leonardoalt/status/1600845724618326016): gas savings, increased security, simpler optimizations and easier debugging

**Layer 1**

- EIP4844 implementer [call video](https://www.youtube.com/watch?v=2lSGS9weOv0) and [notes](https://twitter.com/terencechain/status/1600195265700339713)

- SELFDESTRUCT [removal analysis](https://hackmd.io/X-waAY49SrW9i36SKOVuGQ)

- [Reth](https://www.paradigm.xyz/2022/12/reth) (EL client in Rust): open sourced, full sync support expected Q1

- Endpoint proposal so [DVT validator clients can support committee aggregations](https://blog.obol.tech/committee-aggregations-with-distributed-validators/)

- Verkle tree [PoS testnet](https://twitter.com/gballet/status/1600088800943710209) (Beverly Hills)

- Protolambda’s [history of PoS spec releases & testnets](https://twitter.com/protolambda/status/1599437869994496000)

**For stakers**

- New MEV-Boost non-censoring relay: [Aestus](https://aestus.live/)

**Client releases**

- Consensus Layer:
    - Teku [v22.12.0](https://github.com/ConsenSys/teku/releases/tag/22.12.0): dependencies updated

- Execution Layer:
    - Besu [v22.10.2](https://github.com/hyperledger/besu/releases/tag/22.10.2): hotfix for segfaults in v22.10.1
    
    - Erigon [v2.31.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.31.0): eth/66 & eth/67 devp2p support and optimized eth\_estimateGas RPC

**Layer 2**

- zkSync v2.0 [L1 to L2](https://twitter.com/bkiepuszewski/status/1600792830129016832) and [L2 to L1](https://twitter.com/bkiepuszewski/status/1601138527508393990) message passing

- Tincho: [Arbitrum bridge griefing attack](https://www.notonlyowner.com/research/message-traps-in-the-arbitrum-bridge), relayer could have unbounded gas consumption

**EIPs/Standards**

- [EIP6077](https://github.com/ethereum/EIPs/pull/6077/files): Invalidation abstraction for signature-based operations powered by ERC712

- [EIP6093](https://github.com/ethereum/EIPs/pull/6093/files): Custom errors for ERC tokens

- [EIP6105](https://github.com/ethereum/EIPs/pull/6105/files): Marketplace extension for ERC721

- [EIP6110](https://github.com/ethereum/EIPs/pull/6110/files): Supply validator deposits on chain

* * *

### **This newsletter is made possible thanks to** [**Tenderly**](https://tenderly.co/)**’s new** [**Web3 Gateway**](https://dashboard.tenderly.co/register?redirectTo=gateways)**!**

![Tenderly Web3 Gateway](https://weekinethereumnews.com/wp-content/uploads/2022/12/tenderly-1024x439.jpg)

The Tenderly platform enables Web3 developers to build, test, monitor, and operate smart contracts in one place. To cover each aspect of the dapp development lifecycle, Tenderly expanded its product offering and released Tenderly Web3 Gateway. This is a production node as a service that delivers fast and easy access to the blockchain.

Tenderly Web3 Gateway is fully integrated with the rest of the platform, combining infrastructure with development tooling and observability. It enables blockchain developers to:

- Speed up read-heavy workloads up to eight times

- Set up reliable node infrastructure with 100% blockchain data consistency

- Reduce node infrastructure management overhead

- Scale dapps with ease to meet their growing user base

- Unify dapp development by combining infrastructure with tooling and observability

- Improve development teams’ velocity and collaboration by eliminating development silos

- Preview transaction outcomes directly from Tenderly Web3 Gateway before sending them on-chain

[Try Tenderly Web3 Gateway](https://dashboard.tenderly.co/register?redirectTo=gateways).

* * *

**Stuff for developers**

- Solidity [roadmap](https://github.com/orgs/ethereum/projects/26) & [developer survey](https://blog.soliditylang.org/2022/12/07/solidity-developer-survey-2022-announcement/)

- Fe (language) [bug bounty](https://blog.fe-lang.org/posts/bountiful-break-things-and-get-paid/) contest [cracked via bug in 15-puzzle implementation](https://twitter.com/plotchy/status/1600894668304105474)

- [Testnet ETH](https://collect-test-eth.org/) for contract deployers, one time claim of 10 Sepolia & Goerli ETH

- [3D roller coaster](https://twitter.com/xtremetom/status/1600542212735090711): generated on-chain, proof of concept

- List of beginner [developer resources](https://github.com/edakturk14/ethereum-developer-resources#readme)

- Sol2uml [v2.3.0](https://github.com/naddison36/sol2uml/releases/tag/v2.3.0): (UML generator from Solidity) adds squash feature

- samczsun’s [abi-guesser](https://github.com/samczsun/abi-guesser#readme): TypeScript library to guess type of ABI-encoded data

- Guide to using [VanillaJS to interact with a contract](https://codingwithmanny.medium.com/use-vanillajs-to-connect-to-metamask-read-from-a-contract-write-to-a-contract-7a3d213ac438) via MetaMask

- [Grim-reaper](https://github.com/massun-onibakuchi/grim-reaper#readme): Aave v3 on-chain liquidation bot in Huff

- Optimism’s [BaseServiceV2](https://twitter.com/kelvinfichter/status/1601061812648448000): base class for long running TypeScript services

- [React-native-helios](https://github.com/cawfree/react-native-helios#readme): wrapper for Helios light client, runnable in Expo

- [Semaphore boilerplate](https://github.com/semaphore-protocol/boilerplate#readme): web app components for users to create IDs & leave feedback; [demo](https://main.d3rb6vhozk5q4b.amplifyapp.com/)

**Security**

- [Hybrid Echidna](https://blog.trailofbits.com/2022/12/08/hybrid-echidna-fuzzing-optik-maat/): Echidna (property based fuzzer) + Maat (symbolic execution framework) improves on random fuzzing by using symbolic analysis to generate fuzzing inputs

**Ecosystem**

- Ethereum Foundation:
    - Attitudes to [staking survey](https://stakingsurvey.paperform.co/)
    
    - Merge data challenge [winners](https://blog.ethereum.org/2022/12/05/merge-data-challenge-results) from 45 data & analysis blog posts
    
    - [Q3 grantees](https://blog.ethereum.org/2022/12/07/esp-allocation-q3-22) share $8 million in funding

- Clr.fund [LatAm grants round](https://ethcolombia.clr.fund/#/leaderboard) recipients

- Protocol Guild (core protocol contributors) [first six months of pilot](https://twitter.com/protocolguild/status/1600912258694930432), $5 million distributed of $9.7 million donated

- ETHIndia (ETHGlobal) [projects](https://ethindia2022.devfolio.co/projects)

- [Christian Reitwiessner stepped down](https://blog.soliditylang.org/2022/12/05/solidity-core-team-updates/) as Solidity Team Lead

- New Ethereum wiki: [Inevitable Ethereum](https://inevitableeth.com/)

**Enterprise**

- [EY’s Nightfall v3](https://www.reddit.com/r/ethfinance/comments/zdajlx/so_what_happened_to_nightfall/) to be decentralized, enterprise only and deployed by the community

**Application layer**

- [Maker D3M](https://twitter.com/MakerDAO/status/1599787972664115200) integrating with Compound to provide a predictable 2% borrow rate for Dai

- DeFi Saver [Compound v3 extension](https://blog.defisaver.com/defi-saver-compound-extension-improved-eoa-support/) so that users don’t need to create a proxy contract

- [OpenSea](https://twitter.com/opensea/status/1600913295300792321) cutoff for creator fee enforcement extended to January 2, optional creator fees allowed and ownership of Operator Filter Registry being transferred to a collective

- [Orthogonal Trading defaults](https://maple.finance/news/maple-severs-all-ties-with-orthogonal-trading/) on loans via Maple Finance

- Vitalik’s [application areas that excite](https://vitalik.ca/general/2022/12/05/excited.html): money, DeFi, identity, DAOs & hybrid apps

* * *

### Job Listings

- EF Robust Incentives Group seek a [research scientist](https://jobs.lever.co/ethereumfoundation/cd2382ec-abbd-493b-b942-b5e2a61a6c0a)

- [Code integration tester](https://jobs.lever.co/ethereumfoundation/6feeb8cb-bd05-4f24-9fda-9ba3be98e5a4) wanted by Ethereum Foundation

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Video of [SBF admitting to commingling assets](https://www.youtube.com/watch?v=4o_jPzBZSIo)

- SBF secretly funded [the 2021 buyout of The Block](https://www.axios.com/2022/12/09/bankman-fried-funded-crypto-news-site-block), plus millions to The Block’s new owner

- [Binance caused gas prices to spike](https://twitter.com/binance/status/1601273556142551040) as they moved funds around to prepare for audit

**General**

- Skiff [calendar](https://skiff.com/calendar): end-to-end encrypted

- [Apple](https://www.apple.com/newsroom/2022/12/apple-advances-user-security-with-powerful-new-data-protections/) adding opt-in iCloud end-to-end encryption for photos & backups, physical key sign in for Apple ID & iMessage contact key verification

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-10-2022](https://weekinethereumnews.com/week-in-ethereum-news-december-10-2022)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- **Dec 20 –** [**Attitudes to staking survey**](https://stakingsurvey.paperform.co/) **deadline**

- **Jan 8 –** [**Solidity developer survey**](https://blog.soliditylang.org/2022/12/07/solidity-developer-survey-2022-announcement/) **deadline**

- **Jan 17-31 –** [**Gitcoin grants round**](https://go.gitcoin.co/blog/announcing-the-gitcoin-alpha-tests)

- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

- Mar 15-16 – [ETHDubai](https://www.ethdubaiconf.org/)

- **Apr 3-6 –** [**Edcon**](https://edcon.io/) **Vienna**

- **Apr 12-14 –** [**NFT NYC**](https://www.nft.nyc/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

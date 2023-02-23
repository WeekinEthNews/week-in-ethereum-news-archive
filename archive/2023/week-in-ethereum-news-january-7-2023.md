---
title: "Week in Ethereum News <br> January 7, 2023"
date: "2023-01-07"
---

## **Eth News and Links**

**Shapella (Shanghai + Capella) upgrade**

- Latest core devs execution [call video](https://www.youtube.com/watch?v=SmcMwdHZqg8&t=116s).  Summary by [Tim Beiko](https://twitter.com/abcoathup/status/1611111538336878592).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1611042386611929089) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-execution-call-152/):
    - **EOF removed from Shanghai** to not delay withdrawals
    
    - No other EIPs being added e.g. EIP1153 (transient storage)
    
    - Withdrawal-devnet-1 running with all client combinations
    
    - **Contract devs**: EIP3860 (limit & meter initcode) changing to error with out of gas exception
    
    - Discussion on including SSZ withdrawal roots on execution layer for light clients

- Consensus specs [v1.3.0-rc.0](https://github.com/ethereum/consensus-specs/releases/tag/v1.3.0-rc.0): Capella specs feature complete & stable unless unexpected issues

**Cancun + D-starname upgrade**

- EIP4844 (proto-danksharding) implementers [call notes](https://twitter.com/terencechain/status/1610333893735124993)

- KZG ceremony:
    - [Security review](https://github.com/ethereum/kzg-ceremony/blob/main/Sigma_Prime_Ethereum_Foundation_KZG_Ceremony_Security_Assessment.pdf) \[PDF\] of sequencer in Rust & front end in React
    
    - Implementing [powers of tau contributor](https://arnaucube.com/blog/powersoftau.html)
    
    - Powers of Tau [ceremony client](https://github.com/jsign/go-kzg-ceremony-client#readme) in Go, optional entropy from http endpoint & drand network

**Layer 1**

- [Core devs & consensus calls renamed](https://github.com/ethereum/pm#ethereum-project-management-repository) to core devs call execution (ACDE) & consensus (ACDC)

- Proposal for [EOF v2](https://notes.ethereum.org/@ipsilon/eof2-proposal) including Vitalik’s idea to ban code introspection

- [Mevboost.pics](https://twitter.com/nero_eth/status/1609491027043225600) adds block builder slot share over time

- ERC4337 (account abstraction) decentralized mempool [working group notes](https://github.com/JohnRising/4337-bundler-working-group/blob/main/20230104%20Meeting%20Notes.md)

**Client releases**

- Consensus Layer
    - Lodestar [v1.3.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.3.0): networking & performance improvements and keymanager API conformance

**Layer 2**

- Options for [zkEVMs to price gas](https://twitter.com/_bfarmer/status/1611223861604892673)

- L2beat: [LayerZero bridge security](https://medium.com/l2beat/circumventing-layer-zero-5e9f652a5d3e) is fundamentally a trusted model

**EIPs/Standards**

- [EIP6212](https://github.com/ethereum/EIPs/pull/6260/files): Buyable NFT tokens on-chain and royalties

- [EIP6268](https://github.com/ethereum/EIPs/pull/6268/files): Non transferability indicator for ERC1155

- [EIP6269](https://github.com/ethereum/EIPs/pull/6269/files): Full EVM equivalence

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

- [Solidity compiler appends encoded IPFS hash of contract metadata](https://mirror.xyz/joenrv.eth/DdbK6GR-CkeYxHoU8sKl0AFYbGeQwZcvCM5Qvzipr0g) to bytecode for verification

- Guide to [using PrevRandao](https://soliditydeveloper.com/prevrandao)

- Paul Berg: [Solidity supports functions as parameters](https://twitter.com/paulrberg/status/1609917508223475712), useful in testing e.g. [Seaport](https://github.com/ProjectOpenSea/seaport/blob/1.2/test/foundry/FulfillOrderTest.t.sol#L64-L71)

- [EVM quirks](https://twitter.com/jtriley_eth/status/1609216690147020803) and how they are handled in Solidity & Vyper

- [Setup remixd](https://jamesbachini.com/remixd-tutorial/) to use Remix with local filesystem

- CTFs:
    - [Mr Steal Yo Crypto](https://mrstealyocrypto.xyz/), uses Hardhat
    
    - Making of [HappyNewYear CTF](https://mirror.xyz/vicnaum.eth/reNCgNs7e0rDNx7h8Yt0a9xbS7wFss4950Dl8tYr2kY)
    
    - Damn Vulnerable DeFi [backdoor solution](https://stermi.xyz/blog/damn-vulnerable-defi-challenge-11-solution-backdoor)
    
    - [Shop puzzle](https://twitter.com/0xCygaar/status/1610114831000170496) & solution
    
    - Secureum bootcamp [race-13 quiz solution](https://ventral.digital/posts/2023/1/3/race-13-of-the-secureum-bootcamp-epoch)

- [TurboETH](https://twitter.com/KamesGeraghty/status/1609872647965261825): dapp build system, app template, ERC20 & ERC721 components & hooks, beta

- Use TrueBlocks to [find all contracts created by an address](https://tjayrush.medium.com/recipe-factories-ce78fa4c5f5b)

- [Guide to equivalence checking](https://www.truscova.com/blog_article_2.php) Solidity functionality with a reference implementation using Z3 theorem prover

- [UniRep protocol](https://mirror.xyz/privacy-scaling-explorations.eth/FCVVfy-TQ6R7_wavKj1lCr5dd1zqRvwjnDOYRM5NtsE): private & non-repudiable reputation system

**Security**

- [Circom-pairing library](https://medium.com/veridise/circom-pairing-a-million-dollar-zk-bug-caught-early-c5624b278f25) vulnerability disclosed, missing data validation

**Ecosystem**

- Ethereum.org [Q1 website roadmap](https://github.com/ethereum/ethereum-org-website/issues/9090)

**Application layer**

- [OpenSea](https://twitter.com/opensea/status/1611486589087109124) supports Arbitrum Nova and joins Data Availability Committee

- [Coinbase cb.id ENS names](https://twitter.com/CoinbaseWallet/status/1611093998894219265): claimable via their mobile wallet or extension

- [Invisible NFTs](https://invisible-nft.surge.sh/): ENS-bound NFTs for use as avatars in ENS profile using CC-licensed art

- [Proposal for ENS privacy](https://blog.chainsafe.io/bringing-privacy-to-ens-chainsafes-proposed-integration-using-aztec-network-4c75716e3ea1) using Aztec Network

- [Clique](https://twitter.com/clique2046/status/1611414047869775872): attest Twitter account on OP Attestation Station

* * *

### Job Listings

- [Status](https://status.im/) is hiring a [Technical Writer for Waku Product](https://grnh.se/41bd7e051us), [all other jobs here](https://grnh.se/9fc6e6fc1us)

- Join a16z-backed Story Protocol as a founding [smart contract developer](https://jobs.lever.co/storyprotocol/e08066d4-8d73-46ab-975c-dd5a284e1a83).

- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)

- Help Alchemy bring web3 to 1 billion people as a [Customer Product Engineer](https://grnh.se/040ffae65us).

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Biden administration reverses](https://www.federalreserve.gov/newsevents/pressreleases/bcreg20230103a.htm) Trump administration's pro-stablecoin banking advisory

- [NY Attorney General sues former Celsius CEO](https://ag.ny.gov/press-release/2023/attorney-general-james-sues-former-ceo-celsius-cryptocurrency-platform-defrauding) for defrauding investors

- Bankruptcy judge ruled [Celsius owns customer deposits in Earn](https://cases.stretto.com/public/x191/11749/PLEADINGS/1174901042380000000067.pdf) \[PDF\] as per their Terms of Use

- [Cameron Winklevoss publicly asks](https://twitter.com/cameron/status/1609913051427524608) Barry Silbert to determine by January 8 how DCG/Genesis will pay back $900 million to Gemini Earn customers 

- [US SEC objected](https://www.coindesk.com/policy/2023/01/04/sec-files-limited-objection-to-binanceuss-1b-deal-for-voyager-assets/) to Binance's proposed $1 billion purchase of Voyager assets

- [Coinbase settled with New York Department of Financial Services](https://www.coinbase.com/blog/Coinbase-and-NYDFS-reach-agreement-to-resolve-compliance-investigation) for $50 million penalty & $50 million for compliance

- [Mutant Ape Planet NFT creator](https://www.justice.gov/usao-edny/pr/non-fungible-token-nft-developer-charged-multi-million-dollar-international-fraud) charged with defrauding purchasers in rug pull

- [Wyre winding down](https://www.axios.com/2023/01/03/wyre-shutdown-crypto-winter) after failed acquisition by Bolt

**General**

- [200 million Twitter user profiles released](https://twitter.com/0x796/status/1611371424945512460), vulnerable Twitter API likely queried using email addresses from other data breaches

- [CircleCI](https://circleci.com/blog/january-4-2023-security-alert/) warns users to rotate secrets after security incident

- [Storj warrant canary wasn’t updated](https://news.ycombinator.com/item?id=34192336), architect advises sharing illegal content could lead to a warrant

- Remco: [polynomial commitments benchmark](https://xn--2-umb.com/23/pc-bench/index.html) to compare proof systems

- [Functional commitments](https://geometry.xyz/notebook/functional-commitments-zk-under-a-different-lens): prove execution of a private program over public inputs

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-january-7-2023](https://weekinethereumnews.com/week-in-ethereum-news-january-7-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jan 8 – [Solidity developer survey](https://blog.soliditylang.org/2022/12/07/solidity-developer-survey-2022-announcement/) deadline

- Jan 11 – Flashbots [MEV Roast: Privacy](https://collective.flashbots.net/t/mev-roast-privacy-january-11th-2023/935)

- Jan 17-31 – [Gitcoin grants round](https://go.gitcoin.co/blog/announcing-the-gitcoin-alpha-tests)

- Jan 31 – [KZG ceremony grants](https://blog.ethereum.org/2022/12/15/kzg-ceremony-grants-round) deadline

- Feb 24 - Mar 1 – [ETHDenver BUIDLWeek](https://www.ethdenver.com/)

- Mar 2-5 – [ETHDenver Hackathon](https://www.ethdenver.com/)

- Mar 10-29 – [Scaling Ethereum](https://ethglobal.com/events/scaling2023) (ETHGlobal) virtual

- Mar 15-16 – [ETHDubai](https://www.ethdubaiconf.org/)

- Mar 16-18 – [ETH Porto](https://ethporto.org/)

- Mar 28-30 – [Ethereum Rio](https://www.ethereumbrasil.com/ethereumrio)

- Apr 3-6 – [Edcon](https://edcon.io/) Vienna

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- Apr 14-16 – [ETHGlobal Tokyo](https://tokyo.ethglobal.com/)

- **Apr 14-16 –** [**ETHZurich**](https://ethereumzuri.ch/) **conference**

- May 26–28 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Jun 23–25 – [ETHGlobal Toronto](https://ethglobal.com/events/toronto)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–25 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

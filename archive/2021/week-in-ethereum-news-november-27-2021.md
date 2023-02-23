---
title: "Week in Ethereum News <br> November 27, 2021"
date: "2021-11-27"
---

## **Eth News and Links**

**Mainnet execution layer**

- Vitalik’s [roadmap for scaling rollups](https://notes.ethereum.org/@vbuterin/data_sharding_roadmap), calldata expansion (EIP4488/90), then ~4 shards (similar scale of Altair upgrade), then N shards (committee secured) and then data availability sampling to complete sharding rollout
- Latest [core devs call video](https://www.youtube.com/watch?v=js4HLK4MyQI&t=385s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1464262630139334658):
    - Update your node for Arrow Glacier upgrade
    - [Kintsugi](https://notes.ethereum.org/@djrtwo/kintsugi-milestones) devnet 2 next week, aiming for December “final devnet”
    - Discussion on lowering cost of rollups (EIP4488 vs EIP4490), attempt to prototype and decide if upgrade can be shipped before PoW switch off
- Geth released details of [DoS vulnerability via malicious snap/1 request](https://github.com/ethereum/go-ethereum/security/advisories/GHSA-59hh-656j-3p7v), fixed in v1.10.9; run [geth version-check](https://twitter.com/go_ethereum/status/1463066580779249673) to check for published vulnerabilities
- Geth [v1.10.13](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.13): fixes log retrieval for old archive nodes, legacy transaction filtering in tx pool & snap sync crash with malicious packets
- Nethermind [v1.12.0](https://github.com/NethermindEth/nethermind/releases/tag/1.12.0): upgraded to .NET v6.0, supports Apple silicon
- [Overview of witnesses](https://hackmd.io/@jldunne/Hkl39vHOF) and role they play in stateless Ethereum
- History expiry [AMA](https://www.reddit.com/r/ethereum/comments/qzvsfq/impromptu_technical_ama_on_history_expiry), options are one-time expiry of PoW history a few months after PoW switch off and/or regular rolling expiry (EIP 4444)

**EIPs/Standards**

- [EIP4469](https://github.com/ethereum/EIPs/blob/716e54e78690be3688549862f41f918c6c615e98/EIPS/eip-4469.md): Wrapped metaverse token
- [EIP4488](https://github.com/ethereum/EIPs/blob/a12d2155f51319461b6a18ff9fc924c5d7e29c71/EIPS/eip-4488.md): Transaction calldata gas cost reduction with total calldata limit
- [EIP4490](https://github.com/ethereum/EIPs/blob/85b1193e111c9dbc7d6b8f6214d0e134320bc551/EIPS/eip-4490.md): Second transaction data gas cost reduction
- [EIP4494](https://github.com/ethereum/EIPs/blob/6669f57178dc3d56036a37f08e135306a360524d/EIPS/eip-4494.md): Permit for ERC721 NFTs

**Proof of Stake consensus layer**

- Danny Ryan’s [Finalized PoS update](https://blog.ethereum.org/2021/11/22/finalized-no-32/): Kintsugi sprint first devnet launched then broken, stakers must update for Arrow Glacier upgrade
- consensus-specs [v1.1.6](https://github.com/ethereum/consensus-specs/releases/tag/v1.1.6): critical upgrades to fork choice and minor iteration on Kintsugi specs
- [Lodestar (Typescript)](https://twitter.com/dapplion/status/1464033020680224777) proposed its first mainnet block, fifth consensus client
- [Tutorial to run Nimbus with Nethermind](https://our.status.im/kintsugi-merge/) on Kintsugi devnet
- [Weak subjectivity sync](https://notes.ethereum.org/@djrtwo/ws-sync-in-practice) approaches to get state rather than out of band
- State of research: [censorship resistance](https://notes.ethereum.org/@vbuterin/pbs_censorship_resistance) under block proposer/builder separation; Vitalik argues for a hybrid model 
- [mev-boost](https://github.com/flashbots/mev-boost): first version of Flashbots middleware open-sourced
- Proposal for a non-middleware [Flashbots with consensus clients](https://hackmd.io/QoLwVQf3QK6EiVt15YOYqQ?view)

**Layer2**

- Polynya’s explainer of rollup-centric scaling [roadmap](https://polynya.medium.com/rollup-centric-ethereum-roadmap-november-2021-update-f8a8f6f518ce)
- [Aztec (zk rollup) private network](https://medium.com/aztec-protocol/infinite-privacy-new-anonymity-paradigms-with-aztec-network-1b02e84bbce2) is more private than privacy mixers
- [Estimate of tokens trapped on mainnet](https://medium.com/@codyborn/value-fragmentation-8c8336f97cfd) due to high gas prices

* * *

### **This newsletter is made possible thanks to [Kwenta](https://kwenta.io/) by [Synthetix](https://synthetix.io/)!**

![Kwenta](https://weekinethereumnews.com/wp-content/uploads/2021/04/IMG_20210418_190328_618-1024x512.jpg)

[Kwenta](https://kwenta.io/) enables traders to access real-world and derivative assets on-chain using the power of the Synthetix protocol. 

Long or short popular synthetic cryptocurrencies, commodities, forex, and equities without the limits or compromises of a centralized exchange. 

You can now also use [L2 Kwenta on Optimism](https://blog.kwenta.io/everything-you-need-to-know-about-using-kwenta-on-l2/) for low gas fees and blazing fast transactions!

Decentralized Perpetual Futures coming soon.

* * *

**Stuff for developers**

- OpenZeppelin Contracts [v4.4](https://forum.openzeppelin.com/t/openzeppelin-contracts-4-4/19706): GovernorSettings to manage settings via proposals, PaymentSplitter supports ERC20, VestingWallet for ETH/ERC20
- Remix IDE [v0.20.1](https://medium.com/remix-ide/release-v0-20-0-0-20-1-notes-e7182560a1bf): editor changed to Monaco (used in VSCode)
- [Remix analytics](https://medium.com/remix-ide/remixs-analytics-report-366596a99e36): 24k visits a day & 800k deployments in October
- Hardhat [v2.7.0](https://github.com/nomiclabs/hardhat/releases/tag/hardhat%402.7.0): adds FIFO mode to Hardhat Network's mempool and customizable coinbase address
- Ganache [v7.0.0 beta.1](https://github.com/trufflesuite/ganache/releases/tag/ganache%407.0.0-beta.1): local blockchain (formerly ganache-cli), beta.0 added zero-config mainnet forking using Infura
- Otterscan [v2021.11.03](https://twitter.com/wmitsuda/status/1462912722178347015): visual transaction trace tool, requires Erigon update
- [ERC721Loanable](https://github.com/mattdf/ERC721Loanable): extension to loan NFT for up-front premium, proof of concept
- Sourcify (source code verification) supports [Optimism](https://twitter.com/sourcifyeth/status/1463875221375623171) & [Boba Network](https://twitter.com/sourcifyeth/status/1464172996625633280)
- [Verify with Sourcify](https://twitter.com/sourcifyeth/status/1462835169748996105) using Hardhat, drag & drop Hardhat output to Sourcify, select contract and verify
- [Verifying Etheria (early NFT project) contract](https://medium.com/dedaub/a-six-year-old-solc-riddle-6f213fc33485) from 2015 on Etherscan, Solidity v0.1.6
- [Storage slot discovery](https://twitter.com/bantg/status/1462810217448620035): modify state such as token balances by poking balanceOf view function
- Beginner: [Solidity mapping vs array](https://www.devtwins.com/blog/understanding-mapping-vs-array-in-solidity)
- [eth-tools](https://github.com/odyslam/eth-tools): APIs to sign, verify, send & call, using CloudFlare workers and MetaMask provider
- StarkNet [practical lessons learnt](https://hackmd.io/@RoboTeddy/BJZFu56wF) from implementing a project
- [Using BigQuery datasets](https://mirror.xyz/nick.eth/INhEmxgxoyoa8kPZ3rjYNZXoyfGsReLgx42MdDvn4SM) to analyse Ethereum data
- [MultiFaucet](https://faucet.paradigm.xyz/): (testnet faucet) adds Rinkeby & Arbitrum testnets

**Security**

- Unlock [contract upgraded using compromised private key](https://unlockprotocol.notion.site/unlockprotocol/Sunday-November-21st-2021-Incident-Update-a8e05ba111284d5ba43872fa5f00bccb) on xDAI and Polygon, 50k Unlock tokens stolen
- Wolf Game [reentrancy vulnerability](https://twitter.com/not__stoops/status/1462638499316699137) with ERC721 safeTransferFrom, staking and claiming rewards were paused
- Aave v2 and xSUSHI vulnerability (similar to Cream) [post mortem](https://governance.aave.com/t/analysis-of-xsushis-incident/6335)
- [Secureum (auditing bootcamp) course material](https://github.com/x676f64/secureum-mind_map): blog posts, videos, assignments and quizzes

**Ecosystem**

- [EIP1559 burnt 1 million ETH](https://twitter.com/ultrasoundmoney/status/1463494305381822464) in 109 days
- [Ethburned.wtf](https://www.ethburned.wtf/) shows how much an account has burnt, supports ENS
- Suggestion to revive [Finney as a currency unit](https://www.reddit.com/r/ethereum/comments/r1h5xu/should_we_revive_the_finney/) due to unit bias
- [MetaMask supports GridPlus Lattice1](https://consensys.net/blog/news/metamask-x-lattice1-the-hardware-wallet-designed-for-ethereum-users-is-now-supported) hardware wallet

**Application layer**

- [UMA event based expiry KPI options](https://medium.com/uma-project/introducing-milestone-kpi-options-2a8ea4cf480e): expire when KPI metric met or when the time runs out
- [Pika Protocol](https://twitter.com/PikaProtocol/status/1462765366078173184) (perpetual swap exchange): guarded launch on Optimism
- [Ondo Finance](https://blog.ondo.finance/ondo-and-feis-liquidity-service-launches-with-100m-in-committed-capital-f08ef15fe0fd) liquidity as a service, alternative to liquidity mining campaigns
- [Synthetix](https://blog.synthetix.io/debt-pool-synthesis/) roadmap to merge debt pools on mainnet and layer 2
- [The Infinite Machine](https://thedefiant.io/the-infinite-machine-movie-nfts-funding/) book to be made into a movie funded via NFTs

* * *

### **Job Listings**

- Kwenta seeks a talented [Solidity Engineer](https://blog.kwenta.io/kwenta-open-position-solidity-engineer/) to join as a Core Contributor 
- ethereum.org team is hiring a [Product Designer](https://ethereum.org/en/about/product-designer/)
- Nethermind 1-3 month [internship program](https://www.notion.so/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)
- Ethereum Foundation hiring a [Research Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=48&source=weekinethnews) for PoS consensus layer

**Reach people experienced with Ethereum.**  $420 for two issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US federal agencies plan to provide [crypto policy clarity for banks](https://www.federalreserve.gov/newsevents/pressreleases/files/bcreg20211123a1.pdf) \[PDF\] in 2022
- [US Comptroller](https://www.occ.gov/news-issuances/news-releases/2021/nr-occ-2021-121.html): banks must have adequate controls in place before engaging in crypto activities
- US Senate banking committee [requests information from stablecoin issuers](https://twitter.com/ronwhammond/status/1463274970063200267)
- [Implied volatility](https://lambert-guillaume.medium.com/on-chain-volatility-and-uniswap-v3-d031b98143d1) of an asset using Uniswap v3 pools
- Kain Warwick’s [origin story of yield farming](https://twitter.com/kaiynne/status/1462549593455878146)
- [Citi to hire 100 people](https://www.coindesk.com/business/2021/11/22/citi-plans-to-hire-100-staffers-for-beefed-up-crypto-division/) for blockchain and digital assets division

**General**

- Ethereum Foundation and UNICEF partnership [update](https://blog.ethereum.org/2021/11/24/ef-unicef-update/)
- [Locally Testable Codes](https://www.quantamagazine.org/researchers-defeat-randomness-to-create-ideal-code-20211124/) with constant rate, distance, and locality
- SNARK-based [VDF implementation](https://zkproof.org/2021/11/24/practical-snark-based-vdf/)
- ECFFT algorithm [explainer](https://ethresear.ch/t/the-ec-fft-algorithm-without-elliptic-curve-and-isogenies/11346)
- [NFT](https://blog.collinsdictionary.com/language-lovers/get-your-crypto-at-the-ready-nfts-are-big-in-2021/) is Collins Dictionary word of the year

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-november-27-2021](https://weekinethereumnews.com/week-in-ethereum-news-november-27-2021)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Dec 1-16 – [Gitcoin Grants Round 12](https://gitcoin.co/grants/)
- Dec 3 – PoW switch off [second community call](https://github.com/ethereum/pm/issues/419)
- Dec ~8 – [Arrow Glacier](https://blog.ethereum.org/2021/11/10/arrow-glacier-announcement/) upgrade block 13,773,000
- Jan 24-26 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford University)
- **Feb 17 – [Schelling Point](https://schellingpoint.gitcoin.co/) (Denver)** 
- Feb 18-20 – [ETHDenver](https://www.ethdenver.com/)
- Mar 28-30 – [ETHDubai](https://www.ethdubai.xyz/)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

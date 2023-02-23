---
title: "Week in Ethereum News <br> May 28, 2022"
date: "2022-05-28"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- [Mainnet-shadow-fork-6](https://twitter.com/abcoathup/status/1529303473493520384) transition to PoS on May 31
- Ropsten testnet [reached Terminal Total Difficulty](https://notes.ethereum.org/@timbeiko/ropsten-ttd-override) (TTD) before Ropsten beacon chain genesis:
    - miner added hash rate & lowered gas limit in malicious stress test
    - TTD being overridden to very large value to prevent merge
    - override TTD after Ropsten beacon chain genesis & Bellatrix upgrade to merge around June 8
- [Test the merge](https://twitter.com/m25marek/status/1528644957422206976) with Nethermind

**Mainnet execution layer**

- Latest core devs [call video](https://www.youtube.com/watch?v=5mMd-XHAv2Q&t=207s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1530265096156434432):
    - two consensus layer Merge releases: Bellatrix followed by setting TTD
    - no decision on delaying difficulty bomb, discussed 2-4 month delay coupled with Paris execution layer Merge upgrade
    - short discussion on EIP4844 (proto-danksharding) & EIP2537 (BLS precompile)
- Ropsten testnet Paris releases:
    - Geth [v1.10.18](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.18): manually override TTD
    - Erigon [v2022.05.08-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.05.08)
    - Nethermind [v1.13.1](https://github.com/NethermindEth/nethermind/releases/tag/1.13.1)
    - Besu [v22.4.2](https://github.com/hyperledger/besu/releases/tag/22.4.2)
- [OpenEthereum](https://twitter.com/OpenEthereumOrg/status/1529147048758595585) client (formerly Parity) deprecated
- [Speed up EIP4844 transaction validation](https://github.com/ethereum/EIPs/pull/5088) (using KZG proofs), reduces verification time to 3.5ms
- Understanding the crypto in Verkle trees: the difference between [bandersnatch and banderwagon](https://hackmd.io/@6iQDuIePQjyYBqDChYw_jg/BJ2-L6Nzc)

**Proof of Stake consensus layer**

- Beacon chain [7-block deep reorg](https://twitter.com/terencechain/status/1529566839033933824): caused by mix of proposer boost upgraded & non-upgraded nodes and timing of late arriving block.  **Upgrade your nodes**!
- Ropsten beacon chain Bellatrix releases:
    - Teku [v22.5.1](https://github.com/ConsenSys/teku/releases/tag/22.5.1)
    - Nimbus [v22.5.1](https://github.com/status-im/nimbus-eth2/releases/tag/v22.5.1)
    - Lighthouse [v2.3.0-rc.0](https://github.com/sigp/lighthouse/releases/tag/v2.3.0-rc.0)
    - Prysm [v2.1.3-rc.2](https://github.com/prysmaticlabs/prysm/releases/tag/v2.1.3-rc.2)
- [Checkpoint sync safety](https://www.symphonious.net/2022/05/21/checkpoint-sync-safety/): get from trusted source and verify
    - Even [Infura being hacked](https://www.symphonious.net/2022/05/23/checkpoint-sync-what-if-infura-is-hacked/) is not much of a risk, but you should still verify your checkpoint
- Analysis of [Swap-or-Not Single Secret Leader Election (SSLE)](https://ethresear.ch/t/analysis-of-swap-or-not-ssle-proposal/12700) proposal
- [Lido discussion](https://research.lido.fi/t/should-lido-on-ethereum-be-limited-to-some-fixed-of-stake/2225) on limiting share of stake on the beacon chain 

**EIPs/Standards**

- [EIP4353](https://github.com/ethereum/EIPs/pull/5103/files): interface for staked NFTs
- [EIP5107](https://github.com/ethereum/EIPs/pull/5107/files): Name-bound Tokens

**Layer2**

- [zk-rollup proposal using Practical Verifiable Delay Encryption](https://ethresear.ch/t/mev-resistant-zk-rollups-with-practical-vde-pvde/12677) for MEV minimization

* * *

### **This newsletter is made possible thanks to** [**SpeedRunEthereum**](https://speedrunethereum.com/)**!**

![SpeedRunEthereum](https://weekinethereumnews.com/wp-content/uploads/2022/04/Screenshot-from-2022-04-01-15-39-52.png)

[](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F7611e49a-362d-4b90-a634-b9bb87384b3d_769x208.png)

Are you a web2 dev who wants to get into web3?  

The best way to go from _zero_ to **hero** is [SpeedRunEthereum.com](https://speedrunethereum.com/).

Learn how to build on Ethereum; the superpowers and the gotchas.

Then [speed run Ethereum](https://speedrunethereum.com/) by testing your skills in a [series of challenges](https://speedrunethereum.com/challenge/simple-nft-example) and [join web3](https://twitter.com/austingriffith/status/1493688828661432325).

* * *

**Stuff for developers**

- Tim Beiko’s [Merge reminder](https://twitter.com/timbeiko/status/1528866058022494208): DIFFICULTY opcode will return PREVRANDAO and 12s block times (minus missed slots) rather than ~13s
- ethers js [v5.6.8](https://twitter.com/ethersproject/status/1529232578670120964): update BN.js for hex string bug, doesn’t appear to occur in 256-bit numbers
- ethers js [cheat sheet](https://github.com/thallo-io/ethers-js-cheatsheet#ethers-js-supplementary-examples)
- Foundry: 
    - [Forge Snippets](https://github.com/crisgarner/VSCodeForgeSnippets#readme) for VS Code
    - [signature database](https://twitter.com/samczsun/status/1529281934131466240) support
    - guide to [using Foundry with Hardhat](https://book.getfoundry.sh/config/hardhat.html)
- ERC721A [v4.0.0](https://twitter.com/cygaar_dev/status/1529196910531121152): removes OpenZeppelin Contracts dependency, upgradeable version uses EIP2535 (Diamonds)
- [MergeReward](https://gist.github.com/m1guelpf/6d09b85d70a1dfd00d394b2acf789eeb): contract pays first caller after the Merge by checking difficulty is bigger than 2^64
- Remco’s [Yul parser](https://github.com/recmo/yul#yul-language-tools): Rust based
- [Web3.py customization options](https://snakecharmers.ethereum.org/web3-py-patterns-customizations/): middleware, custom methods, external modules and custom providers
- [dApp Starter](https://github.com/m1guelpf/dapp-starter#readme) using Typescript, Next.js, Tailwind CSS, RainbowKit, ethers and wagmi
- [RainbowKit mint NFT demo](https://github.com/peduarte/rainbowkit-mint-nft-demo#readme): Next.js NFT minting front end 
- [Hop airdrop sybil hunt](https://twitter.com/richardchen39/status/1528919705498574849): Union-Find graph algorithm to find connected subgraph components in O(1) time
- [StackExchange](https://ethereum.meta.stackexchange.com/questions/697/custom-ethereum-design-and-logo-information-gathering) to create custom site design for Ethereum
- Patrick McCorry’s crypto class [resources](https://cryptocurrencyclass.github.io/) (8 sessions)
- Patrick Collins: [web3 development](https://github.com/smartcontractkit/full-blockchain-solidity-course-js) using JavaScript (32 hours of video)

**Security**

- MEV bot [exploited for 8 ETH](https://twitter.com/BlockSecTeam/status/1529293056179986432)

**Ecosystem**

- Ethereum roadmap [deep dive](https://members.delphidigital.io/reports/the-hitchhikers-guide-to-ethereum): dank sharding, history & state management, MEV and the Merge
- ETHGlobal [HackMoney finalists](https://twitter.com/ethglobal/status/1529576980873617410)
- Sync [mainnet in under 24 hours on a $189 ARM board](https://twitter.com/EthereumOnARM/status/1529383797107699712)

**Enterprise**

- GameStop [Wallet](https://wallet.gamestop.com/): Chrome browser extension, mainnet and LoopRing Layer 2

**Application layer**

- Mirror [Writing NFTs](https://dev.mirror.xyz/5gt60vKFJZ_tR1BjoJ7-Y0sNw7REebStHjzFU5x73J0): sell and collect posts as NFTs on Optimism
- [Zora](https://twitter.com/ourZORA/status/1529861100954689536): create music (with album art), video and SVG NFTs
- [Uniswap](https://twitter.com/uniswap/status/1529102980296867842) $1 trillion cumulative trading volume
- [Fairmint](https://blog.fairmint.co/we-raised-7-3-million-in-our-sleep-now-your-startup-can-too-965a7e7e0534) (tokenized equity) open to all
- Vitalik: [evaluate automated stablecoins](https://vitalik.eth.limo/general/2022/05/25/stable.html); can they wind down to zero users and can they charge a negative interest rate

* * *

### **Job Listings**

- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Trail of Bits [Security Apprenticeship](https://jobs.lever.co/trailofbits/b2d6ce87-6b01-462f-965a-597a273ce26f) (3 months)
- Ethereum Foundation need a [People Operations Lead](https://jobs.lever.co/ethereumfoundation/8046bbe5-6343-4ecf-8296-37dc2a5bf915?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Sourcify (source code verification) need a [TypeScript Developer](https://jobs.lever.co/ethereumfoundation/db85cf1d-6ffd-42a6-8f0d-f5a91c6ddf4a?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- [Hiring Coordinator](https://jobs.lever.co/ethereumfoundation/7f5bf10b-ea68-4364-a378-e34ae345a212?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) wanted by Ethereum Foundation

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US Federal Reserve](https://www.federalreserve.gov/publications/files/2021-report-economic-well-being-us-households-202205.pdf) \[PDF\]: 12% of adults held/used crypto, 11% held as an investment, 2% used for payments and 1% sent to family/friends
- UK financial regulator [first crypto sprint](https://twitter.com/will_harborne/status/1528669113341681664)
- Stable coin [dashboard](https://stablecoins.wtf/)
- Seth Green’s [Bored Ape stolen](https://www.buzzfeednews.com/article/sarahemerson/seth-green-bored-ape-stolen-tv-show) in phishing scam, ape used in upcoming animated show, claims to maintain IP ownership

**General**

- [US FTC](https://www.ftc.gov/business-guidance/blog/2022/05/twitter-pay-150-million-penalty-allegedly-breaking-its-privacy-promises-again): Twitter fined $150 million for using phone & email provided for security in targeted ads
- [US Department of Justice](https://www.justice.gov/opa/pr/department-justice-announces-new-policy-charging-cases-under-computer-fraud-and-abuse-act): good-faith security research shouldn’t be charged under Computer Fraud and Abuse Act
- [Caulk](https://eprint.iacr.org/2022/621): lookup arguments in sublinear time, 100x faster than Poseidon

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-may-28-2022](https://weekinethereumnews.com/week-in-ethereum-news-may-28-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in_ **_bold_**_)_**:**

- **Jun 1 – applications close for OxPARC** [**Halo2 Learning group**](https://0xparc.org/blog/halo2-learning-group)
- Jun 3 – [Merge community call #4](https://github.com/ethereum/pm/issues/532)
- Jun 8-23 – [Gitcoin Grants Round 14](https://gitcoin.co/grants/)
- Jun 10 – [Austin DeFi](https://2022.austindefi.org/) summit
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETH NYC](https://nyc.ethglobal.co/)
- Jul 1 – [Data Availability Sampling](https://github.com/ethereum/requests-for-proposals/blob/master/open-rfps/das.md) proposals due
- **Jul 6-8 –** [**ETHBarcelona**](https://ethbarcelona.com/)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 5-13 – [ETH Seoul](https://2022.ethseoul.org/)
- Aug 8-10 – [ETHToronto](https://www.ethtoronto.ca/)
- Aug 11-14 – [ETH LATAM (Buenos Aires)](https://twitter.com/ethlatam/status/1524146640474587137)
- **Aug 19-21 –** [**ETHMexicoCity**](https://mexico.ethglobal.com/)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 28 – [DeFi San Francisco](https://2022.defi-sf.com/) summit
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev) (hackathon & conference)
- Sep 2-4 – [ETHSantiago](https://twitter.com/EthereumStgo)
- **Sep 2-28 –** [**ETHOnline**](https://online.ethglobal.com/')
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- **Sep 27-29 –** [**Ethereum SP**](https://twitter.com/Ethereum_Brasil/status/1530320916667895808) **(São Paulo)**
- **Oct 7-9 –** [**ETHBogotá**](https://bogota.ethglobal.com/)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- **Nov 4-6 –** [**ETHSanFrancisco**](https://sf.ethglobal.com/)
- **Nov 18-20 – ETHGlobal** [**Web3 Weekend**](https://web3weekend.ethglobal.com/)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- **Dec 2-4 –** [**ETHIndia**](https://ethindia.co/)

**Did you get forwarded this newsletter?** [_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive it weekly_**

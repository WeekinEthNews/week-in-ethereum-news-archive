---
title: "Week in Ethereum News <br> November 6, 2021"
date: "2021-11-06"
---

## **Eth News and Links**

**Mainnet execution layer**

- PoW switch off [community call](https://www.youtube.com/watch?v=_kfS9jAUY6g&t=18s):
    - average block times change from ~13s to 12s, contracts may have [hardcoded ~13s assumption](https://twitter.com/TimBeiko/status/1456644168986419200)
    - Dankrad’s slides on [finding the safe head of the chain](https://docs.google.com/presentation/d/1MUVaFyd9ce3hPQ5L-UhqVSfxf1ajMYFbkActkp5xNKI/edit#slide=id.p1)
- Erigon [v2021.11.01](https://github.com/ledgerwatch/erigon/releases/tag/v2021.11.01): first beta release, not downgradeable

**EIPs/Standards**

- [EIP4399](https://eips.ethereum.org/EIPS/eip-4399): Supplant DIFFICULTY opcode with RANDOM

**Proof of Stake consensus layer**

- Danny Ryan’s [Finalized PoS update](https://blog.ethereum.org/2021/11/02/finalized-no-31/): proposed forkchoice fixes can mitigate 3 liveness & reorg attacks and won’t delay switching off PoW 
- Tweet thread of [reorgs in PoS and mitigation strategies](https://twitter.com/casparschwa/status/1454511836267692039)
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_211105)
- [PoS implementers call](https://youtu.be/9U_xj_zCMYg?t=63). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/B1wBrwbPF): 
    - Kintsugi [milestone tracker](https://notes.ethereum.org/@djrtwo/kintsugi-milestones) to a persistent testnet early December
    - Pyrmont testnet to be shut down
- [Staking rewards](https://hackmd.io/@sproul/altair-rewards) after Altair upgrade are more variable: 
    - Attestations: 0.0040-0.0042 ETH per day
    - Blocks: 0.018-0.03 ETH per block
    - Sync committee membership: 0.08 ETH per sync committee selection
- [MEV-Boost](https://ethresear.ch/t/mev-boost-merge-ready-flashbots-architecture/11177) for validators, work in progress Flashbots architecture sitting between consensus and execution clients

**Layer2**

- [Future of zk rollups](https://hackmd.io/@canti/rkUT0BD8K) to scale Ethereum, sidechains should take the pragmatic approach and become zk-rollups
- [Connext adds mainnet support](https://twitter.com/connextnetwork/status/1456381261036113923), transfer stablecoins between mainnet, Arbitrum and selected sidechains

* * *

### **This newsletter is made possible thanks to [NEAR](https://near.org/) & [Aurora](https://aurora.dev/)!**

![Aurora Chainlink Hackathon](https://weekinethereumnews.com/wp-content/uploads/2021/11/Aurora-Chainlink-Hackathon-2021-1024x576.png)

Chainlink Fall 2021 Hackathon is taking place on October 22 - November 28. Join smart contract developers to reinvent applications in various industries in this biggest Chainlink hackathon so far.

Aurora is providing $25,000 to the Chainlink Fall 2021 Hackathon.

Participate in one of Aurora’s challenges, contribute to the growth of the NFT movement, and win up to $10,000!

Create a contract that allows moving NFTs back and forth between NEAR and Aurora.

Create a connector that allows moving native NEAR NFTs back and forth from NEAR to Ethereum using Aurora’s Rainbow Bridge.

Develop with Aurora and Chainlink to spur a major surge of innovation across the NFT economy, and the larger smart contract ecosystem.

Details: [chainlink-fall-hackathon-2021.devpost.com](https://chainlink-fall-hackathon-2021.devpost.com)

* * *

**Stuff for developers**

- [Solidity docs code examples](https://twitter.com/solidity_lang/status/1456233507538227207) can be opened in Remix 
- [solidity-trigonometry](https://github.com/mds1/solidity-trigonometry): basic trig functions, sin & cos are 2-2.5k gas
- [nft-swap-sdk](https://github.com/trader-xyz/nft-swap-sdk): TypeScript SDK using 0x v3 protocol to swap NFTs
- [NFT Floor Market](https://twitter.com/cybourgeoisie/status/1455552910394368010): on chain NFT marketplace contract, no fees other than royalties, unaudited
- Otterscan [v2021.10.05](https://twitter.com/wmitsuda/status/1455247090821521412): improved ABI outline UI for verified contracts and resolving token names from addresses
- [ArchiveNode](https://twitter.com/ArchiveNode/status/1455150809876992002): free access to small time developers to archive data
- [StarkNet playground](https://starknet.io/playground/): compile and deploy Cairo contracts
- [Warp (Solidity to Cairo transpiler) example](https://medium.com/nethermind-eth/composability-the-final-piece-of-the-puzzle-8c7ca5dfd470) of transpiling two composable contracts & deploying them
- [starknet-react-example](https://github.com/fracek/starknet-react-example): connect React app to StarkNet Cairo contract
- [zksnarks-library](https://github.com/kevinz917/zksnarks-library): commonly used logic and examples implemented into SNARKs using the Circom language
- [plonkit](https://github.com/fluidex/plonkit): zkSNARK toolkit to work with Circom

**Security**

- Fuse community [pool drained](https://twitter.com/Mudit__Gupta/status/1455627465678749696) after VUSD price manipulated on Uniswap v3, TWAPs can be subject to manipulation
- [Solidity not affected by Trojan Source](https://twitter.com/alexberegszaszi/status/1455162941146288128), Solidity Underhanded Contest 2020 winner exploited Unicode direction markers & was fixed in v0.7.6
- Tincho’s [Damn Vulnerable DeFi v2](https://www.damnvulnerabledefi.xyz/v2-release.html): Solidity v0.8, four new levels, new (broken) integrations and Hardhat + Ethers tests

**Ecosystem**

- Ethereum Foundation [Q2 grantees](https://blog.ethereum.org/2021/11/04/esp-allocation-update-q2-2021/), $8m in grants 
- Devcon Archive [v2](https://blog.ethereum.org/2021/11/03/devcon-archive-v2/): improved UX & content discovery, more content on IPFS and community curated playlists
- Optimism’s $1m retroactive public goods funding [recipients](https://twitter.com/optimismPBC/status/1455780701479964675)
- [Padawan DAO](https://twitter.com/pet3rpan_/status/1455279420269375495): funding scholarships for highschool and university students to attend their first crypto conferences

**Enterprise**

- US Postal Service [Day of the Dead NFT stamp art](https://medium.com/veve-collectibles/usps-series-1-day-of-the-dead-b5891e0d0baa) on VeVe (Immutable)
- Marvel [Eternals](https://www.marvel.com/articles/gear/eternals-gather-for-marvel-mightys-digital-collectibles) movie NFTs on VeVe (Immutable)
- [Burger King US loyalty program](https://www.bk.com/crypto) offers chance to win 1 ETH or 1 memecoin via RobinHood
- Paradigm Founder [Matt Huang joins Stripe’s board to help guide web3](https://stripe.com/newsroom/news/matt-huang-joins-stripe-board) strategy

**Application layer**

- [ENS DAO](https://ens.mirror.xyz/-eaqMv7XPikvXhvjbjzzPNLS4wzcQ8vdOgi9eNXeUuY): users can claim & delegate governance tokens per account, [token farm accounts](https://twitter.com/nicksdjohnson/status/1456048492141441027) are being manually excluded
- Maker [DAI Direct Deposit Module](https://twitter.com/hexonaut/status/1455507332469821440): privileged access for Aave to mint DAI
- [Notional v2](https://blog.notional.finance/notional-v2-is-live/) live on mainnet, longer-dated maturities and flexible dates
- [Angle Finance](https://blog.angle.money/angle-is-live-on-the-ethereum-mainnet-a8253162daf0) live on mainnet, Euro stablecoin
- Aave [v3 overview](https://governance.aave.com/t/introducing-aave-v3/6035)
- NFTX [Swaps](https://twitter.com/nftx_/status/1455484494123831303): swap NFTs in same collection
- [Spaces](https://www.ourspaces.xyz/): message any address or ENS, token gated chats

* * *

### **Job Listings**

- Toucan: [Solidity dev](https://toucan-protocol.notion.site/Join-the-Flock-c5782edb754b48e598a8cdd74a4dc93c) to build web3 infrastructure to reverse climate change
- OpenZeppelin hiring a [Technical Marketing Manager](https://openzeppelin.com/jobs/opening/?gh_jid=4602368003)
- Solidity is hiring a [C++ dev](https://ethereum.bamboohr.com/jobs/view.php?id=40&source=weekinethnews)

**Reach people experienced with Ethereum.**  $420 for two issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US Presidents Working Group on Financial Markets stablecoin [statement](https://home.treasury.gov/system/files/136/PWG-Stablecoin-Statement-12-23-2020-CLEAN.pdf) calling for congressional action
- [Commonwealth Bank](https://www.commbank.com.au/articles/newsroom/2021/11/CBA-to-offer-crypto-services.html) (major Australian bank) to add crypto services to its banking app using Gemini
- [Turing-complete governance](https://baby.mirror.xyz/O7a922A-9zT4C4UwssRExkftdHywJ-13sR2rxQ-t__k), composable & arbitrarily programmable
- Bankless: [Ethereum is the triple point blockchain](https://newsletter.banklesshq.com/p/the-triple-point-blockchain-market) 
- [Early employees to sue ConsenSys](https://www.coindesk.com/business/2021/11/02/consensys-shareholders-readying-legal-action-over-share-valuation/) over asset valuations

**General**

- Harry Denley: Twitter and Facebook [server side unfurling engines can be abused for phishing](https://harrydenley.com/faking-twitter-unfurling/)
- Vitalik on [crypto cities](https://vitalik.ca/general/2021/10/31/cities.html), make existing processes more trusted & transparent and experiment with city tokens & participatory governance
- [Random oracles in cryptography](https://kobi.one/2021/10/31/random-oracles.html), using hashes that are not good imitations of random oracles can lead to broken protocols
- Vitalik: [Incremental verification](https://vitalik.ca/general/2021/11/05/halo.html) and SNARKs with no pairings and no trusted setups
- Bounties worth $172k for [breaking zk friendly hash functions](https://www.zkhashbounties.info/), Rescue Prime, Feistel-MiMC, Poseidon and Reinforced Concrete

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-november-6-2021](https://weekinethereumnews.com/week-in-ethereum-news-november-6-2021)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Oct 25 - Dec 13 – [Gitcoin DAO Global hackathon](https://gitcoin.co/hackathon/dao-global/onboard) (virtual)
- Nov 11 – [Optimism upgrade](https://twitter.com/optimismPBC/status/1451339513964359682)
- Nov 16 – [Formal Verification in the Ethereum Ecosystem](https://runtimeverification.com/events/formalverificationeth/)
- **Dec 1-16 – [Gitcoin Grants Round 12](https://twitter.com/gitcoin/status/1454244939169214472)**
- Dec ~8 – [Arrow Glacier](https://github.com/ethereum/execution-specs/blob/master/network-upgrades/mainnet-upgrades/arrow-glacier.md) upgrade block 13,773,000
- Jan 24-26 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford University)
- Feb 11-20 – [ETHDenver](https://www.ethdenver.com/)
- Mar 28-30 – [ETHDubai](https://www.ethdubai.xyz/)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

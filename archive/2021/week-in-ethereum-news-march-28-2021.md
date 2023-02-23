---
title: "Week in Ethereum News <BR> March 28, 2021"
date: "2021-03-28"
---

## **Eth News and Links**

**Mainnet**

- Beiko’s summary of [what’s happening in upgrade planning](https://hackmd.io/@timbeiko/acd/https%3A%2F%2Fhackmd.io%2F%40timbeiko%2FH1US36qzO): Berlin live on testnets, 1559 scheduled for Jul/Aug, whether to freeze features until we turn off PoW
- EthereumJS with [v5.2.1](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs%2Fblockchain%405.2.1) is ready for Berlin, as is [py-evm](https://github.com/ethereum/py-evm/releases/tag/v0.4.0-alpha.1)
- Proposed [verkle tree scheme for Eth state](https://www.reddit.com/r/ethereum/comments/mdbkp2/proposed_verkle_tree_scheme_for_ethereum_state/)
- An early spec for [state retrieval network](https://ethresear.ch/t/state-network-dht-development-update-2/9005)

**EIPs/Standards**

- [EIP3416](https://eips.ethereum.org/EIPS/eip-3416): Median gas premium
- [EIP3436](https://github.com/ethereum/EIPs/blob/677661067fc5714f63f386e3d8aca2606b0ca54b/EIPS/eip-3436.md): Clique block choice rule for less deadlocks

**Proof of Stake**

- Latest [proof of stake call](https://youtu.be/Q0EbnFViJFk?t=107). Notes from [Alex Stokes](https://twitter.com/ralexstokes/status/1375095774749491206) and [Ben Edgington](https://hackmd.io/@benjaminion/ry2SbM5VO)
- Danny Ryan's [Finalized](https://blog.ethereum.org/2021/03/24/finalized-no-24/) update - Altair upgrade spec pre-release, the security RFP
- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210328), lots of context from Ben on the things in this section
- PR for a [spec to turn off PoW](https://github.com/ethereum/eth2.0-specs/pull/2257) via fork choice change
- First “turn off PoW” transaction prototypes: SigmaPrime [pairs with Catalyst](https://twitter.com/sigp_io/status/1374979655782989824) and Aditya [uses py-evm and the spec](https://twitter.com/adiasg/status/1373938241200549889)
- Prater [devnet launch went well](https://prater.beaconcha.in/)
- [Open challenges in staggering shards](https://www.reddit.com/r/ethereum/comments/mbksxt/shard_block_staggering_for_faster_block_times/) for very fast block times
- Ethstaker’s community call on [turning off PoW with lead devs Mikhail Kalinin and Guillaume Ballet](https://www.youtube.com/watch?v=tL8l7GGCpw0)
- chaind [v0.3.1](https://github.com/wealdtech/chaind/releases/tag/v0.3.1) to analyze beacon chain data, adds eth1 deposits, Prometheus metrics
- Step by step [video guides to staking at home](https://twitter.com/unvetica/status/1375288837648216064)

**Layer2**

- Arbitrum’s [mainnet release candidate](https://medium.com/offchainlabs/arbitrum-updates-buckle-up-80483d71718c), includes BLS sigs. Compatible with EVM at bytecode, so your Solidity contracts and tools work.
- Hop [cross-EVMchain AMM exchange](https://medium.com/hop-protocol/hop-send-tokens-across-rollups-30f14c432f7c) to go live in April with xdai, Polygon and Arbitrum
- Optimism [delays launch](https://optimismpbc.medium.com/optimistically-cautious-767a898f90c8) until at least July, testnet for Scaling Ethereum hackathon in April
- Zk rollup [Hermez is live](https://twitter.com/hermez_network/status/1374663423678689287) with ETH, HEZ, WBTC, USDT and DAI transfers

* * *

### **This newsletter is made possible thanks to Matcha!**

![Matcha](https://weekinethereumnews.com/wp-content/uploads/2020/06/matcha-avatar.png)

Matcha aggregates liquidity across decentralized exchange networks to offer you the best price on every token swap on both spot **and limit orders**!

Now you can [trade 1000+ DeFi tokens](https://matcha.xyz/?id=wien) on Matcha!

* * *

**Stuff for developers**

- Solidity [v0.8.3](https://blog.soliditylang.org/2021/03/23/solidity-0.8.3-release-announcement/) - bugfix for keccak caching in the optimizer
- OpenZeppelin Contracts [v0.4](https://blog.openzeppelin.com/openzeppelin-contracts-4-0), SafeMath now just a wrapper, storage optimizations, GSN v2
- Remix [v0.11](https://medium.com/remix-ide/remix-release-0-11-1-cdb3063327d?source=friends_link&sk=a5311bb887d4a25c0de586584e934845) series adds Workspaces
- Latest [dapptools (hevm, seth, dapp) release](https://github.com/dapphub/dapptools/releases/tag/hevm%2F0.45.0), eip712 signing, better fuzzing and symbolic execution
- [Micro eth signer](https://github.com/paulmillr/micro-eth-signer) fully functional 5kB (+26kB dependencies) library
- Make your [app GnosisSafe compatible](https://medium.com/@gnosisPM/turn-your-dapp-into-a-gnosis-safe-app-in-5-minutes-5cdb33a1cd46) in 5 mins
- [Usedapp framework](https://medium.com/ethworks/introducing-usedapp-framework-for-rapid-dapp-development-4959361f242a) from EthWorks uses ethers, web3-react, Maker’s multicall, and Waffle
- [Infernal simple dapp](https://github.com/admazzola/infernal-simple-dapp) with Vue and NodeJS
- [Let’s find a prime](https://medium.com/nethermind-eth/lets-find-a-prime-d5ee8b4643cc) using Cairo
- Tutorial for [Hardhat deploy](https://github.com/wighawag/tutorial-hardhat-deploy#readme)
- Introducing [NFT flash loans](https://medium.com/nft20/introducing-nft-flash-loans-97ff8c9298d4)
- [Fe dev update](https://snakecharmers.ethereum.org/fe-development-update-4/) 4, includes uniswap v2 demo

**Security/incidents**

- [Forcing bad swaps on yield farming](https://medium.com/dedaub/yield-skimming-forcing-bad-swaps-on-yield-farming-397361fd7c72) by manipulating the price and calling harvest
- Samczsun and Tina Zhen [save $4.5m from an ElasticDAO](https://medium.com/elasticdao/elasticdao-smart-contract-and-security-audits-400f424281b6) unguarded transfer function
- [Conkas](https://github.com/nveloso/conkas) modular static analysis tool
- One year [fuzzing the Solidity compiler](https://blog.trailofbits.com/2021/03/23/a-year-in-the-life-of-a-compiler-fuzzing-campaign/)

**Ecosystem**

- An expansive guide to the [Ethereum blockspace market](https://www.aniccaresearch.tech/blog/ethereum-blockspace-who-gets-what-and-why)
- [Shutter network](https://shutter.ghost.io/introducing-shutter-network-combating-frontrunning-and-malicious-mev-using-threshold-cryptography/): threshold cryptography to combat frontrunning; Goerli testnet version released soon
- [NFTHack winners](https://twitter.com/ETHGlobal/status/1373732014038335492)
- EF [q4 2020 grantees](https://blog.ethereum.org/2021/03/22/esp-allocation-update-q4-2020/)
- $4m in 2021 EF grants to [support Ethereum client diversity](https://blog.ethereum.org/2021/03/23/supporting-ethereums-client-ecosystem/) to Besu, Geth, Nethermind, OpenEthereum, and Turbogeth
- Ethereum on ARM: [updated Raspberry Pi4 images](https://www.reddit.com/r/ethereum/comments/mc83tp/ethereum_on_arm_image_for_the_raspberry_pi_4_with/) for all mainnet and PoS clients

**Enterprise**

- [Spanish corporate coalition for digital identity](https://www.intelligentcio.com/eu/2021/03/25/spanish-companies-join-forces-to-promote-digital-identity-using-blockchain-technology/) built on Ethereum

**Application layer**

- [Uniswap v3](https://twitter.com/Uniswap/status/1374407380520239109) announced: concentrated liquidity positions for less trader slippage, fee flexibility, better oracles
- Gyroscope’s [incentivized testnet](https://medium.com/gyroscope-protocol/gyrosoft-all-weather-simulator-join-the-gyroscope-gamified-testnet-b6c5366ec87e)
- Giveth [relaunches](https://medium.com/giveth/the-future-of-giving-is-here-d480388a3338) with fee-free donations, and noob-friendly by using Torus
- Monty Python’s John Cleese is selling an [NFT drawing of the Brooklyn Bridge](https://twitter.com/JohnCleese/status/1372944852325789704)
- [Time Mag is selling its 3 “God/Truth/Fiat is dead” NFT covers](https://twitter.com/brianstelter/status/1373837686780350472). So even a [NYTimes columnist is doing it](https://www.nytimes.com/2021/03/24/technology/nft-column-blockchain.html?s=09#click=https://t.co/9ItGZvID8B)
- [This Artwork Earns Yield](https://thisartworkearnsyield.com/), a spinoff of Simon’s always onsale art
- Robin Sloan & Nick Johnson’s [Amulets](https://twitter.com/WildAmulet/status/1374506730575437828) - NFTs minted (40k gas!) when you find short poems whose SHA256 hash contains many consecutive eights.

**Regulation/business/tokens**

- [Eth as ultrasound money](https://newsletter.banklesshq.com/p/ultra-sound-money-), David Hoffman’s long read
- [Staked Eth trust](https://twitter.com/staked_us/status/1375086818379636743), custody by Fireblocks to get exposure to staked ETH
- [Value accrual in the NFT stack](https://coopahtroopa.mirror.xyz/A16NP2XXi9RdHptfdF9WHR0Xq_E1XDmUgMwPmJYOG7w)
- [NewYorker Beeple profile](https://www.newyorker.com/tech/annals-of-technology/how-beeple-crashed-the-art-world) reveals he immediately sold his ETH from Christie’s payday
- [Public opinion period on FATF’s attempt to choke DeFi](http://www.fatf-gafi.org/publications/fatfrecommendations/documents/public-consultation-guidance-vasp.html) with regulations. Deadline to file a comment is April 20

**General**

- Vitalik: [legitimacy is the scarce resource](https://vitalik.ca/general/2021/03/23/legitimacy.html)
- Interview with [EF Executive Director Aya Miyaguchi](https://empodera.org/impact/en/experiences/experience/aya-miyaguchi)
- [Aggregatable distributed keygen](https://www.benthamsgaze.org/2021/03/24/aggregatable-distributed-key-generation/) paper in blog post form
- The SNL [skit on NFTs](https://www.youtube.com/watch?v=mrNOYudaMAc)

* * *

## **Job Listings**

- New DeFi protocol Tokemak seeks [Solidity](https://opolist.opolis.co/opps/8/) and [Frontend](https://opolist.opolis.co/opps/9/) devs. Attractive comp
- Gnosis is hiring! [Ethereum Core Developer](http://bit.ly/3cZMzeS), [Frontend Engineer](http://bit.ly/3vM126R), [Rust Engineer](http://bit.ly/3f1Jkq7)
- Chainsafe is looking for a [Typescript dev](https://chainsafe.io/careers/openpositions/ethereum-typescript-developer) to work on Lodestar eth2 client
- Nomic Labs (Hardhat/Buidler) is hiring a [senior dev and an engineering manager](https://www.notion.so/Nomic-Labs-jobs-991b37c547554f75b89a95f437fd5056)
- Junior devs: Nethermind is looking for [junior Solidity, data analysts, nodeJs devs](https://twitter.com/nethermindeth/status/1371830788329779210)

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-march-28-2021/](https://weekinethereumnews.com/week-in-ethereum-news-march-28-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Apr 9 - May 14 - ETHGlobal’s [Scaling Ethereum](https://scaling.ethglobal.co/) hackathon
- April 14 - [Berlin upgrade fork](https://github.com/ethereum/pm/issues/248#issuecomment-782069875) (testnets: Ropsten Mar 10, Goerli Mar 17, Rinkeby Mar 24)
- April 16 - [Rollup community grant](https://esp.ethereum.foundation/en/rollup-grants/) applications due
- April 20 - deadline for [beacon chain security and testing RFP](https://notes.ethereum.org/@lsankar/security-rfp)
- **April 20 - deadline to [comment on FATF anti-DeFi](http://www.fatf-gafi.org/publications/fatfrecommendations/documents/public-consultation-guidance-vasp.html) regulatory proposal**
- April 22 - [Ethereum in the Enterprise 2021](https://www.conference2021.entethalliance.org/)
- May 14 - papers due for [WoSCA 2021](https://trailofbits.github.io/WoSCA/)
- Jul 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

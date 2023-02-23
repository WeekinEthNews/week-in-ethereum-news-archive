---
title: "Week in Ethereum News <BR> Feb 28, 2021"
date: "2021-02-28"
---

## **Eth News and Links**

**Mainnet**

- Vitalik and Micah propose a [different state-shrinking approach](https://ethresear.ch/t/resurrection-conflict-minimized-state-bounding-take-2/8739), a yearlong form of regenesis
- Test suite [v7.0.2](https://github.com/ethereum/tests/releases/tag/7.0.2) - Berlin fork with access lists
- [EIP3298](https://eips.ethereum.org/EIPS/eip-3298): removal of refunds, eg no more GasToken. Proposed for London
- [EIP3300](https://github.com/ethereum/EIPs/blob/9034dbdf1b526773e5210125fbadaa7ae4df8ace/EIPS/eip-3300.md): Phase out refunds, an EIP3298-alternative

**EIP1559**

- EIP[1559 proposed for the London fork](https://github.com/ethereum/pm/issues/254) in July, should be discussed next core devs call
- Data from the [1559 large state performance test](https://hackmd.io/@abdelhamidbakhta/eip1559-perf-update)
- Beiko’s [1559 update](https://hackmd.io/@timbeiko/1559-updates/https%3A%2F%2Fhackmd.io%2F%40timbeiko%2F1559-update-007): commentary on most of the links here
- F2Pool [supports 1559](https://f2pool.medium.com/staying-on-the-b-right-side-of-history-eip-1559-bd36522eec17), a full list of [mining pool opposition/support](https://bi.etherscan.io/public/dashboards/herQuzBsRSG74mltImaH4jnnMnRR7LNsDkh3cpyT?org_slug=default)
- A list of applications and projects by [whether they support 1559](https://github.com/ethereum-cat-herders/1559-outreach)
- [Miners will accept eip1559](https://insights.deribit.com/market-research/miners-will-accept-eip-1559-here-is-why/), because the alternatives are far worse for them
- Establishing bounds for [fee burn under eip1559](https://insights.deribit.com/market-research/establishing-bounds-for-miner-revenue-in-eip-1559/) using MEV
- Leonardos, Monnot, et al: [Dynamic analysis of 1559 basefee](https://arxiv.org/abs/2102.10567)
- [Understanding fees in 1559](https://barnabe.substack.com/p/understanding-fees-in-eip1559)
- A Twitter thread summarizing perspectives in the 1559 [community call](https://twitter.com/TimBeiko/status/1365299318589120513)

**Proof of Stake**

- Ethereum proof of stake has more than [100k validators](https://stakers.info/)
- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210227)
- Latest [Eth2 call](https://youtu.be/yrDVhoTg5XU?t=283). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/B1BZs7SMO) and [Alex Stokes](https://twitter.com/ralexstokes/status/1364971012018872330), first upgrade probably happens in June
- High level [plan for first upgrade](https://notes.ethereum.org/@djrtwo/hf1-plan) -> spec, ephemeral testnets, multiclient testnets, as said above: targeted for June
- Spec [v1.0.1](https://github.com/ethereum/eth2.0-specs/releases/tag/v1.0.1), adds withdrawal credentials for trustless staking pools
- [Secret shared validators](https://medium.com/coinmonks/eth2-secret-shared-validators-85824df8cbc0) update
- Latest [lighthouse client update](https://lighthouse.sigmaprime.io/update-34.html): explains the block propagation improvement as well as source/head/target rewards, plus an amusing memory optimization

**Layer2**

- dYdX [launches their Starkware zkrollup](https://dydx.exchange/blog/alpha) for cross-margined perpetuals, it’s on mainnet for invitees only, full public release planned for a few weeks
- Optimism plans [mainnet in March](https://medium.com/ethereum-optimism/dope-hires-moar-mainnet-in-march-174fa8966361)
- Deversifi adds [swaps on its](https://twitter.com/deversifi/status/1363804660847493122) Validium implementation
- [Efficient mechanism to prove ORU calldata](https://ethresear.ch/t/efficient-mechanism-to-prove-oru-calldata/8770)
- An [optimistic/zkrollup combination](https://ethresear.ch/t/a-pre-consensus-mechanism-to-secure-instant-finality-and-long-interval-in-zkrollup/8749) idea

* * *

### **This newsletter is made possible thanks to [Matcha](https://matcha.xyz/?id=wien) by [0x](https://0x.org/)!**

![Matcha](https://weekinethereumnews.com/wp-content/uploads/2020/06/matcha-avatar.png)

Matcha aggregates liquidity across decentralized exchange networks to offer you the best price on every token swap on both spot **and limit orders**!

Now you can [trade 1000+ DeFi tokens](https://matcha.xyz/?id=wien) on Matcha!

* * *

**Stuff for developers**

- Faster Truffle [v5.2](https://github.com/trufflesuite/truffle/releases/tag/v5.2.0) via webpack5 update, supports multiple solc versions
- Blocknative’s [gas platform](https://www.blocknative.com/blog/introducing-gas-platform) uses transaction pool for gas price predictions
- Etherscan implements a [diffchecker](https://etherscan.io/contractdiffchecker)
- Getting [Geth running on RISC-V](https://blog.davidburela.com/2020/12/03/ethereum-on-risc-v/)
- Starkware’s [voting app in Cairo tutorial](https://www.cairo-lang.org/from-voting-to-trustless-eth-bridges-via-signature-aggregation/) can be modified for signature aggregation

**Security/incidents**

- Cryptopunks [frontrunning from lack of frontend protection](https://twitter.com/aradtski/status/1364714105525964811)
- samczun finds [ForTube vulnerability](https://medium.com/the-force-protocol/fortube-security-vulnerability-fix-c5847359ba7d) where verification logic could be bypassed
- [PrimitiveFinance postmortem](https://primitivefinance.medium.com/postmortem-on-the-primitive-finance-whitehack-of-february-21st-2021-17446c0f3122) after Dedaub found a lack of checking who called Uniswap
- A look at how the [Furucombo proxy got compromised](https://twitter.com/Kurt_M_Barry/status/1365876788757471234) for about $15m
- Armor [founder gets social engineered](https://twitter.com/ArmorFi/status/1365863250827620352)
- Github: avoiding [npm substitution attacks](https://github.blog/2021-02-12-avoiding-npm-substitution-attacks/)

**Ecosystem**

- [Quantifying MEV](https://medium.com/flashbots/quantifying-mev-introducing-mev-explore-v0-5ccbee0f6d02): the flashbots [dashboard](https://explore.flashbots.net/) and tx frontrunning explorer: at least $314m in MEV since start of 2020, with $57m in Jan 2021. 88% of it so far captured by traders, not miners
- Chainlink now [aggregates oracle responses offchain](https://blog.chain.link/off-chain-reporting-live-on-mainnet/) resulting in only 1 mainnet transaction
- [Umbra stealth payments](https://www.scopelift.co/blog/umbra-phase-one) is on Rinkeby testnet, looking for testers and aiming for April mainnet

**Enterprise**

- JPMorgan [testing satellite-to-satellite IoT payments in space](https://www.reuters.com/article/idUSL1N2KT0RA) using Quorum
- [6 massive commodity trading firms consortia chain goes live](https://www.ledgerinsights.com/cargill-adm-backed-commodities-agribusiness-blockchain-covantis-live/), built on Quorum, with corn and soybean exports from Brazil

**Application layer**

- [BAT roadmap v2](https://brave.com/bat-roadmap-2-0/): redesigned Brave crypto wallet, dex aggregator possibly with Brave’s own liquidity pools and/or on l2
- Livepeer video [transcoding up 20x+ since summer](https://medium.com/livepeer-blog/metrics-that-matter-minutes-of-video-transcoded-by-the-livepeer-network-e9b298d9ac5f)
- Kyber paper on [Dynamic AMMs](https://files.kyber.network/DMM-Feb21.pdf) flexible fees and flexible pricing curves
- Cover introduces [credit default swaps](https://coverprotocol.medium.com/introduce-credit-default-swaps-a68a3a22b7aa) starting with Ruler

**Regulation/business/tokens**

- Canada likely to get the [first Ether ETF](https://www.businesswire.com/news/home/20210225005360/en/CI-Global-Asset-Management-Files-Preliminary-Prospectus-for-World%E2%80%99s-First-Ether-ETF) on TSX under ETHX
- Coinshares launches an [ETH product on Six Swiss](https://www.bloomberg.com/news/articles/2021-02-24/coinshares-is-launching-an-exchange-traded-ethereum-product) exchange
- Bitfinex pays $18.5m to settle with NYAG over Tether probe. Bitfinex puts out [press release](https://www.bitfinex.com/posts/608) emphasizing no admission of wrongdoing. [NYAG press release is subtitled](https://ag.ny.gov/press-release/2021/attorney-general-james-ends-virtual-currency-trading-platform-bitfinexs-illegal): “…Overstating Reserves, Hiding Approximately $85m in Losses…” Tether/Bitfinex now banned in New York.
- Common Stack: the [commons simulator game is live](https://medium.com/commonsstack/the-commons-simulator-game-is-live-e1986615a105)
- Chris Dixon: [NFTs and Kevin Kelly’s 1000 true fans](https://a16z.com/2021/02/27/nfts-and-a-thousand-true-fans/)

**General**

- [Coinbase files S-1](https://www.sec.gov/Archives/edgar/data/1679788/000162828021003168/coinbaseglobalincs-1.htm), so we get to see financials and user stats. Lost 30m in 2019, made 330m in 2020, 1.3b 2020 topline, 43m users, [no headquarters](https://blog.coinbase.com/coinbase-is-a-decentralized-company-with-no-headquarters-a9762c02546), etc
- NYT notices [NFT art](https://www.nytimes.com/2021/02/22/business/nft-nba-top-shot-crypto.html) sales
- Revised [Proof-Carrying Data without Succinct Arguments](https://eprint.iacr.org/2020/1618) paper

* * *

## **Job Listings**

- Get paid to work on open source! [Rust](https://chainsafe.io/careers/openpositions/rust-developer), [Golang](https://chainsafe.io/careers/openpositions/lead-golang-developer), [Solidity](https://chainsafe.io/careers/openpositions/solidity-engineer). [Join ChainSafe](https://chainsafe.io/careers/openpositions)!
- Earn governance rights as a Tracer Perpetual Swap Alpha Tester, [apply here.](https://tracer-finance.typeform.com/to/CLDvv8H7)
- [Chorus One](https://chorus.one/careers/) has open engineering & business positions
- [Props](https://www.propsproject.com/) is hiring [General Counsel](https://www.propsproject.com/careers?gh_jid=2931365) and [Head of Finance & Capital Markets](https://www.propsproject.com/careers?gh_jid=2933297)
- Trail of Bits is looking for a [blockchain security engineer](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf)
- 0x: [devs of all types](https://0x.org/about/jobs) and a [data analyst](https://boards.greenhouse.io/0x/jobs/4220949002)
- ethereum.org is [hiring a front end dev](https://ethereum.bamboohr.com/jobs/view.php?id=32)
- [Apply](https://tracer-finance.typeform.com/to/hdGN3pYu) to govern the way we trade with the Tracer DAO. 
- Prysmatic Labs is looking for a [Go dev to work on their eth2 client](https://prysmaticlabs.com/careers)
- Eth2 client Teku is looking for a “[mid- to senior-level Java dev](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210227)”
- Nimbus [eth2 client looking for developer experience lead](https://status.im/our_team/open_positions.html?gh_jid=2386730)

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-feb-28-2021/](https://weekinethereumnews.com/week-in-ethereum-news-feb-28-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Feb 28 - [Nimbus Grafana dashboard](https://twitter.com/ethnimbus/status/1360273972944920582) submissions due
- Mar 1-5 - Ethereum Foundation’s [Ecosystem Support Program](https://twitter.com/EF_ESP/status/1362817256774893568) office hours
- Mar 5 - Financial Cryptography [DeFi academic workshop](https://fc21.ifca.ai/defi/)
- **Mar 10-25 - [Gitcoin CLR matching grants](https://gitcoin.co/grants/) round**
- Mar 19-21 - ETHGlobal’s [NFT Hack](https://nft.ethglobal.co/)
- Apr 9 - May 14 - ETHGlobal’s [Scaling Ethereum](https://scaling.ethglobal.co/) hackathon
- April 14 - [Berlin upgrade fork](https://github.com/ethereum/pm/issues/248#issuecomment-782069875) (testnets: Ropsten Mar 10, Goerli Mar 17, Rinkeby Mar 24)
- May 14 - papers due for [WoSCA 2021](https://trailofbits.github.io/WoSCA/)
- Jul 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

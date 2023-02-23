---
title: "Week in Ethereum News <BR> May 23, 2021"
date: "2021-05-23"
---

## **Eth News and Links**

**Mainnet execution layer**

- Why we [needed to increase gas for state access opcodes](https://blog.ethereum.org/2021/05/18/eth_state_problems/).  Hubert Ritzdorf, Matthias Egli and Daniel Perez had found a cheap way to spam attack the network.  Dynamic state snapshots in Geth as mitigation in combination with EIP2929 and EIP2930.
- [EIP1559 cheatsheet](https://hackmd.io/@q8X_WM2nTfu6nuvAzqXiTQ/1559-wallets) for wallet devs & users
- London testnet Baikal shows [EIP1559 transaction data in block explorer](https://twitter.com/timbeiko/status/1395416223395975169)
- Beiko's [core devs update](https://hackmd.io/@timbeiko/acd/https%3A%2F%2Fhackmd.io%2F%40timbeiko%2Facd-update-003): an overview of progress on London and turning off PoW
- [Turbo-Geth renaming to Erigon](https://twitter.com/ErigonEth/status/1394273529613389825), also reimplementing Erigon into C++ and Rust clients named Silkworm and Akula respectively
- Vitalik’s [dust cleanup ideas](https://ethereum-magicians.org/t/some-medium-term-dust-cleanup-ideas/6287)

**EIPs/Standards**

- [EIP3584](https://eips.ethereum.org/EIPS/eip-3584): Block Access List

**Proof of stake consensus layer**

- Latest [PoS implementers call](https://youtu.be/A1L7wLYAqnM?t=145).  Notes from [Ben Edgington](https://hackmd.io/@benjaminion/r1-aSk4tu) and [Alex Stokes](https://twitter.com/ralexstokes/status/1395419727875379200).  Client improvements and getting ready for Altair upgrade 
- [Teku speeds up syncing](https://consensys.net/blog/teku/teku-and-infura-team-up-to-make-the-fastest-ethereum-2-0-client-sync) with weak subjectivity checkpoints and Infura
- [Nimbus v1.3.0](https://github.com/status-im/nimbus-eth2/releases/tag/v1.3.0): safer and easier options to migrate from other clients
- Latest [what’s new in PoS](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210522). Ben’s view is that PoW switch off is more likely to happen in Q1 2022 than this year

**Layer2**

- Kris Kaczor’s tweetstorm [comparing Arbitrum and Optimism](https://twitter.com/krzKaczor/status/1395812308451004419)’s optimistic rollups
- Etherscan now provides a [block explorer for Optimism](https://optimismpbc.medium.com/integrating-etherscan-24a3811a765c)
- [The Verifier’s Dilemma in-depth](https://medium.com/onther-tech/optimistic-rollup-is-not-secure-enough-than-you-think-cb23e6e6f11c) for fraud proof systems
- [Connext’s virtual AMMs and liquidity auctions](https://medium.com/connext/solving-the-liquidity-problem-88bde201501) for load balancing in cross-chain swaps
- An overview of the [differences between optimistic rollups and zk rollups](https://insights.deribit.com/market-research/making-sense-of-rollups-part-one-optimistic-vs-zero-knowledge/)
- Patrick McCorry: [the bridge determines what is Layer 2](https://stonecoldpat.medium.com/a-note-on-bridges-layer-2-protocols-b01f8fc22324)

* * *

### **This newsletter is made possible thanks to [Celer](https://www.celer.network/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

[Celer](http://celer.network/) is a coherent layer-2 scaling platform on Ethereum powered by [Generalized State Channel Network](https://www.celer.network/docs/celercore/index.html) and [Rollup](https://medium.com/celer-network/adding-hybrid-pos-rollup-sidechain-to-celers-coherent-layer-2-platform-d1d3067fe593) technology. 

Celer recently launched [Layer2.finance](https://layer2.finance/), a layer-2 rollup-based DeFi aggregator that acts as a low-cost and trust-free gateway for the users to explore and benefit from the existing DeFi ecosystem with 100X lower cost. Layer2.finance achieves scalability “in-place” with no protocol migration needed and therefore, does not cause liquidity fragmentation or break composability. You can use the app here: [app.l2.finance](http://app.l2.finance). 

Follow Celer on [twitter](https://twitter.com/CelerNetwork), [blog](https://blog.celer.network/), [discord](https://discord.com/invite/Trhab5w) and [telegram](https://t.me/celernetwork).

* * *

**Stuff for developers**

- [Ethers v5.2.0](https://blog.ricmoo.com/highlights-ethers-js-may-2021-2826e858277d), custom contract errors, detect replacement transactions
- [Starlight](https://github.com/EYBlockchain/starlight): EY’s prototype transpiler to write ZKapps in Solidity
- The most popular secp256k1 library (elliptic) for node & browsers is lightly maintained.  Consider [switching to noble](https://twitter.com/paulmillr/status/1393193702542254081)
- [EVM tool to run ABI encoded data](https://github.com/fxfactorial/run-evm-code) for a receiver, sender and block
- [evm-fp](https://github.com/paulrberg/evm-fp): multiplies by 1e18 to make tests more declarative
- [GSN v2](https://blog.opengsn.org/whats-technically-new-in-gsn-v2-68ab9ad0cc1)’s decentralized meta transaction relayers launches with better relay routing and anti-griefing protections: allow users to pay gas in any token/fiat
- Wallet devs join the [London Infrastructure Readiness](https://github.com/ethereum/pm/issues/323) call, includes what [naming to expose to users](https://twitter.com/timbeiko/status/1395478940186071040)
- A tutorial on using [Splunk to analyze Geth metrics, logs and ledger data](https://medium.com/splunk-dlt/geth-hosting-with-splunk-62045c615ab4)
- Share with web devs - we need them: [Austin Griffith scaffold-eth onboarding video for web2 devs](https://twitter.com/austingriffith/status/1394656757721403400)
- freeCodeCamp's [intro to web3](https://www.freecodecamp.org/news/what-is-web3/)

**Security**

- Binance’s chain suffers multiple attacks: 
    - Bunny Finance [~$45m lost in economic exploit](https://twitter.com/FrankResearcher/status/1395196961108774915) by manipulating the BUNNY mint price
    - Venus’s $100m+ in [cascading liquidations](https://twitter.com/FrankResearcher/status/1394900186435096578) from manipulating price reported by a Chainlink oracle
    - bEarn $11m lost due to [bug in internal withdraw logic](https://peckshield.medium.com/bearn-fi-incident-inconsistent-asset-denomination-between-vault-strategy-9b24b68ab1c0)
- Analysis of [Meebit NFT rare mint claim exploit](https://iphelix.medium.com/meebit-nft-exploit-analysis-c9417b804f89)
- yEarn finds [flaw in yvWETH MakerDAO strategy accounting logic](https://github.com/yearn/yearn-security/blob/master/disclosures/2021-05-20.md); no funds lost

**Ecosystem**

- Ethereum will use [~99.95% less energy when we switch off](https://blog.ethereum.org/2021/05/18/country-power-no-more/) proof of work
- [Vitalik burns 90% of their remaining dog meme tokens](https://etherscan.io/tx/0x7a69f558bdc4aaf1e6bab9473c84cb2fddbd1e419c44d5c22eb88bedeb09657c) with message: plans to donate 10% and asks projects not to give him tokens/power without consent
- Out: “seed phrase.” In: “[secret recovery phrase](https://twitter.com/pedrouid/status/1393974705162440705)”
- [Addressing common criticisms about Ethereum](https://www.reddit.com/r/ethereum/comments/najp2c/addressing_common_criticisms_about_ethereum/)
- [Coinbase Wallet browser extension](https://blog.coinbase.com/coinbase-wallet-introduces-new-browser-extension-dd067403b86): confirm transactions on mobile app

**Enterprise**

- Birra Peroni goes [live on mainnet using EY OpsChain Traceability](https://www.ey.com/en_gl/news/2021/05/birra-peroni-is-the-first-industrial-organization-to-mint-unique-non-fungible-tokens-using-ey-opschain-traceability) to notarize information and tokenize goods as NFTs

**Application layer**

- [DeFi performance](https://twitter.com/jack_clancy93/status/1395399566644682757) during ETH price drop: DEX $10B volume day
- [Uniswap V3 flipped V2](https://twitter.com/RyanWatkins_/status/1395775319936806914) to be number one DEX
- The Wharton School: [DeFi Beyond the Hype](https://wifpr.wharton.upenn.edu/wp-content/uploads/2021/05/DeFi-Beyond-the-Hype.pdf)
- [Dark Forest v0.6](https://blog.zkga.me/announcing-v6) game is live: series of rounds over 2-3 months
- Rick and Morty co-creator Dan Harmon’s new [animated series Krapoplis](https://www.hollywoodreporter.com/tv/tv-news/dan-harmon-blockchain-nft-crypto-series-fox-1234954403) to use NFT marketplace
- [Charlie Bit My Finger video to be deleted from YouTube](https://medium.com/originprotocol/charlie-bit-my-finger-makes-internet-history-again-1e4a3c54db65) after being auctioned as NFT

**Regulation/business/tokens**

- [US Federal Reserve to release discussion paper in summer (US)](https://www.federalreserve.gov/newsevents/pressreleases/other20210520b.htm) on digital payments and establishing a CBDC
- US proposal for businesses to [report $10k+ crypto transactions to IRS](https://www.cnbc.com/2021/05/20/us-treasury-calls-for-stricter-cryptocurrency-compliance-with-irs.html)
- Three Chinese financial industry groups announced member [institutions shall not conduct business related to virtual currency](https://www.forbes.com/sites/jonathanponciano/2021/05/18/china-bans-banks-from-crypto-business-saying-speculative-trading-seriously-infringing-on-financial-order/?sh=160a9d277898)
- Placeholder VC: [Isomorphism in DAO governance](https://www.placeholder.vc/blog/2021/5/20/isomorphism-in-dao-governance)
- Proposed roadmap for [Synthetix](https://blog.synthetix.io/a-little-dash-of-hopium/): 4 subprojects will get their own token for coordinating micro-incentives within the projects 
- UK Conservative MP mentions ETH [flipping BTC in parliament](https://twitter.com/TomTugendhat/status/1395472853991051265) speech
- If Ethereum was a public company: [Ethereum Q1 results](https://draecomino.substack.com/p/ethereum-q1-2021-results) - transaction fees up 200x to $1.7 billion compared to $8 million in Q1 2020

**General**

- Dankrad Feist explains [what a 51% attack can and can’t do](https://dankradfeist.de/ethereum/2021/05/20/what-everyone-gets-wrong-about-51percent-attacks.html)
- Vitalik: [Limits to blockchain scalability](https://vitalik.ca/general/2021/05/23/scaling.html)
- [Social consensus is Layer 0](https://www.buildblockchain.tech/blog/code-law-and-the-nature-of-consensus) of blockchains
- [Run Node.js natively in the browser](https://blog.stackblitz.com/posts/introducing-webcontainers/), with [plans to get Hardhat working in a WebContainer](https://twitter.com/ericsimons40/status/1395905320564629508)
- Wired’s account of [RSA getting cracked in 2011](https://www.wired.com/story/the-full-story-of-the-stunning-rsa-hack-can-finally-be-told/)
- If you run Windows, [installing a CIS language keyboard](https://krebsonsecurity.com/2021/05/try-this-one-weird-trick-russian-hackers-hate/) can help keep your machine malware-free

* * *

## **Job Listings**

- Quant (options trading) is [hiring](https://jobs.lever.co/QuantLabs) for Solidity, full stack, & designers
- Very large game company [looking for devs/marketing](https://twitter.com/finestonematt/status/1395051881844592641) for NFT product
- WalletConnect: [Tech Product Manager](https://angel.co/company/walletconnect/jobs/1384299-technical-product-manager) and [DevOps/Backend Engineer](https://angel.co/company/walletconnect/jobs/1384334-devops-backend-engineer)
- Trail of Bits' [Blockchain Security Analyst Apprenticeship](https://jobs.lever.co/trailofbits/b2d6ce87-6b01-462f-965a-597a273ce26f) program
- Synthetix: [Growth Marketer](https://jobs.defialliance.co/companies/synthetix/jobs/4454460-growth-marketer), [Designer](https://jobs.defialliance.co/companies/synthetix/jobs/4538964-senior-designer), [Front End Eng](https://jobs.defialliance.co/companies/synthetix/jobs/4136036-front-end-engineer) and [Blockchain Eng](https://jobs.defialliance.co/companies/synthetix/jobs/4136037-senior-blockchain-engineer)

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of the workflow.

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-may-23-2021/](https://weekinethereumnews.com/week-in-ethereum-news-may-23-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- **May 26 - [London Infrastructure Readiness](https://github.com/ethereum/pm/issues/323) call**
- May 28 – optimistic rollup [Arbitrum launches](https://medium.com/offchainlabs/wen-arbitrum-634969c14713)
- May 28-30 – ETHGlobal’s [Web3 Weekend](https://web3.ethglobal.co/)
- **May 29 - Road to Devcon Quest: [EthStaker Painting Party](https://ethstaker.cc/road-to-devcon/)**
- May 31 – deadline to apply for [Eth core dev apprenticeship](https://blog.ethereum.org/2021/05/13/core-dev-apprenticeship/)
- June 18 – July 9 – [ETHGlobal – Hack Money 2021](https://hackmoney.ethglobal.co/)
- June 25-27 – [Edcon](https://www.edcon.io/) (Shenzhen/online)
- **July 10 - Road to Devcon Quest: [Devcon Trivia Game](https://ethstaker.cc/road-to-devcon/)**
- July 14 – [tentative date for London hard fork](https://docs.google.com/spreadsheets/d/1Y3yyTqeqRO1O2UFVkNkHK_V5oRulZd6y-JJbSnKYrb4/edit#gid=0) (Ropsten June 9, Goerli June 16, Rinkeby June 23)
- July 20-22 – [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

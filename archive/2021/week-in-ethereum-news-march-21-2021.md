---
title: "Week in Ethereum News <BR> March 21, 2021"
date: "2021-03-21"
---

## **Eth News and Links**

**Mainnet**

- Proposal to [prioritize turning off PoW](https://github.com/ethereum/pm/issues/278)
- Latest [core devs call](https://youtu.be/AclPXsRlgSc?t=26). Beiko’s [notes](https://twitter.com/TimBeiko/status/1372959274070986754): London upgrade fork will be 1559 and 3404 (mostly removing gas refunds). Turning off PoW preferred for the q4 2021 upgrade fork.
- Turbogeth [latest alpha](https://github.com/ledgerwatch/turbo-geth/releases/tag/v2021.03.01) release is Berlin ready
- New bugfix client releases for Berlin upgrade fork: Besu [v21.1.2](https://github.com/hyperledger/besu/releases/tag/21.1.2), OpenEthereum [v3.2.1](https://github.com/openethereum/openethereum/releases/tag/v3.2.1)
- [MiMC hashing using EVM384](https://hackmd.io/bHRfQfWaRmuIbNLTEQ6fyg). Lower gas cost than Circom, might need a setup mechanism to deal with Montgomery multiplication quirks
- [Scalable gossip for state network](https://ethresear.ch/t/scalable-gossip-for-state-network/8958)
- Lakshman's [state size management explainer](https://twitter.com/lakshmansankar/status/1372645109414563840) as to why verkle trees and epochal state expiry is currently the plan

**EIPs/Standards**

- [EIP3382](https://eips.ethereum.org/EIPS/eip-3382): hardcoded gas limit
- [EIP3404](https://github.com/ethereum/EIPs/blob/b52d409cdbdc6d296890913b3521a96b6d1bca04/EIPS/eip-3404.md): overhaul SLOAD/SSTORE costs and refunds
- [EIP3403](https://github.com/ethereum/EIPs/blob/8b1c4f7be8580bff9da11c6b099201b72f57fe3f/EIPS/eip-3403.md): remove gas refund except when changing SSTORE value to 0

**Proof of Stake**

- [Weak subjectivity checkpoint](https://eth2-fork-mon.stokes.io/#nav-ws-data) explainer, how this enables fast PoS sync
- Long-term plan to [upgrade to Casper CBC](https://www.reddit.com/r/ethereum/comments/m8pvfb/longterm_cbc_casper_plans/), possibly needing faster crypto
- Request for [security and testing proposals](https://notes.ethereum.org/@lsankar/security-rfp). Deadline April 20
- [Single secret leader election](https://www.reddit.com/r/ethereum/comments/m9j5cy/single_secret_leader_election_protocols/) explainer - keep the block producer secret to thwart attacks
- Lodestar’s plan to become an [eth2 light client in your browser](https://medium.com/chainsafe-systems/a-lodestar-for-eth2-da9e1a1ea8f2)
- Stakers: remember to update your nodes for the Berlin fork upgrade (no link)

**Layer2**

- [zkmoney](https://medium.com/aztec-protocol/launching-aztec-2-0-rollup-ac7db8012f4b): Aztec launches zk-zkrollup with private transactions, currently with a 1 ETH transaction cap. More on the [zk-zk architecture with TurboPLONK](https://medium.com/aztec-protocol/aztecs-zk-zk-rollup-looking-behind-the-cryptocurtain-2b8af1fca619)

* * *

### **This newsletter is made possible thanks to Trail of Bits!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/05/2314423.jpeg)

Trail of Bits wants YOU to [apply for a position](https://www.trailofbits.com/careers) on their team! Positions are open for blockchain security engineers, project managers, product managers, financial controllers, and more. Make a career-defining contribution and help direct the future of blockchain security at Trail of Bits.

* * *

**Stuff for developers**

- WalletConnect [v1.4](https://github.com/WalletConnect/walletconnect-monorepo/releases/tag/1.4.0), dynamic registry for mobile linking, 80kb modal
- Fork of Maker’s [multicall](https://github.com/0xsequence/sequence.js/tree/master/packages/multicall), fast batched rpc calls for your dapp, 1 line of code integration
- [Integrate ENS with `ReverseRecord`](https://medium.com/the-ethereum-name-service/integrate-ens-reverse-record-into-your-dapp-to-show-ownership-and-participation-of-your-users-882a4703fee2) to return multiple ENS names in a function call
- [Fundamentals of gas tokens](https://blog.openzeppelin.com/fundamentals-of-gas-tokens/) (until London fork renders them useless)
- Tutorial on [building an AMM](https://www.cairo-lang.org/build-a-scalable-cairo-basesd-automated-market-maker/) using StarkWare’s Cairo language
- [Restoring a buggy “this artwork is always on sale”](https://blog.simondlr.com/posts/the-story-of-restoring-a-digital-artwork-that-is-always-on-sale) by selling it to a new contract
- Sign of the times: guides to create and deploy an NFT from [OpenZeppelin](https://forum.openzeppelin.com/t/create-an-nft-and-deploy-to-a-public-testnet-using-remix/6358) and [Quiknode](https://www.quiknode.io/guides/solidity/how-to-create-and-deploy-an-erc-721-nft)

**Security/incidents**

- Cream and Pancake [victim of a DNS hijacking](https://medium.com/cream-finance/postmortem-report-of-dns-hijacking-66ab9c6ce63d)
- A [governance attack on True Seigniorage Dollar](https://twitter.com/TrueSeigniorage/status/1370956726489415683)

**Ecosystem**

- MetaMask v9.2 [adds multiple hardware wallet acounts](https://github.com/MetaMask/metamask-extension/releases/tag/v9.2.0)
- DuneAnalytics [v2](https://duneanalytics.com/blog/dune-v2), much faster and auto refresh
- [Flashbots now have 12% of hashpower](https://medium.com/flashbots/flashbots-transparency-report-february-2021-8ac45b467d0a), bundle simulation now in ethers and web3py
- [Rescuing tokens in a compromised account](https://twitter.com/smpalladino/status/1373048978443472897) using Flashbots
- [Quantifying realized extractable value](https://hackmd.io/IGlkjRDrTmSJf_MM_f2Bcg), an MEV framework
- Attacking the attackers: tricky [ERC20 reaps 130 ETH](https://twitter.com/fifikobayashi/status/1372916327837405184) from sandwich attackers and [sandwich attackers are sandwiching sandwichers](https://twitter.com/fifikobayashi/status/1372338964326092802)

**Enterprise**

- Gartner Supply Chain Breakthrough of the Year award: [Microsoft’s e2e item tracability solution built on Ethereum](https://www.gartner.com/en/newsroom/press-releases/2021-03-18-gartner-announces-supply-chain-winners-of-the-2021-power-of-the-profession-awards)
- Meitu buys a [second round of $22m in ETH](https://corp-static.meitu.com/corp-new/ENG.pdf) and $18m in BTC

**Application layer**

- Sotheby’s to [auction Archillect/Murat Pak artwork](https://www.sothebys.com/en/coming-soon-collaboration-with-leading-digital-artist-pak)
- MetaKovan [drops pseudonymity](https://metapurser.substack.com/p/nfts-the-first-5000-beeples), funds five $100k scholarships for storytellers
- [Patrick Mahomes sells NFTs](https://www.espn.com/nfl/story/_/id/31078049/kansas-city-chiefs-patrick-mahomes-enters-world-nfts), following [Gronk making almost 2m](https://twitter.com/NTmoney/status/1371256030982668289)
- Mark Cuban to [sell MavPunks](https://twitter.com/mcuban/status/1373434052649320449), Charmin is selling [NFT(P)](https://rarible.com/charmin)
- [Mandalas:](https://mandalas.eth.link/) autogenerated bitmaps on bonding curve; no backend, it’s all onchain (I bought one)
- [Showtime](https://tryshowtime.com/): a museum/social layer for NFT cryptoart
- [USDC tops 10b](https://www.circle.com/blog/usdc-market-cap-tops-10-billion), Maker with a proposal to raise [ETH debt ceiling from 2.5b to 15b](https://twitter.com/MakerDAO/status/1372979697517174785)

**Regulation/business/tokens**

- FATF aims to kill DeFi with [insanely restrictive AML guidance](http://www.fatf-gafi.org/media/fatf/documents/recommendations/March%202021%20-%20VA%20Guidance%20update%20-%20Sixth%20draft%20-%20Public%20consultation.pdf)
- Bank of America: [DeFi is more disruptive than Bitcoin](https://www.coindesk.com/bank-of-america-defi-potentially-more-disruptive-than-bitcoin)
- [Reef calls out FTX/Alameda](https://medium.com/reef-finance/our-official-response-to-recent-events-regarding-alameda-a1978f7fbe57) for a token flip deal gone bad. Rekt [sides with Reef](https://www.rekt.news/reef-vs-alameda/)
- Tyler Cowen: the [NFT craze makes sense](https://www.bloomberg.com/opinion/articles/2021-03-17/the-nft-craze-actually-does-make-sense)
- Justin Drake’s [Eth as ultrasound Money meme](https://twitter.com/drakefjustin/status/1371755140399632388) continues to pick up steam as fee burning should exceed issuance
- Vlad Zamfir [sues over rights to the Casper name](https://twitter.com/VladZamfir/status/1372323671310807040)

**General**

- Vitalik’s “[how bulletproof-style polynomial commitments work](https://twitter.com/VitalikButerin/status/1371844878968176647)” visual explainer
- Groth: [non-interactive distributed keygen and resharing](https://eprint.iacr.org/2021/339)
- Nvidia [driver update accidentally unlocked RTX3060](https://www.msn.com/en-us/news/technology/nvidia-confirms-it-accidentally-unlocked-rtx-3060-ethereum-mining/ar-BB1eDzHA) for Eth mining
- [Honeybee](https://blog.trailofbits.com/2021/03/19/un-bee-lievable-performance-fast-coverage-guided-fuzzing-with-honeybee-and-intel-processor-trace/): speed up Intel Processor Trace for faster coverage-guided fuzzing
- Phone numbers in crypto considered harmful: a [hacker got all my text messages for $16](https://www.vice.com/en/article/y3g8wb/hacker-got-my-texts-16-dollars-sakari-netnumber)

* * *

## **Job Listings**

- ethereum.org is [hiring a front end dev](https://ethereum.bamboohr.com/jobs/view.php?id=32)
- Building blockchains with [ChainSafe](https://chainsafe.io/careers/openpositions). Join us! [Rust](https://chainsafe.io/careers/openpositions/rust-developer), [Golang](https://chainsafe.io/careers/openpositions/lead-golang-developer), [Solidity](https://chainsafe.io/careers/openpositions/solidity-engineer), [TS](https://chainsafe.io/careers/openpositions/ethereum-typescript-developer)
- Junior devs: Nethermind is looking for [junior Solidity, data analysts, nodeJs devs](https://twitter.com/nethermindeth/status/1371830788329779210)
- Nomic Labs is hiring a [senior dev and an engineering manager](https://www.notion.so/Nomic-Labs-jobs-991b37c547554f75b89a95f437fd5056)
- New DeFi protocol Tokemak seeks [Solidity](https://opolist.opolis.co/opps/8/) and [Frontend](https://opolist.opolis.co/opps/9/) devs. Attractive comp
- [Powerloom Protocol](https://powerloom.io/) is looking for [Distributed Systems Engineers](https://angel.co/company/powerloom/jobs) in Bangalore
- Auditors! [Join Trail of Bits](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) and make a career-defining contribution

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-march-21-2021/](https://weekinethereumnews.com/week-in-ethereum-news-march-21-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Mar 25 - [Gitcoin CLR matching grants](https://gitcoin.co/grants/) round ends (ahem: [Week in Eth News](https://gitcoin.co/grants/237/week-in-ethereum-news))
- **Mar 27 - Ethstaker’s [“learn to stake” workshop](https://ethstaker.cc/ethereum-2-0-validator-workshop-2/)**
- Apr 9 - May 14 - ETHGlobal’s [Scaling Ethereum](https://scaling.ethglobal.co/) hackathon
- April 14 - [Berlin upgrade fork](https://github.com/ethereum/pm/issues/248#issuecomment-782069875) (testnets: Ropsten Mar 10, Goerli Mar 17, Rinkeby Mar 24)
- April 16 - [Rollup community grant](https://esp.ethereum.foundation/en/rollup-grants/) applications due
- **April 20 - deadline for [beacon chain security and testing RFP](https://notes.ethereum.org/@lsankar/security-rfp)**
- April 22 - [Ethereum in the Enterprise 2021](https://www.conference2021.entethalliance.org/)
- May 14 - papers due for [WoSCA 2021](https://trailofbits.github.io/WoSCA/)
- Jul 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

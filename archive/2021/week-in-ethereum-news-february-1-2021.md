---
title: "Week in Ethereum News <BR> Feb 1, 2021"
date: "2021-02-01"
---

## **Eth News and Links**

**Eth1**

- [Persistent txpool proposal](https://gist.github.com/karalabe/821a1cd0270984a4198e904d34623b6c)
- Proposed revamp of [stateless Eth roadmap](https://ethresear.ch/t/complete-revamp-of-the-stateless-ethereum-roadmap/8592); focus on the clients, need client specifically focused on stateless?
- [Alternative bounded-state-friendly address scheme](https://ethresear.ch/t/alternative-bounded-state-friendly-address-scheme/8602) with CREATE3 and epoch prefix
- [Reforming core devs call](https://hackmd.io/@timbeiko/acd-feedback) discussion doc

**EIPs/Standards**

- [EIP3238](https://github.com/ethereum/EIPs/blob/ca510acf968eb20a3b62d9fc26479c8ea9b9b41a/EIPS/eip-3238.md): delay difficulty bomb 12 months
- [ERC3224](https://github.com/ethereum/EIPs/blob/b92a65e0473f4c1e9118c74ed069c1040721bc4e/EIPS/eip-3224.md): human readable transaction technique standard for app devs

**Eth2**

- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210129), includes graphic from Leo Bago’s client node count
- Proposal for [first upgrade of Eth’s proof of stake chain](https://notes.ethereum.org/@vbuterin/HF1_proposal): light client support, spread processing over the epoch, fork choice hardening, increase slashing/inactivity penalties as planned. Cap validators at 524k?
- Latest [eth2 call](https://youtu.be/_WK3k_k-4w8?t=336). Notes from [Ben](https://hackmd.io/@benjaminion/H1FdGQxlx) and [Alex](https://twitter.com/ralexstokes/status/1354806080207917065), get ready for [Feb 2 workshops](https://twitter.com/icebearhww/status/1355577160308690945)

**Layer2**

- Arbitrum releases [testnet with lots of apps](https://offchain.medium.com/arbitrum-rollout-demo-defi-ecosystem-built-on-arbitrums-layer-2-testnet-e3bee7df1fc3).
- A guide to [optimistic rollups](https://research.paradigm.xyz/rollups) and to [Optimism](https://research.paradigm.xyz/optimism) in particular
- [Hop cross-rollup](https://ethresear.ch/t/hop-send-tokens-across-rollups/8581) token bridge
- Cartesi with a [TrueBit-style verification/fraud proof game](https://medium.com/cartesi/scalable-smart-contracts-on-ethereum-built-with-mainstream-software-stacks-8ad6f8f17997) for RISC-V Linux
- Aztec and Starkware release [Polaris prover license](https://medium.com/aztec-protocol/introducing-polaris-d4eb0c9da1b4) for rollup code
- The road to [StarkNet](https://medium.com/starkware/on-the-road-to-starknet-a-permissionless-stark-powered-l2-zk-rollup-83be53640880), a zk-rollup from StarkWare coming end of 2021 with apps written in [Cairo](https://www.cairo-lang.org/playground/)

* * *

### **This newsletter is made possible thanks to [Matcha](https://matcha.xyz/?id=wien) by [0x](https://0x.org/)!**

![Matcha](https://weekinethereumnews.com/wp-content/uploads/2020/06/matcha-avatar.png)

Matcha aggregates liquidity across decentralized exchange networks to offer you the best price on every token swap on both spot **and limit orders**!

Now you can [trade 1000+ DeFi tokens](https://matcha.xyz/?id=wien) on Matcha!

* * *

**Stuff for developers**

- Solidity [v0.8.1](https://blog.soliditylang.org/2021/01/27/solidity-0.8.1-release-announcement/), SMTChecker supports external calls
- [Solidity developer survey](https://blog.soliditylang.org/2021/01/26/solidity-developer-survey-2020-results/) results. Now launches [Solidity Discourse forum](https://blog.soliditylang.org/2021/02/01/launching-the-solidity-forum/)
- PWC: changes in [Solidity v0.8.x that you may have missed](https://www.pwc.ch/en/insights/digital/change-in-080-solidity-compiler.html)
- [Paradigm CTF](https://twitter.com/paradigm_ctf/status/1353786644361523203) starts Feb 5
- OpenZeppelin’s [Hardhat/Truffle upgrades plugin](https://forum.openzeppelin.com/t/upgrades-with-peace-of-mind-structs-edition/5526) now supports structs and enums
- Austin Griffith’s scaffold-eth challenge/tutorial: [build staking app](https://github.com/austintgriffith/scaffold-eth/blob/challenge-1-decentralized-staking/README.md)
- [Flash loan arb bot with Infura](https://blog.infura.io/build-a-flash-loan-arbitrage-bot-on-infura-part-i/) tutorial
- hevm [v0.44](https://github.com/dapphub/dapptools/releases/tag/hevm%2F0.44.0), accepts solidity json output built via `--standard-json`
- [Benchmarking pairing-friendly elliptic curves libraries](https://hackmd.io/@zkteam/eccbench)
- Iden3’s [rapidSNARK](https://github.com/iden3/rapidsnark), a fast prover written in C++ for circom and snarkjs

**Security/incidents**

- [Typhoon.cash vulnerabilities](https://avner1122.medium.com/typhoon-cash-vulnerabilities-e82b0faa54b6)
- Secureum analyzes [Hermez’s audits](https://secureum.substack.com/p/making-hermez-safu-secureum-4)

**Ecosystem**

- [Reddit announces partnership with EF](https://www.reddit.com/r/ethereum/comments/l6c3kx/reddit_announces_partnership_with_the_ethereum/) to get Ethereum to Reddit-scale production
- [Devcon Bogotá is postponed](https://blog.ethereum.org/2021/01/26/the-longer-road-to-devcon/), EthCC now planned for July

**Enterprise**

- [USAA and State Farm will go into production](https://newsroom.statefarm.com/blockchain-solution-solves-state-farm-usaa-subrogation-challenge/) with their [Quorum based solution](https://weekinethereumnews.com/june-1-2019/) to track and pay each other for auto claims
- China’s [Blockchain-based Service Network will now have Quorum](https://consensys.net/blog/press-release/consensys-announces-partnership-with-chinas-blockchain-services-network/) available
- Visa CEO says on earnings call they’re looking at [supporting stablecoin on/offramps](https://www.fool.com/earnings/call-transcripts/2021/01/28/visa-v-q1-2021-earnings-call-transcript/) for Visa cards, hence why they’ve been [hiring Eth devs](https://www.coindesk.com/visa-hiring-ethereum-developer-for-new-distributed-application)

**Application layer**

- [xINCH](https://medium.com/xtoken/introducing-xinch-powerful-yield-f37c18724810): an auto-claim and compound wrapper for 1Inch staking
- UMA: [borrow USDC with your ETH for free](https://medium.com/uma-project/ulabs-notes-borrow-usdc-with-your-eth-for-free-ab687991728f) (or at negative interest!)
- Opium is offering [tranched CDOs](https://medium.com/opium-network/introducing-risk-tranching-to-defi-cdai-fixed-vs-turbo-return-50028fde8811) built on Compound. Senior tranche is fixed rate, junior tranche is high risk/reward
- [Spendless](https://spendless.io/blog/2021/01/27/spendless-explainer) - direct your stablecoin interest to charity or save via yearn frontend
- An alternative Zora frontend: [zora.gallery](https://twitter.com/_anishagnihotri/status/1355098515052109827)
- [$essay](https://j.mirror.xyz/uVGCCwwm3k341lPpxaJmHTZROESVse9Pe_rmbiuUAC0) tokenized crowdfunding for an essay where the holders get 10% of future trades
- Atari creating a [classic Atari games arcade](https://decentraland.org/blog/announcements/dcl-x-atari/) in Decentraland
- Mark Cuban is [minting NFTs](https://blogmaverick.com/2021/01/31/the-store-of-value-generation-is-kicking-your-ass-and-you-dont-even-know-it/)

**Regulation/business/tokens**

- Coinbase to [go public via direct listing](https://blog.coinbase.com/coinbase-announces-proposed-direct-listing-3a52c4298ccc) selling shares directly, no underwritten IPO process
- Fincen [reopens comment period](https://www.fincen.gov/news/news-releases/fincen-extends-reopened-comment-period-proposed-rulemaking-certain-convertible), if you want to comment on Mnuchin’s anti-crypto regulations. It ends today for reporting counterparty info, and on March 1 for the rest
- Brukhman: [appraisal games and NFT pricing/liquidity](https://blog.coinfund.io/appraisal-games-and-the-nft-liquidity-problem-904afe6bc7af)
- Dune Analytics: the [real-time quarterly report](https://duneanalytics.com/blog/revolution-not-quarterly)
- pNetwork offers [wrapped DOGE on Ethereum](https://twitter.com/pNetworkDeFi/status/1347670661796388865)

**General**

- [What happens if you reuse a nonce in cryptography](https://github.com/christianlundkvist/blog/blob/master/2021_01_25_nonce_reuse_in_encryption/nonce_reuse_in_encryption.md)? Bad stuff.
- [How SNARKs are possible](https://vitalik.ca/general/2021/01/26/snarks.html) with polynomial commitments
- The state of tooling for [verifying constant-timeness of cryptographic implementations](https://neuromancer.sk/article/26)
- What [miner revolts are really possible](https://micah-zoltu.medium.com/what-does-a-miner-revolt-look-like-a99216fe270e) anyway?
- Google says [North Korea is trying to hack security researchers](https://blog.google/threat-analysis-group/new-campaign-targeting-security-researchers/)
- Important ASAP security updates: if you’re an iPhone user, [update iOS](https://support.apple.com/en-us/HT212146). If you run Linux, [update sudo](https://nvd.nist.gov/vuln/detail/CVE-2021-3156)

* * *

## **Job Listings**

- MetaMask is hiring engineers for a variety of positions. Apply [here](https://consensys.net/open-roles/2572388/).
- [Cartesi](https://cartesi.io/), a rollups solution, [is looking to hire skilled engineers](https://angel.co/company/cartesi/jobs)
- Trail of Bits is looking for a [technical editor/writer](https://jobs.lever.co/trailofbits/8bf936ff-b86c-462e-80b2-4d58004bc68d) & [security engineer](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf)
- 0x looking for [devs of all types](https://0x.org/about/jobs) and a [data analyst](https://boards.greenhouse.io/0x/jobs/4220949002)
- Reddit: [Senior backend/Ethereum engineer](https://boards.greenhouse.io/reddit/jobs/2419120)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-feb-1-2021/](https://weekinethereumnews.com/week-in-ethereum-news-feb-1-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **Feb 2 - [Eth2 sharding and merge workshops](https://hackmd.io/@hww/workshop_feb_2021)**
- Feb 5 - [Nimbus Grafana challenge](https://our.status.im/nimbus-grafana-challenge/) submissions deadline (prizes up to $5k)
- Feb 5-12 - [EthDenver](https://www.ethdenver.com/) (virtual)
- **Feb 5-7 - [Paradigm CTF](https://twitter.com/paradigm_ctf/status/1353786644361523203)**
- Feb 8 - [CME launches ETH futures](https://www.cmegroup.com/trading/ether-futures.html)
- Mar 5 - Financial Cryptography [DeFi academic workshop](https://fc21.ifca.ai/defi/)
- **[Jul 20-22](https://twitter.com/EthCC/status/1354132445231251457)** - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

---
title: "Week in Ethereum News <br> January 14, 2023"
date: "2023-01-14"
---

## **Eth News and Links**

**Shapella (Shanghai + Capella) upgrade**

- Latest core devs execution [call video](https://youtu.be/Z-0z5-7hGvo?t=15). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/Hkm5x5acj)
    - Discussion of [using gwei](https://notes.ethereum.org/@ralexstokes/withdrawals-in-gwei) and using same formats in EL/CL
    
    - Capella [release candidate spec](https://github.com/ethereum/consensus-specs/releases/tag/v1.3.0-rc.1)

- Why is [Warm Coinbase (gas repricing) being added to Shapella](https://etherworld.co/2023/01/13/how-warm-coinbase-helps-in-gas-cost-reduction/)?

**Cancun + Deneb**

- [KZG Ceremony](https://ceremony.ethereum.org/) is live!
    - ~57 more days in the first general contribution period (currently a long wait)
    
    - ~2500 have already contributed. Only **one contributor** needs to be honest

- Latest 4844 implementer [call video](https://youtu.be/FnKOHR92dXU). Notes from [Terence](https://twitter.com/terencechain/status/1612857882755858435)
    - devnet4 coming up before public testnet

**Layer 1**

- [EF research AMA](https://www.reddit.com/r/ethereum/comments/107cqi8/ama_we_are_ef_research_pt_9_11_january_2023/) is a mustread from start to finish
    - Various topics: the [need for more than just 4844](https://old.reddit.com/r/ethereum/comments/107cqi8/ama_we_are_ef_research_pt_9_11_january_2023/j3lsbja/), technological solutions [thwart attempted censorship](https://old.reddit.com/r/ethereum/comments/107cqi8/ama_we_are_ef_research_pt_9_11_january_2023/j3m2z23/), what is [Ethereum good for anyway?](https://old.reddit.com/r/ethereum/comments/107cqi8/ama_we_are_ef_research_pt_9_11_january_2023/j3lz3iv/), coming to consensus on [roadmap prioritization](https://old.reddit.com/r/ethereum/comments/107cqi8/ama_we_are_ef_research_pt_9_11_january_2023/j3lppce/), minimizing [EVM changes for zkEVM](https://old.reddit.com/r/ethereum/comments/107cqi8/ama_we_are_ef_research_pt_9_11_january_2023/j3t8ab5/), should [Ethereum ossify?](https://old.reddit.com/r/ethereum/comments/107cqi8/ama_we_are_ef_research_pt_9_11_january_2023/j3pqz7i/), [synchronous composability](https://old.reddit.com/r/ethereum/comments/107cqi8/ama_we_are_ef_research_pt_9_11_january_2023/j3uge1d/) across zkrollups and [what is the Robust Incentives Group working on?](https://old.reddit.com/r/ethereum/comments/107cqi8/ama_we_are_ef_research_pt_9_11_january_2023/j3visx8/)

- Lido [benchmarks DVT](https://twitter.com/irina_everstake/status/1612536005135044609) (DVT decentralizes staking pools)

**Client releases**

- Consensus Layer
    - Lighthouse [v3.4](https://github.com/sigp/lighthouse/releases/tag/v3.4.0), high priority release. Proposer boost reorgs should incentivize performance improvements

- Execution layer
    - Erigon [v2.34](https://github.com/ledgerwatch/erigon/releases/tag/v2.34.0), a few releases this week with debug trace improvements, multicore CPU threading and MBDX upgrade

**MEV**

- [Flashbots privacy roast](https://youtu.be/Di5fO99lCPo?t=643)

- Prestwich: the [next 5 years of MEV](https://medium.com/@Prestwich/mev-the-next-five-years-63f84fffdf36)

- [Crazy frontrun](https://twitter.com/bertcmiller/status/1613566397954621442): frontrunner copies exploiter’s 4 previous transactions over 50+ blocks

**Layer 2**

- [Optimism and Arbitrum transactions flip Ethereum mainnet](https://twitter.com/PaoloRebuffo/status/1613800598251646976) transactions

**EIPs/Standards**

- [ERC6150](https://github.com/keeganlee/EIPs/blob/80571ca99550c576c807a5ba50ccf25e27f9f21e/EIPS/eip-6150.md): Hierarchical NFTs

* * *

### **This newsletter is made possible thanks to** [**SpeedRunEthereum.com**](https://speedrunethereum.com/)**!**

[![Speed Run Ethereum](https://substackcdn.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F289fcd14-37a9-4ab8-a961-3ff952692f6f_766x463.png "Speed Run Ethereum")](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F289fcd14-37a9-4ab8-a961-3ff952692f6f_766x463.png)

Test your skills and learn how to build apps on Ethereum at [SpeedRunEthereum.com](https://speedrunethereum.com/).

* * *

**Stuff for developers**

- Hardhat and Foundry plugin [v1](https://github.com/NomicFoundation/hardhat/releases/tag/%40nomicfoundation/hardhat-foundry%401.0.0)

- Foundry toolchain now [caches RPC calls in CI flows](https://github.com/foundry-rs/foundry-toolchain)

- If you've deployed a contract to Mainnet, Goerli, or Sepolia before Nov 15, 2022, you can [claim 10 goerli + 10 sepolia eth](https://grabteeth.xyz/)

- [Chugsplash](https://twitter.com/ChugSplash_io/status/1611598563301007360): tool to deploy and upgrade smart contracts securely

- [Turborepo starter kit](https://github.com/alexallah/ethereum-healthmon): NextJS, WAGMI, Ethers, Tailwind, Hardhat, Typechain

- Paul Berg on solving [stack too deep](https://twitter.com/PaulRBerg/status/1612043506545033218)

- Now over [225 contracts to fork and easily deploy](https://www.cookbook.dev/) on Cookbook.dev

- [Node health monitoring](https://github.com/alexallah/ethereum-healthmon) tool

**Security**

- [Damn Vulnerable Defi v3](https://www.damnvulnerabledefi.xyz/v3-release/)

- slither [v0.9.2](https://github.com/crytic/slither/releases/tag/0.9.2), 2 new detectors, integrates OpenAI’s codex to generate natspec and find bugs with GPT3

- Beware of [Multi-block MEV and Compound Governor](https://ease.org/most-governance-contracts-have-an-upcoming-vulnerability-we-should-all-pay-attention-to/)

- [2022 in Ethereum security](https://ventral.digital/posts/2022/12/15/ethereum-smart-contract-auditors-2022-rewind) review

**Ecosystem**

- [DAOdrops](https://twitter.com/dao_drops/status/1613617869375344647): 250k USDC retroactive goods funding to be distributed via vote by 1) DAO voters, 2) POAP holders, 3) code deployers. Nominations open now.

- [Randomness on Ethereum](https://www.paradigm.xyz/2023/01/eth-rng) using SNARKs and VDFs

- Proof of concept to use [Nym to anonymize RPC calls](https://github.com/EdenBlockVC/spook)

- [PeltaShield](https://pelta.tech/quick-setup.html): tool to simulate your transactions via RPC call

**Enterprise**

- Norwegian government using Arbitrum to [maintain cap tables of unlisted companies](https://medium.com/blockchangers/how-norway-is-using-ethereum-arbitrum-for-shareholder-management-500e59c586d3)

- [Société Générale withdraws 7 million Dai](https://www.theblock.co/post/201972/investment-firm-societe-generale-mints-7-million-in-stablecoin-loan-from-makerdao) of its 30m Dai authorization backed by home loan bonds

**Application layer**

- [Zkitter](https://mirror.xyz/privacy-scaling-explorations.eth/P4jDH1gLrVQ-DP5VyIKQrlPAJUTDhtXZkFl2vp8ewSg): post under your username or anon, public key written to Arbitrum for account recovery. Uses various zk tools: Interep, RLN, Semaphore

- [chai.money](https://chai.money/) back online to accrue the DSR on your Dai (currently 1%)

- Get the risk-free rate onchain? [Ondo](https://blog.ondo.finance/announcing-tokenized-us-treasuries-and-bonds/) to tokenize 3 different ETFs of US treasuries/bonds and will [fork Compound](https://blog.fluxfinance.com/announcing-flux-finance-defi-meets-real-world-assets/) for its security tokens

- Revamped [Gitcoin Grants alpha](https://go.gitcoin.co/blog/announcing-the-gitcoin-alpha-round) round launches next week with open source, Eth infra and climate solutions matching pools

- [Ethunwrapp](https://ethunwr.app/): retrospective of your onchain activity in 2022

* * *

### Job Listings

- Arx, creators of KONG Cash and HaLo tags is hiring a [Solidity developer](https://arx.org/jobs).

- [Status](https://status.im/) is hiring a [Technical Writer for Waku Product](https://grnh.se/41bd7e051us), [all other jobs here](https://grnh.se/9fc6e6fc1us)

- Join a16z-backed Story Protocol as a founding [smart contract developer](https://jobs.lever.co/storyprotocol/e08066d4-8d73-46ab-975c-dd5a284e1a83).

- [Lighthouse seeking support tech](https://old.reddit.com/r/ethstaker/comments/1076qqr/lighthouse_is_looking_for_a_support_technician/) to help its stakers

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Wyre [saved](https://twitter.com/sendwyre/status/1613673423032418306) and processing withdrawals normally

- [Gemini accuses Genesis of fraud](https://twitter.com/cameron/status/1612806661508567042)

- SEC [charges Gemini and Genesis](https://www.sec.gov/news/press-release/2023-7) calling GeminiEarn a security

- [Nexo raided](https://archive.ph/GPWUY) by Bulgarian police

- [Treasury dodges Emmer inquiry](https://twitter.com/RepTomEmmer/status/1612862784512954383) over Tornado sanctions

- [Metropolitan drops crypto.com](https://www.businesswire.com/news/home/20230109005186/en/) and all other crypto clients

**General/crypto**

- [Benchmarking RISC Zero and Polygon Miden](https://delendum.xyz/2023/01/11/zk-system-benchmarking.html)

- A [primer on pairings](https://alinush.github.io/2022/12/31/pairings-or-bilinear-maps.html)

- [S𝛑PETs](https://ethresear.ch/t/s-pets-sustainable-practically-indistinguishable-privacy-enhanced-transactions/14565): private transactions using ECDSA or Schnorr

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

[Permalink for this week’s issue](https://weekinethereumnews.com/week-in-ethereum-news-january-14-2023-thanks-to-speedrunethereum-com-for-making-this-issue-possible/)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jan 17-31 – [Gitcoin grants round](https://go.gitcoin.co/blog/announcing-the-gitcoin-alpha-tests)

- Jan 31 – [KZG ceremony grants](https://blog.ethereum.org/2022/12/15/kzg-ceremony-grants-round) deadline

- **Jan 31 – deadline to nominate for** [**Optimism retroactive public goods round 2**](https://community.optimism.io/docs/governance/retropgf-2/#scope-of-retropgf-2)

- Feb 24 - Mar 1 – [ETHDenver BUIDLWeek](https://www.ethdenver.com/)

- **Feb 3 – deadline to nominate for** [**DAOdrops**](https://daodrops.io/) **retroactive public goods funding**

- Mar 2-5 – [ETHDenver Hackathon](https://www.ethdenver.com/)

- Mar 10-29 – [Scaling Ethereum](https://ethglobal.com/events/scaling2023) (ETHGlobal) virtual

- Mar 15-16 – [ETHDubai](https://www.ethdubaiconf.org/)

- Mar 16-18 – [ETH Porto](https://ethporto.org/)

- Mar 28-30 – [Ethereum Rio](https://www.ethereumbrasil.com/ethereumrio)

- Apr 3-6 – [Edcon](https://edcon.io/) Vienna

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- Apr 14-16 – [ETHGlobal Tokyo](https://tokyo.ethglobal.com/)

- Apr 14-16 – [ETHZurich](https://ethereumzuri.ch/) conference

- **Apr 21-23 –** [**EthTaipei**](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) **hackathon**

- **Apr 24-25 –** [**EthTaipei**](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) **conference**

- May 26–28 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Jun 23–25 – [ETHGlobal Toronto](https://ethglobal.com/events/toronto)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–25 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

### [_Sign up_](https://weekinethereum.substack.com/subscribe#about) _for this email list_

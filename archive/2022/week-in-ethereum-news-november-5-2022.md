---
title: "Week in Ethereum News <br> November 5, 2022"
date: "2022-11-05"
---

## **Eth News and Links**

**Layer 1**

- Latest consensus layer [call video](https://www.youtube.com/watch?v=GWkhFCvwOT4&t=68s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/SkCPPHZHs) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-consensus-layer-call-97/):
    - Full & partial withdrawals to be processed in a single queue-less pipeline
    - EIP4844 (proto-danksharding) to be developed on top of withdrawals
    - Block value to be added to EngineAPI to allow comparing MEV-Boost vs locally built blocks
    - MEV-Boost [update](https://collective.flashbots.net/t/mev-boost-status-update-2022-11-03/695)
- MEV-Boost:
    - [Analysis of MEV-Boost blocks](https://twitter.com/blocknative/status/1587948088445935617): private transactions (non-public mempool) are 3.8% of MEV-Boost blocks
    - [Censorship resistance](https://stonecoldpat.substack.com/p/mev-boost): define & measure censorship, use collective enforcement (e.g. crLists) and prepare User Activated Soft Fork to force exit & penalize censoring validators
    - [Flashbots builder needs to charge a fee](https://mirror.xyz/sajz.sismo.eth/WK26Itw23TFa3tsncYjarpfjHvqEJfPul0bgDPMyYd8) to increase diversity
    - [Bulk data export](https://collective.flashbots.net/t/flashbots-relay-bulk-data-exports-payloads-and-builder-submissions/700) for Flashbots relay
- [Inclusion.watch](https://www.inclusion.watch/): 79% probability of Tornado transactions being included in a block within a minute

**For stakers**

- Pintail: analysis of [validator returns](https://pintail.xyz/posts/since-the-merge/): third party block builders are the majority and outperform validators who build their own blocks
- Guide to [migrate validator keys between two machines](https://ethstaker.gitbook.io/ethstaker-knowledge-base/tutorials/validator-key-migration)
- [Proposal for stakers testnet](https://notes.ethereum.org/@mario-havel/stakers-testnet): ephemeral testnet dedicated for testing staking setups

**Research**

- [Verkle Tree retrieval](https://twitter.com/giuliorebuffo/status/1586490619236597760) using IPFS snapshots proof of concept shows possible offline conversion route for transition to Verkle Trees

**Client releases**

- Execution Layer:
    - Besu [v22.10.0](https://consensys.net/blog/news/besu-22-10-0-quarterly-release-brings-big-improvements-for-performance-resiliency-on-ethereum-mainnet/): fixes and improvements for staking and resilience
    - Erigon [v2.29.0](https://twitter.com/ErigonEth/status/1588554753893621762): logging to files and [upstreamed Otterscan patches](https://twitter.com/wmitsuda/status/1588070711280680960)
    - Geth
        - [latest](https://twitter.com/vdwijden/status/1588133028546625537): improves profitability of local block building
        - [v1.10.26](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.26): snap sync improvements
    - Nethermind [v1.14.5](https://github.com/NethermindEth/nethermind/releases/tag/1.14.5): rollback of v1.14.4 unnecessarily activating snap sync on synced nodes

**Layer 2**

- Vitalik’s proposed [rollup milestones to maturity](https://ethereum-magicians.org/t/proposed-milestones-for-rollups-taking-off-training-wheels/11571): 
    - Stage 0 (full training wheels): on-chain transactions, full rollup node, operator cannot freeze/steal user assets by censoring and no active fraud/validity proof
    - Stage 1 (limited training wheels): running fraud/validity proof with security council override and upgrade timelock greater than fraud proof period
    - Stage 2 (no training wheels): two or more distinct fraud/validity provers, security council can adjudicate if there is a bug & provers disagree and upgrade timelock greater than 30 days

**EIPs/Standards**

- [EIP5850](https://github.com/ethereum/EIPs/pull/5850/files): Complex numbers stored in `bytes32` types
- [EIP5851](https://github.com/ethereum/EIPs/pull/5851/files): Zero-Knowledge KYC certificates
- [EIP5865](https://github.com/ethereum/EIPs/pull/5865/files): NFT avatar
- [EIP5875](https://github.com/ethereum/EIPs/pull/5875/files): Opcode for transaction number

* * *

### **This newsletter is made possible thanks to Starbloom Ventures!**

![Starbloom Ventures](https://weekinethereumnews.com/wp-content/uploads/2021/11/Screenshot-from-2021-11-19-15-25-51.png)

Starbloom Ventures is a first round venture fund founded by Evan Van Ness to invest in the future of web3.

* * *

**Stuff for developers**

- [App devs should use Sepolia testnet](https://twitter.com/lightclients/status/1587914219214999552) rather than Goerli testnet due to Goerli supply issues
- forge-std [v1.0.0](https://twitter.com/msolomon44/status/1587171153918840833) (Foundry test library): `bound` updated with edge biasing, `stdChains` variable,  ERC20/165/721/1155/4626 interfaces, `assumeNoPrecompiles` helper and `vmSafe` interface
- Remix [project site](https://remix-project.org/): online IDE, desktop IDE, VS Code extension, Remixd CLI and plugins
- Paul R Berg's [Solidity tips](https://typefully.com/PaulRBerg/nkgrFkU)
- [Solidity-template](https://github.com/mattstam/solidity-template#readme): Foundry for unit tests & Hardhat for integration tests
- Waffle [v4](https://medium.com/truefieng/waffle-4-is-out-c0754f9c7271) (JavaScript based testing framework): improved matchers and deprecated Jest in favor of Mocha
- Challenges/CTFs
    - EKOparty [CTF challenges](https://www.ctfprotocol.com/tracks/eko2022)
    - Optimizor Club [SQRT challenge](https://github.com/OptimizorClub/sqrt_foundry_template#readme): solutions [1](https://twitter.com/high_byte/status/1587534080945659905) & [2](https://twitter.com/kanewallmann/status/1588127465356300288)
    - RareSkills gas puzzles: [Mint 150 NFTs](https://twitter.com/rareskills_io/status/1585390826943049729) & [ERC165](https://twitter.com/rareskills_io/status/1587927413455192065)
    - Huff (language) [challenges](https://twitter.com/huff_language/status/1586425112135278592)
- OpenZeppelin [merkle-tree](https://github.com/OpenZeppelin/merkle-tree#readme): JavaScript library to generate merkle trees & proofs
- Web3.py [multithreading](https://snakecharmers.ethereum.org/web3-py-patterns-multithreading/) patterns
- [blockies-nft](https://github.com/wighawag/blockies-nft#readme) generated on-chain in Solidity
- ETHGlobal [guides](https://ethglobal.com/guides)

**Security**

- Dappnode [$165k exploit](https://twitter.com/DAppNode/status/1586769313872101376), private key generated using fork of Profanity
- Rubic [$200k exploit](https://twitter.com/CryptoRubic/status/1587704548688367619), admin private key compromised
- BribeV2 [vulnerability disclosed](https://github.com/yearn/yearn-security/blob/master/disclosures/2022-11-01.md), patched in BribeV3 (aka yBribe)

**Ecosystem**

- Vitalik’s [updated roadmap diagram](https://twitter.com/vitalikbuterin/status/1588669782471368704): adds single slot finality as Merge milestone, Verge endgame of fully SNARKed Ethereum and the Scourge transaction inclusion
- Goerli testnet supply issues [discussion](https://github.com/eth-clients/goerli/issues/129#issuecomment-1298896603); proposed [testnet lifecycle](https://ethereum-magicians.org/t/proposal-predictable-ethereum-testnet-lifecycle/11575), launch new testnet every 2 years with lifespan of maximum 5 years
- ETHLisbon hackathon [winners](https://eth-lisbon.notion.site/Winners-0b5e1564d84044718ec6d5be50f6d108) and [list of projects](https://taikai.network/ethlisbon/hackathons/ethlisbon-2022/projects)
- Ethereum.org [learning quizzes](https://twitter.com/ethdotorg/status/1587833328240971777)

**Enterprise**

- [Israel finance ministry](https://news.vmware.com/technologies/vmware-blockchain-ethereum-momentum) piloting issuance of government bonds using VMware
- Visa [FIFA World Cup](https://twitter.com/cuysheffield/status/1587469469844049921) goal generated art NFTs

**Application layer**

- OpenSea [copymint detection system](https://twitter.com/opensea/status/1587194630432497664) and [malicious URL detection & post-theft resale prevention](https://opensea.io/blog/announcements/our-efforts-to-prevent-nft-theft/)
- [Art Gobblers](https://artgobblers.com/) (art factory) live on mainnet
- [Nouns Builder](https://nouns.build/): no code creation of on-chain art DAOs
- Gearbox [v2](https://twitter.com/GearboxProtocol/status/1587184991624208384) (composable leverage) live

* * *

### Job Listings

- Avantgarde Finance seeking [Full Stack Dev in Web3/DeFi](https://apply.workable.com/avantgarde-finance/j/3974DA97B8/) to build on Enzyme
- EF Robust Incentives Group seek a [research scientist](https://jobs.lever.co/ethereumfoundation/cd2382ec-abbd-493b-b942-b5e2a61a6c0a)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- EF are hiring a [code integration tester](https://jobs.lever.co/ethereumfoundation/6feeb8cb-bd05-4f24-9fda-9ba3be98e5a4)

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Vitalik [on regulation](https://twitter.com/vitalikbuterin/status/1586557896351186944)
- Hong Kong government [policy statement](https://www.info.gov.hk/gia/general/202210/31/P2022103000454.htm): risk-based guardrails, public consultation on regulations and pilot green bond tokenisation & e-HKD

**General**

- MakerDAO co-founder [Nikolai Mushegian](https://nikolai.fyi/) found [dead in Puerto Rico](https://twitter.com/OmniCraig/status/1586432239105060864)
- [OpenSSL v3.0](https://www.openssl.org/blog/blog/2022/11/01/email-address-overflows/): two high severity vulnerabilities fixed

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-november-5-2022](https://weekinethereumnews.com/week-in-ethereum-news-november-5-2022)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- **Nov 7 – Clr.fund** [**LatAm round**](https://twitter.com/clrfund/status/1587077979053727746) starts
- Nov 11-13 – [ETHBrno](https://ethbrno.cz/) (Czech Republic)
- Nov 25-27 – [ETH Vietnam](https://www.eth-vietnam.com/)
- Dec 1 – [Columbia cryptoeconomics workshop](https://bit.ly/columbiacryptoeconomics) (New York)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- Dec 5 – [EF Layer 2 grants](https://esp.ethereum.foundation/layer-2-grants) deadline
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

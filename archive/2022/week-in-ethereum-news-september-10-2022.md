---
title: "Week in Ethereum News <br> September 10, 2022"
date: "2022-09-10"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- Countdown to the Merge: TTD predicted September 14 by [Bordel](https://bordel.wtf/) & [797](https://797.io/themerge)
- Reminder: [stakers must run an execution layer client](https://twitter.com/evan_van_ness/status/1567893018451099649)
- Beacon chain [upgraded to Bellatrix](https://twitter.com/terencechain/status/1567115533233049606), 5% drop in participation [almost recovered](https://twitter.com/remy_roy/status/1567539002411999232)
- mainnet-shadow-fork-13 [merged](https://twitter.com/abcoathup/status/1568359386443317248) successfully, last shadow fork before the Merge
- Stay up to date on the [latest bugfix releases](https://blog.ethereum.org/2022/08/24/mainnet-merge-announcement)

**Execution layer**

- Erigon [v2022.09.01-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.09.01): fixes for invalid block production and block snapshot production
- Besu [v22.7.2](https://github.com/hyperledger/besu/releases/tag/22.7.2): fixes & improvements in sync, peering and logging
- Nethermind [v1.14.1](https://github.com/NethermindEth/nethermind/releases/tag/1.14.1): workaround for empty block production, merge edge case fixes and improvements to eth\_syncing & eth\_getProof
- [Shanghai upgrade planning](https://ethereum-magicians.org/t/shanghai-core-eip-consideration/10777): async discussions for candidate EIPs

**Proof of Stake consensus layer**

- PoS implementers [call video](https://www.youtube.com/watch?v=ir-gnBm2GZ4&t=188s). Notes from [Christine Kim](https://www.galaxy.com/research/insights/ethereum-consensus-layer-call-95/):
    - [Kiln testnet](https://blog.ethereum.org/2022/09/09/kiln-shutdown) will be shut down next week
    - Proposal to take a break from core dev & CL calls for ~4 weeks around Devcon
- Lighthouse [strict-fee-recipient flag](https://twitter.com/sigp_io/status/1567688757633232897) prevents block production, remove flag & restart
- Nimbus [v22.9.0](https://github.com/status-im/nimbus-eth2/releases/tag/v22.9.0): fix for pre-TTD block production after restart, improved compatibility with Besu, Prysm & slow block builders and faster block processing on Raspberry Pi
- Prysm [v3.1.1](https://github.com/prysmaticlabs/prysm/releases/tag/v3.1.1): fork choice pruning fix and a gossipsub optimization
- [List of checkpoint sync endpoints](https://github.com/eth-clients/checkpoint-sync-endpoints#readme) for the Beacon chain
- [2% of validators registered](https://boost-relay.flashbots.net/) for Flashbots MEV-Boost relay
- [Predicting staking rewards](https://www.attestant.io/posts/exploring-execution-block-rewards-sep-22/) and [modelling validator MEV returns](https://pintail.xyz/posts/post-merge-mev/)
- [Goldfish](https://www.paradigm.xyz/2022/09/goldfish): proposed provably secure replacement for LMD GHOST fork-choice rule

**Layer 2**

- [Guide to creating a caching contract](https://ethereum.org/en/developers/tutorials/all-you-can-cache/) to reduce costs on layer 2

**EIPs/Standards**

- [EIP5573](https://github.com/ethereum/EIPs/pull/5573/files): Sign-In with Ethereum capabilities
- [EIP5585](https://github.com/ethereum/EIPs/pull/5585/files): ERC721 NFT authorization
- [EIP5593](https://github.com/ethereum/EIPs/pull/5593/files): Restrict web3 provider object API injection
- [EIP5604](https://eips.ethereum.org/EIPS/eip-5604): NFT Lien
- [EIP5606](https://github.com/ethereum/EIPs/pull/5606/files): Proxy NFTs
- [EIP5615](https://github.com/ethereum/EIPs/pull/5615/files): ERC1155 supply extension
- [EIP5625](https://github.com/ethereum/EIPs/pull/5625/files): NFT Metadata JSON schema dStorage extension

* * *

### **This newsletter is made possible thanks to** [**Nexus Mutual**](https://nexusmutual.io/)**!**

![Nexus Mutual Protocol Cover](https://weekinethereumnews.com/wp-content/uploads/2022/03/Nexus-Mutual-Protocol-Cover-1024x586.png)

The yield is still out there.  When you discover the next opportunity make sure you don’t get rekt. 

Protect yourself against: 

- hacks with Protocol Cover 
- depegging with Yield Token Cover
- CeFi blow-ups with Custody Cover 

Maximize yield. Minimize Risk. Enjoy peace of mind knowing Nexus Mutual has you covered. Become a member and [protect your assets](https://app.nexusmutual.io/cover) against the major risks in crypto.

* * *

**Stuff for developers**

- Solidity [v0.8.17](https://blog.soliditylang.org/2022/09/08/solidity-0.8.17-release-announcement/): fixes [storage write removal bug](https://blog.soliditylang.org/2022/09/08/storage-write-removal-before-conditional-termination/), more efficient overflow checks for multiplication and language server analyzes all files by default
- [Solidity versions](https://twitter.com/bantg/status/1566075249959079937) and [EVM opcodes](https://twitter.com/bantg/status/1566348908405587969) ordered by usage on mainnet
- EthereumJS [releases](https://twitter.com/efjavascript/status/1567150203047739394): native JavaScript BigInts, Merge is default hard fork, integrated Noble crypto libraries, Trie pruning and a pure non-overhead EVM
- Foundry: [JSON parsing](https://twitter.com/odysseas_eth/status/1566421675633266688), [formatting](https://twitter.com/gakonst/status/1566627137502584832), pattern for [private keys in deploy scripts](https://twitter.com/msolomon44/status/1567204143689011200) and [patched 0-day](https://twitter.com/elyx0/status/1568258205309878272)
- [ethers.js update](https://blog.ricmoo.com/highlights-ethers-js-september-2022-d7bda0fc37ed): v6 branch, support for safe & finalized tags, unicode for ENS fixed and action rejected error code
- Ape [v0.5.0](https://github.com/ApeWorX/ape/releases/tag/v0.5.0) (Python contract framework): automated Etherscan verification, transaction return values and query properties of blocks & events
- [fasteth](https://github.com/Alcibiades-Capital/fasteth#readme): async Python library for Ethereum JSON RPC
- [Gradual Ownership Optimization](https://www.paradigm.xyz/2022/09/goo) (GOO): issue fungible tokens from an NFT and incentivize users to hold both tokens in proportion
- [Cloud-ZK](https://medium.com/@ingonyama/cloud-zk-a-toolkit-for-developing-zkp-acceleration-in-the-cloud-3d670c09c6ed): toolkit for zk-proofs using FPGAs in AWS cloud
- Secureum A-MAZE-X [CTF challenges](https://github.com/secureum/DeFi-Security-Summit-Stanford#readme) and [solutions](https://ventral.digital/posts/2022/8/27/secureum-a-maze-x-stanford-ctf)

**Security**

- Wyvern Protocol (p2p exchange protocol) [memory overwrite vulnerability](https://blocksecteam.medium.com/a-new-memory-overwrite-vulnerability-discovered-in-wyvern-protocol-5285996c297d) disclosed
- Primitive [$34k math approximation error](https://twitter.com/MevRefund/status/1568216188630736897), 0.05 ETH could be swapped for 1700 USDC every 30 minutes
- Trail of Bits guidelines & best practices to [build secure contracts](https://github.com/crytic/building-secure-contracts#readme)
- [Analysis of BGP hijacking attack](https://blog.coinbase.com/celer-bridge-incident-analysis-895a9fc77e57) targeting Celer on August 17

**Ecosystem**

- **Warning**: [you will lose money from replay attacks](https://forum.makerdao.com/t/pecu-announcement-maker-protocol-the-merge-and-future-forks-of-ethereum/17789) if you interact with any PoW fork and don’t know what you are doing
- Stateful Works [Merge manual](https://stateful.mirror.xyz/mYXVnZ_0mP0eTtKMb1-NJqo3a8cRXGMySfk_0ep_Oeg): perspectives from 60+ core contributors
- [EF grantees](https://blog.ethereum.org/2022/09/07/esp-q1-q2-allocation-update) were allocated $17.6 million in Q1 & Q2
- samczsun’s [Ethereum Tags Database](https://tags.eth.samczsun.com/): tag & label addresses

**Enterprise**

- [NBA partners with Sorare](https://www.nba.com/news/nba-nbpa-sorare-fantasy-game-release) for upcoming NFT fantasy basketball game

**Application layer**

- [Compound v2 cETH market restored](https://twitter.com/compoundfinance/status/1567323147967336448) after reverting to old price oracle
- [Coinbase proposal](https://forum.makerdao.com/t/mip81-coinbase-usdc-institutional-rewards/17703) to custody USDC from Maker and pay interest
- Uniswap [Just in Time liquidity research](https://uniswap.org/blog/jit-liquidity)
- Vitalik’s ideas for [ENS demand-based recurring fees](https://vitalik.eth.limo/general/2022/09/09/ens.html) and [Nick’s response](https://mirror.xyz/nick.eth/EAH91vsu24WlvIqs3os-ISEpgnqIic0Y3z_asUVtGy4)
- [True Names (ENS) suing GoDaddy](https://www.coindesk.com/policy/2022/09/08/firm-behind-ethereum-name-service-and-virgil-griffith-sue-godaddy-over-sale-of-ethlink/) to recover eth.link
- Idea for [permissioned privacy pools](https://ethresear.ch/t/permissioned-privacy-pools/13572) to fund fresh addresses using allowlists & blocklists
- [MoonCats](https://twitter.com/jakegallen_/status/1567230230955442178) separating from Ponderware, transitioning to side project
- Jonathan Mann’s [5000th song](https://twitter.com/songadaymann/status/1568240969501351936)
- [Gitcoin Grants using sybil-resistant stamps](https://gitcoin.co/blog/wtf-is-trust-bonus/) on Ceramic network to compute trust bonus

* * *

### **Job Listings**

- Multichain oracle: [Technical content writer](https://bobhub.gitbook.io/bobhub/)
- EF’s Privacy & Scaling Explorations team: [Web3 Engineer](https://jobs.lever.co/ethereumfoundation/ece6534a-b946-4996-b7e7-713bd1ec0353?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- ØVIX + GOGO Protocol: [Senior DeFi Blockchain Developer](https://join.com/companies/cryptogogos/5585820-blockchain-developer-at-crypto-start-up?utm_source=ETHnewsletter&utm_medium=email&utm_campaign=WeekInEthNews)

**Job listings: $600** for four issues (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Lawsuit [challenging US Treasury’s Tornado Cash sanctions](https://blog.coinbase.com/defending-privacy-in-crypto-e09db33dece8), funded by Coinbase
- US bankruptcy filing [argues Celsius was insolvent in 2020](https://cases.stretto.com/public/x191/11749/PLEADINGS/1174909072280000000015.pdf) \[PDF\]

**General**

- [Google countdown to the Merge](https://www.google.com/search?q=ethereum+merge) with bears
- Flashbots Research: [First Come First Served (FCFS)-based ordering of transactions](https://writings.flashbots.net/research/fcfs-and-front-running/) mitigates front-running to an extent but can’t prevent it
- [US IRS data leak](https://www.bleepingcomputer.com/news/security/irs-data-leak-exposes-personal-info-of-120-000-taxpayers/) exposed 120k tax payers personal info

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-10-2022](https://weekinethereumnews.com/week-in-ethereum-news-september-10-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Sep ~15 – [the Merge](https://blog.ethereum.org/2022/08/24/mainnet-merge-announcement/) (TTD: 58750000000000000000000); [**live stream**](https://ethstaker.cc/the-official-ethereum-merge-livestream/)
- Sep 16 – [Ethereum Protocol Fellowship](https://blog.ethereum.org/2022/09/01/ethereum-protocol-fellowship-third) applications close
- Sep 16-18 - [EthBerlin](https://ethberlin.ooo/)
- Sep 22 – [Gitcoin Grants round 15](https://twitter.com/gitcoin/status/1558498622949523456) ends **(support** [**Week in Eth News**](https://gitcoin.co/grants/2785/week-in-ethereum-news)**)**
- Sep 23 - [ETH HCMC](https://2022.ethhcmc.com/) summit (Ho Chi Minh)
- Sep 23-24 - [ETHSantiago](https://ethsantiago.com/)
- **Oct 6-8 –** [**Web3 Lagos**](https://event.web3bridge.com/)
- Oct 7-16 – [Devcon week](https://devcon.org/en/devcon-week/) (Bogotá)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- Oct 7-9 – [Infinite hackathon](https://infinite-hackathons.eth.limo/) (Bogotá)
- Oct 11-14 – [Devcon 6](https://devcon.org/) (Bogotá)
- Oct 18-23 – [Eth Medellin](https://www.ethmedellin.co/) (Colombia)
- Oct 26-28 – [Eth Panama](https://twitter.com/EthPanama)
- Oct 28-30 – [ETH Lisbon](https://www.ethlisbon.org/)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 11-13 – [ETHBrno](https://mirror.xyz/ethbrno.eth/6BH9cUVuD85hy5O0L5cOOOE7niSA9Yo5eWsXVzKOlO4) (Czech Republic)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- **Nov 25-27 –** [**ETH Vietnam**](https://www.eth-vietnam.com/)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

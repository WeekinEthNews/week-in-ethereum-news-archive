---
title: "Week in Ethereum News <br> December 4, 2021"
date: "2021-12-04"
---

## **Eth News and Links**

**Mainnet execution layer**

- **Update your nodes for [Arrow Glacier](https://ethernodes.org/arrow_glacier) upgrade**
- Tim Beiko’s [core devs update](https://tim.mirror.xyz/3pbg3_DnCqF10FGp28yURGqKaobGX5zDP3oRcKGBSyA):
    - Kintsugi on devnet-2, long lived devnet planned for mid December
    - Deep dive into EIP4488 to make rollups cheaper by reducing calldata costs
- Erigon [v2021.12.01](https://github.com/ledgerwatch/erigon/releases/tag/v2021.12.01): transaction pool price bump enabled, consistent with Geth, bump priority fee & max fee by 10%+ to replace transaction
- Nethermind [v1.12.1](https://github.com/NethermindEth/nethermind/releases/tag/1.12.1): hotfix for CLI & HealthChecksUI issues after .NET 6 upgrade
- EIP4488 [1MB block calldata limit analysis](https://twitter.com/nicksdjohnson/status/1465104492769079297), 67 blocks have exceeded the proposed limit, 65 of 67 were from StarkWare experiment
- [Verkle tree structure](https://blog.ethereum.org/2021/12/02/verkle-tree-structure/) explainer, shallower trees and smaller proofs
- [Impact of address space compression](https://ethresear.ch/t/what-would-break-if-we-lose-address-collision-resistance/11356) proposal (20 byte address: 4 byte prefix, 2 byte period & 14 byte hash), loses address collision resistance

**EIPs/Standards**

- [EIP4511](https://github.com/ethereum/EIPs/blob/d7b569fcea5fa2defa2325c7df568ddb8818afb1/EIPS/eip-4511.md): Execute Past Semantic Abort
- [EIP4512](https://github.com/ethereum/EIPs/blob/5534381c42df4814e29720fd100681147f5b1aec/EIPS/eip-4512.md): Non-Fungible Token with usage rights
- [EIP4519](https://github.com/ethereum/EIPs/blob/570bfe5efc0dc00988c3141888c2ec21fa737f2f/EIPS/eip-4519.md): SmartNFT

**Proof of Stake consensus layer**

- [Help test](https://hackmd.io/WKpg6SNzQbi1jVKNgrSgWg) PoW switch off in the weekly devnets
- Beacon chain [first birthday](https://twitter.com/terencechain/status/1465941243850944516), 263k validators, $40 billion staked
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_211203):
    - Ben’s [annotated spec](https://upgrading-ethereum.info/altair/annotated-spec) updated for Altair
    - Work in progress [Upgrading Ethereum book](https://upgrading-ethereum.info/altair/)
- PoS [implementers call](https://www.youtube.com/watch?v=1fIg_t6hZ8U&t=77s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/S1trJ8UFK): 5 consensus clients working with Geth to follow chain on Kintsugi devnet-2
- Kintsugi spec [v3](https://hackmd.io/@n0ble/kintsugi-spec)
- Prysm [v2.0.4](https://github.com/prysmaticlabs/prysm/releases/tag/v2.0.4): fix to alleviate bandwidth usage
- Lido (staking pool) [node and validator metrics report](https://drive.google.com/file/d/1M9bOFalecnJf_pcYoxO7fWN4P1IH8PZ0/view) \[PDF\]: 38% Prysm vs 59% network-wide average
- [Flashbots PoS working group](https://medium.com/flashbots/announcing-the-flashbots-eth2-working-group-599b2b92634b) for development & adoption of an MEV solution post PoW switch off

**Layer2**

- [StarkNet Alpha](https://medium.com/starkware/starknet-alpha-now-on-mainnet-4cf35efd1669) live on mainnet, supports general computation & composability, no transaction fees until fee mechanism introduced
- [Discussion on resolving StarkNet DDoS vector](https://community.starknet.io/t/management-of-reverted-transactions-in-starknet/136): reverted transactions aren’t included and hence don’t pay fees
- [zkSync fiat onramp](https://twitter.com/zksync/status/1466483774280065032) via Ramp, just in time for Gitcoin grants round 12
- [ZKOPRU](https://medium.com/privacy-scaling-explorations/zkopru-on-testnet-ba5b2d65ffa1): optimistic rollup using zk proofs to make transfers private, live on testnet

* * *

### **This newsletter is made possible thanks to [NEAR](https://near.org/)!**

![NEAR](https://weekinethereumnews.com/wp-content/uploads/2021/10/near_logo_stack.jpg)

NEAR has [launched Simple Nightshade sharding](https://near.org/blog/near-launches-nightshade-sharding-paving-the-way-for-mass-adoption/) to pave the way for greater throughput as NEAR reached [50 million transactions](https://twitter.com/NEARProtocol/status/1465643042803572737) this week!

Simple Nightshade has four different state shards.  For devs and users, it’s important to note that NEAR treats cross-contract calls the same regardless of whether two contracts are on the same shard.

Early in 2022, [phase 1 will introduce chunk-only producers](https://near.org/decentralize/), who only validate one shard and allow for further decentralization via more validators.  Full Nightshade is scheduled for q3 2022 and will feature full sharding of both state and processing.

Learn more about what’s going on in NEAR in the community-driven [NEARweek](https://nearweek.com/) newsletter.

* * *

**Stuff for developers**

- Tim Beiko’s [impact of PoW switch off](https://blog.ethereum.org/2021/11/29/how-the-merge-impacts-app-layer/) on application layer: 
    - Mining & ommer block fields set to zero equivalent
    - BLOCKHASH opcode changes to weaker pseudorandomness, DIFFICULTY opcode renamed RANDOM
    - Block time in PoS is every 12 seconds except when a slot is missed (<1% of the time)
    - Safe head block expected to be in canonical chain, finalized block has been accepted as canonical by >2/3 of validators
- Ethers.js [v5.5.2](https://github.com/ethers-io/ethers.js/releases/tag/v5.5.2): adds Arbitrum & Optimism to networks/providers
- [Hardhat VSCode extension](https://twitter.com/HardhatHQ/status/1465408316365053955) signup for private beta
- Vyper [v0.3.1](https://github.com/vyperlang/vyper/releases/tag/v0.3.1): immutable variables, uint8 type, checkable raw\_call
- Fe [v0.11.0](https://github.com/ethereum/fe/releases/tag/v0.11.0-alpha) alpha, Rust like modules, functions on structs, clearer array syntax
- [evm-codes](https://tairasim.com/evm-codes/): interactive reference to EVM opcodes, includes gas costs, examples and playground
- [Using SMTChecker](https://fv.ethereum.org/2021/12/01/smtchecker-dapptools/) formal verification module in Solidity compiler with  Remix & Dapptools
- Slither used to detect [missing withdrawal functionality](https://twitter.com/popular_12345/status/1465466147315220481) in Wizard & Dragons contract
- [Send message](https://twitter.com/henrilieutaud/status/1466324729829154822) from StarkNet Alpha to mainnet
- [keccak256-circom](https://github.com/vocdoni/keccak256-circom): experimental implementation of Keccak256 hash function in circom circuit
- [Monero Ethereum atomic swap](https://github.com/noot/atomic-swap) work in progress prototype
- [Ephemeral networks](https://ethereum-magicians.org/t/ephemeral-networks-and-chain-ids/7674) cause issues with deployment systems & MetaMask caching, possible solutions: random chain id or new identifier

**Security**

- BadgerDAO [~$120 million exploit](https://rekt.news/badger-rekt/) via token approvals from apparent compromised front end, contracts now paused, [check](https://etherscan.io/tokenapprovalchecker) token approvals
- MonoX [~$31 million exploit](https://medium.com/monoswap/exploit-post-mortem-33921a779b43) on Ethereum and Polygon, pool drained via price manipulation of projects token
- Visor Finance [user pool & test pools exploited](https://twitter.com/Mudit__Gupta/status/1464657484367339527), spot price manipulation, user funds reimbursed from treasury
- 0xhabitat team’s Gnosis Safe [drained](https://blog.gnosis.pm/the-0xhabitat-multisig-got-drained-an-analysis-16ab74ddf42), phishing attack got multisig owners to sign malicious transactions
- dYdX [~$2 million was at risk](https://twitter.com/dydxprotocol/status/1464572467872247815), contract vulnerability with set allowances used for deposit, funds rescued in partnership with samczsun

**Ecosystem**

- Vitalik’s updated [Ethereum roadmap diagram](https://twitter.com/vitalikbuterin/status/1466411377107558402): PoW switch off, rollup scaling via sharding, statelessness, purge of historical data & tech debt, plus extras
- Formalizing the definition of [Maximal Extractable Value](https://writings.flashbots.net/research/formalization-mev/) (MEV)
- Flashbots work in progress research on [cross-domain MEV](https://arxiv.org/abs/2112.01472)

**Enterprise**

- Budweiser US changed Twitter name to beer.eth and [sold 1936 beer can NFTs](https://us.budweiser.com/NFT) for fiat and crypto, with flat $75 fee for minting
- Skiff decentralized document collaboration adds [login with MetaMask](https://www.skiff.org/updates/log-in-with-metamask)
- [Adidas](https://twitter.com/adidasoriginals/status/1466443459951271939) changes Twitter profile pic to their Bored Ape

**Application layer**

- [Tornado Cash](https://tornado-cash.medium.com/tornado-cash-deployment-proposal-on-arbitrum-fb02e508fe74) live on Arbitrum
- Perpetual Protocol [v2](https://medium.com/perpetual-protocol/perpetual-protocol-v2-is-live-on-optimism-mainnet-5b9520bc02a2) live on Optimism
- [Lemma](https://twitter.com/lemmafinance/status/1466127877074657281) basis trading protocol live on Arbitrum
- [Premia](https://twitter.com/PremiaFinance/status/1465789249056354304) single sided staking for call and put pools live on Arbitrum
- [Component](https://medium.com/element-finance/component-launches-yield-token-compounding-tool-built-on-element-finance-ea6da04bdf98) Yield token compounding tool, experimental beta
- [DeversiFi](https://deversifi.com/blog/clarifying-the-dvf-airdrop-methodology/) governance token airdrop to active users, 31% in one category were filtered out as airdrop hunters
- [Bleeps](https://bleeps.art/) NFTs, sounds generated on-chain from synthesizer in Yul outputting a wave file
- [The Signature](https://blog.simondlr.com/posts/the-signature-exploring-time-amp-provenance-in-nft-art), Simon de la Rouviere’s conceptual art NFT exploring provenance
- RARA [NFT RA!CE](https://rara.mirror.xyz/5WNrK3VvIO4Lw4F1iBYuLbx7op3O9L_EQ2EFVpebSnI): NFT curation via like to earn
- [isotile](https://twitter.com/isotile/status/1466870552342192132): any NFT can now be added to a room

* * *

### **Job Listings**

- Ethereum Foundation: [DevOps](https://ethereum.bamboohr.com/jobs/view.php?id=53&source=weekinethnews) for Consensus Layer clients in lead up to merge
- Trail of Bits [summer internship 2022](https://jobs.lever.co/trailofbits/de190abd-ec89-4c72-bda8-d411741a4c32)
- Nethermind 1-3 month [internship program](https://www.notion.so/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)
- ethereum.org team are hiring a [Product Designer](https://ethereum.org/en/about/product-designer/)

**Reach people experienced with Ethereum.**  $420 for two issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US Treasury Secretary says [FATF guidance on crypto doesn’t cover](https://twitter.com/jerrybrito/status/1465684848773840899) hardware wallet manufacturers, unhosted wallet providers, devs or miners who don’t take custody of funds
- [Public domain NFTs](https://metaversal.banklesshq.com/p/nfts-and-cc0), community develops IP and derivatives extend NFT brand
- [DAO contributor compensation](https://thedefiant.io/a-big-test-for-daos-honing-new-compensation-and-contribution-practices/): combination of base compensation, bonuses and governance power

**General**

- [MyCrypto Winter](https://winter.mycrypto.com/) returns for fourth year; security tip advent calendar
- [Faster PLONK verification](https://hackmd.io/@dJO3Nbl4RTirkR2uDM6eOA/BkoOdpwFF) for Halo-like proof-carrying data
- [Zero-knowledge blocklisting](https://eprint.iacr.org/2021/1577) IACR paper, aggregating groth16 proofs 

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-4-2021](https://weekinethereumnews.com/week-in-ethereum-news-december-4-2021)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- **Dec 7 – [Implement on-chain governance](https://twitter.com/openzeppelin/status/1466746540526030848) with OpenZeppelin**
- Dec ~8 – [Arrow Glacier](https://blog.ethereum.org/2021/11/10/arrow-glacier-announcement/) upgrade block 13,773,000
- **Dec 9  – Polygon [zk day](https://polygonzk.ethglobal.com/)**
- **Dec 11 – [Codeless Conduct](https://medium.com/@alexnmr/announcing-codeless-conduct-no-coding-skills-needed-efa0a409b360) no-code hackathon (virtual)**
- Dec 16 – [Gitcoin Grants Round 12](https://gitcoin.co/blog/whats-new-in-the-gitcoin-grants-product/) ends **(support [Week in Eth News](https://gitcoin.co/grants/2785/week-in-ethereum-news))**
- Jan 24-26 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford University)
- Feb 17 – [Schelling Point](https://schellingpoint.gitcoin.co/) (Denver) 
- Feb 18-20 – [ETHDenver](https://www.ethdenver.com/)
- Mar 28-30 – [ETHDubai](https://www.ethdubai.xyz/)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

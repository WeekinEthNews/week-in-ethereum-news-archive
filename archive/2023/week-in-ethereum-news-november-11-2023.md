---
title: "Week in Ethereum News <br> November 11, 2023"
date: "2023-11-11"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=TQ2XEvMzvFg&t=143s). Recap by [Tim Beiko](https://mirror.xyz/abcoathup.eth/ehKl7k9Osvm3jsJbOJtr8XivJBfhIRsK18ATfvv2aVA).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1722635956719866015) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-174/):
    - Goerli shadowfork 0 upgraded to Dencun ([testing analysis](https://notes.ethereum.org/@ethpandaops/goerli-sf-0-analysis))
    
    - Blob gas price in RPC: adding single blobGasPrice method & adding to feeHistory
    
    - [EIP7545](https://eips.ethereum.org/EIPS/eip-7545) (Verkle proof verification precompile) presented

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.48%**](https://dune.com/hildobby/eth2-staking) **is increasing towards** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~85% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm 43% & Lighthouse 34%, any client bug over 33.3% could mean loss of finality

- [Geographic diversity needed for stakers & nodes](https://nodewatch.io/), particularly outside of US/Canada/EU

**Layer 1**

- Otterscan [v2.2-ALPHA](https://github.com/otterscan/otterscan/releases/tag/v2.2.0): improved Sourcify integration and UI improvements

- [Reth snapshots](https://blog.merkle.io/blog/reth-snapshots-faster-syncing-ethereum): public snapshots by merkle, sync a node in 6 hours 

**For Stakers**

- Stereum [v2](https://github.com/stereum-dev/ethereum-node/releases/tag/v2.0.0) (node launcher): install/manage node via UI

**Client releases**

- Consensus layer:
    - Lodestar [v1.12.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.12.0): various updates, upgrade validator & beacon node clients together
    
    - Nimbus [v23.10.1](https://github.com/status-im/nimbus-eth2/releases/tag/v23.10.1): hotfix for peer scoring issue in v23.10.0

- Execution layer:
    - Nethermind [v1.22.0](https://github.com/NethermindEth/nethermind/releases/tag/1.22.0): improved memory management (consumption reduced ~25%)

**Research**

- [Validator smoothing commitments](https://ethresear.ch/t/validator-smoothing-commitments/17356): out of protocol solution to improve permissionless liquid staking protocols, node operators pay upfront to run validators for a minimum duration 

- [Inclusion list framework](https://ethresear.ch/t/the-costs-of-censorship-a-modeling-and-simulation-approach-to-inclusion-lists/17382) to evaluate designs on censorship resistance metrics 

- [MEV burn benefits](https://ethresear.ch/t/dr-changestuff-or-how-i-learned-to-stop-worrying-and-love-mev-burn/17384): improves validator economics, lessens builder liquidity requirements, increases cost of censorship and improves resilience in a mass MEV event

- [Signature Merge](https://ethresear.ch/t/signature-merging-for-large-scale-consensus/17386): massive-scale signature aggregation using recursive SNARKs & PCD

**Layer 2**

- [OP Reth](https://twitter.com/gakonst/status/1721254692796428294): Reth (execution layer client) can be used in OP Stack

- Justin Drake: [based rollup/validium preconfirmations](https://ethresear.ch/t/based-preconfirmations/17353) of transaction execution, latencies on the order of 100ms

**EIPs/Standards**

- EIPs
    - [EIP7553](https://github.com/ethereum/EIPs/pull/7949/files): Separated payer transaction

- ERCs (application layer):
    - [ERC7554](https://github.com/ethereum/ERCs/pull/97/files): NFTs benefits attachment via metadata (ERC721 extension)
    
    - [ERC7555](https://github.com/ethereum/ERCs/pull/99/files): Single sign-on for account discovery
    
    - [ERC7556](https://github.com/ethereum/ERCs/pull/100/files): Embedded accounts as smart modules

**Stuff for developers**

- Solidity [v0.8.23](https://soliditylang.org/blog/2023/11/08/solidity-0.8.23-release-announcement): fixes invalid verbatim deduplication bug

- Remix [v0.37.0](https://medium.com/remix-ide/remix-release-v0-37-0-dbc750f7ab15): adds Semaphore Circom template, auto-complete loads ERC files and translations in Spanish/French/Italian/Simplified Chinese

- Secureum RACE #23: [8 question Solidity quiz & answers](https://veridise.notion.site/veridise/RACE-23-Answers-d63cb0b5373f43f0ba43612e89596547)

- Fe (language) bug bounty: [Simple DAO](https://blog.fe-lang.org/posts/simple-dao-written-in-fe-go-break-it)

- Proposal for [Edge](https://jtriley.substack.com/p/the-edge-programming-language) (EVM domain specific language), currently at specification stage

- [Superchain faucet](https://blog.oplabs.co/providing-easier-access-to-testnet-eth-across-the-superchain-with-the-superchain-faucet/): claim 0.05 testnet ETH for OP Stack testnets

- [500 testnet ETH](https://twitter.com/_pk910_/status/1721472568765345955) (Sepolia & Holešky) claimable by Devconnect attendees using Zupass

- [Zupass Scaffold-ETH 2](https://github.com/BuidlGuidl/zupass-scaffold-eth-2#readme) starter kit

- pcaversaccio’s [Hardhat template](https://github.com/pcaversaccio/hardhat-project-template-ts#readme): updated to ethers v6 & Hardhat configuration variables

- [VSCode Solidity inspector](https://github.com/PraneshASP/vscode-solidity-inspector#readme): adds support for .tree files

- [EVM tracing](https://github.com/paradigmxyz/ultimate_evm_tracing_reference#readme) reference

- [TypeChain](https://twitter.com/krzkaczor/status/1721936603919032415) deprecated

**Security**

- AAVE [security incident](https://governance.aave.com/t/aave-v2-v3-security-incident-04-11-2023/15335), forks of v2/v3 should disable stable rate mode borrowing

- MEV bot [$2 million exploit](https://rekt.news/ripmevbot2/) via unprotected swap function

- Raft [1.6k ETH exploit](https://twitter.com/frankresearcher/status/1723099971824582713), 1570 ETH burnt, attacker lost 4 ETH

- The Standard on Arbitrum [$260k exploit](https://twitter.com/thestandard_io/status/1722079924243386795) via price manipulation

- zkSync Era [vulnerability disclosed](https://medium.com/chainlight/uncovering-a-zk-evm-soundness-bug-in-zksync-era-f3bc1b2a66d8), 50k USDC bounty paid

**Ecosystem**

- Devconnect [live stream](https://app.streameth.org/) for selected events

- ETH Lisbon [hackathon projects](https://taikai.network/ethlisbon/hackathons/ethlisbon-2023/projects)

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 9.9 to 323.6 gwei, with 28.9 gwei average
    - Zero net issuance currently at 21.7 gwei 
    
    - 6.6k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $1,829 - $2,133, currently $2,080

- [ETHBTC](https://ratiogang.com/): currently 0.056 (Flippening at ~0.16)

**Notable at app layer**

- USDC & EURC [v2.2](https://www.circle.com/blog/announcing-usdc-v2.2): phased rollout, reduces gas costs & supports ERC1271

- [Coinbase Verifications](https://twitter.com/CoinbaseCloud/status/1722702330406060282): onchain user attestations for account & country verified by Coinbase, uses Ethereum Attestation Service (EAS)

- Sablier UI [dynamic streams](https://blog.sablier.com/dynamic-streams-in-the-sablier-ui/): adds timelock, unlock-linear & unlock-cliff

- CoW Swap [programmatic orders](https://blog.cow.fi/introducing-the-programmatic-order-framework-from-cow-protocol-088a14cb0375): approve orders with a single signature, execute automatically

- [Notional v3](https://blog.notional.finance/notional-v3-is-live-on-arbitrum/) live on Arbitrum, adds variable rate lending/borrowing & leveraged liquidity strategies

- [Show Up](https://twitter.com/wslyvh/status/1721548077268435318) (RSVP for events): request deposits on registration, attendees get paid for showing up

- [Bountycaster](https://www.bountycaster.xyz/faq) (bounties platform) live on Farcaster, beta

- [Gaslite Drop](https://twitter.com/poppunkonchain/status/1723102711191597057) adds airdrop to X (Twitter) post replies, filter & token gate recipients

- Sound [magic upload](https://sound.mirror.xyz/Z5fnJyTvTnHJs1Bb_CgzbL5eNFJu0D2BKHomBmrPYFU): zero gas upload, only requires an email address

- Optimism [We ❤️ The Art](https://optimism.mirror.xyz/K6b7_LpAK88jWo0FJLRGflxxpIzbgVJdYfGZ3pFcfUM): NFT creator contest (AI, generative, music & 1of1s), 1M OP in prizes

* * *

### Job Listings

- Aragon: [Senior smart contract developer](https://jobs.lever.co/aragon/2f3cf4c4-041a-4978-aa6b-78f447358956) w EIP, auditing experience

- Nethermind: [Smart Contract Auditor](https://grnh.se/cf4858b2teu), [Smart Contract Auditor (Rust)](https://grnh.se/e2a692a2teu) & [BizDev](https://grnh.se/9fbf4582teu)

- [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db) wanted by EF

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

- Gnosis seek [DevRels](https://gnosis.jobs.personio.com/job/1296307?_pc=1517287&display=en) & [Backend Devs](https://gnosis.jobs.personio.com/job/1284509?_pc=1517287)

**Job listings: $600 for four issues** (75 character limit).  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [UK FCA & Bank of England proposals](https://www.bankofengland.co.uk/news/2023/november/fca-and-bank-of-england-publish-proposals-for-regulating-stablecoins) for regulating stablecoins

- [OFAC](https://home.treasury.gov/news/press-releases/jy1874) sanctioned Ekaterina Zhdanova for laundering & moving funds on behalf of Russian elites

- [SEC facing challenges hiring crypto specialists](https://twitter.com/jeffjohnroberts/status/1721543698784419917) due to prohibition of holding

- [Open problems in DAOs](https://arxiv.org/abs/2310.19201) for researchers

- [DAO decentralization](https://arxiv.org/abs/2311.03530): Voting-Bloc Entropy (VBE) decentralization metric & a practical Dark DAO

**General**

- Exchange hacks: [$126M for Poloniex](https://rekt.news/poloniex-rekt/)

- [ApeFest attendees report eye/skin issues](https://twitter.com/BoredApeYC/status/1722419475440701487), likely caused by UV lights

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-november-11-2023](https://weekinethereumnews.com/week-in-ethereum-news-november-11-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul), [update 2](https://blog.ethereum.org/2023/11/03/devconnect-ist-update-2)

- Nov 15-21 – [DCxPrague](https://dcxprague.org) (Devconnect satellite event in Prague)

- Nov 15-29 – [Gitcoin Grants 19](https://grants.gitcoin.co/#GG19-Rounds)

- Nov 16-19 – [Pragma](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Nov 18 – [Ethereum Costa Rica](https://www.meetup.com/ethereumcr/events/295894129/)

- Nov 30 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) deadline (max $1k for local meetups)

- Dec 4 – [ETHVenice](https://ethvenice.com/)

- Dec 6-7 – [Columbia CryptoEconomics workshop](http://columbiacryptoeconomics.org/) (New York)

- Dec 8-10 – ETHGlobal [ETHIndia](https://ethindia.co/) (Bangalore) 

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

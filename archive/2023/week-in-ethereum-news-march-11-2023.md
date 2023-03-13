---
title: "Week in Ethereum News <br> March 11, 2023"
date: "2023-03-11"
---

## **Eth News and Links**

**Shapella (Shanghai + Capella) upgrade**

- Update your Goerli testnet nodes ready for [Shapella upgrade on March 14](https://github.com/ethereum/execution-specs/blob/master/network-upgrades/mainnet-upgrades/shanghai.md#upgrade-schedule)

- Consensus layer Sepolia releases:
    - Lighthouse [v3.5.1](https://github.com/sigp/lighthouse/releases/tag/v3.5.1)
    
    - Lodestar [v1.5.1](https://github.com/ChainSafe/lodestar/releases/tag/v1.5.1)
    
    - Nimbus [v23.3.0](https://github.com/status-im/nimbus-eth2/releases/tag/v23.3.0)
    
    - Prysm [v3.2.2](https://github.com/prysmaticlabs/prysm/releases/tag/v3.2.2)
    
    - Teku [v23.3.0](https://github.com/ConsenSys/teku/releases/tag/23.3.0)

- Execution layer Sepolia releases:
    - Besu [v23.1.1](https://github.com/hyperledger/besu/releases/tag/23.1.1)
    
    - Erigon [v2.40.1](https://github.com/ledgerwatch/erigon/releases/tag/v2.40.1)
    
    - Geth [v1.11.4](https://github.com/ethereum/go-ethereum/releases/tag/v1.11.4)
    
    - Nethermind [v1.17.1](https://github.com/NethermindEth/nethermind/releases/tag/1.17.1)

- [MEV-Boost guide](https://flashbots.notion.site/MEV-Boost-Capella-Upgrades-00cea01704794f6eb4f792c55b69c441) updated with recommended versions for Shapella Goerli upgrade

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=C5SmmkriuwA&t=365s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/BkIOGvPy2) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-consensus-call-104/):
    - Discussions on blob signing API, SSZ, adding parent slot to blocks/attestations and draft Verge spec

**Dencun (Cancun + Deneb) upgrade**

- KZG Ceremony:
    - [71k+ contributors](https://ceremony.ethereum.org/), 19k+ in the lobby, only 2 days left in _first_ general contribution period

- Latest EIP4844 implementers [call video](https://www.youtube.com/watch?v=8hDlg-x6MjE&t=3s). Notes from [Terence](https://twitter.com/terencechain/status/1633163513245110272)

**Layer 1**

- Proposal for [execution layer clients to suggest using a local block](https://github.com/ethereum/execution-apis/pull/388) based on their view of execution data

- Verkle testnet [Kaustinen](https://twitter.com/parithosh_j/status/1633772212359421956) reborn, using proofs in blocks to conform with the consensus spec

- Ethereum Protocol Fellows cohort 3 [projects](https://github.com/eth-protocol-fellows/cohort-three/tree/master/projects#readme) & [final presentations](https://www.youtube.com/watch?v=oF_BRlXMVNY) \[video\]

- [E-star name discussion](https://ethereum-magicians.org/t/e-star-name-for-consensus-layer-upgrade-after-deneb/13248) for Consensus Layer upgrade after Deneb

**Layer 2**

- Arbitrum proposal to [reduce challenge period for optimistic rollups](https://ethresear.ch/t/reducing-challenge-times-in-rollups/14997), uses Proof of Stake discrete slot times to detect possible forking censorship (block filtering)

- Justin Drake: [based (L1 sequenced) rollups](https://ethresear.ch/t/based-rollups-superpowers-from-l1-sequencing/15016), L1 proposers include rollup blocks as part of L1 blocks

- Concept of [multi-verifiers for validating bridges](https://ethresear.ch/t/multi-verifiers-as-a-hedge-against-validating-bridge-implementation-vulnerabilities/14974): increases security but at the expense of bridging cost

**EIPs/Standards**

- EIPs:
    - [EIP712](https://eips.ethereum.org/EIPS/eip-712): Typed structured data hashing and signing; (updated to match common implementations [without author approval](https://twitter.com/_SamWilsn_/status/1633494479490498560))
    
    - [EIP6601](https://github.com/ethereum/EIPs/pull/6601/files): EVM Modular Arithmetic Extensions (EVMMAX)

- ERCs:
    - [ERC6617](https://eips.ethereum.org/EIPS/eip-6617): Bit based permission
    
    - [ERC6662](https://github.com/ethereum/EIPs/pull/6662/files): AA account metadata for authentication (ERC4337 extension)
    
    - [ERC6672](https://github.com/ethereum/EIPs/pull/6672/files): Multi-redeemable NFTs

* * *

**This newsletter is made possible thanks to** [**Tenderly**](https://tenderly.co/)**’s** [**Web3 Gateway**](https://dashboard.tenderly.co/register?redirectTo=gateways)**!**

![Tenderly Web3 Gateway](https://weekinethereumnews.com/wp-content/uploads/2022/12/tenderly-1024x439.jpg)

The Tenderly platform enables Web3 developers to build, test, monitor, and operate smart contracts in one place. To cover each aspect of the dapp development lifecycle, Tenderly expanded its product offering and released Tenderly Web3 Gateway. This is a production node as a service that delivers fast and easy access to the blockchain.

Tenderly Web3 Gateway is fully integrated with the rest of the platform, combining infrastructure with development tooling and observability. It enables blockchain developers to:

- Speed up read-heavy workloads up to eight times

- Set up reliable node infrastructure with 100% blockchain data consistency

- Reduce node infrastructure management overhead

- Scale dapps with ease to meet their growing user base

- Unify dapp development by combining infrastructure with tooling and observability

- Improve development teams’ velocity and collaboration by eliminating development silos

- Preview transaction outcomes directly from Tenderly Web3 Gateway before sending them on-chain

[Try Tenderly Web3 Gateway](https://dashboard.tenderly.co/register?redirectTo=gateways).

* * *

**Stuff for developers**

- [Solidity developer survey 2022 results](https://blog.soliditylang.org/2023/03/10/solidity-developer-survey-2022-results/): Hardhat usage at 75%, Remix 42%, Foundry jumped to 30%, Truffle down to 17%; Solidity v0.8 usage at 90%

- [Goerlinator](https://goerlinator.xyz/): ETH Denver attendees can claim 50 Goerli ETH

- [SS2ERC721](https://github.com/showtime-xyz/SS2ERC721#readme): batch mints for up to 1228 addresses using SSTORE2, experimental

- [Console.huff](https://github.com/AmadiMichael/Huff-Console#readme): console.log for Huff, uses Foundry with experimental StdStyle support

- snekmate [v0.0.1](https://github.com/pcaversaccio/snekmate/releases/tag/v0.0.1) (Vyper contracts): ERC20/721/1155/4626, ownable/access control & utilities 

- ethers.js [v6](https://docs.ethers.org/v6/migrating/) (soft launched) & [v6.1](https://github.com/ethers-io/ethers.js/blob/main/CHANGELOG.md#ethersv610-2023-03-07-0210): ES2020 BigInt replaces BigNumber, imports in the root package and Typed API to call contracts

- [viem](https://twitter.com/wagmi_sh/status/1632814443972395010): lightweight composable TypeScript modules to interface Ethereum (alternative to ethers.js/web3.js)

- Scaffold-Eth [v2](https://github.com/scaffold-eth/se-2#readme): Typescript, NextJS, wagmi, RainbowKit & Hardhat; contract hot reloading & burner wallets

- [noble-curves](https://twitter.com/paulmillr/status/1633804139472777218): JavaScript library for elliptic curves now production-ready

- [AnyABI](https://anyabi.xyz/): fetch ABI using chain ID & address for contracts verified on Etherscan or Sourcify

- [Equivalence checking](https://twitter.com/zachobront/status/1633906650514898947) using Halmos (symbolic execution tool)

- CTFs:
    - Curta CTF 2 × 4 = 8 challenge [solved](https://twitter.com/0xkarmacoma/status/1632551527729758208) using Halmos
    
    - Curta CTF 0xF1A9 challenge [solution](https://twitter.com/0x796/status/1634245725574905858) using Foundry 
    
    - Base challenge [solution](https://mirror.xyz/0x65b54A4646369D8ad83CB58A5a6b39F22fcd8cEe/uyisyXLf0vrBv9jhnGMe9fnacE5mAaXkDwg6mP2a9sk) using Foundry
    
    - [Ethernaut in Yul](https://dev.to/teddav/solving-the-ethernaut-with-yul-2a4h) using Foundry
    
    - Sussy Huff [solution](https://gist.github.com/Jinmo/b6951c223ad19c8f1fa7b5a1aadc5e9a)

- [Dune SQL](https://dune.com/blog/introducing-dune-sql): queries as views, querying using addresses and 256 bit integer data types

- Echidna [v2.1.0](https://github.com/crytic/echidna/releases/tag/v2.1.0): on-chain fuzzing using state via RPC, experimental Windows support

- Semaphore [v3.2.0](https://github.com/semaphore-protocol/semaphore/releases/tag/v3.2.0): Sepolia & Optimism Goerli testnet support, SemaphoreEthers to fetch on-chain data

**Security**

- Tender Finance [$1.59 million exploit](https://tenderfi.medium.com/march-7-postmortem-170373e93cd1) via decimal error in oracle integration, 62 ETH bounty agreed

**Ecosystem**

- Phil Daian: [geographic decentralization](https://collective.flashbots.net/t/decentralized-crypto-needs-you-to-be-a-geographical-decentralization-maxi/1385) needed to avoid centralization

- ETHDenver [videos](https://www.youtube.com/playlist?list=PLAy4HNUNlzRlPMWDNd1Oxun1X54EqP8K1) and [hackathon winners](https://twitter.com/ethereumdenver/status/1632501068134506496)

- [ETHGlobal](https://ethglobal.medium.com/updates-to-the-2023-ethglobal-hackathon-season-1d2a9d418c91) postponed Istanbul (likely until November), added Lisbon as a replacement, moved Toronto to Waterloo and added Pragma 1 day conference

- [Etherscan](https://twitter.com/etherscan/status/1634188648144052226) adds gas guzzlers, block producers & contract statistics dashboards

**Enterprise**

- Coinbase [Wallet as a Service](https://www.coinbase.com/blog/coinbase-announces-wallet-as-a-service-now-any-company-can-seamlessly): APIs to create Multi-Party Computation (MPC) wallets, split between the end user & Coinbase

**Application layer**

- [Privacy Pools v0](https://twitter.com/ameensol/status/1632083054272430080): live on Optimism, non-custodial mixer with opt-in/opt-out anonymity sets, unaudited, experimental

- [Oasis](https://twitter.com/chrisbducky/status/1633889732882227207) disabled upgradeability after funds were recovered from Wormhole exploiter

- [Iron Bank froze Alpha Homora accounts](https://rekt.news/iron-alpha/) due to $30 million debt from 2021 exploit

- [Maker proposal](https://forum.makerdao.com/t/proposal-to-increase-debt-ceiling-for-mip65-by-750m-to-1250m/20060) to buy additional $750 million in US Treasuries

- Element Finance [Council Kit](https://blog.element.fi/launching-council-kit/): SDK to create & manage DAOs

- [Senate](https://twitter.com/senatelabs/status/1633518240558194699): track governance proposals across various DAOs 

- Reservoir's [Seaport Oracle](https://twitter.com/reservoir0x/status/1633556174774882321): co-sign for off chain cancellations & price changes of listings & bids

- ethOS [v2](https://twitter.com/EthereumPhone/status/1633875656969945088) (mobile OS): native web3 browser, mint NFTs from photos and app store

* * *

### Job Listings

- L2BEAT 💗 is hiring a Senior Software Engineer & Product Owner. [Apply here!](https://l2beat.notion.site/We-are-hiring-Work-at-L2BEAT-e4e637265ae94c5db7dfa2de336b940f)

- Certora is hiring a [Senior Enterprise Sales Rep](https://www.certora.com/#careers).

- [Immutable](https://www.immutable.com/) is hiring a [Protocol Blockchain Engineer](https://jobs.lever.co/immutable/03e6848f-6cc7-4295-a162-7910b0368c4d).

- Frax Finance is expanding their official core developer team. [Apply here!](https://docs.google.com/forms/d/e/1FAIpQLSem7KL-FFgsuxaUMww4OXMxdJ-qXfyWJ_IvGdqVteBSM5FgxA/viewform)

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Silvergate Bank](https://ir.silvergate.com/news/news-details/2023/Silvergate-Capital-Corporation-Announces-Intent-to-Wind-Down-Operations-and-Voluntarily-Liquidate-Silvergate-Bank/default.aspx) winding down

- [Silicon Valley Bank](https://www.fdic.gov/news/press-releases/2023/pr23016.html) closed by California regulator with FDIC as receiver

- [US Office of the Investor Advocate](https://pcaobus.org/resources/information-for-investors/investor-advisories/investor-advisory-exercise-caution-with-third-party-verification-proof-of-reserve-reports) cautions relying on Proof of Reserve reports

- Simon de la Rouviere: [NFT royalties matter](https://sceneswithsimon.substack.com/p/why-nft-royalties-matter), they allow creators to relinquish IP rights, give away NFTs and still make money to continue creating

**General/crypto**

- [Summer of Protocols](https://efdn.notion.site/Summer-of-Protocols-3d7983d922184c4eb72749e9cb60d076): 18 week program, funding full & part time protocol researchers

- [Polynonce](https://research.kudelskisecurity.com/2023/03/06/polynonce-a-tale-of-a-novel-ecdsa-attack-and-bitcoin-tears/): ECDSA key recovery attack using a batch of consecutive & ordered signatures

- [SHA-3 buffer overflow vulnerability](https://eprint.iacr.org/2023/331) found in several implementations

- [Icicle](https://medium.com/@ingonyama/introducing-icicle-an-open-source-gpu-library-for-zero-knowledge-acceleration-aad8c35b7f0a): library for ZK acceleration using CUDA-enabled GPUs, used in [Danksharding builder](https://medium.com/@ingonyama/fast-danksharding-using-icicle-6411565bb245)

- [Poseidon2](https://eprint.iacr.org/2023/323): optimized version of Poseidon hash function

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-march-11-2023](https://weekinethereumnews.com/week-in-ethereum-news-march-11-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- **Mar 13 –** [**Shapella community call**](https://github.com/ethereum/pm/issues/741)

- Mar 14 – [Goerli testnet upgrades to Shapella](https://github.com/ethereum/execution-specs/blob/master/network-upgrades/mainnet-upgrades/shanghai.md#upgrade-schedule)

- Mar 15-16 – [ETHDubai](https://www.ethdubaiconf.org/)

- Mar 16-18 – [ETH Porto](https://ethporto.org/)

- **Mar 21 – deadline for** [**Summer of Protocols**](https://efdn.notion.site/Application-5b71c238d6bd44cf9137946ef7767e53)

- Mar 28-30 – [Ethereum Rio](https://www.ethereumbrasil.com/ethereumrio)

- Mar 31 - Apr 2 – [ETHSamba](https://twitter.com/ethsamba/status/1631326304447627265) (Rio) hackathon & conference

- Mar 31 – deadline for [EF account abstraction grants round](https://esp.ethereum.foundation/account-abstraction-grants)

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- **Apr 13-16 –** [**Pragma Tokyo**](https://ethglobal.com/events/pragma-tokyo) & [ETHGlobal Tokyo](https://tokyo.ethglobal.com/) hackathon

- Apr 14-16 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference & hackathon

- Apr 21-25 – [EthTaipei](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) hackathon & conference

- Apr 27-30 – [Istanbul ETH Privacy](https://www.leadingprivacy.com/istanbul) conference & hackathon

- May 5-10 – [ETHTallinn](https://ethtallinn.org/) hackathon & [NFT Tallinn](https://nfttallinn.com/) conference

- **May 12-14 –** [**ETHGlobal Lisbon**](https://ethglobal.com/events/lisbon)

- May 19-23 – [EDCON](https://edcon.io/) Montenegro (changed from Vienna)

- May 20-21 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 24-26 – [Spaghett ETH](https://naples.spaghett-eth.com/) (Naples) conference

- May 26-28 – [ETHDublin](https://www.ethdublin.io/) hackathon

- Jun 2-4 – [ETH Seoul](https://2023.ethseoul.org/)

- Jun 2-6 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 9-11 – [ETHPrague](https://ethprague.com/) conference & hackathon

- **Jun 23–25 –** [**ETHGlobal Waterloo**](https://ethglobal.com/events/waterloo2023) **(changed from Toronto)**

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Aug 16-19 – [Ethereum Argentina](https://twitter.com/EtherArgentina/status/1625857633260552200) (Buenos Aires)

- Aug 30 - Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- **Sep 1-3 –** [**Ethcon Korea**](https://ethcon.kr/) **hackathon**

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- **Sep 11-13 –** [**DappCon**](https://www.dappcon.io/) **(Berlin)**

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–25 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

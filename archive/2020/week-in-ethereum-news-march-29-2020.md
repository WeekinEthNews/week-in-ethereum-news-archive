---
title: "Week in Ethereum News<BR> March 29, 2020"
date: "2020-03-29"
---

## **Eth News and Links**

**Eth1**

- [Geth v1.9.11’s eth/65 data propagation](https://twitter.com/peter_szilagyi/status/1243496759294337026) has reduced bandwidth 75%
- Nethermind [v1.7.12](https://github.com/NethermindEth/nethermind/releases/tag/1.7.12) has eth/65 support
- Notes from the [latest stateless call](https://ethresear.ch/t/stateless-ethereum-march-25th-call-digest/7202)
- Guillaume Ballet on [why we switch from hex to binary and how the overlay tree works](https://medium.com/@gballet/ethereum-state-tree-format-change-using-an-overlay-e0862d1bf201)
- Evaluating the [proposals to reduce witness size](https://ethresear.ch/t/survey-of-proposals-to-reduce-block-witness-size/7173/)
- [Eth on ARM updated images](https://www.reddit.com/r/ethereum/comments/fo1p2b/ethereum_on_arm_nethermind_and_hyperledger_besu/) to run full nodes on Raspberry Pis: Geth, Nethermind, Parity, Besu.

**Eth2**

- Latest [eth2 implementer call](https://youtu.be/Vn1oHH55yPk?t=245). Ben Edgington’s [notes](https://hackmd.io/@benjaminion/BkdbG45II)
- Least Authority’s [audit report of eth2 spec](https://leastauthority.com/blog/ethereum-2-0-specifications/)
- Notes from the [latest networking call](https://hackmd.io/@benjaminion/rkEn7C_88)
- Mikerah explores [hybrid networking architectures for validator privacy](https://ethresear.ch/t/exploring-a-hybrid-networking-architecture-for-improved-validator-privacy-in-eth2-0/7207)
- Latest [Nimbus client update](https://our.status.im/nimbus-march-update/), full interop is main focus. processing validators and sigs 5x faster
- RuntimeVerification: [verifying ewasm code](https://medium.com/dlabvc/verifying-ethereum-flavored-wasm-ewasm-code-de91ab3179be)
- Carl Beekhuizen's [sharded consensus explainer](https://blog.ethereum.org/2020/03/27/sharding-consensus/), and why signature aggregation is so vital

**Eth2+**

- [Hashmap-based polynomial commitments](https://ethresear.ch/t/hashmap-based-polynomial-commitments-for-state/7186)
- [Multi-layer hashmaps for state storage](https://ethresear.ch/t/multi-layer-hashmaps-for-state-storage/7211)
- [ZKStudyClub video on polynomial commitments](https://www.youtube.com/watch?v=Fti600ag_I8) with Justin, Vitalik and Dankrad
- [Casper CBC achieves liveness](https://eprint.iacr.org/2020/362.pdf) even in async networks

Layer2

- [AZTEC zk-zkrollup](https://medium.com/aztec-protocol/aztec-fast-privacy-with-zk%C2%B2-rollup-7c742f45457) with PLONK proofs. Will soon ship 100 private transactions per second on mainnet
- [Error-correcting code to optimize ZK-rollup verifier](https://ethresear.ch/t/error-correcting-code-to-optimize-zk-rollup-verifier/7192)
- A revamped [Nutberry optimistic rollup](https://ethresear.ch/t/abra-ka-dabra-a-k-d-a-revamped-nutberry-protocol/7175) plan

**Stuff for developers**

- Solidity v0.6.x features: [fallback and receive](https://solidity.ethereum.org/2020/03/26/fallback-receive-split/)
- [Yul+](https://medium.com/@fuellabs/introducing-yul-a-new-low-level-language-for-ethereum-aa64ce89512f) from Fuel Labs. Features added to Yul’s low-level intermediate language: enums, constants, booleans, memory structures, safemath
- Truffle [v5.1.19](https://github.com/trufflesuite/truffle/releases/tag/v5.1.19). fully decode internal function pointers, new --bail flag in TruffleTest
- [MetaMask Ethereum provider survey](https://docs.google.com/forms/d/e/1FAIpQLSc9iZf2xZEx-ae3-0C9zk6Kmi8tBCvsVxD30fDBEVUj5JuOyA/viewform)
- Catching weird [bugs in Solidity with invariant checks](https://medium.com/@muellerberndt/catching-weird-security-bugs-in-solidity-smart-contracts-with-invariant-checks-435582dfb5bd)
- Slither [v0.6.10](https://github.com/crytic/slither/releases/tag/0.6.10) - 5 new detectors, support for Solidity v0.6
- Samczsun finds a [bug in Synthetix release](https://blog.synthetix.io/bug-disclosure/)
- Build an [API to interact with Compound](https://medium.com/compound-finance/compound-ethereum-api-with-infura-1f5c555fd4a2)
- Using the [debugger in Remix](https://medium.com/remix-ide/remix-debugger-b542ea24a0d) online IDE
- [Building frontends with React and NetworkJS](https://blog.infura.io/dapp-frontend-network)
- [OpenZeppelin CLI v2.8](https://forum.openzeppelin.com/t/openzeppelin-cli-2-8-opt-out-of-upgradeability/2477), now you can opt out of upgradeability
- [Survey of upgradeability standards](https://medium.com/coinmonks/summary-of-ethereum-upgradeable-smart-contract-r-d-part-2-2020-db141af915a0)
- [ELI5smartcontracts](https://www.reddit.com/r/ethereum/comments/fpp287/solidity_to_eli5_compiler_human_readable_smart/): input Solidity code and the website tells you what it does
- [Nim libp2p tutorial](https://our.status.im/nim-libp2p-tutorial-chat/) of peer to peer chat
- Zeropool’s [Fawkes](https://ethresear.ch/t/fawkes-crypto-zksnarks-framework-from-zeropool/7201) framework in Rust for building bellman circuits
- Iden3’s [Circom v0.5](https://blog.iden3.io/introducing-circom-0-point-5.html) - updated tutorial. Open sourced very fast finite field libraries, getting close to being production ready for writing snark circuits.

**Ecosystem**

- An annotated version of Vitalik’s [Eth2020 roadmap](https://ethos.dev/ethereum-2020-roadmap/)
- Another tool to [understand/revoke what contracts you have given authority](https://james-sangalli.github.io/eth-allowance/) to spend your tokens
- [Ceramic](https://medium.com/ceramic/introduction-to-the-ceramic-protocol-8d56951ae3f), a permissionless protocol on Eth & IPFS for tamper-proof documents

**Enterprise**

- Ericsson: [designing a decentralized marketplace](https://www.ericsson.com/en/blog/2020/3/decentralized-marketplace-cloud)
- Hyperledger Besu [v1.4.2](https://github.com/hyperledger/besu/releases/tag/1.4.2) - improved onchain privacy groups

**Governance, DAOs, and standards**

- [Governance in decentralized networks](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3551099), a survey paper from Streamr's Risto Karjalainen
- A [primer on Moloch v2](https://medium.com/raid-guild/moloch-evolved-v2-primer-25c9cdeab455), how new features improve grants and enable for-profit DAOs
- The [MKR token is now controlled by its governance](https://blog.makerdao.com/the-transfer-of-mkr-token-control-to-governance-the-final-step/)
- [ERC2567](https://github.com/ethereum/EIPs/issues/2567): Human-Readable Parameters for Contract Function Execution
- [EIP2565](https://github.com/ethereum/EIPs/blob/1c10758235b5a1ec7f452cb238930f7967202310/EIPS/eip-2565.md): Repricing of the EIP-198 ModExp precompile

**Application layer**

- [Uniswap announces v2](https://uniswap.org/blog/uniswap-v2/): token to token pairings, protocol fee, oracles, flash swaps
- [TheSandbox partnering with Atari](https://medium.com/sandbox-game/partnership-announcement-the-sandbox-ft-atari-c0a828ed32c5) to feature their titles
- Mailchain’s [Dapplaunch](https://medium.com/@Mailchain_xyz/at-ethlondon-we-built-dapplaunch-a-web-3-marketing-platform-31bfd58e7f55), a web3 email marketing tool
- You can now play Austin Griffith’s [Galleass game on xDai](https://www.youtube.com/watch?v=UY-hMgjVvxk&feature=youtu.be)
- Maker’s flop auctions [successfully concluded for ~253 DAI](http://flops.live/) average price
- 3 [critical trading risks mitigated](https://medium.com/sunrise-over-the-merkle-trees/how-augur-v2-tackles-three-critical-trading-risks-912e53dc591a) in Augur v2
- Synthetix’s [Hadar release](https://blog.synthetix.io/the-hadar-release/) includes Brent Crude oil, FTSE100 and S&P Global1200
- UMA’s [priceless synthetic token](https://medium.com/uma-project/priceless-synthetic-tokens-f28e6452c18b) design pattern to reduce oracle dependency
- [Furucombo](https://furucombo.app), a GUI for combining DeFi transactions into 1
- [TrustlessFund](https://medium.com/trustless-fund/introducing-trustless-fund-67111a0869a6), a timelock for ETH and tokens
- [LEND721](https://medium.com/@deimantasspucys/launching-lend721-platform-on-ethereum-mainnet-e5054b040446), an NFT borrowing platform, is live on mainnet

**Tokens/Business/Regulation**

- SDNY judge [halts Telegram token distribution](http://www.innercitypress.com/sdnycrypto2secvtelegram032420.html) with preliminary injunction

**General**

- Vitalik’s [garbled circuits primer](https://vitalik.ca/general/2020/03/21/garbled.html)
- Semaphore had to restart the [random value generation process](https://medium.com/@weijiek/restarting-the-semaphore-random-value-generation-process-980e19db11da)
- Hive, the community-led fork of Steem, is currently trading for significantly more [more than STEEM after Tron’s hijack attempt](https://steempeak.com/communityfork/@hiveio/announcing-the-launch-of-hive-blockchain)

* * *

## **Dates of Note**

Upcoming dates of note _(_new in **bold**_)_**:**

- Apr 3 - [EEA Mainnet Working Group](https://medium.com/@tasd/first-public-meeting-of-enterprise-ethereum-alliance-mainnet-working-group-scheduled-9ec6c6afc98e) public meeting
- Apr 3-6 - [NonCon](https://noncon.org/) (Vienna) - [now virtual](https://twitter.com/ParallelePolis/status/1237450754761293830)
- **Apr 7 - [Gitcoin Grants CLR, round 5](https://gitcoin.co/grants/) ends (shameless plug: [my grant](https://gitcoin.co/grants/237/week-in-ethereum-news))**
- Apr 13 - Deadline to apply for [50k euro for blockchain startup](https://blockchers.eu/open-calls/)s in Europe
- Apr 24-26 - [EthTurin](https://ethturin.com/) - now virtual
- Apr 29-30 - [SoliditySummit](https://solidity-summit.ethereum.org/) (Berlin) - [now virtual](https://twitter.com/ethchris/status/1237833026257764359)
- May 8-9 - [Ethereal Summit](https://www.etherealsummit.com/) (NYC) - [now virtual](https://www.etherealsummit.com/news/join-us-for-the-ethereal-virtual-summit-2020)
- May 22-31 - [Ethereum Madrid](https://ethereummadrid.com/hackathon-2020-update/) public health virtual hackathon
- June 17 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

* * *

## **Thank you, ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum News. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

* * *

## **I really want you to link to [weekinethereumnews.com](https://weekinethereumnews.com/)**

Issue permalink: [https://weekinethereumnews.com/week-in-ethereum-news-march-29-2020/](https://weekinethereumnews.com/week-in-ethereum-news-march-29-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

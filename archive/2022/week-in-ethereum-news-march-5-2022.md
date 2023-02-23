---
title: "Week in Ethereum News <br> March 5, 2022"
date: "2022-03-05"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest core devs call [video](https://www.youtube.com/watch?v=ZKPElqIfteU&t=247s). Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1499865801687375877):
    - Kiln public testnet next week
    - JSON RPC discussion if safe head or latest block should be default
    - Shanghai upgrade priorities are withdrawals, lower rollup fees, agreed EVM improvements and quick wins  
    - Shanghai candidates: EIP4863 push withdrawals, EIP4844: shard blob transactions & EIP3651: warm COINBASE 
    - Not including in Shanghai EIP3978: gas refunds on reverts
    - Name for Execution Layer PoW switch off to be decided next week
- [Blocks per week](https://ethresear.ch/t/blocks-per-week-as-an-indicator-of-the-difficulty-bomb/12120) indicate when the difficulty bomb explodes

**Proof of Stake consensus layer**

- Consensus specs [v1.1.10](https://github.com/ethereum/consensus-specs/releases/tag/v1.1.10): random renamed to prev\_randao, light client patches & ignores attestations voting for wrong finalized checkpoint
- Teku [v22.3.0](https://github.com/ConsenSys/teku/releases/tag/22.3.0): beacon chain explorer metrics & removes Pyrmont support
- Ben Edgington’s Upgrading Ethereum book [chapter on hash tree roots & merkleization](https://eth2book.info/altair/part2/building_blocks/merkleization)
- [Benchmarking staking clients](https://www.attestant.io/posts/evaluating-beacon-nodes-2022/) versus multi-client Vouch validator, which is considered best practice for staking services
- [Nimbus on their Insecura attack](https://our.status.im/nimbus-update-march/): understanding how weak subjectivity can be exploited via checkpoint sync & options for strengthening the defenses

**PoW switch off**

- [merge-devnet-5](https://twitter.com/parithosh_j/status/1499351263728779269) launched, Kiln v2 public testnet now launching next week
- [Join devnet-5 using Lodestar](https://github.com/ChainSafe/lodestar/pull/3821) and Geth/Nethermind with one command

**EIPs/Standards**

- [EIP4863](https://github.com/ralexstokes/EIPs/blob/5707de1597152ea6e3e4900e0e0b8cf012f90478/EIPS/eip-4863.md): Beacon chain push withdrawals
- [EIP4844](https://eips.ethereum.org/EIPS/eip-4844): Shard Blob Transactions

**Layer2**

- [Optimism to reduce fees by 30-40%](https://medium.com/ethereum-optimism/the-road-to-sub-dollar-transactions-part-2-compression-edition-6bb2890e3e92) with calldata batch compression at end of March using zlib, longer term plan to use zstd with a dictionary
- [Pathfinder](https://github.com/eqlabs/pathfinder#readme) v0.1.0: StarkNet full node in Rust, alpha
- [Arbitrum AnyTrust](https://medium.com/offchainlabs/introducing-anytrust-chains-cheaper-faster-l2-chains-with-minimal-trust-assumptions-31def59eb8d7) chains announced, ultra low cost transactions, hash of data posted on mainnet, operated by committee, assumes minimal members honest as can fallback to rollup.  [Similar trust assumptions](https://twitter.com/DZack23/status/1499827685001940997) to Validium
- Polynya: [historical storage](https://polynya.medium.com/the-endgame-bottleneck-historical-storage-e83c101d2a7c) as the final bottleneck, state growth will be solved by statelessness, validity proofs, state expiry and PBS

* * *

### **This newsletter is made possible thanks to [Celer](https://www.celer.network/)!**

![Celer](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

Celer ([new website launched!](http://celer.network/)) is a multi-chain operating system that allows the various application logic, liquidity and states, normally segregated across different chains, to communicate with one another and enables seamless inter-chain composability for dApp developers and projects.

Developers can build inter-chain-native dApps using the Celer [Inter-chain Message SDK](https://im-docs.celer.network/developer/celer-im-overview) with efficient liquidity utilization, coherent application logic, and shared states. 

Users of Celer-enabled dApps, such as the [cBridge](http://cbridge.celer.network/) asset bridge, can enjoy the benefits of a diverse multi-blockchain ecosystem with the simplicity of a single-transaction UX from a single chain.

* * *

**Stuff for developers**

- Hardhat [v2.9.0](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.9.0): faster mainnet forking, parallel testing with Mocha, parallel contract compilation & large block mining for Hardhat Network
- How [3D interactive on-chain NFT](https://mirror.xyz/angelsay.eth/Fpqj6Hawn-IWGgXm9oEYXyscIgolotYscShuNaVTmI4) was built using gITF (Graphics Language Transmission Format)
- [EVM walk through](https://noxx.substack.com/p/evm-deep-dives-the-path-to-shadowy) of opcodes using a simple storage contract
- Guide on using [Arbitrum Address registry](https://twitter.com/omw_to_the_moon/status/1497898934013997061) to reduce calldata
- TrueBlocks [beta](https://github.com/TrueBlocks/trueblocks-core/releases/tag/v0.26.2-beta): ENS support, docker version, OpenAPI based server, monitoring, index any EVM & share on IPFS and Unchained Index
- [Eth Testing](https://github.com/VGLoic/eth-testing#readme): generate mock Web3 Provider to simulate blockchain interaction in tests, alpha
- [starknet-scaffold](https://github.com/tarrencev/starknet-scaffold#readme): template using Nile and pytest
- [Rails tutorial](https://dev.to/q9/finally-authenticating-rails-users-with-metamask-3fj) to authenticate users with MetaMask
- [Optimizing Echidna fuzzer](https://blog.trailofbits.com/2022/03/02/optimizing-a-smart-contract-fuzzer/): profiling the Haskell code found bottlenecks

**Security**

- Treasure NFT marketplace [exploit](https://rekt.news/treasure-dao-rekt/), listed NFTs bought for free due to missing check for non-zero quantity
- [Sherlock CTF exploitable contracts](https://github.com/sherlock-protocol/sherlock-ctf-0x0#readme): created by 32 Secureum participants

**Ecosystem**

- Vitalik: [encapsulated vs systemic complexity](https://vitalik.ca/general/2022/02/28/complexity.html) in protocol design
- Ethereum Foundation [academic grants available](https://blog.ethereum.org/2022/03/01/academic-grants-round/) to fund formal research
- [MetaMask](https://twitter.com/metamask/status/1498730701939789831) gas UI improvements for EIP1559, opt in
- [Sign-In with Ethereum](https://blog.spruceid.com/sign-in-with-ethereum-is-a-game-changer-part-1/): unify apps with common messaging & interface 

**Enterprise**

- Harvard Business Review: [how brands should use NFTs](https://hbr.org/2022/02/how-your-brand-should-use-nfts)
- [KPMG Canada](https://home.kpmg/ca/en/home/media/press-releases/2022/02/kpmg-purchases-world-of-women-wow-non-fungible-token.html) buys World of Women NFT

**Application layer**

- 0x Protocol [v4 NFT swap support](https://twitter.com/0xproject/status/1498394341886234626) live on mainnet
- [Yield Protocol](https://medium.com/yield-protocol/yield-protocol-launches-on-arbitrum-31b6d8dd564) live on Arbitrum
- [Yearn](https://medium.com/iearn/clarifying-2020-mergers-an-independent-iron-bank-a6f8f3f4c25e) entities demerging to operate independently
- [Ribbon Finance](https://ribbonfinance.medium.com/verbn-is-live-d88a36933413) veRBN (Curve style tokenomics) live
- [ApeX Protocol](https://twitter.com/OfficialApeXdex/status/1498243202821738496) (derivatives trading) beta live on Arbitrum
- Cryptex Finance [TCAP](https://twitter.com/CryptexFinance/status/1494916428452880386) (total crypto market cap token) beta live on Optimism
- [Stratos](https://twitter.com/stratosnft/status/1499160452412047361) (NFT marketplace) live on Arbitrum, by Quixotic team
- [Always Never Yours](https://twitter.com/BeetsDAO/status/1499007738805841920) project, music NFT by Jonathan Mann, experiment with Harberger taxes

* * *

### **Job Listings**

- Mark Cuban seeks a [web3 front-end developer](https://forms.office.com/r/M81g5RNgXX). Send a work sample to apply.
- [Lead blockchain engineer / architect](https://everse.notion.site/Lead-Blockchain-Engineer-Architect-845acc3ef4c64784b19d4f2cede8161c) for a social video platform
- EF research hiring [Networking Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=54&source=weekinethnews)
- [Nomic Foundation](https://www.notion.so/Nomic-Foundation-jobs-991b37c547554f75b89a95f437fd5056) hiring Rust Tech Lead & Ethereum Tech Lead
- [Senior Technical Writer](https://ethereum.bamboohr.com/jobs/view.php?id=51&source=weekinethnews) to take ownership & completely redo the Geth docs
- Roles at Gnosis [Sr DevRel Eng.](https://grnh.se/3052a2da2us) [Sr Production/Reliability Eng.](https://grnh.se/3345ebe02us) [DevOps Eng.](https://apply.workable.com/blockscout/j/0D9C5798DC/)

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Ukraine accepting crypto](https://twitter.com/Ukraine/status/1497594592438497282) donations, announces & then [cancels airdrop](https://twitter.com/FedorovMykhailo/status/1499348177002151937) for donators, plans for NFTs instead; over [$36 million donated](https://dune.xyz/msilb7/Ukraine-Crypto-Donations)
- [Infura & OpenSea](https://www.theblockcrypto.com/post/136336/a-look-at-metamask-infura-opensea-and-the-countries-they-do-not-serve) block users in listed jurisdictions to comply with US sanctions; MetaMask can be used with your own node or any [RPC endpoint](https://ethereumnodes.com/) but uses Infura by default
- [US Treasury risk assessments](https://twitter.com/mud2monarch/status/1499067403270909954) for money laundering & terrorist financing, crypto use is in the minority compared with fiat, though expected to increase
- [BitConnect founder](https://www.justice.gov/opa/pr/bitconnect-founder-indicted-global-24-billion-cryptocurrency-scheme) indicted in US for $2.4 billion Ponzi, still at large
- MakerDAO decentralized workforce [explainer](https://twitter.com/makerdao/status/1498674457929519105)
- Norswap’s [economic analysis of Olympus DAO](https://norswap.com/olympus-econ/)
- [Musings on operating DAOs](https://www.reverie.ooo/post/musings-on-governance): reinvest treasury, require conflict reporting, accountable committee leaders, high bar for contributors, triage governance ideas, give signal to token holders and assume politics
- [Hardening Nouns treasury against threats](https://dialectic.ch/editorial/nouns-governance-attack-2): recommends implementing dynamic quorum & dynamic penalty

**General**

- Majority of [ConsenSys shareholders](https://www.prnewswire.com/news-releases/blockchain-company-consensys-faces-multi-billion-dollar-audit-as-shareholders-claim-board-breaches-fiduciary-duties---attributed-to-arthur-falls-301493433.html) request audit to investigate alleged irregularities
- [BBC News](https://www.bbc.com/news/technology-50150981) available via Tor in English, Russian & Ukrainian
- [ecGFp5](https://github.com/pornin/ecgfp5#readme): specialized elliptic curve
- [Security analysis of elliptic curves](https://eprint.iacr.org/2022/277) over sextic extension of small prime fields
- [Skiff Workspaces](https://www.skiff.org/updates/introducing-skiff-workspaces): end-to-end encrypted competitor to Google Docs

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-march-5-2022](https://weekinethereumnews.com/week-in-ethereum-news-march-5-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Mar 9-24 – [Gitcoin Grants Round 13](https://gitcoin.co/blog/announcing-grants-round-13/) (support [Week in Eth News](https://gitcoin.co/grants/2785/week-in-ethereum-news))
- **Mar 10 – [Foundry Seminar](https://twitter.com/SpearbitDAO/status/1499135064717811715)**
- **Mar 11 – [Execution Layer upgrade naming](https://github.com/ethereum/pm/issues/491) for PoW switch off**
- Mar 11-20 – [Ethereum Rio](https://www.ethereum.rio/)
- Mar 15 – [Cryptocurrency Class](https://mirror.xyz/0xaFaBa30769374EA0F971300dE79c62Bf94B464d5/oGqGP2NOK9g7QPl1sMKkzql_Fh0P6hKbpYLZ-EkQTXU) starts (virtual) 
- Mar 16 – submission deadline for [Underhanded Solidity Contest](https://underhanded.soliditylang.org/)
- Mar 17-18 – [ETH Austin](https://2022.ethaustin.org/) summit
- Mar 29-31 – [ETHDubai](https://www.ethdubaiconf.org/)
- Apr 7-9 – [ETH Portland](https://2022.ethportland.com/) hackathon
- Apr 18-25 – [Devconnect](https://devconnect.org/schedule) (Amsterdam)
- **Apr 22 – deadline for [EF academic grants round](https://esp.ethereum.foundation/academic-grants)**
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- May 3-8 – [spaghettETH](http://spaghett-eth.com/) (Milan)
- May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETHNewYork](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

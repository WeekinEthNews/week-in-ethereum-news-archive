---
title: "May 4, 2019"
date: "2019-05-04"
---

## **Ethereum News and Links**

**Layer 1**

- Latest [Eth2.0 implementers call](https://www.youtube.com/watch?v=bi7lh5Ie3x0). This week we have two different versions: Mamy’s [detailed notes](https://gist.github.com/mratsim/cc20f89f66708e8e16506502158c35f5), and NoteGarden is more [high level](https://note.garden/blog/call-summary-eth-2-0-implementers-no-17-may-2-2019/)
- Sigma Prime [Eth2 client update](https://lighthouse.sigmaprime.io/update-10.html) - BLS library standards, 25x merkle root speedup through caching
- Nimbus [Eth2 client update](https://our.status.im/nimbus-dev-update-byzantium/) - public testnet performance improvements. Pledges to get a few things ready by Devcon: cross-client production-ready phase0 testnet as well as phase1 prototype. Plus a POC light client and polished Whisper.
- [Lodestar client vision](https://medium.com/chainsafe-systems/future-vision-for-lodestar-f5b1ae66377): “browser compatible ETH2.0 client (and light client) “ to help dev tools transition to Eth2
- [Eth2 networking](https://docs.google.com/presentation/d/1S6REcV5mr5HHsOK5OvdCbbif3vzjgTrP2HdSI2XYdPc/edit#slide=id.g5136bc899d_0_723) slides from Kevin Chia
- [layer-1-minimizing phase 2 state execution proposal](https://ethresear.ch/t/a-layer-1-minimizing-phase-2-state-execution-proposal/5397)
- [Fast verification of multiple BLS signatures](https://ethresear.ch/t/fast-verification-of-multiple-bls-signatures/5407)
- Justin Drake on [VDF ASIC](https://www.reddit.com/r/ethereum/comments/bjk2tm/vdf_randomness_on_ethereum_20_is_broken/eme6xhb/?context=3)s: An “attacker needs to be 100x faster than our ASICs to break the randomness … \[even\] if 100x+ is achieved, the randomness gracefully decays to the not-too-shabby RANDAO”

**Layer 2**

- [Connext to build v2 on Counterfactual](https://medium.com/connext/towards-an-interoperable-future-f144012c857f) for interoperability
- [Counterfactual](https://medium.com/@statechannels/development-update-5-05-03-19-cf64ece3f9f6) dev update.
- [Vector Addition State Machine interpreter compatible with generalized state channels](https://ethereum-magicians.org/t/vector-addition-state-machine-interpreter-compatible-with-generalized-state-channels/3235)
- [Burner Wallet on LeapDAO/MoreViablePlasma](https://leapdao.org/blog/Popup-Economy-at-Blocksplit/)
- [LiquidityNetwork v2 mobile app](https://blog.liquidity.network/2019/05/02/liquidity-v2-mobile-app-release/) release

**Stuff for developers**

- Solidity [v0.5.8](https://github.com/ethereum/solidity/releases/tag/v0.5.8) “further completes ABIEncoderV2, SMTChecker and Yul and improves the optimizer." Also Solidity [v0.4.26](https://github.com/ethereum/solidity/releases/tag/v0.4.26) backports bugfixes for v4
- web3.js [v1.0.0-beta.54](https://github.com/ethereum/web3.js/releases/tag/v1.0.0-beta.54)
- Truffle [v5.0.15](https://github.com/trufflesuite/truffle/releases/tag/v5.0.15) and Ganache v[2.0.2-beta.0](https://github.com/trufflesuite/ganache/releases/tag/v2.0.2-beta.0)
- Alpha version of [Play](https://play.ethereum.org/editor-solidity/), a simplified Remix for beginners
- [IEEE 754 quadruple precision (128 bit) floating point](https://github.com/abdk-consulting/abdk-libraries-solidity) Solidity library
- [Fixed point math](https://medium.com/cement/fixed-point-math-in-solidity-616f4508c6e8) in Solidity library
- [ABI and RLP for the JVM](https://github.com/esaulpaugh/headlong)
- [solang](https://github.com/hyperledger-labs/solang): Solidity to wasm PoC compiler using llvm written in Rust
- GodsUnchained on [gas efficient mass NFT creation](https://blog.godsunchained.com/2019/04/28/1-million-nfts-isnt-cool/)
- How to [integrate 3Box with profiles](https://medium.com/3box/3box-builders-series-how-to-integrate-with-profiles-34078af41c47)
- [Introduction to Formality](https://medium.com/@maiavictor/introduction-to-formality-part-1-7ae5b02422ec)
- [web3 on AWSLambda](https://coderecipe.ai/architectures/57148351)
- [sbt-Ethereum](https://www.sbt-ethereum.io/). deployment and development tool for Scala tools and apps. Steve Randy Waldman explains why he built it: to [use Eth as a Petri dish for communities](https://www.interfluidity.com/v2/7153.html)
- ConsenSys [Ethereum tools portal](https://ethereum.consensys.net/ethereum-dev-portal)

**Ecosystem**

- A new [ethereum.org launched](https://blog.ethereum.org/2019/04/30/beginning-a-new-ethereum-org/) to be a portal to community resources and maintained through Github pull requests
- ENS permanent registrar is now deployed. You have [one year to migrate](https://manager.ens.domains/)
- [Metacash](https://medium.com/lamarkaz/dai-in-the-hands-of-all-8ed335879ae9): gasless (using metatransactions with CREATE2) noncustodial Dai wallet for Android, with iOS coming.
- RicMoo on CREATE2 magic: [offchain contract wallets which can be updated](https://blog.ricmoo.com/wisps-the-magical-world-of-create2-5c2177027604)

**Enterprise**

- Microsoft publishes [Azure Ethereum dev kit](https://marketplace.visualstudio.com/items?itemName=azblockchain.azure-blockchain)
- JPMorgan and Microsoft [partnership for Quorum adoption](https://news.microsoft.com/2019/05/02/j-p-morgan-and-microsoft-announce-strategic-partnership-to-drive-enterprise-adoption-of-quorum/)
- [Atomic Crosschain Transactions for Ethereum Private Sidechains](https://arxiv.org/abs/1904.12079)
- Podcast: [John Wolpert debates R3’s Richard Brown](https://www.insureblocks.com/ep-53-debate-public-vs-private-blockchains-for-enterprises-with-r3-and-consensys/)
- [Privacy in Pantheon v1.1](https://pegasys.tech/privacy-in-pantheon-how-it-works-and-why-your-enterprise-should-care/)

**Live on mainnet**

- [CDP Saver](https://cdpsaver.com/) live on mainnet. Repay and boost in one click. Auto liquidation prevention coming soon.
- [dYdX v2 is live](https://medium.com/dydxderivatives/dydx-is-live-48df862105c0) on mainnet

**Governance and Standards**

- Results for [Aragon second vote](https://blog.aragon.org/final-results-from-aragon-network-vote-2/). 3 AGPs rejected, though [one whale deciding the results](https://www.evanvanness.com/post/184616403861/aragon-vote-shows-the-perils-of-onchain-governance) illustrates some of the perils of onchain governance
- [dxDao white paper](https://github.com/gnosis/dx-daostack/blob/master/dxdao-whitepaper-v1.pdf). Scheduled to [launch May 29](https://twitter.com/gnosisPM/status/1123220961568882688).
- [ERC1973](https://github.com/ethereum/EIPs/pull/1973/files): mint and distribute tokens per block to dapp users
- [EIP1985](https://github.com/ethereum/EIPs/pull/1985/files): sane limits for EVM parameters

**Application layer**

- Secondary and tertiary [educational institutions in Singapore will issue degrees](https://www.channelnewsasia.com/news/singapore/students-graduating-tamper-resistant-digital-certificates-11499166) using [OpenCerts](https://opencerts.io/)
- [Degrees of decentralization in DeFi](https://hackernoon.com/how-decentralized-is-defi-a-framework-for-classifying-lending-protocols-90981f2c007f)
- [DeFiScan](https://medium.com/mycrypto/introducing-defiscan-io-40b8d2c3d445) - check your Compound, Uniswap and Spankchain balances from one site
- RAC, Goldroom and Ujo [launch a music label](https://www.billboard.com/biz/articles/news/digital-and-mobile/8509564/rac-and-goldroom-launch-minerva-music-a-label-that)
- Status [v0.12](https://our.status.im/0-12-0-mobile-release-introducing-discover/) - adds dapp curation through SNT staking
- Maker [Stability Fee at 19.5%](https://blog.makerdao.com/executive-vote-stability-fee-19-5/)

**Interviews, Podcasts, Videos, Talks** 

- [Rick Dudley](https://ethhub.substack.com/p/discussing-the-ethereum-roadmap-with) on Into the Ether
- [PlasmaGroup AMA](https://www.youtube.com/watch?v=5QqWB3ZMqdQ) and freestyle
- [Andrew Keys keynote](https://youtu.be/X2pJ1X2TqEw?list=PLlfzA-RvFAdwoSg38sngJohLqBgm8PavE) at Harvard Business
- Aztec’s [Zac Williamson](https://www.zeroknowledge.fm/75) on Zero Knowledge

**Tokens / Business / Regulation**

- Fidelity report arguing that [institutional money is coming to crypto](https://medium.com/@FidelityDigitalAssets/new-research-institutional-investments-likely-to-increase-over-next-5-years-729fb1ca3c52)
- [Q&A with Caitlin Long](https://media.consensys.net/what-wyomings-13-new-crypto-laws-mean-for-blockchain-in-the-us-1bcf8b7a39d4) about Wyoming’s new crypto laws
- London club [West Ham join PSG and Juventus in using Socios](https://www.whufc.com/news/articles/2019/april/30-april/west-ham-united-agree-partnership-socioscom) to issue fan tokens
- [Why Ethereum will likely emerge as the preferred platform in capital markets](https://medium.com/fluidity/the-power-of-open-networks-public-blockchain-adoption-in-capital-markets-aee6bf1b002d)

**General**

- There were rumors Facebook would launch its crypto project at F8, but it did not. WSJ had initial paywalled report. Wired reports the [possible options WSJ laid out](https://www.wired.com/story/facebooks-cryptocurrency-might-work-like-loyalty-points/).
- [Stellar crashes if just two nodes fail](https://sites.google.com/view/stellar-analysis). Both of which are run by…Stellar.
- Elon Musk tweets “[Ethereum](https://twitter.com/elonmusk/status/1123033196642201600),” which leads to back and forth with Vitalik Buterin, with Vitalik offering his thoughts on [applications best suited to Ethereum](https://twitter.com/VitalikButerin/status/1123136930177118209).

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- May 9 - [Fluidity Summit](https://www.fluiditysummit.com/) (NYC)
- May 10-11 - [Ethereal](https://etherealsummit.com/?ref=weekinethereum) (NYC)
- May 16 - [Eth2 workshop](https://www.eventbrite.com/e/road-to-interop-tickets-60384211803) (NYC)
- May 16 - [Token Summit](http://tokensummit.com/) (NYC)
- May 17-19 - [ETHNewYork](http://ethnewyork.com/)
- May 17 - Deadline to accept [proposals for Instanbul upgrade](https://en.ethereum.wiki/roadmap/istanbul) fork
- May 23-25 - [Swarm Orange Summit](https://www.eventbrite.com/e/swarm-orange-summit-madrid-2019-tickets-57378034245) (Madrid)
- **May 24-26 - [Ethereum Madrid Hackathon](https://ethereummadrid.com/hackathon-2019/)**
- May 27-28 - [EthCon Korea](https://ethcon.kr/) (Seoul)
- June 8-9 - [WASM in blockchains](https://avive.github.io/wasm_on_the_blockchain/#/) (Berlin)
- June 22-24 - [Zcon1](https://www.zfnd.org/zcon/) (Split, Croatia)
- **July 3-5 - [WindingTree’s HackTravel](https://windingtree.com/hacktravel-lisbon-2019) (Lisbon)**
- Aug 2-4 - [ETHIndia](https://ethindia.co/) (Bangalore)
- Aug 2-4 - [TruffleCon](https://www.truffleframework.com/trufflecon2019) (Redmond)
- Aug 21-23 - [Dappcon](https://dappcon.io/) (Berlin)
- Aug 23-25 - [ETHBerlin](https://ethberlinzwei.com/)
- Sep 16-17 - [Starkware sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- Oct 8-11 - [DeVcon](https://twitter.com/EFDevcon/status/1120312795902377994) (East Asia)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I own Week In Ethereum. Editorial control has always been 100% me. 

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **It’s annoying how many link to the old URL. This is the new one: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/may-4-2019/](https://weekinethereumnews.com/may-4-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

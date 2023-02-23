---
title: "Week in Ethereum News <BR> September 1, 2019"
date: "2019-09-01"
---

## **Eth News and Links**

**Eth1**

- There’s an ongoing debate as to how much Eth1 should make breaking changes. In this instance, it’s about opcode repricing which might break code deployed on the chain, even though it is a bad practice to rely on static gas pricing. Sorpaas says [no breaking changes](https://twitter.com/sorpaas/status/1167154294551994369) please, though that’s opposed to the original sustainability movement which got mislabeled "eth1x." It’s not an easy debate in a decentralized ecosystem, though we have repriced opcodes before, because that’s necessary to avoid DoS attacks.
- Swende’s [1884 security considerations](https://github.com/holiman/eip-1884-security)
- ChainSecurity’s Hubert Ritzdorf analysis of [deployed code potentially affected by EIP1884](https://gist.github.com/ritzdorf/1c6bd72955391e831f8a397d3152b4e0)
- Swende [2046 benchmarking](https://github.com/holiman/goevmlab/tree/master/examples/callPrecompiles) in Geth. 2046 reduces cost of calls to precompiles
- an [EVM backend for LLVM](https://medium.com/etclabscore/the-evm-llvm-is-coming-to-ethereum-classic-what-you-need-to-know-c13962f25571) from ETC Labs Core
- [evmone](https://github.com/ethereum/evmone): fast EVM implementation in c++
- [Péter Szilágyi](https://twitter.com/peter_szilagyi/status/1167414521935384578): “we have an experimental Geth full node weighing 139GB on #Ethereum mainnet: 94GB on HDD and 45GB on SSD. It's in sync”
- Parity [v2.6.2-beta](https://github.com/paritytech/parity-ethereum/releases/tag/v2.6.2) and [v2.5.7-stable](https://github.com/paritytech/parity-ethereum/releases/tag/v2.5.7) to fix a DoS attack of publicly exposed RPCs. Kudos to Amberdata for reporting.

**Eth2**

- Latest [What’s New in Eth2](https://notes.ethereum.org/@ChihChengLiang/Sk8Zs--CQ/https%3A%2F%2Fbenjaminion.xyz%2Fnewineth2%2F20190831.html?type=book)
- Latest [Eth2 implementers call](https://www.youtube.com/watch?v=sz87_i5Uy1I). [Mamy](https://gist.github.com/mratsim/b481ee7c598353298f111059d688be0c) and [Ben](https://docs.google.com/document/d/1jA4H6uQvPsWYrOUGFJeQWqXzP6YUq6BFKfPYAI7_y3g/edit) both took notes.
- [Nimbus client](https://our.status.im/nimbus-berlin-update/) update - working on launch mechanics and interoperability.
- [Lodestar client](https://medium.com/chainsafe-systems/lodestar-update-c456534af215) update - BLS optimization, disc v5, and Eric Tu wrote the fastest JavaScript SHA256 implementation
- Spec [v0.8.3](https://github.com/ethereum/eth2.0-specs/releases/tag/v0.8.3) came out a week ago. updates to tests and networking.
- phase 1 spec has Sep 30th target date for completeness
- Some privacy proposals: [Privacy-Preserving Casper FFG using Traceable Ring Signatures](https://ethresear.ch/t/privacy-preserving-casper-ffg-using-traceable-ring-signatures/6054) and [ZKP to remove the mapping ip address / wallet’s public key of a validator](https://ethresear.ch/t/anonymity-a-zkp-to-remove-the-mapping-ip-address-wallets-public-key-of-a-validator/6049)
- EF released a list of [Eth2 grants](https://blog.ethereum.org/2019/08/26/announcing-ethereum-foundation-and-co-funded-grants/), focused on client teams and interop/networking, as well as some R&D for light clients and also for phase1 proof of custody. There are also 3 open bounties: phase 0 consensus, [Legendre PRF](https://legendreprf.org/bounties/), and [STARK friendly hash](https://starkware.co/hash-challenge/)
- [Danny Ryan talks Eth2](https://ethhub.substack.com/p/talking-ethereum-20-with-danny-ryan) on Into the Ether
- Rocketpool’s [second beta to test out decentralized Eth2 staking pools](https://medium.com/rocket-pool/rocket-pool-2-v1-beta-launch-afc467c8195d)
- Vitalik’s list of [things that will change for app devs in Eth2](https://twitter.com/VitalikButerin/status/1167510279736967168). This is not short-term planning but things to keep in mind for the future.

**Layer 2**

- FunFair founder Jeremy Longley with a detailed walkthrough of their [state channel architecture](https://funfair.io/a-reference-implementation-of-state-channel-contracts/) and code
- “[A unified state channel specification for Ethereum](http://statechannels.org/)” to lay “the foundation for a fully interoperable ecosystem” so that building on channels is as easy as possible for app devs
- AdEx: How we built the [largest payment channel network on Ethereum](https://gist.github.com/Ivshti/29552cdf20eda21191f7c795fd46de2a). 9 million transactions with only 13k USD onchain because they trigger a payment via channel for every ad impression. 10 cents in gas paid for millions of unidirectional, one-to-many payments. A good example of programmatic micropayments made possible by state channels.
- Raiden [light client v0.1](https://github.com/raiden-network/light-client/releases/tag/v0.1)
- Vitalik: the [dawn of hybrid layer 2](https://vitalik.ca/general/2019/08/28/hybrid_layer_2.html)
- [Optimistic rollup](https://medium.com/plasma-group/ethereum-smart-contracts-in-l2-optimistic-rollup-2c1cef2ec537). Bonds/challenges to ensure valid transactions, instead of zk proofs, but easier to generalize for all applications and not just payments.

**Stuff for developers**

- Building [holographic consensus on Aragon](https://blog.aragon.one/first-aragon-app-holographic-consensus-part-2/) tutorial
- [Airscript v0.5.4](https://ethresear.ch/t/airscript-language-for-defining-zk-starks/5649/25) - performance speedups for STARKs, approaching single thread limits
- [Noble BLS12-381 pairing-friendly curve](https://github.com/paulmillr/noble-bls12-381)
- Truffle [v5.0.34](https://github.com/trufflesuite/truffle/releases/tag/v5.0.34) now supports Node12
- [Rapid dapp prototyping](https://medium.com/@austin_48503/rapid-dapp-prototyping-3823e1f565c4) with Austin Griffith
- first [Postgres extension to run WebAssembly](https://medium.com/wasmer/announcing-the-first-postgres-extension-to-run-webassembly-561af2cfcb1)
- [EthFS, a Unix-like filesystem](https://www.reddit.com/r/ethdev/comments/cxg348/introducing_ethfs_a_unixlike_filesystem_for/), check it out on testnet
- Making a [Remix plugin tutorial](https://github.com/pi0neerpat/remix-plugin-one-click-dapp/blob/master/README.md?source=post_page-----3e910070a2b1----------------------#create-your-own-remix-plugin)
- [Build a smart fridge with Streamr](https://medium.com/streamrblog/streamr-build-smart-fridge-iot-ruuvitag-node-red-ibm-cloud-fridge-d834bb6dc779), RuuviTags, Node-RED, IBM Cloud Watson Studio tutorial
- [Getting started with IPFS in Ethereum Grid](https://medium.com/ethereum-grid/getting-started-with-ipfs-in-ethereum-grid-80875cd70e6)
- [web3.js vs ethers.js](https://github.com/adrianmcli/web3-vs-ethers)
- A [code walkthrough of MolochDAO v2](https://www.youtube.com/watch?v=A6MWCBFN1Kw)
- You can now view and export Etherscan’s [verified source codes with a license](https://etherscan.io/contractsVerified?filter=opensourcelicense)
- [Vyper v0.1 beta12](https://vyper.readthedocs.io/en/v0.1.0-beta.12/release-notes.html#v0-1-0-beta-12). Also: a Kauri collection of articles on [getting started with Vyper](https://kauri.io/public-profile/9a8a9958ac1b70c49cce9693ccb0230f13f63505)

**Ecosystem**

- How to [participate in the ENS shortname auction](https://medium.com/the-ethereum-name-service/the-eth-short-name-auction-what-you-need-to-know-70ceebe24269). Starts Sep 1
- [Anonymous login using SNARKs/Semaphore](https://ethresear.ch/t/login-with-semaphore-authenticate/6034)
- Videos from the [Swarm Summit](https://www.youtube.com/channel/UCu6ywn9MTqdREuE6xuRkskA/videos)
- AZTEC’s [Ignition Ceremony](https://medium.com/aztec-protocol/aztec-announcing-our-ignition-ceremony-757850264cfe) starts in October, you can apply now to be part of it. This multi-party computation ceremony will likely get used in many future zk implementations.

**Enterprise**

- [Pantheon becomes Hyperledger Besu](https://www.hyperledger.org/blog/2019/08/29/announcing-hyperledger-besu) - the first public chain client in Hyperledger. “Besu” is Japanese for base.
- [Pantheon v1.2.2](https://pegasys.tech/solutions/pantheon/)
- EEA [telecom use cases](https://entethalliance.org/wp-content/uploads/2019/08/EEA_Telecom_Use_Cases.pdf) report (PDF)
- Oxfam, Sempo and ConsenSys in [Vanuatu for direct transfers of humanitarian aid](https://media.consensys.net/blockchain-for-social-impact-project-unblocked-cash-case-study-58a38fe23ba1) to citizens, rather than indirectly through leaky governments

**Governance and Standards**

- [EIP2253](https://ethereum-magicians.org/t/eip-2253-add-wallet-getaddressbook-json-rpc-method/3592): Add wallet\_getAddressBook JSON-RPC method
- [EIP2256](https://ethereum-magicians.org/t/eip-2256-add-wallet-getownedtokens-json-rpc-method/3600): Add wallet\_getOwnedTokens JSON-RPC method
- [EIP2250](https://ethereum-magicians.org/t/eip-2250-gas-price-range/3585): Gas Price Range
- EIPxxxx: [Web3 Login Permissions](https://ethereum-magicians.org/t/web3-login-permissions/3583). And MetaMask’s [intro to web3 permissions](https://medium.com/metamask/introducing-web3-permissions-c55b3d73563f)
- [ENS Login](https://medium.com/authereum/introducing-ens-login-25123d73e8b1): open standard for wallet integration
- Mike Goldin on the [state of DAOs in the TCR call](https://www.youtube.com/watch?v=vtdAlwNgKnw)
- [SelloutDAO](https://devpost.com/software/sellout-dao): sell your vote in any MolochDAO fork
- A proposal failed that would have given back some of the DigixDAO’s ETH, and there were [lots of unhappy people](https://twitter.com/kermankohli/status/1166563689178304519)

**Live on mainnet**

- [Erasure Protocol](https://medium.com/numerai/the-erasure-protocol-awakens-48a34cc4b5d0) live on mainnet with ErasureBay. “Open marketplace for information,” publish, create reputation, profit. Get griefed if wrong.
- [Official Star Trek collectible ships](https://www.startrek.com/news/blockchain-technology-star-trek) for sale live on mainnet. These collectible tokens will later be playable in [Lucid Sight’s game](https://csc-game.com/store)

**Application layer**

- [Dharma v2](https://blog.dharma.io/introducing-dharma-v2-now-in-beta-757b227206b) in beta, built on Compound for fixed rates with fiat on/offramps
- [PoolTogether v2](https://medium.com/pooltogether/inside-pooltogether-v2-0-e7d0e1b90a08): auto re-entry, interest is immediate, can join or leave pool at any time
- You can play the [Prisoner’s Dilemma onchain](https://cryptogame.ml/) (caveat emptor)
- [LSDai](https://devpost.com/software/lsdai): tokenized interest rate swaps
- TokenSet’s [50 day moving average](https://medium.com/set-protocol/introducing-the-eth-50-day-moving-average-set-66af12499d7d) automated trading strategy. I think these are super cool and bought a few.
- [Torque](https://medium.com/bzxnetwork/introducing-torque-borrowing-made-simple-8eb494925d16): indefinite, fixed rate loans borrowed from bZx’s Fulcrum lending pools. “Torque did not require substantial smart contract development — the tools were already there”

**Tokens / Business / Regulation**

- Synthetix: we were “dead wrong” in trying to [develop on centralized chains like EOS](https://blog.synthetix.io/cross-chain-infrastructure-revisited/) because Eth network effects are real. As Robert Leshner [notes](https://twitter.com/rleshner/status/1167621482324713472), “there are now more developers building on Compound Finance than there are developers building on either EOS or Tron.”
- Another Flippening: [Tether active addresses is multiples higher on Eth](https://coinmetrics.substack.com/p/coin-metrics-state-of-the-network-fe8) than on BTC
- [NFTs are the “hello world!” of the internet of property](https://hackernoon.com/the-internet-of-property-is-here-hello-world-j72bk3uj0)

**General**

- Three DeFi newsletters worth tracking: Ryan Sean Adams’ [Bankless](https://bankless.substack.com), Camila Russo’s [The Defiant](https://thedefiant.substack.com/), and Nodar Janashia’s [DeFi tutorials](https://defitutorials.substack.com). Moar competition.
- [ETH DKG](https://eprint.iacr.org/2019/985): distributed key generation from onchain code
- Vitalik: [quadratic voting with sortition](https://ethresear.ch/t/quadratic-voting-with-sortition/6065)
- For Week in Ethereum News’ 3 year anniversary, I did an annotated version of this week’s issue. Using [Unlock Protocol](https://unlock-protocol.com/), you can view it by purchasing a limited edition [collectible NFT for the 3rd anniversary](https://weekinethereumnews.com/three-year-anniversary-edition/). Proceeds will be donated to things within the Ethereum ecosystem.

* * *

## **🎂 3 year anniversary 🎂**

Just to repeat the advertisement immediately above: you can [buy the limited edition NFT for 0.11 Eth](https://weekinethereumnews.com/three-year-anniversary-edition/) which will unlock the annotated edition.

All proceeds will be back into Ethereum somehow, likely donated to a public good, at my discretion. And who knows, maybe there will be future benefits for the 200 NFT holders?

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Sep 1 - [ENS 3-6 character auction](https://medium.com/the-ethereum-name-service/the-eth-short-name-auction-what-you-need-to-know-70ceebe24269) starts
- Sep 2-16 - [Decentraland SDK virtual hackathon](https://hack.decentraland.org/?with=weekinethereum) (250k USD in prizes. There’s a referral code on that link that gets both you and me something extra)
- Sep 3 - Deadline to [apply for EU Horizon Prize](https://ec.europa.eu/info/funding-tenders/opportunities/portal/screen/opportunities/topic-details/blockchain-eicprize-2019). 1m € each to 5 "Blockchains for Social Good" projects
- Sep 6-8 - [ETHBoston](https://eth.boston/)
- Sep 10-11 - [DeFi Summit](https://defisumm.it/) (London)
- Sep 15 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff/)
- Sep 15 - [Ethereal Tel Aviv](https://etherealsummit.com/events/ethereal-tel-aviv/)
- Sep 16 - [Tachyon accelerator application](https://labs.consensys.net/tachyon/) deadline
- Sep 15-16- [StarkWare sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- Sep 22 - [IDEO virtual hackathon](https://coinlist.co/build/ideo) ends
- **Sep 27 - [ErasureCon](https://erasure.xxx/con) (password: information) (SF)**
- Oct 7 - [ENS workshop](https://medium.com/the-ethereum-name-service/ens-workshop-applications-are-now-open-f46db6c63384) (Osaka)
- Oct 8-11 - [DeVcon](https://devcon.org/) (Osaka) and [Devcon social events calendar](http://osaka.kickback.events/events/)
- **Oct 19-20 - [Crosslink](https://crosslink.taipei/) (Taipei)**
- Nov 8-10 - [ETHWaterloo](https://ethwaterloo.com/)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I own 100% Week In Ethereum. Editorial control has always been me.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **This headline stays as long as so many people continue to link to old URL and not the right one: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [](https://weekinethereumnews.com/week-in-ethereum-news-september-1-2019/)[https://weekinethereumnews.com/week-in-ethereum-news-september-1-2019/](https://weekinethereumnews.com/week-in-ethereum-news-september-1-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

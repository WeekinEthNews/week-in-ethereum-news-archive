---
title: "Week in Eth News <BR> October 11, 2020"
date: "2020-10-11"
---

## **Eth News and Links**

**Eth1**

- [Getting rid of RLP in binary tries](https://medium.com/@gballet/structure-of-a-binary-state-tree-part-1-48c587836d2f)
- Latest [eip1559 call](https://www.youtube.com/watch?v=SHVfypwL5W8). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1314239524810051585).
- Incubed [v3.1](https://github.com/blockchainsllc/in3-c/releases/tag/v3.1.0). ultralight client now has sentry option and new ABI encoder

**EIPs/Standards**

- [EIP3026](https://eips.ethereum.org/EIPS/eip-3026): BW6-761 curve operations
- [ERC3023:](https://github.com/ethereum/EIPs/blob/6b15a3da608cb49e271d6f7a9fe8422629bb4c0c/EIPS/eip-3023.md) Contract wallet detection
- [ERC3030](https://github.com/ethereum/EIPs/blob/cb13fd17b3a21fd889941513e09251335a7ee927/EIPS/eip-3030.md): BLS Remote Signer HTTP API

**Proof of Stake launch**

- [Proof of stake launch (“eth2”) spec v1.0.0](https://github.com/ethereum/eth2.0-specs/releases/tag/v1.0.0-rc.0), release candidate
- phase 0 [launch EIP merged](https://eips.ethereum.org/EIPS/eip-2982)
- [Formal verification of the deposit contract](https://github.com/PegaSysEng/deposit-sc-dafny) in Dafny
- [eth2 bounty program](https://eth2bounty.ethereum.org/) launched
- [A balancing attack on Gasper](https://ethresear.ch/t/a-balancing-attack-on-gasper-the-current-candidate-for-eth2s-beacon-chain/8079), a variation on Ryuya’s flipflop attack last year
- The response: add [“synchronization bottleneck” gadget](https://notes.ethereum.org/6EAsltAXSIeMHeRztEGRdg) to LMD Ghost
- [Estimate sequencer unpredictability](https://ethresear.ch/t/a-quick-script-for-estimating-how-unpredictable-the-sequencer-is-with-various-ssle-setups/8065) in secret leader election
- phase 1: [2D data availability](https://ethresear.ch/t/2d-data-availability-with-kate-commitments/8081) using Kate commitments
- [Opcode changes for swapping PoS](https://hackmd.io/XEq28xrRTsWUdLzRvAbCpg?view) in for PoW

**Layer2**

- [Curve implemented on zkSync](https://medium.com/matter-labs/curve-zksync-l2-ethereums-first-user-defined-zk-rollup-smart-contract-5a72c496b350)’s Zinc VM, live on testnet
- StarkWare: [zk-rollups more capital efficient](https://medium.com/starkware/the-optimistic-rollup-dilemma-c8fc470ca10c) than optimistic rollups due to withdrawal period
- Hermez [zk-rollup releases whitepaper](https://blog.hermez.io/the-hermez-white-paper-is-out/)
- [TheGraph will use State Channels](https://thegraph.com/blog/the-graph-brings-state-channels-to-ethereum) on mainnet

* * *

### **This newsletter is made possible thanks to [Matcha by 0x](https://matcha.xyz/?id=wien)!**

![Matcha](https://weekinethereumnews.com/wp-content/uploads/2020/06/matcha-avatar.png)

Matcha aggregates liquidity across decentralized exchange networks to offer you the best price on every token swap. [Trade 30+ DeFi tokens](https://matcha.xyz/?id=wien) on Matcha today!

* * *

**Stuff for developers**

- Solidity [v0.7.3](https://solidity.ethereum.org/2020/10/07/solidity-dynamic-array-cleanup-bug/) - dynamic array bugfix
- WalletConnect [v1.3](https://twitter.com/pedrouid/status/1314605111231086593), better mobile to desktop
- Remix [v0.10.5](https://medium.com/remix-ide/remix-0-10-5-is-released-aba6cedd161d), bring your own web3 provider (eg WalletConnect plugin), debugger connected to archive node
- [Smock](https://github.com/ethereum-optimism/smock) - mock Solidity in JavaScript
- Typechain [v2](https://github.com/ethereum-ts/TypeChain/releases/tag/typechain%402.0.1), full stack traces, fixes decoding of enums in libs
- [ENSjs](https://medium.com/the-ethereum-name-service/releasing-ensjs-and-announcing-ens-integration-workshop-63ffad001446) supports majority of ENS operations
- Vyper [v0.2.6](https://github.com/vyperlang/vyper/releases/tag/v0.2.6), includes two critical bugfixes
- Learn [Vyper tutorial, part 2](https://vyper.fun/#/2/introduction)
- Using [Nethereum and Unity](https://medium.com/coinmonks/part-2-using-nethereum-in-unity-5b09f2d8c718)
- [Getting started with Infura](https://blog.infura.io/getting-started-with-infuras-ethereum-api/) using Nodejs over websocket or https
- A [guide for noobs to Eth coding security](https://www.linumlabs.com/articles/a-brief-overview-of-why-you-should-absolutely-insist-on-audits-for-smart-contracts)
- A [honeypot contract to understand frontrunning](https://sergeypotekhin.com/detect-ethereum-front-runners/)
- 0x economist Peter Zeitz discovers [critical bug in Curve/Swerve](https://medium.com/@peter_4205/curve-vulnerability-report-a1d7630140ec) using a flashloan when the curve updates
- [Digital signatures on Ethereum](https://medium.com/mycrypto/the-magic-of-digital-signatures-on-ethereum-98fe184dc9c7), a primer
- Santi Palladino: The [state of contract upgrades](https://blog.openzeppelin.com/the-state-of-smart-contract-upgrades/)

**Ecosystem**

- MetaMask announces [more than 1 million monthly active users](https://medium.com/metamask/metamask-exceeds-1-million-monthly-active-users-9da72a1e915d) and is monetizing by adding an [aggregator of aggregators swap tab](https://consensys.net/blog/press-release/consensys-introduces-token-swaps-for-metamask/)
- Matt Leising’s [Out of the Ether](https://www.wiley.com/en-us/Out+of+the+Ether%3A+The+Amazing+Story+of+Ethereum+and+the+%2455+Million+Heist+that+Almost+Destroyed+It+All-p-9781119602934) book released
- Bloxroute benchmarks [speedup in transaction propagation](https://medium.com/bloxroute/sending-raw-transactions-fast-measuring-how-much-improvement-bloxroute-can-bring-to-node-service-20652b2afcf3) using their API
- If you [approve token spends by dodgy anon projects](https://medium.com/zengo/unicats-go-phishing-eaf39ff9da64), don’t be surprised when you lose money, _even if you get out before the rug pull_

**Application layer**

- [Endaoment](https://twitter.com/pythianism/status/1313139468568719360): donor-advised funds on Ethereum; USDC held on-chain and sent to charities as directed. Lower overhead means lower fees. Live on mainnet now.
- Streamr’s [framework to build data unions](https://blog.streamr.network/its-time-to-build-data-unions/) to sell your date collectively is live on mainnet
- Stablecoin trading still hot: [Shell Protocol](https://medium.com/shell-protocol/shell-protocol-launches-first-stablecoin-pool-f874d383d25e) is live on mainnet
- [Cofix AMM](https://medium.com/dragonfly-research/introducing-cofix-a-next-generation-amm-199aea686b6b): higher liquidity close to market price when volatility is low, using the Nest oracle
- Kyber’s moves to [adapt to market conditions](https://blog.kyber.network/kyber-continue-delivering-a-sustainable-liquidity-infrastructure-for-defi-f9945cab503)

**Regulation/business/tokens**

- the United States federal [framework for criminal crypto enforcement](https://www.justice.gov/ag/page/file/1326061/download)
- John [McAfee charged with fraud](https://www.courtlistener.com/docket/18506139/1/securities-and-exchange-commission-v-mcafee/) by the SEC
- [Why ETH is headed for 5000 USD](https://thecryptocactus.substack.com/p/my-thoughts-on-3000-ethereum)
- The [multiple personal token future](https://forefront.news/blog/feat-chris-the-multiple-personal-token-future/)

**General**

- [PLONK by hand explainer](https://research.metastate.dev/plonk-by-hand-part-1/) (link to part 1, here is link to [part 2](https://research.metastate.dev/plonk-by-hand-part-2-the-proof/))
- [ElGamal encryption, decryption, and rerandomization, with circom support](https://ethresear.ch/t/elgamal-encryption-decryption-and-rerandomization-with-circom-support/8074)
- Reason Magazine has the [first of a 4 part series on the cypherpunks](https://www.youtube.com/watch?v=YWh6Yzr12iQ)
- Brave’s new [onion service to make its sites available over TOR](https://brave.com/new-onion-service/)
- a16z [crypto startup documentary](https://www.youtube.com/watch?v=jVehCoqJgYQ)
- Bruno Maçães: Ethereum as the basis for the [evolution of the city state](https://www.city-journal.org/technological-developments-new-systems-of-governance)

* * *

## **Job Listings**

- DeFi devs! Yield is hiring for Solidity and front-end – contact@yield.is
- Live for DeFi? [mStable](https://twitter.com/mstable_) is looking for a [Smart Contract/Protocol Developer](https://cryptocurrencyjobs.co/engineering/mstable-protocol-developer-defi)
- Nori is [hiring senior engineers and UX](https://nori.com/careers) for their CO2 removal marketplace
- Variant Fund is hiring a [data-driven analyst](https://twitter.com/jessewldn/status/1314203670146420736) to join the investment team
- Dev-centric [Head of Product Marketing](https://jobs.lever.co/chainlink/611491c5-58e1-43de-a91e-65c0345cd1f0) sought for Chainlink!
- Trail of Bits hiring elite [blockchain security engineers](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & [app security](https://jobs.lever.co/trailofbits/8b7f7fc1-efb0-4e89-b406-784c3a2d77e4)
- 0x is hiring devs! [Full-stack, back-end, front-end or Solidity](https://0x.org/about/jobs)
- Celer Network: hiring Solidity and Go devs. Email: hiring@celer.network

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **🥩 Staking pool questionnaire: October 15 🥩** 

My [questionnaire for staking pools](https://docs.google.com/document/d/1wrzKXff2XwY4Bu5ynVqvlPXI4xqM4-Hwx7Jh7_-1IGg/edit) is due October 15th.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow the newsletter on twitter: [@WeekinEthNews](https://twitter.com/WeekInEthNews)

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-eth-news-october-11-2020/](https://weekinethereumnews.com/week-in-eth-news-october-11-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Oct 12 - [Zinken testnet (eth2 launch dress rehearsal](https://github.com/goerli/medalla/blob/master/zinken/README.md)). **[Launch viewing party](https://www.reddit.com/r/ethstaker/comments/j2t949/announcing_the_zinken_eth2_testnet_launch_viewing/)** 
- Oct 19-26 - [EthLagos energy hackathon](https://ethlagos.io/)
- Oct 20 - [submission deadline for Medalla data challenge](https://ethereum.org/en/eth2/get-involved/medalla-data-challenge/)
- **Oct 29 - [ETHBKK](https://pages.atato.com/ethbkk)**
- Oct 31 - [submission deadline for Underhanded Solidity Contest](https://underhanded.soliditylang.org/)
- Nov 6-7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)
- Nov 16 - [MetaMask Provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7)
- **Dec 3 - [Ethereum in the Enterprise - Asia Pacific](https://twitter.com/EntEthAlliance/status/1314652848655872000)**

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

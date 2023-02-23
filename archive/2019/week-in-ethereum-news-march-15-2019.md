---
title: "March 15, 2019"
date: "2019-03-16"
---

## **Ethereum News and Links**

**Layer 1**

- Latest issue of [what’s new in eth2](https://notes.ethereum.org/c/Sk8Zs--CQ/https%3A%2F%2Fbenjaminion.xyz%2Fnewineth2%2F20190315.html)
- Beacon chain [spec v0.5](https://github.com/ethereum/eth2.0-specs/releases/tag/v0.5.0)
- Latest [Eth2.0 implementer call](https://www.youtube.com/watch?v=zeceWlmxseY). [Agenda](https://github.com/ethereum/eth2.0-pm/issues/33) to follow along.
- [Wire protocol for Eth2](https://github.com/Whiteblock/hobbits) from Whiteblock
- [Nimbus dev update](https://our.status.im/nimbus-development-update-03/): sim progress, speed optimizations, beginnings of fork choice and a wire protocol implementation
- [Prysmatic dev update](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-24-prysmatic-labs-6d081025d47): LMD Ghost fork, e2e testing tool, Sparse Merkle trie tools for validator post activation
- [Yeeth dev update](https://medium.com/yeeth/yeeth-updates-2-52f564b53d00): libp2p implementation, BLS, spec contributions
- [Eth2 data visualizer](https://github.com/GregTheGreek/eth2.0-data-visualizer) built at EthParis
- Piper Merriam on [serialization options in Eth2](https://notes.ethereum.org/QF8jgOQbRTWUhK1zoi8D4Q#)
- protolambda’s eth2 [state transition function](https://github.com/protolambda/zrnt) in Go
- [Validator economics in Eth2](https://tokeneconomy.co/validator-economics-of-ethereum-2-0-part-2-the-ether-vacuum-418f1b32c99e), part 2
- Jacek Sieka’s [beacon chain in practice](https://twitter.com/jcksie/status/1106255441082937345?s=21) explainer
- Hsiao-Wei’s “[life of a beacon chain validator](https://docs.google.com/presentation/d/1JlQ8fVZUvt7ywRcI7mj1ExmPxcNII2xKT4lkgnkq7gU/edit#slide=id.g52948b393d_2_75)” slides

**Layer 2**

- Connext’s [DaiCard](https://medium.com/connext/introducing-the-dai-card-fc46520078d3) launches on mainnet. Instant Dai payments over state channels. Limited to $30 right now as it is still beta.
- Matter Labs is working to [implement a Sonic SNARK structure](https://medium.com/matter-labs/grant-from-the-ethereum-foundation-for-matter-labs-64338f3dd938) (ie, no trusted setup) with first benchmarks at ZK Summit in a week
- [Cryptostaw](https://medium.com/matic-network/tackling-the-adoption-issue-one-dapp-at-a-time-e756fbabfea0) - “decentralized Venmo” built on Matic Network/Plasma. Live on Kovan.
- Enuma enumerates on its [trustless exchange and SDK](https://blog.enuma.io/update/2019/03/08/trustless-noncustodial-exchange.html)
- Pisa: [Vision for Off-chain and Non-Custodial Smart Contract Networks](https://medium.com/pisa-research/vision-for-off-chain-and-non-custodial-smart-contract-networks-a2fc67e1ca73). Patrick McCorry’s survey of layer 2 and how a 3rd party watchtower helps them reach full potential.

**Stuff for developers**

- Solidity v[0.5.6](https://github.com/ethereum/solidity/releases/tag/v0.5.6)
- [OpenZeppelin v2.2](https://github.com/OpenZeppelin/openzeppelin-solidity/releases/tag/v2.2.0)
- Truffle [v5.0.8](https://github.com/trufflesuite/truffle/releases/tag/v5.0.8)
- [Buidler beta 2](https://medium.com/nomic-labs-blog/buidler-beta-2-contribute-code-and-get-paid-17925f191f95) with TypeScript support for tests and configuration
- [Solidity IDE v2](https://github.com/System-Glitch/Solidity-IDE)
- [Nodesmith](https://medium.com/nodesmith-blog/announcing-the-nodesmith-ethereum-beta-eab286d5075d): an API for Ethereum’s JSON RPC
- Tutorial: [OpenLaw API + Truffle + React.js](https://medium.com/@OpenLawOfficial/openlaw-api-tutorial-build-a-complete-dapp-with-the-openlaw-api-truffle-react-js-d064717ad41d)
- [Enjin’s SDK live on the Unity](https://blog.enjincoin.io/the-blockchain-sdk-by-enjin-is-live-on-the-unity-asset-store-a0b05f498b6e) Asset Store.
- [NFT QR dispenser](https://medium.com/coinmonks/nft-qr-dispenser-b91c88da7ee)
- TheGraph compares [GraphQL to SQL](https://medium.com/graphprotocol/graphql-will-power-the-decentralized-web-d7443a69c69a)
- How Mythril went from [simple symbolic analyzer to security platform](https://medium.com/consensys-diligence/the-tech-behind-mythx-smart-contract-security-analysis-32c849aedaef)
- Portis SDK [adds Gas Station Network](https://medium.com/@portis/sponsor-your-users-gas-fees-with-portis-and-tabookey-s-gas-stations-network-7fd7c8406869) so apps can sponsor gas fees for users
- what’s new in [iExec SDK v3](https://medium.com/iex-ec/devletter-28-sdk-upgrade-iexec-v3-c3fd158f0832)

**Ecosystem**

- [What is Burner Wallet and what is xDai?](https://settle.finance/blog/what-is-the-burner-wallet-and-whats-xdai/) explainer. Also, the Helena prediction markets platform [moved to xDai](https://media.consensys.net/prediction-markets-platform-becomes-first-dapp-on-xdai-sidechain-f26e6d691799)
- Taylor Monahan: the [impossible balance between security and usability](https://medium.com/mycrypto/the-impossible-balance-between-usability-security-55000c9fc46d)
- Kent Barton: [scaling civility](https://blog.goodaudience.com/scaling-civility-how-to-preserve-ethereums-most-crucial-strength-439e227e3091). Also: [Aya Miyaguchi’s statement](https://twitter.com/mi_ayako/status/1105909839350374400) on community values.
- Submissions from [ETHParis](https://ethparis.devpost.com/submissions) and [EthUofT](https://ethuoft2019.devpost.com/submissions). My favorite was Marius van der Wijden’s [GPU Snark](https://devpost.com/software/gpu_snarks) - 148x speedup on the Fast Fourier Transform part of the proof

**Enterprise**

- Oaken Innovations/Brisa/ViaVerde on [MOBI prizewinner Vento](https://medium.com/@projectoaken/when-will-blockchain-applications-have-a-current-valuable-and-practical-use-case-6c6550b65b4b). Tokenized euro on Ethereum/Quorum for tolling, parking, etc
- Middle East real estate developer Emaar planning to sell a token for “[full referral and loyalty system across the entire group](https://www.emaar.com/en/press-release-listing/2019/march/emaar-engages-blockchain-industry-veteran-lykke-ag)”
- [Air cargo billing, costing and reconciliation system](https://news.microsoft.com/en-sg/2019/03/13/cargo-community-network-partners-with-microsoft-to-launch-the-worlds-first-blockchain-air-cargo-billing-costing-and-reconciliation-system/?ocid=AID725565_TWITTER_oo_spl100000480864708). Article doesn’t say but since blockchain = Ethereum, it was [built on Ethereum](https://twitter.com/DavidBurela/status/1105967661085650944)

**Governance and Standards**

- Latest [core developers call](https://www.youtube.com/watch?v=GQ0kbH0iSfI). [Agenda](https://github.com/ethereum/pm/issues/83) to follow along.
- r/ethereum is going through some [governance growing pains](https://www.reddit.com/r/ethereum/comments/azyqdu/a_statement_call_for_discussion_from_some_of_the/eib1ar2/)
- Loredana: [Implementing a Layer 2 voting mechanism with noncustodial onboarding](https://medium.com/@loredana.cirstea/implementing-a-layer-2-decentralized-voting-mechanism-on-ethereum-with-noncustodial-onboarding-a7c7d26db241)
- [EIP1155 is in last call](http://eips.ethereum.org/EIPS/eip-1155)
- [ERC1843](https://github.com/ethereum/EIPs/issues/1843): Claims token standard
- [ERC1844](https://eips.ethereum.org/EIPS/eip-1844): ENS interface discovery
- [EIP1829](https://github.com/ethereum/EIPs/pull/1829/files): Ecmul precompile

**Application layer**

- The 2019 season of [Major League Crypto Baseball](https://medium.com/mlb-crypto-baseball/batter-up-mlbc-2019-is-coming-ee2b9d13f051): player performance will influence how often the player is minted. They’re also moving everyday gameplay actions offchain.
- Veil now lets you [create your own markets](https://medium.com/veil-blog/create-your-own-prediction-market-d41ec7c19675)
- Melon: [goodbye Melonport, hello world](https://medium.com/melonport-blog/goodbye-melonport-hello-world-a64b5d116b13)
- [Spankchain 2019 plans](https://medium.com/spankchain/spank-to-the-future-our-updated-roadmap-402f319e5c56): private shows, international models, accepting credit cards, video purchasing.

**Interviews, Podcasts, Videos, Talks** 

- Eth1 leader [Alexey Akhunov](https://podcast.ethhub.io/ethereum-1x-ensuring-the-future-sustainability-of-ethereum-with-alexey-akhunov) on Into the Ether
- Kyber’s [Loi Luu](https://blog.enigma.co/decentralize-this-episode-22-loi-luu-efa2c337ca05) on Decentralize This
- Uniswap’s [Hayden Adams](https://unchainedpodcast.com/how-uniswap-quickly-became-one-of-the-most-popular-dexes/) with Laura Shin
- KZen’s [Omer Shlomovits](https://thebitcoinpodcast.com/hashing-it-out-38/) on Hashing It Out
- Skale Network’s [Stan Kladko](https://www.youtube.com/watch?v=XwqmnaPHsX8) on NEAR’s Whiteboard Series
- MolochDAO’s [Ameen Soleimani](https://medium.com/pov-crypto/pov-crypto-episode-34-rise-of-moloch-ethereum-2-0-c3e6cf54087e) on POV Crypto
- Truffle’s [Tim Coulter](http://www.se-radio.net/2019/02/se-radio-episode-356-tim-coulter-on-smart-contracts/) on Software Engineering Radio
- All the [EthCC talks](https://www.reddit.com/r/ethereum/comments/azm61n/all_videos_from_ethcc_19_in_paris/)
- Vitalik Buterin “[scalable blockchains as data layers](https://www.youtube.com/watch?v=mOm47gBMfg8&feature=youtu.be)” from Taipei meetup

**Tokens / Business / Regulation**

- SEC Chairman Clayton [agrees with Hinman’s statement](https://coincenter.org/files/2019-03/clayton-token-response.pdf) outlining why Eth is not a security
- House Republican Leader Kevin McCarthy calls for US [Congressional transparency using blockchain](https://www.republicanleader.gov/blockchain-can-make-our-government-more-efficient-transparent-and-secure/)
- Samani: value capture in [base chains and applications](https://multicoin.capital/2019/03/14/on-value-capture-at-layers-1-and-2/)
- Fred Wilson on [Decentralized Finance](https://avc.com/2019/03/decentralized-finance/), though he only got into the basics of DeFi activity.
- Interesting analysis of [LAND markets](https://tokeneconomy.co/decentraland-lords-9953d0de1e5c) in Decentraland
- [Short selling in bonding curves](https://blog.oceanprotocol.com/enabling-short-selling-in-bonding-curves-part-2-4d9da68324fb)

**General**

- Joe Lubin: in 2 years, [Ethereum will handle millions of transactions per second](https://media.consensys.net/joe-lubin-at-sxsw-ethereum-will-handle-millions-of-transactions-per-second-within-two-years-699268985227)
- Gitcoin is doing another [$50,000 grant matching program](https://medium.com/gitcoin/gitcoin-grants-50k-open-source-fund-e20e09dc2110)
- Starkware: [Arithmetization II](https://medium.com/starkware/arithmetization-ii-403c3b3f4355)
- Trustlines Network is rebooting as a [proof of stake sidechain to Ethereum](https://medium.com/trustlines-protocol/introducing-the-trustlines-blockchain-682abe31e022)
- [Mainnet hub of Cosmos](https://blog.cosmos.network/blastoff-the-cosmos-hub-mainnet-is-live-41a7c749e0d0) launches
- Omise’s [Go.exchange](https://trade.go.exchange/) soft launched
- MyEtherWallet launches [EthVM](https://ropsten.ethvm.com/) block explorer. Ropsten only at the moment.
- “[Hunting Huobi scams](https://medium.com/mycrypto/hunting-huobi-scams-662256d76720)” Harry’s writeups of phishing attacks are always interesting

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Mar 22 - [Zero Knowledge Summit 0x03](https://www.zeroknowledge.fm/summit) (Berlin)
- Mar 27 - Infura [end of legacy key support](https://blog.infura.io/infura-dashboard-update-9f02d0643eb3) 
- April 4-5 - [Deconomy](https://deconomy.com/seoul2019/) (Seoul)
- April 8-14 - [Edcon](https://www.edcon.io/) hackathon and conference (Sydney)
- Apr 19-21 - [ETHCapetown](http://ethcapetown.com/)
- Apr 29 - [Oslo Blockchain Day](https://osloblockchainday.no/)
- May 9 - [Fluidity Summit](https://www.fluiditysummit.com/) (NYC)
- May 10-11 - [Ethereal](https://etherealsummit.com/?ref=weekinethereum) (NYC)
- May 16 - [Token Summit](http://tokensummit.com/) (NYC)
- May 17-19 - [ETHNewYork](https://medium.com/ethglobal/ethglobal-2019-updates-get-your-calendars-ready-1977e9315aee)
- May 17 - Deadline to accept [proposals for Instanbul upgrade](https://en.ethereum.wiki/roadmap/istanbul) fork
- May 23-25 - [Swarm Orange Summit](https://www.eventbrite.com/e/swarm-orange-summit-madrid-2019-tickets-57378034245) (Madrid)
- June 22-24 - [Zcon1](https://www.zfnd.org/zcon/) (Split, Croatia)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)

  
I own Week In Ethereum. Editorial control has always been 100% me. 

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **Update links to new URL: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/march-15-2019/](https://weekinethereumnews.com/march-15-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

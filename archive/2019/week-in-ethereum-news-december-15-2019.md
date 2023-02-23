---
title: "Week in Eth News <BR> December 15, 2019"
date: "2019-12-15"
---

## **Eth News and Links**

**Eth1**

- Latest [core devs call](https://www.youtube.com/watch?v=HpoBvMylPfk&feature=youtu.be). [Notes](https://twitter.com/TimBeiko/status/1205483535513137157). Lots of EIP1559 (fee market change) discussion now that it has been implemented. Decided to go forward with EIP2384 for Muir Glacier, anyone can propose changes afterwards. Also lots of talk about 1962 precompile calls.
- Update your clients for the Muir Glacier fork in early January. Geth, Nethermind, Besu all are ready. Parity, Aleth are coming.
- Piper Merriam on the [4 steps to an eth1 stateless client network](https://www.reddit.com/r/ethereum/comments/e8ujfy/are_stateless_clients_a_dead_end/faf9a6x/?context=3)
- Background on [eth1 very long-term sustainability problems and options](https://blog.ethereum.org/2019/12/10/eth1x-files-fast-sync/)

**Eth2**

- [Lighthouse public testnet](https://lighthouse.sigmaprime.io/update-19.html), v0.1, the “first with a mainnet configuration”
- phase 0 [spec v0.9.3](https://github.com/ethereum/eth2.0-specs/releases/tag/v0.9.3)
- Notes from the last [light client call](https://medium.com/chainsafe-systems/light-client-task-force-call-2-bdb3d24d2b2b)
- [Undertanding eth2 staking deposits](https://www.attestant.io/posts/understanding-ethereum-staking-deposits/)
- Aditya Asgaonkar [explores cross shard communication](https://www.adiasg.me/2019/12/14/exploring-cross-shard-communication-in-eth2-0.html)
- _Editorial note: ignore any fake news about launch date changing._

**Layer2**

- [Celer light client SDK](https://medium.com/celer-network/introducing-the-celer-light-client-sdk-d5c3498fa6b), runs in the browser

**Stuff for developers**

- Solidity [v0.5.14](https://github.com/ethereum/solidity/releases/tag/v0.5.14), defaults to Istanbul, SMT/ewasm updates
- Remix IDE [v0.9.2](https://medium.com/remix-ide/remix-ide-v0-9-2-release-893a71b25740)
- Ethcode [v0.8](https://github.com/quantanet/ethcode/releases/tag/v0.0.8), now supports Vyper. available in VScode
- [Deep dive into eip1167 minimal proxy contract](https://blog.openzeppelin.com/deep-dive-into-the-minimal-proxy-contract/)
- 0age: [the more minimal proxy](https://medium.com/coinmonks/the-more-minimal-proxy-5756ae08ee48)
- [Automated deploy to ENS and IPFS](https://medium.com/@triplespeeder/automated-deploy-to-ipfs-and-ens-12bae2f40302)
- Steve Marx: [destroying the indestructible registry](https://diligence.consensys.net/blog/2019/12/destroying-the-indestructible/)
- Blocknative’s [onboard.js](https://blog.blocknative.com/blog/onboard-js) to easily support many wallets
- Runtime Verification: [K vs Coq as language verification frameworks](https://runtimeverification.com/blog/k-vs-coq-as-language-verification-frameworks-part-1-of-3/)  
    

**Ecosystem**

- Can Ethereum rollups beat Visa’s 2000 transactions per second? Iden3’s analysis of post-Istanbul [Ethereum throughput limits with rollup](https://iden3.io/post/istanbul-zkrollup-ethereum-throughput-limits-analysis).
- How [Infura manages nodes with VIPnode](https://blog.infura.io/how-infura-uses-vipnode-to-manage-ethereum-nodes-972cf2acc0f0)
- Parity’s [update on grant progress](https://www.parity.io/an-update-on-paritys-ethereum-foundation-grant-progress/): 75% of grant paid based on milestones
- Networking: [Waku spec v0.2](https://forum.vac.dev/t/waku-project-and-progress/24/3) and Whiteblock’s [no tag back gossiping](https://medium.com/whiteblock/no-tag-back-gossiping-c8b99906e891)

**Enterprise**

- Nike files a [patent application for tokenized shoes on Ethereum](http://patft.uspto.gov/netacgi/nph-Parser?Sect1=PTO2&Sect2=HITOFF&p=1&u=%2Fnetahtml%2FPTO%2Fsearch-bool.html&r=1&f=G&l=50&co1=AND&d=PTXT&s1=Nike&s2=Crypto&OS=Nike+AND+Crypto&RS=Nike+AND+Crypto) and breeding them, a la Cryptokitties
- BancoSantander repurchased and cancelled the bond mainnet, of September 10th, 2019 issuance date. “[This unequivocally proves that a debt security can be managed through its full lifecycle on a blockchain](https://twitter.com/_JohnWhelan/status/1204342309040644096)”
- “[Seize the day: public blockchain is on the horizon](https://assets.ey.com/content/dam/ey-sites/ey-com/en_gl/topics/blockchain/ey-public-blockchain-opportunity-snapshot.pdf)” Forrester/EY enterprise survey says 75% will use public chains (read: Ethereum) in the future
- Paul Brody op-ed: [If you build a blockchain, will anyone come?](https://www.theblockcrypto.com/post/50065/if-you-build-a-blockchain-will-anyone-come) “Public blockchains like Ethereum offer a better choice for enterprise users”
- [Quorum plugin for Remix](https://medium.com/remix-ide/quorum-plugin-for-remix-ee232ebca64c)
- Hyperledger Besu [v1.3.7](https://github.com/hyperledger/besu/releases/tag/1.3.7) - critical fix for mainnet users, muir glacier compatible

**Governance and standards**

- [Extending MolochDAO’s features](https://medium.com/@thelaoofficial/the-lao-joins-forces-with-moloch-dao-and-metacartel-to-begin-to-standardize-dao-related-smart-b6ee4b0db071): TheLAO, Moloch and MetaCartel to standardize for venture-style investments and accommodation of security token standard
- Maker’s [governance security module puts a 24 hour delay](https://blog.makerdao.com/governance-security-module-gsm/) on all governance decisions. This was in response to Micah Zoltu’s “[how to turn 20m into 340m in 15 seconds](https://medium.com/@MicahZoltu/how-to-turn-20m-into-340m-in-15-seconds-48d161a42311).” The 0 delay was explicitly a tradeoff as MCD launched to ensure that Maker could respond nimbly to any problems.
- [Vocdoni](https://twitter.com/vocdoni/status/1204667203255177216): an app for anonymous, onchain voting

**Application layer**

- [Sablier is live on mainnet](https://twitter.com/SablierHQ/status/1205533344886411264), continuous streaming money
- [Synthetix inflation changed](https://blog.synthetix.io/the-capella-release/) to exponential decay in the inflation rate with a 2.5% terminal rate
- Set Protocol integrates [Compound’s cTokens so sets earn interest](https://medium.com/set-protocol/introducing-ctokens-on-tokensets-e08bc3b4e05c)
- RealT’s [first property sells out](https://www.reddit.com/r/ethfinance/comments/ea8suo/the_first_property_ever_to_be_tokenized_on/)
- [Undercollateralized lending](https://twitter.com/AlexMasmej/status/1204354944301707265) as next DeFi trend?
- [Kong.cash releases their whitepaper](https://www.reddit.com/r/ethereum/comments/e8zz2g/kong_physical_cryptocurrency/). As seen at Devcon, Kong is physical crypto cash

**Tokens / Business / Regulation**

- [SEC charges fraudulent ICO](https://www.sec.gov/news/press-release/2019-259)
- Saga goes live on mainnet with an [algorithmic version of the IMF’s SDR](https://www.finextra.com/newsarticle/34932/saga-launches-global-stabilised-digital-currency)
- ING is planning to [get into crypto custody](https://www.reuters.com/article/us-crypto-currencies-ing-exclusive-idUSKBN1YF2GN)
- ConsenSys Activate’s [standards for token launches](https://codefi.consensys.net/blog/activate-token-launch-standards)  
    

**General**

- [Speeding up verification of groth16 batches](https://eprint.iacr.org/2019/1177.pdf)
- [Simple explanation of circuits and zero knowledge proofs](https://medium.com/web3studio/simple-explanations-of-arithmetic-circuits-and-zero-knowledge-proofs-806e59a79785)
- A [comprehensive primer on recursive SNARKs](https://www.michaelstraka.com/posts/recursivesnarks/)
- “[design a circuit construction protocol](https://twitter.com/KaiGellert/status/1204344110037053442) (such as used in TOR) that is 1) non-interactive, 2) immediate forward-secret, and 3) requires only O(n) message exchanges”
- [Filecoin launches testnet](https://filecoin.io/blog/filecoin-testnet-mining/)
- Using [reinforcement learning to model selfish mining incentives](https://pegasys.tech/reinforcement-learning/)
- Will [quantum supremacy affect blockchain](https://consensys.net/blog/blockchain-development/how-will-quantum-supremacy-affect-blockchain/)?

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Jan 1 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff-update/)
- Jan 1-30 - [EthIndia online hackathon](https://online.ethindia.co/)
- Jan 6-20 - Gitcoin [take back the web online hackathon](https://gitcoin.co/hackathon/take-back-the-web/?)
- Jan ~4 - [Muir Glacier upgrade](https://ethernodes.org/muir_glacier) to delay difficulty increase
- Jan 31 - deadline for [EU ledger 200k euro grants](https://fundingbox.com/spaces/ledger-ledger-news-and-updates/5dbfcb7d52317832f85906c8) for blockchain startups
- Feb 14-16 - [ETHDenver](https://www.ethdenver.com/)
- Mar 3-5 - [EthCC](https://ethcc.io/) (Paris)
- Mar 29-Apr4 - [EthLagos](https://ethlagos.io/)
- Apr 3-7 - [Edcon](https://www.edcon.io/) (Vienna)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

It’s amazing to me how many people email me when every issue has a link at the bottom saying not to email me to get in the newsletter.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **I want your links, because Google needs help: [weekinethereumnews.com](https://weekinethereumnews.com/)**

Archive on the web if you’re linking to it:  [https://weekinethereumnews.com/week-in-eth-news-december-15-2019/](https://weekinethereumnews.com/week-in-eth-news-december-15-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

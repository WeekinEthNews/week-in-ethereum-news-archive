---
title: "Week in Ethereum News <BR> September 15, 2019"
date: "2019-09-15"
---

## **Eth News and Links**

**Eth1**

- Trinity [v0.1.0-alpha.28](https://github.com/ethereum/trinity/releases/tag/v0.1.0-alpha.28) - get synced in an hour with BeamSync
- [EthereumJS VM v4.1](https://www.reddit.com/r/ethereum/comments/d365tk/ethereumjs_vm_v41_with_fullfeatured_istanbul/), ready for the Istanbul upgrade
- [ProgPoW hardware audit by Bob Rao](https://medium.com/ethereum-cat-herders/progpow-audits-released-ed4973ebe073) after the Least Authority software audit released the previous week. Unclear what next steps are.

**Eth2**

- **Interop week is over, but the results are spectacular: [seven Eth2 clients talking to each other](https://twitter.com/JonnyRhea/status/1172233598109442049).** This was the last major hurdle before clients focus on optimizations, auditing, and UX in preparation for launch.
- Nimbus has a mostly [pre-interop client update](https://our.status.im/nimbus-status-update-pre-interop/): exit mechanics, better monitoring, and Nimplay - a nim DSL for Ethereum.

**Stuff for developers**

- [Patterns to fight front-running](https://forum.openzeppelin.com/t/protecting-against-front-running-and-transaction-reordering/1314)
- [Factory contracts improve security](https://diligence.consensys.net/posts/2019/09/factories-improve-smart-contract-security/)
- Airswap quickly found a [vulnerability in deployed mainnet code](https://medium.com/fluidity/critical-vulnerability-in-a-new-airswap-smart-contract-c1204e04d7d3), 10 addresses affected that need to revoke authorizations.
- [VSCode plugin for Surya’s interactive call graphs](https://marketplace.visualstudio.com/items?itemName=tintinweb.solidity-visual-auditor)
- Truffle [v5.0.36](https://github.com/trufflesuite/truffle/releases/tag/v5.0.36) - better stack trace
- Drizzle [v1.5](https://www.trufflesuite.com/blog/drizzle-150-a-new-beginning) - new monorepo and Vue plugin
- Interact with [mainnet contracts in Ganache](https://medium.com/@sambrichards/how-to-interact-with-ethereums-mainnet-in-a-development-environment-with-ganache-3d8649df0876)
- How Melon set up a [monitoring tool with The Graph](https://medium.com/melonprotocol/graphing-the-melon-protocol-fdcbbc0475b5)
- [Graphene v1](https://blog.golemproject.net/graphene-v1-0-has-been-released/) to use Intel SGX from Linux
- [decentralized Solidity source code verification](https://github.com/ethereum/source-verify/blob/master/verify.js)
- [Dedicated IPFS networks](https://medium.com/pinata/dedicated-ipfs-networks-c692d53f938d)
- POA Network’s [TokenBridge adds arbitrary message relaying](https://forum.poa.network/t/tokenbridge-contracts-3-0-0-release/3013)
- Loredana [demo on dTyped Solidity](https://youtu.be/pBsual6FogE)
- [Tranquility](https://medium.com/ethworks/tranquility-a-better-smart-contract-programming-language-3038678ba34d): what Ethworks wants and is planning for a new Eth language
- An [update on Formality](https://www.reddit.com/r/haskell/comments/d2gcyw/just_letting_you_know_that_formality_has_evolved/), it is now “usable... ish,” compiler planned by the end of the year.

**Ecosystem**

- A writeup of the [ZeroPool zk anon multi-asset pool](https://ethresear.ch/t/zeropool-explanation/6122) from EthBoston
- [Perpetual Powers of Tau](https://medium.com/@weijiek/announcing-the-perpetual-powers-of-tau-ceremony-to-benefit-all-zk-snark-projects-c3da86af8377) ceremony
- [Swarm monthly update](https://medium.com/ethereum-swarm/ethereum-swarm-team-newsletter-august-2019-f49adc376318) - now supports bandwidth incentivization
- [3Box Followers](https://medium.com/3box/3box-followers-your-open-social-graph-1f5e42c50afd) - an open web3 social graph
- An update on [Universal Login](https://medium.com/universal-ethereum/universal-login-explained-the-easiest-way-to-on-board-users-to-your-dapp-8a297d8915d0) with Avsa demo
- Gas limit is creeping up as a community campaign to convince miners to raise the limit appears to have succeeded. It’s got up to almost 8.4m but is at 8.2x as I type, but gas prices haven’t budged (no link)

**Enterprise**

- [Banco Santander with the first end-to-end on-chain $20m bond](https://www.santander.com/csgs/Satellite/CFWCSancomQP01/en_GB/Corporate/Press-room/2019/09/12/Santander-launches-the-first-end-to-end-blockchain-bond.html) and John Whelan’s thoughts on the [future of security tokens](https://twitter.com/_JohnWhelan/status/1172842724686516230)
- [Joe Lubin joins Hyperledger governing board](https://www.hyperledger.org/announcements/2019/09/11/consensys-joins-hyperledger-as-a-premier-member).
- Voting isn’t just a problem in onchain governance: low turnout leads to [IBM holding a majority of Hyperledger’s technical steering committee](https://www.coindesk.com/ibm-now-holds-6-of-11-seats-on-hyperledgers-steering-board)
- Hyperledger Besu [v1.2.3](https://pegasys.tech/solutions/hyperledger-besu/) (formerly known as Pantheon)

**Standards and governance topics**

- [ERC2269](https://github.com/ethereum/EIPs/issues/2269): fiat representation standard
- [ERC2270](https://github.com/ethereum/EIPs/issues/2270): generate Ethereum accounts from digital ID

**Application layer**

- [Augur v1 cutoff changed to Jan 1](https://www.augur.net/blog/v1-cutoff-update/), contingent on a progressively increased Initial Reporter stake
- Gnosis’ [Sight prediction market](https://twitter.com/koeppelmann/status/1172162269893025794) is in beta
- Set launches a [12 day exponential moving average](https://medium.com/set-protocol/introducing-exponential-moving-averages-on-tokensets-ada559ad2b9d) play
- [Status v0.13.2 iOS hotfix](https://our.status.im/breaking-changes-ahead-v1-is-coming-hot-fix-0-13-2/) ahead of a v1 release in q4. v1 is a breaking change that requires deleting the beta versions, so backup your key!
- Kyber adds a [fiat onramp using Coindirect](https://medium.com/kyberswap/buy-crypto-with-fiat-at-kyberswap-372e41865b09)
- [Completely decentralized marketplace](https://diazgonewild.com/doc/mad_stores_whitepaper-v090.pdf) using Turms Message Transport
- Avantgarde to take the lead [developing Melon protocol](https://medium.com/avantgardefinance/welcome-to-avantgarde-f-69122178d466) in exchange for MLN
- An opus on [Mattereum’s vision](https://medium.com/humanizing-the-singularity/how-post-industrial-capitalism-and-a-new-type-of-big-data-will-save-the-planet-6574b1d75bf6)
- UMA’s [synthetic token builder](https://medium.com/uma-project/announcing-the-uma-synthetic-token-builder-8bf37c645e94) is live on Rinkeby testnet.
- [Dai Savings Rate in multi-collateral Dai](https://blog.makerdao.com/an-update-on-the-dai-savings-rate-in-multi-collateral-dai/)
- dydx adds a [native ETH/DAI market](https://medium.com/dydxderivatives/dydx-launches-native-eth-dai-market-30ced19701ae)
- Dai Stability Fee [down to 12.5%](https://twitter.com/nanexcool/status/1172955126627282945)
- A [catalog of the many flavors of Dai](https://github.com/jordanlyall/dai-universe). Like EthBoston’s [SwanDAI](https://twitter.com/willprice221/status/1171088964486389762?) - black swan exposure through synthetics using UMA
- Move your funds from [Dharma v1 to v2](https://blog.dharma.io/how-to-move-your-funds-to-dharma-v2-52666b2907cf)
- [Aragon v0.8](https://blog.aragon.org/aragon-0-8-camino/) - improved setup flow, new design, email subscriptions for votes

**Tokens / Business / Regulation**

- The Tether Flippening draws nigh: [300m USDT moved from Bitcoin to Ether](https://twitter.com/Tether_to/status/1172031965090000896)
- Seychelles national stock exchange does an [IPO of its equity using a security token](https://www.coindesk.com/first-tokenized-ipo-launches-on-national-stock-exchange). On Eth, of course.
- Sparkle, a “[redistributive currency](https://medium.com/@MicahWhite/if-occupy-created-bitcoin-cceda9e7c246),” although paying 3% upfront means you need “[about 3x your investment to be contributed before recouping your original contribution](https://medium.com/@danfinlay/review-of-the-sparkle-token-by-occupy-co-founder-micah-white-e1e32167d6cb)”
- Mougayar: [Ethereum and the Chinese Bamboo Tree](http://startupmanagement.org/2019/09/14/why-ethereums-churn-is-normal-and-the-chinese-bamboo-tree-analogy/). It’s growing like crazy, just some people can’t see it yet.
- France and Germany joint statement saying [they’ll block Facebook’s Libra](https://www.reuters.com/article/us-facebook-cryptocurrency-france-german-idUSKCN1VY1XU)
- [OpenSea’s ERC1155 token marketplace](https://medium.com/opensea/now-open-erc-1155-marketplace-816257ab0da7) is open

**General**

- ZCash/ECC’s Sean Bowe discovers [HALO](https://electriccoin.co/blog/halo-recursive-proof-composition-without-a-trusted-setup/): zk proofs with no trusted setup
- StarkWare’s [STARK-friendly hash challenges](https://twitter.com/EliBenSasson/status/1172024878398136320) is live
- Matter Labs’ IACR paper: [Transparent Polynomial Commitment Scheme with Polylogarithmic Communication Complexity](https://eprint.iacr.org/2019/1020)
- Full documentary of Bounties Network’s [Bounty for Basura](https://www.youtube.com/watch?v=7S9uxDRJAdo) (13m)
- [Gemini now offers custody](https://medium.com/gemini/introducing-gemini-custody-936c77977de1) for funds and institutions
- For the 3rd straight week, I did an annotated version of the newsletter. Anyone who has bought the NFT can read it. Same link, you can still buy the NFT. (and you can also use [Unlock’s Wordpress plugin](https://unlock-protocol.com/blog/wordpress-plugin/) to easily sell your own) See immediately below:

* * *

## **🎂 3 year anniversary 🎂**

Just to repeat the advertisement immediately above: you can [buy the limited edition NFT for 0.11 Eth](https://weekinethereumnews.com/three-year-anniversary-edition/) which will unlock the annotated edition.

All proceeds will be back into Ethereum somehow, likely donated to a public good, at my discretion.

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Sep 16 - [Tachyon accelerator application](https://labs.consensys.net/tachyon/) deadline
- **Sep 16-30 [Gitcoin CLR matching](https://gitcoin.co/blog/gitcoins-q3-match-100k-to-oss-projects/)**
- **Sep 16-30 [Decentraland GameJam](https://gamejam.decentraland.org/?with=weekinethereum) hackathon**
- **Sep 16-27 [Graph virtual hackathon](https://thegraph.com/hackathon)**
- **Sep 23-Oct 6 - [Road to Devcon](https://hackathons.gitcoin.co/the-road-to-devcon/) virtual hackathon**
- Sep 27 - [ErasureCon](https://erasure.xxx/con) (password: information) (SF)
- **Oct 5-6 - [Cryptoeconomics System Summit](https://cryptoresearch.pubpub.org/) (Boston)**
- Oct 7 - [ENS workshop](https://medium.com/the-ethereum-name-service/ens-workshop-applications-are-now-open-f46db6c63384) (Osaka)
- Oct 8-11 - [Devcon](https://devcon.org/) (Osaka) and [Devcon social events calendar](http://osaka.kickback.events/events/)
- Oct 19-20 - [Crosslink](https://crosslink.taipei/) (Taipei)
- Nov 5-6 - [Decentralized insurance D1Conf](https://blog.etherisc.com/d1conf-2019-to-focus-on-blockchain-adoption-november-5-6th-in-malta-3b8b582ac7b4) (Malta)
- Nov 8-10 - [ETHWaterloo](https://ethwaterloo.com/)
- **Jan 1 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff-update/)**

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

It’s amazing to me how many people email me when every issue has a link at the bottom saying not to email me to get in the newsletter.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **This headline stays as long as so many people continue to link to old URL and not the right one: [weekinethereumnews.com](https://weekinethereumnews.com/)**

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/week-in-ethereum-news-september-15-2019/](https://weekinethereumnews.com/week-in-ethereum-news-september-15-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

---
title: "February 22, 2019"
date: "2019-02-24"
---

## Ethereum News and Links

**Constantinople upgrade fork this week**

- Constantinople’s network upgrade is scheduled to happen around Feb 28th at block 7280000. Update your clients so you don’t get left behind. Here’s the [Foundation’s FAQ](https://blog.ethereum.org/2019/02/22/ethereum-constantinople-st-petersburg-upgrade-announcement/) if you’re curious about what this means for you. The link also has links to the most recent client versions.

**Layer 1**

- \[eth1\] [part 4](https://medium.com/@akhounov/looking-back-at-the-ethereum-1x-workshop-26-28-01-2019-part-4-a69b48e14309), [part 5](https://medium.com/@akhounov/looking-back-at-the-ethereum-1x-workshop-26-28-01-2019-part-5-24ee8a9cbc40) and [part 6](https://medium.com/@akhounov/looking-back-at-the-ethereum-1x-workshop-26-28-01-2019-final-part-6-988134a36073) of Alexey’s eth1 workshop retrospective. Click part 6 for an overview of each different part to understand what was discussed at the eth1 workshop.
- \[eth1\] [Ewasm 1.x precompiles](https://medium.com/@gballet/ewasm-1-x-precompiles-part-1-66ee7e7345d1), part 1
- \[eth2\] Buterin: [Maximally simple account abstraction without gas refunds](https://ethresear.ch/t/maximally-simple-account-abstraction-without-gas-refunds/5007)

**ZK/privacy**

- [Zether and Sigmabullets](https://crypto.stanford.edu/~buenz/papers/zether.pdf) for confidential/anonymous transactions. 7m gas now, but could be lowered to 1.7m with EIP1108 and 1109. Paper by Bünz, Agrawal, Zamani and Boneh.
- Starkware on [STARK math, pt2](https://medium.com/starkware/arithmetization-i-15c046390862)
- Barry WhiteHat: [Semaphore](https://ethresear.ch/t/semaphore-rln-rate-limiting-nullifier-for-spam-prevention-in-anonymous-p2p-setting/5009), rate limiting with SNARKs to fight spam
- [Zero knowledge proofs using bulletproofs](https://medium.com/@loveshharchandani/zero-knowledge-proofs-using-bulletproofs-4a8e2579fc82)
- WASM-compatible [Miximus in Rust](https://github.com/drewstone/rust-miximus) POC

**Plasma and sidechains**

- [Staking for Loom’s PlasmaChains](https://medium.com/loom-network/loom-plasmachain-staking-is-officially-live-how-to-stake-your-loom-and-help-secure-plasmachain-e321dc462674) client is live
- Streamr opensourced [Monoplasma](https://medium.com/streamrblog/monoplasma-revenue-share-dapps-off-chain-6cb7ee8b42fa) for one to many payments
- At EthDenver, [Hoard’s Plasma Dog did 28.5k transactions](https://twitter.com/hoardexchange/status/1097181657218629634?s=19) on OmiseGo’s MoreViablePlasma implementation which saved ~$2300 in transaction fees by not putting them on the mainchain.
- a [Plasma watchtower](https://github.com/c-o-l-o-r/watchtower) built at EthDenver by Will Villanueva and Matt Garnett
- Why Ocean Protocol chose to [launch on a PoA chain](https://blog.oceanprotocol.com/ocean-on-poa-vs-ethereum-mainnet-decd0ac72c97)
- [Getting started with SKALE](https://medium.com/skale/getting-started-with-skale-part-1-5d6a025c95fd) sidechain network (testnet launched at EthDenver)
- Liquidity Network paper on [NOCUST](https://eprint.iacr.org/2018/642.pdf) with SNARKs for checkpoints
- Gluon Plasma goes live with [Leverj’s exchange on mainnet](https://blog.leverj.io/leverj-now-on-ethereum-mainnet-bd016af01cb7).

**State channels**

- FunFair is [planning to opensource](https://www.reddit.com/r/ethereum/comments/arjdbt/state_channel_based_gambling/egouwgw/) a more generalized version of its FateChannels
- “I just closed a mainnet Raiden Network channel. Through it I received or mediated 6600 payments and sent 430 payments with 1 wei being the smallest amount. It cost ~$0.30 in tx fees to open, close and settle the channel.” - [Jacob Czepluch](https://twitter.com/_czepluch/status/1098954683123748865).
- New Raiden release: [v0.100.2](https://github.com/raiden-network/raiden/releases/tag/v0.100.2) - webUI, bugfixes, and now you can run Raiden on Raspberry Pi
- Celer continues to run a [weekly Gomoku contest](https://medium.com/celer-network/celer-network-25th-weekly-project-progress-report-2-18-2-22-ee03a7f8ff83) where the top 64 scores get Eth. (Disclosure: I’ve won both weeks so far)

**Stuff for developers**

- [Building a decentralized Reddit, pt3](https://embark.status.im/news/2019/02/18/building-a-decentralized-reddit-with-embark-part-3/). Embark tutorial.
- [Getting started with the Buidler](https://medium.com/nomic-labs-blog/how-to-get-started-with-buidler-68beb6b9bb04) task runner
- [Etherlime v1.0.2](https://github.com/LimeChain/etherlime/releases/tag/v1.0.2) adds a flattener and React shape
- Truffle [v5.0.5](https://github.com/trufflesuite/truffle/releases/tag/v5.0.5)
- [Solhint v2](https://medium.com/protofire-blog/welcome-solhint-v2-0-shareable-configs-and-custom-plugins-ef9fac5dabb5) - Solidity linter
- [Brownie](https://medium.com/hyperlink-technology/introducing-brownie-a763859409ca): a Python framework for testing, deploying and interacting with your EVM code
- [Philippe Castonguay](https://medium.com/@PhABC/here-are-a-few-things-you-can-do-with-create2-that-create-cant-permit-f9e8809e6efd) on why Create2
- How Ronan Sandford (ex-EtherPlay) [architected his new game The Sandbox](https://medium.com/sandbox-game/blockchain-features-in-the-sandbox-7db91fcc615c)
- 3Box’s [human friendly web3 activity feed](https://medium.com/3box/a-more-human-web3-activity-feed-2d3b8f62afec)
- A t[axonomy of front running attacks](https://medium.com/consensys-diligence/transparent-dishonesty-taxonomy-of-front-running-attacks-on-blockchain-317d8ff78068)
- [Formal verification for noobs, pt 3](https://medium.com/ethworks/formal-verification-for-n00bs-part-3-an-attempt-to-prevent-classic-hack-with-klab-8e8d13318086)
- MythX [security plugin for Truffle](https://github.com/ConsenSys/truffle-security). MythX to give [25% of revenue to MythX tool plugins](https://medium.com/consensys-diligence/why-you-should-buidl-on-mythx-api-and-earn-revenue-share-in-dai-13d8bc7ca803)
- Finding all [underflows with eveem](http://eveem.org/static/underflows.pdf) and BigQuery
- [EthQL update](https://blog.infura.io/ethql-update-and-ethdenver-recap-b99cf9625b2)
- [Query Ethereum with SQL](https://eth.events/news/query-ethereum-with-sql/)

**Ecosystem**

- Grants: [Ethereum Foundation released a group](https://blog.ethereum.org/2019/02/21/ethereum-foundation-grants-program-wave-5/) of grantees (Matter’s rollup, LeapDAO Plasma, Shadowlands, py-libp2p, DeepSea, Eth on Arm, and Görli testnet), and [Gnosis](https://blog.gnosis.pm/gnosis-ecosystem-fund-update-i-f64dfd185f33) released its first group. Also [Maker gave a grant to DexPay](https://medium.com/dexlab-io/introducing-dexpay-and-makerdao-grant-announcement-f437f2e87da3) point of sale terminal
- Outcomes of the recent Status, web3foundation, and Validity labs [messaging protocol workshop](https://our.status.im/messaging-protocol-workshop-outcomes/)
- [Swarm v0.3.11 released](https://www.reddit.com/r/ethswarm/comments/asmfhe/swarm_v0311_released/)
- Proposed short ENS [auction reservation process](https://discuss.ens.domains/t/short-name-auction-reservation-process-proposed-process/836)
- Main event of the week: [Afri quit the Ethereum community](https://www.reddit.com/r/ethereum/comments/as8y75/statement_from_afri_i_did_not_quit_social_media_i/) in response to social media trolls. Many signed a [letter in response](https://docs.google.com/document/d/1poTd8ROh0WGu52jTsvWtJlIfuhg_oCN-6jaT03A5e1Y/edit). Afri is an Ethereum hero; that will never change. It’s a sad reminder that social attacks by outsiders can be effective. The only countermeasure is to frequently say _thank you_ to the many people who go above and beyond.
- ETHGlobal announced [upcoming hackathons](https://medium.com/ethglobal/ethglobal-2019-updates-get-your-calendars-ready-1977e9315aee) through 2019: Paris, Cape Town, New York, India, Boston, Waterloo
- EthDenver [finalists](https://kauri.io/collection/5c69c8c39c73740001dab899). [Winners of sponsor prizes](https://kauri.io/article/f4f31c650bd349f198b2aaf80a41ebed/v1/ethdenver-bounty-winners). [All the submissions](https://kauri.io/collection/5c5d8d27cc2d870001b6f741/ethdenver-2019-submissions), as there were many great submissions.
- Most core Ethereum devs [strongly prefer Eth](https://www.reddit.com/r/ethereum/comments/arw075/ama_about_ethereum_leadership_and_accountability/#egq7cik) to other crypto and are incentive aligned with Eth holders.

**Live on mainnet**

- Augur frontend [Guesser](https://medium.com/guesser/opening-guesser-to-the-public-introducing-bet-of-the-week-daf69f5742b5) is live. It’s got some prediction markets about the Oscars.
- [Convergent](https://beta.convergent.cx/#/): personal tokens on a pre-set price curve. “Invest in your friends.”
- Leverj’s exchange went live as mentioned above in Plasma section.
- NuoNetwork’s [non-custodial margin trading to leverage up 2x](https://medium.com/nuo-news/nuo-introducing-non-custodial-margin-trading-with-5x-leverage-b042f2fe533f)
- MolochDAO deployed to main net, and thus is now accepting membership and grant requests. [Whitepaper](https://github.com/MolochVentures/Whitepaper/blob/master/Whitepaper.pdf) on using a grants DAO to fund public goods.

**Enterprise**

- Pegasys: [Why IBFT 2.0](https://pegasys.tech/another-day-another-consensus-algorithm-why-ibft-2-0/)’s privacy improvements are good for enterprises and consortia
- iExec gets [900k euros from French government](https://medium.com/iex-ec/iexec-selected-as-a-winner-of-the-investment-for-the-future-programme-by-bpi-a-french-public-45d486d317fd) to adapt their computing platform to enterprise
- Update on Parity’s collaboration with [World Food Programme to bring cash payments to Syrian refugees](https://www.parity.io/un-world-food-programme-uses-parity-ethereum-to-aid-100-000-refugees/). Now 10x bigger: 100k transfers every month

**Governance and Standards**

- Given that [55-60% of miners are voting for ProgPow,](https://www.etherchain.org/charts/progpow) I think we can assume a lower limit on what % of hashpower is GPUs.
- [ERC1761](https://github.com/ethereum/EIPs/issues/1761): Scoped Approval Interface
- [ERC1756](https://github.com/ethereum/EIPs/issues/1756): Practical Randomness via Dual Contract
- [ERC1757](https://github.com/ethereum/EIPs/issues/1757): Reputation Mechanism to Claim Issuers
- [ERC1767](https://github.com/ethereum/EIPs/pull/1767/files): GraphQL interface to Ethereum node data

**Application layer**

- Digix targets [March 30th for governance](https://medium.com/@Digix/digix-dev-update-22-feb-2019-387076e1d1d0) launch, also storing gold in Canada as well as Singapore
- [Aragon Agent](http://blog.aragon.one/aragon-agent-beta-release/) - an account owned by an Aragon org to interact trustlessly with other web3 apps
- Golem v[0.19.0](https://blog.golemproject.net/brass-golem-beta-0-19-0-de67220eb30b) - new provider marketplace and migration to Docker for Windows
- [Request Protocol v2 alpha](https://blog.request.network/request-protocol-version-2-alpha-release-by-romaric-juniet-78f4153be4d5) release
- [FunFair 2019 roadmap](https://funfair.io/roadmap-update-h1-2019/): no 3rd party KYC app, more third party titles, and launching white label casinos.
- Maker to raise [stability fee to 1.5%](https://blog.makerdao.com/stability-fee-increase-february-22nd/)

**Interviews, Podcasts, Videos, Talks** 

- [Justin Drake indepth Eth2 walkthrough on NEAR's Whiteboard Series](https://youtu.be/S262StTwkmo?list=PL9tzQn_TEuFWweVbfTbaedFdwVrvaYPq4)
- Justin Drake [VDF talk](https://youtu.be/Kmm6BXXfsnI) and more from [VDF Day](https://www.youtube.com/playlist?list=PLaM7G4Llrb7y075mVXGmSABDP9Nb_PsBq) including Dan Boneh, Ben Wesolowski, and Filecoin
- Bounties Network [Mark Beylin and Simona Pop](https://podcast.ethhub.io/bounties-network-empowering-humans-to-incentivize-and-self-organize) on Into the Ether
- [Austin Griffith and Igor Barinov](https://www.zeroknowledge.fm/65) talk xDai on Zero Knowledge

**Tokens / Business / Regulation**

- Breaker (formerly SingularDTV) to put [proceeds from the Trust Machine](https://medium.com/@BreakerWorldwide/sngls-holders-become-part-of-the-trust-machine-experiment-5226ad688438) movie into a token they’ll give to their tokenholders as of ~March 13
- Dan Elitzer on the inevitable [financial engineering future](https://tokeneconomy.co/superfluid-collateral-in-open-finance-8c3db15efac) of open finance
- Monegro: [Cryptonetwork governance as capital](https://www.placeholder.vc/blog/2019/2/19/cryptonetwork-governance-as-capital)
- Responses to the [CFTC’s request for comments](https://comments.cftc.gov/PublicComments/CommentList.aspx?id=2941&ctl00_ctl00_cphContentMain_MainContent_gvCommentListChangePage=1_50)
- Institutional investor consultant Cambridge Associates published a [report](https://www.docdroid.net/0ZpsVwu/cryptocurrencies-venture-into-the-unknown-v2.pdf) arguing that funds should take a crypto position. [Bloomberg](https://www.bloomberg.com/news/articles/2019-02-18/it-s-time-to-consider-crypto-says-pension-and-endowment-adviser) article.
- [Brian Armstrong op-ed on custody](http://fortune.com/2019/02/21/cryptocurrency-custody-misconceptions-coinbase-ceo/) is worth a read if you hold crypto. He says they have $500 million under custody from institutions.  
    

**General**

- MetaMask passes [1m installs in the Chrome Store](https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn)
- CasperLabs is funding [Vlad Zamfir’s CBC Casper research](https://decryptmedia.com/5315/ethereum-core-developer-defects-to-rival), which seems like a win for Vlad, Ethereum, CBC, and CasperLabs.
- “the Bitcoin structure was quite brilliant, it seems like there’s some merit to Ethereum as well, and maybe some of the others” - [Elon Musk](https://twitter.com/econoar/status/1097982864665137153) in an interview this week
- Tweetstorm: [what are BLS sigs](https://twitter.com/cryptodavidw/status/1097180267985293312)?
- Paper: [new instantiation of a VDF](https://eprint.iacr.org/2019/166.pdf)
- There were some [crazy transaction fees this week](https://www.reddit.com/r/ethereum/comments/as7ejb/reminder_be_careful_while_developing_someone_just/), presumably due to forgetting a decimal point on the gas price.
- Lots of speculation about Samsung including Ethereum wallets on phone. Only confirmation I can find is this [line from a press release](https://news.samsung.com/us/samsung-galaxy-s10-more-screen-cameras-unpacked-2019/): “Galaxy S10 is built with defense-grade Samsung Knox, as well as a secure storage backed by hardware, which houses your private keys for blockchain-enabled mobile services.”
- Results for Gitcoin’s [25k “Liberal Radicalism” matching grants](https://medium.com/gitcoin/radical-results-gitcoins-25k-match-2c648bff7b19)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Feb ~28 - [Constantinople](http://didtheethereumblockchainreach1tbyet.5chdn.co/) (block 7280000)
- Mar 4 - [Ethereum Magicians](https://ethereum-magicians.org/t/council-of-paris-2019-announcement/2438) (Paris)
- Mar 5-7 - [EthCC](https://ethcc.io/) (Paris)
- Mar 8-10 - [ETHParis](https://ethparis.com/) 
- Mar 8-10 - [EthUToronto](https://www.ethuoft.ca/)
- Mar 22 - [Zero Knowledge Summit 0x03](https://www.zeroknowledge.fm/summit) (Berlin)
- Mar 27 - Infura [end of legacy key support](https://blog.infura.io/infura-dashboard-update-9f02d0643eb3) 
- April 4-5 - [Deconomy](https://deconomy.com/seoul2019/) (Seoul)
- April 8-14 - [Edcon](https://www.edcon.io/) hackathon and conference (Sydney)
- Apr 19-21 - [ETHCapetown](http://ethcapetown.com/)
- Apr 24-26 - [Truffle Elevate](https://www.eventbrite.com/e/truffle-elevate-dublin-2019-blockchain-development-workshop-tickets-53831596755) (Dublin)
- May 9 - [Fluidity Summit](https://www.fluiditysummit.com/) (NYC)
- May 10-11 - [Ethereal](https://etherealsummit.com/?ref=weekinethereum) (NYC)
- **May 17-19 - [ETHNewYork](https://medium.com/ethglobal/ethglobal-2019-updates-get-your-calendars-ready-1977e9315aee)**
- May 17 - Deadline to accept [proposals for Instanbul upgrade](https://en.ethereum.wiki/roadmap/istanbul) fork
- June 22-24 - [Zcon1](https://www.zfnd.org/zcon/) (Split, Croatia)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)

  
I own Week In Ethereum. Editorial control has always been 100% me. 

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## Update links to new URL: [weekinethereumnews.com](https://weekinethereumnews.com/) 

Archive on the web if you’re linking to it: [](https://weekinethereumnews.com/february-22-2019/)[https://weekinethereumnews.com/february-22-2019/](https://weekinethereumnews.com/february-22-2019/)

Cent link for the night view: [https://beta.cent.co/+zik0xx](https://beta.cent.co/+zik0xx)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

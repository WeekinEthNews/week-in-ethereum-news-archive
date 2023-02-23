---
title: "Week in Ethereum News <BR> July 28, 2019"
date: "2019-07-29"
---

## **Ethereum News and Links**

**Layer 1**

- Ben Edgington: [the Cathedral, the Bazaar, and the eth2 roadmap](https://media.consensys.net/ethereum-2-0s-latest-strides-forward-13f63652e57d). If you want a succinct “current state of Eth2” in prose, read this.
- Prysmatic [Eth2 client update](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-31-prysmatic-labs-e00d4d684b76) - fixing bugs, BLS sigs and state root validations fully enabled in run time
- Networking is the focus right now, so Matthew Slipper’s [Eth2 and libp2p report](https://docs.google.com/document/d/17OMi1MedOetF4Febijsc6KvGeNZdDQMb0yeC4QixOxw/edit#) for MolochDAO is timely. Protocol Labs’ Raúl Kripalani responds: how to improve the [Eth2 and libp2p effort](https://discuss.libp2p.io/t/report-a-study-of-libp2p-and-eth2/229)

**Layer 2**

- Cryptoeconomics Lab: [developing toward layer 2 interoperability](https://medium.com/cryptoeconomics-lab/cel-development-direction-to-the-greater-abstraction-6860f87ce0eb)
- [Routing fees in Raiden](https://medium.com/raiden-network/dynamic-mediation-fees-in-raiden-explained-dbc29f032e4b)
- [StarkExchange](https://medium.com/starkware/starkexchange-fast-withdrawals-using-cookie-jars-88eefea6a11a): Fast withdrawals using Cookie Jars
- “[In 14 days, 5,127 players from 62 countries played 53,180 layer-2 enabled games](https://twitter.com/celernetwork/status/1155639759202422790?s=21)” on Celer’s state channel network.

**Client releases**

- [Geth v1.9.1](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.1)
- [Ethereum on ARM](https://www.reddit.com/r/ethereum/comments/cgr9y4/ethereum_on_arm_nanopct4_and_raspberry_pi_images/): new NanoPC-T4 and Raspberry Pi images with new supported devices and Prysmatic Eth2 client and VIPnode support

**Stuff for developers**

- Solidity’s SMTchecker now supports [multi-transaction checks and unbounded loops](https://medium.com/@leonardoalt/smtchecker-toward-completeness-1a99c02e0133)
- [web3js stable release](https://medium.com/@samuel_91690/1-0-release-web3-js-ddd23d3c8f62). Breaking changes go into v2
- Truffle [v5.0.29](https://github.com/trufflesuite/truffle/releases/tag/v5.0.29) with stable web3js
- Vyper [v0.1.0-beta.11](https://vyper.readthedocs.io/en/v0.1.0-beta.11/release-notes.html#v0-1-0-beta-11)
- Provable (Oraclize) [OpenZeppelin starter kit](https://medium.com/oraclize/announcing-the-provable-openzeppelin-starter-kit-integration-9be369abc85c). Previously Zepkit, Zeppelin is [rebranding all products under OpenZeppelin](https://blog.openzeppelin.com/openzeppelin-rebranding/).
- OpenZeppelin [network.js front end web3 injection library](https://forum.openzeppelin.com/t/welcome-a-new-frontend-library-openzeppelin-network-js/1106). Also: ZeppelinOS/OpenZeppelinSDK [now has node 12 support](https://forum.openzeppelin.com/t/openzeppelin-sdk-2-5-2-with-node-12-support/1110)
- [Turn any deployed Eth code into a REST API](https://dash.fabrx.io/apis/all/) from Fabrx
- A [VRF Solidity library](https://medium.com/witnet/announcing-our-verifiable-random-function-vrf-library-in-solidity-c847edf123f7) from Witnet
- [Beware of the proxy: learn how to exploit function clashing](https://forum.openzeppelin.com/t/beware-of-the-proxy-learn-how-to-exploit-function-clashing/1070)
- Loredana Alias and dType video demos for [Wiki on Eth](https://www.youtube.com/watch?v=SOORplbwHME) and [generalized DNS for linked data & docs](https://youtu.be/5K8ZSy_rhaI)
- EthDenver2018 winner [Elk’s hardware dev kit is live on Kickstarter](https://www.kickstarter.com/projects/233173198/elk-the-dev-board-for-the-decentralized-world)
- Kauri launches communities, starting with [Ethereum for Java devs](https://kauri.io/community/5d2f30daaba2920001c82409)

**Ecosystem**

- [Speaker, builder and student Devcon applications](https://twitter.com/EFDevcon/status/1154419909792849920) re-open today for a week. Rolling decisions but everyone should hear by mid-August.
- [Winners of Gitcoin’s Beyond Blockchain](https://gitcoin.co/blog/beyond-blockchain-the-winners-more/) virtual hackathon
- [Tornado mixer](https://twitter.com/rstormsf/status/1154148852993183745) using snarks live on Kovan testnet
- [Austin Griffith video on the DAOG](https://www.youtube.com/watch?v=zIswnVh9qc4) - DAO game. Trippy, but very interesting concept
- Update on [ENS short name reservation criteria](https://discuss.ens.domains/t/an-update-on-the-short-name-reservation-process/1091/5). Also EthSimple’s new [ENS explorer](https://medium.com/@EthSimple/introducing-ethsimple-2-0-cde4ccb28b5e).
- [MetaMask Mobile is out in beta](https://medium.com/metamask/metamask-mobile-public-beta-a-feature-guide-and-walkthrough-9d01de7190ae)

**Governance and Standards**

- Latest [core devs call](https://youtu.be/DzmfR2P9kFk?t=70). [Notes](https://github.com/ethereum/pm/blob/a0c3a021bee9ae8c6a3d7a216afd374de6c88582/All%20Core%20Devs%20Meetings/Meeting%2066.md). EIPs **currently accepted** into Istanbul: 1344 (chain ID opcode), 2028 (calldata gas reduction), 2024 (blake2b), 1108 (alt\_bn128). EIPs **tentatively accepted**: 2200 (the new version of 1283 from Constantinople), 1962 (ECC precompile), 1884 (trie dependent reprice), 1057 (ProgPoW)
- ProgPoW is back into Istanbul (pending audit results), because the [audit is back on](https://medium.com/least-authority/https-medium-com-least-authority-kicking-off-our-review-of-progpow-be1368ae9a50).
- Preliminary report from [ZCash ProgPoW audit](https://github.com/ZcashFoundation/GrantProposals-2018Q2/issues/25#issuecomment-513876705): “ProgPoW is viable, but its use of GPU compute resources is far from optimal and its biggest advantage over Ethash isn't its "programmability" but rather its different than Ethash's reads from the DAG.”
- Ropsten Istanbul fork now scheduled for September 4th.
- [ERC2212](https://github.com/ethereum/EIPs/issues/2212): Interest earning stakes
- Jesse Walden: the [most interesting apps will need to be actively governed](https://a16z.com/2019/07/22/incomplete-contracts/)
- [Results from Aragon’s third vote](https://twitter.com/sohkai/status/1155417315216908288). The late-voting whale from last time voted in the middle this time, which effectively ended voting.

**Application layer**

- [Multicollateral Dai security roadmap](https://blog.makerdao.com/mcd-bug-bounty-announcement-and-security-roadmap-update/)
- [Numerai launches ErasureBay](https://medium.com/numerai/introducing-erasurebay-7a5de91b78d2), an open market for any kind of information
- [DaiHard](https://www.reddit.com/r/ethereum/comments/chl924/relaunching_the_borderless_unkillable_cryptofiat/): a fiat to crypto onchain exchange using burnable payments
- [Cryptogaming communities have relatively little overlap](https://nonfungible.com/blog/non-fungible-tokens-communities-analysis-2019)
- [Pooled cDai](https://twitter.com/boredGenius/status/1154427230023327744): pool your Dai together, send to Compound, send the interest to a beneficiary
- [Guesser expands to 10 weekly markets](https://medium.com/guesser/guesser-com-10-weekly-markets-and-a-fresh-new-website-b530fe270c6c), gets guesser.com and new UI
- [UNICEF Ventures using Bounties Network](https://www.forbes.com/sites/unicefusa/2019/07/23/revving-the-innovation-engine/#6d0c71dc2ba9) to track mentorship sessions

**Interviews, Podcasts, Videos, Talks** 

- [Péter Szilágyi and Martin Swende](http://thebitcoinpodcast.com/hashing-it-out-54/) discuss Geth v1.9 on Hashing It Out
- [Ameen Soleimani](https://www.youtube.com/watch?v=YgEXImQLoq4) on Epicenter
- 0x’s [Will Warren and Amir Bandeali](https://wyre-talks.simplecast.com/episodes/ep-44-powering-exchange-0x-roadmap-update) on Wyre Talks
- Cent’s [Cameron Hejazi](https://anchor.fm/wizardofdapps/episodes/Episode-12-Cent-co-with-Cameron-Hejazi-e4o7dk) on Wizard of Dapps
- [Anton Evangelatov and Rafael Matias](https://www.youtube.com/watch?v=E7lLimOnj90) presentation on Swarm
- Colony’s [Auryn MacMillan](https://daocast.io/s02e05) on DaoCast
- Latest [decentralized data call](https://youtu.be/gGXsQlfXKmA)
- [Ryan Sean Adams](https://medium.com/@TrustlessState/ether-the-triple-point-asset-with-ryan-sean-adams-73ce7bf6e669) on POV Crypto
- Matic’s [Jaynti Kanani](https://ethhub.substack.com/p/matic-scalable-and-instant-ethereum) on Into the Ether

**Tokens / Business / Regulation**

- [Monerium issues EU compliant Icelandic Krona e-money](https://twitter.com/monerium/status/1154353245298601984) on the mainnet
- SEC issues 2nd [no action letter to Pocketful of Quarters](https://www.sec.gov/corpfin/pocketful-quarters-inc-072519-2a1), another case where it was painfully obvious that the token isn’t a security.
- Fluidity’s [Tokenized Asset Portfolio](https://medium.com/fluidity/introducing-the-tokenized-asset-portfolio-7710e4239ab6), a legal and technical model to tokenize real world assets to use as DeFi collateral
- The [emerging decentralized finance stack](https://medium.com/@TrustlessState/ethereum-the-digital-finance-stack-4ba988c6c14b)
- [Fundament gets German regulatory approval](https://www.coindesk.com/german-regulators-approve-280-million-ethereum-token-sale) for 250m euro of real estate bonds, running on mainnet with no minimum investment

**General**

- History: this week marks the 5th anniversary of the Eth sale, and the 4th anniversary of the genesis block.
- Mougayar: [even with a dearth of marketing, Ethereum’s bazaar keeps growing](http://startupmanagement.org/2019/07/24/critical-thoughts-on-ethereums-unbundling-stack-and-marketing/)
- MyEtherWallet’s [beginner’s guide to Ethereum](https://www.mewtopia.com/absolute-beginners-guide/)
- [CDP creation skyrocketed from being on Coinbase Earn](https://twitter.com/balajis/status/1155332161601359872). An interesting experiment in incentivizing onchain activity.
- “[99.98 per cent of Americans were correctly re-identified in any available 'anonymised' dataset by using just 15 characteristics](https://techxplore.com/news/2019-07-anonymizing-personal-privacy.html)”

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- July 29-Aug 15 - [Grow Ethereum](https://hackathons.gitcoin.co/grow-ethereum/) virtual hackathon
- Aug 2-4 - [ETHIndia](https://ethindia.co/) (Bangalore)
- Aug 2-4 - [TruffleCon](https://www.truffleframework.com/trufflecon2019) (Redmond)
- **Aug 5-Sep 22 - [IDEO virtual hackathon](https://coinlist.co/build/ideo)**
- **Aug 16 - 18 - [ConsenSys Grants hackathon](https://pages.consensys.net/toronto-grants-hackathon) (Toronto)**
- Aug 21-23 - [Dappcon](https://dappcon.io/) (Berlin)
- **Aug 23 - [Last day for IDEX withdrawals](https://medium.com/idex/idex-kyc-transition-period-and-updated-asset-availability-for-us-markets-set-to-begin-d45e945f842d) without KYC**
- Aug 23-25 - [ETHBerlin](https://ethberlinzwei.com/)
- **Aug 29-30 - [ERC1400 security token hackathon](https://medium.com/@ramvi/invitation-to-hackathon-in-oslo-29-30-august-1d8ec54a26ad) (Oslo)**
- Sep 2-16 - [Decentraland SDK virtual hackathon](https://hack.decentraland.org/?with=weekinethereum) **(250k USD in prizes. There’s a referral code on that link that gets both you and me something extra)**
- Sep 3 - Deadline to [apply for EU Horizon Prize](https://ec.europa.eu/info/funding-tenders/opportunities/portal/screen/opportunities/topic-details/blockchain-eicprize-2019). 1m € each to 5 "Blockchains for Social Good" projects
- Sep 6-8 - [EthBoston](https://eth.boston/)
- Sep 15 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff/)
- Sep 15 - [Ethereal Tel Aviv](https://etherealsummit.com/events/ethereal-tel-aviv/)
- Sep 15-16- [StarkWare sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- **Oct 7 - [ENS workshop](https://medium.com/the-ethereum-name-service/ens-workshop-applications-are-now-open-f46db6c63384) (Osaka)**
- Oct 8-11 - [DeVcon](https://devcon.org/) (Osaka)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I own 100% Week In Ethereum. Editorial control has always been me.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **This headline stays as long as so many people continue to link to old URL and not the right one: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [](https://weekinethereumnews.com/week-in-ethereum-news-july-28-2019/)[https://weekinethereumnews.com/week-in-ethereum-news-july-28-2019/](https://weekinethereumnews.com/week-in-ethereum-news-july-28-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

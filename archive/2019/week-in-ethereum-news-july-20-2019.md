---
title: "Week in Ethereum News <BR> July 20, 2019"
date: "2019-07-21"
---

## **Ethereum News and Links**

**Layer 1**

- [What’s New in Eth2](https://notes.ethereum.org/c/Sk8Zs--CQ/https%3A%2F%2Fbenjaminion.xyz%2Fnewineth2%2F20190719.html)
- [Eth 2.0 Research AMA](https://www.reddit.com/r/ethereum/comments/cdg8v6/ama_we_are_the_eth_20_research_team_pt_2/). A [succinct tweetstorm](https://twitter.com/econoar/status/1150890624725315584) version from Eric Conner
- [9 things you didn’t know about Eth2](https://our.status.im/9-things-you-didnt-know-about-ethereum-2-0/)
- Rocketpool’s [Eth2 staking pool with a beta on testnet](https://medium.com/rocket-pool/development-update-17-july-2019-f3af7466cbd3) is coming soon.
- Great overview of [Eth2 and execution environments](https://drive.google.com/file/d/1ufvspealOGje6GPp-yJnCeO73bch1wRe/edit) from ConsenSys R&D’s Robert Drost
- [Efficient detection of surround voting](https://github.com/protolambda/eth2-surround) from protolambda
- A [walkthrough of the Beacon Chain spec](https://notes.ethereum.org/jDcuUp3-T8CeFTv0YpAsHw?view)

**Layer 2**

- [Burn relay registry](https://ethresear.ch/t/burn-relay-registry-decentralized-transaction-abstraction-on-layer-2/5820): burn small % of fees for spam resistant layer 2 transaction relayers
- [Atomic swap Plasma predicate](https://plasma.build/t/architecture-design-idea-of-atomic-swap-predicate/124) architectural design
- MESG’s [Plasma Guard](https://medium.com/mesg/plasma-is-not-secure-unless-you-watch-it-196d23130367) - demo and code of OmiseGo Plasma watchtower
- [StarkDex pt3](https://medium.com/starkware/starkdex-deep-dive-the-stark-core-engine-497942d0f0ab), the STARK core engine

**Client releases**

- Trinity [v0.1.0-alpha.27](https://github.com/ethereum/trinity/releases/tag/v0.1.0-alpha.27) - BEAM sync prototype

**Stuff for developers**

- [Infura Plus](https://blog.infura.io/today-we-are-launching-infura-plus-c19114c1849d): premium subscription tiers
- Elena Nadolinski’s [list of zk tools](https://docs.google.com/presentation/d/1-QB6DAHliQRAUW5rdCqSRQ_w6W2yGTidB61UWzq_p20/edit#slide=id.g5dd7a461f4_0_512)
- [Making sense of state channels for devs, pt 2](https://medium.com/celer-network/c-l4-8525ffc2d5f)
- [Cobra](https://github.com/cobraframework/cobra): new dev environment framework
- Waffle [2.0.14](https://github.com/EthWorks/Waffle/releases/tag/2.0.14) supports human-readable ABI as output
- [Ganache TimeTraveler](https://github.com/ejwessel/GanacheTimeTraveler/): move forward or backward in time
- An easier way to [deploy your code with TruffleTeams](https://www.trufflesuite.com/blog/an-easier-way-to-deploy-your-smart-contracts)
- [Speeding up IPFS with Piñata](https://medium.com/pinata/ipfs-scalability-f0a6f8a7d42b)
- [Drop in ENS support](https://medium.com/the-ethereum-name-service/new-react-ens-address-component-lets-you-drop-in-ens-support-to-your-dapp-b31863ba85a6) with React component
- What does Trueblocks mean when it says it is a [decentralized block explorer](https://medium.com/coinmonks/a-time-ordered-index-of-time-ordered-immutable-data-e28ced3417cc)?
- EthNewYork winner [ExeDAO](https://medium.com/@exedao/exedao-secure-arbitrary-execution-on-ethereum-smart-contracts-b5a1854d30b2): run any contract through your DAO as long as it doesn’t include storage modification opcodes

**Ecosystem**

- Ethereum [governance survey results](https://medium.com/coinmonks/ethereum-governance-survey-results-c67c11695f2a)
- [Toward an interoperable name service](https://medium.com/the-ethereum-name-service/towards-interoperable-name-service-standard-9e6c0dd0ee35)
- [p2p data sync for mobile](https://vac.dev/p2p-data-sync-for-mobile) from Status
- MetaCartel has 750 ETH in its grants DAO to [support UX and usability of web3 apps](https://medium.com/metacartel/metacartel-dao-rises-e0646393718b)

**Governance and Standards**

- Latest [core devs call](https://youtu.be/41kiRf1E-jI?t=143). Per the [notes](https://github.com/ethereum/pm/blob/734be683d3bef403ac883e7ab13b2b7e4d3022b2/All%20Core%20Devs%20Meetings/Meeting%2065.md): EIP 2028 accepted for Istanbul fork, EIP2200 tentatively accepted. ProgPoW audit not done so not included in Istanbul. EIPs with reference implementations 1352, 1845, 1985, 2027 and 2046 still under consideration for Istanbul.
- [EIP2200](https://github.com/ethereum/EIPs/blob/e4d4ea348e06c54d0075c400dc7b72430d427ff1/EIPS/eip-2200.md): Rebalance net-metered SSTORE gas cost with consideration of SLOAD gas cost change
- Why EIP2028 makes sense, and Starkware’s experiment to show [we can reduce gas cost 4x for data](https://ethereum-magicians.org/t/eip-2028-transaction-data-gas-cost-reduction/3280/24)
- [ERC2193](https://github.com/loredanacirstea/EIPs/blob/779d145a140f086e93576acbd82faaab1c0c2012/EIPS/eip-2193.md): Alias - decentralized type system. More on [Alias](https://medium.com/@loredana.cirstea/flexible-alias-or-why-ens-is-obsolete-a1353030f445): “a homogeneous standard for identifying resources by human-readable qualifiers” and a [simple video demo of Alias](https://youtu.be/7jYVjoLsx1A)
- [Outsource sybil resistance in your DAO](https://bitfalls.com/2019/07/16/outsourcing-sybil-resistance-in-your-dao-with-modifiers/) to HumanityDAO

**Application layer**

- [Augur Liquidity Partner Program](https://www.augur.net/blog/pooling-liquidity/): more promotion in exchange for pooling liquidity
- [Auctions and Keepers in Multi Collateral Dai](https://github.com/makerdao/developerguides/blob/master/keepers/auctions/auctions-101.md)
- [0x Mesh p2p network](https://twitter.com/0xProject/status/1152005400809504768) is in beta
- [DefiPulse adds the DefiList](https://defipulse.com/blog/meet-the-defi-list/)
- Uniswap’s SOCKS got forked, now we have [SOCKS CLASSIC](https://medium.com/@unisocksclassic/why-we-decided-to-fork-socks-223c08eb488f). I kid you not.
- Spankchain now has [international models, and also now accepts credit cards](https://medium.com/spankchain/spank-live-update-international-and-fiat-5abc7defecea)
- [WBTC added to Compound](https://medium.com/compound-finance/adding-wbtc-to-the-compound-protocol-b032da38511c). They also [hit the $100m mark](https://twitter.com/rleshner/status/1152683453059489794) in assets supplied at Compound.
- [Trend trading strategies](https://medium.com/set-protocol/introducing-trend-trading-strategies-on-tokensets-8e69ed268a41) from SetProtocol. Automated trend following strategies make a ton of sense in crypto, and may be tax advantaged in some jurisdictions.

**Interviews, Podcasts, Videos, Talks** 

- E&Y’s [Paul Brody](https://www.reddit.com/r/ethtrader/comments/cf4x60/paul_brody_on_ey_ethereum_and_enterprise/) does an EthCommunitySeries interview
- Set Protocol’s [Felix Feng and Alex Soong](https://ethhub.substack.com/p/set-protocol-automating-asset-management) on Into the Ether
- WednesdayCoin’s [Mike Vargas](https://anchor.fm/wizardofdapps/episodes/Episode-11-Wednesday-Coin-with-Mike-Vargas-e4l90l) on Wizard of Dapps
- [Joey Krug](https://podcasts.apple.com/us/podcast/61-augur-conversation-on-crypto-user-acquisition-joey/id1350649166?i=1000444680842) on Blockcrunch
- Parity’s [Pierre Krieger](https://www.youtube.com/watch?v=_9o6RTYG_xk) talks libp2p
- Abraham.ai art DAO’s [Gene Kogan](https://overcast.fm/+N6TEwPLlE) on Digitally Rare
- Trail of Bits’s [Dan Guido](http://thebitcoinpodcast.com/hashing-it-out-53/) on Hashing It Out
- Nexus Mutual’s [Hugh Karp](https://twitter.com/DavidJN79/status/1150748593608900610) on Base Layer

**Tokens / Business / Regulation**

- [France set to approve a few token sales](https://www.reuters.com/article/us-crypto-currencies-regulation-france/france-to-approve-first-crypto-issuers-as-new-rules-loom-idUSKCN1UB18P)
- [IDEX implements KYC](https://medium.com/idex/idex-kyc-transition-period-and-updated-asset-availability-for-us-markets-set-to-begin-d45e945f842d), and announces restrictions on what assets Americans can trade
- Prospective [web3 business models](https://medium.com/ahnboard/web3-business-models-in-the-wild-fdbc93f9713b)
- Scott Lewis’s [Eth valuation worksheet](https://docs.google.com/spreadsheets/d/1eQysicmKjkSllgBBss5YY490y96G2hfSRVzcfakOwXM/edit#gid=0)

**General**

- [Machine learning to detect bad output](https://medium.com/@epiclabs.io/machine-learning-for-video-transcoding-verification-in-livepeers-ecosystem-i-e020ed11d6b4) by Livepeer transcoders
- [Land banks and American colonial money supply](https://medium.com/coinmonks/makerdao-18th-century-edition-bd15722d9193): a historical corollary to Maker’s Dai
- Chris Robison thread on [DAOs as Medieval Age guilds](https://twitter.com/CBobRobison/status/1151964362229207040)
- Raul Jordan suggests [Libra’s code base does not imply eventual decentralization](https://www.tokendaily.co/blog/a-close-look-at-libra-s-source-code) since regular users can’t access the state.
- [cryptoscamDB](https://medium.com/mycrypto/introducing-cryptoscamdb-org-77125e140650) from MyCrypto. Because there are scammers all over crypto and Harry tracks them.

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- **July 22-29 - [0x upgrade vote](https://blog.0xproject.com/vote-with-zrx-to-add-support-for-erc-1155-and-the-staticcallassetproxy-49a855807bcd) for ERC1155 and StaticCallAssetProxy**
- **July 25 - [Aragon vote #3](https://blog.aragon.org/final-details-for-aragon-network-vote-3/)**
- **July 26 - Next core devs call**
- **July29-Aug15 - [Grow Ethereum](https://hackathons.gitcoin.co/grow-ethereum/) virtual hackathon**
- Aug 2-4 - [ETHIndia](https://ethindia.co/) (Bangalore)
- Aug 2-4 - [TruffleCon](https://www.truffleframework.com/trufflecon2019) (Redmond)
- Aug 21-23 - [Dappcon](https://dappcon.io/) (Berlin)
- Aug 23-25 - [ETHBerlin](https://ethberlinzwei.com/)
- **Sep 2-16 - [Decentraland SDK virtual hackathon](https://hack.decentraland.org/)**
- Sep 3 - Deadline to [apply for EU Horizon Prize](https://ec.europa.eu/info/funding-tenders/opportunities/portal/screen/opportunities/topic-details/blockchain-eicprize-2019). 1m € each to 5 "Blockchains for Social Good" projects
- Sep 6-8 - [EthBoston](https://eth.boston/)
- Sep 15 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff/)
- Sep 15 - [Ethereal Tel Aviv](https://etherealsummit.com/events/ethereal-tel-aviv/)
- Sep 15-16- [StarkWare sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- Oct 8-11 - [DeVcon](https://devcon.org/) (Osaka)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I own 100% Week In Ethereum. Editorial control has always been me.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **This headline stays as long as so many people continue to link to old URL and not the right one: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/week-in-ethereum-news-july-20-2019/](https://weekinethereumnews.com/week-in-ethereum-news-july-20-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

---
title: "June 21, 2018"
date: "2018-06-21"
---

## **News and Links**

**Protocol**

- EIP1011 deprecated in favor of [casper + sharding](https://medium.com/@djrtwo/casper-%EF%B8%8F-sharding-28a90077f121). It “brings us to a full-PoS, sharded, scalable blockchain much sooner”
- New [Casper+Sharding](https://notes.ethereum.org/SCIg8AH5SA-O4C1G1LYZHQ?view) spec
- Drake: [Artificial beacon chain penalties](https://ethresear.ch/t/artificial-beacon-chain-penalties/2302)
- Casey Detrio: [Synchronous cross-shard transactions with consolidated concurrency control and consensus](https://ethresear.ch/t/synchronous-cross-shard-transactions-with-consolidated-concurrency-control-and-consensus-or-how-i-rediscovered-chain-fibers/2318)
- Drake: [Optimised handling of proposer and attester signatures](https://ethresear.ch/t/optimised-handling-of-proposer-and-attester-signatures/2280)
- Buterin: [Attestation committee based full PoS chains](https://ethresear.ch/t/attestation-committee-based-full-pos-chains/2259)
- Latest [Casper standup](https://www.youtube.com/watch?v=d8GeuRbBI6k)
- Tom Close: [Force-Move games state channels framework](https://medium.com/statechannels/introducing-the-force-move-games-framework-for-state-channels-b32dd953c13f)
- Fichter: [Griefing Vectors in Confirmation Signatures](https://ethresear.ch/t/griefing-vectors-in-confirmation-signatures/2301)
- [Double Batched Merkle Log Accumulators](https://ethresear.ch/t/double-batched-merkle-log-accumulators-for-efficient-plasma-commitments/2313) to make Plasma commitments cheaper
- [Paying rent with deposits](https://ethresear.ch/t/paying-rent-with-deposits/2221/20)?
- UTexas paper on [merkleizing levelDB](https://www.cs.utexas.edu/~vijay/papers/hotstorage18-eth.pdf) for Ethereum
- Latest [core devs call](https://www.youtube.com/watch?v=8-AZys80RrU). Lane’s [notes](https://github.com/ethereum/pm/blob/master/All%20Core%20Devs%20Meetings/Meeting%2040.md).
- [Swarm PoC3](https://blog.ethereum.org/2018/06/21/announcing-swarm-proof-of-concept-release-3/) released  
    

**Stuff for developers**

- Zkstark mixer [Miximus](https://github.com/barryWhiteHat/miximus) is live on [Rinkeby](https://rinkeby.etherscan.io/address/0xb586453a8e44c86e012958e48a0deced462bd16e)
- There’s been a [decent chunk of the network used recently by airdrops](https://www.reddit.com/r/ethereum/comments/8sd8ik/are_airdrops_abusing_our_network/), so [Jeff Coleman reminds](https://twitter.com/technocrypto/status/1009543517645963267) projects that they can save lots of money by using Richard Moore’s [Merkle Air Drops](https://blog.ricmoo.com/merkle-air-drops-e6406945584d)
- MetaMask will no longer [reload pages on network change](https://medium.com/metamask/breaking-change-no-longer-reloading-pages-on-network-change-4a3e1fd2f5e7)
- [Exploring Eth storage cost](https://blog.foam.space/exploring-ethereum-storage-costs-with-the-foam-developer-tools-96d84e1a06b5) with FOAM’s dev tools
- 7 challenges in [Dharma’s JS fiddle](https://blog.dharma.io/fiddle-with-dharma-js-600cb589a13a)
- A rough [ERC721 implementation in Vyper](https://github.com/maurelian/erc721-vyper) from Maurelian
- [IPFS Pubsub React](https://github.com/eolszewski/ipfs-pubsub-chatroom) boilerplate
- UI for the [simplest multisig wallet](https://medium.com/@Radhika.Anand/the-simplest-multisig-wallet-part-2-939519be954c)
- [Cava](https://github.com/consensys/cava): core libraries for blockchain dev in Java and Kotlin
- [Embark v3.1](https://blog.status.im/embark-3-1-planet-express-60493ca0ad79) -  better testing, lightweight wallet functionality, a transaction logger, profiler, clever imports, ENS support
- [Truffle v4.1.12](https://github.com/trufflesuite/truffle/releases/tag/v4.1.12)
- Comprehensive [list of Solidity attack vectors](https://blog.sigmaprime.io/solidity-security.html) and how to avoid them

**Ecosystem**

- Status unveiled [Nimbus](https://github.com/status-im/nimbus/blob/master/doc/Nimbus%20-%20An%20Ethereum%202.0%20Sharding%20Client_xt.md#january---february-2018), an Eth client in Nim for resource constrained devices. More from Status: [building custom mailservers and bootnodes](https://blog.status.im/building-censorship-resistant-tools-and-the-introduction-to-custom-bootnodes-and-mail-servers-c2b44ae5e807), which they needed to get around Russian anti-Telegram IP blocking
- Parity: [why we believe in WASM](https://paritytech.io/wasm-smart-contract-development/), though [Brendan Eich has some skepticism](https://twitter.com/BrendanEich/status/1009562709904330760)
- [MyCrypto v1.1](https://medium.com/mycrypto/new-feature-address-book-ccfcc56dc833) with address book
- Nick Johnson’s state of [ENS slides](https://docs.google.com/presentation/d/1HHKX_r_E-yWy5t9UcMSlQBghUpexHKYkhH2JvYwGTSQ/edit#slide=id.p)
- [CryptoPrimitive Academy](https://www.reddit.com/r/ethereum/comments/8smqe0/creating_useful_dapps_is_easier_than_people_think/) - free series of dapp dev seminars starting next Monday
- A [Whisper explainer](https://www.sitepoint.com/ethereum-messaging-whisper-status/)
- AirSwap: [decentralized exchanges are the web3 app stores](https://blog.airswap.io/the-app-store-of-ethereum-is-powered-by-tokens-25a3af0f71da)
- [VIPNode update](https://medium.com/@shazow/vipnode-progress-update-b3b53e4ea7a2)
- [Verifying identify in Venezuela](https://blog.zeppelin.solutions/verifying-identity-in-venezuela-through-the-tpl-5bccd0a7d5fb) using Zeppelin’s Transaction Permission Layer
- All [uPort protocols and libraries](https://medium.com/uport/a-complete-list-of-uports-protocols-libraries-and-solutions-63e9b99b9fd6)
- Latest [Open Block Explorers](https://www.youtube.com/watch?v=1tfKasW3EQ4) call

**Live on mainnet**

- [SpankChain’s public beta](https://twitter.com/SpankChain/status/1007680210286739456) went live on mainnet
- Dharma relayer [Bloqboard is live](https://dapp.bloqboard.com/) on mainnet
- iEx.ec deployed their [marketplace and hub contracts on mainnet](https://medium.com/iex-ec/iexec-dev-letter-21-v2-mainnet-security-audits-whats-next-380f96d02e86) in a soft launch. Public working pools in September

**Governance and Standards**

- I was wrong last week. ERC721 is [now officially finalized](https://github.com/ethereum/EIPs/pull/1170) with a relatively last minute [breaking change](https://github.com/ethereum/EIPs/issues/721#issuecomment-398465608)
- [EIP1153](https://eips.ethereum.org/EIPS/eip-1153): transient storage opcodes. FEM [discussion](https://ethereum-magicians.org/t/eip-transient-storage-opcodes/553/11).
- [ERC1129](https://eips.ethereum.org/EIPS/eip-1129): standardized dapp announcements
- [ERC1154](https://github.com/ethereum/EIPs/issues/1161): Oracle interface
- [ERC1155](https://github.com/ethereum/EIPs/issues/1155): mint ERC20 and ERC721 tokens in same contract
- [ERC1167](https://eips.ethereum.org/EIPS/eip-1167): Minimal proxy contract
- [ERC1152](https://github.com/ethereum/EIPs/pull/1152): Access control with NFTs
- [ERC1172](https://github.com/ethereum/EIPs/pull/1172): wallet and shop standard for tokens
- [ERC1165](https://github.com/ethereum/EIPs/issues/1165): registry for human-readable contract descriptions
- Some discussion on [ERC792](https://github.com/ethereum/EIPs/issues/792) arbitration standard
- Dean Eigenmann’s meditations on what [we can learn from the EOS governance anti-pattern](https://medium.com/@decanus/meditations-on-eos-f74790dc45ac).
- How Nexus Mutual is [thinking about DAO governance](https://medium.com/nexus-mutual/dao-governance-a-pragmatic-approach-27d529ad0819)
- Kent Barton’s [5 takeaways from the recent Ethereum values survey](https://medium.com/@seven7hwave/scaling-the-community-five-takeaways-from-the-ether-f327fb00adb1)

**Project Updates**

- Loom Network’s [Zombie Battleground NFT card game is on Kickstarter](https://medium.com/loom-network/zombie-battleground-launches-on-kickstarter-fc7579e51e1a) and has already raised [$210k out of 250k](https://www.kickstarter.com/projects/328862817/zombie-battleground-the-new-generation-of-ccg-tcg?ref=weekinethereum) in less than a week
- The [6 companies tokenizing their equity](https://blog.neufund.org/meet-the-first-companies-tokenizing-their-equity-on-blockchain-8dd2a9c4091f) with Neufund
- An [AMA with Althea Mesh](https://www.reddit.com/r/darknetplan/comments/8rscom/we_are_the_althea_development_team_ama/)
- Iconomi [Q2 dev update](https://medium.com/iconominet/development-overview-q2-2018-fd11fc14388b)
- FunFair to [launch their own casino](https://funfair.io/funfair-technologies-company-update/) to dogfood their product
- AXA’s “Fizzy” flight delay insurance now [open to French and Italians](https://medium.com/@laurentbenichou/fizzy-axa-reaches-a-new-milestone-fadd41f20e11) and [publishes its code](https://medium.com/@humanGamepad/fizzy-axa-smart-contract-explaind-740df52894fd) which notarizes your transaction.
- You can now use your [Gnosis tokens to generate OWL](https://blog.gnosis.pm/generate-your-first-owl-using-gno-2205eb098f8)
- [Optionality](https://www.reddit.com/r/ethdev/comments/8si2rp/optionality_create_and_trade_options_on_erc20/) token options trading platform live on Kovan
- Grid+ imminent [regulatory approval to sell electricity](https://blog.gridplus.io/grid-progress-report-6-14-2018-a5aa64a71251) at retail
- Kleros will provide [decentralized arbitration for seasteading](https://medium.com/kleros/kleros-blue-frontiers-partnership-decentralized-justice-for-floating-cities-3c089830cbae)
- NYTimes writeup of [ex-Denver Post folks joining Civil](https://mobile.nytimes.com/2018/06/17/business/media/denver-post-blockchain-colorado-sun.html)
- Userfeeds is shutting down current company but [CTO is raising money to focus on being a product](https://blog.userfeeds.io/part-ii-new-beginnings-a7520702b5be) instead of platform
- [Colony live on Rinkeby testnet](https://blog.colony.io/colony-rinkeby-283c4a074127) for devs in their hackathon. Also, the [Colony stack](https://blog.colony.io/what-does-colony-look-like-edd7e709fc86)
- Maker DAO’s [Foundation Proposal](https://medium.com/makerdao/foundation-proposal-caeb382465c1) - the first vote on Aug 22

**Interviews, Podcasts, Videos, Talks** 

- Hashing It Out discussion of [Casper + Sharding](https://thebitcoinpodcast.com/hashing-it-out-12/)
- Mythril’s [Gerhard Wagner](http://www.thesmartestcontract.com/8) on Smartest Contract
- All the videos from [Oslo Blockchain Day](https://medium.com/blockchangers/recap-from-oslo-blockchain-day-2018-25e8976991d2)
- [State channel panel](https://www.youtube.com/watch?v=jzoS0tPUAiQ&feature=youtu.be&t=2h10m9s) at MIT’s Layer 2 summit
- Emin Gün Sirer [talk on Avalanche](https://www.youtube.com/watch?v=AXrrqtFlGow)
- Alejandro Machado talks [crypto use in his native Venezuela](https://itunes.apple.com/us/podcast/the-coin-pod/id1350143328#)
- Spankchain’s [Ameen Soleimani](http://www.thesmartestcontract.com/7) on Smartest Contract
- [John Pacific and David Nuñez](https://thebitcoinpodcast.com/hashing-it-out-11/) from NuCypher on Hashing It Out
- Coinbase’s [Adam White](https://itunes.apple.com/us/podcast/coinbases-adam-white-on-a-momentous-day-in-crypto-ep-023/id1347049808?i=1000413848610&mt=2) with Laura Shin

**Tokens** 

- [Inflation funding in practice](https://medium.com/livepeer-blog/inflation-funding-in-practice-in-delegated-stake-based-protocols-15cd9400e458) in Livepeer. Paratii also looking to [incent curation through inflation](https://medium.com/paratii/pti-token-summary-edf048d36245)
- [Curation markets with infinite staking](https://medium.com/paratii/curation-markets-infinite-staking-247e8b72caa3)
- [Artonomous](https://github.com/simondlr/artonomous) - Simon de la Rouviere experiment to sell daily art on curved bond
- Mapping the [NFT landscape](https://medium.com/point-nine-news/mapping-the-emerging-non-fungible-token-landscape-ee56f0d1079f)
- Foam’s [TCRs for points of interest on maps](https://blog.foam.space/foam-main-net-preview-token-curated-registries-for-geographic-points-of-interest-af3f0eba5cee)
- [Gatekeepers](https://medium.com/@jonthnH/designing-gatekeepers-using-token-curated-registries-and-work-tokens-to-manage-access-control-720b8923eb5) : TCRs and work tokens for access control
- Vitalik’s slides on [mechanism design challenges](https://docs.google.com/presentation/d/1MLwN2-pBufDmUNprf-r8LXFCm1Ua8skphzDTNPTaiUQ/edit#slide=id.p)

**General**

- Ethereum Foundation helps underwrite for Stanford’s new [Center for Blockchain Research](https://engineering.stanford.edu/news/stanford-computer-scientists-launch-center-blockchain-research)
- How do you get your kids to do chores? You IoT the heck out of your house with [chore tracking and then pay your kids in crypto](https://thenextweb.com/hardfork/2018/06/18/this-insanely-cool-diy-smart-home-features-alexas-ai-and-ethereums-blockchain/) on completion.
- Lots of Ethereum in lastest [Thiel Fellows](https://www.businesswire.com/news/home/20180622005131/en/Thiel-Foundation-Announces-2018-Thiel-Fellows)
- Docusign will let you [store a document hash on Ethereum](https://www.docusign.com/blog/momentum-2018-time-modern-systems-agreement/)
- EY and Microsoft launch [content permissions and royalties management](https://www.ey.com/gl/en/newsroom/news-releases/news-ey-and-microsoft-launch-blockchain-solution-for-content-rights-and-royalties-management-for-media-and-entertainment-industry) using Quorum that will be used first for XBox game publishers.
- Tether releases [independent report](https://tether.to/fss-report-transparency-update/) of fiat matching Tether supply
- Be wary of MetaMask [phishing attempts from Cloudflare security holes](https://medium.com/metamask/new-phishing-strategy-becoming-common-1b1123837168)

## **Dates of Note**

**Upcoming dates of note:**

- June 24 -- [Colony](https://blog.colony.io/announcing-the-colony-global-hackathon-1d9bf9004407) online hackathon finishes
- June 25 -- [Etherisc](https://blog.etherisc.com/dip-token-generating-event-will-start-on-25-june-2018-db8c5aa832ac) token sale starts
- June 28 -- [BuildEth](http://www.buildeth.io/) (San Francisco)
- June 30 -- [Solidity Gas Golfing](https://g.solidity.cc/) challenge deadline
- June 30-July1 -- [Off the chain](https://binarydistrict.com/courses/master-workshop-off-the-chain/) state channel workshop (Berlin)
- July 6-7 -- TechCrunch [blockchain and Ethereum events](https://techcrunch.com/2018/06/03/announcing-the-techcrunch-ethereum-meetup-alongside-our-blockchain-event-in-zug/) (Zug)
- July 9 -- [Augur](https://medium.com/@AugurProject/augur-weekly-development-update-may-23rd-4d78befe7bf8) scheduled to launch
- July 12 -- [Sharding and Casper workshop](https://www.meraevents.com/event/ethereum-foundation-workshop-iit-delhi?ucode=weekinethereum) with Karl Floersch and Justin Drake (New Delhi)
- July 12-18 -- [IC3 Eth Bootcamp](http://www.initc3.org/events/2018-07-12-IC3-Ethereum-Crypto-Boot-Camp.html) (Ithaca, NY)
- July 14-15 -- [FEM governance meetings](https://ethereum-magicians.org/t/proposed-agenda-for-the-council-of-berlin-set-for-july-14-15/377) in Berlin
- July 19-20 -- [DappCon](https://www.dappcon.io/) (Berlin)
- July 24-26 -- [NIFTY](https://nifty.gg/) hackathon and NFT conference (Hong Kong)
- August 3-4 -- [Discon](https://discon.io/) (Boulder, CO)
- August 10-12 -- [EthIndia](https://ethindia.co/) hackathon (Bangalore)
- August 22 -- Maker DAO ‘[Foundation Proposal](https://medium.com/makerdao/foundation-proposal-caeb382465c1)’ vote
- September 6 -- [Security unconference](https://ethereum-magicians.org/t/wiki-gathering-of-security-community/433) (Berlin)
- September 7-9 -- [EthBerlin](http://ethberlin.com/) hackathon
- September 7-9 -- WyoHackathon (Wyoming)
- Oct 5-7 -- [TruffleCon](http://truffleframework.com/trufflecon2018) in Portland
- Oct 5-7 -- EthSanFrancisco hackathon
- Oct 22-24 -- [Web3Summit](http://web3summit.com/) (Berlin)
- Oct 30 - Nov 2 -- [Devcon4](https://devcon.ethereum.org/) (Prague)
- December -- EthSingapore hackathon

## **If you appreciate this newsletter, thank ConsenSys**

I'm thankful that [ConsenSys](http://consensys.net/) has brought me on and given me time to do this newsletter.  
  

![](https://steemitimages.com/640x0/https://res.cloudinary.com/hhsslviub/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F7ae9356f-3652-4de2-a85e-57e514ddbd44_240x240)

Editorial control is 100% me.  If you're unhappy with editorial decisions, blame me.

## **Shameless self-promotion**

  
Most of what I link to I tweet first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

This newsletter is supported by [ConsenSys](https://consensys.net/)

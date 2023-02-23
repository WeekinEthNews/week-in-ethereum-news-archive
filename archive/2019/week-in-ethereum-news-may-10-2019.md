---
title: "May 10, 2019, Week in Ethereum News"
date: "2019-05-11"
---

## **Ethereum News and Links**

**Layer 1**

- [Prysmatic releases its Eth2 testnet](https://medium.com/prysmatic-labs/ethereum-2-0-phase-0-testnet-release-1e9e682db910)
- [Finality in Eth2](https://medium.com/@ralexstokes/how-secure-is-ethereum-2-0-consensus-41523a59f270). Put differently: why Eth2 will be much more final and secure than Eth1 or BTC - as this week’s aborted attempt by Binance to re-org BTC showed
- An Eth2 [randomness explainer - RanDAO and VDFs](https://our.status.im/two-point-oh-randomness/)
- Drake: how to create [timelock puzzles targeting RSA VDF ASIC](https://ethresear.ch/t/fixed-modulus-timelock-puzzles/5402)s with a hardcoded modulus.
- [Gas market ideas for eth2, phase 2](https://ethresear.ch/t/an-optimistic-generic-gas-market-executor-for-phase-2/5429)
- Academic paper [benchmarking EVM opcode pricing](https://arxiv.org/pdf/1905.00553.pdf)

**Client releases**

- [Nethermind v0.9.9](https://www.reddit.com/r/ethereum/comments/bmlp2u/nethermind_099_45gb_mainnet_fast_sync_in_5_hours/) - fast sync with mainnet in just 5 hours by not downloading transaction receipts

**Stuff for developers**

- A [Scratch3 extension](https://github.com/naddison36/eth-scratch3#eth-scratch3) to make it easy and kid-friendly to build games on Eth
- Truffle [v5.0.17](https://github.com/trufflesuite/truffle/releases/tag/v5.0.17)
- Buidler: [task runner as coordinator for all your Eth dev tools](https://medium.com/nomic-labs-blog/buidler-compounding-value-for-ethereum-developers-425141a41b7b)
- [What’s new in web3py v5 beta](https://medium.com/@khtclowes/whats-new-in-web3py-v5-7c5c60d26834)
- Fix your [Solidity and Truffle versioning issues with NPX](https://medium.com/blockchangers/how-to-fix-your-truffle-and-solidity-versioning-with-npx-from-npm-51b5fcb0825f)
- Nick Dodson’s [311 byte eip712 compliant multisig](https://github.com/SilentCicero/MultiSignatureWallet)
- [Flint statically-typed programming language](https://arxiv.org/abs/1904.06534) for safer Eth code by Schrans, et al
- [Gas optimization in Solidity, pt 1: variables](https://medium.com/coinmonks/gas-optimization-in-solidity-part-i-variables-9d5775e43dde)
- A graphical look at the [functions in Maker’s architecture](https://medium.com/coinmonks/maker-dao-transactions-illustrated-691ad2715cf7)
- Details on [vulnerability in Maker’s voting app](https://blog.zeppelin.solutions/technical-description-of-makerdao-governance-critical-vulnerability-facce6bf5d5e)
- [Detecting reentrancy issues using fuzzing](https://medium.com/consensys-diligence/detecting-reentrancy-issues-in-smart-contracts-using-fuzzing-e81474ba3a2e)

**Ecosystem**

- Ethereum Foundation, ConsenSys, Vitalik Buterin and Joseph Lubin to try to [join the Moloch grants DAO](https://molochdao.com/proposals) for 1000 ETH each. Meanwhile Metacartel to [fork Moloch for a grants DAO](https://medium.com/metacartel/forking-moloch-dao-d140a37d6649) to “coordinate the sharing of product insights and user data”
- [Soltix releases v0.1](https://github.com/eth-sri/soltix/releases/tag/v0.1) of automated framework for testing Solidity compilers
- More Burner Wallet house parties as onboarding to crypto: this time [in Australia with extension Burner Apps](https://medium.com/flex-dapps/we-used-a-burner-wallet-to-create-a-micro-economy-for-drunk-people-at-our-house-party-and-it-was-812b2d9f7a35) (somewhat similar to Austin’s Emojicoin exchange)
- EthDenver2018 winners resurface with [Elk](https://www.reddit.com/r/ethereum/comments/bkz1cd/im_working_on_a_development_board_for_building/), a dev board to prototype blockchain connected devices, in advance of June kickstarter
- [Dappnode v0.2](https://medium.com/dappnode/dappnode-goes-v0-2-0-5635399f24a0) - OpenVPN and Debian

**Enterprise**

- [Starbucks working to track its coffee bean supply chain](https://news.microsoft.com/transform/starbucks-turns-to-technology-to-brew-up-a-more-personal-connection-with-its-customers/) using Quorum
- EY has a [code security analyzer in private beta](https://www.ey.com/en_gl/news/2019/04/ey-launches-smart-contract-testing-service-for-blockchain-clients), indicating a strong dedication to Eth mainnet
- Tutorial on [AZTEC zero knowledge transactions in Pantheon](https://pegasys.tech/running-aztec-zero-knowledge-transactions-on-pantheon-tutorial/)
- Bloomberg [writeup on Societe General’s 100m euro](https://www.bloomberg.com/news/articles/2019-05-09/socgen-introduces-crypto-to-2-trillion-market-for-covered-bonds) covered bond
- Ajit Tripathi: [Enterprise blockchain is real](https://medium.com/@triptananda/enterprise-blockchain-is-real-552a83407af7)
- [US Treasury Dept is building a proof of concept for asset tracking on a private Eth chain](https://twitter.com/scott_lew_is/status/1125760179633565698)

**Governance and Standards**

- Akhunov: how [Ethereum governance really works](https://medium.com/@akhounov/ethereum-1x-as-an-attempt-to-change-the-process-783efa23cf60) and why he likes working groups as a process change
- Latest [core devs call](https://www.youtube.com/watch?v=CNcBuJ6wivE). [Notes](https://github.com/ethereum/pm/blob/27019db6d1088509251afc4ed926a982a0ecb517/All%20Core%20Devs%20Meetings/Meeting%2061.md).
- [ERC1996](https://github.com/ethereum/EIPs/pull/1996/files): Put tokens ‘on hold’
- [EIP2003](https://github.com/ethereum/EIPs/pull/2003/files): EVMC modules for implementations of precompiled contracts
- [ERC777 is finalized](https://eips.ethereum.org/EIPS/eip-777). An [ERC777 explainer](https://www.wealdtech.com/articles/understanding-erc777-token-contracts/).

**Application layer**

- Maker’s [multi-collateral Dai 101](https://github.com/makerdao/developerguides/blob/master/mcd/mcd-101/mcd-101.md). Also, per the bug disclosure this week, if you have [MKR in the old voting contract](https://www.reddit.com/r/MakerDAO/comments/ble9j1/notice_critical_update_to_governance_voting/), move it back to your wallet ASAP
- [Grid+’s Lattice1 hardware agent](https://blog.gridplus.io/lattice1-pre-sales-and-added-grid-redemption-functionality-3709feb43d21) in pre-sale with GRID discount. 60+ Texans signed up for power yesterday with Grid+
- [AuroraDAO rebranding to IDEX](https://medium.com/idex/aurora-dao-rebranding-to-idex-9611e5ef810f), claims more alltime trades than EtherDelta
- OpenLaw and 6 leading Canadian law firms [automate an M&A escrow agreement](https://medium.com/@OpenLawOfficial/leading-canadian-law-firms-collaborate-on-blockchain-based-smart-contract-project-b3fe1a6fa9a9)
- [Brave at 2m DAUs](https://twitter.com/BrendanEich/status/1126344850104696833)
- LiquidShare and PegaSys working on “[European post-trade settlement infrastructure for shares in small and medium sized enterprises](https://content.consensys.net/wp-content/uploads/PegaSys-x-LiquidShare-press-release_May-10.pdf)”
- [Deterministic art using block data](https://ethblockart.now.sh)
- Cent adds [messaging and ETH transfers](https://beta.cent.co/+xumglj)
- [William Shatner authenticates a collectible using Mattereum](https://twitter.com/WilliamShatner/status/1126698809566744577)

**Interviews, Podcasts, Videos, Talks** 

- [Joe Lubin](https://twitter.com/Shaughnessy119/status/1125412014933803008) on Chain Reaction
- Digix’s [Shaun Djie](https://ethhub.substack.com/p/digix-the-golden-path-forward-with) on Into the Ether
- [Edcon videos](https://www.youtube.com/watch?v=P4loHGCplX4&list=PL6-IF807eaBGtwcxiOCf4kO4IK7SGzDpK) going up
- Set Protocol’s [Felix Feng and Inje Yeo](https://simplecast.com/s/e92a5a78) on WyreTalks
- Agoric’s [Mark Miller](https://epicenter.tv/episode/286/) on Epicenter
- Zcash’s [Sean Bowe](https://www.zeroknowledge.fm/76) on Zero Knowledge
- [Vitalik interview](https://mybuild.techcommunity.microsoft.com/sessions/77290?source=sessions#top-anchor) at Microsoft Build

**Tokens / Business / Regulation**

- Uniswap’s [Unisocks](https://unisocks.exchange/), a limited edition, dynamically-priced pair of Uniswap socks. Price already up on the bonding curve from $12 to ~$35
- [RealT](https://medium.com/realtplatform/introducing-realt-tokenizing-real-estate-on-ethereum-9b8a995dc3fe) live with a rental house in Detroit. LLC owns property and tokenizes the LLC. Rent gets paid in Dai.
- [HumanityDAO](https://medium.com/marbleorg/introducing-humanity-90ddf9ead235): a TCR for sybil-resistance
- MyCrypto’s [token standard explainer](https://medium.com/mycrypto/the-technology-behind-ethereum-tokens-5615527e1af8)
- ConsenSys Legal and Latham&Watkins release [Automated Convertible Note](https://consensys.net/convertible-note/) on OpenLaw. Who needs the SAFT?
- Look out OTC: DutchX has [less slippage than exchanges for large orders](https://blog.gnosis.pm/dutchx-dai-auctions-challenge-c28dde0d489)
- LA Democrat Rep Brad Sherman renewed [his call to ban cryptocurrencies](https://twitter.com/coincenter/status/1126574631605997569)
- FinCEN released guidance on how they think [money transmission laws apply](https://www.fincen.gov/sites/default/files/2019-05/FinCEN%20CVC%20Guidance%20FINAL.pdf) to various subsets of crypto. This led Vitalik to write about [control as liability](https://vitalik.ca/general/2019/05/09/control_as_liability.html)
- SEC Commissioner Peirce speech on [interpreting](https://www.sec.gov/news/speech/peirce-how-we-howey-050919) _[Howey](https://www.sec.gov/news/speech/peirce-how-we-howey-050919)_ [for crypto](https://www.sec.gov/news/speech/peirce-how-we-howey-050919) warns that unclear guidance is pushing the industry outside of the US
- [CFTC ready to approve ETH futures](https://www.coindesk.com/cftc-would-approve-ether-futures-if-asked-insider-says), per Coindesk

**General**

- Binance got hacked for 7000 BTC. Some Bitcoin core devs suggested they should [roll back the chain for the entire day](https://www.reddit.com/r/ethereum/comments/bm4vxu/vitalik_buterin_ethereum_did_a_surgical_irregular/) to give the stolen BTC to miners instead of attackers. Eventually Binance chose not to try.
- ZkCapital is doing a [blockchain research weekly newsletter](https://zkcapital.substack.com/)
- [FloodXMR](https://eprint.iacr.org/2019/455.pdf) paper argues you could previously de-anonymize Monero by flooding transactions for a tiny annual sum. Unclear how much it would cost now.
- [Starkad and Poseidon](https://eprint.iacr.org/2019/458): New Hash Functions for Zero Knowledge Proof Systems

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- May 16 - [Eth2 workshop](https://www.eventbrite.com/e/road-to-interop-tickets-60384211803) (NYC)
- May 16 - [Token Summit](http://tokensummit.com/) (NYC)
- May 17-19 - [ETHNewYork](http://ethnewyork.com/)
- May 17 - Deadline to accept [proposals for Instanbul upgrade](https://en.ethereum.wiki/roadmap/istanbul) fork
- May 23-25 - [Swarm Orange Summit](https://www.eventbrite.com/e/swarm-orange-summit-madrid-2019-tickets-57378034245) (Madrid)
- May 24-26 - [Ethereum Madrid Hackathon](https://ethereummadrid.com/hackathon-2019/)
- May 27-28 - [EthCon Korea](https://ethcon.kr/) (Seoul)
- June 8-9 - [WASM in blockchains](https://avive.github.io/wasm_on_the_blockchain/#/) (Berlin)
- **June 10-11 [Blockchain for Social Impact conference](https://conference.blockchainforsocialimpact.com/) (NYC)**
- June 22-24 - [Zcon1](https://www.zfnd.org/zcon/) (Split, Croatia)
- July 3-5 - [WindingTree’s HackTravel](https://windingtree.com/hacktravel-lisbon-2019) (Lisbon)
- **July 19 - [BuildETH](https://www.buildeth.io) (San Francisco)**
- Aug 2-4 - [ETHIndia](https://ethindia.co/) (Bangalore)
- Aug 2-4 - [TruffleCon](https://www.truffleframework.com/trufflecon2019) (Redmond)
- Aug 21-23 - [Dappcon](https://dappcon.io/) (Berlin)
- Aug 23-25 - [ETHBerlin](https://ethberlinzwei.com/)
- Sep 16-17 - [Starkware sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- **Oct 8-11 - [DeVcon](https://devcon.org/) (Osaka)**

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I own Week In Ethereum. Editorial control has always been 100% me. 

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **It’s annoying how many link to the old URL. This is the new one: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/may-10-2019-week-in-ethereum-news/](https://weekinethereumnews.com/may-10-2019-week-in-ethereum-news/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

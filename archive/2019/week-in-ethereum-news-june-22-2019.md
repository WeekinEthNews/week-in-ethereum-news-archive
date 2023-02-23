---
title: "Week in Ethereum News<BR> June 22, 2019"
date: "2019-06-23"
---

## **Ethereum News and Links**

**Layer 1**

- [What’s New in Eth2](https://notes.ethereum.org/c/Sk8Zs--CQ/https%3A%2F%2Fbenjaminion.xyz%2Fnewineth2%2F20190621.html). Since it is the first issue in awhile, it’s a good summary of where Eth2 is at.
- [Nimbus Eth2 client dev update](https://our.status.im/nimbus-dev-update/) - up to date on spec. Nimbus and SigmaPrime’s Lighthouse clients are talking to each other.
- [Eth2 client interoperability plan](https://github.com/ethereum/eth2.0-pm/tree/master/interop/hobbits)
- [Near-instant transaction confirmation via staggered shard block production](https://ethresear.ch/t/near-instant-transaction-confirmation-via-staggered-shard-block-production/5643)
- CBC Casper: [efficient LMD GHOST](https://github.com/CarlBeek/CBC_LMD)

**Layer 2**

- [Phonon Network](https://blog.gridplus.io/the-phonon-network-59835328b799): scalable, private payment system using Grid+’s SafeCards. Alex and Karl also discuss Phonon on [Into the Ether](https://ethhub.substack.com/p/grid-lattice1-hardware-wallet-and)
- Connext to [release single-node v2.0 on Counterfactual](https://medium.com/connext/connext-update-10-4a3a8850b90) in July, followed by multihop in Q3
- An [overview of channels, Plasma and rollups layer2 scaling](https://nearprotocol.com/blog/layer-2/)
- Latest [Plasma implementers call](https://www.youtube.com/watch?v=5RpYoU6xD_M)

**Stuff for developers**

- [EthereumJS VM v4-beta](https://www.reddit.com/r/ethereum/comments/c2fdpk/ethereumjs_vm_v400beta1_release_typescript_evm/) a rewrite in TypeScript
- [Gas exactimation](https://medium.com/truffle-suite/ethereum-gas-exactimation-1158a996eb8c) in Ganache
- Tutorial: [implement an oracle in Solidity](https://medium.com/@pedrodc/implementing-a-blockchain-oracle-on-ethereum-cedc7e26b49e)
- The [Alethio API](https://medium.com/alethio/announcing-the-alethio-api-f5cfd55d8676). Amberdata [compares its API](https://medium.com/amberdata/which-blockchain-data-api-is-right-for-you-3f3758efceb1) to its competitors
- Loredana’s demo of a [file System with on-chain semantic search on dType, Ethereum](https://www.reddit.com/r/ethereum/comments/c3cpt6/file_system_with_onchain_semantic_search_on_dtype/)
- [Host your app with IPFS+ENS and access it via EthDNS](https://medium.com/the-ethereum-name-service/how-to-host-your-dapp-with-ipfs-ens-and-access-it-via-ethdns-c96046059d87)
- [8Pay for infinitely recurring subscriptions](https://medium.com/8pay/the-subscription-market-54994c93ef7b)
- [BurnerWallet Factory](https://medium.com/@dmihal/your-own-burner-wallet-in-3-minutes-introducing-the-burner-factory-prototype-48452e1ff48) - make your own in a few minutes
- [Cloudflare's Ethereum Gateway](https://blog.cloudflare.com/cloudflare-ethereum-gateway/)

**Ecosystem**

- [EF-supported teams: development update](https://blog.ethereum.org/2019/06/21/ef-supported-teams-development-report-2019-pt-1/). Extensive updates from each EF team.
- [Eth.wiki](https://eth.wiki/)
- Argent unveils [Hopper](https://medium.com/argenthq/introducing-hopper-mobile-web-friendly-privacy-for-ethereum-d02a8c400dad), “a zero-knowledge-based trustless mixer” to deposit 1 eth and withdraw to different address
- Better UX for noobs: [gas spectrum transactions](https://medium.com/authereum/gas-spectrum-transactions-bd34b65107b) (sign multiple transactions with a spectrum of gas prices)
- [Shiftly](https://medium.com/shiftly/introducing-shiftly-on-mainnet-find-the-best-prices-swap-instantly-c20e7218d795) - a bit like old-school Shapeshift using dexes

**Enterprise**

- [Ethereum Foundation joins Hyperledger and Enterprise Ethereum Alliance](https://www.reddit.com/r/ethereum/comments/c21fig/ethereum_foundation_joins_hyperledger_and/)
- Gartner: [7 mistakes to avoid in enterprise blockchain](https://itbrief.co.nz/story/seven-mistakes-to-avoid-in-blockchain-projects-gartner)
- [Quorum v2.2.4](https://github.com/jpmorganchase/quorum/releases/tag/v2.2.4)
- See also below: MetLife live on Eth mainnet

**Governance and Standards**

- Latest [core devs call](https://www.youtube.com/watch?v=Cl5zGk-3Ej4). Tim Beiko’s [live tweetstorm notes](https://twitter.com/TimBeiko/status/1142067867376136199) going through proposed EIPs. Accepted for Istanbul: EIP2024 blake2b precompile and EIP1702 generalized account versioning
- [EIP2124](https://github.com/ethereum/EIPs/issues/2125): Zero RTT chain compatibility check
- [EIP2123](https://github.com/ethereum/EIPs/blob/33d5f62fd6f89889102630df7d6f1088f08bdfff/EIPS/eip-2123.md): State-based Hard Fork Signaling
- [ERC2126](https://github.com/ethereum/EIPs/blob/bc1d1d6ea7eac55b2006509c46771046b84b95ca/EIPS/eip-2126.md): Signature Type Recognition
- Final: EIP1155 [Multi token standard](http://eips.ethereum.org/EIPS/eip-1155)
- Last call: EIP685 [chainID for JSON-RPC](http://eips.ethereum.org/EIPS/eip-695) and EIP1344 [chainID opcode](http://eips.ethereum.org/EIPS/eip-1344)

**Live on mainnet**

- Insurance giant [MetLife is live on mainnet with a pilot program](https://www.forbes.com/sites/stevenehrlich/2019/06/19/metlife-plans-to-disrupt-2-7-trillion-life-insurance-industry-using-ethereum-blockchain/#b3d229b27702) “to help loved ones quickly determine if the deceased was protected with a policy and automatically file a claim”
- [Ethsites](https://ethsites.io/), a censorship-resistant “registry of websites stored on the Ethereum blockchain” available through a Javascript snippet
- Treum (formerly Viant) live on mainnet [tracking and tracing commercial organic hemp](https://content.consensys.net/wp-content/uploads/Treum-_-June-20-2019-1.pdf)

**Application layer**

- [Augur v2 to integrate bZx](https://www.augur.net/blog/margin-lending/) for margin trading
- First [3rd party casino from RaketheRake goes live](https://funfair.io/crypto-casino-launch/) on FunFair
- [Pay as you use in Golem](https://blog.golemproject.net/pay-as-you-use-in-golem/), necessary in gWasm
- [Etherisc and Oxfam going live with insurance](https://www.linkedin.com/feed/update/urn:li:activity:6546696515849605120/) product for Sri Lankan farmers. Oxfam with ConsenSys and Sempo also [trials Dai for aid in Vanatu](https://www.coindesk.com/oxfam-trials-delivery-of-disaster-relief-using-ethereum-stablecoin-dai)
- Dharma now offers [customizable loans](https://blog.dharma.io/upgrading-our-borrow-experience-50693d23229c) to pick your own terms.
- Dai Stability Fee up for a [vote on going to 17.5%](https://blog.makerdao.com/executive-vote-stability-fee-17-5-june-21/)
- William Shatner isn’t just involved with Mattereum, he’s [founding a company to use Mattereum to track memorabilia](https://www.forbes.com/sites/michaeldelcastillo/2019/06/20/william-shatners-startup-brings-new-meaning-to-enterprise-ethereum/#68e101ff4c1f) provenance from creation

**Interviews, Podcasts, Videos, Talks** 

- Austin Griffith on [Hashing It Out](https://thebitcoinpodcast.com/hashing-it-out-49/) and [Wizard of Dapps](https://anchor.fm/wizardofdapps/episodes/Episode-7-Burner-Wallet-with-Austin-Griffith-e4cnjq)
- Grid+’s [Alex Miller and Karl Kreder](https://ethhub.substack.com/p/grid-lattice1-hardware-wallet-and) on Into the Ether
- Darma’s [Andrew Keys and James Slazas](https://twitter.com/Shaughnessy119/status/1141388580490813440) on ChainReaction
- Augur’s [Alex Chapman](https://www.youtube.com/watch?v=kpW08CiSK9g) on NEAR’s Whiteboard series
- Maker’s [Mariano Conti](https://medium.com/@TrustlessState/58-the-frontier-of-dai-with-mariano-conti-8e532cdc48a4) on POV Crypto
- Uniswap’s [Hayden Adams](https://epicenter.tv/episode/292/) on Epicenter

**Tokens / Business / Regulation**

- Sensitivity analysis of [Status sticker markets](https://our.status.im/token-economics-research-sticker-market/)
- [Two year retrospective on CryptoPunks](https://www.larvalabs.com/blog/2019-6-21-1-1/cryptopunks-two-year-anniversary). Last month the busiest since Jan 2018.
- YouNow/Props is going to do a [Reg A+ “offering” in order to give away Props](https://blog.propsproject.com/sec-filing-to-enable-millions-of-users-to-earn-and-use-props-tokens-448ed251f656). I wonder how many millions they had to spend in order to convince the SEC to let them give away tokens.
- [ACTUS and Polymath integration](https://medium.com/at-par/tokenize-all-financial-products-767e20780006) to offer nearly 100% of all financial instruments on Polymath
- [FATF international body wants countries to mandate sharing requirements](http://www.fatf-gafi.org/publications/fatfrecommendations/documents/public-statement-virtual-assets.html) for crypto exchanges

**General**

- Messaging app [Line is near approval for a crypto exchange in Japan](https://www.bloomberg.com/news/articles/2019-06-20/line-said-to-near-approval-of-japan-license-for-crypto-exchange)
- [Learning cryptography: finite fields](https://medium.com/loopring-protocol/learning-cryptography-finite-fields-ced3574a53fe) from Loopring
- Facebook’s Libra got [announced this week](https://developers.libra.org/docs/the-libra-blockchain-paper). Protolambda [compares Libra](https://twitter.com/protolambda/status/1141010796786401281) and says what they got [wrong vis a vis Eth1 and Eth2](https://twitter.com/protolambda/status/1141435774052818946)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- June 24- July 10 - [Gitcoin’s Beyond Blockchain](https://gitcoin.co/blog/beyond-blockchain-hackathon/) virtual hackathon
- June 25-27 - [EthPlanet hackathon](https://www.huodongxing.com/event/8495466131800) (Beijing)
- July 3-5 - [WindingTree’s HackTravel](https://windingtree.com/hacktravel-lisbon-2019) (Lisbon)
- July 19 - [BuildETH](https://www.buildeth.io/) (San Francisco)
- July 19-21 - [State of Scale](https://www.stateofscale.com/) (Los Angeles)
- July 22-23 - [Buidl](https://www.buidl.asia/) 2019 (Seoul)
- Aug 2-4 - [ETHIndia](https://ethindia.co/) (Bangalore)
- Aug 2-4 - [TruffleCon](https://www.truffleframework.com/trufflecon2019) (Redmond)
- Aug 21-23 - [Dappcon](https://dappcon.io/) (Berlin)
- Aug 23-25 - [ETHBerlin](https://ethberlinzwei.com/)
- Sep 3 - Deadline to [apply for EU Horizon Prize](https://ec.europa.eu/info/funding-tenders/opportunities/portal/screen/opportunities/topic-details/blockchain-eicprize-2019). 1m € each to 5 "Blockchains for Social Good" projects
- Sep 6-8 - [EthBoston](https://eth.boston/)
- Sep 15 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff/)
- Sep 15 - [Ethereal Tel Aviv](https://etherealsummit.com/events/ethereal-tel-aviv/)
- Sep 15-16- [StarkWare sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- Oct 8-11 - [DeVcon](https://devcon.org/) (Osaka)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I own 100% Week In Ethereum. Editorial control has always been me.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **It’s annoying how many link to the old URL. This is the new one: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [](https://weekinethereumnews.com/week-in-ethereum-news-june-22-2019/)[https://weekinethereumnews.com/week-in-ethereum-news-june-22-2019/](https://weekinethereumnews.com/week-in-ethereum-news-june-22-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

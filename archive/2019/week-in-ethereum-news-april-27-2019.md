---
title: "April 27, 2019"
date: "2019-04-28"
---

## **News and Links**

**Eth1**

- [Adjustable degrees of statefulness in Eth1 clients](https://medium.com/@akhounov/the-shades-of-statefulness-in-ethereum-nodes-697b0f88cd04). [Casey Detrio’s tweetstorm](https://twitter.com/cdetrio/status/1121848688727527424) also has useful context
- Ashikhmin and Akhunov: [Red Queen sync protocol](https://github.com/yperbasis/silkworm/blob/master/doc/sync_protocol_v1.pdf)
- [EVMC v6.2.0](https://github.com/ethereum/evmc/releases/tag/v6.2.0)

Eth2

- [Eth2.0 spec v0.6.0](https://github.com/ethereum/eth2.0-specs/releases/tag/v0.6.0)
- [Economic model of eth2 staking incentives](http://hackingresear.ch/economic-incentives/)
- [Prysmatic client update](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-26-prysmatic-labs-c32fb28c403f)
- A [Hobbits wire protocol explainer](https://medium.com/whiteblock/introducing-hobbits-a-lightweight-wire-protocol-for-eth-2-0-b1bfae5e4843)
- Eth2 phase2: [Fast cross-shard transfers via optimistic receipt roots](https://ethresear.ch/t/fast-cross-shard-transfers-via-optimistic-receipt-roots/5337)
- [Refinement and verification of CBC Casper](https://medium.com/layerx/cbc-casper-and-formal-verification-1954cbd1d971). Isabelle proof.

**Layer 2**

- Comparison between [state channel watchtower methods](https://medium.com/crypto-punks/lightning-vs-raiden-watchtowers-accountability-business-models-celer-pisa-833384f01ad0)
- Abridged: [layer 2 packaged up into an SDK](https://medium.com/abridged-io/abridged-launch-announcement-155b3eb9ef57) to make it easy for devs. Early access soon.

**Stuff for developers**

- ChainSecurity’s [VerX](https://medium.com/chainsecurity/verx-full-functional-verification-for-ethereum-contracts-now-at-your-fingertips-f8d20085e4ec) “automated verifier for certifyingcustom functional requirements” of Eth code
- Skale’s [C++ library for BLS Threshold Signatures](https://github.com/skalenetwork/libBLS)
- [launchdapp](https://www.reddit.com/r/ethereum/comments/bgxuwx/launchdapp_hosting_your_dapp_made_simple/) from Zastrin to make dapp frontend hosting easy
- An [overview of scaling now solutions](https://kauri.io/article/7ccaaa2fe7f344d5bf53807cb5c01530/v4/top-5-ways-to-scale-your-ethereum-blockchain-application-(dapp)) for architecting your dapp
- [eth-owl](https://www.reddit.com/r/ethdev/comments/bh6ezj/ethowl_now_supports_email_notifications_watch_any/): watch Eth address for transaction notifications by email. Much like [Dagger](https://matic.network/dagger/).
- [Smart contracts integration with Nethereum](https://kauri.io/article/b54334b0695342c1bbe161c4c4467b50)
- Truffle [v5.0.14](https://github.com/trufflesuite/truffle/releases/tag/v5.0.14). If you want to join the web3 revolution, join [Truffle University](https://www.reddit.com/r/ethdev/comments/bgm4kz/were_relaunching_truffle_university_and_wed_like/)
- [OpenZeppelin v2.3.0](https://forum.zeppelin.solutions/t/openzeppelin-2-3-0-release-candidate/572) release candidate

**Ecosystem**

- [Gnosis Safe gets formally verified](https://blog.gnosis.pm/formal-verification-a-journey-deep-into-the-gnosis-safe-smart-contracts-b00daf354a9c) by Runtime Verification
- The CryptoKitties folks called DapperLabs unveil their [Dapper smart contract wallet](https://medium.com/dapperlabs/why-dapper-is-a-smart-contract-wallet-ef44cc51cfa5)
- [Turms](https://medium.com/coinmonks/four-applications-of-turms-anonymous-message-transport-9505d9ba2388?sk=c9f856c778315de0a8b406d3747688f4): an expensive and slow encypted messaging between Eth addresses. Something like an onchain Earn.com
- [ETHCapeTown submissions](https://ethcapetown.devpost.com/submissions)
- [Pocket Network MVP is live](https://hackernoon.com/solving-full-node-centralization-pocket-core-mvp-release-35c220ac2b01): “a decentralized relay network for full-node infrastructure”

**Enterprise**

- “Societe Generale … [issued EUR 100m of covered bonds](https://www.societegenerale.com/en/newsroom/first-covered-bond-as-a-security-token-on-a-public-blockchain) as a security token, directly registered on the Ethereum blockchain.” The bonds were issued to itself; still an interesting pilot.
- [Nike files trademark for cryptokicks](https://www.bizjournals.com/portland/news/2019/04/24/nike-files-trademark-application-for-cryptokicks.html). Flashback to [EthDenver 2018](https://blog.aragon.org/aragon-ethdenver-recap-4a869a68bda2/), and sneaker tracking has always been something we’ve thought would happen.
- Coindesk reports [Samsung is developing an Ethereum-based chain](https://www.coindesk.com/samsung-developing-ethereum-based-blockchain-may-issue-own-token) and may do a token

**Live on mainnet**

- Set Protocol’s [Strategy Enabled Tokens](https://medium.com/set-protocol/tokensets-is-live-automate-your-crypto-portfolio-now-50f88dcc928d) are live on mainnet. Automated trading to buy the dumps and sell the pumps.
- [XYO Matrix](https://medium.com/xyonetwork/xyo-matrix-is-now-live-on-mainnet-f55e957aa49d) live on mainnet

**Governance and Standards**

- Latest [core devs call](https://www.youtube.com/watch?v=O_DE4NwOz9A). [Notes from the call](https://note.garden/blog/call-summary-ethereum-core-devs-no-60-april-26-2019/). ProgPoW audit funded and planned for next hard fork. Aiming for 6 month hard fork cycle.
- Mougayar’s [EF and spending proposals](http://startupmanagement.org/2019/04/22/how-ethereum-could-evolve/)
- [ERC1967](https://github.com/ethereum/EIPs/pull/1967/files): Standard Proxy Storage Slots
- [ERC1958](https://github.com/ethereum/EIPs/issues/1958): Smart contract functions payable in tokens
- [ERC1959](https://github.com/ethereum/EIPs/pull/1959): Valid chainID opcode
- [ERC1962](https://github.com/ethereum/EIPs/pull/1962/files): EC arithmetics and pairings with runtime definitions

**Application layer**

- [Brave Ads officially launches](https://brave.com/brave-ads-launch/). If you enable ads in the Rewards section, you get 70% of ad revenue with BAT
- bZx compares [their leverage tokens to dYdX’s leverage tokens](https://medium.com/bzxnetwork/how-do-fulcrums-ptokens-and-dydx-s-margin-tokens-compare-a3badae4b004)
- Dharma thinks their [14% lending rate can help generate Dai demand](https://blog.dharma.io/dharma-is-great-for-dai-80d4edfe696e) to restore the peg
- [Airswap Instant 2.0](https://medium.com/fluidity/airswap-instant-2-0-d10906447838)
- [Cent implements Fortmatic](https://beta.cent.co/+epeh7e) so its users don’t need a browser extension
- [Decentraland has avatars](https://decentraland.org/blog/announcements/explore-decentraland-in-style) now. Ever closer to Snow Crash.
- “[Wikipedia and Augur are public utilities](https://www.augur.net/blog/wikipedia-markets/).”
- Maker [stability fee to 16.5%](https://blog.makerdao.com/executive-vote-stability-fee-16-5/). Meanwhile, from the drama a few weeks ago, this is [Andy’s side](https://www.scribd.com/document/407743542/Zandy-s-Story) and [Matt’s side](https://old.reddit.com/r/MakerDAO/comments/bhzcgc/matts_story/) of the story

**Interviews, Podcasts, Videos, Talks** 

- [Justin Drake](https://www.zeroknowledge.fm/74) on Zero Knowledge
- bZx’s [Tom Bean & Kyle Kistner](https://blog.sendwyre.com/the-future-of-margin-lending-in-crypto-22dd07dd9a49) on Wyre Talks
- Dharma’s [Nadav Hollander](https://youtu.be/PdY0Pt9lVbI) talks to Brian Armstrong
- Giveth’s [Griff Green](https://epicenter.tv/episode/284/) on Epicenter
- [Austin Griffith](https://podcast.ethhub.io/austin-griffith-path-to-mass-adoption-with-the-burner-wallet) on Into the Ether

**Tokens / Business / Regulation**

- Dether debuts [continuous auctions/Harberger taxes](https://medium.com/dether/zone-out-a-new-way-to-own-land-on-ethereum-969b73b82bd4) for geographical exclusivity for sellers
- Burniske: [value capture and quantification](https://static1.squarespace.com/static/5a479ee3b7411c6102f75729/t/5cc352619055370001785494/1556304481918/Value+Capture+and+Quantification_+Cryptocapital+vs+Cryptocommodities.pdf)

**General**

- Etrade [launching Eth trading](https://www.bloomberg.com/news/articles/2019-04-26/e-trade-is-said-to-be-close-to-launching-cryptocurrency-trading)
- New York AG obtained a [local court order against Bitfinex/Tether](https://ag.ny.gov/press-release/attorney-general-james-announces-court-order-against-crypto-currency-company-under) that asserts that Tether was not fully backed. Bitfinex [responded](https://www.bitfinex.com/posts/356). Breaker points out a common thread: the [payment processor also dealt with Quadriga](https://breakermag.com/crypto-capital-is-the-common-thread-between-bitfinex-quadrigacx-and-other-troubled-exchanges/). Alex Miller’s [tldr is perfect.](https://twitter.com/crypto_dev_alex/status/1122135825746157568)
- [Fast hashing to BLS12-381](https://eprint.iacr.org/2019/403)
- Protocol Labs and Ethereum Foundation are [collaborating on VDF research](https://filecoin.io/blog/collaboration-on-vdfs/)

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Apr 29 - [Oslo Blockchain Day](https://osloblockchainday.no/)
- May 4 - [ENS Permanent Registrar](https://medium.com/the-ethereum-name-service/dns-permanent-registrar-and-hackathons-ens-development-summary-03-2019-401a30e6316d) launches
- May 9 - [Fluidity Summit](https://www.fluiditysummit.com/) (NYC)
- May 10-11 - [Ethereal](https://etherealsummit.com/?ref=weekinethereum) (NYC)
- May 16 - [Eth2 workshop](https://www.eventbrite.com/e/road-to-interop-tickets-60384211803) (NYC)
- May 16 - [Token Summit](http://tokensummit.com/) (NYC)
- May 17-19 - [ETHNewYork](http://ethnewyork.com/)
- May 17 - Deadline to accept [proposals for Instanbul upgrade](https://en.ethereum.wiki/roadmap/istanbul) fork
- May 23-25 - [Swarm Orange Summit](https://www.eventbrite.com/e/swarm-orange-summit-madrid-2019-tickets-57378034245) (Madrid)
- May 27-28 - [EthCon Korea](https://ethcon.kr/) (Seoul)
- June 8-9 - [WASM in blockchains](https://avive.github.io/wasm_on_the_blockchain/#/) (Berlin)
- June 22-24 - [Zcon1](https://www.zfnd.org/zcon/) (Split, Croatia)
- Aug 2-4 - [ETHIndia](https://ethindia.co/) (Bangalore)
- Aug 2-4 - [TruffleCon](https://www.truffleframework.com/trufflecon2019) (Redmond)
- Aug 21-23 - [Dappcon](https://dappcon.io/) (Berlin)
- Aug 23-25 - [ETHBerlin](https://ethberlinzwei.com/)
- Sep 16-17 - [Starkware sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- **[Oct 8-11 - DeVcon (East Asia)](https://twitter.com/EFDevcon/status/1120312795902377994)**

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I own Week In Ethereum. Editorial control has always been 100% me. 

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **It’s annoying how many link to the old URL. This is the new one: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/april-27-2019/](https://weekinethereumnews.com/april-27-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

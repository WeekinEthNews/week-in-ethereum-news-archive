---
title: "December 21, 2018"
date: "2018-12-21"
---

## News and Links

**Layer 1**

[What’s new in eth2](https://notes.ethereum.org/c/Sk8Zs--CQ/https%3A%2F%2Fbenjaminion.xyz%2Fnewineth2%2F20181219.html)

Notes from [last Eth2 call](https://github.com/ethereum/eth2.0-pm/blob/master/eth2.0-implementers-calls/call_008.md)

Vitalik wants [feedback on Eth2 materials](https://www.reddit.com/r/ethereum/comments/a6e0au/request_for_public_feedback_how_well_organized/)

Code for [Artemis](https://github.com/PegaSysEng/artemis), the Beacon chain Java client from PegaSys

ELI5: [randomness in Eth2 using a VDF](https://twitter.com/drakefjustin/status/1074813944039178241)

Combining [Avalanche RANDAO and VDFs](https://ethresear.ch/t/combining-avalanche-randao-and-verifiable-delay-functions/4544)

[Backwards-Forwards sync of Ethereum clients](https://ethereum-magicians.org/t/backwards-forwards-sync-of-ethereum-clients/2258) through requesting reverse diffs

On [raising the gas limit](https://ethereum-magicians.org/t/on-raising-block-gas-limit-and-state-rent/2249/4) (and storage management fees). Also a hypothetical on [how many magnitudes more throughput we can get from the PoW chain](https://ethereum-magicians.org/t/hypothetical-maximum-scale-of-eth-1-x/2264)

Mustafa Al-Bassam: [Towards on-chain non-interactive data availability proofs](https://ethresear.ch/t/towards-on-chain-non-interactive-data-availability-proofs/4602)

Vitalik: [discouragement attacks](https://github.com/ethereum/research/blob/master/papers/discouragement/discouragement.pdf)

**Layer 2**

- Raiden is live on mainnet! (see ahem, the live on mainnet section)
- Economics of [Loom Networks’ PlasmaChain](https://medium.com/loom-network/plasmachain-validator-staking-economics-part-1-e816d5825849) validators
- [Plasma Winter](https://github.com/matterinc/plasma_winter) account model Plasma with with zkSNARK proved state transitions
- [Payment channel protocol for light client server incentivization](https://ethereum-magicians.org/t/micropayment-technologies-for-service-incentivization/2237)

**Stuff for developers**

- [Truffle v5](https://truffleframework.com/blog/truffle-v5-has-arrived) is out of beta
- [Ganache v2 beta](https://github.com/trufflesuite/ganache/releases/tag/v2.0.0-beta.1)
- [MetaMask developer docs](https://metamask.github.io/metamask-docs/)
- Solidity [v0.5.2](https://github.com/ethereum/solidity/releases/tag/v0.5.2)
- web3j [4.1 for android out of beta](https://medium.com/blk-io/christmas-has-come-early-for-web3j-android-developers-27425534272b)
- [ZeppelinOS](https://github.com/zeppelinos/zos/releases/tag/v2.1.0-rc.0) and [OpenZeppelin](https://github.com/OpenZeppelin/openzeppelin-solidity/releases/tag/v2.1.0-rc.1) v2.1 releases candidates with Truffle 5 and Solidity 0.5.x
- State of Zeppelin’s [EVM packages](https://blog.zeppelinos.org/state-of-evm-packages-end-of-2018/?utm_campaign=weekinethereum)
- [Optimistic contracts](https://medium.com/@decanus/optimistic-contracts-fb75efa7ca84): assume data submission is legit until proven false, verified through bonding/slashing
- Piñata: the [power of IPFS as an on-demand CDN](https://medium.com/pinata/the-ipfs-network-c815a735bd0d)
- [RLP in Typescript](https://github.com/ethereumjs/rlp/releases/tag/v2.2.0)
- Walkthrough of [0x Instant and 0x Launch Kit](https://blog.0xproject.com/walkthrough-0x-instant-and-0x-launch-kit-c0fc0fefbc04)
- Austin Griffith [Burner Wallets 2.0](https://medium.com/@austin_48503/cypherpunk-speakeasy-v0-0-1-6e6b6b9cc884) in action to buy beer at blockchain meetup
- Steve Mark: [security issues in meta transactions](https://medium.com/consensys-diligence/silent-but-vulnerable-ethereum-gas-security-concerns-adadf8bfb180)
- Bingen Eguzkitza’s suggestions to [becoming a Solidity dev](https://blog.aragon.one/tips-and-tricks-to-get-started-with-solidity/)
- Ocean Protocol’s [Squid Libraries](https://blog.oceanprotocol.com/ocean-protocol-squid-library-java-c92a6035ce39) in JavaScript or Python to make it easier to build front ends or data pipelines on Ocean. Neat example of app using the [Squid libraries and Orbit db](https://outlierventures.io/research/ocean-protocol-orbit-db-machine-learning-app/) from Outlier Ventures

**Clients**

- PegaSys [0.8.3](https://github.com/PegaSysEng/pantheon/releases/tag/0.8.3) - hard fork ready
- [v6.0.0-beta.3 of the ethereum consensus tests](https://www.reddit.com/r/ethereum/comments/a7ghuj/v600beta3_of_the_ethereum_consensus_tests_has/)
- Progress on the [Mana client in Elixir](https://medium.com/poa-network/mana-ethereum-preparing-for-constantinople-d4c57af7d21f)
- [Eth on ARMbian](https://www.reddit.com/r/ethereum/comments/a7a339/ethereum_on_arm_etharmbian_is_now_hardforkready/). Geth and Parity images now hard fork ready (I got it wrong last week, sorry!)

**Ecosystem**

- [EthGlobal 2018 in review](https://medium.com/ethglobal/ethglobal-2018-wrap-up-and-looking-ahead-to-2019-d9676e141eca). 3,800 hackers (1000+ new to Solidity) from 65 countries. >500 projects submitted.
- Ethereum Foundation’s call to [identify impactful Eth dapps](https://ethereumfoundation.typeform.com/to/JJNqRP)
- Amberdata’s [Eth 2018 in review](https://2018.ethereuminreview.com/) data viz.
- Alethio on [miners choosing empty blocks](https://medium.com/alethio/a-minor-winter-270bea0c4dd2) for profit
- The VB Foundation donated 1k eth to [Prysmatic Labs](https://twitter.com/VitalikButerin/status/1075181710730506240), [Chainsafe](https://twitter.com/VitalikButerin/status/1075198387346116610) and [SigmaPrime](https://twitter.com/VitalikButerin/status/1075214050362093568) for their eth2 clients.
- [zkDAI](https://medium.com/@atvanguard/zkdai-private-dai-transactions-on-ethereum-using-zk-snarks-9e3ef4676e22): private Dai transactions with SNARKs
- Status proposal for [PRBS Whisper alternative](https://discuss.status.im/t/prbs-protocol-proposal-an-incentivized-whisper-like-protocol-for-status/849)
- [Radical Address](https://medium.com/@radicaladdress/radical-address-27f186380f02): simple ENS name purchasing
- ENS: Plans for [3-6 character name auction](https://discuss.ens.domains/t/announcing-the-ens-3-6-character-auction/754) starting at end of q1
- [Argent](https://medium.com/argenthq/a-new-era-for-crypto-security-57909a095ae3): no more seed phrases, instead a recovery account/multisig that does not have access to your assets. You can use a hardware wallet, a trusted friend or their Argent Guard service
- [Universal Logins update](https://medium.com/@avsa/universal-logins-update-new-live-demo-b3d5dcbec681). It has a [live demo](https://example.universallogin.io/)

**Live on mainnet**

- Raiden is [live on mainnet in alpha testing](https://medium.com/raiden-network/red-eyes-mainnet-release-announcement-d48235bbef3c). ie, break it, get bug bounty

**Enterprise**

- Societe Generale processed [the first letter of credit on Komgo](https://twitter.com/SG_CIB/status/1076183789402025984)
- Bloomberg says [Facebook is developing a Whatsapp stablecoin](https://www.bloomberg.com/news/articles/2018-12-21/facebook-is-said-to-develop-stablecoin-for-whatsapp-transfers?srnd=premium). My guess is that they eventually just give up and use a centralized database because they won’t be able to stomach giving up control.
- Blythe Masters [exits Digital Asset](http://fortune.com/2018/12/18/blythe-masters-digital-assets-blockchain/) for “personal reasons”
- LiquidShare’s [pilot platform for European SME post-trade infrastructure](https://www.liquidshare.io/pressmedia/liquidshare-launches-the-pilot-phase-of-its-blockchain-post-trade-infrastructure-for-erupean-smes/) opens on Euronext’s markets
- In January, Brazilian National Social Development Bank to launch [trial of collateralized real stablecoin on Eth mainnet](https://www.coindesk.com/this-brazilian-bank-is-using-ethereum-to-issue-a-stablecoin)
- Tyler Smith: [blockchain as industry data commons](https://medium.com/@rtylersmith/blockchain-used-as-an-industry-data-commons-278e57efa15c)

**Governance and Standards**

- The [dxDAO](https://blog.gnosis.pm/introducing-the-dxdao-27ec4301eced) to launch on April 4th to govern the DutchX protocol, with 50% of tokens going to those who trade on DutchX.
- Maker stability fee at 0.5%, [winning in a narrow vote](https://vote.makerdao.com/)
- All the links for the [Gangnam ProgPOW testnet](https://twitter.com/DontPanicBurns/status/1073930712317874176)
- [ERC820](https://eips.ethereum.org/EIPS/eip-820) is in last call
- [ERC1667](https://github.com/ethereum/EIPs/issues/1667): standard Plasma MVP

**Application layer**

- The [state of Gnosis](https://blog.gnosis.pm/the-state-of-gnosis-8cb9f49e3533): how it all ties together
- [DDEX is forking 0x](https://medium.com/hydro-protocol/why-we-are-forking-0x-97dc48ee0426) as the Hydro Protocol. [0x responds](https://blog.0xproject.com/ecosystem-update-ddex-and-the-0x-roadmap-5d201cafa133) and officially [rebrands to 0x](https://blog.0xproject.com/evolving-the-0x-brand-4158f06d795a).
- [0x ecosystem acceleration](https://blog.0xproject.com/announcing-the-0x-ecosystem-acceleration-program-89d1cb89d565) grants
- Uport and Ethense [educational certificates on your self-sovereign identity](https://medium.com/uport/ethense-and-uport-bring-educational-certificates-to-self-sovereign-identity-7a6b6c2f41c0)
- Update on insurance giant [AXA’s Fizzy flight insurance app](https://www.reddit.com/r/ethereum/comments/a66pgk/some_news_regarding_fizzyaxa_more_flights_open/): 70% flights covered, 10k transactions, mostly “from a B2B deal.”
- Atari games _[RollerCoaster Tycoon](https://www.animocabrands.com/atari-partners-with-animoca-brands)_ [and](https://www.animocabrands.com/atari-partners-with-animoca-brands) _[Goon Squad](https://www.animocabrands.com/atari-partners-with-animoca-brands)_ [coming to Ethereum](https://www.animocabrands.com/atari-partners-with-animoca-brands) in second half of 2019
- Exploring the [emerging crypto debt markets](https://blog.dharma.io/exploring-the-emerging-crypto-debt-markets-36e3800fd7c5)
- [MakerScan](https://makerscan.io/) is pretty slick.
- [Aragon v0.6.2](https://twitter.com/AragonOneTeam/status/1076054957957238784)
- [Golem v0.18.3](https://blog.golemproject.net/brass-golem-beta-0-18-3-7e76360deb7b)
- [Augur v1.8.6](https://github.com/AugurProject/augur-app/releases/tag/v1.8.6)
- DecryptMedia [profiles Grid+](https://decryptmedia.com/2018/12/20/electric-dreams/)
- Qoo10 [builds ecommerce platform](https://www.techinasia.com/qoo10-launches-blockchain-marketplace-cryptocurrency) where you can only use their token for purchases and listings.

**Interviews, Podcasts, Videos, Talks**

- [Martin Holst Swende](https://www.zeroknowledge.fm/56) on Zero Knowledge
- St Louis Fed Reserve’s [David Andolfatto](https://epicenter.tv/episode/266/) on Epicenter
- [Amir Taaki](http://thethirdweb.net/2018/12/17/amir-taaki-using-technology-to-reconstruct-the-social-moral-fabric/) with Arthur Falls
- [Afri Schoedon](https://itunes.apple.com/us/podcast/paritys-afri-schoedon-clients-serenity-g%C3%B6rli-private/id1438148082?i=1000426034048&mt=2) on 51Percent
- Latest
- Storj’s [Shawn Wilkinson and JT Olio](https://thebitcoinpodcast.com/hashing-it-out-34/) on Hashing It Out
- [Georgios Konstantoploulos](https://thebitcoinpodcast.com/hashing-it-out-33/) on Hashing It Out
- [Liam Horne](https://podcast.ethhub.io/scaling-ethereum-with-state-channels-liam-horne-of-l4-ventures) on Into the Ether

**Tokens / Business / Regulation**

- [Melonomics in a nutshell](https://medium.com/melonport-blog/everything-you-always-wanted-to-know-about-melon-but-were-too-afraid-to-ask-9ea3fda6d71f). I wouldn’t be surprised if many future token models look like this.
- Exploring [bonding curve collateral](https://medium.com/protea/exploring-bonding-curve-collateral-c37d4f922bbd)
- Kyle Samani’s [questions from the idea maze](https://multicoin.capital/2018/12/20/questions-from-the-crypto-idea-maze/)
- Scott Locklin explains the [Fisher equation of exchange and says crypto has velocity all wrong](https://basicattentiontoken.org/token-economics-considering-token-velocity/)
- Should be interesting to watch [Cashbet fraud lawsui](https://cryptobriefing.com/cashbet-lawsuit-ico-investor-claims/)t. Charlie Shrem was an advisor and they paid ArsenalFC for an ad.
- [Token Taxonomy Act](https://davidson.house.gov/media-center/press-releases/congressmen-warren-davidson-darren-soto-introduce-ico-fix-businesses): 3 Rs and 1 D in the US House intro a crypto bill during a lame duck session. Despite what crypto clickbait media may tell you, this does not augur particularly well for the US becoming more crypto friendly any time soon
- Coinbase head lawyer Brian Brooks in NYT: [America Could Lead the Transition to a Digital Currency Reserve](https://www.nytimes.com/2018/12/18/business/dealbook/digital-reserve-currency.html).
- Jurisdictional arbitrage in action: [Swiss government wants to become more crypto friendly](https://www.swissinfo.ch/eng/business/dlt-report_switzerland-sets-legal-foundations-for-blockchain-industry/44617654)

**General**

- Cosmos [Game of Stakes testnet](https://blog.cosmos.network/let-the-games-begin-21e66e34e2fd) goes live
- [Substrate 1.0 beta](https://medium.com/paritytech/substrate-has-arrived-f14f91536278) is out. AdEx released [payment channels on Substrate](https://github.com/adexnetwork/adex-protocol-substrate)
- [Reducing shielded proving time](https://z.cash/blog/reducing-shielded-proving-time-in-sapling/) in Zcash Sapling
- [Jarvis and Friday vulnerabilities found](https://drive.google.com/file/d/16NOFiKxoBqe3zeRAr7quUgRbcGQTitsL/view). Crypto peer review in action
- [Swingby](https://medium.com/swingby-protocol/introducing-swingby-2d2296ef12d0): hash timelocked BTC but minted as ERC20 token with collateralized ETH
- [wBTC update](https://blog.kyber.network/wbtc-progress-update-dec-2018-84e42b33843c). First wrapped BTC minted
- Bloomberg thinks [Tether has the money it says it does](https://www.bloomberg.com/news/articles/2018-12-18/crypto-mystery-clues-suggest-tether-has-the-billions-it-promised?utm_source=weekinethereum)
- Coinbase Earn launches. [Gain ZRX by learning 0x](https://blog.coinbase.com/earn-cryptocurrency-while-learning-about-new-digital-assets-cc2df3537fc7)
- [Facebook gave Spotify, Netflix and the New York Times access to all sorts of user data](https://www.nytimes.com/2018/12/18/technology/facebook-privacy.html), apparently including private messages
- Donate [Eth to Heifer International](https://medium.com/cryptocare/ethereum-social-impact-collaboration-donate-ether-to-support-heifer-international-61a382400744) (a longtime Nick Johnson favorite) and get an NFT

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Jan 10 - [Mobi Grand Challenge](https://mobihacks.devpost.com/) hackathon ends
- **Jan 10-Feb7 - [0x and Coinlist virtual hackathon](https://blog.0xproject.com/0x-coinlist-hackathon-3b48ddbfd21c)**
- Jan ~15 - Constantinople [hard fork at block 7080000](https://twitter.com/peter_szilagyi/status/1071052095535628288)
- **Jan 17 - [Aragon vote on funding](https://github.com/aragonone/flock/blob/master/teams/Aragon%20One/2019.md) original AragonOne team**
- Jan 29-30 - [AraCon](https://aracon.one/) (Berlin)
- Feb 7-8 - Melonport’s [M1 conf](https://m-1.melonport.com/) (Zug)
- Feb 15-17 - [ETHDenver](https://www.ethdenver.com/) hackathon (ETHGlobal) next hacker application round closes December 31st
- Feb 23-25 - EthAustin (EthUniversal)
- Mar 4 - [Ethereum Magicians](https://ethereum-magicians.org/t/ethmagicians-gathering-at-ethcc-2019-initial-call/2177) (Paris)
- Mar 5-7 - [EthCC](https://ethcc.io/) (Paris)
- **Mar 8-10 - [ETHParis](https://ethparis.com/) (ETHGlobal)**
- Mar 27 - Infura [end of legacy key support](https://blog.infura.io/infura-dashboard-update-9f02d0643eb3) (Jan 23 begins Project ID prioritization)
- Apr 19-21 - [ETHCapetown](http://ethcapetown.com/) (ETHGlobal)

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).

![: : ](https://d3b3sm9t19x0yd.cloudfront.net/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F88b0273f-b85b-40c3-b3a2-d2c6a37a0603_240x240)

I own Week In Ethereum. Editorial control has always been 100% me. If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

## **Use dapps - this issue is on [Cent](https://cent.co/)**

One of my best friends launched [Stoop](https://www.stoop.website/), an [Android](https://play.google.com/store/apps/details?id=com.stoop&hl=en)/[iOS](https://itunes.apple.com/sa/app/stoop-inbox/id1438978466?mt=8) newsletter reader. It uses a dedicated email and clean design experience to keep your information diet healthy. If you subscribe to newsletters, you will like it.

This issue is on Cent. Cool product, [growing rapidly](https://medium.com/cent-official/introducing-channels-editing-user-colors-copy-paste-and-nsfw-options-1396a32bfb7f), iterating fast. No commitments on future issues, but at least wanted to try it out for an issue. Check it out.

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

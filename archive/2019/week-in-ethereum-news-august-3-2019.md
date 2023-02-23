---
title: "Week in Ethereum News <BR> August 3, 2019"
date: "2019-08-03"
---

## **Ethereum News and Links**

**Layer 1**

- [Eth2 networking spec](https://github.com/ethereum/eth2.0-specs/blob/f3c11852d79bc5488b016c0538e2dd0a24609237/specs/networking/p2p-interface.md)
- Latest [Eth2 implementer call](https://www.youtube.com/watch?v=ReSiB2940AE). [Mamy’s notes](https://gist.github.com/mratsim/3c3c07da603bfedf417292d22b3eae33).
- Latest [What's New in Eth2](https://notes.ethereum.org/c/Sk8Zs--CQ/https%3A%2F%2Fbenjaminion.xyz%2Fnewineth2%2F20190802.html)
- [Lighthouse eth2 client update](https://lighthouse.sigmaprime.io/update-14.html): focused on testnet stability and networking
- [Lodestar eth2 client update](https://medium.com/chainsafe-systems/lodestar-updates-bb8be9386404): shifting to a browser-ready light client
- Robert Drost’s BuildEth [talk on execution environments](https://www.youtube.com/watch?v=gHWMEmM940o&feature=youtu.be) for phase 2 of eth2. Probably the easiest 10 minute explanation you will get.
- Updated [Eth2 mindmap](https://www.mindomo.com/mindmap/eth2-sharding-4408ec348bee4501aa125c3e3cd251d3)
- Vitalik’s twitter explainer of [stateless clients in context](https://twitter.com/VitalikButerin/status/1155566281229254657): markets for storage or data forever with free ride?
- [Spam resistant block creator selection via burn auction](https://ethresear.ch/t/spam-resistant-block-creator-selection-via-burn-auction/5851)
- [Multi-Threaded Data Availability On Eth 1](https://ethresear.ch/t/multi-threaded-data-availability-on-eth-1/5899)
- Slipper’s [EIP1559 implementation study](https://docs.google.com/document/d/1yqvvfrQ_He0fN1SsUcvZNBdyhv__d8-1QPyteCbNT6Q/edit#heading=h.7a2iqimr656z)

**Layer 2**

- [Raiden UI wizard](https://medium.com/raiden-network/introducing-the-raiden-wizard-6c7c61c5b695) onboarding tool

**Stuff for developers**

- Austin Griffith: an [intro to Eth for developers](https://medium.com/@austin_48503/intro-to-ethereum-development-a3821cc49ca0), livecoding video and writeup. Austin is now working on a [burner identity library](https://medium.com/@austin_48503/kirby-32491315c5)
- Samczsun finds another code vulnerability: [Livepeer slashing logic](https://samczsun.com/the-livepeer-slashing-vulnerability/)
- Understanding [ERC777 re-entrancy vulnerability if such a token were listed](https://blog.openzeppelin.com/exploiting-uniswap-from-reentrancy-to-actual-profit/) on Uniswap
- Zeppelin is kicking off a [cryptography for devs](https://forum.openzeppelin.com/t/the-crypto-in-cryptocurrencies-and-beyond/1107) series
- [EIP712 structs in Python](https://medium.com/treum_io/introducing-eip-712-structs-in-python-27eac7f38281)
- See the [whole execution flow for a given transaction](https://medium.com/tenderly/a-tenderly-update-debugging-ethereum-transactions-verifying-contracts-and-other-newsworthy-4d7f20317f92) with Tenderly
- [Elle](https://media.consensys.net/introducing-elle-a-formally-verified-evm-compiler-to-write-more-secure-ethereum-code-90d1038e1886): a formally verified EVM compiler building on Isabelle
- [websnark v0.0.5](https://github.com/iden3/websnark/releases/tag/v0.0.5). snark proof generation and verifier in WebAssembly. faster verification time in browser, verifiers for MNT6753-BoweGabizon and BN128-Groth16

**Ecosystem**

- [AWS $100k VDF competition](https://aws.amazon.com/blogs/startups/competition-forever-change-blockchain/) for people who like math and FPGA designs, sponsored by a coalition including Ethereum Foundation.
- Blockade Games tying [Lightning Network to Eth NFTs and code](https://medium.com/blockadegames/using-bitcoin-lightning-network-as-an-interface-to-ethereum-smart-contracts-7cbaecd05779). One of the most bullish things for Ethereum is how many Bitcoiners have to build on it.
- [Grid v1.5](https://medium.com/ethereum-grid/ethereum-grid-1-5-0-release-announcement-993c7047560a) - a desktop Eth tool UI, adds support for IPFS, RPC testing, Geth 1.9.
- If you haven’t seen Alethio’s monthly [data viz of DeFi users](https://medium.com/alethio/the-defi-series-monitoring-activities-user-community-growth-f274946d0ac9) that’s all over social media, it’s worth a click.
- [Smart wallets to solve key management](https://blog.gnosis.pm/smart-wallets-are-here-121d44519cae) with 2fa and social recovery.
- If you want to advertise to Eth devs, Codefund now has exclusive [advertising on Etherscan’s testnet pages](https://twitter.com/codefundio/status/1156248412020465664). I asked Etherscan for testnet-only ads awhile back, so it’s great to see it

**Enterprise**

- How PegaSys is [setting the standard for permissioning](https://media.consensys.net/how-pegasys-is-setting-the-standard-for-permissioning-in-dlt-3112615ae70b) with the Pantheon v1.2 client by whitelisting accounts on mainnet.
- [Ondiflow and BP pilot for onshore oilfield tracking activities](https://www.ondiflo.com/news073019) on a private chain automated with IoT data

**Governance and Standards**

- Latest [core devs call](https://youtu.be/fJd_xYnYrUU?t=542). Tim Beiko’s [summary](https://twitter.com/TimBeiko/status/1157299093259137024). Per the pull request showing the Istanbul EIP [decisions made on the call](https://github.com/ethereum/EIPs/pull/2226/files), EIPs 663, 1380, 1985, 2045, and 2046 were added as “tentatively accepted.” There was discussion around doing a second Instanbul fork and/or when to do the next fork after Istanbul. Disappointingly, the call lacked a rep from Geth as well as Parity.
- [ERC2225](https://github.com/ethereum/EIPs/blob/1f0704654ef09d0f746e210bc33b0ab71ed50f17/EIPS/eip-2225.md): Methods to merge EVM chains
- [ERC2222](https://github.com/ethereum/EIPs/issues/2222): fund distribution token standard
- [ERC2224](https://github.com/ethereum/EIPs/blob/e525876afe867dcffbe48d93875a04fd2d0fd006/EIPS/eip-2224.md): Automatic signature request (wallet\_autoSign)

**Application layer**

- You can now [tip for tweets](https://brave.com/tip-with-brave/) in the latest version of Brave
- Augur’s [affiliate plan](https://www.augur.net/blog/augur-affiliate-referrals/). Also a 3 minute survey for [anyone who has ever tried to use Augur](https://twitter.com/AugurProject/status/1156247557661609984)
- Decentraland [private beta looks impressive](https://decentraland.org/blog/project-updates/client-private-beta/)
- Set’s [moving average tokens rebalanced](https://twitter.com/SetProtocol/status/1157318449011363841) for the first time, with a 23% gain in Eth for holders. Here’s a thread on the [dutch auction rebalancing](https://twitter.com/SetProtocol/status/1156620239833985024).
- [0x introduces coordinators](https://blog.0xproject.com/0x-roadmap-2019-part-5-introducing-coordinators-1406365ecbd) - execution rules for a specific pool of liquidity.
- Spankchain’s SpankPay: a [payment rail for the adult industry](https://medium.com/spankchain/spankchain-launches-spankpay-a-crypto-payment-solution-with-its-first-two-partners-c734b85d355)
- [Create an open investment bank using OpenLaw](https://medium.com/@OpenLawOfficial/build-an-open-investment-bank-using-openlaw-c11f2d56057f). They’ll also implement E&Y’s Nightfall. [Dai invoices on OpenLaw](https://twitter.com/r_ross_campbell/status/1156585643251834883) look slick.

**Interviews, Podcasts, Videos, Talks** 

- Maker’s [Rune Christensen](https://epicenter.tv/episode/298/) on Epicenter
- MetaCartel’s [Peter Pan](https://ethhub.substack.com/p/metacartel-improving-and-funding) on Into the Ether
- [Ben Fisch](https://www.zeroknowledge.fm/88) talks accumulators on Zero Knowledge
- Nexus Mutual’s [Hugh Karp](https://anchor.fm/wizardofdapps/episodes/Episode-13-Nexus-Mutual-with-Hugh-Karp-e4qe6l) on Wizard of Dapps

**Tokens / Business / Regulation**

- SEC is soliciting bids for [Ethereum and Bitcoin data feeds](https://www.fbo.gov/index.php?s=opportunity&mode=form&id=82573739c2786e1342a89ef8be47d060&tab=core&tabmode=list&=)
- Loopring [LRC staking](https://medium.com/loopring-protocol/loopring-3-0-lrc-utility-model-d7da9ac79d3d): lockup your LRC for fees, plus dexes stake for reputation and/or fee reduction
- [NBA and DapperLabs (CryptoKitties) announce NFT collecitibles for moments](https://medium.com/dapperlabs/nba-bb67f4a2861d) like Kawhi’s fall away buzzer beater. The sale should be live in time for the NBA season with the associated game in 2020.
- [Stablecoin transaction volume on Ethereum passes Venmo](https://tradeblock.com/blog/stablecoin-on-chain-transaction-volumes-soar-outpace-venmo)

**General**

- A daily log of [what the Ethereum ecosystem shipped in July](https://concourseopen.com/blog/30-days-of-eth-july-2019/)
- [MyCrypto Summer](https://medium.com/mycrypto/mycryptosummer-has-launched-f967b93be57) crypto education series. Send this to your friends
- Lefteris’ [crypto portfolio analytics and tax prep software](https://github.com/rotkehlchenio/rotkehlchen/releases/tag/v1.0.0) Rotkehlchen v1 release
- [Cosmos staking pools appear to be headed to zero fees](https://forum.cosmos.network/t/on-the-interrelationship-between-the-security-budget-and-the-business-prospects-of-the-cosmos-network/2547)
- Zooko asks [Zcash community to keep block funding](https://medium.com/@zooko_25893/a-personal-letter-about-the-possibility-of-a-new-zcash-dev-fund-f6d30df64392)
- LocalEthereum planning on [adding trusted third party identity attestations](https://blog.localethereum.com/preventing-identity-theft-with-optional-id-verification/index.html?utm_source=r3).

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- **Aug 4 - deadline to [apply for re-opening of Devcon speaker, builder, student](https://blog.ethereum.org/2019/07/29/devcon-updates-announcing-wave-2-a-new-application-window-and-more/) applications**
- Aug 5-Sep 22 - [IDEO virtual hackathon](https://coinlist.co/build/ideo)
- **Aug 6 - Devcon [tickets, wave 2](https://blog.ethereum.org/2019/07/29/devcon-updates-announcing-wave-2-a-new-application-window-and-more/)**
- **Aug 10 - ENS [shortname reservation ends](https://discuss.ens.domains/t/an-update-on-the-short-name-reservation-process/1091)**
- Aug 15 - [Grow Ethereum](https://hackathons.gitcoin.co/grow-ethereum/) virtual hackathon ends
- Aug 16 - 18 - [ConsenSys Grants hackathon](https://pages.consensys.net/toronto-grants-hackathon) (Toronto)
- Aug 21-23 - [Dappcon](https://dappcon.io/) (Berlin)
- Aug 23 - [Last day for IDEX withdrawals](https://medium.com/idex/idex-kyc-transition-period-and-updated-asset-availability-for-us-markets-set-to-begin-d45e945f842d) without KYC
- Aug 23-25 - [ETHBerlin](https://ethberlinzwei.com/)
- Aug 29-30 - [ERC1400 security token hackathon](https://medium.com/@ramvi/invitation-to-hackathon-in-oslo-29-30-august-1d8ec54a26ad) (Oslo)
- Sep 2-16 - [Decentraland SDK virtual hackathon](https://hack.decentraland.org/?with=weekinethereum) (250k USD in prizes. There’s a referral code on that link that gets both you and me something extra)
- Sep 3 - Deadline to [apply for EU Horizon Prize](https://ec.europa.eu/info/funding-tenders/opportunities/portal/screen/opportunities/topic-details/blockchain-eicprize-2019). 1m € each to 5 "Blockchains for Social Good" projects
- Sep 6-8 - [EthBoston](https://eth.boston/)
- Sep 15 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff/)
- Sep 15 - [Ethereal Tel Aviv](https://etherealsummit.com/events/ethereal-tel-aviv/)
- Sep 15-16- [StarkWare sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- Oct 7 - [ENS workshop](https://medium.com/the-ethereum-name-service/ens-workshop-applications-are-now-open-f46db6c63384) (Osaka)
- Oct 8-11 - [DeVcon](https://devcon.org/) (Osaka)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I own 100% Week In Ethereum. Editorial control has always been me.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **This headline stays as long as so many people continue to link to old URL and not the right one: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/week-in-ethereum-news-august-3-2019/](https://weekinethereumnews.com/week-in-ethereum-news-august-3-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

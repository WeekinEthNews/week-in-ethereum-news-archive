---
title: "Week in Ethereum News <BR> August 8, 2021"
date: "2021-08-08"
---

## **Eth News and Links**

**Mainnet execution layer - London fork happened and 1559 is live!**

- Latest [core devs call](https://youtu.be/jNxAB3WpAD0?t=189) video. Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1423673711127842821); shortest call ever assessing the smooth success (so far!) of the London upgrade
- 1559 monitoring and ETH burning dashboards: [Etherchain Burn](https://etherchain.org/burn), [Watch the Burn](https://watchtheburn.com/), [Ultrasound Money](https://ultrasound.money/), [Python script to show boxplots](https://github.com/perama-v/fee-feed) from your node, [Otterscan](https://github.com/wmitsuda/otterscan/releases/tag/v2021.07.05-otterscan) (uses your Erigon node).
    - After 3 days, over 15k ETH burned
- An 1559 [fee estimator for the next block](https://www.blocknative.com/gas-estimator)
- On the first day, 1559 led to [negative issuance](https://twitter.com/k06a/status/1423360055571791872) for half an hour
- Wallets beginning to support 1559 transactions, eg [MetaMask extension](https://twitter.com/danfinlay/status/1423340794199429124) starts this week. There was a last minute [wallet UX issue](https://twitter.com/gregthegreek/status/1422692406114271232) leading to web3js and Infura hotfix releases pre-London
- 1559 doesn’t reduce gas fees, here’s some [things to keep in mind](https://twitter.com/trent_vanepps/status/1423353532200198145) during transition
- Ansgar: how [1559 reduces MEV and gives it to the protocol](https://hackmd.io/@adietrichs/eip-1559) by bifurcating the inclusion and ordering markets for transactions
- Some debate in the [address extension space](https://ethereum-magicians.org/t/thoughts-on-address-space-extension-ase/6779) research area

**EIPs/Standards**

- [EIP3709](https://github.com/ethereum/EIPs/blob/d67798b2646da04dfa82dd1443cc7c0a6d90e60e/EIPS/eip-3709.md): deprecate transaction type 1

**Proof of stake consensus layer**

- [A model for cumulative committee-based finality](https://ethresear.ch/t/a-model-for-cumulative-committee-based-finality/10259), a possible alternative to CBC in the future
- What’s coming in [prysm v2 for stakers](https://medium.com/prysmatic-labs/changes-coming-in-prysm-v2-stakers-need-to-know-be2601fbd4f5); breaking changes for Altair fork
- [Dafny](https://github.com/ConsenSys/eth2.0-dafny), official release of formally verified spec of Eth staking
- [ethmodel.io](https://www.ethmodel.io/): cadCAD’s simulator of total ETH supply and staking yield

**Layer2**

- Arbitrum to [launch this month](https://offchain.medium.com/a-is-for-arbitrum-a-is-for-august-71391582d95b) in a few weeks with some safety rails
- [NXTP](https://twitter.com/ConnextNetwork/status/1423677600350842890) for crosschain transfers and contract calls from Connext. Onchain data model only, uses subgraphs

* * *

### **This newsletter is made possible thanks to [Kwenta](https://kwenta.io/) by [Synthetix](https://synthetix.io/)!**

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F49469a41-f71d-47b3-af75-483b2e24a735_1024x512.jpeg)](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F49469a41-f71d-47b3-af75-483b2e24a735_1024x512.jpeg)

[Kwenta](https://kwenta.io/) enables traders to access real-world and derivative assets on-chain using the power of the Synthetix protocol. 

Long or short popular synthetic cryptocurrencies, commodities, forex, and equities without the limits or compromises of a centralized exchange. 

You can now also use [L2 Kwenta on Optimism](https://blog.kwenta.io/everything-you-need-to-know-about-using-kwenta-on-l2/) for low gas fees and blazing fast transactions!

* * *

**Stuff for developers**

- web3js [v1.5.1](https://github.com/ChainSafe/web3.js/releases/tag/v1.5.1) - should update for 1559
- [web3J](https://blog.web3labs.com/announcing-web3j-support-for-eip-1559) adds 1559 support for Java devs
- Nethereum [v4.0.2](https://github.com/Nethereum/Nethereum/releases/tag/4.0.2) supports Eth\_FeeHistory for v1.10.6 until next Geth release
- Switch to [WalletConnect v1.5.2](https://twitter.com/WalletConnect/status/1421092594365472773) ASAP
- [UseDapp](https://medium.com/ethworks/introducing-usedapp-developer-tools-d52fe77e8230) - browser extension to give you developer tools network tab in web3 frontends
- [Hardhat packager](https://github.com/paulrberg/hardhat-packager) plugin to prepare artifacts and TypeChain bindings for registry deployment
- [How to fork mainnet with Hardhat](https://www.quicknode.com/guides/web3-sdks/how-to-fork-ethereum-mainnet-with-hardhat) step by step
- [Reorgme](https://github.com/0xsequence/reorgme): create reorgs on private chains
- [sol2uml](https://www.npmjs.com/package/sol2uml) now supports file-level structs and enums which Solidity introduced in 0.6.x
- abi-to-sol [v0.5](https://github.com/gnidan/abi-to-sol/releases/tag/v0.5.0) accepts custom errors in input ABIs and corresponding outputs
- [Login with Eth](https://twitter.com/isaacpatka/status/1422188383472848897) quickstart for devs
- build an [AssemblyScript chain on TheGraph](https://twitter.com/DennisonBertram/status/1421809775889817604), Dennison Bertram PoC
- If Santi Palladino was writing his [Eth for web devs](https://twitter.com/smpalladino/status/1421901085279756300) book now…

**Security**

- Popsicle Finance [hacked for ~$25m](https://twitter.com/Mudit__Gupta/status/1422797923037814786) via new depositors allowed to withdraw rewards from deployment; same bug as WildCredit
- Ashiq Amien finds [access control bug in Alchemix](https://medium.com/immunefi/alchemix-access-control-bug-fix-debrief-a13d39b9f2e0)
- Fake partnership via [Andre Cronje deepfake video call](https://blackswantoken.medium.com/the-andre-cronje-mis-hap-fake-partnership-cryptocurrency-fraud-678eef5f0c75)?
- Using a honeypot to [investigate Twitter reply scams](https://blog.mycrypto.com/investigating-twitter-reply-scam-rings/)
- Want to be an auditor? [Secureum](https://twitter.com/0xRajeev/status/1423166798438932485) bootcamp is extending the application deadline (it’s free!)

**Ecosystem**

- [Eth scalability roadmap](https://www.reddit.com/r/ethfinance/comments/ovudmr/roadmap_from_the_end_users_perspective/) from a user’s POV
- Bot on bot MEV violence: [tx.origin arb bot executes attacker’s arbitrary call](https://twitter.com/bertcmiller/status/1421543854856146947). Now made [~$1m](https://twitter.com/bertcmiller/status/1421806913101180938)
- Videos from yesterday’s [reorg.wtf online summit](https://hackmd.io/cEw2Z-QcR1yvQ8wAeQZdnQ)
- [Rabby browser extension](https://rabby.io/) (open source, forks at least some of MetaMask, caveat emptor)
- [Ethereum miner revenue higher than Bitcoin](https://www.theblockcrypto.com/linked/113234/ethereum-miner-revenue-higher-than-bitcoins-for-third-month-running) for the 3rd consecutive month

**Enterprise**

- GoQuorum [v21.7.0](https://github.com/ConsenSys/quorum/releases/tag/v21.7.0) - new consensus engine for the QBFT algorithm.
- Hyperledger Besu [v21.7.2](https://github.com/hyperledger/besu/releases/tag/21.7.2) - some hotfixes for London

**Application layer - all the focus on London**

- Louis Vitton launches “[Louis the Game](https://twitter.com/wenewmoments/status/1422914158740213760)” with NFTs on Ethereum
- [Oiler Network has an alpha on mainnet](https://alpha.oiler.network/) (with fake USDC) for 1559-enabled gas hedging
- A simple [bill splitting app](https://twitter.com/mikery/status/1422095060691300352)
- More [Real World Assets for Maker](https://twitter.com/mrabino1/status/1423662915283001346): Matthew Rabinowitz starts Delaware trust for corporate office leases
- You can get [~7% fixed APR on USDC at Element](https://app.element.fi/pools/0x787546Bf2c05e3e19e2b6BDE57A203da7f682efF) (disclosure: Evan is an advisor; of course there’s code risk, but that’s a solid fixed rate)

**Regulation/business/tokens**

- US Senate drama: Yellen’s Treasury Dept glommed crypto regulations onto Biden’s trillion dollar infrastructure bill; Wyden (D-OR), Lummis (R-WY), Toomey (R-PA) amendment to make the anti-crypto regulations less bad, but Warner (D-VA), Portman (R-OH) and Sinema (D-AZ) create special carve out for PoW (and later other favored tech). Biden pushed Warner's special carve out for PoW miners.
    - Votes are supposed to be today, follow [Jake Chervinsky](https://twitter.com/jchervinsky) on Twitter for updates. Currently it appears leadership is pressuring for a compromise
    - Ryan Selkis compiled some [undecided Senators](https://twitter.com/search?q=%40twobitidiot%20are%20you%20planning%20to%20support&src=typed_query&f=live): Lujan (D-NM), Collins (R-ME), Merkley (D-OR), Cantwell (D-WA), Bennett (D-CO), Manchin (D-WV), Markey (D-MA), Van Hollen (D-MD), Cortez Masto (D-NV), Rosen (D-NV), Gillibrand (D-NY), Cassidy (R-LA), Romney (R-UT), Hickenlooper (D-CO), Kelly (D-CO), Tuberville (R-AL), Hagerty (R-TN), Ossoff (D-GA)
- You can’t be tough on BigTech [while trying to kill off alternatives](https://www.techdirt.com/articles/20210805/16245947312/you-cant-be-tough-big-tech-while-killing-off-alternatives-to-it.shtml) to it
- SEC settles with [DMM to disgorge profits from token sale](https://www.sec.gov/news/press-release/2021-145) and pay $125k individual fines
- JP Koning: [stablecoins are regulated](https://jpkoning.blogspot.com/2021/08/stablecoin-regulatory-strategies.html)
- Justin Drake’s updated [model for Eth supply and sell pressure reduction](https://docs.google.com/spreadsheets/d/1vrK5sY5ooq-F8dcyRhmmAJ5YtgkvWKWP3OfGCZIYxSA/edit#gid=0)
- Vineyard Holdings: a [DCF valuation model for Eth](https://vineyardholdings.net/2021/07/31/ethereum/)
- Nikhil Shamapant: [1559 and the triple halving thesis](https://squish.substack.com/p/eip1559-the-squish-chaos-edition)

**General/crypto**

- Facebook opensources [Winterfell](https://engineering.fb.com/2021/08/04/open-source/winterfell/) STARK prover/verifier
- If you’re doing a trusted SNARK setup, [try this easy to use UI](https://medium.com/privacy-scaling-explorations/trusted-setup-ui-update-f8f95fc17a37)
- Online courses on [Probabilistically Checkable Proofs](https://www.youtube.com/playlist?list=PLGkwtcB-Dfpyqf_fV6S8PiwVdRN695yh4) and [Interactive Proofs](https://www.youtube.com/playlist?list=PLGkwtcB-DfpyjJfxPUdwWpg_ygk2OIp9-) by Ale Chiesa and Tom Gur
- [Blind signatures over elliptic curves](https://arnaucube.com/blog/blind-signatures-ec.html) explainer
- Apple inserts backdoor to [scan your phone](https://www.eff.org/deeplinks/2021/08/apples-plan-think-different-about-encryption-opens-backdoor-your-private-life) in violation of their [privacy promise](https://twitter.com/matthew_d_green/status/1424003292401741825)
- Google [employees regularly browse your data](https://www.vice.com/en/article/g5gk73/google-fired-dozens-for-data-misuse)
- [Pplpleaser profile](https://fortune.com/2021/08/06/nft-art-pplpleasr-fortune-cover-ethereum-defihow-crypto-changed-my-life/) in Fortune

* * *

## **Job Listings**

- [Founding auditor at Yearn's yAcademy](https://yacademy.github.io/jobs/), $10,000 referral reward if hired
- Solidity is [hiring a C++ dev](https://ethereum.bamboohr.com/jobs/view.php?id=40&source=weekinethnews)
- WalletConnect looking for [Javascript/Typescript devs](https://twitter.com/WalletConnect/status/1421397382391078924)
- Rotki tracking and tax app hiring [Python backend dev](https://rotki.com/jobs/backend/) & [Vue/Typescript dev](https://rotki.com/jobs/frontend)
- Ethereum Foundation: [Test Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=39) for consensus and execution layers
- Nethermind [internship program](https://www.notion.so/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-8-2021/](https://weekinethereumnews.com/week-in-ethereum-news-august-8-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Aug 12 - applications close for [EF small grants for events](https://esp.ethereum.foundation/en/devcon-grants/)
- Aug 13 - [Sign in with Ethereum RFP](https://notes.ethereum.org/@djrtwo/sign-in-with-ethereum-RFP) extended deadline
- Aug 13 - Post-London assessment [wallet/infra call](https://github.com/ethereum/pm/issues/369)
- Aug 17 - applications close for [written pieces on public goods projects](https://gitcoin.co/blog/seeking-a-new-kind-of-public-good/)
- Aug 27-29 - [Edcon](https://www.edcon.io/) (Shenzhen/online)
- Oct 1-3 - [EthAtlanta](https://ethatl.com/) enterprise-focused hackathon & keynotes
- Oct 22-24 - [ETH Lisbon](https://ethlisbon.org/)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

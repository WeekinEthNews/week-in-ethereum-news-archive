---
title: "Week in Ethereum News <BR> January 19, 2020"
date: "2020-01-19"
---

## **Eth News and Links**

**Eth1**

- Notes from the [latest eth1 research call](https://blog.ethereum.org/2020/01/17/eth1x-files-digest-no-2/). How to get to binary tries.
- Guillaume Ballet argues for [WASM precompiles for better eth1](https://medium.com/@gballet/improving-scalability-withwasm-precompiles-df75e536f93e) to prepare for eth2
- StarkWare mainnet tests find that a much [bigger block size does not affect uncle rate](https://ethereum-magicians.org/t/eip-2028-transaction-data-gas-cost-reduction/3280/35) and argues that a further decrease in gas for transaction data would be warranted
- Guide to running [Geth/Parity node or eth2 Prysm/Lighthouse testnet on Raspberry Pi4](https://www.reddit.com/r/ethereum/comments/epxy8l/ethereum_on_arm_ethereum_1020_ecosystem/)
- Nethermind [v1.4.8](https://github.com/NethermindEth/nethermind/releases/tag/1.4.8)

**Eth2**

- The [incentives for good behavior and whistleblowing](https://blog.ethereum.org/2020/01/13/validated-staking-on-eth2-1-incentives/) in Eth2 staking
- Danny Ryan’s [quick Eth2 update](https://blog.ethereum.org/2020/01/16/eth2-quick-update-no-7/) - updated docs explaining the spec currently under audit
- Options for [eth1 to eth2 bridges and phase1 fee market](https://ethresear.ch/t/phase-1-fee-market-and-eth1-eth2-bridging/6775)
- [Simulation environment for eth2 economics](https://github.com/ethereum/rig/blob/master/eth2economics/code/beaconrunner/beacon_runner.ipynb)
- Ryuya Nakamura proposes the [subjective finality gadget](https://ethresear.ch/t/casper-ffg-meets-subjective-finality/6764)
- [Lighthouse client update](https://twitter.com/paulhauner/status/1217349576278999041) - 40x speedup in fork choice, 4x database speedup, faster BLS
- [Prysmatic client update](https://medium.com/prysmatic-labs/eth-2-0-dev-update-42-mainnet-capable-testnet-now-hiring-53d4d08d3901) - testnet with mainnet config
- A guide to [staking on Prysmatic’s testnet](https://medium.com/@steve.berryman/installing-and-running-an-ethereum-2-prysm-validator-on-the-testnet-c004dd7eece8)
- How to [build the Nimbus client on Android](https://our.status.im/building-nimbus-on-android/)
- [Evaluating Eth2 staking pool](https://www.attestant.io/posts/evaluating-staking-services/) options

**Layer2**

- Plasma Group -> [Optimism](https://medium.com/ethereum-optimism/optimism-cd9bea61a3ee), raises round from Paradigm/ideo for optimistic rollups
- [Auctioning transaction ordering rights](https://ethresear.ch/t/mev-auction-auctioning-transaction-ordering-rights-as-a-solution-to-miner-extractable-value/6788) to re-align miner incentives
- A writeup of [Interstate Network’s optimistic rollup](https://gitcoin.co/grants/334/interstate-network-evm-generic-optimistic-rollups?tab=description)

**Stuff for developers**

- Truffle [v5.1.9](https://github.com/trufflesuite/truffle/releases/tag/v5.1.9), now Istanbul compatible.
- Truffle’s [experimental console.log](https://github.com/trufflesuite/truffle-logger-example/issues/3)
- New [features in Embark v5](https://embark.status.im/news/2020/01/13/announcing-embark-5/)
- [SolUI](https://solui.dev/): generate IPFS UIs for your Solidity code. akin to [oneclickdapp.com](https://oneclickdapp.com/)
- BokkyPooBah’s [Red-Black binary search tree](https://github.com/bokkypoobah/BokkyPooBahsRedBlackTreeLibrary) library and [DateTime library](https://github.com/bokkypoobah/BokkyPooBahsDateTimeLibrary) updated to Solidity v0.6
- Overhauled [OpenZeppelin docs](https://docs.openzeppelin.com/openzeppelin/)
- [Exploring commit/reveal schemes](https://medium.com/swlh/exploring-commit-reveal-schemes-on-ethereum-c4ff5a777db8)
- Using the [MythX plugin with Remix](https://blog.mythx.io/howto/verifying-smart-contract-security-with-remix-part-1-basic-bug-detection-and-solidity-assertions/)
- [Training materials for Slither, Echidna, and Manticore](https://github.com/crytic/building-secure-contracts) from Trail of Bits
- Soon you’ll need to pay for [EthGasStation’s API](https://ethgasstation.info/blog/changes-to-egs-api/)
- As of Feb 15, you’ll need a [key for Etherscan’s API](https://medium.com/etherscan-blog/psa-for-developers-implementation-of-api-key-requirements-starting-from-february-15th-2020-b616870f3746)

**Ecosystem**

- Gavin Andresen [loves Tornado.Cash](http://gavinandresen.ninja/private-thoughts) and published some [thoughts](http://gavinandresen.ninja/a-more-private-eth-wallet) on making a [wallet on top of Tornado Cash](https://gist.github.com/gavinandresen/aeed66e7e23c905f885362e6fbe3a81d)
- [MarketingDAO is open for proposals](https://medium.com/marketingdao/ethereum-marketing-dao-is-now-open-for-proposals-ac3405086501)
- [Almonit.eth.link launches](https://medium.com/the-ethereum-name-service/the-first-search-engine-for-the-dweb-ens-ipfs-has-launched-79b9fae7a9dc), a search engine for ENS + IPFS dweb
- Build token [pop-up economies with the BurnerFactory](https://medium.com/@dmihal/token-factory-build-tokens-pop-up-economies-with-the-burner-factory-39ccea9f47ac)

**Enterprise**

- [EEA testnet launch](https://consensys.net/blog/enterprise-blockchain/what-the-eea-testnet-launch-means-for-blockchain-and-enterprise/) running Whiteblock’s [Genesis testing](https://twitter.com/whiteblock/status/1217584982023118848?s=20) platform
- [Plugin APIs in Hyperledger Besu](https://pegasys.tech/introducing-plugin-apis-in-hyperledger-besu/)
- [Privacy and blockchains primer](https://consensys.net/blog/enterprise-blockchain/how-is-blockchain-verifiable-by-the-public-and-yet-anonymous/) aimed at enterprise
- A massive [list of corporations building on Ethereum](https://twitter.com/AdamScochran/status/1217524744909660162)
- [Sacramento Kings using Treum](https://www.reddit.com/r/ethereum/comments/ep9m80/nba_team_auctioning_basketball_stars_jersey_on/) supply chain tracking to authenticate player equipment

**Governance and standards**

- [EIP2464](https://github.com/ethereum/EIPs/blob/8ea8691380b3d6c01d7e0da7d0485e113e728d8d/EIPS/eip-2464.md): eth/65 transaction annoucements and retrievals
- [ERC2462](https://github.com/ethereum/EIPs/blob/102d8b8305d507f293ae5fd4727822b6bfa99cd0/EIPS/eip-2462.md): interface standard for EVM networks
- [ERC2470](https://github.com/ethereum/EIPs/blob/69f2fb14ca46fa784891dd975357d4f4d8596b51/EIPS/eip-2470.md): Singleton Factory
- [bZxDAO](https://bzx.network/blog/introducing-bzxdao): proposed 3 branch structure to decentralize bZx

**Application layer**

- Livepeer [upgrades to Streamflow release](https://medium.com/livepeer-blog/livepeers-streamflow-protocol-update-is-complete-and-a-new-tokenholder-site-is-launched-163a94ac8ebd) - GPU miners can transcode video with negligible loss of hashpower so video transcoding gets cheaper
- Molecule is live on mainnet with a [bonding curve for a clinical trial for Psilocybin microdoses](https://twitter.com/Molecule_to/status/1217867542380847105)
- [Liquidators](https://medium.com/dragonfly-research/liquidators-the-secret-whales-helping-defi-function-acf132fbea5e): the secret whales helping DeFi function. Good walkthrough of DeFi network keepers.
- [Curve](https://compound.curve.fi/): a uniswap-like exchange for stablecoins, currently USDC<>DAI
- New [Golem release](https://blog.golemproject.net/brass-golem-beta-0-22-0/) has Concent on mainnet, new usage marketplace, and Task API on testnet
- [Gitcoin as social network](https://twitter.com/owocki/status/1218559001232695297)
- [rTrees](https://medium.com/rtrees/announcing-rtrees-5e21a856b20). Plant trees with your rDai

**Tokens/Business/Regulation**

- The [case for a trillion dollar ETH market cap](https://bankless.substack.com/p/the-trillion-dollar-case-for-eth-eb6)
- [Continuous Securities Offering handbook](https://medium.com/@thibauld/introducing-the-continuous-securities-offering-handbook-724b6e889296)
- The [SEC does not like IEOs](https://www.sec.gov/oiea/investor-alerts-and-bulletins/ia_initialexchangeofferings)
- Former CFTC Chair Giancarlo and Accenture to [push for a blockchain USD](https://newsroom.accenture.com/news/former-cftc-chair-launches-the-digital-dollar-project.htm)
- Tokenizing yourself (selling your time/service via token) was all the rage this week, [kicked off by Peter Pan](https://twitter.com/pet3rpan_/status/1216421211183271936). Here’s a [guide to tokenizing yourself](https://bankless.substack.com/p/how-to-tokenize-yourself-full)
- [Avastars](https://nft.substack.com/p/the-art-of-avastars): generative digital art from NFTs

**General**

- Chris Dixon: [Inside-out vs outside-in tech adoption](https://a16z.com/2020/01/17/inside-out-vs-outside-in-technology/)
- [baby snark](https://twitter.com/socrates1024/status/1217934151434764288): Andrew Miller’s tutorial on implementation and soundness proof of a simple SNARK
- [Blake3 hash function](https://github.com/BLAKE3-team/BLAKE3)
- Justin Drake [explains polynomial commitments](https://twitter.com/drakefjustin/status/1217814776329441283)
- New bounty (3000 USD) for [improving cryptanalysis on the Legendre PR](https://legendreprf.org/bounties)
- Mona El Isa’s a [day in the life for asset management in 2030](https://medium.com/melonprotocol/a-day-in-the-life-of-an-asset-manager-in-the-summer-of-2030-4f18009a5020). We need more web3 science fiction

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Jan 20-21 - Parity’s [OpenEthereum Rust client](https://www.eventbrite.com/e/openethereum-workshop-tickets-88507864405) workshop (Berlin)
- Jan 21 - [Gitcoin grants](https://gitcoin.co/blog/gitcoin-grants-2020/) quadratic matching ends. (my grant is [here](https://gitcoin.co/grants/237/week-in-ethereum-news)!)
- **Jan 26 - deadline for [MarketingDAO proposals](https://medium.com/marketingdao/ethereum-marketing-dao-is-now-open-for-proposals-ac3405086501)**
- Jan 31 - deadline for [EU ledger 200k euro grants](https://fundingbox.com/spaces/ledger-ledger-news-and-updates/5dbfcb7d52317832f85906c8) for blockchain startups
- Feb 8 - [Augur v1 cutoff](https://twitter.com/AugurProject/status/1214545983205494784)
- Feb 14-16 - [ETHDenver](https://www.ethdenver.com/)
- **Feb 20 - [Decentraland launch](https://decentraland.org/blog/announcements/decentraland-announces-publich-launch/)**
- Feb 28-Mar 1 - [ETHLondon UK](https://ethlondon.com/)
- Mar 3-5 - [EthCC](https://ethcc.io/) (Paris)
- Mar 29-Apr4 - [EthLagos](https://ethlagos.io/)
- Apr 3-7 - [Edcon](https://www.edcon.io/) (Vienna)
- **April 24-26 - [EthTurin](https://ethturin.com)**
- May 15 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum News. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

It’s amazing to me how many people email me when every issue has a link at the bottom saying not to email me to get in the newsletter.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **I want your links, because Google needs help: [weekinethereumnews.com](https://weekinethereumnews.com/)**

Archive on the web if you’re linking to it:  [https://weekinethereumnews.com/week-in-ethereum-news-january-19-2020/](https://weekinethereumnews.com/week-in-ethereum-news-january-19-2020/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly**

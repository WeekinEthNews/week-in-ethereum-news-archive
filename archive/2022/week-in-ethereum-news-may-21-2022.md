---
title: "Week in Ethereum News <br> May 21, 2022"
date: "2022-05-21"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- [Client bug bounties now $250k](https://blog.ethereum.org/2022/05/16/secured-no-4/), doubles to $500k for merge upgrades live on public testnets & targeted for mainnet
- Mainnet-shadow-fork-5 [went exceedingly well](https://twitter.com/dannyryan/status/1527309676441833473), equal split of execution & consensus layer clients
- [Ropsten beacon chain](https://twitter.com/terencechain/status/1526927001826648066) genesis May 30, with merge targeted around June 8
- [Help test the merge](https://twitter.com/shegenerates/status/1527290682519392258) on Kiln, make transactions and qualify for an NFT
- [Metrics exporter](https://github.com/samcm/ethereum-metrics-exporter#readme) for execution & consensus nodes, client-agnostic metrics using JSON-RPC/Beacon Node API without additional config

**Mainnet execution layer**

- [Nethermind benefits](https://twitter.com/urozmej/status/1527396760095756297): snap sync, full pruning, plugin architecture, MEV support and fast JSON RPC
- Besu [Bonsai Tries](https://consensys.net/blog/news/test-staking-ahead-of-the-merge-with-improved-bonsai-tries-state-storage/): faster for head state but slower for historical state
- Besu [v22.4.1](https://github.com/hyperledger/besu/releases/tag/22.4.1): Ropsten testnet TTD config
- Erigon [v2022.05.05-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.05.05): memory footprint reduced and merge fixes
- [Silkworm](https://erigon.substack.com/p/current-status-of-silkworm-and-silkrpc) C++ implementation of Erigon; currently faster than Erigon in all stages, Apache 2.0 license
- [Guide to Condrieu Verkle testnet](https://twitter.com/gballet/status/1526488286386069505) and how to interpret block proofs

**Proof of Stake consensus layer**

- Updated [client diversity](https://twitter.com/sproulm_/status/1526703018745376768) estimates: [Prysm less than 50%](https://twitter.com/vitalikbuterin/status/1526934223486976000), Lighthouse ~33%
- Danny Ryan’s [Finalized PoS update](https://blog.ethereum.org/2022/05/19/finalized-no-35/): 
    - ETH Staking 350k DAI quadratic funding round
    - [Data Availability Sampling RFP](https://github.com/ethereum/requests-for-proposals/blob/master/open-rfps/das.md) with $1.5 million funding
- PoS implementers [call video](https://www.youtube.com/watch?v=-6dZVes6aWc&t=250s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/HyzJna7vc) & [Christine Kim](https://docsend.com/view/zye63j53qxwrvbje):
    - Client releases expected next week for Ropsten testnet merge
    - Next shadow fork May 30
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220520)
- Nimbus [v22.5.0](https://github.com/status-im/nimbus-eth2/releases/tag/v22.5.0): proposer boost, supports latest Bellatrix (merge) spec, preview of BLS threshold signature support; [don’t use with Infura](https://twitter.com/ethnimbus/status/1527430149045731343)
- Prysm [v2.1.2](https://github.com/prysmaticlabs/prysm/releases/tag/v2.1.2): optimizations & bug fixes 

**EIPs/Standards**

- [EIP5094](https://github.com/ethereum/EIPs/pull/5094/files): URI Format for Ethereum Network Switching

**Layer2**

- Optimism [Bedrock](https://dev.optimism.io/introducing-optimism-bedrock/) source available, MIT license
- Binance [supports Optimism](https://www.binance.com/en/support/announcement/3ee5a24e46754c278eaf769fcd4b7edf?ref=AZTKZ9XS)

* * *

### **This newsletter is made possible thanks to** [**Nexus Mutual**](https://nexusmutual.io/)**!**

![Nexus Mutual Protocol Cover](https://weekinethereumnews.com/wp-content/uploads/2022/03/Nexus-Mutual-Protocol-Cover-1024x586.png)

[](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F7d8d5b05-1c58-437e-9eeb-0cb7ad9e7567_1600x915.png)

Go where the yield takes you, but don’t let the next hack set you back. Regardless of where you are chasing yield, Protocol Cover can protect your productive crypto assets across L1s, L2s, and scaling solutions. 

Maximize yield. Minimize risk. Enjoy peace of mind knowing Nexus Mutual has you covered. [Become a member](https://nexusmutual.io/) and cover your asse(t)s against the major risks in DeFi.

* * *

**Stuff for developers**

- Solidity [v0.8.14](https://blog.soliditylang.org/2022/05/18/solidity-0.8.14-release-announcement/): fixes for ABI-encoding nested arrays directly from calldata and data location during inheritance
- Foundry: [Solidity model checker](https://twitter.com/leonardoalt/status/1525509198636777473) and improved [Etherscan verification](https://twitter.com/gakonst/status/1526691363407790080)
- [more-evm-puzzles](https://github.com/daltyboy11/more-evm-puzzles#readme): focused on CREATE and CALL opcodes
- EVM Deep Dives: [DELEGATECALL](https://noxx.substack.com/p/evm-deep-dives-the-path-to-shadowy-a5f)
- [Tx Uncled](https://txuncle.metachris.com): check if transaction was uncled
- [Flashbots-cli](https://github.com/zeroXbrock/flashbots-cli#readme): interact with Flashbots relay
- [CloudFlare](https://blog.cloudflare.com/ea-web3-gateways/) Ethereum and IPFS gateways public access
- OpenSea [Seaport](https://github.com/ProjectOpenSea/seaport#readme): decentralized NFT swap protocol, gas optimized, MIT license, fuzz testing using Foundry
- [Etherscan Sepolia](https://twitter.com/etherscan/status/1526523646273265664) testnet explorer
- [Faucet Link](https://faucetlink.to/): list of testnet faucets, status and Sybil protection used
- Rinkeby testnet [to be deprecated](https://github.com/ethereum/go-ethereum/pull/24884) as [centralized to Geth team & complex to merge](https://twitter.com/peter_szilagyi/status/1526065078604292097)

**Security**

- Wormhole [uninitialized proxy disclosed](https://medium.com/immunefi/wormhole-uninitialized-proxy-bugfix-review-90250c41a43a), $10 million bounty paid
- Nascent’s [Simple security toolkit](https://github.com/nascentxyz/simple-security-toolkit#readme): development process, audit readiness checklist, pre-launch security checklist and incident response plan template
- Hats [Capture the Flag post mortem](https://hatsfinance.medium.com/capture-the-flag-postmortem-bbc1b5afdf2c): exploit ERC721 safeTransfer call back

**Ecosystem**

- Cloudflare to [stake their own ETH](https://blog.cloudflare.com/next-gen-web3-network/) to support the Merge, won’t run PoW
- [Protocol Guild pilot](https://twitter.com/StatefulWorks/status/1527675087847051265) (reward core Ethereum contributors) with $2.7 million from Lido
- [MEV sandwich](https://twitter.com/bertcmiller/status/1527757146716348416) of $13.5 million stablecoin swap
- Reminder: [the merge won’t (significantly) lower gas fees](https://willthemergelowergasprices.org/) 

**Enterprise**

- [Polygon Nightfall](https://blog.polygon.technology/introducing-polygon-nightfall-mainnet-decentralized-private-transactions-for-enterprise/) (optimistic rollup with zero knowledge for privacy) unaudited beta live, aimed at enterprise
- [Norwegian central bank](https://www-norges--bank-no.translate.goog/bankplassen/arkiv/2022/eksperimentell-testing-av-digitale-sentralbankpenger/?_x_tr_sl=no&_x_tr_tl=en) to prototype CBDC

**Application layer**

- [DAOhaus](https://twitter.com/nowdaoit/status/1526593440103817216) (no-code Moloch DAO launcher) live on Optimism
- [LinkTree](https://linktr.ee/blog/three-new-nft-features-to-build-your-web3-brand-and-community/): NFT gallery, use NFT for pfp & background and token gated links
- [Unlock Protocol](https://unlock-protocol.com/blog/recurring-subscription-nft) adds recurring memberships
- [Rico](https://bank.dev/): Nikolai’s evolution of Dai/Rai, multi-collateral & uses a controller

* * *

### **Job Listings**

- [Hiring Coordinator](https://jobs.lever.co/ethereumfoundation/7f5bf10b-ea68-4364-a378-e34ae345a212?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) wanted by Ethereum Foundation
- Sourcify (source code verification) need a [TypeScript Developer](https://jobs.lever.co/ethereumfoundation/db85cf1d-6ffd-42a6-8f0d-f5a91c6ddf4a?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Ethereum Foundation need a [People Operations Lead](https://jobs.lever.co/ethereumfoundation/8046bbe5-6343-4ecf-8296-37dc2a5bf915?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Trail of Bits [Security Apprenticeship](https://jobs.lever.co/trailofbits/b2d6ce87-6b01-462f-965a-597a273ce26f) (3 months)

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Strengthen a Uniswap v3 TWAP oracle](https://twitter.com/haydenzadams/status/1526704413867397120) by depositing full range liquidity
- Cole South: [why I sold all my Bitcoin for ETH](https://colesouth.com/no-bitcoin/)
- [Soulbound Tokens & The Dread Pirate Roberts](https://twitter.com/micahzoltu/status/1527564710266036224): bind Soulbound tokens to a soul NFT, allowing souls to be transferred

**General**

- [Skiff Mail](https://skiff.com/mail): end-to-end encrypted email
- Domain hijacks impact [SpiritSwap](https://spiritswap.medium.com/post-mortem-on-this-weekends-dns-event-cb61c11f5c2f) (Fantom) and [QuickSwap](https://twitter.com/quickswapdex/status/1525306033400188928) (Polygon)
- Scale of [Real-Time Bidding data broadcasts](https://www.iccl.ie/wp-content/uploads/2022/05/Mass-data-breach-of-Europe-and-US-data-1.pdf) \[PDF\]: US users online activity & location exposed 747 times per day
- Differences between [threshold BLS aggregation and BLS aggregation](https://db2510.github.io/blogs/aggregation/)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-may-21-2022](https://weekinethereumnews.com/week-in-ethereum-news-may-21-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in_ **_bold_**_)_**:**

- May 24 – [ETH Staking QF Round](https://blog.clr.fund/350k-eth-staking-qf-round/) ends
- **Jun 3 –** [**Merge community call #4**](https://github.com/ethereum/pm/issues/532)
- Jun 8 – [Ropsten testnet upgrades to PoS](https://twitter.com/trent_vanepps/status/1525138148879220742)
- **Jun 8-23 –** [**Gitcoin Grants Round 14**](https://gitcoin.co/grants/)
- Jun 10 – [Austin DeFi](https://2022.austindefi.org/) summit
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETH NYC](https://nyc.ethglobal.co/)
- **Jul 1 –** [**Data Availability Sampling**](https://github.com/ethereum/requests-for-proposals/blob/master/open-rfps/das.md) **proposals due**
- Jul 6-8 – [ETHBarcelona](https://twitter.com/eth_barcelona/status/1516773782538448896)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- **Aug 5-13 –** [**ETH Seoul**](https://2022.ethseoul.org/)
- Aug 8-10 – [ETHToronto](https://www.ethtoronto.ca/)
- Aug 11-14 – [ETH LATAM (Buenos Aires)](https://twitter.com/ethlatam/status/1524146640474587137)
- Aug 18-19 – [Ethereum SP](https://twitter.com/EthereumRio/status/1520490449009528832) (São Paulo)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 28 – [DeFi San Francisco](https://2022.defi-sf.com/) summit
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev) (hackathon & conference)
- **Sep 2-4 –** [**ETHSantiago**](https://twitter.com/EthereumStgo)
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** [_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive it weekly_**

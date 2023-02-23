---
title: "Week in Ethereum News <br> June 4, 2022"
date: "2022-06-04"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- [Ropsten testnet is ready to turn off PoW forever](https://blog.ethereum.org/2022/05/30/ropsten-merge-announcement/) with [TTD set](https://blog.ethereum.org/2022/06/03/ropsten-merge-ttd/)
    - Tool to [predict TTD](https://ethresear.ch/t/predicting-ttd-on-ethereum/12742) arrival
    - Stakers/nodes must manually override TTD in [latest client release](https://blog.ethereum.org/2022/06/03/ropsten-merge-ttd/)
    - Manual override is useful practice in case of miner hijinx on mainnet
    - Guides on [running Ropsten nodes](https://notes.ethereum.org/@launchpad/ropsten) or specifically a [Geth/LH Ropsten node](https://github.com/remyroy/ethstaker/blob/main/merge-ropsten.md)
    - Ropsten [beacon chain is live](https://twitter.com/parithosh_j/status/1531298447797760000)
    - Reminder: Ropsten to be deprecated post-Merge
    - [Merge Community Call](https://www.youtube.com/watch?v=qG-A5i6x6N8&t=3s) discussion
- Latest [PoS implementer call](https://www.youtube.com/watch?v=4oI48BEijVw). Notes by [Ben Edgington](https://hackmd.io/@benjaminion/BkmzqV8uq)
    - Lighthouse/Prysm changing deposit tracking to be more robust against unlikely edge case of minute block times
- Mainnet shadow fork 6 again merged [successfully with some minor issues](https://notes.ethereum.org/PhbNw_cGSQ-VKqzGl4bPcg?view)

**Mainnet execution layer**

- Polynya: [understanding the historical storage bottleneck](https://polynya.mirror.xyz/EpFL1V1amxa8maE-TyjfiifJMij_KZNMvReTDxpVoA4)

**Proof of Stake consensus layer**

- [Liquid staking derivatives](https://notes.ethereum.org/@djrtwo/risks-of-lsd) over 25% of stake considered harmful
    - Putting ETH into any liquid staking when it is over 25% of total stake is putting your ETH at risk
    - Lido currently at [about 30%](https://dune.com/eliasimos/Eth2-Liquid-Staking)
    - Justin Drake: design for [solo staker liquid staking derivative](https://ethresear.ch/t/liquid-solo-validating/12779), but uses SGX
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220603)
- Understanding [Eth PoS as the next generation of consensus protocols](https://twitter.com/sreeramkannan/status/1530474715990478848)
- An explanation of proposer boost and the recent [7 block beacon chain reorg](https://barnabe.substack.com/p/pos-ethereum-reorg)

**EIPs/Standards**

- [ERC5114](https://github.com/ethereum/EIPs/pull/5114/files): Soulbound token
- [ERC5115](https://github.com/ethereum/EIPs/pull/5115/files): Super composable yield token
- [ERC5131](https://github.com/ethereum/EIPs/pull/5131/files): ENS subdomain authentication
- [ERC5133](https://github.com/ethereum/EIPs/pull/5133/files): Difficulty bomb delay _(Editor’s note: I’m_ **_strongly against_** _this_ at the moment_)_

**Layer2**

- Optimism [token launched](https://optimism.mirror.xyz/qvd0WfuLKnePm1Gxb9dpGchPf5uDz5NSMEFdgirDS4c) with its first airdrop
    - Hiccups: [JSON-RPC chain reads crashed](https://twitter.com/optimismPBC/status/1531798286037680129) but sequencer flawless
    - Simple Docker setup to [run your own Optimism node](https://github.com/smartcontracts/simple-optimism-node)
- ImmutableX is [turning 2% fees on](https://immutablex.medium.com/fees-on-immutable-x-79d3e7207b12) to be sustainable

* * *

### **This newsletter is made possible thanks to** [**Starbloom Ventures**](https://twitter.com/StarbloomVent)**!**

![Starbloom Ventures](https://substackcdn.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Ff8f36912-89bc-4712-a3f5-cfff1571bf45_613x313.png "Starbloom Ventures")

[](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Ff8f36912-89bc-4712-a3f5-cfff1571bf45_613x313.png)

Starbloom Ventures is a **first round** venture fund founded by [Evan Van Ness](https://twitter.com/evan_van_ness) to invest in the future of web3. 

We pledge 10% of investing profits to support Ethereum public goods.

* * *

**Stuff for developers**

- Foundry [Solidity Scripting and Deploy](https://twitter.com/gakonst/status/1531056739470016512)
- [thirdweb deploy](https://twitter.com/joenrv/status/1531318160439201793) - no private key deploy flow and auto-Sourcify verifiction as well as automatic SDKs for React/Node/Python/Go
- [Delegatable](https://mirror.xyz/0x55e2780588aa5000F464f700D2676fD0a22Ee160/pTIrlopsSUvWAbnq1qJDNKU1pGNLP8VEn1H8DSVcvXM): Solidity library to sign off-chain messages that grant non-transferrable powers to other people
- [MEV Explorer](https://metablock.dev/tools/mev/): mev-inspect-js frontend; supports Eth, Polygon, and Arbitrum.
- Implementing [zk-lotteries with Circom](https://killari.medium.com/implementing-zero-knowledge-lotterys-circom-circuits-part-1-2-16910b3732a2) on top of Tornado Cash’s Nova

**Security**

- Metamask pays [$120k bug bounty for iframe clickjacking vuln](https://medium.com/metamask/metamask-awards-bug-bounty-for-clickjacking-vulnerability-9f53618e3c3a)
- Rocketpool [employee’s computer exploited](https://dao.rocketpool.net/t/post-mortem-security-incident-26-05/701) for 15 ETH

**Ecosystem**

- Skiff offers [end-to-end encrypted email using your Eth wallet](https://twitter.com/skiffprivacy/status/1532090120798543872) and ENS
- A tweetstorm version of last week’s [Eth roadmap](https://twitter.com/0xb17z/status/1532039402234314752) explainer
- [Massdrop](https://massdrop.multisender.app/): a frontend to do a Merkle airdrop

**Application layer**

- DeFiSaver [live on Arbitrum and Optimism](https://blog.defisaver.com/defi-saver-is-now-live-on-arbitrum-and-optimism/)
- [Conviction voting using GTC](https://twitter.com/austingriffith/status/1532717789118705664) to sort frontend display of Gitcoin grants
- [Proof of Integrity](https://twitter.com/proof_integrity/status/1532453663721111554) - a pilot program in Buenos Aires slums to ensure UBI doesn’t just go to those who don’t need it
- 1inch [integrates Synthetix atomic exchanges](https://twitter.com/synthetix_io/status/1531683261944156160) for less slippage on big trades
- [MobyMask](https://mirror.xyz/0x55e2780588aa5000F464f700D2676fD0a22Ee160/8whNch3m5KMzeo6g5eblcXMMplPf8UpW228cSh3nmzg): using web of trust to manage phishing reports
- Rune’s [Endgame plan](https://forum.makerdao.com/t/the-endgame-plan-parts-1-2/15456) for MakerDAO: a synthetic ETH product and a first metaDAO with yield farming

* * *

## **Job Listings**

- Ethereum Foundation: [generalist developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) to drive strategic ecosystem inits
- Sourcify: [TypeScript/nodejs developer](https://jobs.lever.co/ethereumfoundation/db85cf1d-6ffd-42a6-8f0d-f5a91c6ddf4a?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) wanted
- [People Operations Lead](https://jobs.lever.co/ethereumfoundation/8046bbe5-6343-4ecf-8296-37dc2a5bf915?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) at EF
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)
- [Hiring Coordinator](https://jobs.lever.co/ethereumfoundation/7f5bf10b-ea68-4364-a378-e34ae345a212?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) wanted by EF

**Job listings: $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet/Arbitrum/Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Nate Chastain [charged with money laundering and wire fraud](https://www.justice.gov/usao-sdny/pr/former-employee-nft-marketplace-charged-first-ever-digital-asset-insider-trading-scheme) in SDNY for OpenSea insider trading
- [Pooly](https://twitter.com/lay2000lbs/status/1529827211401842694): buy NFT to support PoolTogether legal defense against the Liz Warren staffer’s class action suit
- Absurd lawsuit to hold all [bZx founders **and** tokenholders liable for security bugs](https://www.thefashionlaw.com/new-lawsuit-asks-who-is-the-blame-when-a-dao-goes-wrong/)
- ~25 academics/BigTech employees wrote a [technically sloppy letter to Congress against crypto](https://twitter.com/matthew_d_green/status/1531963408727396354)

**General**

- [MS Word in Windows “Follina” unpatched zero-day vuln](https://msrc-blog.microsoft.com/2022/05/30/guidance-for-cve-2022-30190-microsoft-support-diagnostic-tool-vulnerability/). Reminder: almost all loss of crypto comes from Windows users. \[_Disclosure: small MSFT shareholder for almost 30 years_\]
- WSJ reports that [Fidelity is hiring to support Eth custody and trading services](https://www.wsj.com/articles/fidelitys-crypto-focused-business-plans-tech-hiring-spree-11653991200)
- Coinbase [rescinding offers that employees had already accepted](https://blog.coinbase.com/update-on-hiring-plans-bcedfa634989) after [promising 2 weeks ago that they wouldn’t](https://twitter.com/TeamBlind/status/1532769735393169410)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-june-4-2022/](https://weekinethereumnews.com/week-in-ethereum-news-june-4-2022/)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Jun 8-23 – [Gitcoin Grants Round 14](https://gitcoin.co/grants/)
- Jun 10 – [Austin DeFi](https://2022.austindefi.org/) summit
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETH NYC](https://nyc.ethglobal.co/) **(ETH Global)**
- Jul 1 – [Data Availability Sampling](https://github.com/ethereum/requests-for-proposals/blob/master/open-rfps/das.md) proposals due
- Jul 6-8 – [ETHBarcelona](https://ethbarcelona.com/)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 5-13 – [ETH Seoul](https://2022.ethseoul.org/)
- Aug 8-10 – [ETHToronto](https://www.ethtoronto.ca/)
- Aug 11-14 – [ETH LATAM (Buenos Aires)](https://twitter.com/ethlatam/status/1524146640474587137)
- Aug 19-21 – [ETHMexicoCity](https://mexico.ethglobal.com/) **(ETH Global)**
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 28 – [DeFi San Francisco](https://2022.defi-sf.com/) summit
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev/) (hackathon & conference)
- Sep 2-4 – [ETHSantiago](https://twitter.com/EthereumStgo)
- Sep 2-28 – [ETHOnline](https://online.ethglobal.com/')
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Sep 27-29 – [Ethereum SP](https://twitter.com/Ethereum_Brasil/status/1530320916667895808) (São Paulo)
- **Oct 7-9 –** [**ETHBogotá**](https://bogota.ethglobal.com/) **(ETH Global)**
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) **(ETH Global)**
- Nov 18-20 – ETHGlobal [Web3 Weekend](https://web3weekend.ethglobal.com/)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) **(ETH Global)**

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

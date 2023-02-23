---
title: "Week in Ethereum News <br> July 9, 2022"
date: "2022-07-09"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- Sepolia testnet [merged successfully](https://twitter.com/parithosh_j/status/1544968914777645056):
    - [TTD config issue](https://twitter.com/EthDreamer/status/1544747167167946753) specific to PoW testnets
- Mainnet-shadow-fork-8 [merged successfully](https://twitter.com/evan_van_ness/status/1544380378680549376)
- [Mainnet-shadow-fork-9](https://twitter.com/abcoathup/status/1545239647847993344) merges July 14, plan to test MEV-boost

**Mainnet execution layer**

- Tim Beiko’s [core devs update](https://tim.mirror.xyz/xkhOUpYC8UUNlTgGehhl63XF5QZnxAOvW3EOK9MWPeQ): stakers prepare for merge, block times back to ~13s after Gray Glacier upgrade, testnets being deprecated & community calls
- Latest core devs [call video](https://youtu.be/K_Cjn74lMSY?t=687). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1545472282973245440) and [Christine Kim](https://twitter.com/christine_dkim/status/1545497249857146881):
    - Goerli merge TTD to be set at next PoS implementers or core devs call
    - Discussion of Latest Valid Hash edge cases
    - MEV-boost discussion
- Erigon [v2022.07.02-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.07.02): passes all 114 [engine Hive tests](https://hivetests2.ethdevops.io/)
- Besu [v22.4.4](https://github.com/hyperledger/besu/releases/tag/22.4.4): fixes for snap-sync & state root mismatch/worldstate unavailable
- Geth [fix for regression impacting merge sync](https://twitter.com/vdwijden/status/1543990855471710210) on Sepolia and Ropsten testnets
- KZG ceremony [call video](https://www.youtube.com/watch?v=wvFVpDm3iVs): audit of SDK output mid-August, audit of full system end-October, spec to be made executable

**Proof of Stake consensus layer**

- Prysm [v2.1.3](https://github.com/prysmaticlabs/prysm/releases/tag/v2.1.3): merge fixes
- Nimbus: [light proxy](https://twitter.com/jcksie/status/1543843699188170752) becomes possible using beacon chain light client protocol post-merge
- foobar: [Proof of Stake explainer](https://0xfoobar.substack.com/p/ethereum-proof-of-stake) with common misconceptions

**Layer2**

- [Aztec Connect](https://medium.com/aztec-protocol/aztec-network-launches-first-ever-private-defi-solution-for-ethereum-e5ec7624d430) (privacy zk rollup) live on mainnet; zk.money DeFi aggregator supports Element and Lido
- Proposal for [Layer2 bridge risk framework](https://gov.l2beat.com/t/l2bridge-risk-framework/31)
- Hop [transfer delays post mortem](https://authereum.notion.site/Arbitrum-Bridge-Week-Delays-Post-Mortem-ac1f6681f8c241a8ad524ba2047d083e) during Arbitrum Odyssey bridging

**EIPs/Standards**

- [EIP5202](https://github.com/ethereum/EIPs/pull/5202/files): Factory contract format

* * *

### **This newsletter is made possible thanks to** [**Hardhat**](https://hardhat.org/)!

![](https://weekinethereumnews.com/wp-content/uploads/2021/06/hardhat-rectangle-1024x325.png)

[](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F031a7efa-a9c2-4656-9eec-eaaf79e28665_1400x441.png)

Hardhat has just released a refreshed experience for new projects: [Hardhat Toolbox](https://medium.com/nomic-foundation-blog/hardhat-2-10-0-a-refreshed-experience-56281ef73964). With minimal boilerplate and set up effort, it's the **best way to get started with building for Ethereum**.

Hardhat Toolbox packs most of the functionality you'll need into a single package. No additional plugins required to get started. It also includes a new replacement for hardhat-waffle that is tightly integrated with Hardhat which offers extra features and better error messages.

[Check out the announcement](https://medium.com/nomic-foundation-blog/hardhat-2-10-0-a-refreshed-experience-56281ef73964) for more information, and install Hardhat 2.10.0 to try it out!

* * *

**Stuff for developers**

- Hardhat [v2.10.0](https://medium.com/nomic-foundation-blog/hardhat-2-10-0-a-refreshed-experience-56281ef73964) + Hardhat Toolbox opinionated bundle of plugins: deploy & interact with ethers.js, test with Mocha & Chai, interact with Hardhat Network, verify on Etherscan, gas reporting, test coverage and type bindings for TypeScript
- [Hardhat for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=NomicFoundation.hardhat-solidity) out of beta
- [surl](https://github.com/memester-xyz/surl/#readme) (http library): make web requests from Solidity scripts & tests
- [stack-packer](https://github.com/d1ll0n/stack-packer#readme): generate Solidity library for packed structs on the stack
- Fe [v0.19.1-alpha](https://github.com/ethereum/fe/releases/tag/v0.19.1-alpha): return nested structs, adopts curly braces, traits as bounds for generic functions and complex types as array elements
- [micro-web3](https://github.com/paulmillr/micro-web3#readme): minimal web3.js implementation 
- [MetaMask](https://medium.com/metamask/metamask-api-method-deprecation-2b0564a84686) API deprecating eth\_decrypt & eth\_getEncryptionPublicKey
- [Semaphore v2](https://medium.com/privacy-scaling-explorations/semaphore-v2-is-live-f263e9372579): create private identities, add identities to groups & send anonymous signals

**Security**

- Synthetix [logic error disclosed](https://medium.com/immunefi/synthetix-logic-error-bugfix-review-40da0ead5f4f), $150k bounty
- Yield [roll over vulnerability disclosed](https://twitter.com/yield/status/1545119888309567489), $10k bounty
- Axie/Ronin bridge $600million exploit [entry point was fake job offer PDF](https://www.theblock.co/post/156038/how-a-fake-job-offer-took-down-the-worlds-most-popular-crypto-game)
- samczsun breaks down an [attempted attack using a crypto stealer](https://twitter.com/samczsun/status/1544186151585533952)

**Ecosystem**

- EF Research Team [AMA](https://www.reddit.com/r/ethereum/comments/vrx9xe/ama_we_are_ef_research_pt_8_07_july_2022/)
- [ethOS](https://twitter.com/EthereumPhone/status/1544363266469683204) (mobile OS) supports unlocked Pixel 3 & 5a; light node, OTA updates 

**Application layer**

- [Maker DAO](https://twitter.com/MakerDAO/status/1545080938320875522) approves $100 million vault for US bank
- [Aave proposes GHO](https://governance.aave.com/t/introducing-gho/8730) collateral-backed USD stablecoin
- Tornado Cash [Classic UI open sourced](https://tornado-cash.medium.com/tornado-cash-classic-ui-is-now-open-source-4b542b705a97)
- [PoolTogether](https://twitter.com/pooltogether_/status/1545416501414338560) live on Optimism
- [sudoAMM](https://twitter.com/sudoswap/status/1545535663365165063) decentralized NFT marketplace protocol

* * *

### **Job Listings**

- [Waku](https://waku.org/) is hiring [Software & DevRel Engineer](https://grnh.se/55c532491us) and [Product Marketing Manager](https://grnh.se/146431af1us) 
- Ethereum Foundation seek a [Front End Developer](https://jobs.lever.co/ethereumfoundation/40ed733c-d3af-4026-b1b2-57ef7e70f788?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- GridPlus hiring a [Go/protocol dev for the private, scalable PhononDAO](https://gridplus.io/pages/careers#PhononEngineer)
- [Nexus Mutual: Frontend/Solidity](https://nexusmutual.recruitee.com/): Help build the web3 Risk Marketplace
- Taiko ZKRollup: [hiring senior golang & rust backend developers](https://taiko.xyz/career).
- Status hiring:[Comms & Activism Director](https://grnh.se/0a1f0ea71us), [React Native UI](https://grnh.se/2fada6031us) & [C++, Qt/QML](https://grnh.se/bf6d5d011us) Devs

**Job listings: $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet/Arbitrum/Optimism. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US government employees](https://twitter.com/OfficeGovEthics/status/1544818474014449665) holding crypto restricted from participating in crypto regulation
- Jake Chervinsky: [predictions for US SEC in Q3/Q4](https://twitter.com/jchervinsky/status/1542965858233995265), exchange rule to be finalized in October and new enforcement actions before end of September
- [Three Arrows Capital](https://www.coindesk.com/business/2022/07/01/three-arrows-capital-files-for-bankruptcy-in-new-york-tied-to-british-virgin-islands-proceeding/) (3AC) filed for Chapter 15 bankruptcy in New York
- [Former Celsius asset manager](https://twitter.com/0x_b1/status/1545153652624691200) alleges that Celsius is a ponzi
- [Class action lawsuit against Solana](https://twitter.com/DeFiDefenseLaw/status/1545024045737017344) alleges unregistered security sold to retail

**General**

- [Chrome zero-day](https://www.bleepingcomputer.com/news/security/google-patches-new-chrome-zero-day-flaw-exploited-in-attacks/): heap overflow vulnerability in WebRTC component
- [Chinese data leak](https://twitter.com/cz_binance/status/1543905416748359680) of 1 billion residents, apparently due to credentials published in a blog
- Balaji Srinivasan’s book [The Network State](https://thenetworkstate.com/) released
- [NIST selects quantum-resistant algorithms](https://www.nist.gov/news-events/news/2022/07/nist-announces-first-four-quantum-resistant-cryptographic-algorithms): CRYSTALS-Kyber for general encryption and CRYSTALS-Dilithium, FALCON & SPHINCS+ for digital signatures

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-9-2022](https://weekinethereumnews.com/week-in-ethereum-news-july-9-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Jul 14 – [Devcon ticket auction & raffle](https://raffle.devcon.org/) ends
- Jul 15 – [Merge community call #5](https://github.com/ethereum/pm/issues/564)
- Jul 17 – [EF Fellowship program](https://fellowship.ethereum.foundation/) applications close
- Jul 18 – [Devcon wave 01 tickets](https://devcon.org/en/tickets/)
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Jul 22-24 – [EthCC Hackathon](https://ethcchack.com/) (Paris)
- Aug 5-13 – [ETH Seoul](https://2022.ethseoul.org/)
- Aug 8-10 – [ETHToronto](https://www.ethtoronto.ca/)
- Aug 11-13 – [ETH LATAM](http://ethlatam.org/) (Buenos Aires)
- Aug 19-21 – [ETHMexicoCity](https://mexico.ethglobal.com/) (ETH Global)
- Aug 20 – [Paradigm CTF](https://twitter.com/paradigm_ctf/status/1542277548670758912) starts
- **Aug 26-27 –** [**HackSummit**](https://sf.hacksummit.org/) **(San Francisco)**
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev/) (hackathon & conference)
- Sep 2-28 – [ETHOnline](https://online.ethglobal.com/') (ETH Global)
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 8-10 – [ETHSantiago](https://twitter.com/EthereumStgo)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Sep 16-18 - [EthBerlin](https://ethberlin.ooo/)
- Sep 27-29 – [Ethereum SP](https://twitter.com/Ethereum_Brasil/status/1530320916667895808) (São Paulo)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- Oct 10 – [DeFi Bogotá](https://2022.defibogota.org/)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

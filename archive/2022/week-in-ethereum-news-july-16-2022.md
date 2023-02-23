---
title: "Week in Ethereum News <br> July 16, 2022"
date: "2022-07-16"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- [Tentative Merge timeline](https://twitter.com/evan_van_ness/status/1547638881478004736) to turn off PoW in mid to late September: 
    - Goerli testnet August 11
    - Pick mainnet TTD in mid-August assuming Goerli successfully merges
    - Mainnet merge lightly penciled in for week of September 19
- PoS implementers [call video](https://www.youtube.com/watch?v=yBEPzzeo1a4&t=123s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/BkxQTpqpi9) and [Christine Kim](https://twitter.com/i/notes/1546872394467495938):
    - Mainnet-shadow-fork-9 merged, TTD hit earlier than estimated, config issue & some known client issues.  Finalized when config issue fixed
    - Goerli shadow fork planned for next week
    - MEV-boost implementation audited, discussed when relays should start
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220715)
- If you’re paranoid about [your validator getting DoS’d](https://ethereum-magicians.org/t/how-i-learned-to-stop-worrying-about-the-dos-and-love-the-chain/9941) run a sentry node until Ethereum ships single secret leader election (SSLE) to fix the problem
- [Constantine](https://our.status.im/fastest-bls-signature-implementation/) BLS implementation, 14% faster for signing & 18% faster for verification than BLST
- Proposal to support [middleware-based distributed validator clients](https://ethresear.ch/t/distributed-validator-middlewares-and-the-aggregation-duty/13044)

**Layer2**

- Arbitrum’s [Nova](https://offchain.medium.com/introducing-nova-arbitrum-anytrust-mainnet-is-open-for-developers-9a54692f345e) (using AnyTrust) is open for developers; data availability committee (adds assumption that two members are honest)
- StarkNet [Token](https://medium.com/starkware/part-1-starknet-sovereignty-a-decentralization-proposal-bca3e98a01ef) announced for governance, fees & staking; 49.9% initial distribution to investors and core contributors
- [L2Beat](https://twitter.com/l2beat/status/1547498863921188864) adds info on permissioned addresses to help users understand the temporary centralization trade offs each rollup is making

**EIPs/Standards**

- [EIP5216](https://github.com/ethereum/EIPs/pull/5216/files): ERC1155 approval by amount extension
- [EIP5218](https://github.com/ethereum/EIPs/pull/5222/files): NFT rights management
- [EIP5219](https://github.com/ethereum/EIPs/pull/5219/files): Decentralized HTTP
- [EIP5247](https://github.com/ethereum/EIPs/pull/5247/files): Smart proposal
- [EIP5252](https://github.com/ethereum/EIPs/pull/5252/files): Account-bound finance
- [EIP5267](https://eips.ethereum.org/EIPS/eip-5267): Retrieval of EIP712 domain 

* * *

### **This newsletter is made possible thanks to** [**Nexus Mutual**](https://nexusmutual.io/)**!**

![Nexus Mutual Protocol Cover](https://weekinethereumnews.com/wp-content/uploads/2022/03/Nexus-Mutual-Protocol-Cover-1024x586.png)

[](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fa85c7ccd-aca7-4297-9ad4-9ecfba5177d5_1024x586.png)

The yield is still out there.  When you discover the next opportunity make sure you don’t get rekt. 

Protect yourself against: 

- hacks with Protocol Cover, 
- depegging with Yield Token Cover
- CeFi blow-ups with Custody Cover. 

Maximize yield. Minimize Risk. Enjoy peace of mind knowing Nexus Mutual has you covered. Become a member and [protect your assets](https://app.nexusmutual.io/cover) against the major risks in crypto.

* * *

**Stuff for developers**

- [Flexible Voting](https://www.scopelift.co/blog/introducing-flexible-voting) extension to OpenZeppelin Governor, allows lending contracts to delegate votes so you can earn yield & participate in governance at the same time
- [ERC721i](https://medium.com/charged-particles/infinite-erc721i-pre-minting-1-million-nfts-for-3-9a791a1f9a33): pre-mint NFT collection, uses ERC2309 ConsecutiveTransfer event
- [PRBTest](https://github.com/paulrberg/prb-test#readme): test assertions & log utils for Solidity, drop-in replacement for DSTest
- [Guide to creating Yul contracts](https://blog.angle.money/playing-with-yul-cd4785e456d8): convert simple Solidity contract to Yul
- [xchain](https://github.com/zobront/xchain#readme): cross chain calls from Solidity tests & scripts
- [Automate web3 UI testing](https://twitter.com/mikery/status/1546512981470679043) using wagmi and Storybook
- [create-web3](https://github.com/e-roy/create-web3#readme) (CLI for dapp projects): adds choice of CSS frameworks
- [WalletConnect iOS App Link](https://docs.walletconnect.com/mobile-linking#ios-app-link-constraints): avoid issues when triggering wallet interactions
- Web3.py [off-chain lookups](https://snakecharmers.ethereum.org/web3-py-patterns-off-chain-lookups/)
- [Mempool deep dive](https://noxx.substack.com/p/flashbots-kings-of-the-mempool) via Flashbots auction
- [Just-in-Time calldata decoding](https://mirror.xyz/alexmiller.eth/kiwpU01XZh-rCgDDRA-jB2-pjosjogGIqCZkxryZ9Oo): GridPlus’ approach

**Security**

- BiFi [1852 ETH exploit](https://bifrost.medium.com/post-mortem-bifi-btc-illegal-address-registration-c21ce3ba9fc8), key of address issuing server exposed
- OMNI [1300 ETH exploit](https://twitter.com/BlockSecTeam/status/1546141457933025280), reentrancy of onERC721Received
- [Uniswap v3 LPs targeted](https://twitter.com/uniswap/status/1546886731521212416) in airdropped token phishing scam
- Matthew Di Ferrante’s [process to build secure contracts](https://mirror.xyz/mattdf.eth/InOuMtm9aQ1M2EIYpdqtIBE0AXRxCkp90pxtGFylHfc)

**Ecosystem**

- Merge community [call #5 video](https://www.youtube.com/watch?v=Wr0B6lSoQi8&t=8s)
- [BLS signature aggregation](https://mirror.xyz/0x6afeB3d9E380787e7D0a17Fc3CA764Bb885014FA/D3g-4UPRLkAnug-p6AZYfjgXWo-psaTulyu3SaL35vg): understanding the cryptography that makes Ethereum staking unique from every other purported “PoS” system

**Enterprise**

- EEA [business readiness report](https://entethalliance.org/wp-content/uploads/2022/06/EEA_Ethereum_Business_Readiness_Report_2022_v1.1_June_29_2022.pdf) \[PDF\]

**Application layer**

- Gamestop [NFT marketplace](https://twitter.com/GameStopNFT/status/1546885983169261568) public beta
- [Web3 Citizen](https://twitter.com/KamesGeraghty/status/1546479270473609216): soulbound token with decentralized identifiers, alpha
- [ENS Fairy](https://ensfairy.xyz/): gift an ENS name
- Limo [v2](https://twitter.com/eth_limo/status/1547679619070889987) (ENS content delivery): Layer2 & off-chain lookups
- 0x API [slippage protection](https://blog.0x.org/slippage-protection-for-0x-api/): MEV-aware order routing for trades
- [Overtime](https://medium.com/@OvertimeMarkets.xyz/sports-fans-hold-onto-your-seats-the-excitement-of-sports-trading-is-coming-to-the-blockchain-e8ea9b174bd6) (sports prediction market) live on Optimism

* * *

### **Job Listings**

- Overlay (backed by Polychain,1kx,ParaFi) hiring a [Senior Solidity Developer](https://www.notion.so/Overlay-Senior-Solidity-Dev-38c9130a01a844b39ef1bb81f82aae16)
- [Nexus Mutual: Frontend/Solidity](https://nexusmutual.recruitee.com/): Help build the web3 Risk Marketplace
- GridPlus hiring a [Go/protocol dev for the private, scalable PhononDAO](https://gridplus.io/pages/careers#PhononEngineer)
- Ethereum Foundation seek a [Front End Developer](https://jobs.lever.co/ethereumfoundation/40ed733c-d3af-4026-b1b2-57ef7e70f788?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- [Waku](https://waku.org/) is hiring [Software & DevRel Engineer](https://grnh.se/55c532491us) and [Product Marketing Manager](https://grnh.se/146431af1us)

**Job listings: $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet/Arbitrum/Optimism. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Celsius](https://blog.celsius.network/important-community-update-dafde3c6b456) filed for Chapter 11 bankruptcy
- [OpenSea](https://twitter.com/dfinzer/status/1547648521607659522) let go ~20% of team
- Breakdown of [USDC reserve assets](https://6778953.fs1.hubspotusercontent-na1.net/hubfs/6778953/USDC%20Reserves%20Reports/USDC%20Reserve%20Breakdown_June.pdf) \[PDF\]

**General**

- [OP\_Return wars of 2014](https://blog.bitmex.com/dapps-or-only-bitcoin-transactions-the-2014-debate/): why dapps are built on Ethereum rather than Bitcoin
- Vitalik’s [thoughts on network states](https://vitalik.ca/general/2022/07/13/networkstates.html)
- Remco: [math behind Groth16](https://xn--2-umb.com/22/groth16/index.html)
- [Zordle](https://github.com/nalinbhardwaj/zordle#readme): Wordle with zk proof to share results without revealing words

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-16-2022](https://weekinethereumnews.com/week-in-ethereum-news-july-16-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Jul 18 – [Devcon wave 01 tickets](https://devcon.org/en/tickets/)
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Jul 22-24 – [EthCC Hackathon](https://ethcchack.com/) (Paris)
- **Jul 24 –** [**EF Fellowship program**](https://fellowship.ethereum.foundation/) **applications close**
- Aug 5-13 – [ETH Seoul](https://2022.ethseoul.org/)
- Aug 8-10 – [ETHToronto](https://www.ethtoronto.ca/)
- Aug 11-13 – [ETH LATAM](http://ethlatam.org/) (Buenos Aires)
- Aug 19-21 – [ETHMexicoCity](https://mexico.ethglobal.com/) (ETH Global)
- **Aug 20-22 –** [**Paradigm CTF**](https://ctf.paradigm.xyz/)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev/) (hackathon & conference)
- Sep 2-28 – [ETHOnline](https://online.ethglobal.com/')  (ETH Global)
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Sep 16-18 - [EthBerlin](https://ethberlin.ooo/)
- Sep 27-29 – [Ethereum SP](https://twitter.com/Ethereum_Brasil/status/1530320916667895808) (São Paulo)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

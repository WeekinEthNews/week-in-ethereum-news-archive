---
title: "Week in Ethereum News <br> July 23, 2022"
date: "2022-07-23"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- Goerli is the final testnet to merge before mainnet, [TTD expected August 9-11](https://github.com/ethereum/execution-specs/pull/563)
- Goerli-shadow-fork-5 [merged successfully](https://twitter.com/abcoathup/status/1550421109199486977)
- [Mainnet-shadow-fork-10](https://twitter.com/abcoathup/status/1549951666203795456) merges July 28

**Mainnet execution layer**

- Latest core devs [call video](https://www.youtube.com/watch?v=N80PgxELDYg&t=183s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1550221047122628608) and [Christine Kim](https://twitter.com/i/notes/1550142474873610241):
    - Node operators need to run both execution & consensus layer clients
    - Fork ID to be set retroactively in clients a week post Merge
    - EL clients to enable Engine API for user setup before TTD is set
    - MEV-boost safeguards to prevent liveness failures are being documented, proposing to only use MEV-boost after the Merge has finalized 
    - Update on EIP4444 (bound historical data), next step to test export/import on Goerli testnet post Merge
- EthereumJS client [v0.6](https://github.com/ethereumjs/ethereumjs-monorepo/tree/master/packages/client/merge): PoS testnet support, sync JavaScript EL+CL clients
- Besu [v22.7.0-RC-2](https://github.com/hyperledger/besu/releases/tag/22.7.0-RC2): performance improvements & fixes
- KZG ceremony [call video](https://www.youtube.com/watch?v=7c4FybMLvjg&t=190s): test [website](https://trustedsetuptest.web.app/), planning contribution at Devcon
- Vitalik’s proposals to [adjust memory gas costs](https://notes.ethereum.org/@vbuterin/proposals_to_adjust_memory_gas_costs)

**Proof of Stake consensus layer**

- Lighthouse [v2.4.0](https://github.com/sigp/lighthouse/releases/tag/v2.4.0): mainnet improvements and Goerli testnet support
- Teku [v22.7.0](https://github.com/ConsenSys/teku/releases/tag/22.7.0): Goerli testnet support and panda Merge banner
- Lodestar [v0.41.0](https://github.com/ChainSafe/lodestar/releases/tag/v0.41.0): Goerli testnet support
- MEV-boost [info website](https://boost.flashbots.net/)
- Obol [Athena](https://blog.obol.tech/the-athena-testnet/) public testnet for Distributed Validator Technology middleware
- Miga Labs [validator migration experiments](https://medium.com/@migalabs/eth2-0-fluid-validator-migration-7c830557c154): 250 validators migrated across six clients

**Layer2**

- zkEVM zk-rollup announcements:
    - Polygon zkEVM [open sources implementation](https://blog.polygon.technology/the-future-is-now-for-ethereum-scaling-introducing-polygon-zkevm)
    - Scroll [pre-alpha testnet](https://mirror.xyz/scroll.eth/XQyXDgyxoefag6hcBgGJFz8qrb10rmSU-zUBvY3Q9_A)
    - zkSync v2.0 [roadmap](https://matterlabs.medium.com/100-days-to-mainnet-6f230893bd73), promises mainnet in 100 days
- [TxStreet transaction visualizer](https://twitter.com/txstreetCom/status/1549016696618377216) adds Arbitrum, beta 

**EIPs/Standards**

- [EIP4883](https://github.com/ethereum/EIPs/pull/4888/files): Composable SVG NFT 
- [EIP5269](https://github.com/ethereum/EIPs/pull/5269/files): ERC interface detection
- [EIP5289](https://github.com/ethereum/EIPs/pull/5289/files): Notary interface
- [EIP5313](https://eips.ethereum.org/EIPS/eip-5313): Light Contract Ownership 
- Discussion on [how EIP numbers should be picked](https://github.com/ethereum/EIPs/issues/5294)

* * *

### **This newsletter is made possible thanks to** [**SpeedRunEthereum**](https://speedrunethereum.com/)**!**

![SpeedRunEthereum](https://weekinethereumnews.com/wp-content/uploads/2022/04/Screenshot-from-2022-04-01-15-39-52.png)

[](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F02748e06-2396-4b28-9ace-17df408947b8_769x208.png)

Are you a web2 dev who wants to get into web3?  

The best way to go from _zero_ to **hero** is [SpeedRunEthereum.com](https://speedrunethereum.com/).

Learn how to build on Ethereum; the superpowers and the gotchas.

Then [speed run Ethereum](https://speedrunethereum.com/) by testing your skills in a [series of challenges](https://speedrunethereum.com/challenge/simple-nft-example) and [join web3](https://twitter.com/austingriffith/status/1493688828661432325).

* * *

**Stuff for developers**

- Remix [v0.25.0](https://medium.com/remix-ide/remix-v0-25-0-released-5b8902464413): clone Git repos, open Solidity from Etherscan & GitHub, Foundry remappings and improved provider labels for deploying
- [solady](https://github.com/Vectorized/solady#readme) (gas optimized Solidity snippets): MerkleProof, ECDSA, Sort, Base64, LibString, LibBitmap and SafeTransferLib
- [huffmate](https://github.com/pentagonxyz/huffmate#readme) (contract library in Huff): auth, data structures, math and tokens
- Paul R Berg’s [Foundry Template](https://github.com/paulrberg/foundry-template#readme) with PRBTest, Forge Std, Solhint, Prettier, GitHub Actions and Conventional Commits
- Nethereum [v4.7.0](https://github.com/Nethereum/Nethereum/releases/tag/4.7.0) (.Net library): new Unity library with better RPC client adapter support
- Tenderly [Gas Profiler](https://blog.tenderly.co/how-to-reduce-smart-contract-gas-usage/): analyze function gas usage
- New UI for OpenZeppelin’s [Ethernaut](https://ethernaut.openzeppelin.com/) CTF; StErMi’s [Ethernaut solutions](https://stermi.medium.com/lets-play-ethernaut-ctf-learning-solidity-security-while-playing-1678bd6db3c4)
- Ethernaut DAO CTF [car market solution](https://stermi.medium.com/ethernautdao-ctf-wallet-solution-1793f990c2d5)
- Tincho: [deep dive into what happens when sending 1 DAI](https://www.notonlyowner.com/learn/what-happens-when-you-send-one-dai)

**Security**

- PREMINT [300+ NFTs stolen](https://blog.premint.xyz/p/july-17-2022-incident-update), malicious JavaScript via image upload vulnerability
- OpenZeppelin Contracts advisory: [ERC165Checker](https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-qh9x-gcfh-pcrw) & [SignatureChecker](https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-4g63-c64m-25w9) may revert
- [ConsenSys Diligence](https://consensys.net/blog/diligence/smart-contract-auditing-with-turn-token/) auctioning NFTs for 40 hours of audit time
- List of historical [reentrancy attacks](https://github.com/pcaversaccio/reentrancy-attacks#readme)

**Ecosystem**

- EthCC [videos](https://www.youtube.com/channel/UC_kOxlaYNOTtNwtwySZ0B8w/videos) including Vitalik on [longer term future of the protocol](https://www.youtube.com/watch?v=kGjFTzRTH3Q)
- Polynya: [cancel/delay danksharding](https://polynya.mirror.xyz/sA0qPEbQ99HXCEXEi3BW34HXohMpLyDDM1a4AJhCF4E), proto-danksharding is enough
- Ethereum.org: [misconceptions about the Merge](https://ethereum.org/en/upgrades/merge/#misconceptions)

**Application layer**

- [Tabula](https://twitter.com/GnosisGuild/status/1549056708563140608): publications on IPFS with hash published on mainnet or sidechains
- [ENS Vision](https://www.ens.vision/): dedicated ENS marketplace 
- [ENS small grants](https://www.ensgrants.xyz/): 1 ETH grants for five projects each month
- Karma (DAO reputation) [Discord bot](https://twitter.com/showkarma_xyz/status/1550147940542341120) \[Disclosure: Starbloom portfolio\]

* * *

### **Job Listings**

- [Nexus Mutual: Frontend/Solidity](https://nexusmutual.recruitee.com/): Help build the web3 Risk Marketplace
- Status is hiring [UI Designer](https://grnh.se/8c816d6b1us) & [Web Developer](https://grnh.se/d64808fa1us). [All jobs!](https://jobs.status.im/)
- Overlay (backed by Polychain,1kx,ParaFi) hiring a [Senior Solidity Developer](https://www.notion.so/Overlay-Senior-Solidity-Dev-38c9130a01a844b39ef1bb81f82aae16)
- Ethereum Foundation seek a [Front End Developer](https://jobs.lever.co/ethereumfoundation/40ed733c-d3af-4026-b1b2-57ef7e70f788?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- GridPlus hiring a [Go/protocol dev for the private, scalable PhononDAO](https://gridplus.io/pages/careers#PhononEngineer)

**Job listings: $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US [DoJ](https://www.justice.gov/usao-sdny/pr/three-charged-first-ever-cryptocurrency-insider-trading-tipping-scheme) charged former Coinbase employee with wire fraud in insider trading scheme; [SEC](https://www.sec.gov/news/press-release/2022-127) insider trading charges labeled nine tokens as securities
    - [Coinbase](https://blog.coinbase.com/coinbase-does-not-list-securities-end-of-story-e58dc873be79) argues it doesn’t list securities
- [US government](https://twitter.com/OfficeGovEthics/status/1549141207670001664) employees must disclose NFTs & fractional NFTs over $1000 held for investment purposes
- [Minecraft](https://www.minecraft.net/en-us/article/minecraft-and-nfts) won’t allow NFT integrations or use of in-game content for NFTs

**General**

- Franklin [bid 100 ETH on their own joke ENS](https://twitter.com/franklinisbored/status/1549838025882042373), they accepted bot bid of 1.9 ETH without canceling original bid, original 100 ETH bid was then accepted
- [MEV in CFMMs](https://people.eecs.berkeley.edu/~ksk/files/MEV_CFMM.pdf) \[PDF\]: sandwich attacks in some scenarios can counterintuitively improve routing (inverse Braess paradox)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-23-2022](https://weekinethereumnews.com/week-in-ethereum-news-july-23-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Jul 24 – [EF Fellowship program](https://fellowship.ethereum.foundation/) applications close
- **Jul 26 –** [**Devcon wave 03 + 04 tickets**](https://devcon.org/en/tickets/)
- **Aug 1 –** [**Devcon Scholars**](https://scholars.paperform.co/) **applications close**
- Aug 5-13 – [ETH Seoul](https://2022.ethseoul.org/)
- Aug 8-10 – [ETHToronto](https://www.ethtoronto.ca/)
- **Aug 9-11 –** [**Goerli testnet merge**](https://github.com/ethereum/execution-specs/pull/563)
- Aug 11-13 – [ETH LATAM](https://ethlatam.org/) (Buenos Aires)
- **Aug 12 –** [**Merge Community Call #6**](https://github.com/ethereum/pm/issues/580)
- Aug 19-21 – [ETHMexicoCity](https://mexico.ethglobal.com/) (ETH Global)
- Aug 20-22 – [Paradigm CTF](https://ctf.paradigm.xyz/)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev/) (hackathon & conference)
- Sep 2-28 – [ETHOnline](https://online.ethglobal.com/')  (ETH Global)
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Sep 16-18 - [EthBerlin](https://ethberlin.ooo/)
- Sep 27-29 – [Ethereum SP](https://twitter.com/Ethereum_Brasil/status/1530320916667895808) (São Paulo)
- **Oct 7-16 –** [**Devcon week**](https://devcon.org/en/devcon-week/) **(Bogotá)**
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

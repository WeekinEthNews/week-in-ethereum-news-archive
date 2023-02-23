---
title: "Week in Ethereum News <br> June 18, 2022"
date: "2022-06-18"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- [Merge readiness checklist](https://launchpad.ethereum.org/en/merge-readiness/) for solo stakers & staking providers
- [Mainnet-shadow-fork-7](https://twitter.com/abcoathup/status/1536920372784025600) merges June 22, equal client split, test fixes deployed on Ropsten
- Sepolia testnet [permissioned beacon chain](https://twitter.com/terencechain/status/1536708573446561797) genesis June 20

**Mainnet execution layer**

- [Gray Glacier upgrade](https://blog.ethereum.org/2022/06/16/gray-glacier-announcement/) on block 15,050,000 (around June 29) to delay difficulty bomb by 700k blocks (~100 days) and place a hard limit by when the Merge must occur (unless major issues are found in testing requiring a bomb delay).
- Update your execution layer clients for Gray Glacier:
    - Besu [v22.4.3](https://github.com/hyperledger/besu/releases/tag/22.4.3)
    - Erigon [v2022.06.04-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.06.04) & [v2022.04.05-deprecated](https://github.com/ledgerwatch/erigon/releases/tag/v2022.04.05) (ex-beta)
    - Geth [v1.10.19](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.19)
    - Nethermind [v1.13.3](https://github.com/NethermindEth/nethermind/releases/tag/1.13.3)
- Besu [Grafana dashboard](https://grafana.com/grafana/dashboards/16455)
- EIP4844 [call video](https://www.youtube.com/watch?v=flx1hDUV8O0).  Recap by [Tim Beiko](https://twitter.com/TimBeiko/status/1537869030857486337) and [notes](https://docs.google.com/document/d/1KgKZnb5P07rdLBb_nRCaXhzG_4PBoZXtFQNzKO2mrvc/edit): 
    - Demo of prototype sending, retrieving and verifying blob data; currently outstanding is sync and blob fee market
    - Prototype of [KZG ceremony](https://github.com/dknopik/towers-of-pau#readme) done at EthPrague by Daniel Knopik and Marius Van Der Wijden

**Proof of Stake consensus layer**

- PoS implementers [call video](https://www.youtube.com/watch?v=WHOZ_2tlTqk&t=164s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/HJFkBhdK9):
    - Builder API (MEV boost) implementation & testing progress
    - Recommend not running MEV boost until ~1 hour after the Merge
    - Walkthrough of proposal for post-Merge deposit processing
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220617)
- Teku [v22.6.0](https://github.com/ConsenSys/teku/releases/tag/22.6.0): Sepolia testnet config, optimized epoch transition & fork choice updates
- Lodestar [v0.38.1](https://github.com/ChainSafe/lodestar/releases/tag/v0.38.1): Sepolia testnet config
- Lighthouse [v2.3.1](https://github.com/sigp/lighthouse/releases/tag/v2.3.1): fix for clock drift and optimisations to epoch processing
- Polynya estimates [PoS will use 0.3% silicon resources of PoW](https://twitter.com/epolynya/status/1537292430017372160)

**EIPs/Standards**

- ERC4626 tokenized vault standard [promo website](https://erc4626.info/)
- [EIP5164](https://github.com/ethereum/EIPs/pull/5164/files): Cross-Chain Execution
- [EIP5163](https://github.com/ethereum/EIPs/pull/5163/files): Rich Site-Proposed Contract Metadata

* * *

### **This newsletter is made possible thanks to** [**Nexus Mutual**](https://nexusmutual.io/)**!**

![Nexus Mutual Protocol Cover](https://weekinethereumnews.com/wp-content/uploads/2022/03/Nexus-Mutual-Protocol-Cover-1024x586.png)

[](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F57111adf-f627-4a76-b0fc-c2bbd01d173e_1600x915.png)

Go where the yield takes you, but don’t let the next hack set you back. Regardless of where you are chasing yield, Protocol Cover can protect your productive crypto assets across L1s, L2s, and scaling solutions. 

Maximize yield. Minimize risk. Enjoy peace of mind knowing Nexus Mutual has you covered. [Become a member](https://nexusmutual.io/) and cover your asse(t)s against the major risks in DeFi.

* * *

**Stuff for developers**

- Solidity [v0.8.15](https://blog.soliditylang.org/2022/06/15/solidity-0.8.15-release-announcement/): fix for optimizer removing some memory writes in inline assembly ([found by Certora](https://medium.com/certora/overly-optimistic-optimizer-certora-bug-disclosure-2101e3f7994d)), fix for writing dirty values when copying bytes arrays, improved inlining and selector for events & custom errors
- [Tenderly](https://blog.tenderly.co/new-features-web3-actions-war-rooms-sandbox-debugger-extension/) adds serverless functions, sandbox, war room aid kit and debugger Chrome extension
- Ape [v0.3.0](https://github.com/ApeWorX/ape/releases/tag/v0.3.0): (contract dev framework) Geth & Parity-style tracing and new caching APIs
- [eth\_lift](https://github.com/storming0x/ethlift-rs#readme) ethdiff: diff of local Solidity file (Foundry & Brownie) vs Etherscan verified source
- [zk Soul-Bound token](https://github.com/enricobottazzi/ZK-SBT#readme) using iden3 and Circom
- [Hardhat-circom v3.2.x](https://github.com/projectsophon/hardhat-circom/releases/tag/v3.2.2): circuit testing integrated with Mocha, export calldata from Groth16 & PLONK snarkjs bindings
- Sepolia testnet [RPC](https://twitter.com/unnawut/status/1536835158481211392)
- [Sol Challenge](https://github.com/massun-onibakuchi/sol-challenge#readme): CTF challenges, tests in TypeScript 
- StErMi’s [solutions to EVM puzzles](https://stermi.medium.com/lets-play-evm-puzzles-learning-ethereum-evm-while-playing-43a8354a02b3)
- [Merkle tree gas optimization](https://twitter.com/krzKaczor/status/1536353263519514624) using tightly packed bitfields
- [Decompiling](https://noxx.substack.com/p/mev-memoirs-into-the-arena-chapter-3e9) an unverified MEV bot contract

**Security**

- Inverse Finance [$5.8 million oracle price manipulation](https://rekt.news/inverse-rekt2/), [attack was backrun](https://twitter.com/mevrefund/status/1537421091697836032) by arb bot otherwise it would have been frontrun by generalized frontrunner
- OpenSea [Shared Storefront config vulnerability](https://twitter.com/z0age/status/1537276889504415744), allowed selling of Shared Storefront NFTs that the seller didn’t own
- [Browser extension wallet vulnerability](https://halborn.com/halborn-discovers-critical-vulnerability-affecting-crypto-wallet-browser-extensions/) that could allow access to secret recovery phrase in plain text where the user viewed the phrase on import on a non-encrypted hard drive; patched in [MetaMask](https://medium.com/metamask/security-notice-extension-disk-encryption-issue-d437d4250863) 
- Certora Prover finds that a [Maker invariant was a variant](https://hackmd.io/@SaferMaker/DAICertoraSurprise)

**Ecosystem**

- Vitalik: [non-financial use cases of blockchains](https://vitalik.ca/general/2022/06/12/nonfin.html) and [privacy use cases of ZK-SNARKs](https://vitalik.ca/general/2022/06/15/using_snarks.html)
- ETH Prague [hackathon projects](https://ethprague-2022.devpost.com/project-gallery)
- Propose [locations for Devcon 7](https://forum.devcon.org/t/propose-locations-for-devcon-7/359)

**Application layer**

- [OpenSea migrating to Seaport](https://opensea.io/blog/announcements/launching-seaport-saving-the-community-millions-in-fees/): removes setup fee, lower gas costs, allows offers on collections and traits
- [Nouns Vision Glasses](https://nounsvision.com/): NFT to redeem for physical Nouns glasses
- MetaMask adds [Dark Mode](https://twitter.com/MetaMask/status/1537480157706915841) to browser extension
- [CAPE](https://twitter.com/EspressoSys/status/1537431407621832707) (Configurable Asset Privacy for Ethereum) on Goerli testnet, wrap ERC20 tokens into a token with customizable privacy 
- [Maker DAO](https://vote.makerdao.com/executive/template-executive-vote-temporarily-disable-the-aave-dai-direct-deposit-module-d3m-june-15-2022#proposal-detail) voted to disable Aave DAI direct deposit module (D3M) due to market conditions
- Circle launching [Euro Coin](https://www.circle.com/blog/euro-coin-is-coming-on-june-30) (asset backed stablecoin) on June 30

* * *

### **Job Listings**

- Taiko ZKRollup: [zkEVM researchers/developers](https://taiko.xyz/career) wanted.
- Status is hiring! [Communications & Activism Director](https://grnh.se/0a1f0ea71us) See: [All jobs](https://grnh.se/9fc6e6fc1us)
- Sourcify: [TypeScript/nodejs developer](https://jobs.lever.co/ethereumfoundation/db85cf1d-6ffd-42a6-8f0d-f5a91c6ddf4a?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) wanted
- [Hiring Coordinator](https://jobs.lever.co/ethereumfoundation/7f5bf10b-ea68-4364-a378-e34ae345a212?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) wanted by EF
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)
- [People Operations Lead](https://jobs.lever.co/ethereumfoundation/8046bbe5-6343-4ecf-8296-37dc2a5bf915?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) at EF
- EF: [generalist developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) to drive strategic ecosystem initiatives

**Job listings: $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet/Arbitrum/Optimism. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Coin Center](https://www.coincenter.org/coin-center-has-filed-a-court-challenge-against-the-treasury-dept-over-unconstitutional-financial-surveillance/) court challenge of US Treasury tax code requirement to report date of birth & social security number of sender when receiving $10k in crypto
- Attempt to [serve notice via NFT](https://twitter.com/jerrygianakis/status/1536423045140725760) in the US on an anonymous defendant
- US SEC Commissioner Peirce: “[I have no idea](https://www.sec.gov/news/speech/peirce-remarks-regulatory-transparency-project-conference)” why the SEC does nothing on crypto ETFs
- Rekt: [Celsius](https://rekt.news/celsius-rekt/) CeFi lender paused withdrawals, swaps and transfers
- WSJ: [Three Arrows Capital considering asset sales or bailout](https://www.wsj.com/articles/battered-crypto-hedge-fund-three-arrows-capital-considers-asset-sales-bailout-11655469932) after heavy losses

**General**

- Proposed [off-chain & scriptless mixer](https://ethresear.ch/t/offchain-and-scriptless-mixer/12851) using an MPC
- [Skiff Drive](https://twitter.com/skiffprivacy/status/1537119521382666241): end-to-end encrypted file storage, 10Gb free
- [Backdoored versions of mobile wallets](https://blog.confiant.com/how-seaflower-%E8%97%8F%E6%B5%B7%E8%8A%B1-installs-backdoors-in-ios-android-web3-wallets-to-steal-your-seed-phrase-d25f0ccdffce) created to steal secret recovery phrases
- [Hertzbleed](https://www.hertzbleed.com/): remote timing attack on constant-time cryptographic code on x86 CPUs

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-june-18-2022](https://weekinethereumnews.com/week-in-ethereum-news-june-18-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 23 – [Gitcoin Grants Round 14](https://gitcoin.co/grants/) ends (support [Week in Eth News](https://gitcoin.co/grants/2785/week-in-ethereum-news))
- Jun 24-26 – [ETH NYC](https://nyc.ethglobal.co/) (ETH Global)
- Jun 27 – [Devcon speaker](https://devcon.org/en/applications/) applications close
- **Jun 29 –** [**Gray Glacier upgrade**](https://blog.ethereum.org/2022/06/16/gray-glacier-announcement/) **(block 15,050,000)**
- Jun 30 – [Devcon discounted ticket](https://devcon.org/en/tickets/) applications close
- Jul 1 – [Data Availability Sampling](https://github.com/ethereum/requests-for-proposals/blob/master/open-rfps/das.md) proposals due
- Jul 6-8 – [ETHBarcelona](https://ethbarcelona.com/)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 18 – [Devcon wave 01 tickets](https://devcon.org/en/tickets/)
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 5-13 – [ETH Seoul](https://2022.ethseoul.org/)
- Aug 8-10 – [ETHToronto](https://www.ethtoronto.ca/)
- Aug 11-14 – [ETH LATAM](https://twitter.com/ethlatam/status/1524146640474587137) (Buenos Aires)
- Aug 19-21 – [ETHMexicoCity](https://mexico.ethglobal.com/) (ETH Global)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- **Aug 27-28 –** [**HackSummit**](https://sf.hacksummit.org/) **(San Francisco)**
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev/) (hackathon & conference)
- Sep 2-28 – [ETHOnline](https://online.ethglobal.com/')
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 8-10 – [ETHSantiago](https://twitter.com/EthereumStgo)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Sep 16-18 - [EthBerlin](https://ethberlin.ooo/)
- Sep 27-29 – [Ethereum SP](https://twitter.com/Ethereum_Brasil/status/1530320916667895808) (São Paulo)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- **Oct 10 –** [**DeFi Bogotá**](https://2022.defibogota.org/)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 18-20 – ETHGlobal [Web3 Weekend](https://web3weekend.ethglobal.com/)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

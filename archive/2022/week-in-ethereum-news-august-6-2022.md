---
title: "Week in Ethereum News <br> August 6, 2022"
date: "2022-08-06"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- [Mainnet Merge TTD & Bellatrix epoch](https://twitter.com/TimBeiko/status/1555251189721075713) to be set next week on the consensus layer call assuming Goerli merge goes well, Merge TTD will be updated on next core devs call if 5GB DAG size causes a big drop in hashrate
- Goerli testnet merge:
    - Beacon chain (Prater) [upgraded to Bellatrix](https://twitter.com/terencechain/status/1555190240838832134)
    - Bordel [predicts Goerli merge](https://bordel.wtf/) August 10-11
    - Goerli-shadow-fork-6 [merged successfully](https://twitter.com/abcoathup/status/1555436779313852416), no client issues, [30% ran MEV-boost](https://boost.flashbots.net/mev-boost-status-updates/successful-mev-boost-testing-through-goerli-shadow-fork-6-merge)
- [Sepolia testnet post-Merge upgrade](https://blog.ethereum.org/2022/08/03/sepolia-post-merge-upgrade/) at block 1735371 (August ~17), update your execution layer clients to disconnect peers that haven’t transitioned to PoS

**Execution layer**

- Latest core devs [call video](https://www.youtube.com/watch?v=vJYzfRH62Ok&t=225s). Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1555241740113547264) and [Christine Kim](https://docsend.com/view/2asfhwi2z5ierk4k):
    - Proposed post-merge Engine API & Checkpoint Sync changes
    - Flashbots open sourcing MEV-boost relay in September
    - Executable spec for execution layer to be tried in parallel to Core EIPs
- Besu [v22.7.0](https://github.com/hyperledger/besu/releases/tag/22.7.0): peering improvements and Merge fixes
- KZG ceremony [call video](https://www.youtube.com/watch?v=BDPQBVP6XHs): Python implementation of the spec
- [Verifying large amounts of KZG multiproofs](https://ethresear.ch/t/a-universal-verification-equation-for-data-availability-sampling/13240) for Data Availability Sampling
- Academic paper finds F2pool manipulated [time stamps](https://medium.com/@aviv.yaish/uncle-maker-time-stamping-out-the-competition-in-ethereum-d27c1cb62fef) to maximize their profits by uncling other blocks

**Proof of Stake consensus layer**

- [Beacon chain deposits](https://twitter.com/etherscan/status/1554105870245433345): Lido at 31%, Coinbase + Kraken + Binance at 30%, only ~14% of validators are unlabeled
- Lighthouse [v2.5.1](https://github.com/sigp/lighthouse/releases/tag/v2.5.1): fixes for 100MB per month memory footprint increase & fork choice error
- Teku [v22.8.0](https://github.com/ConsenSys/teku/releases/tag/22.8.0): MEV-boost support, libp2p & fork choice optimizations
- Prysm [v2.1.4-rc.1](https://github.com/prysmaticlabs/prysm/releases/tag/v2.1.4-rc.1): Goerli merge support
- [Flashbots](https://writings.flashbots.net/writings/understanding-mev-boost-liveness-risks/) building a [relay monitor](https://hackmd.io/@ralexstokes/SynPJN_pq) & circuit breaker for MEV-boost as defense against block withholding attacks

**Layer2**

- Arbitrum One [upgrades to Nitro](https://medium.com/offchainlabs/prepare-your-engines-nitro-is-imminent-a46af99b9e60) August 31
- Delphi Digital: [guide to rollups](https://members.delphidigital.io/reports/the-complete-guide-to-rollups)
- Vitalik: [zk-EVM types & tradeoffs](https://vitalik.eth.limo/general/2022/08/04/zkevm.html), Ethereum-equivalent, EVM-equivalent (full, full except for gas costs & almost) and high-level-language equivalent
- BLS Wallet [overview & demo](https://medium.com/privacy-scaling-explorations/bls-wallet-bundling-up-data-fb5424d3bdd3), bundles actions signed with BLS signatures to reduce data stored on chain & transaction costs

**EIPs/Standards**

- [EIP4987](https://eips.ethereum.org/EIPS/eip-4987): Held token interface 
- [EIP5283](https://github.com/ethereum/EIPs/pull/5283/files): Semaphore for Reentrancy Protection
- [EIP5375](https://github.com/ethereum/EIPs/pull/5375/files): NFT Author Information and Consent
- [EIP5380](https://github.com/ethereum/EIPs/pull/5380/files): ERC721 Entitlement Extension
- [EIP5409](https://github.com/ethereum/EIPs/pull/5409/files): ERC1155 Non-Fungible Token extension

* * *

### **This newsletter is made possible thanks to** [**Hardhat**](https://hardhat.org/)**!**

![](https://weekinethereumnews.com/wp-content/uploads/2021/06/hardhat-rectangle-1024x325.png)

[](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F031a7efa-a9c2-4656-9eec-eaaf79e28665_1400x441.png)

The Hardhat for Visual Studio Code extension adds language support for Solidity to Visual Studio Code, and provides editor integration for Hardhat projects.

It supports:

- Code completion
- Go to definition, type definition and references
- Symbol renames
- Solidity code formatting
- Inline code validation from compiler errors/warnings for Hardhat projects
- Hover help for variables, function calls, errors, events etc.
- Code actions (quick fixes) suggested from compiler errors/warnings for Hardhat projects
    - Implement missing functions on interface with stubs
    - Constrain mutability by adding `view/pure` to function signature
    - Meet inheritance requirements by adding `virtual/override` on function signature
    - Provide accessibility by adding `public/private` to function signature

Get it from the [VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=NomicFoundation.hardhat-solidity)

* * *

**Stuff for developers**

- Foundry [fuzz test 2x speedup](https://twitter.com/gakonst/status/1554505392452882432) via caching bytecode analysis
- Tenderly [Sandbox](https://blog.tenderly.co/how-to-prototype-smart-contracts-in-tenderly-sandbox/): prototype contracts in a browser
- web3.js [v1.7.5](https://github.com/ChainSafe/web3.js/releases/tag/v1.7.5): security update of dependencies, doc updates & fixes 
- [snekmate](https://github.com/pcaversaccio/snekmate#readme): Vyper building blocks; ECDSA, CreateAddress, Create2Address & EIP712
- [ethp2p](https://github.com/rjected/ethp2p#readme) (Rust): encode/decode raw Eth p2p messages
- [ConnectKit](https://twitter.com/family/status/1554545269764603904): React components to connect wallets, uses wagmi, beta 
- Ethernaut DAO CTF [EthernautDAOToken solution](https://stermi.xyz/blog/ethernautdao-ctf-ethernautdao-token-solution)
- [evm.elf](https://github.com/axic/evm.elf#readme): code that is valid EVM and Linux binary (ELF)
- [BrainSTARK](https://aszepieniec.github.io/stark-brainfuck/): guide to designing a Turing-complete zk-STARK engine for the Brainfuck language
- Google [Paranoid](https://github.com/google/paranoid_crypto#readme) library: check cryptographic artifacts for known weaknesses

**Security**

- Nomad bridge [$190 million exploit](https://rekt.news/nomad-rekt/), invalid messages were treated as proven after upgrade changed message checking, exploit had multiple copycats
    - Currently ~20% [has been returned](https://etherscan.io/address/0x94A84433101A10aEda762968f6995c574D1bF154)
- Pre-audit [checks](https://jeffrey-scholz.medium.com/the-ultimate-100-point-checklist-before-sending-your-smart-contract-for-audit-af9a5b5d95d0) for contracts
- Projects need users to agree [10% bug bounty reward in advance](https://micah-zoltu.medium.com/how-to-change-your-black-hats-into-white-hats-91bc676cd9a3)

**Ecosystem**

- Finematics: [Merge explainer video](https://finematics.com/the-ethereum-merge-explained/)

**Enterprise**

- Instagram [NFT support](https://twitter.com/MetaNewsroom/status/1555197567532732417) expands to 100 countries
- [Tiffany & Co NFTiffs](https://nft.tiffany.com/): 250 CryptoPunk custom pendants & matching NFTs sold out quickly for 30 ETH each
- EEA: [NIST compliance](https://entethalliance.org/opinion-enterprise-blockchains-redux-how-to-be-not-not-nist-compliant-without-breaking-the-bank/) for blockchain applications

**Application layer**

- Proposal to [create Uniswap Foundation](https://gov.uniswap.org/t/temperature-check-create-the-uniswap-foundation/17358)
- PoolTogether [delegation](https://medium.com/pooltogether/the-best-way-to-get-your-friends-into-defi-f1cef2561241): delegate a deposit to a user who only has a wallet
- [dWeb Services](https://twitter.com/dweb_services/status/1554457150595932166): ENS website IPNS pinning service
- Metagame [Logbook NFT](https://twitter.com/BrennerSpear/status/1555320481560944640) of human readable transactions
- [Moonbirds](https://twitter.com/kevinrose/status/1555262099093200896) NFTs moving to CC0 license
- [SongADEX](https://twitter.com/songadaymann/status/1555620350653865984): Song a day NFT trait collecting

* * *

### **Job Listings**

- Ethereum Foundation seek a [People Operations Lead](https://jobs.lever.co/ethereumfoundation/8046bbe5-6343-4ecf-8296-37dc2a5bf915?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Overlay (backed by Polychain,1kx,ParaFi) hiring a [Senior Solidity Developer](https://www.notion.so/Overlay-Senior-Solidity-Dev-38c9130a01a844b39ef1bb81f82aae16)
- ØVIX + GOGO Protocol: [Senior DeFi Blockchain Developer](https://bit.ly/3zc7N4o) & [VP of Engineering](https://bit.ly/3Bk05I3)
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)

**Job listings: $600** for four issues (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Forsage founders & promoters charged](https://www.sec.gov/news/press-release/2022-134) in alleged fraudulent pyramid scheme
- [Dropil founders sentenced](https://www.justice.gov/usao-cdca/pr/two-orange-county-men-sentenced-federal-prison-conning-investors-out-19-million-through) to US federal prison for securities fraud
- [US CFTC rugpulls PredictIt's](https://www.predictit.org/platform-announcements) de facto regulatory approval

**General**

- 9k private keys compromised on Solana: [Slope mobile wallet](https://twitter.com/slope_finance/status/1555100731706949639) logged secret recovery phrases to a central server in plain text, investigation still ongoing
- CoinDesk: [dev created 11 identities for interlocking protocols](https://www.coindesk.com/layer2/2022/08/04/master-of-anons-how-a-crypto-developer-faked-a-defi-ecosystem/) to invent 75% of Solana’s TVL
- Helium has [~$2b market cap despite just ~$6500 in monthly wireless revenue](https://mashable.com/article/helium-lime-web3-crypto)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-6-2022](https://weekinethereumnews.com/week-in-ethereum-news-august-6-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Aug 6-12 – [Goerli testnet merge](https://blog.ethereum.org/2022/07/27/goerli-prater-merge-announcement/)
- Aug 8-10 – [ETHToronto](https://www.ethtoronto.ca/)
- **Aug 11 –** [**Devcon wave 07 + 08 tickets**](https://devcon.org/en/tickets/)
- Aug 11-13 – [ETH LATAM](https://ethlatam.org/) (Buenos Aires)
- Aug 12 – [Merge Community Call #6](https://github.com/ethereum/pm/issues/580)
- Aug 19-21 – [ETHMexicoCity](https://mexico.ethglobal.com/) (ETH Global)
- Aug 20-22 – [Paradigm CTF](https://ctf.paradigm.xyz/)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev/) (hackathon & conference)
- Sep 2-28 – [ETHOnline](https://online.ethglobal.com/')  (ETH Global)
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- **Sep 9-11 –** [**Ethereum SP**](https://www.ethereumbrasil.com/#next) **(São Paulo)**
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Sep 16-18 - [EthBerlin](https://ethberlin.ooo/)
- **Sep 23 -** [**ETH HCMC**](https://2022.ethhcmc.com/) **summit (Ho Chi Minh)**
- **Sep 23-24 -** [**ETHSantiago**](https://ethsantiago.com/)
- Oct 7-16 – [Devcon week](https://devcon.org/en/devcon-week/) (Bogotá)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- Oct 7-9 – [Infinite hackathon](https://infinite-hackathons.eth.limo/) (Bogotá)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

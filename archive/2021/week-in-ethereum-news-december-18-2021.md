---
title: "Week in Ethereum News <br> December 18, 2021"
date: "2021-12-18"
---

## **Eth News and Links**

**Mainnet execution layer**

- [Kintsugi testnet](https://kintsugi.themerge.dev/) is live for the next month, help test PoW switch off:
    - Add testnet to MetaMask, [get 50 testnet Ether](https://faucet.kintsugi.themerge.dev/), use the testnet!
    - Join the testnet; [guide to joining with Geth & Lighthouse](https://github.com/remyroy/ethstaker/blob/main/merge-devnet.md)
    - [Testing ideas](https://hackmd.io/WKpg6SNzQbi1jVKNgrSgWg) for technical folks
- Erigon [v2021.12.03](https://github.com/ledgerwatch/erigon/releases/tag/v2021.12.03): Transaction pool debugging for specific sender addresses 
- Besu [v21.10.4](https://github.com/hyperledger/besu/releases/tag/21.10.4): update due to additional log4j vulnerability
- Proposal to [streamline gas accounting](https://notes.ethereum.org/@vbuterin/verkle_write_gas_extension) under Verkle trees

**EIPs/Standards**

- [EIP4521](https://github.com/ethereum/EIPs/blob/43d367eacca27bb6e251a7a7e783921b9b277695/EIPS/eip-4521.md): ERC721/20-compatible transfer
- [EIP4546](https://github.com/ethereum/EIPs/blob/7069a3c4b6c59e755a000fc870b0085920eadb2c/EIPS/eip-4546.md): Wrapped Deposits
- [EIP4573](https://github.com/ethereum/EIPs/blob/5b0e6575d0eb7578f238b52e78b85d12fa6989e4/EIPS/eip-4573.md): Entry Points and Procedures for EVM Code Sections

**Proof of Stake consensus layer**

- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_211217)
- PoS implementers call (no recording). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/HyxWQTdqY): working on optimistic sync (ideas welcome)
- [Light client sync](https://hackmd.io/s0mC78fHSZqhssRwJbLK9g), alternative to optimistic sync
- Teku [v21.12.2](https://github.com/ConsenSys/teku/releases/tag/21.12.2): update due to additional log4j vulnerability
- Armiarma beacon chain crawler [v1](https://medium.com/@migalabs/presenting-the-ant-crawler-release-6268387a88dc) (Ant crawler): 58.8% are Prysm nodes

**Layer2**

- [Optimism](https://optimismpbc.medium.com/all-gas-no-brakes-8b0f32afd466) deployment now permissionless; future updates will maintain state, transaction history and event data
- [Immutable X](https://support.immutable.com/hc/en-us/articles/4411697220879/) fiat on-ramp via MoonPay
- [Polygon Nightfall](https://blog.polygon.technology/zk-proofs-protocol-polygon-nightfall-launches-on-testnet-to-provide-low-cost-private-ethereum-transaction/) zk-optimistic rollup testnet
- Arbitrum [compares ZK and Optimistic Rollups](https://medium.com/offchainlabs/optimistic-rollups-the-present-and-future-of-ethereum-scaling-60fb9067ae87)
- Optimistic Rollups 7-day fraud proof window [explainer](https://twitter.com/bkiepuszewski/status/1471116288261038088)
- Celer’s call for an [open canonical token bridge standard](https://blog.celer.network/2021/12/13/say-no-to-vendor-lock-in-calling-for-an-open-canonical-token-bridge-standard/)

* * *

### **This newsletter is made possible thanks to Starbloom Ventures!**

![Starbloom Ventures](https://weekinethereumnews.com/wp-content/uploads/2021/11/Screenshot-from-2021-11-19-15-25-51.png)

Starbloom Ventures is a new early-stage venture fund by Evan Van Ness and James Fickel to invest in the future of web3. 

What does it mean to invest in the future of web3?  This week we published our [request for startups](https://twitter.com/evan_van_ness/status/1471593545085734922).

We’re pledging [10% of profits to support Ethereum public goods](https://twitter.com/evan_van_ness/status/1461840784819425288).  Why isn’t your favorite VC taking the pledge?

* * *

**Stuff for developers**

- [ethereum-code-viewer](https://github.com/dethcrypto/ethereum-code-viewer): open Etherscan verified contracts in browser instance of VS Code, supports multi-file contracts & proxies, just change etherscan contract URL from “.io” to “.deth.net”
- Hardhat [v2.8.0](https://github.com/nomiclabs/hardhat/releases/tag/hardhat%402.8.0): custom hardfork history to fork non-supported networks
- Otterscan [v2021.12.02](https://github.com/wmitsuda/otterscan/releases/tag/v2021.12.02-otterscan): support for revert reasons & custom errors
- [StarkNet.py](https://github.com/software-mansion/starknet.py): StarkNet SDK for Python
- [ApeWorX](https://www.getrevue.co/profile/ApeWorX/issues/introducing-apeworx-beta-issue-1-940734): Python based modular development framework, beta
- [Subway](https://github.com/libevm/subway): example sandwich bot for UniswapV2 pairs
- [Comparison of BigQuery, Nansen, and Dune Analytics](https://mirror.xyz/barniker.eth/J6s7SYB4hUc90LXb7s0lmSNCIydrA2AzxHJep445_xw) using example of querying historical floor price
- MakerDAO [developer survey](https://makerdao.typeform.com/to/eZ4IDyss)

**Security**

- Gelato [G-UNI Router vulnerability](https://twitter.com/gelatonetwork/status/1469813838916866050), $26 million secured with no funds lost, alerted by samczsun, revoke approvals given to vulnerable contract
- Umbra [frontend bug disclosure](https://www.scopelift.co/blog/umbra-frontend-bug-disclosure), no funds lost or at risk, check account is configured properly
- [NFT holder phished](https://twitter.com/dingalingts/status/1470095710888808449), apparent airdrop claim signed using hardware wallet was actually private sale of two NFTs on OpenSea
- Key extraction attacks on [threshold ECDSA implementations](https://hackmd.io/@omershlo/Sk_8JT-qt), $500k bounty paid
- PLONK ZKP C++ [attack using zero](https://cryptosubtlety.medium.com/00-8d4adcf4d255) to create a forged proof that verifiers accept, $15k bounty paid
- Learn to be an auditor at the next [Secureum bootcamp](https://twitter.com/0xRajeev/status/1470910752085065731), starts in January

**Ecosystem**

- Ethereum Foundation [client incentive program](https://blog.ethereum.org/2021/12/13/client-incentive-program/): nine client teams receive 144 validators (4608 ETH) each (50% for Lodestar), withdrawal credentials are vested, first tranche released when withdrawals enabled
- Ethereum.org page on [energy consumption](https://ethereum.org/en/energy-consumption/)
- MetaMask [Transaction Insight](https://metamask.zendesk.com/hc/en-us/articles/4412543412123): decodes transaction data to more human readable format
- Guide to [SQRL](https://medium.com/chainsafe-systems/sqrl-ing-mnemonic-phrases-97e23491bddc) (Simultaneous Qualified Roots with Lure): create a canary account for a secret mnemonic, whilst valuable assets are controlled by the mnemonic plus an extra word using a hardware wallet
- Flashbots: [importance of building the most profitable block](https://writings.flashbots.net/writings/on-the-most-profitable-block/)
- Starter guide to [MEV](https://github.com/0xmebius/mev/blob/main/MEV101.pdf) \[PDF\]
- Ethereum Foundation’s [Devconnect](https://blog.ethereum.org/2021/12/13/announcing-devconnect/): Amsterdam April 2022, bring community together in small groups to discuss, learn & make progress
- [ETHGlobal](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4) 2022 events: Amsterdam, New York, Mexico City, San Francisco, Taipei & Bogota, plus virtual events HackMoney & ETHOnline

**Enterprise**

- [Shopify NFT beta](https://www.shopify.com/nft): mint/airdrop/sell using crypto or fiat, open to US Shopify Plus merchants
- [ConsenSys Rollups](https://consensys.net/blog/press-release/consensys-launches-consensys-rollups-with-the-support-of-mastercard-fostering-innovation-and-scalability-on-the-ethereum-mainnet-for-private-and-permissioned-blockchains/): zk-rollups for mainnet or private ConsenSys Quorum networks, with support from Mastercard
- Adidas Originals sold out 30k [NFTs](https://www.adidas.com/into_the_metaverse) for access to experiences & products
- [NIKE acquires RTFKT](https://news.nike.com/news/nike-acquires-rtfkt) (NFT studio)
- [L'Oréal Paris USA five 1-1 NFTs](https://www.lorealparisusa.com/nft-art), artists retain 100% of sales & 50% of royalties

**Application layer**

- [Lyra](https://blog.lyra.finance/lyra-is-live/) (options trading) token launched natively on Optimism
- Uniswap [Auto Router v2](https://uniswap.org/blog/auto-router-v2): routes across Uniswap v2 & v3, supports Layer 2 and real-time gas estimates
- 1inch [Limit Order Protocol v2](https://blog.1inch.io/the-1inch-limit-order-protocol-v2-is-released-81c6802db1bd): gasless limit orders for ETH and support for DAI style permits
- [Euler](https://blog.euler.finance/euler-launches-on-mainnet-507f343bbe0e) lending markets guarded launch on mainnet
- Balancer [Boosted Pools](https://medium.com/balancer-protocol/balancer-launches-boosted-pools-to-increase-lp-yields-ba3daadb59f9) launches with AAVE, deposit excess liquidity into lending protocols to earn yield
- [Element Finance](https://medium.com/element-finance/fixed-rates-for-everyone-l2-scaling-is-coming-to-element-a4eaaf6957f1) scaling with Aztec Network zk-rollup
- [VeVe migrated 3 million licensed NFTs](https://twitter.com/veve_official/status/1471258952583168000?s=20) to Immutable X
- [Mintable](https://twitter.com/mintable_app/status/1469529421694394370) integrates with Immutable X, gas free minting & trading
- [Unlock Protocol](https://unlock-protocol.com/blog/unlock-protocol-wordpress-plugin) WordPress plugin for content access via NFTs
- [Intergalactic Neon Tokens](https://twitter.com/smpalladino/status/1469881372273790984): on-chain animated SVG NFTs of token symbols based on price

* * *

### **Job Listings**

- [Textile](https://textile.io/) is hiring! [Blockchain Eng](https://grnh.se/f093ec154us), [Backend Eng](https://grnh.se/526aef8d4us), and [Partner Manager](https://grnh.se/06c1dfdf4us)
- IoBuilders is hiring: [Enterprise blockchain devs](https://www.linkedin.com/jobs/view/2753213671), [product managers](https://www.linkedin.com/jobs/view/2753213143) & [more](https://www.linkedin.com/company/iobuilders)
- Kwenta seeks [Frontend Engineer](https://blog.kwenta.io/kwenta-open-position-front-end-developer/), [Solidity Engineer](https://blog.kwenta.io/kwenta-open-position-solidity-engineer/) & [Marketing Lead](https://blog.kwenta.io/kwenta-open-position-marketing-manager/)
- EFF hiring a [Senior Fellow of Decentralization](https://www.eff.org/deeplinks/2021/12/dream-job-alert-senior-fellow-decentralization-eff)
- Bloom Institute of Technology (fka Lambda school) seek [Solidity experts](https://jobs.lever.co/BloomTech/c3ff6acf-c8ad-4957-b1a9-23a5f693598f) 
- OpenZeppelin are hiring a [Community Manager](https://openzeppelin.com/jobs/opening/?gh_jid=4847457003)
- Ethereum Foundation: [DevOps](https://ethereum.bamboohr.com/jobs/view.php?id=53&source=weekinethnews) for Consensus Layer clients in lead up to merge

**Reach developers experienced with Ethereum.  DECEMBER SPECIAL: $200** for two issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US SEC Republican members issue [strong dissent from Gensler’s heavy-handed regulatory agenda](https://www.sec.gov/news/statement/peirce-roisman-falling-further-back-121321)
- AAVE governance votes for [AAVE v3 to use a business license](https://snapshot.org/#/aave.eth/proposal/0x483f30ac318ac7e26fbc9804a48ccd9126078d19c91f19a53c56aeacb7689f4a)
- 2022 reports \[PDF\]: Messari [crypto theses](https://messari.io/pdf/messari-report-crypto-theses-for-2022.pdf) & The Block [digital asset outlook](https://www.tbstat.com/wp/uploads/2021/12/The-Block-Research-2022-Digital-Asset-Outlook.v2.pdf)
- [Ether Capital](https://twitter.com/ethcap/status/1471115850589642765?s=20) stakes 10,240 Ether

**General**

- [South Park](https://www.hollywoodreporter.com/movies/movie-features/south-park-post-covid-the-return-of-covid-movie-mocks-nfts-1235063697/) TV special mocks NFTs
- [Log4j](https://blog.cloudflare.com/protection-against-cve-2021-45046-the-additional-log4j-rce-vulnerability/) additional vulnerability
- NSO [zero-click iMessage exploit](https://googleprojectzero.blogspot.com/2021/12/a-deep-dive-into-nso-zero-click.html) deep dive: virtual computer architecture built from boolean pixel operations using image compression in PDF
- Bi-directional comms via [laser pointed at air gapped office device LEDs](https://intellisec.de/pubs/2021-acsac.pdf) \[PDF\], over 25 metres & 128 kbps throughput, requires modified firmware
- Quantum computing [overview](https://sam-jaques.appspot.com/quantum_landscape): start switching to post quantum soon in multi-decade race before RSA is broken

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-18-2021](https://weekinethereumnews.com/week-in-ethereum-news-december-18-2021)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Jan 22-23 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Jan 24-26 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford University)
- Feb 17 – [Schelling Point](https://schellingpoint.gitcoin.co/) (Denver) 
- Feb 18-20 – [ETHDenver](https://www.ethdenver.com/)
- **Mar 14-17 – [Eth Rio](https://www.ethrio.org/)**
- Mar 28-30 – [ETHDubai](https://www.ethdubai.xyz/)
- **Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)**
- **Jun 10-12 – [ETHPrague](https://ethprague.com/)**
- **Jun 24-26  – [ETHNewYork](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)** 
- **Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)**
- **Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)**
- **Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)**
- **Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)**

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

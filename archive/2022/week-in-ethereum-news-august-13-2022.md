---
title: "Week in Ethereum News <br> August 13, 2022"
date: "2022-08-13"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- Mainnet Merge targets September 15, tentative [TTD: 58750000000000000000000](https://github.com/ethereum/execution-specs/pull/585)
    - TTD to be reconfirmed on next weeks core devs call, 5GB DAG size not expected to cause big drop in hash rate
    - Bellatrix upgrade at [epoch: 144896](https://github.com/ethereum/consensus-specs/pull/2969) September 6 11:34:47am UTC
    - Bordel [predicts mainnet Merge](https://bordel.wtf/) September 15
    - Client releases expected by August 22
- Goerli testnet [merged successfully](https://twitter.com/TimBeiko/status/1557543798523146240), finalizing after some [config & client issues](https://notes.ethereum.org/@parithosh/goerli-merge)
- Somer’s Goerli testnet staking guides: [Teku](https://someresat.medium.com/guide-to-staking-on-ethereum-ubuntu-g%C3%B6erli-teku-6512b26f1372), [Lighthouse](https://someresat.medium.com/guide-to-staking-on-ethereum-ubuntu-g%C3%B6erli-lighthouse-8d0a2a811e6e), [Nimbus](https://someresat.medium.com/guide-to-staking-on-ethereum-ubuntu-goerli-nimbus-3b0e2c0c6e0e) & [Prysm](https://someresat.medium.com/guide-to-staking-on-ethereum-ubuntu-goerli-prysm-4a640794e8b5)
- [Sepolia testnet post-merge upgrade](https://twitter.com/timbeiko/status/1558170512542486528), update your nodes before August 17
- [mainnet-shadow-fork-11](https://twitter.com/abcoathup/status/1557546019339915264) merges August 18

**Execution layer**

- Erigon [v2022.08.01-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.08.01): better management of block snapshot files, fix for small memory leak in header downloading
- KZG ceremony: [design](https://hackmd.io/@6iQDuIePQjyYBqDChYw_jg/SJ-08AoT5) and [reference implementation in Python](https://github.com/crate-crypto/ceremony-specs#readme)
- [Future of light clients](https://blog.chainsafe.io/the-road-ahead-for-ethereum-light-clients-b6fdb7c3b603): browser-based light client and Portal Network ultralight client

**Proof of Stake consensus layer**

- Danny Ryan’s [Finalized PoS update](https://blog.ethereum.org/2022/08/12/finalized-no-36/): be ready for anything for the next ~5 weeks
- PoS implementers [call video](https://www.youtube.com/watch?v=CIAGQMUKEZ4&t=387s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/HkPEOKGA5) and [Christine Kim](https://docsend.com/view/dptr6wcu9zygd92k):
    - Mainnet Merge [TTD](https://notes.ethereum.org/@MarioHavel/merge-ttd) & [Bellatrix epoch](https://hackmd.io/Xq0HavcIRvufUVvA2ZjoUA) calculations, 10 days between upgrades
    - Planning weekly mainnet shadow forks
    - MEV-boost: local building should happen in parallel, circuit breaker uses rolling window to check for skipped slots
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220812)
- Prysm [v2.1.4](https://github.com/prysmaticlabs/prysm/releases/tag/v2.1.4): Merge fixes & improvements

**Layer2**

- Arbitrum [Nova](https://medium.com/offchainlabs/its-time-for-a-new-dawn-nova-is-open-to-the-public-a081df1e4ad2) (using AnyTrust) is open for the public; initial data availability committee includes Consensys, FTX, Google Cloud, Offchain Labs, P2P, Quicknode & Reddit

**EIPs/Standards**

- [EIP5299](https://github.com/ethereum/EIPs/pull/5299/files): Storage scaling pattern
- [EIP5345](https://github.com/ethereum/EIPs/pull/5345/files): Walletconnect silent-signing extension
- [EIP5437](https://github.com/ethereum/EIPs/pull/5437/files): interface for security contact

* * *

### **This newsletter is made possible thanks to** [**Nexus Mutual**](https://nexusmutual.io/)**!**

![Nexus Mutual Protocol Cover](https://weekinethereumnews.com/wp-content/uploads/2022/03/Nexus-Mutual-Protocol-Cover-1024x586.png)

The yield is still out there.  When you discover the next opportunity make sure you don’t get rekt. 

Protect yourself against: 

- hacks with Protocol Cover, 
- depegging with Yield Token Cover
- CeFi blow-ups with Custody Cover. 

Maximize yield. Minimize Risk. Enjoy peace of mind knowing Nexus Mutual has you covered. Become a member and [protect your assets](https://app.nexusmutual.io/cover) against the major risks in crypto.

* * *

**Stuff for developers**

- Solidity [v0.8.16](https://blog.soliditylang.org/2022/08/08/solidity-0.8.16-release-announcement/): fix for [head overflow bug](https://blog.soliditylang.org/2022/08/08/calldata-tuple-reencoding-head-overflow-bug/) in calldata tuple ABI-reencoding; more gas-efficient checked addition & subtraction
- Vitalik’s idea to [use stealth addresses](https://ethresear.ch/t/erc721-extension-for-zk-snarks/13237/2) to privately hold ERC721 NFTs
- Guide to [mining create2 salts](https://twitter.com/z0age/status/1556685487343034375) for efficient contract addresses
- m1guelpf’s [dapp-starter](https://github.com/m1guelpf/dapp-starter#readme): updated with light/dark theme, ConnectKit & wagmi v0.6
- Blocknative [Transaction Distribution Network](https://www.blocknative.com/blog/announcement-transaction-distribution-network): submit a transaction to multiple nodes
- MEV [bundle generator](https://github.com/Alcibiades-Capital/mev_bundle_generator#readme) (Rust) open sourced: graph based, custom Yul multicall
- Ethernaut DAO CTF [hackable contract solution](https://stermi.xyz/blog/ethernautdao-ctf-hackable-solution)

**Security**

- Yield [missing function override](https://medium.com/yield-protocol/post-mortem-of-incident-on-august-5th-2022-7bb70dbb9ada) post mortem, $206k was at risk on Arbitrum
- dYdX [free gas](https://medium.com/@hacxyk/stealing-gas-from-dydx-0-5-eth-a-day-712c5fdc43a3) vulnerability disclosed, $25k bounty paid
- OpenZeppelin Contracts [ECDSA signature malleability](https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-4h98-2769-gh6h) security advisory
- Curve finance [DNS hijack](https://twitter.com/CurveFinance/status/1557505570533478403) via DNS cache poisoning, [$612k stolen](https://www.certik.com/resources/blog/49wUGTmcApcgIxkF3PFwbE-curve-finance-hack-incident-analysis)

**Ecosystem**

- Merge community [call video](https://www.youtube.com/watch?v=AZq1acbjaz4&t=11s)
- [USDC](https://www.circle.com/blog/usdc-and-ethereums-upcoming-merge), [USDT](https://tether.to/en/usdt-supports-eth-proof-of-stake-transition/) & [Chainlink](https://docs.chain.link/docs/ethereum-proof-of-stake-merge/) announce Merge support

**Application layer**

- Reddit [Community Points](https://www.reddit.com/r/CryptoCurrency/comments/wk75p2/pack_your_moons_were_moving_to_mainnet/) migrated to Arbitrum Nova
- [SushiSwap AMM](https://twitter.com/sushiswap/status/1557061537248026624) live on Arbitrum Nova
- [Stratos](https://nova.stratosnft.io) NFT marketplace supports Arbitrum Nova
- OpenSea [stolen items policy](https://twitter.com/opensea/status/1557487545876762625) requires police report to confirm theft
- Gitcoin [Passport](https://gitcoin.co/blog/intro-to-passport): decentralized identifier aggregating web2/web3 authenticator stamps

* * *

### **Job Listings**

- Gnosis Chain looking for [Head of Bridges](https://grnh.se/9bed164e2us), [Head of Validators](https://grnh.se/e51fc7332us) & [DevRel Eng](https://grnh.se/571e88cc2us).
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- ØVIX + GOGO Protocol: [VP of Engineering](https://join.com/companies/cryptogogos/5463001-head-of-software-development-vp-engineering-at-crypto-start-up?utm_source=ETHnewsletter&utm_medium=email&utm_campaign=WeekInEthNews)

**Job listings: $600** for four issues (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US Treasury’s OFAC sanctioned Tornado Cash](https://home.treasury.gov/news/press-releases/jy0916) & associated addresses:
    - [Resources blocked](https://twitter.com/TornadoCash/status/1557048526986780677): GitHub organization & personal accounts of contributors, USDC on Tornado Cash contracts, Infura & Alchemy RPC and eth limo domain
    - Coin Center [response](https://www.coincenter.org/u-s-treasury-sanction-of-privacy-tools-places-sweeping-restrictions-on-all-americans/)
    - [Developer arrested](https://www.fiod.nl/arrest-of-suspected-developer-of-tornado-cash/) in the Netherlands
    - [Chainalysis Tornado Cash sources](https://blog.chainalysis.com/reports/tornado-cash-ofac-designation-sanctions/): 10.5% stolen funds, 17.7% sanctioned addresses
    - [0.1 ETH sent](https://twitter.com/peckshieldalert/status/1557306007935746050) to 400+ ENS addresses from Tornado Cash
- [US SEC settles with Bloom](https://www.sec.gov/litigation/admin/2022/33-11089.pdf) \[PDF\] for selling unregistered securities in ICO
- [Mailchimp](https://www.coindesk.com/business/2022/08/11/e-mail-marketing-firm-mailchimp-suspends-several-crypto-related-accounts/) suspending crypto-related accounts

**General**

- Proposal for [multi-dimensional resource pricing](https://angeris.github.io/papers/block-space.pdf) \[PDF\] in blockchains
- Nathan Schneider: [cryptoeconomics as a limitation on governance](https://mirror.xyz/ntnsndr.eth/zO27EOn9P_62jVlautpZD5hHB7ycf3Cfc2N6byz6DOk)
- [SNARK frontend & backend overheads](https://a16zcrypto.com/measuring-snark-performance-frontends-backends-and-the-future/) and future scalability
- [ÆPIC leak](https://aepicleak.com/): Intel CPU architectural bug leaking uninitialized data, requires privileged access

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-13-2022](https://weekinethereumnews.com/week-in-ethereum-news-august-13-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Aug 19-21 – [ETHMexicoCity](https://mexico.ethglobal.com/) (ETH Global)
- Aug 20-22 – [Paradigm CTF](https://ctf.paradigm.xyz/)
- **Aug 23 –** [**Devcon wave 09 + 10 tickets**](https://devcon.org/en/tickets/)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev/) (hackathon & conference)
- Sep 2-28 – [ETHOnline](https://online.ethglobal.com/') (ETH Global)
- **Sep 6 –** [**Bellatrix upgrade**](https://github.com/ethereum/consensus-specs/pull/2969) **(epoch: 144896)**
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- **Sep 7-22 –** [**Gitcoin Grants round 15**](https://twitter.com/gitcoin/status/1554857322572382208)
- **Sep 9 –** [**Merge Community Call #7**](https://github.com/ethereum/pm/issues/599)
- Sep 9-11 – [Ethereum SP](https://www.ethereumbrasil.com/#next) (São Paulo)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- **Sep ~15 –** [**the Merge**](https://github.com/ethereum/execution-specs/pull/585) **(tentative TTD: 58750000000000000000000)**
- Sep 16-18 - [EthBerlin](https://ethberlin.ooo/)
- Sep 23 - [ETH HCMC](https://2022.ethhcmc.com/) summit (Ho Chi Minh)
- Sep 23-24 - [ETHSantiago](https://ethsantiago.com/)
- Oct 7-16 – [Devcon week](https://devcon.org/en/devcon-week/) (Bogotá)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- Oct 7-9 – [Infinite hackathon](https://infinite-hackathons.eth.limo/) (Bogotá)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- **Mar 2-5 –** [**ETHDenver**](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

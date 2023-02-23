---
title: "Week in Ethereum News <br> November 19, 2022"
date: "2022-11-19"
---

## **Eth News and Links**

**Layer 1**

- [EIP4844 (proto-danksharding)](https://github.com/ethereum/pm/blob/master/Breakout-Room/4844-readiness-checklist.md) readiness checklist
- [EVM Object Format (EOF)](https://twitter.com/lightclients/status/1593270266909450241) EIPs explainer
- Latest consensus layer [call video](https://www.youtube.com/watch?v=IK1jNCQz5yk&t=120s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/rJBcqhXIo) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-consensus-layer-call-98/):
    - [MEV-Boost update](https://hackmd.io/kJQguDvTRXGY4qK0z_j1gA): Flashbots no longer [top builder](https://www.relayscan.io/)  
    - Withdrawals: discussion on setting a bound to avoid sweeping the entire validator set
    - EIP4844 blobs to be verified, will check on testnets
    - Proposal to add getCapabilities to Engine API and improve spec structure
- Consensus specs [v1.3.0-alpha.1](https://github.com/ethereum/consensus-specs/releases/tag/v1.3.0-alpha.1): Capella & EIP4844 improvements ready for R&D testnets
- Flashbots [block builder open sourced](https://writings.flashbots.net/open-sourcing-the-flashbots-builder/)
- MEV-Boost relay [v0.14.0](https://github.com/flashbots/mev-boost-relay/releases/tag/v0.14.0): fix for DoS vulnerability
- Etherscan [MEV Info per block](https://twitter.com/etherscan/status/1593204861969264640): proposer fee recipient & MEV reward, beta
- [ERA files](https://mainnet.era.nimbus.team/) (flat storage format of block & consensus data) for entire beacon chain history

**For stakers**

- [Validator rewards](https://mirror.xyz/ratedw3b.eth/b4Pw-ppAxhetrcl1nsCpHB3z8a5vMl161lUPvnWJzPs): fees & MEV post-Merge increased rewards by ~40% and priority fees up 8% despite transaction volume down

**Research**

- [Horn](https://ethresear.ch/t/horn-collecting-signatures-for-faster-finality/14219): proposal for two-layer BLS signature aggregation, enabling a million validators to vote on the same slot. Would increase slot time by 10 seconds and validator requirements, [impacting home stakers](https://twitter.com/technocrypto/status/1593258719105662976)

**Client releases**

- Consensus Layer:
    - Teku [v22.11.0](https://github.com/ConsenSys/teku/releases/tag/22.11.0): proposer config breaking change, fixes potential DoS vector

**Layer 2**

- [Arbitrum One](https://offchain.medium.com/arbitrum-decentralization-update-39f093768c42) now has 9 validators
- Proposal for [type-theoretic dispute protocols](https://ethresear.ch/t/type-theoretic-dispute-protocols/14213)

**EIPs/Standards**

- [EIP5920](https://github.com/ethereum/EIPs/pull/5920/files): PAY opcode
- [EIP5976](https://github.com/ethereum/EIPs/pull/5976/files): EIP author handbook
- [EIP5982](https://github.com/ethereum/EIPs/pull/5982/files): Role-based access control
- [EIP5987](https://github.com/ethereum/EIPs/pull/5987/files): Permissionless transfer with authorization
- [EIP5988](https://github.com/ethereum/EIPs/pull/5988/files): Add Poseidon hash function precompile
- [EIP5994](https://github.com/ethereum/EIPs/pull/6000/files): Token Pods extensions (ERC20/ERC721)

* * *

### **This newsletter is made possible thanks to** [**Mimic**](https://mimic.fi/)**!**

![mimic](https://weekinethereumnews.com/wp-content/uploads/2022/10/mimic-banner-1024x427.png)

Does your DAO want to **delegate treasury management but keep custody?** Or **trustlessly automate your yield?**

Check out our [Smart Vaults](https://medium.com/mimicfi/introducing-smart-vaults-3438bacc843d) to automate DeFi operations in a secure, trustless, and non-custodial way.

**For DeFi projects**: you can also automate collecting your fees across chains and swapping/distributing them.

Previously Mimic’s co-founders helped build POAP, Balancer, and OpenZeppelin, among others.  _Backed by Starbloom Ventures._

* * *

**Stuff for developers**

- [Solplot](https://github.com/0xClandestine/solplot#readme): Foundry plugin to plot charts in Solidity
- Prettier Solidity [v1.0.0](https://github.com/prettier-solidity/prettier-plugin-solidity/releases/tag/v1.0.0) (Prettier plugin for formatting Solidity): first stable version
- Uniswap [Permit2 & Universal Router](https://uniswap.org/blog/permit2-and-universal-router) contracts deployed on mainnet, Optimism & Arbitrum: 
    - Permit2: permits for any ERC20 token, expiring approvals, signature-based transfers and batch approvals, transfers & revoking allowances
    - Universal Router: ERC20 & NFT in a single swap router
- [Anonymous Vickrey auction](https://blog.aayushg.com/posts/vickrey/): bids sent to uninitialized CREATE2 addresses, proof of concept
- Paul Berg: [time variables as uint40](https://twitter.com/PaulRBerg/status/1591832937179250693) (~35k years into the future) instead of uint256 to save gas
- [SSX](https://blog.spruceid.com/announcing-ssx/) (Self-Sovereign Anything): library to integrate Sign-In with Ethereum (SIWE) for user authentication, session management & user metrics
- [create-wagmi CLI](https://wagmi.sh/docs/create-wagmi): project starter with templates for Next.js, RainbowKit, ConnectKit and Vite
- Guide to [BigQuery custom event data extraction](https://mirror.xyz/nick.eth/KVal7tob7sqZSss27rrFlIpu6i91TJYJJvBzf53kwhQ), query events not in default public datasets
- [react-native-helios](https://github.com/cawfree/react-native-helios#readme): React Native wrapper to embed a16z’s Helios light client in mobile apps
- [miniSTARK](https://github.com/andrewmilson/ministark#readme): GPU accelerated STARK prover
- [Nova Scotia](https://github.com/nalinbhardwaj/Nova-Scotia#readme): middleware for using Circom circuits with Microsoft’s Nova prover

**Security**

- Zellic’s [audit coverage tracker](https://www.zellic.io/blog/audit-drift): audit coverage by contract for selected DeFi protocols, with diff between on-chain vs audited code
- [evm-dafny](https://github.com/ConsenSys/evm-dafny#readme): functional spec of EVM in Dafny, allows formal verification of contract bytecode

**Ecosystem**

- [Use ethstats.dev](https://twitter.com/evan_van_ness/status/1593362389407338497) as ethstats.net domain has expired

**Application layer**

- [Maker Teleport](https://twitter.com/MakerDAO/status/1592537340131430400): fast DAI withdrawals from Arbitrum/Optimism to mainnet
- [ENS Redirect](https://twitter.com/ensredirect/status/1592842841633755136): redirect ENS to any website
- [Custom GitPOAPs](https://medium.com/gitpoap/introducing-custom-gitpoaps-64bbe4204511): award via GitHub user, ENS, Ethereum address or email
- [MobyMask](https://metamask.io/news/security/meta-mask-and-laconic-launch-moby-mask-light-client/): read on-chain phishing reports using a light client
- [Punks legacy project](https://www.businesswire.com/news/home/20221115005630/en/Yuga-Labs-Kicks-Off-First-of-Its-Kind-NFT-Museum-Donation-Initiative-Gifts-CryptoPunk-to-the-Institute-of-Contemporary-Art-Miami) donating Punks to museums, #305 donated to ICA Miami

* * *

### Job Listings

- Avantgarde Finance seeking [Full Stack Dev in Web3/DeFi](https://apply.workable.com/avantgarde-finance/j/3974DA97B8/) to build on Enzyme
- Ethereum Foundation are hiring a [code integration tester](https://jobs.lever.co/ethereumfoundation/6feeb8cb-bd05-4f24-9fda-9ba3be98e5a4)
- [Project Manager](https://jobs.lever.co/ethereumfoundation/d58c7609-667c-4aee-a2c8-e3d91b3c5554) wanted by EF for organizational & team support
- EF Robust Incentives Group seek a [research scientist](https://jobs.lever.co/ethereumfoundation/cd2382ec-abbd-493b-b942-b5e2a61a6c0a)

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- FTX:  
    - Bankruptcy specialist declares [FTX/Alameda to be the worst case of corporate malfeasance](https://s3.documentcloud.org/documents/23310507/ftx-bankruptcy-filing-john-j-ray-iii.pdf) in his career, “complete failure of corporate controls and such a complete absence of trustworthy financial information.”
    - Bahamas Securities Commission [didn’t order reopening of withdrawals for local customers](https://www.scb.gov.bs/wp-content/uploads/2022/11/Securities-Commission-on-FTX-Bahamian-Withdrawals-111222.pdf) \[PDF\], [assumes control of FTX assets](https://www.scb.gov.bs/wp-content/uploads/2022/11/Media-Release-SCB-Assumes-Control-of-Assets-of-FTX-Digital-Markets-Ltd.pdf) \[PDF\]
    - [Unauthorized access](https://www.coindesk.com/business/2022/11/14/ftx-hacker-panicked-still-holds-339m-in-ether-cryptos-arkham-intelligence/) of $300 million assets
- Reminder when looking at proof of reserves: [Crypto.com sent 320k ETH](https://twitter.com/kris/status/1591605600638881792) to Gate exchange in error
- [Privacy-protecting regulatory solutions](https://a16zcrypto.com/privacy-protecting-regulatory-solutions-using-zero-knowledge-proofs-full-paper/) using zk proofs

**General**

- [Secret phrase backups](https://medium.com/@cozyfinance/how-safe-is-your-seed-phrase-5-question-quiz-9260aee39ba9): can it survive a hacker, natural disaster, bad memory, spring cleaning or [your unexpected death](https://twitter.com/brucefenton/status/1593069948523646978)
- [PiEthereumWallet](https://github.com/snarflakes/PiEthereumWallet#readme): build a hardware wallet using a Raspberry Pi
- [Tokensoft doxxed 5k users](https://twitter.com/cryptogle/status/1591542182346997767) as bad actors in [accidental leak](https://twitter.com/TokensoftInc/status/1592034770376339458)
- [RSA verification circuit](https://mirror.xyz/privacy-scaling-explorations.eth/mmkG4uB2PR_peGucULAa7zHag-jz1Y5biZH8W6K2LYM) using halo2 library

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-november-19-2022](https://weekinethereumnews.com/week-in-ethereum-news-november-19-2022)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Nov 20 – Clr.fund [LatAm round](https://ethcolombia.clr.fund/) ends
- Nov 25-26 – [ETH Vietnam](https://www.eth-vietnam.com/)
- Dec 1 – [Columbia cryptoeconomics workshop](https://bit.ly/columbiacryptoeconomics) (New York)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- Dec 5 – [EF Layer 2 grants](https://esp.ethereum.foundation/layer-2-grants) deadline
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

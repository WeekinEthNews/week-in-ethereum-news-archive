---
title: "Week in Ethereum News <br> October 22, 2022"
date: "2022-10-22"
---

## **Eth News and Links**

**Layer 1**

- [Visualization of Tornado Cash transactions](https://tornado-warning.info/) & MEV-Boost relays; guide to [analyzing MEV-Boost](https://medium.com/@toni_w/practical-guide-into-analyzing-mev-in-the-proof-of-stake-era-e2b024509918)
- Ideas for [next MEV-Boost features](https://twitter.com/metachris/status/1581975949817495552)
- EIP4844 proto-danksharding [progress update](https://twitter.com/jessepollak/status/1582784133121859585): targeting Shanghai upgrade, network bandwidth testing will determine target blob sizes
- History of [account abstraction](https://hackmd.io/@matt/r1neQ_B38)

**Research**

- Vitalik updated [paths to single slot finality](https://notes.ethereum.org/@vbuterin/single_slot_finality)

**Client releases**

- Execution layer:
    - Besu [v22.7.7](https://github.com/hyperledger/besu/releases/tag/22.7.7): memory & CPU performance improvements, reduces exceptions, fix for GraphQL and patches Apache Commons Text CVE
    - Erigon [v2.28.1](https://github.com/ledgerwatch/erigon/releases/tag/v2.28.1): fixes for empty proposed blocks and fix for potential deadlock
- Consensus layer:
    - Lodestar [v1.1.1](https://github.com/ChainSafe/lodestar/releases/tag/v1.1.1): sync committee improvements

**Layer 2**

- Polynya: [protocols take time to mature](https://twitter.com/apolynya/status/1582584083044962304), predicts 2024 at the earliest for a secure decentralized rollup

**EIPs/Standards**

- [EIP5787](https://github.com/ethereum/EIPs/pull/5787/files): Digital identity 
- [EIP5791](https://github.com/ethereum/EIPs/pull/5791/files): Physical Backed Tokens; Azuki [PBT explainer](https://www.azuki.com/updates/pbt)
- [EIP5792](https://github.com/ethereum/EIPs/pull/5792/files): Wallet abstract transaction send API
- [EIP5793](https://github.com/ethereum/EIPs/pull/5793/files): eth/68: add tx type to tx announcement
- [EIP5794](https://github.com/ethereum/EIPs/pull/5794/files): eth/69: add withdrawals to block
- [EIP5805](https://github.com/ethereum/EIPs/pull/5805/files): Voting with delegation
- [EIP5806](https://eips.ethereum.org/EIPS/eip-5806): Delegate transaction

* * *

### **This newsletter is made possible thanks to [Mimic](https://mimic.fi/)!**

![mimic](https://weekinethereumnews.com/wp-content/uploads/2022/10/mimic-banner-1024x427.png)

Does your DAO want to **delegate treasury management but keep custody?** Or **trustlessly automate your yield?**

Check out our [Smart Vaults](https://medium.com/mimicfi/introducing-smart-vaults-3438bacc843d) to automate DeFi operations in a secure, trustless, and non-custodial way.

**For DeFi projects**: you can also automate collecting your fees across chains and swapping/distributing them.

Previously Mimic’s co-founders helped build POAP, Balancer, and OpenZeppelin, among others.  _Backed by Starbloom Ventures._

* * *

**Stuff for developers**

- [Open Etherscan verified contract in Remix](https://twitter.com/james_bachini/status/1583041998289633280) by replacing domain in URL
- tincho: [solutions to yet another EVM puzzle](https://www.notonlyowner.com/writeups/yet-another-evm-puzzle/)
- [Cookbook](https://www.cookbook.dev/): discoverable contracts with no-code deploy
- [subway-rs](https://github.com/abigger87/subway-rs#readme): sandwich bot for Uniswap v2, implemented in Rust & Huff
- [Fast G2 subgroup check](https://ethresear.ch/t/fast-mathbb-g-2-subgroup-check-in-bn254/13974) in BN254
- [zk-timelock](https://github.com/timoth-y/zk-timelock#readme): verifiable time-lock encryption using zk proofs, experimental with benchmarks

**Security**

- Bond Protocol’s Ohm bond [$292k exploit](https://twitter.com/peckshield/status/1583416829237526528), no input validation, funds returned
- Timeless Bunni [vulnerability fixed](https://twitter.com/Timeless_Fi/status/1581121279934885888), initial deposits would have been at risk
- DXdao governance [vulnerability disclosed](https://dave.xn--tckwe/posts/exploit/), $80 million could be withdrawn
- Immunefi’s [web3 security resources](https://github.com/immunefi-team/Web3-Security-Library#readme)

**Ecosystem**

- [Open Ethereum problems](https://efdn.notion.site/ROPs-RIG-Open-Problems-c11382c213f949a4b89927ef4e962adf) in game theory, mechanism design and economic modeling
- First month of [negative ETH issuance](https://twitter.com/evan_van_ness/status/1583151914447167488)

**Application layer**

- Lattice [OPCraft](https://dev.optimism.io/opcraft-autonomous-world/): on-chain 3D voxel world built with MUD game engine on Optimism’s OP Stack
- [Sorare NBA](https://twitter.com/SorareNBA/status/1582378206090231809) five player fantasy game live, beta
- [ENS POAP card](https://ens.mirror.xyz/eiy6qiOHuiUl90XasUAsu2iajhb72TTYh2xJIz31xEQ): Devcon swag issued “I met” POAP claim codes via NFC
- [NFT screens](https://avc.com/2022/10/nft-screens/): display NFTs curated via Google Sheets
- Unstoppable domains [stopping .coin support](https://unstoppabledomains.com/blog/coin), offering credits

* * *

### **Job Listings**

- [Join Llama](https://zenith-caboc-8a4.notion.site/Join-Llama-ad66be1cb28541f5b5346aa37d192b79) to help build the future of protocol DAOs: [Solidity](https://zenith-caboc-8a4.notion.site/Smart-Contract-Engineer-ef9426f7cfef4f0d90b596aaeff216e0) and [Backend](https://zenith-caboc-8a4.notion.site/Senior-Backend-Engineer-6a096e7937c248f4a90fba08c3bf14ae)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)
- [Research scientist](https://jobs.lever.co/ethereumfoundation/cd2382ec-abbd-493b-b942-b5e2a61a6c0a) wanted for EF Robust Incentives Group

**Job listings: $600** for four issues (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Draft DCCPA bill](https://twitter.com/alliancedao/status/1582800340520312833) aims to kill DeFi in US; bill lobbied for by FTX/SBF
- beeple: [switch NFT royalties from a sellers fee to a buyer’s premium](https://twitter.com/beeple/status/1581351398259597312)
- Idea to [use NFTs for positive-sum predictions](https://jacob.energy/predicting-provenance.html)

**General**

- Paul Brody: [Ethereum killers are now all zombies](https://www.coindesk.com/layer2/2022/10/19/the-ethereum-killers-are-all-zombies-now/)
- Forbes: [ByteDance planned to monitor the location](https://www.forbes.com/sites/emilybaker-white/2022/10/20/tiktok-bytedance-surveillance-american-user-data/) of specific US TikTok users
- [HyperPlonk](https://eprint.iacr.org/2022/1355) with linear time prover: moves Plonk to the boolean hypercube, removes need for using FFTs and eases parallelization

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-october-22-2022](https://weekinethereumnews.com/week-in-ethereum-news-october-22-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in **bold**)_

- Oct 26-28 – [Eth Panama](https://www.ethpanama.com/)
- **Oct 28 – [Semaphore grants](https://esp.ethereum.foundation/semaphore-grants) deadline**
- Oct 28-30 – [ETH Lisbon](https://www.ethlisbon.org/)
- Oct 31 – [Merge data challenge](https://esp.ethereum.foundation/merge-data-challenge) deadline
- Oct 31-Nov 10 – Clr.fund [LatAm round](https://ethcolombia.clr.fund/)
- Nov 3 – US Treasury [digital assets RFC](https://public-inspection.federalregister.gov/2022-20279.pdf) \[PDF\] deadline
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 11-13 – [ETHBrno](https://ethbrno.cz/) (Czech Republic)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Nov 25-27 – [ETH Vietnam](https://www.eth-vietnam.com/)
- Dec 1 – [Columbia cryptoeconomics workshop](https://bit.ly/columbiacryptoeconomics) (New York)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

_[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive this newsletter weekly**_

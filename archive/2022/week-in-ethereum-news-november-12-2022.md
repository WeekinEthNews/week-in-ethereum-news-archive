---
title: "Week in Ethereum News <br> November 12, 2022"
date: "2022-11-12"
---

## Eth News and Links

**Layer 1**

- Latest core devs [call video](https://www.youtube.com/watch?v=ZZx7d14vE10&t=185s). Notes from [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-call-149/):
    - Shanghai upgrade planning, EIPs jostling to potentially be included along with withdrawals: EOF, EIP4844 (proto-danksharding), EIP4758 (deactivate SELFDESTRUCT), EIP1153 (transient storage) & EIP2537 (BLS12 precompile)
    - Next call to focus on triage of Shanghai upgrade EIPs
    - [Users of SELFDESTRUCT need to shout](https://ethereum-magicians.org/t/eip-4758-deactivate-selfdestruct/8710) as the plan is to deactivate
    - Discussion on censorship resistance vs scaling and improving node UX
- [Helios](https://a16zcrypto.com/building-helios-ethereum-light-client/): light client implemented in Rust, syncs in seconds, experimental
- Withdrawal interop instructions for [Prysm+Geth](https://hackmd.io/-7X3aN3KRvOcY2TsDbFcvQ) and [Prysm+Nethermind](https://hackmd.io/3ajXKu7_Tqm3uBRyxH8KfA?view)
- [EIP4844](https://dev.optimism.io/eip-4844-an-optimistic-bet-on-rollup-scalability/) (blobspace/proto-danksharding) history & push to include in Shanghai upgrade, targeting testnet for end of November; [explainer for builders](https://twitter.com/ralexstokes/status/1591190407777775616)

**For stakers**

- MEV-Boost:
    - [v1.4.0](https://github.com/flashbots/mev-boost/releases/tag/v1.4.0): set minimum bid to accept blocks from relays otherwise build blocks locally
    - [DoS vulnerability patched](https://collective.flashbots.net/t/post-mortem-for-a-relay-vulnerability-leading-to-proposers-falling-back-to-local-block-production-nov-10-2022/727), would have prevented MEV-Boost blocks and forced proposers to fallback to local block production

**Research**

- Barnabé: [state of Proposer-Builder Separation (PBS) research](https://barnabe.substack.com/p/pbs)
- [Reorg resilience & security](https://ethresear.ch/t/reorg-resilience-and-security-in-post-ssf-lmd-ghost/14164) in post-single slot finality LMD-GHOST
- Efficient [BLS multi-signature verification](https://geometry.xyz/notebook/Optimized-BLS-multisignatures-on-EVM) on EVM

**Client releases**

- Execution Layer:
    - Erigon [v2.30.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.30.0): embedded CL light client now the default and new RPC methods: erigon\_cacheCheck & erigon\_getLatestLogs
- Consensus Layer:
    - Lodestar [v1.2.1](https://github.com/ChainSafe/lodestar/releases/tag/v1.2.1): fix to ignore old attestations; [v1.2.0](https://blog.chainsafe.io/lodestar-releases-v1-2-0-e34664a774fd): upgraded libp2p, improved UX and updated agent version

**Layer 2**

- Polynya: [minimum viable rollup decentralization](https://polynya.mirror.xyz/0hmnwXCiainU7HMYes73uH_kjQABRwk6b1WrqgQPAMg) (stage 1: limited training wheels)

**EIPs/Standards**

- Guide to [creating an EIP](https://medium.com/ethereum-magicians/comprehensive-guide-on-writing-and-submitting-an-eip-9474163771f0)
- [EIP5883](https://github.com/ethereum/EIPs/pull/5883/files): Token transfer by social recovery
- [EIP5896](https://github.com/ethereum/EIPs/pull/5896/files): Rejectable NFT
- [EIP5902](https://github.com/ethereum/EIPs/pull/5902/files): Contract event hooks

* * *

### **This newsletter is made possible thanks to** [**SpeedRunEthereum**](https://speedrunethereum.com/)**!**

![Speed Run Ethereum](https://weekinethereumnews.com/wp-content/uploads/2022/10/Speed-Run-Ethereum-banner.png)

Test your skills and learn how to build apps on Ethereum at [SpeedRunEthereum.com](https://speedrunethereum.com/).

* * *

**Stuff for developers**

- OpenZeppelin Contracts [v4.8](https://blog.openzeppelin.com/announcing-openzeppelin-contracts-4-8/): gas efficient batch ERC721 minting, voting gas optimization, two step ownership transfer, log2/10/256, admin for TimelockController and ERC4626 calculations updated to not use decimals
- OpenZeppelin [Contracts Wizard](https://twitter.com/OpenZeppelin/status/1590865466993836033) adds download development package for Hardhat 
- Remix [v0.28](https://medium.com/remix-ide/remix-ide-v0-28-0-release-8786146f6603): manage Git branches in the File Explorer & updated home tab
- Foundry [format and gas snapshot pre-commit hook](https://twitter.com/devanoneth/status/1590922732988157952)
- [Whitenoise CTF 2](https://twitter.com/vex_0x/status/1590748480796262402) using EIP1153 (transient storage)
- RareSkills gas puzzle solutions: [Sqrt](https://twitter.com/orenyomtov/status/1589766317585797120), [ERC165](https://twitter.com/w1nt3r_eth/status/1588942261730963456)
- Norswap: [how to shuffle cards on-chain](https://twitter.com/norswap/status/1590489878726205440) using hashes, Merkle trees & simple zk-proofs
- ConnectKit [v1.0.0](https://family.co/changelog/2022-11-07) (React components to connect wallets): adds Sign in With Ethereum support, avatar component and Nouns theme
- [Zk-starter](https://github.com/cawfree/zk-starter#readme): create arithmetic circuit with corresponding Solidity contract, uses circom & Foundry

**Security**

- DFX Finance [$4 million exploit](https://www.certik.com/resources/blog/27ZZE58zgmjoOnIbygqfJL-dfx-finance), reentrancy of flash loan mechanism

**Ecosystem**

- The [total supply of ETH has decreased](https://www.coindesk.com/markets/2022/11/11/ether-turns-deflationary-as-amount-of-eth-burned-spikes-amid-ftx-induced-market-volatility/) since the Merge
- ETHSanFrancisco hackathon [winners](https://twitter.com/ethglobal/status/1589431653599961089) & [list of projects](https://ethglobal.com/showcase?events=ethsanfrancisco2022)

**Application layer**

- OpenSea [enforcing NFT royalties](https://opensea.io/blog/announcements/on-creator-fees/) for new collections only if they implement a block list, still enforcing royalties for existing collections
- [MagicMirror](https://mirror.xyz/0x57D1eAE9f0972723F0e78EAF4e6C08e90565206F/nx5I7DO1TmePG4w6IaEjqa-DmD4evQeRGL7CWHowO5c): mirror single NFT from Optimism to mainnet for use as Twitter PFPs
- [ENS merch](https://ensmerchshop.xyz/): baseball cap embroidered with ENS name

* * *

### Job Listings

- EF Robust Incentives Group seek a [research scientist](https://jobs.lever.co/ethereumfoundation/cd2382ec-abbd-493b-b942-b5e2a61a6c0a)
- Avantgarde Finance seeking [Full Stack Dev in Web3/DeFi](https://apply.workable.com/avantgarde-finance/j/3974DA97B8/) to build on Enzyme
- [Project Manager](https://jobs.lever.co/ethereumfoundation/d58c7609-667c-4aee-a2c8-e3d91b3c5554) wanted by EF for organizational & team support
- EF are hiring a [code integration tester](https://jobs.lever.co/ethereumfoundation/6feeb8cb-bd05-4f24-9fda-9ba3be98e5a4)

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- FTX blows up:
    - Rekt gives the [play-by-play on the FTX/Alameda implosion](https://rekt.news/ftx-yikes/)
    - Bahamas Securities Commission [freezes FTX assets](https://www.scb.gov.bs/wp-content/uploads/2022/11/Securities-Commission-Statement-on-FTX-101122-Final.pdf) \[PDF\]
    - [filed for bankruptcy](https://twitter.com/z0r0zzz/status/1591100510161227776) & SBF resigns
    - [BlockFi](https://twitter.com/BlockFi/status/1590875997351866368) pauses withdrawals
- [OFAC](https://home.treasury.gov/news/press-releases/jy1087) recategorized Tornado Cash as banned and adds [testnet contracts](https://twitter.com/wadealexc/status/1590800683846217729) to banned list
- SEC wins [summary judgment against LBRY](https://www.sec.gov/litigation/litreleases/2022/lr25573.htm) for not registering their token sale as a security offering
- [US seek to seize 50k BTC](https://www.justice.gov/usao-sdny/pr/us-attorney-announces-historic-336-billion-cryptocurrency-seizure-and-conviction) hacked from Silk Road in 2012
- [Auctioning off the reward paid to token holders for voting](https://a16zcrypto.com/paying-people-to-participate-in-governance/) can increase robustness against governance attacks

**General**

- Taylor Monahan: [get your assets off exchanges and onto your own keys](https://twitter.com/tayvano_/status/1590924743192227840)
- David Mihal’s [CryptoFlows](https://cryptoflows.info/): visualization of flow of value between chains
- [Checking univariate identities](https://hackmd.io/@arielg/ryGTQXWri) in linear time
- [Baloo](https://eprint.iacr.org/2022/1565): protocol for lookup tables, linear on the amount of lookups & independent of table size

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-november-12-2022](https://weekinethereumnews.com/week-in-ethereum-news-november-12-2022)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- **Nov 18 – 0xPARC** [**PARC Squad application**](https://twitter.com/0xPARC/status/1588613959523135488) **deadline**
- **Nov 20 – Clr.fund** [**LatAm round**](https://ethcolombia.clr.fund/) ends
- Nov 25-27 – [ETH Vietnam](https://www.eth-vietnam.com/)
- Dec 1 – [Columbia cryptoeconomics workshop](https://bit.ly/columbiacryptoeconomics) (New York)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- Dec 5 – [EF Layer 2 grants](https://esp.ethereum.foundation/layer-2-grants) deadline
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

---
title: "Week in Ethereum News <br> November 26, 2022"
date: "2022-11-26"
---

## **Eth News and Links**

**Layer 1**

- Latest core devs [call video](https://www.youtube.com/watch?v=HX_Zr_gVeOE&t=92s). Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1595860968298672128):
    - March 2023 semi-aggressive goal for next fork (“Shanghai”) with staking withdrawals (EIP4895) along with EIP3651 (warm COINBASE), EIP3855 (PUSH0) & EIP3860 (limit & meter initcode)
    - Possible additional EIPs for Shanghai to be finalized at next core devs call; impact of adding EIP4844 on withdrawal timeline to be discussed at next week's consensus layer call
    - [Candidates for inclusion](https://github.com/ethereum/execution-specs/pull/656/files) (CFI) in Shanghai or future upgrades: EIP4844 (proto-danksharding), EOF (3540, 3670, 4200, 4750, 5450), EIP1153 (transient storage) & EIP2537 (BLS precompile)
    - EIP4758 (deactivate SELFDESTRUCT) to explore edge cases before being CFI’d
    - [Withdrawal multiclient devnet](https://twitter.com/vdWijden/status/1595386746786779137) launched
    - Proposals for testnet lifecycle with regular shut downs & [validator ephemeral testnet](https://github.com/taxmeifyoucan/ephemeral-testnet); Ropsten testnet shutting down by the end of year
- [EIP4844 devnet 3](https://notes.ethereum.org/@timbeiko/4844-devnet-3) milestone tracker
- [Stress4844](https://github.com/gakonst/stress4844#readme): CLI for submitting large calldata transactions to test networking for EIP4844
- Paradigm building [Reth](https://twitter.com/gakonst/status/1595648232226291712) execution layer client in Rust

**For stakers**

- [Validators can set a minimum bid](https://writings.flashbots.net/the-cost-of-resilience/) before using MEV-Boost, setting a [minimum bid of 0.05 ETH](https://twitter.com/vitalikbuterin/status/1595793106926014466) would produce almost half the blocks locally, increasing censorship resistance
- [Somer’s Geth guides updated](https://github.com/SomerEsat/ethereum-staking-guides/issues/6), adds a TimeoutStopSec to Geth service config to prevent corruption of state database on shutdown

**Research**

- [MinRoot](https://eprint.iacr.org/2022/1626): candidate sequential function for a VDF

**Client releases**

- Consensus Layer:
    - Lighthouse [v3.3.0](https://github.com/sigp/lighthouse/releases/tag/v3.3.0): deposit snapshot sync

**EIPs/Standards**

- [EIP6036](https://github.com/ethereum/EIPs/pull/6036/files): Subscribable NFT extension

* * *

### **This newsletter is made possible thanks to** [**Hardhat**](https://hardhat.org/)**!**

![](https://weekinethereumnews.com/wp-content/uploads/2021/06/hardhat-rectangle-1024x325.png)

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
- Constrain mutability by adding view/pure to function signature
- Meet inheritance requirements by adding virtual/override on function signature
- Provide accessibility by adding public/private to function signature

Get it from the [VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=NomicFoundation.hardhat-solidity)

* * *

**Stuff for developers**

- Hardhat for VS Code [v0.6.0](https://github.com/NomicFoundation/hardhat-vscode/releases/tag/v0.6.0): experimental support for Foundry & hybrid projects
- Proof’s [Solidify](https://github.com/proofxyz/solidify#readme): golang + Solidity library to store arbitrary data on-chain
- [RolodETH](https://github.com/verynifty/RolodETH#readme): address database with names & tags
- [Dnum](https://github.com/bpierre/dnum#readme): TypeScript library for big decimal numbers
- [Guide to building a DAO authentication app](https://blog.developerdao.com/getting-started-with-ssx) with React + Express + SSX
- [OPCraft](https://twitter.com/latticexyz/status/1595192315785744384): making of an on-chain voxel world
- Norswap: [mental poker](https://twitter.com/norswap/status/1594748863574732800) using zk proofs for shuffling & encryption
- Echidna [v2.0.4](https://github.com/crytic/echidna/releases/tag/v2.0.4) (contract fuzzer): adds coverage report in HTML
- Guide to [constructing ZK SNARK circuits](https://jtriley.substack.com/p/constructing-zk-snark-circuits) using the halo2 Rust crate

**Security**

- [Formally verifying WETH contract](https://www.zellic.io/blog/formal-verification-weth), checking invariants using SMT solver Z3

**Ecosystem**

- [Annotated Ethereum roadmap](https://notes.ethereum.org/@domothy/roadmap), summary of each item with links to deeper dives
- Flashbots shares plans for [SUAVE](https://writings.flashbots.net/the-future-of-mev-is-suave/) (Single Unified Auction for Value Expression), a mempool & decentralized block builder for mainnet & layer 2, using custom blockchain & SGX
- [MetaMask & Infura privacy hasn’t changed](https://twitter.com/danfinlay/status/1595848457520308224?s=20&t=4Rw-D_0WI2ruSj29uunVbA), user IP & wallet address is collected by Infura (default RPC for MetaMask)

**Enterprise**

- [UNICEF pilot QF round](https://go.gitcoin.co/blog/gitcoin-unicef-qf-collaboration-pilot) on Gitcoin’s new grants protocol

**Application layer**

- [Maker](https://twitter.com/makerdao/status/1594700128920682503) adds Rocket Pool staked ETH as collateral
- Curve published [stablecoin](https://github.com/curvefi/curve-stablecoin/blob/master/doc/curve-stablecoin.pdf) whitepaper \[PDF\]
- Aave [discussion on reducing long tail asset risk](https://governance.aave.com/t/discussion-reducing-long-tail-asset-risk/10748) after [$1.5 million of CRV bad debt](https://twitter.com/RudyKadoch/status/1595210314685071363)
- [Moonbirds](https://twitter.com/moonbirds/status/1595151996545159168) NFTs now on-chain as bitmaps
- Native Layer 2 NFT marketplaces [Quix (Optimism) & Stratos (Arbitrum) winding down](https://quixotic-labs.notion.site/quixotic-labs/A-Message-from-Quix-83fc2818b5b34b0eb042344535472415), code to be open sourced

* * *

### Job Listings

- Avantgarde Finance seeking [Full Stack Dev in Web3/DeFi](https://apply.workable.com/avantgarde-finance/j/3974DA97B8/) to build on Enzyme
- [Code integration tester](https://jobs.lever.co/ethereumfoundation/6feeb8cb-bd05-4f24-9fda-9ba3be98e5a4) wanted by Ethereum Foundation
- EF Robust Incentives Group seek a [research scientist](https://jobs.lever.co/ethereumfoundation/cd2382ec-abbd-493b-b942-b5e2a61a6c0a)

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Alexey Pertsev (Tornado Cash developer) to remain in jail](https://twitter.com/provoost/status/1595063229230813186) until at least late February
- [New York state](https://gizmodo.com/new-york-crypto-crypto-mining-1849816697) prohibits PoW mining permits for 2 years
- [Analysis of Uniswap airdrop](https://dune.com/blog/uni-airdrop-analysis), only 7% of addresses still hold UNI

**General**

- Vitalik: [make custodial exchanges better](https://vitalik.ca/general/2022/11/19/proof_of_solvency.html) using proof of solvency & validiums
- Facebook collected [user financial info from US income tax prep services](https://www.theverge.com/2022/11/22/23471842/facebook-hr-block-taxact-taxslayer-info-sharing)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-november-26-2022](https://weekinethereumnews.com/week-in-ethereum-news-november-26-2022)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Dec 1 – [Columbia cryptoeconomics workshop](https://bit.ly/columbiacryptoeconomics) (New York)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- Dec 5 – [EF Layer 2 grants](https://esp.ethereum.foundation/layer-2-grants) deadline
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

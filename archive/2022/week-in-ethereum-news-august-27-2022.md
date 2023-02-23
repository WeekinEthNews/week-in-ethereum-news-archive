---
title: "Week in Ethereum News <br> August 27, 2022"
date: "2022-08-27"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- Merge-ready execution client releases, update your [nodes](https://ethernodes.org/merge):
    - Besu [v22.7.1](https://github.com/hyperledger/besu/releases/tag/22.7.1)
    - Erigon [v2022.08.02-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.08.02)
    - Geth [v1.10.23](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.23) (fix for pruning issue in v1.10.22)
    - Nethermind [v1.14.0](https://github.com/NethermindEth/nethermind/releases/tag/1.14.0)
- Merge-ready consensus client releases:
    - Lighthouse [v3.0.0](https://github.com/sigp/lighthouse/releases/tag/v3.0.0)
    - Lodestar [v1.0.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.0.0)
    - Nimbus [v22.8.0](https://github.com/status-im/nimbus-eth2/releases/tag/v22.8.0)
    - Prysm [v3.0.0](https://github.com/prysmaticlabs/prysm/releases/tag/v3.0.0)
    - Teku [v22.8.1](https://github.com/ConsenSys/teku/releases/tag/22.8.1)
- ethereum.org [Merge announcement](https://blog.ethereum.org/2022/08/24/mainnet-merge-announcement):
    - 4x multiplier on Merge vulnerability bounties until September 8. **Up to $1 million for critical bugs**
    - Reminder: node operators/stakers _must_ run an execution and a consensus layer client
- Somer’s mainnet staking guides: [Teku](https://someresat.medium.com/guide-to-staking-on-ethereum-ubuntu-teku-f09ecd9ef2ee), [Lighthouse](https://someresat.medium.com/guide-to-staking-on-ethereum-ubuntu-lighthouse-773f5d982e03), [Nimbus](https://someresat.medium.com/guide-to-staking-on-ethereum-ubuntu-nimbus-31f56657ea8f) & [Prysm](https://someresat.medium.com/guide-to-staking-on-ethereum-ubuntu-prysm-581fb1969460); [migration guide for existing stakers](https://someresat.medium.com/supplementary-guide-to-staking-on-ethereum-for-existing-stakers-57493678a460)
- [Merge checklist](https://www.coincashew.com/coins/overview-eth/ethereum-merge-upgrade-checklist-for-home-stakers-and-validators) for home stakers
- [Flashbots Protect](https://writings.flashbots.net/writings/flashbots-protect-merge-and-beyond/) will be down during the Merge until MEV-boost goes live after ~10 epochs have been finalized
- [mainnet-shadow-fork-12](https://twitter.com/abcoathup/status/1562545482802806784) merges August 31
- Merge data analysis & data visualization [blog post challenge](https://esp.ethereum.foundation/merge-data-challenge)

**Execution layer**

- [Erigon architectural changes](https://hackmd.io/@4_PBxu6jQtO7qASCOn0H6w/SJUyNkuA9) for the Merge
- [Sustainability analysis of danksharding](https://hackmd.io/7NxqZepgR-iP9f4RIyqdbw) on network bandwidth costs
- [Data Availability Sampling](https://www.paradigm.xyz/2022/08/das) explainer & open problems

**Proof of Stake consensus layer**

- Danny Ryan’s [Finalized PoS update](https://blog.ethereum.org/2022/08/26/finalized-no-37)
- PoS implementers [call video](https://www.youtube.com/watch?v=tjmpu8O-xsA&t=113s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/Hy_d7lryj) and [Christine Kim](https://docsend.com/view/68ijsabyy5m8ybi4)
- Final regular edition of [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220826)
- MEV-boost relay monitor [code](https://github.com/ralexstokes/relay-monitor#readme), work in progress
- [consensus-specs](https://github.com/ralexstokes/ethereum-consensus/releases/tag/v0.1.0) in Rust
- [Graffiti fetch](https://github.com/rauljordan/graffiti-fetcher#readme): outputs Beacon chain graffiti since an epoch as CSV
- Coinbase [liquid staking token](https://twitter.com/CoinbaseAssets/status/1562476695357358080): withdraw Coinbase staked ETH on-chain
- [Swell Network](https://blog.swellnetwork.io/mainnet-soft-launch-announcement/) (liquid ETH staking) guarded launch controlled by the DAO
- [Monitoring staking infrastructure](https://www.kiln.fi/post/monitoring-ethereum-staking-infrastructure-at-scale) at scale

**Layer2**

- Arbitrum [Nitro whitepaper](https://github.com/OffchainLabs/nitro/blob/master/docs/Nitro-whitepaper.pdf)

**EIPs/Standards**

- [EIP5505](https://eips.ethereum.org/EIPS/eip-5505): ERC1155 asset backed NFT extension
- [EIP5516](https://eips.ethereum.org/EIPS/eip-5516): Soulbound multi-owned tokens
- [EIP5521](https://eips.ethereum.org/EIPS/eip-5521): Referable NFT
- [EIP5528](https://github.com/ethereum/EIPs/pull/5528/files): Refundable token standard

* * *

### **This newsletter is made possible thanks to** Starbloom Ventures!

![Starbloom Ventures](https://weekinethereumnews.com/wp-content/uploads/2021/11/Screenshot-from-2021-11-19-15-25-51.png)

Starbloom Ventures is a first round venture fund founded by Evan Van Ness to invest in the future of web3.

We pledge 10% of investing profits to support Ethereum public goods.

* * *

**Stuff for developers**

- [Variable Rate Gradual Dutch Auctions](https://www.paradigm.xyz/2022/08/vrgda): sell NFTs using a custom schedule
- [Chuff](https://github.com/alexroan/chuff#readme) (Huff utility contracts): ownable & safe math
- [Delegatable Diamond](https://github.com/delegatable/delegatable-sol/tree/main/contracts/diamond#readme): add Delegatable framework to ERC2535 contracts
- Maurelian’s [Solidity sandbox](https://github.com/maurelian/solidity-sandbox/#readme): simple repo to play with Solidity using Foundry
- [Setup a PoS devnet](https://rauljordan.com/2022/08/21/how-to-setup-a-proof-of-stake-devnet.html) (Prysm+Geth) using Docker
- Truffle [v5.5.28](https://github.com/trufflesuite/truffle/releases/tag/v5.5.28): Truffle Dashboard faster + dark mode
- titanoboa (Vyper interpreter) [user definable precompiles](https://twitter.com/big_tech_sux/status/1562931931423309828)
- Nethereum [v4.8.0](https://github.com/Nethereum/Nethereum/releases/tag/4.8.0): Host wallet RPC methods, batch RPC, AWS Key Manager external signer, EIP712 JSON support and ENS unicode
- MEV [CFMM arbitrage](https://noxx.substack.com/p/dex-arbitrage-mathematical-optimisations) via convex optimization
- [MEV searching](https://writings.flashbots.net/writings/searching-post-merge/) post-Merge
- OxPARC [zkPairing](https://0xparc.org/blog/zk-pairing-2): proof-of-concept implementation of elliptic curve pairings in Circom
- Paradigm CTF [0xMonaco](https://twitter.com/aradtski/status/1561451068265037825): resource management PvP racing game using contracts; writeups of [first](https://twitter.com/z0age/status/1561685707650990084) & [second](https://abdullathedruid.github.io/0xmonaco.html) place + (patched) [exploit to win](https://hackmd.io/@onemanbandplus2/S1Ez1Ulys) in a single turn

**Security**

- NEAR Rainbow bridge [unsuccessfully attacked again](https://twitter.com/alexauroradev/status/1561692371833667585), watchdog detected attack & created a challenge transaction

**Ecosystem**

- Superphiz’s [#stakefromhome](https://twitter.com/hashtag/stakefromhome): home stakers share photos of their setups
- Eric Wall: [case for social slashing](https://ercwl.medium.com/the-case-for-social-slashing-59277ff4d9c7)
- ETHGlobal ETH Mexico [finalists](https://ethglobal.medium.com/ethmexico-2022-b16a4843f2fd)
- Etherscan [token transfer warnings](https://twitter.com/etherscan/status/1561679607874863104) for tokens with poor reputation

**Enterprise**

- EEA [EthTrust security levels specification v1](https://entethalliance.org/enterprise-ethereum-alliance-advances-smart-contract-security-with-ethtrust-specification/)
- [VMware Blockchain](https://octo.vmware.com/introducing-vmware-blockchain-for-ethereum-beta-and-developer-kit/) for Ethereum, SBFT consensus, beta; [Infosys](https://www.infosys.com/services/blockchain/insights/management-solution.html) vital record management built on top
- [Blockchains provide businesses certainty](https://entethalliance.org/why-are-blockchains-useful-for-business/) about the future
- [Dashboard of big brand NFT revenue](https://dune.com/kingjames23/nft-project-possible-data-to-use), NIKE leads thanks to RTFKT acquisition

**Application layer**

- [Compound v3](https://medium.com/compound-finance/compound-iii-is-live-a7983dee7e60) is live, single borrowable asset, collateral won’t earn interest
- [Maker & Huntingdon Valley Bank](https://twitter.com/MakerDAO/status/1562045115828412417) first commercial loan
- [Uniswap Foundation to be created](https://twitter.com/haydenzadams/status/1562413424885243904) after 86 million UNI voted in favor
- Fei Labs proposal to wind down [Tribe DAO](https://tribe.fei.money/t/tip-121-proposal-for-the-future-of-the-tribe-dao/4475), disagreement over [repayment of hack victims](https://tribe.fei.money/t/tip-121-proposal-for-the-future-of-the-tribe-dao/4475/34)
- [eth.link down](https://twitter.com/ENS_DAO/status/1562998396968873984): domain due to be released September 5, beware of phishing attempts
- [ETH.LIMO](https://twitter.com/eth_limo/status/1562485520965312512) DNS over HTTPS resolver for ENS
- Coinbase [cb.id subdomains](https://twitter.com/brian_armstrong/status/1561935998577102850) live
- Aelin [NFT Gated pools](https://mirror.xyz/aelinnews.eth/FeDcPNcpQW3aHJvzyulFK31k6wRS5xZVsPB_hOF6afc)
- [BendDAO](https://thedefiant.io/benddao-emergency-changes) (NFT lending) adjusts liquidation levels

* * *

### **Job Listings**

- Gnosis Chain looking for [Head of Bridges](https://grnh.se/9bed164e2us), [Head of Validators](https://grnh.se/e51fc7332us) & [DevRel Eng](https://grnh.se/571e88cc2us).
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)

**Job listings: $600** for four issues (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Coin Center: [Tornado Cash explainer](https://www.coincenter.org/education/advanced-topics/how-does-tornado-cash-work/)
- [EFF representing Matthew Green](https://www.eff.org/deeplinks/2022/08/code-speech-and-tornado-cash-mixer) for republishing the Tornado Cash repos on GitHub
- [Alexey Pertsev pre-trial detention](https://www.prosecutionservice.nl/latest/news/2022/08/26/remand-suspect-tornado-cash-extended-by-90-days) extended by up to 90 days
- [Tether waiting on law enforcement instruction](https://tether.to/en/tether-holds-firm-on-decision-not-to-freeze-tornado-cash-addresses-awaits-law-enforcement-instruction/) before freezing Tornado Cash addresses
- [Coinbase US voter registration portal](https://blog.coinbase.com/why-were-launching-a-voter-registration-education-initiative-e5b1498d3674) to support crypto-forward policymakers

**General**

- [How crypto can resist](https://saffron.mirror.xyz/E6UKhw0KAZL1TgAeI_pcWSwkUDHOQ5R28OBHknTzy24) being captured by centralized actors
- [Decentralized identity](https://arxiv.org/abs/2208.11443): abstraction vs composability
- [Virgil Griffith](https://twitter.com/BrantlyMillegan/status/1561719432686276609) in solitary confinement due to lack of space, you can write to him
- [Mudge claims Twitter](https://edition.cnn.com/2022/08/23/tech/twitter-whistleblower-peiter-zatko-security/index.html) has major security problems
- [LastPass](https://blog.lastpass.com/2022/08/notice-of-recent-security-incident/) portions of source code stolen via compromised developer account
- [Hetzner](https://www.reddit.com/r/hetzner/comments/wucxs4/comment/ilfoj8u/) (cloud services) states PoW & PoS against their terms

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-27-2022](https://weekinethereumnews.com/week-in-ethereum-news-august-27-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Aug 28 – [Ethereum a New Era](https://go.ueth.org/) (San Francisco)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev/) (hackathon & conference)
- **Sep 3 –** [**Ethereum Lima day**](https://ethlima.org/index.php/eld/)
- Sep 2-28 – [ETHOnline](https://online.ethglobal.com/') (ETH Global)
- Sep 6 – [Bellatrix upgrade](https://blog.ethereum.org/2022/08/24/mainnet-merge-announcement/) (epoch: 144896)
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 7-22 – [Gitcoin Grants round 15](https://twitter.com/gitcoin/status/1558498622949523456)
- Sep 9 – [Merge Community Call #7](https://github.com/ethereum/pm/issues/599)
- Sep 9-11 – [Ethereum SP](https://www.ethereumbrasil.com/#next) (São Paulo)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Sep ~15 – [the Merge](https://blog.ethereum.org/2022/08/24/mainnet-merge-announcement/) (TTD: 58750000000000000000000)
- Sep 16-18 - [EthBerlin](https://ethberlin.ooo/)
- Sep 23 - [ETH HCMC](https://2022.ethhcmc.com/) summit (Ho Chi Minh)
- Sep 23-24 - [ETHSantiago](https://ethsantiago.com/)
- Oct 7-16 – [Devcon week](https://devcon.org/en/devcon-week/) (Bogotá)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- Oct 7-9 – [Infinite hackathon](https://infinite-hackathons.eth.limo/) (Bogotá)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- **Oct 18-23 –** [**Eth Medellin**](https://twitter.com/EthMedellin) **(Colombia)**
- **Oct 28-30 –** [**ETH Lisbon**](https://www.ethlisbon.org/)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- **Nov 11-13 –** [**ETHBrno**](https://mirror.xyz/ethbrno.eth/6BH9cUVuD85hy5O0L5cOOOE7niSA9Yo5eWsXVzKOlO4) **(Czech Republic)**
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

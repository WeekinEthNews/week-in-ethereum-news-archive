---
title: "Week in Ethereum News <BR> October 9, 2021"
date: "2021-10-09"
---

## **Eth News and Links**

**Mainnet execution layer**

- [Bonsai Tries](https://consensys.net/blog/news/bonsai-tries-a-big-update-for-small-state-storage-in-hyperledger-besu) flat storage model reduces Besu full archive to less than 1TB
- Piper Merriam’s [Aperture Portal Network update](https://snakecharmers.ethereum.org/aperture-vol-1/): two clients building a network to serve state

**EIPs/Standards**

- [EIP4345](https://eips.ethereum.org/EIPS/eip-4345): Difficulty Bomb Delay to May 2022

**Proof of stake consensus layer**

- Danny Ryan’s [Altair upgrade announcement](https://blog.ethereum.org/2021/10/05/altair-announcement/): update your staking clients by Oct 27! Bug bounty for critical Altair bugs now up to $100k 
- Client teams working on PoW switch off interop:
    - Devnet [confirmed](https://twitter.com/benjaminion_xyz/status/1446516207159582743); watch the [consensus monitor](http://mergenet.consensus-monitor.stokes.io)
    - [Video](https://www.symphonious.net/2021/10/08/ethereum-merge-local-testnet-demo/) of Teku/Lighthouse with Geth/Besu staying in sync and finalising after Altair upgrade and PoW switch off transition
    - Interop [day by day accomplishments](https://twitter.com/sigp_io/status/1446521008702246913)
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_211008): reflections on interop gathering to create long standing multiclient testnets to switch off PoW
- Consensus specs [v1.1.2](https://github.com/ethereum/consensus-specs/releases/tag/v1.1.2): fixes Altair and PoW switch off test generators
- [MergeMock](https://github.com/protolambda/mergemock): mock execution engine and consensus node for testing
- [Merge-fuzz](https://twitter.com/vdWijden/status/1446461842977591297): framework to test engine API
- List of [consensus client switching guides](https://www.reddit.com/r/ethstaker/comments/pxx0oz/ethstaker_comprehensive_list_of_client_switching/)
- Ethstaker [survey](https://ethstaker.cc/survey/#Z7ZpSghg) to understand needs of stakers
- Rocket Pool (staking pool) [launch delayed](https://twitter.com/Rocket_Pool/status/1445536222881857545) to address vulnerability

**Layer2**

- [StarkNet alpha](https://medium.com/starkware/starknet-alpha-is-coming-to-mainnet-b825829eaf32) on mainnet planned for November: permissioned deployment and no backward compatibility guarantee between alpha & beta
- [Arbitrum testnet explorer](https://testnet.arbiscan.io/) by Etherscan
- [Validity proof amortization](https://polynya.medium.com/the-dynamics-around-validity-proof-amortization-519e9ae291c1): zkRollup transactions get much cheaper with more use
- [zkRollup without transaction history data](https://ethresear.ch/t/a-zkrollup-with-no-transaction-history-data-to-enable-private-smart-contract-execution-with-calldata-efficiency/10961) enables private contract execution with calldata efficiency

* * *

### **This newsletter is made possible thanks to [NEAR](https://near.org/)!**

![NEAR Con Alpha](https://weekinethereumnews.com/wp-content/uploads/2021/09/Near-Con-Alpha.png)

[NEAR CON Alpha](https://nearcon.org/ethereumnews) is taking place in Lisbon on October 26th & 27th. The event is open to everyone to come and celebrate NEAR’s 1 Year Anniversary since Mainnet launch. Immerse yourself in two days of talks, networking, workshops and a whole lot more provided by the NEAR Ecosystem and its Community.

* * *

**Stuff for developers**

- [CREATE3](https://github.com/0xsequence/create3) contract library to deploy contracts, deterministic address depends only on the salt and not the code, fixed 60k extra gas cost
- [SSTORE2](https://twitter.com/Agusx1211/status/1446187302389170183) contract storage, cheaper than native storage for > 64 bytes, up to 17x cheaper than SLOAD and 3x cheaper than SSTORE, unaudited
- [ERC3652PureProxy](https://github.com/1inch/ERC3652/blob/feature/pure-proxy-factory/contracts/ERC3652PureProxy.sol): CREATE2 based pure proxy factory, executes delegate call in constructor
- [Fisher-Yates Shuffle](https://twitter.com/cleanunicorn/status/1445691819098992648), random on chain shuffle, O(n) complexity
- [noble-hashes](https://github.com/paulmillr/noble-hashes): fast, secure, minimal JavaScript implementations of SHA2, SHA3, RIPEMD, BLAKE2, HMAC, HKDF, PBKDF2 & Scrypt
- [prb-math.js](https://www.npmjs.com/package/prb-math.js): JavaScript for PRBMath Solidity library, use in testing
- Ξthernaut’s [Solidity Trivia questions](https://twitter.com/EthernautDAO/status/1445497302722826255)
- [eth-sdk](https://github.com/dethcrypto/eth-sdk): generate type-safe SDK for a contract using the address
- Solidity [dynamic array in storage](https://twitter.com/ylv_io/status/1445104519239643157) can overwrite contract storage when using onlyOwner modifier
- Vyper [v0.3.0](https://github.com/vyperlang/vyper/releases/tag/v0.3.0): refactored legacy backend, unblocks progress on requested features, use with care
- Otterscan [v2021.10.01](https://twitter.com/wmitsuda/status/1444789707540414466): transaction decoding of non-verified contracts and improved support for Sourcify verified contracts
- [mev-inspect-py](https://github.com/flashbots/mev-inspect-py): finds miner payments, token transfers, swaps and arbs
- Guide to [setting up Nile](https://medium.com/@martriay/starknet-tutorial-for-beginners-using-nile-6af9c2270c15) for StarkNet’s Cairo language
- [Auto battler logic](https://killari.medium.com/starks-verifying-a-complex-auto-battler-calculation-on-ethereum-d8698f29808d) in Python with STARK proof in Cairo

**Security**

- COMP at risk increased to ~490k, drip function sent [~200k COMP](https://twitter.com/rleshner/status/1444691278986457095) backlog to Comptroller, community have been returning COMP
- Staking pool [vulnerability](https://blog.lido.fi/vulnerability-response-update/) impacting Lido and Rocket Pool, deposit can be frontrun putting funds at risk, flagged by [StakeWise](https://twitter.com/stakewise_io/status/1445475001696620550), raised in [Eth Research](https://ethresear.ch/t/deposit-contract-exploit/6528) in late 2019
- Searcher contract [exploited](https://twitter.com/bertcmiller/status/1446416008709918732) for $1 million as token approvals function didn’t have appropriate checks

**Ecosystem**

- [Coinbase adopted EIP1559 transactions](https://blog.coinbase.com/the-technical-benefits-of-eip-1559-c41bb85f5924), 9% gas fee saving (~27 ETH per day) and improved confirmation time
- [Flashbots Protect](https://medium.com/flashbots/announcing-flashbots-protect-9e039e9f0aa3): API for dapps to integrate, RPC for wallets to use to send transactions via Flashbots
- Ethereum.org available in [37 languages](https://blog.ethereum.org/2021/10/04/translation-program-update/)
- NFT Fest Australia [videos](https://www.youtube.com/channel/UC9dHe2EmAyFtd3ahosns_1w)
- Nominate projects for [retroactive public goods funding](https://medium.com/ethereum-optimism/retropgf-experiment-1-1-million-dollars-for-public-goods-f7e455cbdca), $1 million given away from Optimism fees

**Application layer**

- [ENS profiles](https://medium.com/the-ethereum-name-service/nft-avatar-support-for-ens-profiles-bd4a5553f089) support NFT avatars
- [Mirror](https://dev.mirror.xyz/valptw8S9eZ1cvzX-JCGga2N_W2hXyurSYbOlNFj4OQ) opens publishing to all
- [Rune pitches a vision for MakerDAO](https://forum.makerdao.com/t/the-case-for-clean-money/10684) where Dai backed by solar, wind and ESG corporate bonds, plus updated tokenomics allowing locked MKR to have greater voting power with more attractive rates 
- Etherscan [visualisations of state of bridges](https://medium.com/etherscan-blog/ethereum-bridges-four-months-on-10ee36f889ae)
- [Difference](https://medium.com/@BraveNewDeFi/save-50-on-nexus-mutual-cover-premiums-how-to-use-wnxm-to-your-advantage-dc017b15aca0) between Nexus Mutual token price (from bonding curve) and wrapped token price (market sentiment) used for 50% discount on buying coverage
- Ethereum leads NFT ecosystem with over [$6 billion in secondary sales](https://www.getrevue.co/profile/masonnystrom/issues/the-multichain-nft-market-798081)
- [Context](https://twitter.com/context/status/1444038168739602435) beta, follow NFT activity of DAOs, creators and collectors
- [RICKS](https://www.paradigm.xyz/2021/10/ricks/) (Recurrently Issued Collectively Kept Shards), use cases include fractionalized NFTs and addressing [DAO apathy](https://twitter.com/danrobinson/status/1446251178099200005)
- [Infinity](https://medium.com/@infinitydotxyz/announcing-infinity-the-ftx-of-nfts-e0c2930b5f48) decentralized NFT marketplace, vampire attack of OpenSea with governance token airdrop

* * *

### **Job Listings**

- Lodestar (consensus client) hiring [TypeScript protocol engineer](https://jobs.smartrecruiters.com/ChainSafeSystemsInc/743999774954864-protocol-engineer-lodestar-backend-typescript-)
- Ethereum Foundation: [Research Intern](https://ethereum.bamboohr.com/jobs/view.php?id=45&source=weekinethnews), read/think/write with Josh Stark
- Nethermind 1-3 month [internship program](https://www.notion.so/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)
- [Team Lead](https://ethereum.bamboohr.com/jobs/view.php?id=43&source=weekinethnews) for the Ecosystem Support Program at the Ethereum Foundation

**Reach people experienced with Ethereum.**  $420 for two issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth. Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Circle received investigative subpoena](https://www.coindesk.com/business/2021/10/05/sec-subpoenas-usdc-stablecoin-backer-circle/) from Enforcement Division of US SEC in July
- [US Justice department](https://www.justice.gov/opa/pr/deputy-attorney-general-lisa-o-monaco-announces-national-cryptocurrency-enforcement-team) creates National Cryptocurrency Enforcement team focusing on money laundering
- IMF: [Crypto ecosystem and financial stability challenges](https://www.imf.org/en/Publications/GFSR/Issues/2021/10/12/global-financial-stability-report-october-2021), stablecoins require regulations proportionate to risk and economic functions they serve
- Bloomberg investigates [reserves backing Tether](https://www.bloomberg.com/news/features/2021-10-07/crypto-mystery-where-s-the-69-billion-backing-the-stablecoin-tether)
- US FDIC reported to be investigating pass through [deposit insurance for stablecoins](https://www.coindesk.com/policy/2021/10/06/us-fdic-said-to-be-studying-deposit-insurance-for-stablecoins/)

**General**

- Text message routing company had [unauthorized access](https://www.vice.com/en/article/z3xpm8/company-that-routes-billions-of-text-messages-quietly-says-it-was-hacked) of its databases, potential access to billions of SMS messages
- [Geofence and keyword warrants](https://www.forbes.com/sites/thomasbrewster/2021/10/04/google-keyword-warrants-give-us-government-data-on-search-users/?sh=142296ba7c97): Google gave US authorities info on anyone near a given location or who searched keywords 
- [Twitch breached](https://blog.twitch.tv/en/2021/10/06/updates-on-the-twitch-security-incident/), with source code and payouts leaked
- [Facebook outage](https://blog.cloudflare.com/october-2021-facebook-outage/) due to config change

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-october-9-2021/](https://weekinethereumnews.com/week-in-ethereum-news-october-9-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Oct 18 – [ENS online workshop](https://medium.com/the-ethereum-name-service/ens-online-workshop-october-2021-ec1fb049b77f)
- Oct 20-21 – [LisCon](https://liscon.org/) (Lisbon)
- Oct 22-24 – [ETH Lisbon](https://ethlisbon.org/) hackathon
- Oct 25 - Dec 13 – [Gitcoin DAO Global hackathon](https://gitcoin.co/hackathon/dao-global/onboard) (virtual)
- Oct 27 – Beacon chain upgrade to Altair [epoch 74240](https://blog.ethereum.org/2021/10/05/altair-announcement/) 
- Oct 28-29 – [ETH Portland](https://2021.ethportland.com/) hackathon
- Nov 1-4 – [NFT.NYC](https://www.nft.nyc/) sold out
- **Mar 28-30 – [ETHDubai](https://www.ethdubai.xyz/)**

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

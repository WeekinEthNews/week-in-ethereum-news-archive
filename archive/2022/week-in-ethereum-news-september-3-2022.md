---
title: "Week in Ethereum News <br> September 3, 2022"
date: "2022-09-03"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- Reminder: [Update your clients before Bellatrix on September 6](https://twitter.com/evan_van_ness/status/1565776410144169984)
    - Check you are running [Merge-ready releases with the latest bug fixes](https://blog.ethereum.org/2022/08/24/mainnet-merge-announcement)
- Merge TTD predicted September 14 by [797](https://797.io/themerge) & September 15 by [Bordel](https://bordel.wtf/); The difference is due to [Bordel using a bigger timespan for data](https://twitter.com/tmiychao/status/1564637160157880323) so is less reactive to hashrate spikes
- mainnet-shadow-fork-12 [merged perfectly](https://twitter.com/abcoathup/status/1565205804487102464)
- [mainnet-shadow-fork-13](https://twitter.com/abcoathup/status/1565663270173696000?s=20&t=PEOViXSdhUwf-zLrbH-R7Q) merges September 9, the last shadow fork before the Merge

**Execution layer**

- Latest core devs [call video](https://www.youtube.com/watch?v=GizYbtINRUs&t=45s). Notes from [Christine Kim](https://docsend.com/view/t5v9qqrjacvnsqri): short call, expect client releases next week for Erigon, Besu & Nethermind
- Erigon [v2022.08.03-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.08.03): fix for invalid block production
- [Large scale graffiti project](https://twitter.com/bantg/status/1563508806981910529) on Goerli testnet helped find invalid block production issue
- evmone (C++ EVM) [v0.9.0](https://github.com/ethereum/evmone/releases/tag/v0.9.0): 18% faster
- [EVM Object Format (EOF) explainer](https://twitter.com/teamipsilon/status/1565292837079597056): five EOF EIPs proposed for future upgrade
- KZG ceremony [call video](https://www.youtube.com/watch?v=ga78qx7TQvc&t=10s): plan to introduce at Devcon with a single contribution, public contributions to hopefully start November/December

**Proof of Stake consensus layer**

- [Client diversity](https://twitter.com/sproulM_/status/1564882712120291328): Prysm ~45% & Lighthouse 34%; Prysm assumed to be slightly lower & Nimbus slightly higher than estimated
- Lighthouse [v3.1.0](https://github.com/sigp/lighthouse/releases/tag/v3.1.0): fixes & optimizations for block production
- Nimbus [v22.8.2](https://github.com/status-im/nimbus-eth2/releases/tag/v22.8.2): fix for v22.8.1 if DEBUG logging enabled
- Teku [v22.9.0](https://github.com/ConsenSys/teku/releases/tag/22.9.0): fix for issue with public key validation
- [Checkpointz](https://github.com/samcm/checkpointz#readme): run a checkpoint sync endpoint or verify checkpoint sync data
- [Flashbots MEV-Boost relay](https://boost.flashbots.net/mev-boost-status-updates/mev-boost-mainnet-relay-live) live
- Proposed options for [block scoring](https://collective.flashbots.net/t/block-scoring-for-mev-boost-relays/202) in MEV-Boost
- [ERA archive file explainer](https://ethresear.ch/t/era-archival-files-for-block-and-consensus-data/13526): flat storage format for historical block & consensus data
- Possible [post-quantum replacement for Whisk](https://crypto.ethereum.org/blog/pq-ssle) in Single Secret Leader Election

**Layer2**

- [Arbitrum One](https://medium.com/offchainlabs/arbitrum-nitro-one-small-step-for-l2-one-giant-leap-for-ethereum-bc9108047450) upgraded to Nitro

**EIPs/Standards**

- [EIP5539](https://github.com/ethereum/EIPs/pull/5539/files): Revocation list registry
- [EIP5548](https://github.com/ethereum/EIPs/pull/5548/files): NFT operator approval control
- [EIP5553](https://eips.ethereum.org/EIPS/eip-5553): Representing IP and its royalty structure
- [EIP5554](https://github.com/ethereum/EIPs/pull/5554/files): NFT legal use, sharing, repurposing and remixing
- [EIP5559](https://eips.ethereum.org/EIPS/eip-5559): Cross chain write deferral protocol
- [EIP5560](https://eips.ethereum.org/EIPS/eip-5560): Redeemable NFTs
- [EIP5564](https://github.com/ethereum/EIPs/pull/5566/files): Stealth address wallets
- [EIP5568](https://github.com/ethereum/EIPs/pull/5568/files): Revert signals
- [EIP5570](https://github.com/ethereum/EIPs/pull/5570/files): Digital receipt NFTs

* * *

### **This newsletter is made possible thanks to** [**Hardhat**](https://hardhat.org/)**!**

![](https://weekinethereumnews.com/wp-content/uploads/2021/06/hardhat-rectangle-1024x325.png)

Hardhat just released support for The Merge, as well as major performance improvements on compilation times, making it _fast_. Solidity developers can now test their contracts in a post-merge environment, with compilation now taking 40% less in most workflows, and a few taking 90% less!

[Install the v2.11.0 release and check out the release notes to learn more](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.11.0).

* * *

**Stuff for developers**

- Hardhat [v2.11.0](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.11.0): test contracts post-Merge and fast compilation
- Remix [v0.26.0](https://medium.com/remix-ide/remix-ide-v0-26-0-release-bcd2371124ff): editor autocomplete, inline error display, jump to definitions, gas estimates; improved contract deploy selector; Vyper repo cloning
- Foundry [fork tests](https://twitter.com/msolomon44/status/1564742781129502722) setup, [fuzzing & invariant config](https://twitter.com/r_krasiuk/status/1565068796951273473) and [guide to file reading/writing](https://twitter.com/msolomon44/status/1565387268105199616)
- titanoboa (Vyper interpreter) [mainnet forking](https://twitter.com/big_tech_sux/status/1564066709707067392)
- web3.js [v4.x alpha](https://blog.chainsafe.io/alpha-release-of-web3-js-v4-x-4a5c7bfb16b1): Typescript rewrite, v1.x feature parity; moving to [web3 GitHub org](https://blog.chainsafe.io/web3-js-repository-migration-announcement-96cbb34e0c7e)
- Otterscan [v2022.08.03](https://twitter.com/otterscan/status/1565717004899721216): checkpoint sync, partial Sourcify matches and ENS emoji fix
- [Quay](https://alcibiades.capital/blog/announcing-quay/): backend API for Seaport marketplaces in Rust, MIT license
- [holders.at](https://holders.at/): snapshot of NFT holders at a specified block, shareable
- [Build an app NFT](https://medium.com/pinata/how-to-build-an-app-nft-7c57b51698e7) on OpenSea using animation URL pointing to IPFS
- [Optimize calldata usage in contracts](https://l2fees.info/blog/rollup-calldata-compression) for layer 2
- [zkPIN](https://github.com/zk-pin/pin#readme): commitment pools with zkSNARKs

**Security**

- Compound v2 [oracle update](https://www.comp.xyz/t/proposal-to-upgrade-to-uav-v3/3270/16) froze cETH market & impacts using ETH as collateral in other v2 markets, update being reverted with 7 day timelock
- KyberSwap [$256k frontend exploit](https://blog.kyber.network/notice-of-exploit-of-kyberswap-frontend-963aa8febd6a) from two victims, malicious code in Google Tag Manager script

**Ecosystem**

- Vitalik’s [Proof of Stake book](https://twitter.com/VitalikButerin/status/1564804705997361153), pre-order signed digital copy & non-transferable NFT
- Apply for Ethereum protocol fellowship [third cohort](https://blog.ethereum.org/2022/09/01/ethereum-protocol-fellowship-third), formerly core dev apprenticeship program
- Flashbots new [website](https://www.flashbots.net/) with dark mode
- NFT marketplace [web traffic visualization](https://twitter.com/0xKofi/status/1564639079454674944): Twitter, young, male, desktop & US users

**Application layer**

- Rune’s idea to [free float DAI](https://forum.makerdao.com/t/the-path-of-compliance-and-the-path-of-decentralization-why-maker-has-no-choice-but-to-prepare-to-free-float-dai/17466); MakerDAO [drama explainer](https://twitter.com/g_dip/status/1564716178819653632): futurists, centralists & decentralists
- [Rai](https://medium.com/reflexer-labs/rai-i-term-tuning-update-a6a8de72f86): adventures in tuning the PI controller parameters
- DeFi Saver [trailing stop](https://blog.defisaver.com/the-holy-grail-of-automated-trading-trailing-stop-now-available-for-makerdao-and-liquity/) automated strategy
- [Babylon Finance](https://medium.com/babylon-finance/babylon-finance-is-shutting-down-b58abf1bc251) shutting down
- [Config](https://twitter.com/wearenewt/status/1565010368077991937): visualizer of DeFi risk parameters, supports Aave
- [ENS .domains gateway](https://twitter.com/ensdomains/status/1564758903950577664), alternative to .limo; recovery of .eth.link still being attempted
- [ENS rarity](https://ensdaonews.substack.com/p/editorial-so-you-think-your-ens-category) and subdomains
- [Snoop Dogg & Eminem](https://twitter.com/vmas/status/1564074360884822018) perform as Bored Apes at the MTV Video Music Awards

* * *

### **Job Listings**

- ØVIX + GOGO Protocol: [Senior DeFi Blockchain Developer](https://join.com/companies/cryptogogos/5585820-blockchain-developer-at-crypto-start-up?utm_source=ETHnewsletter&utm_medium=email&utm_campaign=WeekInEthNews)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)
- Gnosis Chain looking for [Head of Bridges](https://grnh.se/9bed164e2us), [Head of Validators](https://grnh.se/e51fc7332us) & [DevRel Eng](https://grnh.se/571e88cc2us).

**Job listings: $600** for four issues (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- a16z [Can’t Be Evil NFT licenses](https://a16zcrypto.com/introducing-nft-licenses/): commercial rights or personal use variations
- foobar: [NFT royalties are unenforceable](https://0xfoobar.substack.com/p/on-royalties), options for creators to sustainably monetize
- [DAO treasury management in downturns](https://a16zcrypto.com/treasury-management-guide/): priorities are capital preservation, liquidity and income
- [web3 compensation](https://medium.com/@framework/navigating-web3-compensation-a-framework-report-1a053ba41767) (survey of 18 companies): $125k median ($150k US median) plus equity/tokens and remote working

**General**

- [Blockchain drama](https://www.thedefiant.io/avalanche-lawyer-scandal): undercover recordings of crypto lawyer
- Framework for users to [assess reliability of bridges](https://mirror.xyz/0xD4977DF3e967ddb604bB4f4D0d263f69B6c8A3e4/uPhBOMcQQ-TeY2n0naf3M8aLQnb04X2YcO41eaWpFN4)
- [Chrome zero-day](https://www.bleepingcomputer.com/news/security/google-chrome-emergency-update-fixes-new-zero-day-used-in-attacks/), insufficient data validation in Mojo
- [Chromium-based browsers](https://news.ycombinator.com/item?id=32614037) can write to clipboard without permission
- [US data broker selling location data](https://www.eff.org/deeplinks/2022/08/inside-fog-data-science-secretive-company-selling-mass-surveillance-local-police) for individuals gathered from apps to law enforcement

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-3-2022](https://weekinethereumnews.com/week-in-ethereum-news-september-3-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Sep 6 – [Bellatrix upgrade](https://blog.ethereum.org/2022/08/24/mainnet-merge-announcement/) (epoch: 144896)
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 7-22 – [Gitcoin Grants round 15](https://twitter.com/gitcoin/status/1558498622949523456)
- Sep 9 – [Merge Community Call #7](https://github.com/ethereum/pm/issues/599)
- Sep 9-11 – [Ethereum SP](https://www.ethereumbrasil.com/#next) (São Paulo)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Sep ~15 – [the Merge](https://blog.ethereum.org/2022/08/24/mainnet-merge-announcement/) (TTD: 58750000000000000000000)
- **Sep 16 –** [**Ethereum Protocol Fellowship**](https://blog.ethereum.org/2022/09/01/ethereum-protocol-fellowship-third) **applications close**
- Sep 16-18 - [EthBerlin](https://ethberlin.ooo/)
- Sep 23 - [ETH HCMC](https://2022.ethhcmc.com/) summit (Ho Chi Minh)
- Sep 23-24 - [ETHSantiago](https://ethsantiago.com/)
- Oct 7-16 – [Devcon week](https://devcon.org/en/devcon-week/) (Bogotá)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- Oct 7-9 – [Infinite hackathon](https://infinite-hackathons.eth.limo/) (Bogotá)
- Oct 11-14 – [Devcon 6](https://devcon.org/) (Bogotá)
- Oct 18-23 – [Eth Medellin](https://www.ethmedellin.co/) (Colombia)
- Oct 26-28 – [Eth Panama](https://twitter.com/EthPanama)
- Oct 28-30 – [ETH Lisbon](https://www.ethlisbon.org/)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 11-13 – [ETHBrno](https://mirror.xyz/ethbrno.eth/6BH9cUVuD85hy5O0L5cOOOE7niSA9Yo5eWsXVzKOlO4) (Czech Republic)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

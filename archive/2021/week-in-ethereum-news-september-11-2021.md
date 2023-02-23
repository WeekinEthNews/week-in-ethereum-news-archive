---
title: "Week in Ethereum News <BR> September 11, 2021"
date: "2021-09-11"
---

## **Eth News and Links**

**Mainnet execution layer**

- Apply for [second cohort](https://blog.ethereum.org/2021/09/06/core-dev-apprenticeship-second-cohort/) of core dev apprenticeship program, an effort by Piper Merriam to find and train more core devs
- Erigon [v2021.09.02](https://github.com/ledgerwatch/erigon/releases/tag/v2021.09.02): fixes RPC daemon races and bad.block parsing, mdbx update and work on moving tx pool into separate binary
- Geth considering ending support for [archive nodes](https://twitter.com/peter_szilagyi/status/1436226033934606338)

**EIPs/Standards**

- [EIP3855](https://eips.ethereum.org/EIPS/eip-3855): PUSH0 instruction
- [EIP3860](https://eips.ethereum.org/EIPS/eip-3860): Limit and meter initcode

**Proof of stake consensus layer**

- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210910) 🐼
- [PoS implementers call](https://www.youtube.com/watch?v=k3heiZA5j5s&t=104s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/S1smzqwzY) and [Alex Stokes](https://twitter.com/ralexstokes/status/1436001554486554626): create releases in September for planned Altair upgrade in October due to investigating lower sync aggregate participation on testnets 
- WARNING: [Staking pools are negligently putting users’ money at risk](https://twitter.com/superphiz/status/1434851281240301577) if they run the current majority client (or any future majority client)
- [Rocket Pool staged launch](https://medium.com/rocket-pool/rocket-pool-staking-protocol-part-4-2635c44e4f7e) begins October 6
- [Hardening the BLS12-381](https://blog.ethereum.org/2021/09/09/secured-no-1/) elliptic curve
- Validator [private message sharing](https://ethresear.ch/t/private-message-sharing-for-eth2-validators/10664) proposal for privacy and spam resistance, on chain interaction only for registration
- Researcher-oriented [cadCAD masterclass](https://twitter.com/cadCAD_Edu/status/1435580548957749250), learn how to model validator economics

**Layer2**

- David Mihal’s [L2 Fees](https://l2fees.info/): compare costs to transfer ETH/tokens and swap tokens
- Vitalik’s [proposal for rollup friendly NFTs](https://ethresear.ch/t/cross-rollup-nft-wrapper-and-migration-ideas/10507): wrapper NFT, cross-rollup transfers and gas-optimized issuing on mainnet
- [zk Rollups and data shards can achieve global scale](https://polynya.medium.com/why-rollups-data-shards-are-the-only-sustainable-solution-for-high-scalability-c9aabd6fbb48) while remaining technically and economically sustainable
- Why Arbitrum uses [interactive fraud proofs](https://medium.com/offchainlabs/interactive-fraud-proofs-arbitrums-secret-sauce-debc3b019418) instead of re-executing transactions
- [Arbitrum permissionless token bridging](https://offchain.medium.com/continued-path-to-decentralization-bridging-tokens-into-arbitrum-42a94b054560) opens October 22, tokens will be bridged as a basic ERC20 unless projects create a custom ERC20
- Ask centralized exchanges to [support rollup](https://twitter.com/evan_van_ness/status/1435277869115191296) on/off ramps

* * *

### **This newsletter is made possible thanks to [NEAR](https://near.org/)!**

![NEAR Con Alpha](https://weekinethereumnews.com/wp-content/uploads/2021/09/Near-Con-Alpha.png)

[NEAR CON Alpha](https://nearcon.org/ethereumnews) is taking place in Lisbon on October 26th & 27th. The event is open to everyone to come and celebrate NEAR's 1 Year Anniversary since Mainnet launch. Immerse yourself in two days of talks, networking, workshops and a whole lot more provided by the NEAR Ecosystem and its Community.

* * *

**Stuff for developers**

- dapptools [v0.34.1](https://github.com/dapphub/dapptools/releases/tag/dapp%2F0.34.1): test coverage, install contract libraries using tags/branches such as different OpenZeppelin Contracts versions
- seth [v0.11.0](https://github.com/dapphub/dapptools/releases/tag/seth%2F0.11.0): EIP1559 support and helpers for ENS
- [dapptools-template](https://github.com/gakonst/dapptools-template): quick start template for dapptools
- Ricmoo’s ethers.js [update](https://blog.ricmoo.com/highlights-ethers-js-september-2021-1bf7cb47d348): EIP1559 support and ethers playground
- [web3.js users survey](https://blocksurvey.io/survey/1K4bjDmqwtyAsehm1r4KbsdzRRDVyRCDoe/d2e239fd-a6b6-4fdc-9304-1a65459ded5a) to shape v4 rewrite
- [solidity-shell](https://github.com/tintinweb/solidity-shell): interactive Solidity shell with lightweight session recording 
- [loogies-svg-nft](https://github.com/austintgriffith/scaffold-eth/tree/loogies-svg-nft): on chain SVG NFT example using scaffold-eth
- [Generative-Transfer-Art](https://twitter.com/WilsonCusack/status/1434242261588533253) Solidity for on chain SVGs
- [Mint NFTs](https://github.com/flashbots/searcher-minter) using Flashbots
- NFT gated [ephemeral messaging board](https://twitter.com/yoheinakajima/status/1436327517808300033)
- Beginners: [use .env for API credentials](https://blog.infura.io/how-to-use-dotenv-to-enhance-basic-security-within-your-dapp) and don’t commit secrets to Git
- freeCodeCamp beginner Solidity [development course](https://dev.to/patrickalphac/learn-solidity-blockchain-and-smart-contracts-with-this-full-free-course-2bgn) (13 video lessons) using Python and Brownie

**Security**

- [OpenZeppelin UUPS proxy security advisory](https://forum.openzeppelin.com/t/security-advisory-initialize-uups-implementation-contracts/15301), projects should initialize implementation contracts
- DAO Maker ~$4 million [exploit](https://twitter.com/mudit__gupta/status/1434059922774237185), unprotected init function
- [OpenSea ERC721 transfer to ENS bug](https://twitter.com/nicksdjohnson/status/1435381872670826497) introduced and fixed same day, resulted in ownership of first ENS name registered being burnt
- [dYdX SafetyModule upgrade bug](https://dydx.foundation/blog/en/outage-1), storage layout changed in new implementation contract
- Tincho’s (OpenZeppelin) guidelines to integrate [price oracles](https://blog.openzeppelin.com/secure-smart-contract-guidelines-the-dangers-of-price-oracles/) with defensive programming practices
- [Clockwork Finance Framework](https://eprint.iacr.org/2021/1147): automated analysis of economic security of composed DeFi contracts

**Ecosystem**

- High gas fees this week reached [7 twei](https://twitter.com/the_ethernaut/status/1435318241153462274) during an NFT launch
- NFTs should use a [mix of distribution methods](https://twitter.com/0xmons/status/1435050021213245441) for initial supply: dutch auction, raffle, fixed price for early community and gifts to fan creators
- [MEV searcher design](https://twitter.com/bertcmiller/status/1434844547142520832) of a Synthetix liquidation, open source example of back running a transaction
- We need to [lower the barriers to entry](https://snakecharmers.ethereum.org/untapped-potential/), better tools lead to more devs and more devs lead to better tools and more innovative dapps
- ENS [attestation based DNSSEC claims](https://discuss.ens.domains/t/proposal-an-attestation-based-dnssec-implementation/699) proposal, reduces gas to ~10%
- Devcon planned for [2022](https://twitter.com/EFDevcon/status/1435641421810257920)

**Application layer**

- BarnBridge [SMART Alpha](https://medium.com/barnbridge/smart-alpha-is-live-b5f5a893878a): epoch based single asset pools, juniors provide downside protection to seniors in exchange for upside leverage
- SushiSwap’s BentoBox [explainer](https://twitter.com/josephdelong/status/1434209343700930570), application vault where up to 80% of deposited tokens are invested in strategies
- [Cover Protocol and Ruler Protocol](https://defited.medium.com/project-shutdown-cover-ruler-bb2df50e2a95) shutting down
- Lessons from [Kittyverse, Cheeze Wizards and Loot](https://twitter.com/Flynnjamm/status/1434157038142111748): ecosystems need to incentivize developers to build on top rather than build their own
- [Alpha Buy Wall](https://blog.alphafinance.io/launching-alpha-buy-wall-for-nfts/), on chain NFT price floor 
- [Stewart Brand documentary selling NFTs](https://weareasgods.mirror.xyz/crowdfunds/0x69DdE2e4d81720AEfdb50Bc7439EDd32565d21f2) to stream film with aim to make free to everyone
- Sorare adds Spain’s [LaLiga](https://medium.com/sorare/laliga-joins-sorare-419405687d28) NFTs
- [Christie’s to conduct](https://twitter.com/ChristiesInc/status/1435346651217108996) bidding in ETH

**Regulation/business/tokens**

- US [SEC intends to pursue legal action against Coinbase](https://blog.coinbase.com/the-sec-has-told-us-it-wants-to-sue-us-over-lend-we-have-no-idea-why-a3a1b6507009) for planned Lend product
- [Commissioner Peirce](https://www.sec.gov/news/public-statement/peirce-iac-090921) (US SEC): investor protection matters, but so does investor opportunity
- Former US CFTC chair’s book [CryptoDad: The Fight for the Future of Money](https://www.chrisgiancarlo.org/book) available for preorder
- Standard Chartered issues [research report valuing ETH at $26k-35k](https://www.tbstat.com/wp/uploads/2021/09/Ethereum-investor-guide.pdf)
- [DAO report](https://docs.google.com/presentation/d/1fLJvPOvibcCUpJ9ES44_cdoX5Hb7LpDaloGWz5FbUEM/edit#slide=id.gec41538503_0_399): reasons to study DAOs, key takeaways, survey results (~400 participants from ~200 DAOs) and hot takes

**General**

- [Epic vs Apple](https://www.theverge.com/2021/9/10/22662320/epic-apple-ruling-injunction-judge-court-app-store?scrolla=5eb6d68b7fedc32c19ef33b4): in app purchase alternatives to be allowed, potential for Apple to be less restrictive on Ethereum apps
- Apple [delays plans to scan your iPhone](https://www.apple.com/child-safety/) for offending files in iOS15
- [Spook.js](https://www.spookjs.com/) transient execution side channel attack targeting Chrome 
- [Vulnerabilities in tar and @npmcli/arborist](https://github.blog/2021-09-08-github-security-update-vulnerabilities-tar-npmcli-arborist/), upgrade node or npm
- [Voyages of cruise ship Satoshi](https://www.theguardian.com/news/2021/sep/07/disastrous-voyage-satoshi-cryptocurrency-cruise-ship-seassteading), collapse of crypto seasteading project
- [ProtonMail logged French activists IP address](https://protonmail.com/blog/climate-activist-arrest/) after order by Swiss authorities, Proton provides an onion site for anonymous access

* * *

## **Job Listings**

- Rarible is hiring: [VP of Product](https://jobs.lever.co/Rarible/47ed8db0-2161-420c-9321-4ade80e8dece) and [Product Manager](https://jobs.lever.co/Rarible/06d88504-b740-434e-87c0-72846b9ddeeb)
- Enzyme hiring [Solidity Eng.](https://apply.workable.com/avantgarde-finance/j/7E54B2975D/) & [Data Eng.](https://apply.workable.com/avantgarde-finance/j/C105B5596D/) $15k referral for successful hires
- Winding Tree is hiring a [SSI Guru/Smart Contract Dev](https://www.linkedin.com/jobs/view/2700418344/) for ORGiD
- Solidity is [hiring a C++ dev](https://ethereum.bamboohr.com/jobs/view.php?id=40&source=weekinethnews)
- OpenZeppelin is hiring an [Open Source Developer](https://openzeppelin.com/jobs/opening/?gh_jid=4554917003)
- Nomic Labs hiring Snr Software Engineers: [Hardhat Ignition](https://nomiclabs.notion.site/Senior-Software-Engineer-Hardhat-Ignition-71c83f5a5a6b4fef99da95d9dc124d70) & [Hardhat VSCode](https://nomiclabs.notion.site/Senior-Software-Engineer-Hardhat-VSCode-23cfe4ccf56846ada207c83e3a2830c3)

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-11-2021/](https://weekinethereumnews.com/week-in-ethereum-news-september-11-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- **Sep 13 – deadline to apply for [Eth core dev apprenticeship](https://blog.ethereum.org/2021/09/06/core-dev-apprenticeship-second-cohort/)**
- Sep 15-17 – [MetaCartel MCON Denver](https://www.mcon.fun/)
- Sep 17-Oct 15 – [ETHOnline hackathon](https://online.ethglobal.com/)
- Sep 22  – [Gitcoin Grants Round 11](https://gitcoin.co/grants/) ends (support [Week in Eth News](https://gitcoin.co/grants/2785/week-in-ethereum-news))
- Sep 30 – [NFT Fest Australia](https://nftfest.com.au/) (virtual)
- Oct 1-3 – [EthAtlanta](https://ethatl.com/) enterprise-focused hackathon & keynotes
- Oct 20-21 – [LisCon](https://liscon.org/) (Lisbon)
- Oct 22-24 – [ETH Lisbon](https://ethlisbon.org/) hackathon

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

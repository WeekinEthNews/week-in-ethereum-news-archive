---
title: "Week in Ethereum News <br> April 8, 2023"
date: "2023-04-08"
---

## Eth News and Links

**Shapella (Shanghai + Capella) upgrade**

- Reminder: [update your nodes for Shapella upgrade](https://blog.ethereum.org/2023/03/28/shapella-mainnet-announcement) on April 12th at 22:27:35 UTC

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=MrHh_jS4lZY&t=195s). Notes from [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-consensus-call-106/):
    - Mainnet shadow fork 3 finalizing with no client incompatibilities
    
    - Proposal to change blob transaction type from 0x5 to 0x3
    
    - Discussion on MEV Boost issues

**Dencun (Cancun + Deneb) upgrade**

- KZG ceremony [special contributions started](https://twitter.com/trent_vanepps/status/1644051402874933257):
    - [Cryptosat](https://kzg.cryptosat.io/) contributed from space via Crypto2 satellite
    
    - [Marble machine](https://twitter.com/Xofee3/status/1644016160210313218) generated 420 random values

- Latest EIP4844 implementers [call video](https://www.youtube.com/watch?v=k6TDcU2aBDw&t=3s). Notes from [Terence](https://twitter.com/terencechain/status/1642938324938805249)

**Layer 1**

- [Mev-boost-relay bug](https://collective.flashbots.net/t/post-mortem-april-3rd-2023-mev-boost-relay-incident-and-related-timing-issue/1540): ~$20 million drained from sandwich bots, relay revealed block bodies for invalid block headers; [v1.0.0-alpha3](https://github.com/flashbots/mev-boost-relay/releases/tag/v1.0.0-alpha3) patch to publish block before returning to proposer
    - [Offending validator got slashed](https://twitter.com/mikeneuder/status/1642899865288994816) for equivocation

- The [perils of restaking](https://dataalways.substack.com/p/endgame-perils-of-restaking)

- Ben Edgington’s Upgrading Ethereum book [fork choice](https://eth2book.info/bellatrix/part3/forkchoice/) section; search & dark mode added

**For Stakers**

- [Set validator withdrawal address](https://medium.com/@gethwethreth/guide-to-setting-withdrawal-address-for-your-ethereum-validator-using-deposit-cli-76cb2711eec9) using deposit-cli

- [Solo stakers using ⌐◨-◨ graffiti](https://twitter.com/wilsoncusack/status/1643299151751401473) go into monthly draw for ten 1 ETH prizes

- [Goerli validator faucet](https://blog.chainsafe.io/ethereum-testnets-goerli-eth-and-a-way-forward-265b02258700): deposit 3.3 Sepolia ETH to test validator setups on Goerli

- [Lido address change messages](https://twitter.com/lidofinance/status/1643597930945818626) signed ready to broadcast after Shapella

**Layer 2**

- [Arbitrum DAO rejected ratification vote to setup Foundation](https://twitter.com/arbitrum/status/1643699348683870211) but 7.5% token allocation already sent to Foundation with 10M ARB sold for expenses & 40M ARB loaned to market maker, new proposals for Foundation budget & lockup and reduce proposal token threshold

**EIPs/Standards**

- ERCs:
    - [ERC6821](https://github.com/ethereum/EIPs/pull/6821/files): Support ENS name for web3 URL
    
    - [ERC6823](https://github.com/ethereum/EIPs/pull/6830/files): Token mapping slot retrieval extension

* * *

### **This newsletter is made possible thanks to** [**Mimic**](https://mimic.fi/)**!**

![mimic](https://weekinethereumnews.com/wp-content/uploads/2022/10/mimic-banner-1024x427.png)

Are you a founder or dev spending too much time doing transactions and mashing buttons on your hardware wallet just to _collect fees across chains_ or _claim rewards_ and _periodically swap assets_? 

With Mimic, you can **automate swapping, bridging and treasury management**.

Find out why some of the biggest DeFi names trust our [Smart Vaults](https://medium.com/mimicfi/introducing-smart-vaults-3438bacc843d) to automate DeFi operations in a secure, trustless, and non-custodial way.

* * *

**Stuff for developers**

- Remix IDE [v0.32.0](https://medium.com/remix-ide/remix-ide-v0-32-0-release-3385255dccb2): run free functions, fork in GitHub actions, download UML as pdf/png and doc generation from NatSpec in markdown

- [Cookbook Remix plugin](https://twitter.com/cookbook_dev/status/1643629831140065287): find contracts from Cookbook registry

- [Precision loss vulnerabilities](https://dacian.me/precision-loss-errors) classified in Solidity

- [ABI encoding guide](https://r4bbit.substack.com/p/abi-encoding-and-evm-calldata) using Foundry cast

- [Forge-safe-log](https://github.com/Philogy/forge-safe-log#readme): Foundry 32 character logging that doesn’t modify the state of memory

- Fe [v0.22.0](https://blog.fe-lang.org/posts/beyond-alpha-preparing-fe-for-the-future/): first non-alpha release

- [Solhunt](https://github.com/iFrostizz/solhunt#readme): Solidity static analyzer

- [Sporalyzer](https://github.com/0xMob100/sporalyzer#readme): EVM contract size analyzer in JavaScript

- [Guide to event reading](https://web3-ethereum-defi.readthedocs.io/tutorials/multithread-reader.html) in Python using multithreading

- [Universal Frontend](https://twitter.com/nazar_ilamanov/status/1641890861637324801): read/write contract functions on mainnet; supports structs, arrays & tuples

- [Storagoor](https://storagoor.vercel.app): read storage slot for contracts on mainnet & testnets

- Curta CTF Uncertainty Principle [solution](https://twitter.com/0x796/status/1643992379140235264)

- RareSkills [huff-puzzles](https://github.com/rareSkills/huff-puzzles#readme)

- Secureum RACE #16: [8 question Solidity quiz & answers](https://ventral.digital/posts/2023/4/1/race-16-of-the-secureum-bootcamp-epoch-infinity)

- [Dissecting EVM](https://medium.com/@deliriusz/dissecting-evm-using-go-ethereum-eth-client-implementation-part-i-transaction-execution-flow-960a1533e994) via Geth implementation

- viem [v0.2](https://twitter.com/wagmi_sh/status/1642989796753813506): contract instances, create/import private key & mnemonic accounts, account hoisting, automated transport ranking, ENS avatar & text retrieval, transaction & typed data utilities

- [Mainnet datasets](https://twitter.com/wmitsuda/status/1643012781262745606) for ERC20/165/721/1155/1167 in csv

**Security**

- Sentiment [~$1 million exploit](https://twitter.com/peckshieldalert/status/1643423875064270848) on Arbitrum via read-only reentrancy, [funds returned minus $95k](https://twitter.com/sentimentxyz/status/1644039092378689536)

- Enzyme [Gas Station Network implementation vulnerability disclosed](https://twitter.com/enzymefinance/status/1643893025532178432), $400k bounty to be paid

- Token sale project [locked funds on zkSync Era using transfer function](https://twitter.com/zksync/status/1644139364270878720), plan to change [gas metering to support transfer](https://twitter.com/zksync/status/1644459406828924934) & allow fund recovery

- Uniswap Universal Router [reentrancy vulnerability disclosed](https://www.nomoi.xyz/blog/uniswap-vulnerability-disclosure), fixed prior to deployment

- Solidity [function pointer equality bug](https://twitter.com/dedaub/status/1643398669071204352), equality to be removed in v0.9

**Ecosystem**

- [MEV Blocker](https://mevblocker.io/): mainnet RPC, blocks front running & sandwiches, searchers can pay users to back run their transaction

**Enterprise**

- [ANZ bank piloted trading tokenized carbon credits](https://media.anz.com/posts/2023/april-/anz-and-grollo-partner-to-trade-tokenised--australian-carbon-cre) for Australian dollar stablecoin

**Notable at app layer**

- Euler: [recoverable funds returned](https://twitter.com/eulerfinance/status/1643027386802270210) from March exploit; [redemption plan](https://forum.euler.finance/t/plan-for-redemption-of-euler-funds/906)

- [MetaMask adds warnings](https://twitter.com/metamask/status/1643702565140348929) for known scams from OpenSea’s blocklist & Blockaid’s analysis

- [OpenSea Pro](https://twitter.com/openseapro/status/1643314687134556160) (formerly Gem v2) NFT aggregator

- [OpenEden TBILL vault](https://medium.com/@openeden/introducing-tokenized-u-s-treasuries-from-openeden-e40eacd9b762): tokenized US Treasuries currently ~5%, requires KYC

- [Flexible voting](https://twitter.com/ScopeLift/status/1547627175347507205): DAOs can extend Governor to split voting or allow tokens in DeFi to vote or vote privately

* * *

### Job Listings

- EF Ecosystem Support Program seek a [Grant Analyst & Liaison](https://jobs.lever.co/ethereumfoundation/92306cf4-1a7d-4e32-bc23-9762383522b1)

- [Nimbus](https://nimbus.team/#about) is hiring a [Site Reliability Engineer](https://jobs.status.im/?gh_jid=4797968)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US Treasury [DeFi risk assessment](https://home.treasury.gov/news/press-releases/jy1391)

- [Did Elizabeth Warren collude with short seller](https://archive.ph/s0dGU) to destabilize the banking system?

- Foreign Affairs: [the case for banning crypto](https://archive.is/2O5qb)

- [FASB](https://www.fasb.org/page/getarticle?uid=fasb_Media_Advisory_03-23-23) proposed crypto assets be accounted at fair value each reporting period, comments open through June 6

**General/crypto**

- [zkTree](https://polymerlabs.medium.com/introducing-zktree-a-zk-recursion-tree-with-zkp-membership-proofs-571a244e3169): zk recursion tree with ZKP membership proofs

- Ideas for a [Nova-based zk VM](https://zkresear.ch/t/towards-a-nova-based-zk-vm/105)

- [eSTARK](https://eprint.iacr.org/2023/474): extending STARKs with arguments

- [Testudo](https://cryptonet.org/blog/testudo-efficient-snarks-with-smaller-setups): near linear-time prover SNARK with smaller setups

- [UltraGroth](https://hackmd.io/@Merlin404/Hy_O2Gi-h): Groth16-style protocol with lookups

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-april-8-2023](https://weekinethereumnews.com/week-in-ethereum-news-april-8-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Apr 8 – deadline for [Scaffold-Eth-2 hackathon](https://hackathon.buidlguidl.com/)

- Apr 12 – [Mainnet upgrades to Shapella](https://github.com/ethereum/execution-specs/blob/master/network-upgrades/mainnet-upgrades/shanghai.md#upgrade-schedule), **EthStaker** [**viewing party**](https://www.reddit.com/r/ethereum/comments/12bsyy5/come_celebrate_the_shanghaicapella_upgrade_to/)

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- Apr 13-16 – [Pragma Tokyo](https://ethglobal.com/events/pragma-tokyo) & [ETHGlobal Tokyo](https://tokyo.ethglobal.com/) hackathon

- Apr 14-16 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference & hackathon

- Apr 21-25 – [EthTaipei](https://ethtaipei.org/) hackathon & conference

- **Apr 25 - May 9 –** [**Gitcoin Program Beta Round**](https://gitcoin.notion.site/Gitcoin-Grantee-Portal-6adfc92627474bd48a5dfcd1e8438d20)

- Apr 27-30 – [Istanbul ETH Privacy](https://www.leadingprivacy.com/istanbul) conference & hackathon

- Apr 28 – deadline for EF’s [Next Billion fellowship cohort 3](https://blog.ethereum.org/2023/03/16/fellowship-cohort-3-applications)

- May 5-10 – [ETHTallinn](https://ethtallinn.org/) hackathon & [NFT Tallinn](https://nfttallinn.com/) conference

- May 9-12 – [EY blockchain summit](https://web.cvent.com/event/c066d44d-4e50-4d7e-b6fb-3cc0abdae7ff/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7)

- May 12-14 – [ETHGlobal Lisbon](https://ethglobal.com/events/lisbon)

- May 19-23 – [EDCON](https://edcon.io/) Montenegro (changed from Vienna)

- May 20-21 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 24-26 – [Spaghett ETH](https://naples.spaghett-eth.com/) (Naples) conference

- May 26-28 – [ETHDublin](https://www.ethdublin.io/) hackathon

- Jun 2-4 – [ETH Seoul](https://2023.ethseoul.org/)

- Jun 2-7 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 9-11 – [ETHPrague](https://ethprague.com/) conference & hackathon

- Jun 23–25 – [ETHGlobal Waterloo](https://ethglobal.com/events/waterloo2023) (changed from Toronto)

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- **Jul 15-16 –** [**DeFi Security Summit**](https://defisecuritysummit.org/) **(Paris)**

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Aug 13-16 – [ETHToronto](https://www.ethtoronto.ca) & [ETHWomen](https://www.ethwomen.com/)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org) (Buenos Aires)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 30 - Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- **Sep 18-21 –** [**ETH Montréal**](https://ethmontreal.xyz/) **hackathon & conference**

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 27–29 – [ETH Miami](https://ethmiami.net/) festival + hackathon

- Oct 28–30 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- November – Devconnect

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

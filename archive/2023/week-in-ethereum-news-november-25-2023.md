---
title: "Week in Ethereum News <br> November 25, 2023"
date: "2023-11-24"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=_by0UBqrYng&t=322s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1727810699295113339):
    - Devnet-11: mostly stable
    
    - [Devnet-12](https://notes.ethereum.org/@ethpandaops/dencun-devnet-12): planned for next week if 3+ CL clients are ready
    
    - Goerli: upgrade unlikely in December; client team & EF validators will be stopped 3 months after upgrading (or 1 month after mainnet upgrade if later), then 1 month of chaos testing
    
    - [eth\_multicallV1](https://docs.google.com/presentation/d/1lEaqHTY3ud8pe6VAFwLkb-jdoHpTMBfuF1K9OKy-azs) proposed addition to JSON RPC

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 32.00%**](https://dune.com/hildobby/eth2-staking) **is increasing towards** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)
    - Lido node operator [InfStones](https://0d.dwalletlabs.com/the-billion-dollar-exploit-collecting-validators-private-keys-via-web2-attacks-4a385a5bb70d) server vulnerabilities disclosed

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~85% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm 41% & Lighthouse 34%, any client bug over 33.3% could mean loss of finality

- [Geographic diversity needed](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Dapplion: [EIP6914](https://hackmd.io/@dapplion/eip6914) (reuse withdrawn validator indices) may not be required for several years

- MEV [Order Flow Auctions](https://www.monoceros.com/insights/order-flow-auctions) overview

**Client releases**

- Execution layer:
    - Reth [v0.1.0-alpha.11](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.11): Cancun-ready, op-reth, adds eth\_callBundle, eth\_getProof & trace\_filter and more accurate RPC tracing

**EIPs/Standards**

- EIPs
    - [EIP7563](https://github.com/ethereum/EIPs/pull/7971/files): Time Capsule encryption via VDF

- ERCs (application layer):
    - [ERC7564](https://github.com/ethereum/ERCs/pull/111/files): Contract wallet management NFT

**Stuff for developers**

- Foundry:
    - forge-std [v1.7.3](https://github.com/foundry-rs/forge-std/releases/tag/v1.7.3): adds mock ERC20 & ERC721 contracts and new cheat codes: stop/start state diff recording & compute create/create2 address
    
    - Foundry-devops [v0.1.0](https://github.com/Cyfrin/foundry-devops/releases/tag/0.1.0): get most recent deployment, removed ffi requirement
    
    - [anvil-web3](https://github.com/alpinevm/anvil-web3#readme): create & interact with Anvil instances from Python

- Edge (EVM domain specific language) [specification](https://edge-specification.vercel.app/)

- [Impersonator iframe](https://github.com/impersonator-eth/iframe#readme): connect to a dapp in iframe via SafeConnector

- Solidity [inheritance puzzle solution](https://twitter.com/apoorvlathey/status/1726229244593004905)

- [Scaffold-ETH 2 challenges](https://github.com/kmjones1979/scaffold-eth-2-solidity/tree/main#readme) teaching Solidity, Hardhat, NextJS, Scaffold-ETH 2 & The Graph

- Curta Cup CTF solutions: [1st placed team](https://www.youtube.com/watch?v=9aiABoKltG4) \[video\] & [2nd placed team](https://mirror.xyz/%F0%9F%91%85%F0%9F%8C%88%F0%9F%91%85.eth/QLkBG4IkXVtQjm7olpblsMNHmf_YHw9LfDgCZGZ9QtI)

- Dan Finlay: [redeemDelegation](https://ethereum-magicians.org/t/towards-more-conversational-wallet-connections-a-proposal-for-the-redeemdelegation-interface/16690), proposal for more conversational wallet connections

**Security**

- KyberSwap Elastic (concentrated liquidity) [$54M exploit](https://twitter.com/KyberNetwork/status/1728115858889929021) on mainnet, L2s & sidechains; [exploit reproduction](https://github.com/paco0x/kyber-exploit-example#readme)

- Guide to [recovering funds from compromised keys using HackedWalletRecovery](https://officercia.mirror.xyz/014GrOMt24VPHS-_UNWUujCm8HMmyffaskHv5PMeqnA)

**Ecosystem**

- ETHGlobal:
    - Istanbul hackathon [finalists](https://twitter.com/ethglobal/status/1726245596926009623)
    
    - 2024 [hackathon calendar](https://ethglobal.com/events): London, Sydney, Brussels, Singapore, San Francisco & DevCon

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 12.1 to 413.7 gwei, with 31.7 gwei average
    - Zero net issuance currently at 21.8 gwei 
    
    - 7.4k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $1,930 - $2,131, currently $2,076

- [ETHBTC](https://ratiogang.com/): currently 0.055 (Flippening at ~0.16)

**Notable at app layer**

- [Blast (preannounced L2)](https://twitter.com/jarrodWattsDev/status/1727584394796323042) promoted as [native yield](https://twitter.com/adietrichs/status/1727697517914075471), taking deposits (no withdrawal), controlled by 3/5 multisig, pyramid style rewards, ETH deposits being invested via Lido

- Circle [bridged USDC standard](https://www.circle.com/blog/bridged-usdc-standard), L2s can deploy with option to later upgrade to native issuance

- Nick Johnson: [.eth & DNS root](https://twitter.com/nicksdjohnson/status/1726629086372737234) explainer

- evm.storage [EOA pages](https://twitter.com/smlxldotio/status/1727355287198453775): view snapshot of an account at a specific block

* * *

### Job Listings

- Aragon: [Senior smart contract developer](https://jobs.lever.co/aragon/2f3cf4c4-041a-4978-aa6b-78f447358956) w EIP, auditing experience

- [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db) wanted by EF

- Enya Labs: [Lead Security Engineer](https://enyalabs.applytojob.com/apply/vkSNxMxgCT/Founding-Security-Engineer?source=weekinethereumnews), [Sr. Fullstack Dev](https://enyalabs.applytojob.com/apply/FlzWnQ2S7G/Senior-Full-Stack-Developer?source=weekinethereumnews) (with Go exp), [BizDev](https://enyalabs.applytojob.com/apply/eIiMobirGL/Business-Development?source=weekinethereumnews)

- Nethermind: [Lead Software Engineer](https://grnh.se/e2d52f72teu), [BizDev](https://grnh.se/9fbf4582teu) & [CTO](https://grnh.se/4a264c32teu)

**Job listings: $600 for four issues** (75 character limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Binance: [$4.3B settlement](https://www.justice.gov/opa/pr/binance-and-ceo-plead-guilty-federal-charges-4b-resolution) with DoJ, FinCEN, OFAC & CFTC; [CZ resigns](https://twitter.com/cz_binance/status/1727063503125766367) as CEO

- [SEC allege Kraken](https://blog.kraken.com/news/kraken-continues-to-fight-for-its-mission-and-crypto-innovation-in-the-united-states) operates as an unregistered securities exchange

- [Tether froze 225M in stolen USDT](https://tether.to/en/following-investigations-by-tether-okx-and-the-us-department-of-justice-tether-voluntarily-freezes-225m-in-stolen-usdt-linked-to-international-crime-syndicate/) linked to international crime syndicate

- [Wyoming Stable Token Commission](https://stabletoken.notion.site/Scoping-95d69b3c57ff48018ccaecb1c2c47ff6) request for info/proposals for their stablecoin

- [Bittrex Global](https://bittrexglobal.com/) winding down

- [Coindesk bought](https://bullish.com/news-insights/news/bullish-acquires-coindesk-from-digital-currency-group/) by Bullish (centralized exchange)

**General**

- Hacks: HTX & Heco bridge [$99M lost](https://rekt.news/heco-htx-rekt/) and Kronos Research (market maker) [$26M lost](https://rekt.news/kronos-rekt/)

- [Binius](https://www.ulvetanna.io/news/binius-hardware-optimized-snark): implementation in Rust of SNARK for towers of binary fields

- [BabySpartan](https://eprint.iacr.org/2023/1799): Lasso-based SNARK for non-uniform Plonkish arithmetization

- [Fully Homomorphic Encryption](https://taiko.mirror.xyz/2O9rJeB-1PalQeYQlZkn4vgRNr_PgzaO8TWUOM5wf3M) (FHE) explainer

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-november-25-2023](https://weekinethereumnews.com/week-in-ethereum-news-november-25-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Nov 29 – [Gitcoin Grants 19](https://grants.gitcoin.co/#GG19-Rounds) ends (support [Week in Ethereum News](https://explorer.gitcoin.co/#/round/424/0x98720dd1925d34a2453ebc1f91c9d48e7e89ec29/0x98720dd1925d34a2453ebc1f91c9d48e7e89ec29-246))

- Nov 30 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) deadline (max $1k for local meetups)

- Dec 4 – [ETHVenice](https://ethvenice.com/)

- Dec 6-7 – [Columbia CryptoEconomics workshop](http://columbiacryptoeconomics.org/) (New York)

- Dec 7 – Optimism’s [RetroPGF 3 voting](https://vote.optimism.io/retropgf/3) ends (support [Week in Ethereum News](https://vote.optimism.io/retropgf/3/application/0x44be5b3d06daade4fd7a1c3e1bc9428926befe272b72c16f2d72dce66692af13))

- Dec 7-10 – ETHGlobal [Pragma](https://ethglobal.com/events/pragma-india) & [ETHIndia](https://ethindia.co/) (Bangalore)

- Jan 15 – EF’s [Next Billion fellowship cohort 4](https://fellowship.ethereum.foundation/) deadline

- **Feb 23-Mar 3 –** [**ETHDenver**](https://www.ethdenver.com/) **BUIDLWeek & hackathon**

- **Mar 13-14 –** [**ETHLatam**](https://ethlatam.org/) **(San Pedro Sula, Honduras)**

- **Mar 14-17 –** [**Pragma**](https://ethglobal.com/events/pragma-london) **&** [**ETHGlobal London**](https://ethglobal.com/events/london2024)

- **Apr 5-26 – ETHGlobal** [**Scaling Ethereum**](https://ethglobal.com/events/scaling2024) **(virtual)**

- **May 2-5 –** [**Pragma**](https://ethglobal.com/events/pragma-sydney) **&** [**ETHGlobal Sydney**](https://ethglobal.com/events/sydney)

- **May 21-23 –** [**DappCon**](https://www.dappcon.io/) **(Berlin)**

- **May 24-26 –** [**ETHBerlin**](https://ethberlin.org/)

- **Jul 8-11 –** [**EthCC**](https://www.ethcc.io/) **(Brussels)**

- **Jul 11-14 –** [**Pragma**](https://ethglobal.com/events/pragma-brussels) **&** [**ETHGlobal Brussels**](https://ethglobal.com/events/brussels)

- **Aug 23-Sep 13 – ETHGlobal** [**ETHOnline**](https://ethglobal.com/events/ethonline2024) **(virtual)**

- **Sep 20-22 –** [**ETHGlobal Singapore**](https://ethglobal.com/events/singapore2024)

- **Oct 15-20 –** [**Pragma**](https://ethglobal.com/events/pragma-sanfrancisco) **&** [**ETHGlobal San Francisco**](https://ethglobal.com/events/sanfrancisco2024)

- **Nov –** [**ETHGlobal DevCon**](https://ethglobal.com/events/devcon2024)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

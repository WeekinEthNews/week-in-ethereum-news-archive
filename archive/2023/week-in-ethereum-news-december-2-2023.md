---
title: "Week in Ethereum News <br> December 2, 2023"
date: "2023-12-01"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=s3jIn3ot57g&t=256s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-123/):
    - [Devnet-12](https://dencun-devnet-12.ethpandaops.io/) launched, likely to run over holidays, Prysm expect to join in ~2 weeks
    
    - Upgrade process discussion: upgrade documents in PM repo, meta EIPs for each upgrade and considered for inclusion (CFI) label

- Dencun interop testing [call video](https://www.youtube.com/watch?v=8EmUgPWbdU4&t=7s)

**Prague + Electra upgrade**

- [Upgrade meta discussion](https://ethereum-magicians.org/t/prague-electra-network-upgrade-meta-thread/16809): community input into which features (EIPs) to include

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 32.28%**](https://dune.com/hildobby/eth2-staking) **increasing towards** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~84% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm 41% & Lighthouse 34%, any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- [Timing games](https://twitter.com/casparschwa/status/1728879324265365752) are bad for Ethereum
    - [P2P.org](https://twitter.com/VladisMint/status/1729447374286688761) (Lido founders) are delaying requests up to 1 second to increase MEV

- Pari (EF DevOps): [how to create a shadow fork](https://notes.ethereum.org/@parithosh/shadowfork-tutorial)

- Verkle implementers [call notes](https://twitter.com/rudolf6_/status/1730191951100825615)

- Guide to [join Verkle testnet](https://hackmd.io/gZP7Yti0Tna3lgZEgammhQ?view) (verkle-gen-devnet-2)

**For Stakers**

- Dappnode [MEV smoothing pool](https://twitter.com/dappnode/status/1730257622744379729) for solo stakers

- [Obol](https://twitter.com/ObolNetwork/status/1722842773735485946) (distributed validators) live, beta, clusters capped at 1 validator

- Lighthouse [user experience survey](https://docs.google.com/forms/d/e/1FAIpQLSdjE83sru5nAxx4M0W-cH4et5X5sBrgjg2_8JszPrwVG-Wa4w/viewform)

**Client releases**

- Consensus layer:
    - Nimbus [v23.11.0](https://github.com/status-im/nimbus-eth2/releases/tag/v23.11.0): Obol enhanced support, improved scoring algorithms to maximize block rewards with multiple beacon nodes, simple bootstrapping and performance improvements for 10k+ validators on a single machine

- Execution layer:
    - Reth [v0.1.0-alpha.12](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.12): support Canyon upgrade on OP Stack networks (not OP mainnet) and fix for pruned node operators

**Research**

- Barnabe: [Liquefaction](https://mirror.xyz/barnabe.eth/v7W2CsSVYW6I_9bbHFDqvqShQ6gTX3weAtwkaVAzAL4), semantics of liquid staking

- [Chipmunk](https://eprint.iacr.org/2023/1820): synchronized lattice-based multi-signature scheme, plausibly secure against quantum attacks

**Layer 2**

- [RollupCodes](https://www.rollup.codes/): opcodes, precompiles & system contracts for each rollup

**EIPs/Standards**

- EIPs
    - Meta [EIP7568](https://github.com/ethereum/EIPs/pull/8005/files): Hardfork meta backfill - Berlin to Shapella
    
    - Meta [EIP7569](https://github.com/ethereum/EIPs/pull/8006/files): Hardfork meta - Dencun

- ERCs (application layer):
    - [ERC7565](https://github.com/ethereum/ERCs/pull/127/files): Perpetual contract NFTs as collateral for liquidity provision
    
    - [ERC7566](https://github.com/ethereum/ERCs/pull/130/files): Multiplayer onchain game
    
    - [ERC7567](https://github.com/ethereum/ERCs/pull/136/files): Splitable utility NFT extension for ERC721

**Stuff for developers**

- Testnets:
    - [Goerli is deprecated](https://blog.ethereum.org/2023/11/30/goerli-lts-update): client teams & EF will exit validators 3 months after upgrading to Dencun (or 1 month after mainnet Dencun upgrade if later)
    
    - [Sepolia](https://github.com/eth-clients/sepolia#readme): use for application layer testing
    
    - [Holešky](https://github.com/eth-clients/holesky#readme): use for staking & infrastructure testing
    
    - [OP testnets migrating](https://blog.oplabs.co/op-sepolia/) to OP Sepolia from OP Goerli

- [OpenZeppelin Contracts wizard](https://twitter.com/openzeppelin/status/1730245437691449838) adds AI assistant to update code & answer questions, alpha 

- [Wake](https://github.com/Ackee-Blockchain/wake#readme) (previously Woke): Python based Solidity dev framework with vulnerability detectors

- [EVMole](https://github.com/cdump/evmole#readme): extract function selectors from bytecode, Python & JavaScript implementations

- [OP Wagmi](https://github.com/base-org/op-wagmi#readme): wagmi v2 style hooks to interact with OP Stack networks

- Coinbase [build onchain apps](https://github.com/coinbase/build-onchain-apps#readme) starter kit: RainbowKit, wagmi, Next.js & Tailwind CSS

- CTFs:
    - [Ethernaut reforged](https://github.com/McCoady/ethernaut-foundry#readme): solve & submit first 8 challenges using just Foundry
    
    - [Curta CTF](https://twitter.com/curta_ctf/status/1730623025685352794) adds writeups

- [Crypto data advent calendar](https://paradigmxyz.github.io/advent-of-crypto-data/): data ecosystem project featured each day

**Security**

- KyberSwap [plan treasury grants](https://twitter.com/kybernetwork/status/1730631569872916534) for affected users
    - [Elastic exploiter](https://twitter.com/pcaversaccio/status/1730205570936832403) demands to take over the company

- Curve [price oracle usage](https://twitter.com/CurveFinance/status/1730111238653288450)

**Ecosystem**

- [~15% of transactions](https://twitter.com/sui414/status/1730375530003009755) via private transaction pools

- Data visualization of [where all ETH sits onchain](https://twitter.com/TrueWaveBreak/status/1729963461407310138)

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 14.7 to 185.0 gwei, with 34.8 gwei average
    - Zero net issuance currently at 21.8 gwei 
    
    - 9.8k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $1,994 - $2,111, currently $2,084

- [ETHBTC](https://ratiogang.com/): currently 0.054 (Flippening at ~0.16)

**Notable at app layer**

- StakeWise [v3](https://stakewise.medium.com/announcing-the-launch-of-stakewise-v3-55effc24dbe4) live on mainnet, marketplace of staking offers, node operators & stakers can mint LSD

- [Paradigm distances itself from Blast](https://twitter.com/danrobinson/status/1728817674543862023) (despite being lead investor twice for this founder)

- [Gitcoin Grants 19](https://gitcoin-grants-51f2c0c12a8e.herokuapp.com/) completed, $600k donated, 45k donors

- [American Cancer Society](https://www.gitcoin.co/blog/american-cancer-society-gitcoin-grants-stack) Gitcoin grants round on Arbitrum

* * *

### Job Listings

- Aragon: [Senior smart contract developer](https://jobs.lever.co/aragon/2f3cf4c4-041a-4978-aa6b-78f447358956) w EIP, auditing experience

- [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db) wanted by EF

- Enya Labs: [Lead Security Engineer](https://enyalabs.applytojob.com/apply/vkSNxMxgCT/Founding-Security-Engineer?source=weekinethereumnews), [Sr. Fullstack Dev](https://enyalabs.applytojob.com/apply/FlzWnQ2S7G/Senior-Full-Stack-Developer?source=weekinethereumnews) (with Go exp), [BizDev](https://enyalabs.applytojob.com/apply/eIiMobirGL/Business-Development?source=weekinethereumnews)

- Nethermind: [Lead Software Engineer](https://grnh.se/e2d52f72teu), [BizDev](https://grnh.se/9fbf4582teu) & [CTO](https://grnh.se/4a264c32teu)

**Job listings: $600 for four issues** (75 character limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Circle denies baseless Elizabeth Warren claims](https://www.circle.com/blog/circle-refutes-false-claims-on-illicit-financing) on illicit financing & banking Justin Sun

- [SIM Swapper](https://www.justice.gov/usao-cdca/pr/sim-swapper-sentenced-eight-years-prison-campaign-fraud-and-deception-including) sentenced to 8 years prison 

**General**

- Vitalik: [techno-optimism](https://vitalik.eth.limo/general/2023/11/27/techno_optimism.html), d/acc (defensive/decentralization/differential acceleration)

- BSC: [bsc-geth bug](https://twitter.com/moo9000/status/1730156814228967901), bsc-erigon unable to sync

- [Polygon POS proposal](https://forum.polygon.technology/t/pip-30-increase-max-code-size-limit-to-32kb/13266) to increase max contract size from 24kb to 32kb

- [Velodrome](https://twitter.com/VelodromeFi/status/1730556643891364269) & [Aerodrome](https://twitter.com/aerodromefi/status/1730557347129348344) domains were compromised in social engineering attack on provider

- [Twitter](https://securityalliance.notion.site/Twitter-Security-Self-Audit-8fdb80d93a144dbab0f0cc4ff59c2131) 15 minute security self-audit

- [BLUFFS](https://francozappa.github.io/post/2023/bluffs-ccs23/): Bluetooth MitM attack reusing a weak session key 

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-2-2023](https://weekinethereumnews.com/week-in-ethereum-news-december-2-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Dec 4 – [ETHVenice](https://ethvenice.com/)

- Dec 6-7 – [Columbia CryptoEconomics workshop](http://columbiacryptoeconomics.org/) (New York)

- Dec 7 – Optimism’s [RetroPGF 3 voting](https://vote.optimism.io/retropgf/3) ends (support [Week in Ethereum News](https://vote.optimism.io/retropgf/3/application/0x44be5b3d06daade4fd7a1c3e1bc9428926befe272b72c16f2d72dce66692af13))

- Dec 7-10 – ETHGlobal [Pragma](https://ethglobal.com/events/pragma-india) & [ETHIndia](https://ethindia.co/) (Bangalore)

- Jan 15 – EF’s [Next Billion fellowship cohort 4](https://fellowship.ethereum.foundation/) deadline

- **Feb 2-4 –** [**ETH Cinco de Mayo**](https://ethcincodemayo.com/) **hackathon (Cholula, Puebla)**

- Feb 23-Mar 3 – [ETHDenver](https://www.ethdenver.com/) BUIDLWeek & hackathon

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024)

- **Mar 21-24 –** [**ETHTaipei**](https://ethtaipei.org/) **conference & hackathon**

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) (virtual)

- **Apr 5-7 –** [**EthereumZuri.ch**](https://ethereumzuri.ch/) **conference & hackathon**

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney)

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/)

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels)

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels)

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) (virtual)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024)

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024)

- Nov – [ETHGlobal DevCon](https://ethglobal.com/events/devcon2024)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

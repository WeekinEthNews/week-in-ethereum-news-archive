---
title: "Week in Ethereum News <br> November 18, 2023"
date: "2023-11-17"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=wSE8e9MZz3k&t=240s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-122/):
    - Blob sidecar inclusion proof: ~2 more weeks to implement
    
    - [Devnet-12](https://notes.ethereum.org/@ethpandaops/dencun-devnet-12) proposed for end of November, no date yet for Goerli
    
    - Péter Szilágyi’s [EL client diversity proposal](https://gist.github.com/karalabe/e106ac58afc1d611641e543312cf41e3): run one client & statelessly cross-validate with other clients

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.41%**](https://twitter.com/lidodominance/status/1725514124002562363) **is still far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~85% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm 43% & Lighthouse 34%, any client bug over 33.3% could mean loss of finality

- [Geographic diversity needed](https://nodewatch.io/), particularly outside of North America & Europe
    - [Ulisse](https://chainbound.grafana.net/public-dashboards/b39ed764b36548a2a74024eab3de2fe3) (geographical distribution of nodes): 3k locations & 11k nodes

**Layer 1**

- [libMEV](https://libmev.com/): MEV searcher data, beta

**Client releases**

- Consensus layer:
    - Teku [v23.11.0](https://github.com/Consensys/teku/releases/tag/23.11.0): added validator duties timing metrics, increased default number of threads for batch signature verification and added checkpoint-sync-url CLI option

- Execution layer:
    - Besu [v23.10.2](https://github.com/hyperledger/besu/releases/tag/23.10.2): upgrades vulnerable dependencies
    
    - Erigon [v2.54.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.54.0)
    
    - Geth [v1.13.5](https://github.com/ethereum/go-ethereum/releases/tag/v1.13.5): fixes potential data corruption in path scheme during power failure

**Layer 2**

- Vitalik: [return of Plasma](https://vitalik.eth.limo/general/2023/11/14/neoplasma.html), extending to the EVM using validity proofs
    - [EVM plasma](https://ethresear.ch/t/discussion-thread-for-evm-plasma-ideas/17429) discussion

- Lattice [Redstone](https://lattice.xyz/media/2023/redstone): Plasma-inspired data availability on top of OP Stack, live on testnet

- L2BEAT [Liveness dashboard](https://l2beat.com/scaling/liveness): display of batch submission & state update intervals and recent anomalies

**EIPs/Standards**

- EIPs
    - [EIP7557](https://github.com/ethereum/EIPs/pull/7968/files): Block-level warming (of addresses & slots with access lists)

- RIPs (Rollup Improvement Proposals)
    - Meta [RIP7559](https://github.com/ethereum/RIPs/pull/2/files): RIP purpose and guidelines
    
    - [RIP7560](https://github.com/ethereum/RIPs/pull/3/files): Native account abstraction

- ERCs (application layer):
    - [ERC7558](https://github.com/ethereum/ERCs/pull/103/files): Batch (lock/unlock) minimal soulbound NFTs (ERC721 extension)
    
    - [ERC7561](https://github.com/ethereum/ERCs/pull/104/files): Simple NFT (subset of ERC721)
    
    - [ERC7562](https://github.com/ethereum/ERCs/pull/105/files): Account abstraction validation scope rules

**Stuff for developers**

- Foundry
    - forge-std [v1.7.2](https://github.com/foundry-rs/forge-std/releases/tag/v1.7.2): new cheat codes: loadAllocs (set state for accounts from JSON), eth\_getLogs & rpc (arbitrary RPC call)

- ENS [EVM Gateway](https://github.com/ensdomains/evmgateway#readme): generic CCIP-Read gateway for reading & verifying data from L2 contracts

- Trail of Bits [roundme](https://github.com/crytic/roundme#roundme): recommends whether an arithmetic operation needs to round up/down

- [EVM Hound](https://github.com/g00dv1n/evm-hound-rs#readme): Rust library to extract potential function selectors from bytecode

- [AI agent demo](https://mirror.xyz/0x16de9a0d10EFc67EF575e72E40FD4a2A826fdEA7/yBj-fWQxrueXNs8jEjUo-Ozu_Nwt04GaXf1D8LjemtM), send transactions on Base using OpenAI & Syndicate

**Security**

- [SEAL crisis handbook](https://docs.google.com/document/d/1DaAiuGFkMEMMiIuvqhePL5aDFGHJ9Ya6D04rdaldqC0): incident response playbook for contract hacks

**Ecosystem**

- EF’s [Next Billion fellowship](https://fellowship.ethereum.foundation/) cohort 4, applications close January 15

- Etherscan [net transfers](https://twitter.com/etherscan/status/1725523199390306754) of a token for each address

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 14.4 to 239.1 gwei, with 33.9 gwei average
    - Zero net issuance currently at 21.8 gwei 
    
    - 9.1k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $1,912 - $2,101, currently $1,961

- [ETHBTC](https://ratiogang.com/): currently 0.054 (Flippening at ~0.16)

**Notable at app layer**

- [ZKP2P](https://docs.zkp2p.xyz/zkp2p/): USD onramp to Base using Venmo, alpha

- Fireblocks [balance verification](https://www.fireblocks.com/blog/fireblocks-research-team-builds-experimental-token-balance-verification-chrome-extension-using-light-client/) Chrome extension, uses Lodestar light client, experimental

- [Gitcoin Grants](https://twitter.com/gitcoin/status/1724780137588346970) matching updated, Passport score of 15 gives 50% match, 25+ gives full match

* * *

### Job Listings

- Enya Labs: [Lead Security Engineer](https://enyalabs.applytojob.com/apply/vkSNxMxgCT/Founding-Security-Engineer?source=weekinethereumnews), [Sr. Fullstack Dev](https://enyalabs.applytojob.com/apply/FlzWnQ2S7G/Senior-Full-Stack-Developer?source=weekinethereumnews) (with Go exp), [BizDev](https://enyalabs.applytojob.com/apply/eIiMobirGL/Business-Development?source=weekinethereumnews)

- Aragon: [Senior smart contract developer](https://jobs.lever.co/aragon/2f3cf4c4-041a-4978-aa6b-78f447358956) w EIP, auditing experience

- Nethermind: [Smart Contract Auditor](https://grnh.se/cf4858b2teu), [Lead Software Engineer](https://grnh.se/e2d52f72teu) & [BizDev](https://grnh.se/9fbf4582teu)

- Gnosis seek [DevRels](https://gnosis.jobs.personio.com/job/1296307?_pc=1517287&display=en), [Senior Web Devs (Wallet)](https://gnosis.jobs.personio.com/job/1239306?_pc=1517287&display=en) & [Backend Devs](https://gnosis.jobs.personio.com/job/1284509?_pc=1517287)

- [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db) wanted by EF

**Job listings:** $600 for four issues (75 character limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities**.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Coinbase-funded [challenge to OFAC's Tornado Cash action](https://twitter.com/iampaulgrewal/status/1724197703616250094) taken to 5th Circuit

- [International Organization of Securities Commissions](https://www.iosco.org/library/pubdocs/pdf/IOSCOPD747.pdf) recommendations for crypto regulation

- [Singapore grants in-principle approval](https://www.mas.gov.sg/news/speeches/2023/shaping-the-financial-ecosystem-of-the-future) for StraitsX SGD & USD and Paxos USD stablecoins

- [Mutant Ape Planet NFT creator](https://www.justice.gov/usao-edny/pr/nonfungible-token-nft-developer-pleads-guilty-international-scheme-defraud-nft) pled guilty for conspiring to commit wire fraud in rug pull

**General**

- [Randstorm: BitcoinJS vulnerability](https://www.unciphered.com/blog/randstorm-you-cant-patch-a-house-of-cards), vulnerable wallets found from 2011-2015

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-november-18-2023](https://weekinethereumnews.com/week-in-ethereum-news-november-18-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Nov 29 – [Gitcoin Grants 19](https://grants.gitcoin.co/#GG19-Rounds) ends **(support** [**Week in Ethereum News**](https://explorer.gitcoin.co/#/round/424/0x98720dd1925d34a2453ebc1f91c9d48e7e89ec29/0x98720dd1925d34a2453ebc1f91c9d48e7e89ec29-246)**)**

- Nov 30 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) deadline (max $1k for local meetups)

- Dec 4 – [ETHVenice](https://ethvenice.com/)

- Dec 6-7 – [Columbia CryptoEconomics workshop](http://columbiacryptoeconomics.org/) (New York)

- **Dec 7 – Optimism’s** [**RetroPGF 3 voting**](https://vote.optimism.io/retropgf/3) **ends (support** [**Week in Ethereum News**](https://vote.optimism.io/retropgf/3/application/0x44be5b3d06daade4fd7a1c3e1bc9428926befe272b72c16f2d72dce66692af13)**)**

- **Dec 7**\-10 – ETHGlobal [**Pragma**](https://ethglobal.com/events/pragma-india) & [ETHIndia](https://ethindia.co/) (Bangalore) 

- **Jan 15 – EF’s** [**Next Billion fellowship cohort 4**](https://fellowship.ethereum.foundation/) **deadline**

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

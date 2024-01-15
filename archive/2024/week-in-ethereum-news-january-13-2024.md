---
title: "Week in Ethereum News <br> January 13, 2024"
date: "2024-01-12"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=YkHtTudq3Xo&t=398s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-125/):
    - **Goerli shadow fork 2**: stable network with blob spamming using Goerli client releases
    
    - **Fork choice filter change:** to be included in Deneb
    
    - **Consensus layer priorities:** discuss next call, [proposed Electra EIPs](https://github.com/ethereum/consensus-specs/issues/3449) & [PeerDAS](https://github.com/ethereum/EIPs/pull/8105/files)

- Dencun interop testing [call video](https://www.youtube.com/watch?v=JSnJo8T16Z4&t=159s)

- [Ephemery testnet](https://ephemery.dev/) upgrades to Dencun January 18

- [Goerli testnet](https://blog.ethereum.org/2024/01/10/goerli-dencun-announcement) upgrades to Dencun January 17
    - Bug bounty doubled for Dencun specific vulnerabilities, up to $500k

**Client releases for Goerli testnet Dencun upgrade**

- Consensus layer:
    - Lighthouse [v4.6.0-rc.0](https://github.com/sigp/lighthouse/releases/tag/v4.6.0-rc.0): pre-release
    
    - Lodestar [v1.14.0-rc.2](https://github.com/ChainSafe/lodestar/releases/tag/v1.14.0-rc.2): pre-release
    
    - Nimbus [v24.1.1](https://github.com/status-im/nimbus-eth2/releases/tag/v24.1.1)
    
    - Prysm [v4.2.0](https://github.com/prysmaticlabs/prysm/releases/tag/v4.2.0)
    
    - Teku [v24.1.0](https://github.com/Consensys/teku/releases/tag/24.1.0)

- Execution layer:
    - Besu [v24.1.0](https://github.com/hyperledger/besu/releases/tag/24.1.0)
    
    - Erigon [v2.56.2](https://github.com/ledgerwatch/erigon/releases/tag/v2.56.2)
    
    - Geth [v1.13.10](https://github.com/ethereum/go-ethereum/releases/tag/v1.13.10)
    
    - Nethermind [v1.25.0](https://github.com/NethermindEth/nethermind/releases/tag/1.25.0): OP Stack Canyon upgrade support
    
    - Reth [v0.1.0-alpha.14](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.14)

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.84%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)
    - [**Social action options**](https://medium.com/@nfett/social-flex-3-options-3788c3dd4b7a) **to tackle a concentrated actor**

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth 84% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm 41%, any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- Increasing gas limit debate:
    - Péter Szilágyi: [need monitoring & metrics](https://twitter.com/peter_szilagyi/status/1745374731824439531) before making a change
    
    - Marius van der Wijden: [risks](https://mariusvanderwijden.github.io/blog/2024/01/11/GasLimit/) include missed block rate, state size, history size, sync times & client diversity
    
    - Ansgar Dietrichs: EIP4844 is equivalent of [~11M additional gas](https://twitter.com/adietrichs/status/1745183445628699129)
    
    - Dankrad Feist: [wait until after Dencun](https://twitter.com/dankrad/status/1745406611202437356), then also increase calldata cost & number of blobs
    
    - Vitalik: [modest increase](https://www.reddit.com/r/ethereum/comments/191kke6/ama_we_are_ef_research_pt_11_10_january_2024/kh7ekx3) is reasonable

- [Besu halted on mainnet](https://wiki.hyperledger.org/pages/viewpage.action?pageId=117440824) January 6, ~70% of Besu nodes impacted, hot fixed

- [Reth state & history growth](https://twitter.com/gakonst/status/1745510516800524406) dashboard

- Nethermind [State Database](https://medium.com/nethermind-eth/nethermind-client-3-experimental-approaches-to-state-database-change-8498e3d89771) experimental approaches: Paprika, Path-Based Storage & Halfpath

- Explainers: [EIP7002](https://ethereum2077.substack.com/p/eip-7002-execution-layer-exits) (execution layer triggerable exits) & [EIP7251](https://ethereum2077.substack.com/p/eip-7251-increase-max-effective-balance) (increase max effective balance)

**Research**

- [EF Research team AMA](https://www.reddit.com/r/ethereum/comments/191kke6/ama_we_are_ef_research_pt_11_10_january_2024/), discussions include: EIP4844 data publishing without scaling, composability across rollups, Lido, security budget, capping signatures to 8192 per slot, gas limit increase, native (enshrined) rollups, EigenLayer, MEV burn & EIP7251 (increase max effective balance)

- Staking economics: [issuance impact on staking equilibrium](https://notes.ethereum.org/@anderselowsson/HyUIqjo_6) & reward curve options

**MEV**

- Proposals for [relay incentivization](https://ethresear.ch/t/analyzing-missed-slot-through-the-lens-of-relays-a-potential-path-for-relay-incentivization/18257): low-latency relay mesh network and enshrining missed slot penalty on proposers

**Layer 2**

- OP Stack [Canyon upgrade](https://docs.optimism.io/builders/node-operators/network-upgrades/canyon) live on Superchain mainnets, adds Shappella support (including PUSH0), reduces rate of basefee change & adds Create2Deployer

- RollCall (L2 standards) [video](https://www.youtube.com/watch?v=0OzjiHf2dF0&t=2s) & [notes](https://twitter.com/CarlBeek/status/1745472647356387704): RIP7212 (R1 precompile) made final, EIP7587 (reserve RIP precompile addresses) discussion and RIP working groups (precompiles, EIP4844 testing & fee markets)

**EIPs/Standards**

- EIPs
    - [EIP7591](https://github.com/ethereum/EIPs/pull/8102/files): BLS signed transactions
    
    - [EIP7592](https://github.com/ethereum/EIPs/pull/8103/files): Precompile for Falcon signature verification
    
    - [EIP7594](https://github.com/ethereum/EIPs/pull/8105/files): PeerDAS (peer data availability sampling)

- ERCs (application layer):
    - [ERC7589](https://github.com/ethereum/ERCs/pull/186/files): Semi-fungible token roles
    
    - [ERC7590](https://eips.ethereum.org/EIPS/eip-7590): ERC20 holder extension for NFTs
    
    - [ERC7593](https://github.com/ethereum/ERCs/pull/196/files): NFT synthetic evidence

**Stuff for developers**

- Remix [v0.40.0](https://medium.com/remix-ide/remix-release-v0-40-0-17668192db64): Ape framework Vyper compiler, Uniswap v4 templates & Circom v2.1.6

- [GasliteNFT](https://github.com/PopPunkLLC/gaslite-core/blob/main/src/GasliteNFT.sol) (ERC721 base contract): extends ERC721A with Ownable2Step & MerkeProofLib

- RareSkills: [Compound v3 explainer](https://www.rareskills.io/compound-v3-book)

- [Equivalence checking](https://twitter.com/daejunpark/status/1744788041078829432) with Halmos

- [Evm-inspectors](https://github.com/paradigmxyz/evm-inspectors): Revm Inspectors for Parity & Geth style traces and JS Inspector

- Wevm [Vocs](https://vocs.dev/): React-based static documentation generator, content in Markdown or MDX

**Security**

- Wise Lending [~177 ETH exploit](https://twitter.com/peckshield/status/1745907642118123774) via precision issue

- Behind the scenes of [Euler March 2023 exploit](https://www.euler.finance/blog/war-peace-behind-the-scenes-of-eulers-240m-exploit-recovery) & fund recovery

**Ecosystem**

- Optimism’s [RetroPGF round 3 results](https://optimism.mirror.xyz/37Bgum6MfTJWDuE41CH9RXSH5KBm_RCL5zsSFeRZl4E), 30M OP allocated to 501 builders & creators

**Enterprise**

- [Unicef Rwanda](https://twitter.com/unicefrw/status/1742893650730996077) using staking to fund school internet connectivity

- [X (Twitter)](https://techcrunch.com/2024/01/10/x-removes-support-for-nft-profile-pictures/) removed NFT profile picture support

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 9.2 to 483.5 gwei, with 26.2 gwei average
    - Zero net issuance currently at 21.9 gwei 
    
    - 3.2k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,185 - $2,698, currently $2,497

- [ETHBTC](https://ratiogang.com/): currently 0.06 (Flippening at ~0.16)

**Notable at app layer**

- USDC & EURC [v2.2](https://twitter.com/jerallaire/status/1745543903686660419) upgrade complete: reduces gas costs & supports ERC1271

- OpenSea [email onboarding](https://opensea.io/blog/articles/opensea-new-onboarding-experience): create non-custodial wallet via email address using Privy

- Simon de la Rouviere [See You There](https://blog.simondlr.com/posts/see-you-there): 1 of 1 NFT, records holders over 5 years

- [Speedtracer](https://mirror.xyz/sammybauch.eth/K_L1dAMiUc57lOSFBFrHRrSGmwPNy97kE2yYJ8O3Yro) (daily mini game) live on Base, trace a race track & mint highest score

* * *

### Job Listings

- Status is hiring: Technical Chief Operating Officer - [Apply here](https://grnh.se/0ecdaa981us)

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [SEC](https://www.sec.gov/news/statement/gensler-statement-spot-bitcoin-011023) approves BTC ETFs
    - [Commissioner Peirce](https://www.sec.gov/news/statement/peirce-statement-spot-bitcoin-011023): “squandered a decade of opportunities”
    
    - [SEC Twitter account](https://twitter.com/garygensler/status/1744833049064288387) was compromised [via a phone number](https://twitter.com/Safety/status/1744924042681897343) without 2FA

- [Circle](https://www.reuters.com/markets/deals/stablecoin-firm-circle-confidentially-files-us-ipo-2024-01-11/) filed for IPO

- [New York DFS](https://www.dfs.ny.gov/reports_and_publications/press_releases/pr2024011224) settles with Genesis for compliance failures, $8M penalty & cease operations in the state

**General**

- Columbia CryptoEconomics workshop [videos](https://www.youtube.com/playlist?list=PLpktWkixc1gX-L5NT-vuDP54kW--3gDnK)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-january-13-2024](https://weekinethereumnews.com/week-in-ethereum-news-january-13-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jan 15 – EF’s [Next Billion fellowship cohort 4](https://fellowship.ethereum.foundation/) deadline

- Jan 17 – [Goerli testnet](https://eips.ethereum.org/EIPS/eip-7569#activation) Dencun upgrade epoch 231680, [**livestream**](https://www.youtube.com/watch?v=jbhFdUFnWUU)

- Jan 30 – [Sepolia testnet](https://eips.ethereum.org/EIPS/eip-7569#activation) Dencun upgrade epoch 132608 (assuming no issues)

- Feb 2-4 – [ETH Cinco de Mayo](https://ethcincodemayo.com/) hackathon (Cholula, Puebla)

- Feb 3 – [Ethereum Lima Day](https://ethlimaday.org/)

- Feb 7 – [Holešky testnet](https://eips.ethereum.org/EIPS/eip-7569#activation) Dencun upgrade epoch 29696 (assuming no issues)

- Feb 23-Mar 3 – [ETHDenver](https://www.ethdenver.com/) BUIDLWeek & hackathon

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024) hackathon

- Mar 19-21 – [ETH Canal](http://ethcanal.xyz) (Panama City, Panamá) conference & hackathon

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) hackathon & conference 

- Mar 29-31 – [ETH Seoul](https://www.ethseoul.org/) conference

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) virtual hackathon

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Apr 12-14 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/)

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- Jun 3-5 – [ETH Belgrade](https://ethbelgrade.rs/) conference

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 26-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

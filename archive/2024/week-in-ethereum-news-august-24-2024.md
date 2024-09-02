---
title: "Week in Ethereum News <br> August 24, 2024"
date: "2024-08-24"
---

## Eth News and Links

Eight years of Week in Ethereum News

**All core devs**

- [All Core Devs - Consensus (ACDC) #140](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-140-august-22-2024/20768):
    - Pectra (Prague + Electra) upgrade:
        - [**Pectra-devnet-2**](https://pectra-devnet-2.ethpandaops.io/): client teams debugging issues including a few bad blocks, currently not finalizing
        
        - **Pectra-devnet-3**: plan to launch next week
        
        - **EIP7251 max effective balance**: correlation penalty update, fixes overflow
        
        - **EIP7594 PeerDAS**:
            - **EIP7742 uncouple blob count between CL & EL**: general support for including in Pectra
            
            - Blob limits per transaction discussion
    
    - **Fulu** named as next consensus layer upgrade and **Fusaka** (Fulu + Osaka) for combined upgrade
    
    - Probelab: Gossipsub analysis

[**Pectra**](https://eips.ethereum.org/EIPS/eip-7600) **(Prague + Electra) upgrade**

- [Pectra testing call #1](https://ethereum-magicians.org/t/pectra-testing-call-19-august-2024/20846)

- Consensus specs [v1.5.0-alpha.5](https://github.com/ethereum/consensus-specs/releases/tag/v1.5.0-alpha.5): target for peerdas-devnet-2

- [PeerDAS breakout #6](https://ethereum-magicians.org/t/peerdas-breakout-6-august-20-2024/20838):
    - Peerdas-devnet-2: launch in the next week
    
    - Peerdas-devnet-3: rebase to Pectra, launch in 2-3 weeks

- [EOF Implementers call #56](https://ethereum-magicians.org/t/eof-implementers-call-56-aug-21-2024/20853):
    - [Frangio](https://hackmd.io/@frangio/S1VvatXiR): ERC721/1155 need ISCONTRACT and upgradeable proxies could be bricked by EOF contracts not able to DELEGATECALL a legacy contract

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 28.6%**](https://dune.com/hildobby/eth2-staking)**, still too close to** [**33.3% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: **Geth ~52% majority** ([Lido reduced Geth usage by 20% in Q2](https://app.hex.tech/8dedcd99-17f4-49d8-944e-4857a355b90a/app/3f7d6967-3ef6-4e69-8f7b-d02d903f045b/latest?tab=client-diversity#execution-layer))
    
    - Consensus layer: Prysm 36%
    
    - Any client bug over 33.3% could mean loss of finality

- Better [geographic diversity](https://nodewatch.io/) is optimal, particularly outside of North America & Europe

**Layer 1**

- Toni Wahrstätter:
    - [Timing games economies of scale](https://ethresear.ch/t/on-proposer-timing-games-and-economies-of-scale/20309), 30% validator share can delay 0.8s longer than 5% share
    
    - [Reorgs analysis](https://x.com/nero_eth/status/1825849806314422535): trending down, mostly occurring in slot following epoch transitions

- [Xatu consensus layer p2p tables](https://ethpandaops.io/posts/xatu-consensus-layer-p2p/): libp2p gossipsub beacon attestation, beacon block & blob sidecar

- Nethermind: [execution layer client performance](https://nethermind.notion.site/MGas-s-performance-research-across-different-Execution-Layers-1d494e98b431425c878d5a82c63413b1) via engine\_NewPayload response times

- [ePBS p2p market](https://ethresear.ch/t/the-role-of-the-p2p-market-in-epbs/20330): allows small builders to participate in the market

**Client Releases**

- Consensus layer:
    - Prysm [v5.1.0](https://github.com/prysmaticlabs/prysm/releases/tag/v5.1.0): bug fixes, remote signer public key persistence and experimental support for multiple beacon nodes

- Execution layer:
    - Besu [v24.8.0](https://github.com/hyperledger/besu/releases/tag/24.8.0): stack handling update & RPC service improvements

**For Stakers**

- Somer Esat’s [staking guides](https://github.com/SomerEsat/ethereum-staking-guides#readme) updated to add Reth execution layer client

**Layer 2**

- [Offchain Labs roadmap](https://medium.com/offchainlabs/your-chain-your-rules-offchain-labs-technical-roadmap-to-fuel-arbitrum-innovation-f787f2e85966): Stylus, BoLD, censorship timeout, decentralized sequencer, fast withdrawals, chain clusters, multi client support, adaptive pricing and zk hybrid proving

- L2Beat [optimistic rollup fraud proofs](https://medium.com/l2beat/fraud-proof-wars-b0cb4d0f452a), comparing Arbitrum, Cartesi & Optimism

**EIPs/Standards**

- RIPs (Rollup improvement proposals):
    - [RIP7759](https://github.com/ethereum/RIPs/pull/36/files): Layer 2 transaction fees

- ERCs (application layer standards):
    - [ERC7757](https://github.com/ethereum/ERCs/pull/596/files): Instinct-based automatic transactions
    
    - [ERC7758](https://github.com/ethereum/ERCs/pull/598/files): Transfer with authorization (ERC3009 update)
    
    - [ERC7760](https://github.com/ethereum/ERCs/pull/604/files): Minimal upgradeable proxies

**Stuff for developers**

- [Hardhat roadmap](https://blog.nomic.foundation/rust-powered-hardhat-present-future/): OP Stack simulation & Solidity tests in v3, followed by portability via WASM, external EDR API, improved Solidity debugging and simulation of more L2s  

- Remix [v0.53.0](https://medium.com/remix-ide/remix-release-v0-53-0-615d9e7c6c58): generate proofs in Circom compiler plugin

- [SOLX](https://github.com/ZeroEkkusu/solx#readme): transpile TypeScript to Solidity in Foundry tests & scripts

- web3.py [v7](https://snakecharmers.ethereum.org/web3-py-v7-release-announcement/): redesigned WebSocketProvider & new AsyncIPCProvider with subscriptions, class based middleware, batch requests and more ABI utility methods

- [Brontes](https://github.com/SorellaLabs/brontes#readme): analytics pipeline to identify MEV, built on Reth

- [Noble-post-quantum](https://github.com/paulmillr/noble-post-quantum#readme) (JavaScript): implements final FIPS 203/204/205 specs

- CTFs:
    - 5/9 [Tardis](https://github.com/fiveoutofnine/tardis#readme): past Curta CTFs to play locally

- Scaffold-ETH 2 [extensions hackathon](https://extensions.buidlguidl.com/), submit by September 2

**Security**

- Whale [$55M phishing attack](https://rekt.news/whale-hunters-payday/), ownership of Maker vault changed

**Ecosystem**

- Vitalik: [fundamentals](https://x.com/VitalikButerin/status/1826506920393355347) are actually crazy strong right now

- Etherscan [token standard checker](https://etherscan.io/tokentracker): check if contract is ERC20/721/1155 compliant

- [Ethereum Uruguay](https://taikai.network/ethuruguay/hackathons/buildathon-2024/projects) hackathon projects

**Enterprise**

- Sony Block Solutions Labs (Sony joint venture) [Soneium](https://soneium.org/en/blog/introducing-soneium-by-sony-block-solutions-labs-for-the-future-of-web3/): planned OP Stack rollup 

- [State Street](https://newsroom.statestreet.com/press-releases/press-release-details/2024/State-Street-Announces-Agreement-with-Taurus-to-Deliver-Full-Service-Digital-Platform-for-Institutional-Investors/default.aspx) partner with Taurus to provide digital asset products to institutional investors

* * *

### Job Listings

- [Sablier](https://sablier.notion.site/Careers-at-Sablier-d3771d8eefbf44a8a8428436fb950a1d) are hiring a Business Development Lead and Frontend Engineer

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Fees (via [ultrasound.money](https://ultrasound.money)):
    - Gas: 0.6 to 27.2 gwei, 1.5 gwei average; zero net issuance at 23.9 gwei 
    
    - 17k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,565 - $2,797, currently $2,767, all time high $4,878

- [ETHBTC](https://www.coingecko.com/en/coins/ethereum/btc): currently 0.043

**Regulation/business/tokens**

- [US Treasury](https://x.com/KMSmithDC/status/1825695802578076092) removed unhosted wallet rule

- Coindesk: [token theater](https://www.coindesk.com/policy/2024/08/21/crypto-airdrops-ban-us-users-but-americans-are-claiming-tokens-anyway), US employees claimed geoblocked airdrops 

- [Prometheum](https://www.coindesk.com/policy/2024/08/21/controversial-crypto-firm-prometheum-to-treat-uniswap-and-arbitrums-tokens-as-securities) (Gensler favorite) plans to treat UNI & ARB as securities in custody service

**General**

- Vitalik: [plurality philosophy](https://vitalik.eth.limo/general/2024/08/21/plurality.html)

- 🎂 [Eight year anniversary](https://weekinethereumnews.com/week-in-ethereum-news-august-21-2016/) of Week in Ethereum News

* * *

**END OF SERVICE:** plan to [deprecate Week in Ethereum News](https://twitter.com/evan_van_ness/status/1760828369107574872)

Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-august-24-2024](https://weekinethereumnews.com/week-in-ethereum-news-august-24-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Aug 29-31 – [ETHAccra](https://ethaccra.xyz) hackathon

- Aug 31 – [Underhanded Solidity contest](https://soliditylang.org/blog/2024/07/31/underhanded-solidity-contest-2024-announcement/) deadline

- **Sep 2 – Scaffold-ETH 2** [**extensions hackathon**](https://extensions.buidlguidl.com/) **deadline**

- Sep 5-8 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 9-15 – [ETHSafari](https://ethsafari.xyz/) (Kenya)

- Sep 12-14 – [NapulETH](https://napul.eth.limo/) (Napoli)

- Sep 13-14 – [Ethereum México](https://ethmexico.org/)

- Sep 20-22 – [ETHCapeTown](https://www.ethcapetown.com/) hackathon

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Sep 26-27 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 4-6 – [Ethereum Kuala Lumpur](https://www.2024.ethkl.org/) conference & hackathon

- Oct 4-6 – [ETHRome](https://ethrome.org/) hackathon

- Oct 17-19 – [ETHSofia](https://www.ethsofia.com/) conference & hackathon

- Oct 17-20 – [ETHLisbon](https://ethlisbon.org/) hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

- Dec 6-8 – [ETHIndia](https://ethindia.co/) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

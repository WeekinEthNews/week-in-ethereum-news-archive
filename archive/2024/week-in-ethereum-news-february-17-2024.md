---
title: "Week in Ethereum News <br> February 17, 2024"
date: "2024-02-16"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=UTgnbE6jTuE&t=156s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1758202852005331339) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-181/):
    - **Dencun upgrade** client releases expected next week, followed by a mainnet shadow fork
    
    - **Retroactive EIP proposals**: EIP7610 (revert contract creation for non-empty storage) need to discuss Verkle interaction and EIP7523 (deprecate empty accounts) need to verify no empty accounts
    
    - **Pectra upgrade** (small fork targeting late 2024)
        - Discussions on potential EIPs:
            - EIP5806 (delegate transaction), alternative to EIP3074
            
            - EIP7557 (block-level warming)
            
            - EIP2935 (historical block hashes in state) updated for Verkle
            
            - EIP5920 (PAY opcode)
            
            - EIP7609 (decrease TLOAD/TSTORE base cost)
        
        - Agreed to include EIP2537 (BLS precompile)

- consensus-specs [v1.4.0-beta.7](https://github.com/ethereum/consensus-specs/releases/tag/v1.4.0-beta.7): schedule mainnet Dencun upgrade

**Osaka upgrade (meta** [**EIP7607**](https://eips.ethereum.org/EIPS/eip-7607)**)**

- Verkle implementers [call video](https://www.youtube.com/watch?v=rwpNQ8VBDwg&t=4s) & [notes](https://twitter.com/rudolf6_/status/1757355851982241895): updates from client teams & testing team, EIP2935 updated, new EIP7612 and deprecating serialize commitment

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 31.69%**](https://dune.com/hildobby/eth2-staking) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: **Geth 69%** supermajority, could cause a chain split
        - [**Lido’s use of supermajority client**](https://app.hex.tech/8dedcd99-17f4-49d8-944e-4857a355b90a/app/3f7d6967-3ef6-4e69-8f7b-d02d903f045b/latest?selectedStaticCellId=240dc734-931e-46e4-946a-89413b0abd8e) continues to put Ethereum at risk
        
        - [Supermajority dashboard](https://supermajority.info/): simulate Lido operators changing to minority clients
    
    - Consensus layer: **Prysm 38%**, any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- [Local shadowforks](https://twitter.com/parithosh_j/status/1757099658143318322) with single line command using Kurtosis over Docker or Kubernetes

- [Erb (blob archive files)](https://github.com/status-im/nimbus-eth2/pull/5882) design decisions, store blobs alongside Era archive files

- Inclusion list breakout [call video](https://www.youtube.com/watch?v=LhZSunC8Epw&t=5s) & notes from [Terence](https://twitter.com/terencechain/status/1758515062845886749)

**ePBS (enshrined Proposer-Builder Separation)**

- ePBS breakout [call video](https://www.youtube.com/watch?v=63juNVzd1P4&t=140s) & notes from [Terence](https://gist.github.com/terencechain/1f883342b99a910e979805bb034043f9)

- Terence: [minimal ePBS Beacon chain changes](https://ethresear.ch/t/minimal-epbs-beacon-chain-changes/18653)

- Francesco: options to [harden PBS](https://ethresear.ch/t/paths-to-hardening-pbs/18666) without full enshrinement

**MEV**

- [MMASim](https://github.com/M1kuW1ll/MMASim#readme): MEV-Boost auction simulation framework

- [predictive MEV-burn](https://ethresear.ch/t/the-price-is-right-realigning-proposer-builder-incentives-with-predictive-mev-burn/18656): proposal to incentivize builders to predict a blocks value

- [Leaderless auctions](https://twitter.com/_dave__white_/status/1757471352897122672): decentralized MEV-resistant auction with no auctioneer

**Research**

- Barnabe: [rainbow staking](https://ethresear.ch/t/unbundling-staking-towards-rainbow-staking/18683), framework for protocol service providers (professional operators & solo stakers) to participate in spectrum of heavy (slashable) & light (non/partially slashable) services

**For stakers**

- [Blobs use max 103 GiB](https://twitter.com/ethstaker/status/1757421243698176395) (average 50 GiB) plus the [blob pool](https://twitter.com/parithosh_j/status/1757658302555586775)

**Client releases**

- Consensus layer:
    - Teku [v24.2.0](https://github.com/Consensys/teku/releases/tag/24.2.0): mainnet Dencun upgrade

- Execution layer:
    - Besu [v24.1.2](https://github.com/hyperledger/besu/releases/tag/24.1.2): mainnet Dencun upgrade
    
    - Nethermind [v1.25.4](https://github.com/NethermindEth/nethermind/releases/tag/1.25.4): mainnet Dencun upgrade
    
    - Reth [v0.1.0-alpha.18](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.18): mainnet Dencun upgrade and trie performance improvements

* * *

### **Support the** [**Roman Storm & Alex Pertsev legal defense fund**](https://juicebox.money/@free-pertsev-and-storm)

![Open source is not a crime](https://weekinethereumnews.com/wp-content/uploads/2024/01/open-source-is-not-a-crime-1024x341.jpg)

The Biden administration is attempting to criminalize open source software development as part of its war on crypto.

**The fundraiser ends THIS WEEK.** Donate to [defend our innocent Ethereum heroes](https://juicebox.money/@free-pertsev-and-storm).  

* * *

**Layer 2**

- Ed Felten: [blobs explainer for L2 users](https://medium.com/offchainlabs/eip-4844-what-does-it-mean-for-l2-users-5e86ebc4c028), transactions will be cheaper (unknown by how much)

- RollCall (L2 standards) [call video](https://www.youtube.com/watch?v=rwDpX08PiXQ&t=3s) and [notes](https://github.com/ethereum/pm/issues/944#issuecomment-1947556305): L2s generally plan to use blobs soon after Dencun upgrade, recap of breakout calls and proposed RIP7614 (expose call stack to contracts)

- Based rollups:
    - Sequencing & pre-confirmations call [video](https://www.youtube.com/watch?v=2IK136vz-PM)
    
    - Justin Drake answers [shared sequencing concerns](https://twitter.com/drakefjustin/status/1757348299529437509)

- [Starknet airdrop](https://medium.com/@StarknetFoundation/introducing-the-starknet-provisions-program-05d03ce13970) claimable from Feb 20, includes pre-Merge stakers, Protocol Guild, EIP/ERC authors and contributors to Ethereum repos, US not eligible

- [ApeChain](https://twitter.com/yugalabs/status/1757961449664909380) to use Arbitrum

**EIPs/Standards**

- EIPs:
    - [EIP7620](https://github.com/ethereum/EIPs/pull/8209/files): EOF - Contract creation instructions
    
    - [EIP7623](https://eips.ethereum.org/EIPS/eip-7623): Increase calldata cost

- ERCs (application layer):
    - [ERC7621](https://github.com/ethereum/ERCs/pull/251/files): Basket token
    
    - [ERC7622](https://github.com/ethereum/ERCs/pull/252/files): Pre-authorized service payment protocol
    
    - [ERC7624](https://github.com/ethereum/ERCs/pull/260/files): Dynamic identity binding soulbound tokens

**Stuff for developers**

- Foundry:
    - [test & trace performance improvements](https://twitter.com/danipopes/status/1758277127047397478), forge test up to 6x faster
    
    - [Sphinx](https://twitter.com/sphinxdeploy/status/1758174384408207658): DevOps platform to deploy & manage contracts

- Hardhat:
    - [v2.20.0](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.20.0): adds Cancun support (enable in config), blob transactions not yet supported
    
    - [Account Abstraction plugin](https://github.com/defi-wonderland/hardhat-account-abstraction#readme): send sponsored transactions on testnets

- Remix [v0.43.0](https://medium.com/remix-ide/remix-release-v0-43-0-1150e59a81df): adds tool icons on hover in the file explorer, Vyper compiler displays errors in cards and plugins from external teams have warning icon

- VSCode Solidity Inspector [v1.3](https://twitter.com/0xasp_/status/1757102924595974519) adds inline file import suggestions with Foundry remapping support

- [DN404](https://github.com/Vectorized/dn404#readme) (Solidity contract): hybrid ERC20 & ERC721, mints/burns NFTs based on ERC20 balance

- [Intents Engine](https://github.com/NaniDAO/ie#readme): natural language command interface for contracts

- [Czip](https://github.com/0xsequence/czip#readme): calldata compression/decompression in Huff

- Slitherin (custom Slither detectors) [v0.6](https://github.com/pessimistic-io/slitherin/releases/tag/v0.6.0): adds arithmetic overflow detector & Arbitrum detectors

- Sourcify: [finding auxdata in bytecode](https://docs.sourcify.dev/blog/finding-auxdatas-in-bytecode/) for partial source code verification

- [Vyper JupyterLab & Google Colab integration](https://medium.com/@daniel.schiavini/using-your-browser-wallets-network-from-vyper-263e7a46b38b) updated to use browser wallet network directly

- RainbowKit [v2](https://twitter.com/rainbowdotme/status/1757886864823066669): EIP6963 support, wagmi v2, multiple wallet connection sessions and TanStack Query support

- TrueBlocks [Key](https://key.trueblocks.io/): index API, beta

- OpenZeppelin [Ethernaut CTF](https://ctf.openzeppelin.com/) March 16-17

**Security**

- [Security Alliance](https://securityalliance.notion.site/Introducing-the-Security-Alliance-e07c85364140440cb4911a5737461648) (SEAL): draft [whitehat Safe Harbor framework](https://github.com/security-alliance/safe-harbor#readme)

**Ecosystem**

- Mike Neuder & Alex Stokes: [rollup-centric roadmap](https://notes.ethereum.org/@mikeneuder/rcr2vmsvftv)

- Data visualization of [Optimism RetroPGF3 ballots](https://mirror.xyz/cerv1.eth/oAt9piKwPz8cUD_a8lcx2hl-DCLBm1QoGpxDgPFDsB8)

* * *

### Job Listings

- MetaMask Staking: [Staff Software Engineer](https://grnh.se/533bf5521us) and [Software Engineer](https://grnh.se/7efeff9b1us)

- Solidity: [C++ Software Engineer](https://jobs.lever.co/ethereumfoundation/a6e4598e-6c12-493e-8426-438cb0a5eeca) and [Programming Language Researcher](https://jobs.lever.co/ethereumfoundation/d510dfd7-d5dd-435c-9111-1c50112715c1)

- EF seek an [Executive Assistant](https://jobs.lever.co/ethereumfoundation/444bc50a-236e-4a4e-8385-c0454b0044e9) to support senior decision makers

- Sourcify seek a [TypeScript Developer](https://jobs.lever.co/ethereumfoundation/fbcb2cf8-cd58-4140-ab3a-47a402616d50)

**Job listings: $600 for 4 issues** (75 char limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 13.2 to 477.5 gwei, with 34.9 gwei average
    - Zero net issuance currently at 22.3 gwei 
    
    - 6.9k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,476 - $2,859, currently $2,798

- [ETHBTC](https://ratiogang.com/): currently 0.054 (Flippening at ~0.16)

**Notable at app layer**

- Uniswap [v4](https://twitter.com/uniswapfnd/status/1758146187318669666) planned for Q3

- ENS [eth.link](https://discuss.ens.domains/t/ep5-x-social-determine-ens-labs-next-steps-in-eth-link-litigation/18756) $300k settlement offer by Manifold Finance

- Onthis [USDC shortcuts](https://twitter.com/onthisxyz/status/1757442030802764181): send to ENS shortcut to bridge to L2

- Superfluid [distribution pools](https://twitter.com/superfluid_hq/status/1758524506531078409): one to many streams

- Privacy & Scaling Explorations: [Anon Aadhaar v1  
    ](https://mirror.xyz/privacy-scaling-explorations.eth/YnqHAxpjoWl4e_K2opKPN4OAy5EU4sIJYYYHFCjkNOE)

**General**

- [GoFundMe](https://twitter.com/FreeAlexeyRoman/status/1757873646440186039) canceled Roman Storm & Alex Pertsev fundraiser, [donate using crypto](https://juicebox.money/@free-pertsev-and-storm)

- [Breaking BFT](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4727999): total cost of attack estimated at $34B for Ethereum & $5-22B for Bitcoin

- [Skiff](https://skiff.com/data-migration) sunsetting products, acquired by Notion

- Polygon PoS [log parsing vulnerability disclosed](https://www.asymmetric.re/blog/polygon-log-confusion), patched

- [FRIDA](https://eprint.iacr.org/2024/248): data availability sampling from FRI

* * *

Publisher & Founder: [@evan van ness](https://twitter.com/evan_van_ness); Editor: [@abcoathup  
](https://twitter.com/abcoathup)Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) for the most clicked links  
Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-february-17-2024](https://weekinethereumnews.com/week-in-ethereum-news-february-17-2024)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Feb 19 – [Ethereum Protocol Fellowship study group](https://blog.ethereum.org/2024/02/07/epf-study-group) 10 week series starts

- Feb 23-Mar 3 – [ETHDenver](https://www.ethdenver.com/) BUIDLWeek & hackathon

- Mar 4 – [EF academic grants round](https://esp.ethereum.foundation/academic-grants) application deadline

- Mar 13 – [mainnet Dencun upgrade](https://eips.ethereum.org/EIPS/eip-7569#activation) epoch [269568](https://beaconcha.in/epoch/269568)

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024) hackathon

- Mar 19-21 – [ETH Canal](http://ethcanal.xyz) (Panama City, Panamá) conference & hackathon

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- Mar 22-24 – [ETHSamba](https://ethsamba.org/) (Rio)

- Mar 27-30 – [ETH Bucharest](https://www.ethbucharest.xyz/) conference & hackathon

- Mar 29-31 – [ETH Seoul](https://www.ethseoul.org/) hackathon

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) virtual hackathon

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference

- Apr 12-14 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- Apr 16-18 – [EY Global blockchain summit](https://web.cvent.com/event/e0ad2c12-3e65-41a9-bafb-a436754cf4ae/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7) (London)

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney) hackathon

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/) hackathon

- May 31-Jun 2 – [ETHDublin](https://ethdublin.io/) hackathon & conference

- May 31-Jun 2 – [ETHPrague](https://ethprague.com) conference & hackathon

- Jun 3-5 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels) conference

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels) hackathon

- Jul 26-30 – [EDCON Tokyo](https://www.edcon.io/) conference 

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) virtual hackathon

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024) hackathon

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024) hackathon

- Nov 12-15 – [Devcon 7 - Southeast Asia](https://devcon.org/) (Bangkok)

- Nov 15-17 – [ETHGlobal Bangkok](https://ethglobal.com/events/bangkok) hackathon

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

---
title: "Week in Ethereum News <br> February 18, 2023"
date: "2023-02-18"
---

## Eth News and Links

**Shapella (Shanghai + Capella) upgrade**

- Latest all core devs - execution (ACDE) [call video](https://www.youtube.com/watch?v=GmwEa_HI2lE&t=20s). Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1626258565035081728) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-execution-call-155/):
    - Empty block handling bug found on Zhejiang testnet, since patched by Geth, doesn’t impact Sepolia testnet upgrade timeline
    
    - withdrawal-devnet-7: upgraded to Shapella with 600k validators and 360k BLS changes, only stopped finalizing for 1 epoch in a harsher setup than mainnet
    
    - withdrawal-mainnet-shadowfork-2 to test MEV-Boost
    
    - 0 blob EIP4844 transactions banned for now
    
    - Discussions on SSZ in block header, CL minimal presets (test configs), standardizing transaction pool API and approach to deprecate SELFDESTRUCT

- builder-specs [v0.3.0](https://github.com/ethereum/builder-specs/releases/tag/v0.3.0): add Capella support

**Dencun (Cancun + Deneb) upgrade**

- KZG Ceremony:
    - [47,000+ contributors](https://ceremony.ethereum.org/), 4000+ in the lobby, 23 days left in _first_ general contribution period
    
    - [Coinbase](https://twitter.com/jessepollak/status/1624481409933930496) adds call to action to their products

- Latest EIP4844 implementers [call video](https://www.youtube.com/watch?v=poTKRryqrzU&t=4s). Notes from [Terence](https://twitter.com/terencechain/status/1625566598294835200): blobs to be decoupled from blocks

- SSZ breakout [video call](https://www.youtube.com/watch?v=T5aMpivk-Gw&t=5s): discussion on Union vs normalized transaction representation, plan to prototype in next 2 weeks to decide approach to take

**Layer 1**

- Visualization of [MEV-boost block flow](https://nerolation.github.io/mevflow.html) from builder to validator via relayer

- Flashbots: [design for MEV-Share](https://collective.flashbots.net/t/mev-share-programmably-private-orderflow-to-share-mev-with-users/1264), users send transactions to a matchmaker to match with searchers who pay users for using their transactions 

**Client releases**

- Consensus layer:
    - Lodestar [v1.4.3](https://github.com/ChainSafe/lodestar/releases/tag/v1.4.3): Zhejiang testnet support, fix for dropping peers
    
    - Prysm [v3.2.1](https://github.com/prysmaticlabs/prysm/releases/tag/v3.2.1): Capella upgrade for Sepolia testnet
    
    - Teku [v23.2.0](https://github.com/ConsenSys/teku/releases/tag/23.2.0): early access to doppelganger detection and Capella upgrade for Sepolia testnet

- Execution layer:
    - Besu [v23.1.0](https://github.com/hyperledger/besu-docs/releases/tag/23.1.0): move to Java 17 LTS, performance improvements & Bonsai robustness
    
    - Geth [v1.11.0](https://github.com/ethereum/go-ethereum/releases/tag/v1.11.0): Shanghai upgrade support, added Pebble database as LevelDB replacement (requires resync), removed puppeth & mobile development libraries and deprecated personal RPC namespace; [v1.11.1](https://github.com/ethereum/go-ethereum/releases/tag/v1.11.1): patch for empty block processing in Shanghai upgrade
    
    - Nethermind [v1.17.0](https://github.com/NethermindEth/nethermind/releases/tag/1.17.0): Shanghai upgrade for Sepolia testnet & performance improvements

**Research**

- [Censorship resistance](https://iyusufali.xyz/writings/inclusion-lists) using delayed reveal, forward inclusion lists or parallel auctions

**For Stakers**

- Jim McDonald: [withdrawals explainer](https://www.attestant.io/posts/understanding-withdrawals/) and changing withdrawal credentials

- Guide to [preparing a voluntary exit message](https://mirror.xyz/ladislaus.eth/wmoBbUBes2Wp1_6DvP6slPabkyujSU7MZOFOC3QpErs&1) in advance of scenarios such as death or stolen/lost node

**Layer 2**

- zkEVMs race to be first to mainnet:
    - [zkSync Era](https://blog.matter-labs.io/all-aboard-zksync-era-mainnet-8b8964ba7c59) (zkSync v2) opens project onboarding before alpha launch
    
    - [Polygon zkEVM](https://polygon.technology/blog/to-ethereum-with-love-announcing-polygon-zkevm-mainnet-beta-on-march-27th) announce beta launch on March 27

- [Optimism delays Bedrock upgrade vote](https://twitter.com/optimismfnd/status/1626380025418113024) to resolve issues from bounty contest

- [Coinbase](https://twitter.com/coinbaseassets/status/1626296045184376833) finally adds send & receive for ETH & DAI on Arbitrum

- Patrick McCorry: [decentralizing a rollup](https://stonecoldpat.substack.com/p/what-does-it-mean-to-decentralise) needs to ensure [one honest party](https://stonecoldpat.substack.com/p/where-is-the-one-honest-party-for) can send all potential decisions to the contract bridge when the system is under attack by an adversary

- EF Layer 2 [grants round recipients](https://blog.ethereum.org/2023/02/14/layer-2-grants-roundup), $948k to 22 projects

**EIPs/Standards**

- ERCs:
    - [ERC6498](https://github.com/ethereum/EIPs/pull/6498/files): Document signing for contracts
    
    - [ERC6506](https://github.com/ethereum/EIPs/pull/6506/files): P2P escrowed governance incentives

* * *

### **This newsletter is made possible thanks to** [**SpeedRunEthereum**](https://speedrunethereum.com/)**!**

![Speed Run Ethereum](https://weekinethereumnews.com/wp-content/uploads/2022/10/Speed-Run-Ethereum-banner.png)

Test your skills and learn how to build apps on Ethereum at [SpeedRunEthereum.com](https://speedrunethereum.com/).

* * *

**Stuff for developers**

- Foundry:
    - forge-std [v1.4.0](https://github.com/foundry-rs/forge-std/releases/tag/v1.4.0): invariant test helpers included by default, Create2 helpers and flag to disable fallback to default public RPC
    
    - [Guide to invariant testing](https://mirror.xyz/horsefacts.eth/Jex2YVaO65dda6zEyfM_-DXlXhOWCAoSpOx5PLocYgw) with Foundry, example using WETH
    
    - [ignore Solidity warnings](https://twitter.com/paulrberg/status/1625131427737088001) with the ignored\_error\_codes config option
    
    - organize unit tests [using a state tree](https://twitter.com/paulrberg/status/1624763320539525121)

- Seaport [v1.3](https://twitter.com/z0age/status/1626583847751266316): zone checks after token transfers fix, prevent filtering native tokens & more efficient bulk listings

- [NFT Exponential Dutch Auction](https://github.com/with-backed/NFTEDA#readme) (NFTEDA) Solidity for exponential price decay

- Alchemy: [walk through of an account abstraction design](https://www.alchemy.com/blog/account-abstraction), explains why ERC4337 is so complex

- Solhint [v3.4.0](https://github.com/protofire/solhint/blob/37d9b14883c4aac29fde19e4b0bf15996bda6953/CHANGELOG.md): adds rules for named parameters in mappings and banning console.sol & global imports

- [Solplate](https://github.com/PaulRBerg/solplate#readme): generate boilerplate Solidity contract using Rust script

- Fe language [bounty challenges](https://blog.fe-lang.org/posts/bountiful-round-2/): two challenges added

- [Guide to using SMTLIB2](https://www.truscova.com/blog_article_7.php) representation of a contract with an SMT Solver

- samczsun’s [ABI Tools](https://openchain.xyz/tools/abi): decode/encode transaction data 

- [ABI Data](https://abidata.net/): API to fetch & cache contract ABI’s from Etherscan

- [Quix NFT marketplace open sourced](https://github.com/quixotic-dev/backend#readme), Next.js/React frontend and Django backend

- [yGenius](https://medium.com/@marcoworms/ygenius-chat-with-yearn-efa17d3f0ec8): connecting a knowledge base to GPT using gpt\_index library

- Yuga Labs Dookey Dash skill-based [mint game cheats and bots](https://cmichel.io/reverse-engineering-dookey-dash/)

**Security**

- Dexible [$1.5m exploit](https://twitter.com/BeosinAlert/status/1626499932265005058), approved tokens could be transferred

- dForcenet [funds returned](https://twitter.com/dForcenet/status/1625004207395807232) after [exploiter’s IP & device info identified](https://twitter.com/blocksecteam/status/1624980515903381504)

- Balancer [Merkle Orchard logic error disclosed](https://medium.com/balancer-protocol/logic-error-bug-fix-review-da37f0cc9a08), $3.2m was at risk, 50 ETH bounty paid

- Beanstalk [logic error disclosed](https://medium.com/immunefi/beanstalk-logic-error-bugfix-review-4fea17478716), $3.1m was at risk, $181k bounty paid

- SCSVS [v2](https://github.com/ComposableSecurity/SCSVS): updated contract security checklist

**Ecosystem**

- [Half of blocks](https://twitter.com/ultrasoundmoney/status/1625209951944642581) were from non-censoring relays

**Enterprise**

- [Starlight](https://github.com/EYBlockchain/starlight#readme) v1 zApp transpiler

- Baseline Profile [architecture explainer](https://www.baseline-protocol.org/blog/the-baseics/)

**Application layer**

- NFT marketplaces:
    - [Blur airdrop](https://twitter.com/blur_io/status/1625566146241114112) caused [surge in gas prices](https://twitter.com/Mega_Fund/status/1625706554073784322)
    
    - Blur updated [creator royalty policy](https://mirror.xyz/blurdao.eth/vYOjzk4cQCQ7AtuJWWiZPoNZ04YKQmTMsos0NNq_hYs) to enforce full royalties only if OpenSea blocked
    
    - [OpenSea dropped fees to zero](https://twitter.com/opensea/status/1626682043655507969) (for an unspecified time) and made royalties optional (0.5% minimum) unless on-chain enforced, marketplaces with the same policies won’t be blocked

- [Overtime](https://medium.com/@OvertimeMarkets.xyz/overtime-is-coming-to-arbitrum-585c1137508f) (sports markets) expands to Arbitrum

- [UMA oSnap](https://medium.com/uma-project/announcing-osnap-gasless-snapshot-voting-with-on-chain-execution-by-uma-7374ed729b28): DAOs can execute off-chain Snapshot voting using UMA’s optimistic oracle

- RabbitHole [v2](https://rabbithole.mirror.xyz/bSr56KIXbFqrDIgV9Aq9vqYx1O31CTOYrN4KwDmMIow) (learn to earn): users complete quests & mint tradable NFTs to claim rewards

* * *

### Job Listings

- Certora is hiring a [Senior Enterprise Sales Rep](https://www.certora.com/#careers).

- [Cyfrin.io](https://www.cyfrin.io/) is hiring [senior security engineers](https://github.com/ChainAccelOrg/SecurityEngineerReq) $190k-$300k.

- Shell Protocol team is hiring [senior Solidity devs & more](https://shellprotocol.io/posts/now-hiring-for-shell-protocol/), remote or Hawaii

- [Request Network](https://request.network/en/) is hiring a [Community & Communication Manager](https://jobs.lever.co/request/76d0db8a-06bc-42c9-9816-69317c5f8c99)

- [Community Lead for ethereum.org](https://jobs.lever.co/ethereumfoundation/89ff5705-3351-422d-a5d1-b0805e95edec?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) sought by Ethereum Foundation

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US SEC:
    - [Terraform Labs & Do Kwon charged](https://www.sec.gov/news/press-release/2023-32) with securities fraud
    
    - [Paxos issued with Wells notice](https://paxos.com/2023/02/13/paxos-issues-statement/) claiming BUSD is a security
    
    - [Blockchain Association filed amicus brief](https://theblockchainassociation.org/blockchain-association-files-amicus-brief-in-sec-lawsuit-against-ishan-wahi/) for SEC claims that 9 tokens are securities in alleged insider trading lawsuit
    
    - proposal for investment advisers to [custody assets only with qualified custodians](https://www.sec.gov/news/press-release/2023-30), [Commissioner Peirce](https://www.sec.gov/news/statement/peirce-statement-custody-021523) concerned for impact on crypto
    
    - [ex-NBA player Paul Pierce](https://www.sec.gov/news/press-release/2023-34) charged for token promotion without disclosing payment & making misleading statements

- [New York Department of Financial Services](https://www.dfs.ny.gov/consumers/alerts/Paxos_and_Binance) ordered Paxos to stop minting BUSD

- [Alex Pertsev](https://cryptoslate.com/tornado-cash-developer-remanded-in-custody-another-3-months-without-charge/) remains in jail in the Netherlands, next hearing in late April

**General/crypto**

- [Zero-value token transfer](https://www.coinbase.com/blog/zero-transfer-phishing-part-1-attack-analysis) phishing attacks (poison transactions)

- [Ordinals (Bitcoin NFTs) using Emblem Vault](https://twitter.com/PapiVault/status/1624279251934449665) to trade on Ethereum via OpenSea

- [Apple WebKit 0-day](https://www.bleepingcomputer.com/news/security/apple-fixes-new-webkit-zero-day-exploited-to-hack-iphones-macs/), malicious web content could lead to arbitrary code execution

- [NameCheap](https://www.bleepingcomputer.com/news/security/namecheaps-email-hacked-to-send-metamask-dhl-phishing-emails/) third party email gateway was sending phishing email

- [Sangria](https://geometry.xyz/notebook/sangria-a-folding-scheme-for-plonk): folding scheme for PLONK

- Why [zk-rollups are advantaged](https://twitter.com/_bfarmer/status/1626436732282408960) over alt-zk L1s

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-february-18-2023](https://weekinethereumnews.com/week-in-ethereum-news-february-18-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Feb 24 - Mar 1 – [ETHDenver BUIDLWeek](https://www.ethdenver.com/)

- Feb 27 – deadline for [EF academic grants round](https://esp.ethereum.foundation/academic-grants-2023)

- Feb 28 – [Sepolia testnet](https://github.com/eth-clients/sepolia/pull/30) upgrades to Shapella

- Mar 2-5 – [ETHDenver Hackathon](https://www.ethdenver.com/)

- Mar 10-29 – [Scaling Ethereum](https://ethglobal.com/events/scaling2023) (ETHGlobal) virtual

- Mar 15-16 – [ETHDubai](https://www.ethdubaiconf.org/)

- Mar 16-18 – [ETH Porto](https://ethporto.org/)

- Mar 28-30 – [Ethereum Rio](https://www.ethereumbrasil.com/ethereumrio)

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- Apr 14-16 – [ETHGlobal Tokyo](https://tokyo.ethglobal.com/)

- Apr 14-16 – [ETHZurich](https://ethereumzuri.ch/) conference & hackathon

- Apr 21-25 – [EthTaipei](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) hackathon & conference

- Apr 27-30 – [Istanbul ETH Privacy](https://www.leadingprivacy.com/istanbul) conference & hackathon

- May 5-7 – [ETHMalaysia](https://ethmalaysia.com/) conference & hackathon

- May 5-7 – [ETHTallinn](https://ethtallinn.org/) hackathon

- May 9-10 – [NFT Tallinn](https://nfttallinn.com/) conference

- May 19-23 – [EDCON](https://edcon.io/) Montenegro (changed from Vienna)

- May 20-21 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 24-26 – [Spaghett ETH](https://naples.spaghett-eth.com/) (Naples) conference

- May 26–28 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Jun 2-4 – [ETH Seoul](https://2023.ethseoul.org/)

- Jun 23–25 – [ETHGlobal Toronto](https://ethglobal.com/events/toronto)

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- **Aug 16-19 –** [**Ethereum Argentina**](https://twitter.com/EtherArgentina/status/1625857633260552200) **(Buenos Aires)**

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–25 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

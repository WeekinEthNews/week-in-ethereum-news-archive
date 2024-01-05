---
title: "Week in Ethereum News <br> September 2, 2023"
date: "2023-09-02"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=GkSjuiqqkKU&t=29s). Recap by [Tim Beiko](https://twitter.com/abcoathup/status/1697343956433219839).  Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1697381822831919503) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-169/):
    - Devnet 8 to be used for most Dencun testing, devnet 9 will include final spec changes & hopefully be the last devnet
    
    - Public testnet upgrade order: Holešky (new, smaller number of node operators), Goerli (deprecated, has most apps/L2s/stakers) and then Sepolia before mainnet
    
    - Holešky to test 3/6 (target/max) blobs with option to reduce to 2/4 for other testnets/mainnet
    
    - Discussions on Verkle trie live migration vs combining with state expiry and Address Space Extension/Compression

- [Intro to blobspace](https://domothy.com/blobspace/): EIP4844 (proto-danksharding) in Dencun upgrade & full danksharding

**Centralization watch: threatening the value of your ETH**

- **🚨🚨🚨** [**Lido very close**](https://dune.com/hildobby/eth2-staking) **to breaching** [**33% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth supermajority, could possibly cause a chain split
    
    - Consensus layer: two clients over 33%, a bug could mean loss of finality

- Needed: more [geographic diversity for both stakers and nodes](https://nodewatch.io/), particularly outside of US/Can/EU

**Layer 1**

- [Ethereum Execution Layer Specification](https://blog.ethereum.org/2023/08/29/eel-spec) (EELS): Python reference implementation (similar to consensus layer Python spec)
    - [Grant available to update Yellow Paper](https://github.com/ethereum/yellowpaper#repository-currently-outdated) with missing pre-merge fork logic

- Erigon [Caplin](https://erigon.substack.com/p/update-on-caplin-and-roadmap-building) (CL client) roadmap

- Dapplion: [Whisk bootstrapping](https://hackmd.io/@dapplion/whisk_bootstrapping), tradeoffs of bootstrapping strategies

- Otterscan [v1.32.0](https://github.com/otterscan/otterscan/releases/tag/v1.32.0): adds contract interaction (for Sourcify verified contracts)

**Client releases**

- Consensus layer:
    - Lodestar [v1.11.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.11.0): adds Holešky testnet

- Execution layer:
    - Nethermind [v1.20.2](https://github.com/NethermindEth/nethermind/releases/tag/1.20.2)/[v1.20.3](https://github.com/NethermindEth/nethermind/releases/tag/1.20.3): adds Holešky testnet
    
    - Reth [v0.1.0-alpha.8](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.8): sub 1TB full node, configurable pruning for each table and improvements for Transaction Pool & RPC

**Research**

- [Decouple attestation weight](https://ethresear.ch/t/reducing-lst-dominance-risk-by-decoupling-attestation-weight-from-attestation-rewards/16523) from attestation rewards, proposal to reduce risks from liquid staking

- [Cumulative non-expiring inclusion lists](https://ethresear.ch/t/cumulative-non-expiring-inclusion-lists/16520), add-on to inclusion list design

- [Slashing penalties if max effective balance increased](https://ethresear.ch/t/slashing-penalty-analysis-eip-7251/16509) (EIP7251), proposes initial penalty be a constant or scale sublinearly and correlation penalty be modified to scale quadratically

- [PEPC-DVT](https://ethresear.ch/t/pepc-dvt-pepc-with-no-changes-to-the-consensus-protocol/16514): Protocol-Enforced Proposer Commitments without changing consensus

**Layer 2**

- Arbitrum [Stylus](https://medium.com/offchainlabs/stylus-now-live-one-chain-many-languages-eee56ad7266d): build apps for Nitro chains in Rust, C & C++, live on testnet

- Polygon [Chain Development Kit](https://polygon.technology/blog/introducing-polygon-chain-development-kit-launch-zk-l2s-on-demand-to-unlock-unified-liquidity) (CDK): launch a rollup or validium

- StarkWare [Stone prover](https://github.com/starkware-libs/stone-prover#readme) open sourced

**EIPs/Standards**

- ERCs (application layer):
    - [ERC7505](https://github.com/ethereum/EIPs/pull/7528/files): NFT author registry
    
    - [ERC7506](https://github.com/ethereum/EIPs/pull/7547/files): Trusted hint registry

* * *

### **Check out Evan’s new podcast:** [**web3 Builders**](https://podcasters.spotify.com/pod/show/web3builderspodcast)

![Web3 Builders](https://weekinethereumnews.com/wp-content/uploads/2023/08/Web3-Builders.webp)

Are the permabulls lying to you (for clicks and views) about the chances for ETF approval?  

Evan says they are, Will disagrees.  

Listen on [Apple](https://podcasts.apple.com/us/podcast/stanford-blockchain-conf-more-drivechains-greyscales/id1697252853?i=1000626495613), [Spotify](https://podcasters.spotify.com/pod/show/web3builderspodcast/episodes/Stanford-Blockchain-Conf--More-Drivechains--Greyscales-ETF--Genslers-Identical-Twin--Uniswap-Court-and-Yes--Friend-Tech-e28qcm2) or [RSS](https://anchor.fm/s/e5abffc8/podcast/rss).  (Or [watch on YouTube](https://www.youtube.com/watch?v=_r8blTEN-lg))

This is a podcast for people who appreciate nuance more than mindless shilling.

* * *

**Stuff for developers**

- Foundry:
    - [Rivet](https://www.paradigm.xyz/2023/08/rivet): developer wallet (browser extension), integrated with Anvil, alpha
    
    - [Huffpoint](https://github.com/devtooligan/Huffpoint#readme): vm.breakpoint in Huff to use with Foundry debugger

- OpenSea [redeemable NFT](https://docs.opensea.io/changelog/define-the-standard-for-nft-redeemables) draft standards, proof of concept burn to redeem live on mainnet

- [Unique contract designs](https://blog.smlxl.io/ethereum-apocrypha-46e155e21a26): BIG, many to one & one to many proxies, overlapping layouts and deeply nested variables

- [Arbitrum Sepolia testnet](https://twitter.com/ArbitrumDevs/status/1696525956834619856) is live, Arbitrum Goerli will be deprecated later in the year

- [Circomscribe](https://www.zksecurity.xyz/blog/posts/circomscribe/): analyze Circom code

- Trail of Bits adding Vyper support to [Slither](https://github.com/crytic/slither/pull/2099) and [Echidna](https://github.com/crytic/echidna/pull/1108)

**Security**

- Ajna [grief vector disclosed](https://blog.summer.fi/ajna-possible-attack-vector/), repay debt & withdraw

- Balancer disclosed vulnerability [exploited](https://twitter.com/Balancer/status/1696930832760635566) for [$2.1 million](https://twitter.com/BeosinAlert/status/1696362629818908758)

- SharedStake (Liquid staking) [105 ETH exploit](https://medium.com/@chimera_defi/sharedstake-exploit-postmortem-sep-1-2023-50a85061d58c), infinite mint via invalid ownership checks

**Enterprise**

- [Swift tokenization experiments](https://www.swift.com/news-events/press-releases/swift-unlocks-potential-tokenisation-successful-blockchain-experiments) used Sepolia testnet via Chainlink CCIP

- [OnlyFans has ETH](https://twitter.com/WuBlockchain/status/1695685476634833164) on its balance sheet

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 9 to 122 gwei, with average around 21.
    - Negative issuance currently at 20.1 gwei 
    
    - About 400 ETH net burn this week

- ETHUSD: $1610-1735, currently ~$1630

- [ETHBTC](https://ratiogang.com/): .062-.0635, currently .063 (Flippening at ~.16)

**Notable at app layer**

- [Gitcoin Grants 18 closed](https://twitter.com/gitcoin/status/1696516357876043826), $680k donated from 47k donors

- Gitcoin Passport [onchain stamps](https://www.gitcoin.co/blog/gitcoin-passport-onchain-stamps): mint passport on Optimism

- [Hats Protocol v2](https://hats.mirror.xyz/NXJI4Rkk4TafwLvVZLfdlz-sLWdrNlKFmvJq9cKDkiw): assign addresses onchain roles and pick what powers each role gets

- Brian Armstrong: [startups I would build today](https://www.coinbase.com/blog/request-for-builders-startups-i-would-build-today)

- Base apps:
    - [OpenCover](https://twitter.com/OpenCoverDeFi/status/1697232657481183252): cover aggregator
    
    - [NFTA](https://www.nfta.pl/): daily price prediction game via drawing price chart, beta

* * *

### Job Listings

- [Product Manager - L2 Blockchain Effort](https://grnh.se/48614a711us) @ Status: [All jobs](https://grnh.se/9fc6e6fc1us)

- EF Privacy & Scaling Explorations team seek [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4)

**Job listings: $600 for four issues** (75 character limit).  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Grayscale procedural victory over SEC in Bitcoin ETF case](https://twitter.com/jchervinsky/status/1696544309699363201): SEC must provide a coherent response for rejection

- US SEC [charges Impact Theory for selling NFTs](https://www.sec.gov/news/press-release/2023-163) as unregistered securities
    - [Unanimous Republican dissent](https://www.sec.gov/news/statement/peirce-uyeda-statement-nft-082823) from Commissioners Peirce & Uyeda

- [Class action against Uniswap dismissed](https://twitter.com/haydenzadams/status/1696991910370411003), not liable for third-party misuse

- Binance: [BUSD users should convert to other stablecoins](https://www.binance.com/en/support/announcement/binance-encourages-users-to-convert-busd-to-other-stablecoins-prior-to-february-2024-d392843e81fd4bc3a5f7e219aa01f34d) by February 2024

**General**

- [OG wallet drainer update](https://twitter.com/tayvano_/status/1696222653747732802): LastPass appears to be the common link

- [Theft patterns](https://twitter.com/tayvano_/status/1697336529746874521) of OG wallet drainer, private key compromise, sweeper bots and Sha Zhu Pan

- [Rune proposes](https://forum.makerdao.com/t/explore-a-fork-of-the-solana-codebase-for-newchain/21822) Maker chain, use hard forks to recover from governance attacks or tech failures

- [MACI & RLN trusted setup ceremonies](https://twitter.com/ctrlc03/status/1696449276652454061): contribute from the browser (requires GitHub private gist access)

- Ittai Abraham: [Fast Fourier Transform over finite fields](https://decentralizedthoughts.github.io/2023-09-01-FFT/)

- [Improving log lookups](https://eprint.iacr.org/2023/1284) using GKR

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-2-2023](https://weekinethereumnews.com/week-in-ethereum-news-september-2-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Sep 7-9 – [ETHAccra](https://www.ethaccra.xyz/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 15-17 – [ETHChicago](https://www.ethchicago.xyz/) conference & hackathon

- Sep 15 – [Holešky testnet](https://github.com/eth-clients/holesky#readme) genesis

- Sep 18-23 – [ETHSafari](https://ethsafari.xyz/) (Kilifi Kenya)

- Sep 21–24 – [Pragma](https://ethglobal.com/events/pragma-newyork) & [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 6-27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 28-30 – [Paradigm CTF](https://ctf.paradigm.xyz/)

- Oct 13-15 – [Ethereum Kuala Lumpur](https://hack.ethkl.org/) conference & hackathon

- Oct 21 – [Ethereum México](https://twitter.com/ethereum_mexico/status/1684649652639924224)

- Oct 22-24 – [ETH Hong Kong](https://www.ethhongkong.co/)

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Oct 27-29 – [ETH Vietnam](https://www.eth-vietnam.com/)

- Oct 27-29 – [ETH London](https://www.encode.club/eth-london) hackathon

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) deadline (max $1k for local meetups)

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://ethbrno.cz)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 16-19 – [Pragma](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Dec 4-5 – [ETHVenice](https://ethvenice.com/)

- Dec 8-10 – ETHGlobal [ETHIndia](https://ethindia.co/) (Bangalore) 

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

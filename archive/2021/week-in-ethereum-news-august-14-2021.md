---
title: "Week in Ethereum News <BR> August 14, 2021"
date: "2021-08-14"
---

## **Eth News and Links**

**Mainnet execution layer**

- Geth [v1.10.7](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.7): potential breaking change in eth\_feeHistory API
- Erigon [v2021.08.02](https://github.com/ledgerwatch/erigon/releases/tag/v2021.08.02): added txpool\_status, eth\_maxPriorityFeePerGas, eth\_feeHistory; vmTrace in trace\_ RPC methods and improved Grafana metrics
- Nethermind [v1.10.79b](https://github.com/NethermindEth/nethermind/releases/tag/1.10.79b): Fixed memory and CPU usage
- ~17% of transactions are [Type 2 (EIP1559)](https://twitter.com/blocknative/status/1425963886549737473) and growing
- Post London discussion for EIP1559 implementers [call](https://www.youtube.com/watch?v=ZmzIHFuwdg0&t=5s) and [agenda](https://github.com/ethereum/pm/issues/369)
- Piper’s [granular functionality](https://notes.ethereum.org/8LbisMwtR4yK64SBosb_2g) needed by a client for the state network component of the portal network
- [Impact of Verkle trees](https://docs.google.com/document/d/1s3qqzbkQFPcNvhzKPdnxg3MlFbv0YjK1z02SxRtdMs8/edit) on existing contracts, ~26% average gas increase

**EIPs/Standards**

- [EIP3712](https://github.com/ethereum/EIPs/pull/3712): Multiple Fungible Token Standard

**Proof of stake consensus layer**

- [Pyrmont testnet upgrade to Altair](https://github.com/eth2-clients/eth2-networks/pull/56) scheduled for epoch 61650, August 19
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210813)
- PoS implementers [call](https://www.youtube.com/watch?v=24MRTRDJ-iw&t=268s). [Notes](https://hackmd.io/@benjaminion/BJu7IifxY) from Ben Edgington: mainnet Altair upgrade date to be set after upgrading Pyrmont
- [Bootstrapping](https://notes.ethereum.org/@ralexstokes/S1RSe1JlF) beacon chain light clients
- Consensus API spec [v2.0.0](https://github.com/ethereum/eth2.0-APIs/releases/tag/v2.0.0): changes for Altair upgrade
- Lighthouse [v1.5.0-rc.0](https://github.com/sigp/lighthouse/releases/tag/v1.5.0-rc.0): update Pyrmont nodes for Altair upgrade, prereleases are not for mainnet use
- Tweet storm on steps to increase [client diversity](https://twitter.com/colfaxselby/status/1424466820522815499?s=20)
- Validator [monitoring guide](https://github.com/remyroy/ethstaker/blob/main/monitoring.md) using Prometheus, Node Exporter and Grafana

**Layer2**

- [Hermez zero-knowledge EVM](https://blog.hermez.io/introducing-hermez-zkevm/) roadmap 
- Proposal for trustless [L2 to sidechain bridge](https://medium.com/starkware/a-trustless-sidechain-to-starkex-bridge-secured-by-ethereum-61e00f19f7e0) using StarkEx secured by  
    Ethereum
- [Arbitrum portal](https://portal.arbitrum.one/) of dapps, wallets and tools for August launch

* * *

### **This newsletter is made possible thanks to [NEAR](https://near.org/)!**

![NEAR METABUIDL Hackathon](https://weekinethereumnews.com/wp-content/uploads/2021/08/NEAR-METABUIDL.png)

NEAR Protocol is hosting the [METABUIDL Hackathon](https://metabuidl.splashthat.com/EthereumNews)! $1 Million Dollars in prizes and funding will be awarded to top projects in DeFi, Gaming, NFTs, and more. Build with community members, participate in workshops, and hack with NEAR from Aug 27-Sep 12

* * *

**Stuff for developers**

- Solidity [v0.8.7](https://blog.soliditylang.org/2021/08/11/solidity-0.8.7-release-announcement/): exposes block base fee, SMTChecker improvements
- Proposal for Solidity [user defined types and operators](https://forum.soliditylang.org/t/user-defined-types-and-operators/456)
- [Solidity resources](https://docs.soliditylang.org/en/latest/resources.html): IDEs, editors, tools and parsers
- Brownie [v1.16.0](https://github.com/eth-brownie/brownie/releases/tag/v1.16.0) (Python): EIP1559 transactions, Hardhat Network support and signing of defunct messages
- Smock [v2](https://defiwonderland.medium.com/smock-an-optimistic-adventure-in-wonderland-1eec36c3e0dd) (JavaScript mocking library for Solidity): improved assertion API, TypeChain support, fakes and mocks
- WalletConnect [v1.6.0](https://twitter.com/WalletConnect/status/1426226788515078144?s=20): new server infrastructure to prevent outages
- [Calldata decoder](https://apoorvlathey.com/eth-calldata-decoder/): uses ABI from Etherscan or custom ABI
- [ERC20Rewards.sol](https://twitter.com/acuestacanada/status/1425754968749903875) rewards token ownership without needing staking transactions
- [ENS avatar field](https://gist.github.com/Arachnid/9db60bd75277969ee1689c8742b75182) format specification
- [Flashbots bundle stats](https://twitter.com/bertcmiller/status/1425809671592493058): check if and when bundle forwarded to miners
- samczsun: [reentrancy with ERC721 and ERC1155 safe functions](https://www.paradigm.xyz/2021/08/the-dangers-of-surprising-code/)

**Security**

- PolyNetwork [~$600million hack](https://twitter.com/kelvinfichter/status/1425217046636371969), cross-chain contract called to change keepers in permissioned contract; Tether [freeze process](https://twitter.com/paoloardoino/status/1425746596768198657); [Q&A with hacker](https://twitter.com/sniko_/status/1425486798726352901); funds are being returned, [$340million](https://twitter.com/PolyNetwork2/status/1425733950614360064) so far
- Punk Protocol [~$9million hack](https://medium.com/punkprotocol/punk-finance-fair-launch-incident-report-984d9e340eb), exploit was front run with ~$6million returned and a $1million fee for the front runner
- DAO Maker [~$7million hack](https://medium.com/daomaker/dao-maker-statement-thursday-12th-of-august-2c3bb0d1bb69), malicious use of wallet with admin privileges

**Ecosystem**

- MetaMask [v10](https://twitter.com/metamask/status/1425855361974734850): EIP1559 transaction support live on mobile and Firefox, rolling out on Chrome
- GridPlus Lattice1 is first hardware wallet to [support EIP1559 transactions](https://twitter.com/gridplus/status/1425869143149056001)
- [BetaRPC](https://github.com/mevalphaleak/BetaRPC-setup): privately routes ~1% of transactions affected by MEV, integrates TaiChi and MEV relays
- [Plan to rename](https://notes.ethereum.org/@timbeiko/great-renaming) Eth1 to Execution layer and Eth2 to Consensus layer, starting with GitHub and R&D Discord
- What [EF teams worked on](https://blog.ethereum.org/2021/08/12/ef-supported-teams-research-and-development-update-2021-pt-2/) in Q2

**Enterprise**

- Paul Brody: [Enterprises should build on public blockchains](https://finance.yahoo.com/news/why-enterprises-build-public-blockchains-153927831.html), private chains are like corporate intranets

**Application layer**

- [Airdrip](https://twitter.com/RafaellaBaraldo/status/1426189408873627649): DAOs stream call options to contributors and community members
- [Curve Finance](https://twitter.com/AndreCronjeTech/status/1425411604506632192) users can bribe curve holders to vote for their rewards
- Hegic [V8888](https://twitter.com/hegicoptions/status/1425147533777674252): peer-to-pool options trading, experimental beta use at own risk
- Zapper decided [not to switch on 0.4% fee](https://medium.com/zapper-protocol/response-to-community-feedback-on-zapper-fees-836997fc68cb) for Zaps
- [NFT Lottery](https://blog.0xmons.xyz/82403366310): sell NFTs in a raffle
- [Mallows](https://www.mallows.xyz/) proof of concept for bring your own algorithm, offering customized UX in web3/metaverse based on the algorithm in the NFT (Disclosure: purchased 2 Mallows)
- Token Engineering Commons [minimal goal reached for hatch](https://twitter.com/tecmns/status/1425399097985437702)
- [POAP websites](https://tomso11.medium.com/how-to-set-up-a-poap-website-511ef979ea19): create a single unique URL per event to claim
- [Onchain blog](https://twitter.com/vaibhavk97/status/1425555004069343235): read messages in transaction input data for an address
- [NFT widget app](https://apps.apple.com/us/app/nft-widgets/id1580495005) for iOS, displays NFTs as widgets
- Péter Szilágyi’s [I’m the Chad NFT](https://twitter.com/peter_szilagyi/status/1425899328560848903): 1 of 1, claimable when base fee is higher than previously purchased

**Regulation/business/tokens**

- Coinbase [ETH trading volume flipped BTC](https://twitter.com/evan_van_ness/status/1425224714407063552?s=20) in Q2
- First big merger of token protocols: [Polygon buys Hermez Network](https://blog.hermez.io/polygon-hermez-merge/) for 3.5 MATIC for 1 HEZ
- [US Senate passed infrastructure bill](https://twitter.com/jchervinsky/status/1425128977560182787) with anti-crypto tax provision, bill now moves to US House of Representatives
- Circle intends to become a [full-reserve national commercial bank](https://www.circle.com/blog/our-journey-to-become-a-national-digital-currency-bank)
- US SEC [$10million settlement with Poloniex](https://www.sec.gov/news/press-release/2021-147) for operating unregistered digital asset exchange
- [BitMEX to pay $100million](https://www.cftc.gov/PressRoom/PressReleases/8412-21) for illegally operating trading platform and AML violations; founders still have open cases
- Venmo credit card users can now get [Eth instead of frequent flyer miles](https://newsroom.paypal-corp.com/2021-08-10-Introducing-Cash-Back-to-Crypto-with-the-Venmo-Credit-Card)
- Leo Messi signing fee for Paris St Germain [includes club fan tokens](https://www.reuters.com/lifestyle/sports/exclusive-messis-paris-st-germain-package-includes-crypto-fan-tokens-2021-08-12/)

**General**

- Rich get richer argument against PoS is [fundamentally flawed](https://medium.com/@fubuloubu/the-rich-are-getting-richer-supporting-a-global-economic-system-for-billions-of-people-in-the-9cd5c1366434)
- Vitalik: [votes as buy orders](https://ethresear.ch/t/votes-as-buy-orders-a-new-type-of-hybrid-coin-voting-futarchy/10305), hybrid between voting and futarchy
- Packy McCormick: [NFTs as social networks](https://www.notboring.co/p/status-monkeys)
- New York Times: [joining a penguin NFT club as that’s what we do now](https://www.nytimes.com/2021/08/12/technology/penguin-nft-club.html)
- Fred Wilson: [consumer experiences built on crypto](https://avc.mirror.xyz/rjT0_tFp1AQFgRHzLWc6uSyIkwfxxYHMbXQXY6j-bG8) are next big thing
- Art in America: [exhibiting NFTs](https://www.artnews.com/art-in-america/features/nfts-curation-online-exhibitions-crypto-art-1234601534/)
- IC3 blockchain camp [videos](https://www.youtube.com/playlist?list=PLuAi322ybV05UsO49x0BWQbRK7I-mehzz)

* * *

## **Job Listings**

- [Full-stack/mobile lead and architect](https://www.linkedin.com/in/shawnarney). Seeking challenging opportunity.
- Solidity is [hiring a C++ dev](https://ethereum.bamboohr.com/jobs/view.php?id=40&source=weekinethnews)
- WalletConnect looking for [Javascript/Typescript devs](https://twitter.com/WalletConnect/status/1421397382391078924)
- Ethereum Foundation: [Test Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=39) for consensus and execution layers
- Nethermind [internship program](https://www.notion.so/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-14-2021/](https://weekinethereumnews.com/week-in-ethereum-news-august-14-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Aug 17 – applications close for [written pieces on public goods projects](https://gitcoin.co/blog/seeking-a-new-kind-of-public-good/)
- **Aug 17-Sep 7 – Gitcoin [Decentralized Governance Hackathon](https://gitcoin.co/hackathon/dgov/onboard)**
- **Aug 19 – Pyrmont testnet [upgrade to Altair](https://github.com/eth2-clients/eth2-networks/pull/56) (epoch 61650)**
- Aug 27-29 – [Edcon](https://www.edcon.io/) (Shenzhen/online)
- **Sep 15-17 – [MetaCartel MCON Denver](https://www.mcon.fun/)**
- **Sep 17-Oct 15 – [ETHOnline hackathon](https://online.ethglobal.com/)**
- Oct 1-3 – [EthAtlanta](https://ethatl.com/) enterprise-focused hackathon & keynotes
- Oct 22-24 – [ETH Lisbon](https://ethlisbon.org/)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

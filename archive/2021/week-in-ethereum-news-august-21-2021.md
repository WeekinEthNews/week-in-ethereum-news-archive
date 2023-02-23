---
title: "Week in Ethereum News <BR> August 21, 2021"
date: "2021-08-21"
---

## **Eth News and Links**

**Mainnet execution layer**

- Geth releasing [hotfix](https://twitter.com/go_ethereum/status/1428051458763763721) on August 24 for undisclosed high severity security issue
- Latest core devs call [video](https://www.youtube.com/watch?v=rlIgpf2V4ks&t=214s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1428750228237258767);
    - London [retrospective](https://hackmd.io/@timbeiko/london-retro)
    - ~December upgrade for difficulty bomb delay and potentially constant tweaks for EIP1559, no new EIPs before PoW switch off 
    - Clients focusing on PoW switch off and internal improvements
- Erigon [v2021.08.03](https://github.com/ledgerwatch/erigon/releases/tag/v2021.08.03): datadir parameter not backward-compatible and fix for trace\_ RPC
- Nethermind [v1.11.0](https://github.com/NethermindEth/nethermind/releases/tag/1.11.0): added trace\_filter and JSON RPC over IPC 
- [Network capacity ~9% higher post London](https://www.reddit.com/r/ethereum/comments/p4nloh/why_has_the_chain_capacity_increased_by_9_after/) due to ice age delay, pre-London blocks not always being full and EIP1559 formula
- [Visualization of estimated gas price](https://twitter.com/takenstheorem/status/1427130936940851201) 100k blocks before and after London upgrade, less volatility means fewer weekend downswings
- [Node crawler](https://crawler.ethereum.org/) alpha, drill down by client, version and operating system

**EIPs/Standards**

- [EIP3722](https://github.com/ethereum/EIPs/blob/7532ff5af50d227ec7729141595367a51e27465c/EIPS/eip-3722.md): Poster 

**Proof of stake consensus layer**

- Lodestar (TypeScript) [light client prototype](https://medium.com/chainsafe-systems/lodestar-releases-light-client-prototype-40f300361c65): bandwidth and processing load reduced by ~99% of full client
- Pyrmont testnet [upgraded to Altair](https://twitter.com/protolambda/status/1428331065660350474); Pyrmont is being [deprecated](https://twitter.com/dannyryan/status/1427621936536850435) and users should switch to Prater testnet
- Teku [v21.8.1](https://github.com/ConsenSys/teku/releases/tag/21.8.1): improved peer discovery, improved performance for load balanced beacon nodes and clearer sync progress logs
- [Design space](https://hackmd.io/@n0ble/consensus_api_design_space) of Consensus API
- Using [total difficulty threshold as hard fork anchor](https://ethresear.ch/t/using-total-difficulty-threshold-for-hardfork-anchor-what-could-go-wrong/10357), a 7 day scheduled PoW switch off could be 4 days early
- [Ledger adds staking](https://www.ledger.com/blog/lido-available-in-ledger-live-bringing-ethereum-staking-within-your-reach) with Lido (staking pool)
- [Open the ports on your beacon chain nodes](https://www.symphonious.net/2021/08/14/exploring-eth2-why-open-ports-matter/)! Improve the network’s efficiency and reduce risk of censorship

**Layer2**

- [Optimism developer onboarding criteria](https://community.optimism.io/docs/developers/l2/deploy.html), testnet regenesis ~October, ETH may no longer be ERC20 compatible, will use Solidity compiler, EOAs no longer contract wallets and decrease gas usage
- [1inch Network](https://blog.1inch.io/the-1inch-network-expands-to-optimistic-ethereum-2beb89fa63bf) live on Optimism
- [Teleportr](https://twitter.com/0x_clem/status/1428606240293212167): low cost mainnet to Optimism ETH bridge, 0.02ETH limit
- [Boba Network](https://www.enya.ai/press/bobanetwork) is rebranded OMGX Network (optimistic rollup based on Optimism)
- Protolambda tweetstorm: [use execution-consensus API for rollups](https://twitter.com/protolambda/status/1427819901524324360) with minimal diff and full compatibility
- [Warp](https://medium.com/nethermind-eth/warp-your-way-to-starknet-ddd6856875e0): EVM to Cairo (StarkNet’s smart contract language) transpiler
- StarkWare's [shared prover](https://twitter.com/ukolodny/status/1428556705525374978) (SHARP) reduces small apps’ layer 2 costs

* * *

### **This newsletter is made possible thanks to [Celer](https://www.celer.network/)!**

![Celer](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

Celer Network is a layer-2 scaling platform that brings fast, secure and low-cost blockchain applications. [Celer cBridge](http://cbridge.celer.network/) v1.0 is now live on mainnet. Users are now able to use cBridge to instantly transfer tokens across Ethereum, Arbitrum, Polygon and Binance Smart Chain, with many more side chain and layer-2 chain integrations planned for in the near future. Anyone can [run a cBridge node](https://github.com/celer-network/cbridge-node) to join the cBridge Network and provide cross-chain and cross-layer liquidity while generating yields through transaction fees.

* * *

**Stuff for developers**

- web3.js [v1.5.2](https://github.com/ChainSafe/web3.js/releases/tag/v1.5.2): removed default of transactions to Type 0
- Remix IDE [v0.16.2](https://twitter.com/EthereumRemix/status/1427212729748803587): Metamask v10.0.0+ support for type 2 transactions  
- OpenZeppelin Contracts [v4.3](https://blog.openzeppelin.com/openzeppelin-contracts-4-3/): modular on-chain governance based on Compound’s GovernorAlpha/GovernorBravo and ERC interfaces 
- Guide to [verifying a contract on Etherscan](https://forum.openzeppelin.com/t/how-to-verify-a-contract-on-etherscan-bscscan-polygonscan/14225) from OpenZeppelin
- [Hardhat](https://hackmd.io/@fvictorio/hardhat-networks-and-providers) difference between Hardhat Network and other configured networks
- ts-essentials [v8.0.0](https://github.com/krzkaczor/ts-essentials/releases/tag/v8.0.0): updated for TypeScript v4
- [ethers-flashbots](https://github.com/onbjerg/ethers-flashbots) (Rust): ethers middleware to send transactions as Flashbots bundles
- [poseidon-tornado](https://github.com/ChihChengLiang/poseidon-tornado): Tornado Cash fork using Poseidon Hash
- [Typescript-eth-starter](https://github.com/nezz0746/typescript-eth-starter): simple Greeter smart contract on localhost and Rinkeby with React stack
- [Web3-Boilerplate](https://twitter.com/DennisonBertram/status/1427253698602938372): using RedwoodJS, Simple Wallet connector and useDapp
- [Lambda School](https://twitter.com/Austen/status/1428025522584391684) developing blockchain course to convert developers to crypto developers

**Security**

- samczsun [disclosed vulnerability in SushiSwap’s Miso](https://www.paradigm.xyz/2021/08/two-rights-might-make-a-wrong/), ~$350million was at risk due to msg.value used in a loop via delegatecall; formal verification didn’t detect bug as [formal spec missing a rule](https://twitter.com/CertoraInc/status/1428103804449345538)
- [Tally voting bug](https://medium.com/tally-blog/incident-summary-tally-voting-bug-dd6f9cceaae4), against votes sent as for votes due to faulty boolean check in Typescript, used with Uniswap, Fei, Gitcoin, and Idle proposals
- Liquid exchange had [~$90million moved](https://blog.liquid.com/warm-wallet-incident) from compromised warm wallets
- Scammer convinced user to show MetaMask sync with mobile QR via screen share, [MetaMask improved warnings](https://twitter.com/MyCrypto/status/1428151706559205379) not to share this QR code
- Polygon [denial of service vulnerability](https://iosiro.com/blog/temporary-denial-of-service-vulnerability-disclosed-to-and-remediated-by-polygon) disclosed, uninitialized logic contract could be self destructed
- PolyNetwork hack, [ongoing Q&A](https://twitter.com/sniko_/status/1428448414270951426) with hacker

**Ecosystem**

- MetaMask: how to set EIP1559 transaction priority [video](https://www.youtube.com/watch?v=gsfJywNxpi4)
- [Tally](https://blog.tally.cash/a-community-owned-wallet-for-the-new-internet/) web3 wallet being developed, first release to focus on open finance
- Etherscan shows green light bulb for [Type 2 EIP1559 transactions](https://twitter.com/someresat/status/1426979047448276994)
- Vitalik: [moving beyond coin voting governance](https://vitalik.ca/general/2021/08/16/voting3.html)

**Enterprise**

- Draft [Baseline standard](https://github.com/eea-oasis/baseline-standard)
- [Microsoft Argus](https://www.microsoft.com/en-us/research/uploads/prod/2021/08/Argus_SRDS_Camera.pdf) paper on incentive system for anti-piracy campaigns

**Application layer**

- [OpenFrontEnds DAO](https://twitter.com/adamscochran/status/1427447330496819204) to create decentralized front ends for DeFi protocols
- [iceCream](https://forum.cream.finance/t/implementation-of-new-tokenomics/1910): vested, non-transferrable, non-tradeable governance tokens
- Andre Cronje: [liquidity mining rewards](https://andrecronje.medium.com/liquidity-mining-rewards-v2-50896e44f259) using options
- [Beta Finance](https://medium.com/beta-finance/beta-finance-is-live-on-ethereum-mainnet-f1fc32959f3e): lend, borrow and short sell selected tokens
- Proposal for [power perpetuals](https://www.paradigm.xyz/2021/08/power-perpetuals/) (squeeth): perpetual derivative indexed to a power of the price of an underlying instrument such as Ether
- Cryptopunk images and attributes [added on-chain](https://larvalabs.com/blog/2021-8-18-18-0/on-chain-cryptopunks)
- [NFT for biopharma research and IP rights](https://twitter.com/paulkhls/status/1427724533713326082) sold to DAO to fund research
- OpenSea passed Etsy in volume, [$1billion for August](https://twitter.com/xanderatallah/status/1427453596858294272)

**Regulation/business/tokens**

- US CFTC: [ETH \[is\] a non-security commodity](https://twitter.com/CFTCquintenz/status/1426570174036168704)
- Bloomberg: 50 years after dropping the gold standard US needs to [avoid expensive mistake of restrictive regulation](https://www.bloomberg.com/opinion/articles/2021-08-15/niall-ferguson-nixon-the-gold-standard-and-a-bitcoin-bonanza) for crypto
- [Binance requiring KYC](https://www.binance.com/en/support/announcement/51bf294e26324211a4731ca998e110ca) (including government ID and facial verification) for all users
- [Props Loyalty Program ending](https://blog.propsproject.com/a-letter-from-our-ceo-1332f6cabab1) and stopping issuing new Props Tokens due to constraints of US Regulation A+
- ImmutableX [rewarding US users with ETH](https://immutablex.medium.com/important-announcement-imx-alpha-rewards-update-929f7bc89513) rather than protocol token due to US regulatory uncertainty
- Bloomberg’s [Studio 1.0 interview with Vitalik](https://twitter.com/emilychangtv/status/1428204792212385795), includes discussion on the metaverse and skepticism for DeFi on Bitcoin
- Coinbase to be first US publicly traded company to [hold ETH on balance sheet](https://blog.coinbase.com/coinbase-updates-investment-policy-to-increase-investments-in-crypto-assets-a68c752ea786)

**General**

- Chris Dixons tweet storm [blockchains are the new app stores](https://twitter.com/cdixon/status/1427452458813464577)
- [Who owns the metaverse](https://m.mirror.xyz/OlcHFb-umaeoQrmSroGMjRKc2mp2Vm898CBUo0CMHeY), terms of service of social media giants
- Cory Doctorow: [copyright protects creativity, not effort](https://pluralistic.net/2021/08/14/angels-and-demons/#owning-culture)
- Bluesky, started by Twitter to decentralize social media, being led by [Jay Graber](https://twitter.com/arcalinea/status/1427314482154414080) who recently advised [reputation project linking Twitter to web3](https://jaygraber.medium.com/introducing-interrep-255d3f56682)
- [T‑Mobile data breach](https://www.t-mobile.com/news/network/additional-information-regarding-2021-cyberattack-investigation): 7.8million postpaid, 0.8million prepaid and 40million former/prospective customers impacted
- [McEliece-1284 challenge broken](https://twitter.com/AlexanderMay10/status/1427298867465314304) in ~22 CPU years
- [Cairo architecture](https://eprint.iacr.org/2021/1063) and how Cairo proofs are created
- Cloudflare: [Zero-Knowledge proofs for private web attestation](https://blog.cloudflare.com/introducing-zero-knowledge-proofs-for-private-web-attestation-with-cross-multi-vendor-hardware/) with cross/multi-vendor hardware
- [Aggregating hash-based signatures](https://eprint.iacr.org/2021/1048) using STARKs
- [Reinforced Concrete](https://eprint.iacr.org/2021/1038): fast hash function for ZKProofs and verifiable computation
- [Dogecoin Foundation reestablished](https://foundation.dogecoin.com/posts/2021/08/announcement-re-establishing-the-dogecoin-foundation/) with Vitalik as board advisor

* * *

## **Job Listings**

- Hiring a [Front-End (or Full Stack) Engineer](https://blog.kwenta.io/kwenta-open-position-front-end-developer/) at Kwenta
- Ethereum Foundation: [Test Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=39) for consensus and execution layers
- Solidity is [hiring a C++ dev](https://ethereum.bamboohr.com/jobs/view.php?id=40&source=weekinethnews)
- WalletConnect looking for [Javascript/Typescript devs](https://twitter.com/WalletConnect/status/1421397382391078924)
- Nethermind [internship program](https://www.notion.so/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-21-2021/](https://weekinethereumnews.com/week-in-ethereum-news-august-21-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- **Aug 24 – [Geth releasing hotfix](https://twitter.com/go_ethereum/status/1428051458763763721)**
- Aug 27-29 – [Edcon](https://www.edcon.io/) (online)
- Sep 15-17 – [MetaCartel MCON Denver](https://www.mcon.fun/)
- Sep 17-Oct 15 – [ETHOnline hackathon](https://online.ethglobal.com/)
- Oct 1-3 – [EthAtlanta](https://ethatl.com/) enterprise-focused hackathon & keynotes
- Oct 22-24 – [ETH Lisbon](https://ethlisbon.org/)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

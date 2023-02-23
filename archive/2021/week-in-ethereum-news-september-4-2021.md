---
title: "Week in Ethereum News <BR> September 4, 2021"
date: "2021-09-04"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest [core devs call video](https://www.youtube.com/watch?v=XxozI0Wpr7I). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1433831124267147264):
    - Consensus API discussion
    - Work in progress [sync algorithm](https://github.com/fjl/p2p-drafts/blob/master/merge-sync/merge-sync.md) post PoW switch off
    - Fixed gas limit EIP debate
- Erigon [2021.09.01-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2021.09.01): call tracing improved, bad.block flag changed to use block hash, fix for Ropsten testnet diversion
- Nethermind [v1.11.1](https://github.com/NethermindEth/nethermind/releases/tag/1.11.1): support for eth/66 (as eth/65 is being deprecated) and eth\_feeHistory
- [Parallel EVM execution engine](https://twitter.com/brockjelmore/status/1433189610797113357) experiment: 120 tx block, 0 contention had 5x speedup, 100% contention + pessimistic had 17% slowdown

**EIPs/Standards**

- [EIP3788](https://eips.ethereum.org/EIPS/eip-3788): Strict enforcement of chainId
- [EIP3779](https://eips.ethereum.org/EIPS/eip-3779): Safe Control Flow for the EVM

**Proof of stake consensus layer**

- [Prater testnet upgrade](https://twitter.com/terencechain/status/1433422624785190913) to Altair: minor client-specific issues have been patched or under investigation
- [Client diversity needed](https://our.status.im/the-importance-of-client-diversity/) to ensure safest transition from PoW to PoS; dominant client needs to be < 50%, ideally < 33%
- [Stakers get slashed for contradicting themselves,](https://twitter.com/JaEsf/status/1431312295192313864) not for going offline or picking the wrong fork
- Tips from staking [on a Raspberry Pi 4](https://twitter.com/EthereumOnARM/status/1432251814402002948) with consensus and execution clients on one device 
- [Understanding attestation packing efficiencies](https://lighthouse.sigmaprime.io/attestation-packing.html): an anonymized look at the packing efficiency of different staking clients and pools
- Stereum (beacon chain client installer) launcher [v1.5](https://stereum.net/ethereum-node-setup-1-5/)

**Layer2**

- [Arbitrum](https://offchain.medium.com/mainnet-for-everyone-27ce0f67c85e) beta, initial cap of 80k arbgas per second (equivalent of mainnet), token bridge restricted to approved tokens, 7 day exits 
    - Ether and token bridge [tutorial](https://arbitrum.io/bridge-tutorial/)
    - [Arbiscan](https://arbiscan.io/) block explorer by Etherscan
    - Reddit [AMA](https://www.reddit.com/r/ethereum/comments/pgl5a4/were_offchain_labs_the_team_behind_arbitrum_the/) with Arbitrum team
    - Selected [apps](https://portal.arbitrum.one/) live now: Uniswap, Celer’s cBridge, Balancer, Sushiswap, Dodo, MCDEX, Swapr. More apps coming soon
- [Celer cBridge adds support for Optimism](https://twitter.com/CelerNetwork/status/1432751288681316352) for 3 minute exits; transfer between between mainnet, Optimism, Arbitrum and selected sidechains
- StarkNet [Alpha 2](https://medium.com/starkware/starknet-alpha-2-4aa116f0ecfc): composability, local testing and moved to Goerli; OpenZeppelin developing contracts library
- [Immutable X](https://twitter.com/Immutable/status/1433703349061242882) opens gas free NFT minting and trading

* * *

### **This newsletter is made possible thanks to [Kwenta](https://kwenta.io/) by [Synthetix](https://synthetix.io/)!**

![Kwenta](https://weekinethereumnews.com/wp-content/uploads/2021/04/IMG_20210418_190328_618-1024x512.jpg)

[Kwenta](https://kwenta.io/) enables traders to access real-world and derivative assets on-chain using the power of the Synthetix protocol. 

Long or short popular synthetic cryptocurrencies, commodities, forex, and equities without the limits or compromises of a centralized exchange. 

You can now also use [L2 Kwenta on Optimism](https://blog.kwenta.io/everything-you-need-to-know-about-using-kwenta-on-l2/) for low gas fees and blazing fast transactions!

Decentralized Perpetual Futures coming soon.

* * *

**Stuff for developers**

- [Update web3.js for EIP1559 support](https://twitter.com/TimBeiko/status/1433783065638285315) so you don’t cost your users money
- Fe (EVM language) [roadmap](https://snakecharmers.ethereum.org/fes-path-to-production/) to production in 2021
- Remix IDE [v0.17.0](https://medium.com/remix-ide/remix-ide-v0-17-0-is-released-75348f044f8d): Solidity defaults to 0.8.7, EVM default is London, Hardhat console logs in Remix Terminal
- Etherscan adds support for [ERC1155](https://etherscan.io/tokentxns-nft1155) multi token standard
- Guide to [using SMTChecker](https://medium.com/@sblowpckcr/smtchecker-almost-practical-superpower-5a3efdb3cf19) to check Solidity contract invariants
- [Tenderly](https://blog.tenderly.co/tenderly-now-supports-both-solidity-and-vyper/) adds support for Vyper language
- ts-essentials [v8.1.0](https://github.com/krzkaczor/ts-essentials/releases/tag/v8.1.0) (TypeScript): fixes for minor issues
- [fractional-rs](https://github.com/gakonst/fractional-rs) (Rust): CLI & utilities for fractional.art, only supports bid
- [zk-ml](https://github.com/zk-ml/demo): demo of private machine learning. Linear regression in a circom circuit and on chain encrypted data transfer with SNARKS
- Guide to adding support for [ENS in multi network apps](https://medium.com/the-ethereum-name-service/how-to-support-ens-for-multi-chain-dapps-b0a7ff043d77)
- [GitPOAP](https://twitter.com/poapxyz/status/1432168887739637760): code repository maintainers can award POAPs to contributors
- Tutorial to [create a staking dapp](https://stermi.medium.com/how-to-write-your-first-decentralized-app-scaffold-eth-challenge-1-staking-dapp-b0b6a6f4d242) using scaffold-eth
- [Ideas and wish lists](https://twitter.com/wslyvh/status/1433787757676089344) to inspire your web3 project

**Security**

- Cream Finance [exploit](https://medium.com/cream-finance/c-r-e-a-m-finance-post-mortem-amp-exploit-6ceb20a630c5) of 462m AMP and 2.8k ETH, ERC777 reentrancy on AMP token
- xToken [exploit](https://medium.com/xtoken/xsnx-post-mortem-666d35071f38) with $4.5 million loss, incorrect require statement allowed function to be publicly callable 
- OpenZeppelin Contracts [TimelockController vulnerability postmortem](https://forum.openzeppelin.com/t/timelockcontroller-vulnerability-postmortem/14958)
- DeFiYield’s [database](https://blog.defiyield.app/announcing-the-worlds-first-defi-rekt-database-271c6c2a8f7a) of DeFi scams, hacks and exploits
- Writing Dafny proofs to [formally verify beacon chain deposit contract](https://consensys.net/blog/ethereum-2-0/20039/)
- Act v[0.1](https://fv.ethereum.org/2021/08/31/act-0.1/): formal specification language for high level descriptions of smart contracts

**Ecosystem**

- First [full day of negative issuance](https://twitter.com/cory_eth/status/1433944817671684104) due to EIP1559 burn from NFT transactions
- Tim Beiko on the [evolution of the Ethereum scalability roadmap](https://tim.mirror.xyz/CHQtTJb1NDxCK41JpULL-zAJe7YOtw-m4UDw6KDju6c)
- [EIP1559 didn't increase gas prices](https://twitter.com/korpi87/status/1433375443445555200), NFTs did; set priority fee and max fee to not overpay
- Overspending on gas fees [reduced by EIP1559](https://twitter.com/nicksdjohnson/status/1432187721812824073)
- Edcon 2021 [videos](https://www.youtube.com/playlist?list=PL6-IF807eaBFg6Rg22ByDsVXUg1wfaWRz)
- Flashbot [searchers compete on MEV extraction efficiency](https://twitter.com/bertcmiller/status/1432031142589386756), percentage of gas used by each bundle decreases over time
- Etherscan [token holdings page](https://twitter.com/etherscan/status/1433771612231200777) for a given address, beta release
- MetaMask has over [10 million](https://consensys.net/blog/press-release/metamask-surpasses-10-million-maus-making-it-the-worlds-leading-non-custodial-crypto-wallet/) monthly active users

**Enterprise**

- [Baseledger testnet](https://medium.com/unibrightio/high-security-it-synchronization-network-baseledger-launches-powered-by-ubt-2e59e89e1ef): designed for storing and managing baseline proofs, fixed transaction fees denominated and paid in fiat
- Guide to [deploying Quorum](https://consensys.net/quorum/products/guides/getting-started-with-consensys-quorum)

**Application layer**

- Loot [explainer](https://twitter.com/tandavas/status/1432802983528448000): adventurer items as on chain text, bottom up NFT as possible seed for gaming universe; every address has [synthetic loot](https://twitter.com/dhof/status/1433110412187287560)
- [1 million POAPs](https://twitter.com/poapxyz/status/1433480718932402176) have been minted
- Bored and Mutant Ape community [receiving 3D models](https://twitter.com/TaylorGerring/status/1432065454835654658) to use in metaverse
- [Animal coloring book](https://generative-transfer-art.vercel.app/) generative NFT, onchain SVG colored on transfer
- [Trader](https://medium.com/traderxyz/welcome-trader-trade-with-friends-8d4698d1a600): NFT trading with off-chain open order book, using social links
- Doge NFT [fractionalized as $DOG](https://pleasr.mirror.xyz/7hpdJOWRzQx2pmCA16MDxN2FiA3eY6dwcrnEtXKnCJw) by PleasrDAO
- NFT derivative [floor perpetual](https://www.paradigm.xyz/2021/08/floor-perps/), synthetics tracking the floor price of a project, mint by locking up an NFT from the project
- [Dfdao thesis](https://medium.com/dfdao/the-crypto-gaming-governance-thesis-39b85b371e4e): crypto-gaming governance is rapidly iterable, at bleeding edge of decentralized governance design 
- Synthetix [V2x scope](https://blog.synthetix.io/v2x-revisited/): L1 improvements and tech debt, Optimism migration, new mechanisms and governance

**Regulation/business/tokens**

- [BitConnect, founder and US promoter](https://www.sec.gov/news/press-release/2021-172) charged by US SEC alleging $2 billion fraud via unregistered offering of investments to retail
- [US SEC inquiring into DeFi](https://thedefiant.io/sec-defi/) including Uniswap Labs
- Spurred by crypto-friendly Sen Toomey (R-PA), US Senate [Banking Committee asking for public proposals on crypto regulation](https://www.banking.senate.gov/newsroom/minority/toomey-requests-feedback-on-clarifying-laws-around-cryptocurrency-and-blockchain-technologies)
- University of Texas professor’s research suggests [EOS ICO pumped via washtrading](https://www.integrafec.com/post/eos-ico)
- [Challenges to scale DAOs](https://thedefiant.io/scaling-daos/): legal clarity, limiting liability of stakeholders, hiring, compliance for workers and governance
- [How to vet crypto projects](https://medium.com/@seven7hwave/how-to-vet-crypto-projects-and-blockchain-tech-104ae169107): evaluate the problem being solved, the team, audits, the community and what could go wrong technically
- LarvaLabs (CryptoPunks, Autoglyphs and Meebits) [signs with Hollywood agency for content deals](https://www.hollywoodreporter.com/business/digital/uta-cryptopunks-nft-film-tv-vieo-games-1235005392/)

**General**

- The story of the fallout from the [NSA’s 2008 insertion of a backdoor into an encryption standard](https://finance.yahoo.com/news/juniper-breach-mystery-starts-clear-130016591.html)
- Long (and surprisingly interesting!) read: [History of bug bounties](https://duo.com/decipher/lawyers-bugs-and-money-when-bug-bounties-went-boom)
- The case for engineers to [leave FAANG for crypto](https://www.paradigm.xyz/2021/09/the-community-garden-the-case-for-leaving-faang-companies-for-crypto/)
- Vitalik’s insider [Q&A](https://twitter.com/vitalikbuterin/status/1433195737907564545): excitement for zk-SNARKs, NFTs are most surprising use case, 8 cofounder regret and other insights

* * *

## **Job Listings**

- Mark Cuban is seeking a web3 developer. [Send a front-end sample to apply](https://forms.office.com/r/M81g5RNgXX)
- Dark Forest: [Full-Stack Developer](https://darkforest-eth.notion.site/darkforest-eth/Dark-Forest-Full-Stack-Developer-82f4c4f3a88248f580c20b507685c5c8)
- Futureswap is hiring a [Product Marketing Manager](https://angel.co/company/futureswap/jobs/1509809-product-marketing-manager)
- Vac (Status) is looking for a [smart contracts protocol engineer](https://jobs.status.im/en/jobs/20563) for Waku

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-4-2021/](https://weekinethereumnews.com/week-in-ethereum-news-september-4-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Sep 8  – [Gitcoin Grants Round 11](https://twitter.com/gitcoin/status/1430284881678962698) and hackathon starts **(support [Week in Eth News](https://gitcoin.co/grants/2785/week-in-ethereum-news))**
- Sep 15-17 – [MetaCartel MCON Denver](https://www.mcon.fun/)
- Sep 17-Oct 15 – [ETHOnline hackathon](https://online.ethglobal.com/)
- **Sep 30 – [NFT Fest Australia](https://nftfest.com.au/) (virtual)**
- Oct 1-3 – [EthAtlanta](https://ethatl.com/) enterprise-focused hackathon & keynotes
- Oct 20-21 - [LisCon](https://liscon.org/) (Lisbon)
- Oct 22-24 – [ETH Lisbon](https://ethlisbon.org/) hackathon

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

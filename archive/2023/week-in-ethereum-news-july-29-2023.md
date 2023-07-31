---
title: "Week in Ethereum News <br> July 29, 2023"
date: "2023-07-28"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=WtOQPxa6jOE&t=245s). Notes from [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-consensus-call-114/):
    - Dencun upgrade discussions: MEV-Boost testing needed, decided against adding parent beacon block root to execution payload and when to rollout the fork choice change for confirmation rule
    
    - EIPs can be presented in ACDC calls prior to scoping Electra upgrade
    
    - Discussed EIP6914 (reuse withdrawn validator indices) updates and prototype of EIP6110 (validator deposits onchain)
    
    - Increasing CL client [spec compliance](https://docs.google.com/document/d/1HMSxMNY3nZR4NKohIQAhzRTzYnKEJEU9ro8Z8kcnH2c/edit#heading=h.jhia3qtraquu)

- EIP4844:
    - Latest EIP4844 implementer call. Notes from [Terence](https://twitter.com/terencechain/status/1683519689601994753): devnet 8 features, [blob transaction pool design](https://hackmd.io/aVek93y-QmSv1mz2Agc9iQ) and no incentives for MEV-Boost builders to include blobs
    
    - KZG Ceremony [extended until August 23](https://twitter.com/carlbeek/status/1683034067435147265)

**Layer 1**

- [Nethermind implemented stateless verification](https://twitter.com/jasoriatanishq/status/1683454125042995200), allows participation as a stateless client

- [Teku planned caching changes](https://mirror.xyz/rolfy.eth/9rT9Ia_VpbksURo8Bt8GSHaepM0mj0fo3styV-czBUE) & memory reduction

- [Lighthouse subnet backbone revamp](https://lighthouse-blog.sigmaprime.io/update-42.html) & IPv6 support in recent v4.3.0 release

- [Consensus layer mainnet bootnodes](https://twitter.com/pcaversaccio/status/1683799790633582592) location & IP address

- [JIT EVM](https://github.com/paradigmxyz/jitevm#readme): convert EVM to machine code, using LLVM/inkwell, in Rust, proof of concept

**Research**

- Game-theoretic [model for MEV-Boost auctions](https://ethresear.ch/t/game-theoretic-model-for-mev-boost-auctions-mma/16206): builder strategies to win auctions

**Layer 2**

- [Public goods network](https://twitter.com/pgn_eth/status/1683843118284812290) (OP Stack rollup) live, aims to generate funding for public goods

- Optimism [law of chains](https://gov.optimism.io/t/law-of-chains-v0-1-full-draft/6514) proposed neutrality framework for Superchain (OP Stack) participants

**EIPs/Standards**

- EIPs:
    - [EIP7377](https://eips.ethereum.org/EIPS/eip-7377): Migration transaction (one-time transaction for EOA to deploy code to their address)
    
    - [EIP7378](https://github.com/ethereum/EIPs/pull/7378/files): Add time-weighted averaging to the base fee

- ERCs (application layer):
    - [ERC7390](https://github.com/ethereum/EIPs/pull/7390/files): Vanilla options
    
    - [ERC7399](https://github.com/ethereum/EIPs/pull/7400/files): Flash loans
    
    - [ERC7401](https://eips.ethereum.org/EIPS/eip-7401): Parent-governed NFT nesting
    
    - [ERC7405](https://github.com/ethereum/EIPs/pull/7405/files): Portable contract accounts
    
    - [ERC7406](https://github.com/ethereum/EIPs/pull/7406/files): Multi-namespace onchain registry
    
    - [ERC7409](https://github.com/ethereum/EIPs/pull/7409/files): Public NFT emote repository
    
    - [ERC7410](https://github.com/ethereum/EIPs/pull/7410/files): ERC20 update allowance by spender
    
    - [ERC7412](https://github.com/ethereum/EIPs/pull/7412/files): On-demand offchain data retrieval
    
    - [ERC7417](https://github.com/ethereum/EIPs/pull/7418/files): Token converter (convert between ERC20 & ERC223)

* * *

### **This newsletter is made possible thanks to** [**Rysk**](https://www.rysk.finance/)

![Rysk Finance](https://weekinethereumnews.com/wp-content/uploads/2023/07/Rysk-banner-1024x245.jpg)

[Rysk Finance](https://app.rysk.finance) is an AMM for ETH options.

Rysk just launched on Arbitrum with:

- Constant onchain pricing mechanism 

- Tight spreads via deep concentrated liquidity 

Rysk's options AMM also offers _uncorrelated returns_ for liquidity providers. While not risk-free, our [automated delta hedging mechanism](https://blog.rysk.finance/unlocking-rysk-9e890390a2c3) aims to reduce risks in pursuit of superior risk-adjusted returns.

Trade options or provide liquidity for uncorrelated returns at [Rysk Finance](https://app.rysk.finance).

* * *

**Stuff for developers**

- [OpenZeppelin Contracts Wizard](https://twitter.com/openzeppelin/status/1684300974402449408) adds Foundry project download

- Deep dive into [Solady ERC1967Factory](https://www.gmhacker.com/solady-erc1967factory-deep-dive/) for deploying & managing ERC1967 proxies

- [EIP4626 contracts](https://banteg.mirror.xyz/xMsPLpgsv88NFspah0v1SyJHBk0Yp3vSyzCSznr6ZaM) (tokenized vaults) don’t all emit Transfer event on mint, deposit, burn & redeem

- Halmos [v0.1.0](https://a16zcrypto.com/posts/article/release-notes-halmos-v0-1-0/) (symbolic testing): improved performance and expanded EVM & cheatcode support

- WhatsABI [v0.6.0](https://github.com/shazow/whatsabi/releases/tag/v0.6.0) (guesses ABI from bytecode): autoload improvements & bug fixes 

- CTFs:
    - Curta CTF [sacred geometry solution](https://twitter.com/jtriley_eth/status/1683203592344473601)
    
    - [Flashbots CTF](https://ctf.flashbots.net/) August 5-7

**Security**

- EraLend on zkSync Era [$3.4 million exploit](https://rekt.news/eralend-rekt/) via read-only re-entrancy

- Conic Finance [post mortem](https://medium.com/@ConicFinance/post-mortem-eth-and-crvusd-omnipool-exploits-c9c7fa213a3d) for ETH omnipool (read-only reentrancy) & crvUSD omnipool (sandwich) exploits

**Ecosystem**

- ETHGlobal Paris [hackathon finalists](https://twitter.com/ethglobal/status/1683156559847739394)

- Etherscan [input data messages](https://twitter.com/etherscan/status/1684920660550926336), view all transactions with detected messages

**Notable at app layer**

- [Rysk Finance](https://twitter.com/ryskfinance/status/1684202975001030658) (options AMM with uncorrelated returns for LPs) live on Arbitrum \[Disclosure: Starbloom portfolio\]

- [Worldcoin](https://worldcoin.org/blog/announcements/worldcoin-project-launches) (UBI via iris scan) live on Optimism
    - Vitalik on [biometric proof of personhood](https://vitalik.eth.limo/general/2023/07/24/biometric.html)

- [Farcaster](https://twitter.com/dwr/status/1684218017486438403) adds ENS usernames

- A retrospective on [TCR Party](https://medium.com/@Obstropolos/party-on-tcr-party-af0035199b9) 

- Gas guzzler: Pond0x memecoin [allowed anyone to transfer tokens](https://twitter.com/0xQuit/status/1684982136724733952), based on a Solady mock ERC20

* * *

### Job Listings

- [Executive Director](https://www.governmentjobs.com/careers/wyoming/jobs/4126743/stc-0419-executive-director-cheyenne-or-laramie) sought by Wyoming Stable Token Commission

- EF Privacy & Scaling Explorations team seek [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US drops campaign finance charge against SBF](https://twitter.com/WatcherGuru/status/1684593024360239105) claiming that Bahamas didn't agree to that charge

- US SEC:
    - [Accounting firms warned](https://www.sec.gov/news/statement/munter-statement-crypto-072723) about liability from crypto marketing of their non-audit services
    
    - [Quantstamp settles with SEC](https://www.sec.gov/enforce/33-11215-s) for unregistered ICO, fined with proceeds to be returned

- [Couple to plead guilty for laundering $4.5B in BTC](https://unchainedcrypto.com/bitcoins-bonnie-and-clyde-aka-razzlekhan-and-dutch-reach-plea-deals-with-government/) from Bitfinex 2016 hack

- How newly launched [tokens manipulate prices though market makers](https://twitter.com/AriDavidPaul/status/1683627646633013249) so they can dump on retail

**General**

- Lazarus group suspected in payment processor exploits: $60M [AlphaPo](https://rekt.news/alphapo-rekt/) & $37M [CoinsPaid](https://coinspaid.com/tpost/0zx28tmj51-coinspaid-is-back-to-processing-after-be)

- [Apple](https://www.bleepingcomputer.com/news/apple/apple-fixes-new-zero-day-used-in-attacks-against-iphones-macs/) fixes zero-day

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-29-2023](https://weekinethereumnews.com/week-in-ethereum-news-july-29-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Aug 4-18 – [ETHGlobal Superhack](https://ethglobal.com/events/superhack) virtual

- Aug 11-13 – [ETHMunich](https://ethmunich.de/) hackathon

- Aug 15-16 – [ETHToronto](https://www.ethtoronto.ca/) & [ETHWomen](https://www.ethwomen.com/)

- Aug 15-29 – [Gitcoin Grants 18](https://twitter.com/gitcoin/status/1681747409435787264)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org/) (Buenos Aires)

- **Aug 23 –** [**KZG Ceremony**](https://ceremony.ethereum.org/) **closes (extended)**

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 31 - Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 7-9 – [ETHAccra](https://www.ethaccra.xyz/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 15-17 – [ETHChicago](https://www.ethchicago.xyz/) conference & hackathon

- **Sep 21–24 –** [**Pragma**](https://ethglobal.com/events/pragma-newyork) & [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 6-27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 13-15 – [Ethereum Kuala Lumpur](https://hack.ethkl.org/) conference & hackathon

- **Oct 21 –** [**Ethereum México**](https://twitter.com/ethereum_mexico/status/1684649652639924224)

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- **Oct 27-29 –** [**ETH Vietnam**](https://www.eth-vietnam.com/)

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) application deadline

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://lu.ma/ethbrno3)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- **Nov 16-19 –** [**Pragma**](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

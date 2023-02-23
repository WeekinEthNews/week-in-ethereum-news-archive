---
title: "Week in Ethereum News <br> December 31, 2022"
date: "2022-12-31"
---

## **Eth News and Links**

**Shapella (Shanghai + Capella) upgrade**

- EOF specification level [open issues](https://notes.ethereum.org/@ipsilon/eof1-checklist#Spec-level-Open-Issues)
    - Reminder: [EOF needs to hit January deadlines](https://twitter.com/TimBeiko/status/1600945407852703744) otherwise it will be removed

**Cancun + D-starname upgrade**

- [Deneb](https://twitter.com/protolambda/status/1608870312090955777) looks like the default winner for the CL upgrade D-starname

**Layer 1**

- [ERC4337 updated](https://twitter.com/yoavw/status/1608637361570877440) (account abstraction using alt mempool) with bundler reference implementation & compatibility test suite

- Remco: [upper bound for transaction memory](https://xn--2-umb.com/22/eth-max-mem/index.html), 32MB for 30 million gas

**Research**

- James Prestwich: [a history of the MEV community](https://medium.com/@Prestwich/mev-c417d9a5eb3d)

**Client releases**

- Execution Layer
    - Nethermind [v1.15.0](https://github.com/NethermindEth/nethermind/releases/tag/1.15.0): TraceStore plugin, ETH/67 support, fixes for JSON RPC, synchronization, networking, metrics and database corruption resilience

**Layer 2**

- Taiko zkEVM [alpha-1 testnet](https://mirror.xyz/labs.taiko.eth/-lahy4KbGkeAcqhs0ETG3Up3oTVzZ0wLoE1eK_ao5h4)

- [Optimism node on a Rock 5B ARM64 board](https://twitter.com/EthereumOnARM/status/1607373283082792961), proof of concept

- Record month for [gas consumption on mainnet by Layer 2](https://twitter.com/PaoloRebuffo/status/1608793955671605249) (validation transactions + bridges)

**EIPs/Standards**

- [EIP6220](https://github.com/ethereum/EIPs/pull/6220/files): Composable NFTs utilizing equipable parts

- [EIP6224](https://github.com/ethereum/EIPs/pull/6224/files): Contracts registry the dependency injector

- [EIP6228](https://github.com/ethereum/EIPs/pull/6228/files): Extreme ЕRС20, meta-transaction token (MTT)

- [EIP6229](https://github.com/ethereum/EIPs/pull/6229/files): Tokenized vaults with lock-in period

- [EIP6239](https://github.com/ethereum/EIPs/pull/6239/files): Semantic soulbound tokens

* * *

### **This newsletter is made possible thanks to** [**Hardhat**](https://hardhat.org/)**’s VSCode extension!**

![](https://weekinethereumnews.com/wp-content/uploads/2021/06/hardhat-rectangle-1024x325.png)

The Hardhat for Visual Studio Code extension adds comprehensive language support for Solidity to Visual Studio Code and enhances editor integration for Hardhat projects.  

Key features include code completion, go to definition, symbol renaming, and inline code validation from compiler errors/warnings. 

The extension also provides helpful code actions, hover help, and support for adding access modifiers and virtual/override keywords to function signatures. 

Get it from the [VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=NomicFoundation.hardhat-solidity) 

* * *

**Stuff for developers**

- Foundry [Chisel](https://github.com/foundry-rs/foundry/tree/master/chisel#readme): Solidity REPL

- [Etherscan contract verification API](https://twitter.com/etherscan/status/1608796718677753858) adds failure message

- [Uniswap poor oracle](https://github.com/timeless-fi/uniswap-poor-oracle#readme): flash loan proof Uniswap v3 price-out-of-range oracle

- [Norswap on ERC2535 (Diamonds)](https://twitter.com/norswap/status/1607425088491753472): only use to circumvent contract size limitations

- [Fallback](https://github.com/nathanhleung/fallback#readme): create web apps in Solidity, proof of concept

- [Huff-immutables](https://github.com/vicnaum/huff-immutables#readme): constructor-initialized immutables in Huff 

- VSCode Solidity Inspector [v0.0.3](https://github.com/PraneshASP/vscode-solidity-inspector/releases/tag/v0.0.3): view contract storage layout

- Understanding [EVM instruction boundaries](https://mirror.xyz/vicnaum.eth/zJX21EV6bjrPcL_8fnI-0zoChvBw-ZscbL7S7inroro) plus an [EVM regex decompiler](https://gist.github.com/vicnaum/492d9ccfb66dc0f50b1fd8f99239f6a7) (Perl compatible regex)

- [Noble-curves](https://github.com/paulmillr/noble-curves#readme): elliptic curves in JavaScript, zero-dependencies

- Wagmi (React hooks) [v0.10.0](https://github.com/wagmi-dev/wagmi/releases/tag/wagmi%400.10.0): WalletConnect v2 support and useWatchPendingTransactions hook

- [ENS Profile API](https://blog.indexing.co/posts/6xGR3GSQ2lY5Lpo0WRWJlqMutSt241RxdOsDg_ABXRo): access via GraphQL

**Security**

- [DeFi hacks](https://github.com/SunWeb3Sec/DeFiHackLabs#readme) reproduced using Foundry

- [Bug database in Notion](https://twitter.com/tom_eth_dev/status/1606832631282565122), 120+ high severity & 200+ medium 

**Ecosystem**

- [EF supported teams 2022 achievements](https://blog.ethereum.org/2022/12/29/supported-teams-roundup-22): the Merge plus work on withdrawals, EOF, EIP4844, KZG ceremony, RIG open problems, Portal Network, Remix and Solidity & Fe improvements

- [Most called contracts by gas in 2022](https://twitter.com/jconorgrogan/status/1607862621251817474): Uniswap v3, followed by Seaport (OpenSea)

- [Less than a third of validators](https://twitter.com/superphiz/status/1608483869182787587) are solo stakers

**Application layer**

- 1inch [Fusion mode](https://blog.1inch.io/the-1inch-network-releases-a-major-upgrade-fusion-96184d8141d3): swap using rates based on time range chosen, MEV protection, with no network fees

- [Mean Finance](https://twitter.com/mean_fi/status/1607803080430727168) dollar cost average into positions while earning yield on Euler, live on mainnet

- [Top two Solana NFT projects leaving](https://www.coindesk.com/web3/2022/12/26/solanas-top-nft-projects-degods-and-y00ts-to-migrate-chains/) for Ethereum and Polygon

* * *

### Job Listings

- Join Alchemy as the first [Engineering Manager](https://grnh.se/2837b9d35us) to build the future of web3.

- Join a16z-backed Story Protocol as a founding [smart contract developer](https://jobs.lever.co/storyprotocol/e08066d4-8d73-46ab-975c-dd5a284e1a83).

- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Fat app flippening thesis](https://zeeprime.capital/the-fappening): value accrual will flip from protocols to superapp(s)

- Mango Markets attacker [Avraham Eisenberg arrested & charged](https://storage.courtlistener.com/recap/gov.uscourts.nysd.591629/gov.uscourts.nysd.591629.1.0.pdf) \[PDF\] with commodities manipulation & fraud

**General**

- Harry Denley: [anatomy of an NFT stealer](https://twitter.com/sniko_/status/1608530448241532940)

- [Graphic card shipments](https://www.tomshardware.com/news/sales-of-desktop-graphics-cards-hit-20-year-low) hit 20-year low

- Hacker claims to be [selling 400 million users scraped Twitter data](https://www.bleepingcomputer.com/news/security/hacker-claims-to-be-selling-twitter-data-of-400-million-users/) including email & telephone

- [3Commas](https://twitter.com/YS_3Commas/status/1608202390121111552) confirms user API keys leaked after denying exploit

- [SuperNova](https://eprint.iacr.org/2022/1758): recursive proofs of multi-instruction virtual machine executions without paying for universal circuits

- [HyperPlonk](https://hackmd.io/@omershlo/rJhgKJPtj): MLE-SumCheck less hardware friendly than Plonk NTT

- [Plural Funding](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4311507): collusion-resistant Quadratic Funding mechanisms

- Vitalik: [what even is an institution?](https://vitalik.eth.limo/general/2022/12/30/institutions.html)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-31-2022](https://weekinethereumnews.com/week-in-ethereum-news-december-31-2022)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jan 8 – [Solidity developer survey](https://blog.soliditylang.org/2022/12/07/solidity-developer-survey-2022-announcement/) deadline

- Jan 11 – Flashbots [MEV Roast: Privacy](https://collective.flashbots.net/t/mev-roast-privacy-january-11th-2023/935)

- Jan 17-31 – [Gitcoin grants round](https://go.gitcoin.co/blog/announcing-the-gitcoin-alpha-tests)

- Jan 31 – [KZG ceremony grants](https://blog.ethereum.org/2022/12/15/kzg-ceremony-grants-round) deadline

- Feb 24 - Mar 1 – [ETHDenver BUIDLWeek](https://www.ethdenver.com/)

- Mar 2-5 – [ETHDenver Hackathon](https://www.ethdenver.com/)

- Mar 10-29 – [Scaling Ethereum](https://ethglobal.com/events/scaling2023) (ETHGlobal) virtual

- Mar 15-16 – [ETHDubai](https://www.ethdubaiconf.org/)

- **Mar 16-18 –** [**ETH Porto**](https://ethporto.org/)

- Mar 28-30 – [Ethereum Rio](https://www.ethereumbrasil.com/ethereumrio)

- Apr 3-6 – [Edcon](https://edcon.io/) Vienna

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- Apr 14-16 – [ETHGlobal Tokyo](https://tokyo.ethglobal.com/)

- May 26–28 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Jun 23–25 – [ETHGlobal Toronto](https://ethglobal.com/events/toronto)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–25 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

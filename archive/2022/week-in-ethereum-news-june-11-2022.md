---
title: "Week in Ethereum News <br> June 11, 2022"
date: "2022-06-11"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- [Ropsten testnet merge](https://twitter.com/parithosh_j/status/1534653280147718148) a [major success](https://twitter.com/dannyryan/status/1534928763057631232):
    - ~99% participation & proposal rates after config fixes & reboots
    - some client pairs proposing empty blocks
- Latest core devs [call video](https://www.youtube.com/watch?v=dByC5Bw8DvU&t=470s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1535310908997570560):
    - Testnets: Sepolia merge in 3 weeks, Goerli merge in 6 weeks
    - Difficulty bomb to be pushed back ~2.5 months
- [MEV boost](https://writings.flashbots.net/writings/why-run-mevboost/) creates a market for building blocks until proposer-builder separation
- [Performance benchmarking](https://medium.com/@migalabs/analysis-of-ethereum-2-consensus-clients-dfede8e0145e) of consensus layer clients.
    - TLDR: Ethereum has 5 great consensus layer clients: Lighthouse, Lodestar, Nimbus, Prysm & Teku
- [Merge upgrade checklist](https://www.coincashew.com/coins/overview-eth/ethereum-merge-upgrade-checklist-for-home-stakers-and-validators) for solo stakers

**EIPs/Standards**

- [EIP5143](https://github.com/ethereum/EIPs/pull/5143/files): Slippage protection for Tokenized Vault
- [EIP5139](https://github.com/ethereum/EIPs/pull/5139/files): Remote Procedure Call provider lists

**Layer2**

- [Aztec](https://twitter.com/aztecnetwork/status/1535024615969263616) shipping delayed due to transaction size difficulties
- L2 transaction finality [explainer](https://twitter.com/bkiepuszewski/status/1533347284817174528)

* * *

### **This newsletter is made possible thanks to** [**Karma**](https://www.showkarma.xyz/)**!**

![Karma banner](https://weekinethereumnews.com/wp-content/uploads/2022/06/wie-karma-banner-1024x341.png)

[](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Ffdf97a4e-d7f7-4229-bdf8-cf481e04240a_1500x500.png)

[Karma](http://www.showkarma.xyz/) is building a reputation system for DAO contributors. We aggregate DAO activity (currently over [25 DAO](http://www.showkarma.xyz/daos) integrations and 25k [contributors](http://www.showkarma.xyz/#search-profile)!) and work with your community to tailor the score to the needs of your DAO. 

Are you worried that your tokenholders are choosing DAO delegates who don’t actively vote and engage in governance? [Get in touch with us](https://docs.google.com/forms/d/e/1FAIpQLSdyJGG1CK2mzU0jc8FgDaeJyv-zzn6BeSOavfIh3UqeJWiZnA/viewform) to help your tokenholders make informed decisions.

* * *

**Stuff for developers**

- Remix [v0.24.0](https://medium.com/remix-ide/remix-0-24-0-release-4baf7361d1fc): project templates, Solidity compiler config file option, publish code to specified IPFS endpoint
- [Otterscan](https://twitter.com/wmitsuda/status/1533640148444925952) supports Erigon 2 alpha
- Ropsten node [docker compose template](https://gist.github.com/wmitsuda/ce2f5744fffcf90ddf8f07f032d3319c) with Erigon-Prysm and Otterscan 
- [MultiFaucet](https://faucet.paradigm.xyz/) increased to 100 testnet ETH for Ropsten & Goerli testing
- Etherscan [ERC1155 token transfer events](https://twitter.com/etherscan/status/1534141366590373888) endpoint
- [web3 scaffold](https://github.com/holic/web3-scaffold#readme): Foundry, Next.js, RainbowKit, example subgraph
- RainbowKit [CLI](https://twitter.com/markdalgleish/status/1533980822554177541): scaffold RainbowKit, wagmi & Next.js app
- [Ethereum Data Warehouse guide](https://tokenflow.live/blog/user-guide) to run queries on NFT mints & trades
- OxPARC [zkREPL](https://0xparc.org/blog/zkrepl): zkSNARK web based dev environment

**Security**

- [20m OP transferred to Wintermute on Optimism](https://gov.optimism.io/t/message-to-optimism-community-from-wintermute/2595) but the market maker had not deployed their multisig.  Hacker sold 1m OP and returned 18m OP; 1inch’s Anton Bukov [deployed 22k](https://twitter.com/k06a/status/1534849386819334145) more Gnosis Safes with ownership to Optimism multisig
- Aurora [DELEGATECALL vulnerability](https://aurora.dev/blog/aurora-mitigates-its-inflation-vulnerability) disclosed, $200 million was at risk, $6 million bounty paid
- OpenSea [Wyvern vulnerability](https://nft.mirror.xyz/VdF3BYwuzXgLrJglw5xF6CHcQfAVbqeJVtueCr4BUzs) disclosed, $3 million bounty paid
- Sense [oracle manipulation vulnerability](https://medium.com/sensefinance/disclosure-fixing-a-critical-bug-in-the-sense-space-oracle-42a0bed65bc2) disclosed, $50k bounty paid

**Ecosystem**

- [Devcon](https://blog.ethereum.org/2022/06/06/devcon-vi-details/) Bogotá:
    - applications open for builder, student, speaker & volunteer tickets 
    - ticket sales in waves from July 18 and raffle+auction 
    - Ethereum aligned supporter program rather than sponsors 
    - new [Devcon website](https://devcon.org/)
- Etherscan [method filters](https://twitter.com/etherscan/status/1533778322551115776) support EOAs to search for specific types of transactions

**Enterprise**

- [Paypal](https://newsroom.paypal-corp.com/2022-06-07-PayPal-Users-Can-Now-Transfer-Send-and-Receive-Bitcoin-Ethereum-Bitcoin-Cash-and-Litecoin) supports send & receive to ETH wallets for US users

**Application layer**

- Hop [airdrop claims](https://twitter.com/HopProtocol/status/1534963591698427909) open on mainnet
- Synthetix [V3GM](https://blog.synthetix.io/v3gm/): governance on Optimism using combined mainnet & L2 voting power
- [Uniswap research](https://uniswap.org/blog/fee-returns): fee returns on non-rebalancing v3 positions better than v2 by 54% on average
- [Forta token](https://forta.org/blog/fort-airdrop/) (security & operational monitoring), web3 devs, multisig signers & Ethernaut players eligible for airdrop \[Disclosure: I’m eligible as a contributor\]
- Kate Sills: [soulbound tokens should be signed claims](https://katelynsills.com/blockchain/soulbound-tokens/)
- [ApeCoin DAO](https://snapshot.org/#/apecoin.eth/proposal/0x367eecaffc20976a4f913154eceb61279793b06ac0ad93ab948d2d3b207ff860) votes to stay Ethereum by a half a million vote margin

* * *

### **Job Listings**

- [People Operations Lead](https://jobs.lever.co/ethereumfoundation/8046bbe5-6343-4ecf-8296-37dc2a5bf915?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) at EF
- [Hiring Coordinator](https://jobs.lever.co/ethereumfoundation/7f5bf10b-ea68-4364-a378-e34ae345a212?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) wanted by EF
- EF: [generalist developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) to drive strategic ecosystem initiatives
- Sourcify: [TypeScript/nodejs developer](https://jobs.lever.co/ethereumfoundation/db85cf1d-6ffd-42a6-8f0d-f5a91c6ddf4a?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) wanted
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)

**Job listings: $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet/Arbitrum/Optimism. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Jake Chervinsky](https://twitter.com/jchervinsky/status/1534158129331589123): US Senator Lummis proposed crypto regulatory framework bill would make CFTC primary spot market regulator rather than SEC
- Paradigm: [DAO legal entity matrix](https://daos.paradigm.xyz/)
- [Lido proposes solving the principal-agent problem](https://research.lido.fi/t/ldo-steth-dual-governance/2382) by giving stETH holders a veto
- ZachXBT: [Players Only NFT rugpull](https://twitter.com/zachxbt/status/1534537264637825024) by pro athletes
- Coindesk: US SEC [investigating Luna collapse](https://www.coindesk.com/policy/2022/06/09/sec-investigating-company-behind-terrausd-stablecoin-report/)
- Bloomberg: US SEC [investigating Binance’s BNB](https://www.bloomberg.com/news/articles/2022-06-06/us-probes-binance-over-token-that-is-now-world-s-fifth-largest) sale

**General**

- Groth-Sahai proofs [explainer](https://crypto.ethereum.org/blog/groth-sahai-blogpost)
- MongoDB [queryable encryption](https://www.mongodb.com/blog/post/mongodb-releases-queryable-encryption-preview) preview

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-june-11-2022](https://weekinethereumnews.com/week-in-ethereum-news-june-11-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 23 – [Gitcoin Grants Round 14](https://gitcoin.co/grants/) ends **(support** [**Week in Eth News**](https://gitcoin.co/grants/2785/week-in-ethereum-news)**)**
- Jun 24-26 – [ETH NYC](https://nyc.ethglobal.co/) (ETH Global)
- **Jun 27 –** [**Devcon speaker**](https://devcon.org/en/applications/) **applications close**
- **Jun 30 –** [**Devcon discounted ticket**](https://devcon.org/en/tickets/) **applications close**
- Jul 1 – [Data Availability Sampling](https://github.com/ethereum/requests-for-proposals/blob/master/open-rfps/das.md) proposals due
- Jul 6-8 – [ETHBarcelona](https://ethbarcelona.com/)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- **Jul 18 –** [**Devcon wave 01 tickets**](https://devcon.org/en/tickets/)
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 5-13 – [ETH Seoul](https://2022.ethseoul.org/)
- Aug 8-10 – [ETHToronto](https://www.ethtoronto.ca/)
- Aug 11-14 – [ETH LATAM](https://twitter.com/ethlatam/status/1524146640474587137) (Buenos Aires)
- Aug 19-21 – [ETHMexicoCity](https://mexico.ethglobal.com/) (ETH Global)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 28 – [DeFi San Francisco](https://2022.defi-sf.com/) summit
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev/) (hackathon & conference)
- Sep 2-28 – [ETHOnline](https://online.ethglobal.com/')
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- **Sep 8-10 –** [**ETHSantiago**](https://twitter.com/EthereumStgo)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- **Sep 16-18 -** [**EthBerlin**](https://ethberlin.ooo/)
- Sep 27-29 – [Ethereum SP](https://twitter.com/Ethereum_Brasil/status/1530320916667895808) (São Paulo)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 18-20 – ETHGlobal [Web3 Weekend](https://web3weekend.ethglobal.com/)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

---
title: "Week in Ethereum News <br> June 25, 2022"
date: "2022-06-25"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- [Mainnet-shadow-fork-7](https://notes.ethereum.org/PhbNw_cGSQ-VKqzGl4bPcg?view#mainnet-shadow-fork-7) merged with caveats: known [Besu concurrency issue](https://hackmd.io/@RoboCopsGoneMad/B1reW1G9c) and Erigon issue with shadow forks

**Mainnet execution layer**

- **Update your nodes for** [**Gray Glacier upgrade**](https://ethernodes.org/gray_glacier)
- Latest core devs [call video](https://www.youtube.com/watch?v=qu5idP-JLyQ&t=60s). Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1540328722892480513) and [Christine Kim](https://twitter.com/christine_dkim/status/1540382924440121344):
    - Sepolia testnet merge planned for July 6
    - Mainnet shadow fork 8 planned for first week in July
    - Calls moving to Thursdays after next call
- Erigon [v2022.06.05-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.06.05): regression fixes
- Geth making progress on [historical state pruning](https://twitter.com/peter_szilagyi/status/1539183240799563776)
- KZG ceremony [call video](https://www.youtube.com/watch?v=h2J6c95wk9k): plan to start ceremony in November (3 month general participation + 1 month special participation), use output in clients from March
- [NiceNode](https://twitter.com/NiceNodeApp/status/1538233402859458562) (interface to run a client) adds multi-client support
- Vitalik: [possible roadmap for account abstraction](https://notes.ethereum.org/@vbuterin/account_abstraction_roadmap) using ERC4337 and adding features to protocol to make account abstraction the default

**Proof of Stake consensus layer**

- [EF seeks proposals](https://github.com/ethereum/requests-for-proposals/blob/master/open-rfps/staking-operator-docs.md) to create technical documentation for staking operators
- Nimbus [v22.6.0](https://github.com/status-im/nimbus-eth2/releases/tag/v22.6.0): Ropsten & Sepolia testnet support, UX improvements & fixes
- Prysm [v2.1.3-rc.4](https://github.com/prysmaticlabs/prysm/releases/tag/v2.1.3-rc.4): Sepolia testnet support and Panda Merge banner
- [Lido expands node operators](https://blog.lido.fi/additions-to-ethereum-node-operator-set-wave-4/), includes four client teams

**EIPs/Standards**

- [EIP5169](https://github.com/ethereum/EIPs/pull/5169/files): Client script URI for token contracts
- [EIP5170](https://github.com/ethereum/EIPs/pull/5170/files): Asserting authenticity of client script for token contracts
- [EIP5173](https://github.com/ethereum/EIPs/pull/5173/files): NFT future rewards

* * *

### **This newsletter is made possible thanks to** [**SpeedRunEthereum**](https://speedrunethereum.com/)**!**

![SpeedRunEthereum](https://weekinethereumnews.com/wp-content/uploads/2022/04/Screenshot-from-2022-04-01-15-39-52.png)

[](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fbcf44b51-bc5e-4dc8-9233-4c4e51f07802_769x208.png)

Are you a web2 dev who wants to get into web3?  

The best way to go from _zero_ to **hero** is [SpeedRunEthereum.com](https://speedrunethereum.com/).

Learn how to build on Ethereum; the superpowers and the gotchas.

Then [speed run Ethereum](https://speedrunethereum.com/) by testing your skills in a [series of challenges](https://speedrunethereum.com/challenge/simple-nft-example) and [join web3](https://twitter.com/austingriffith/status/1493688828661432325).

* * *

**Stuff for developers**

- [Testnet shutdown timeline](https://blog.ethereum.org/2022/06/21/testnet-deprecation/): Kiln after mainnet Merge, Ropsten Q4, Rinkeby Q2-Q3 2023
- Sepolia testnet [faucet](https://sepoliafaucet.net/)
- EthereumJS VM [v5.9.3](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs%2Fvm%405.9.3) Gray Glacier support
- [Foundry x Huff](https://github.com/huff-language/foundry-huff#readme): compile & test Huff contracts using Foundry
- [NFT gas optimization](https://twitter.com/w1nt3r_eth/status/1538229135897554944) by encoding metadata into the token ID
- [DeFi Hacks](https://github.com/SunWeb3Sec/DeFiHackLabs/#readme): reproduce DeFi incidents using Foundry
- Damn Vulnerable DeFi (CTF) [Foundry version](https://github.com/nicolasgarcia214/damn-vulnerable-defi-foundry#readme) implements all levels
- Nethereum [v4.6.1](https://github.com/Nethereum/Nethereum/releases/tag/4.6.1) (.Net library): MetaMask nuget package, Proof of Humanity integration

**Security**

- Horizon bridge between Ethereum & Harmony [$100 million exploit](https://rekt.news/harmony-rekt/), 2 of 5 multisig had addresses compromised
- Namecheap DNS attack for [DeFi Saver](https://twitter.com/DeFiSaver/status/1540300787988979713), [Convex Finance](https://twitter.com/ConvexFinance/status/1540436217438904320) and [Ribbon Finance](https://twitter.com/ribbonfinance/status/1540250826156871681); check your token approvals

**Ecosystem**

- EF Fellowship Program [cohort #2 applications open](https://blog.ethereum.org/2022/06/21/fellowship-cohort-2-applications-roundup/)
- Wallet devs [call video](https://www.youtube.com/watch?v=0fMUrgdgI_g) and [notes](https://twitter.com/_SamWilsn_/status/1540136627116417024): discussions on EIP5139 RPC provider lists, interoperability testing and multi wallet support in a browser
- Metamorphic contract [detector](https://a16zcrypto.com/metamorphic-smart-contract-detector-tool/)
- [Etherscan watch list](https://twitter.com/etherscan/status/1540300542744100864) adds ERC721 & ERC1155 token transfer support

**Enterprise**

- [Shopify token gated merch](https://www.shopify.com/tokengated-commerce) via Shop app and in-store POS
- [eBay acquired KnownOrigin](https://www.ebayinc.com/stories/news/ebay-acquires-leading-nft-marketplace-knownorigin/) (NFT marketplace)

**Application layer**

- [Uniswap Labs acquired Genie](https://uniswap.org/blog/genie) (NFT market aggregator) to expand into NFTs
- LooksRare [conditional listing](https://twitter.com/LooksRare/status/1539957437729742848): list two items and automatically cancel the listing when one item sells
- [Bancor](https://rekt.news/bancor-lp-rekt/) paused Impermanent Loss Protection due to market conditions
- [Timeless](https://blog.timelessfi.com/posts/mainnet-launch/) (yield market protocol) live on mainnet
- [Arbitrum Odyssey](https://twitter.com/arbitrum/status/1539292126105706496?s=20&t=D-8ZJNjnRjUQHabioXX5Yg): 8 week promotion to encourage bridging and usage of selected projects using NFT rewards

* * *

### **Job Listings**

- GridPlus hiring a [Go/protocol dev for the private, scalable PhononDAO](https://gridplus.io/pages/careers#PhononEngineer)
- [People Operations Lead](https://jobs.lever.co/ethereumfoundation/8046bbe5-6343-4ecf-8296-37dc2a5bf915?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) at EF
- [Status](https://status.im/) is looking for a [Senior Rust Engineer](https://jobs.status.im/?gh_jid=3693623) for [Waku](https://vac.dev/)
- Taiko ZKRollup: [hiring senior golang & rust backend developers](https://taiko.xyz/career).
- EF: [generalist developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) to drive strategic ecosystem initiatives

**Job listings: $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet/Arbitrum/Optimism. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [UK Treasury](https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/1083351/MLRs_SI_2022_-_Consultation_Response_final.pdf) \[PDF\] removes proposed KYC requirement for self hosted wallet transfers
- Erik Voorhees: [benefits of being a DAO for ShapeShift](https://www.moneyandstate.com/blog/way-of-the-dao)
- [Tether launching GBPT](https://tether.to/en/tether-to-launch-gbpt-tether-tokens-pegged-to-the-british-pound-sterling/) (British Pound sterling stablecoin)
- World Economic Forum: [DAOs whitepaper](https://www3.weforum.org/docs/WEF_Decentralized_Autonomous_Organizations_Beyond_the_Hype_2022.pdf) \[PDF\]

**General**

- MEGA cloud storage [vulnerabilities disclosed](https://mega-awry.io/) 
- [Decrypting a message](https://twitter.com/bert_hu_bert/status/1539153322321526785) from 1914

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-june-25-2022](https://weekinethereumnews.com/week-in-ethereum-news-june-25-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Jun 27 – [Devcon speaker](https://devcon.org/en/applications/) applications close
- Jun 29 – [Gray Glacier upgrade](https://ethernodes.org/gray_glacier) (block 15,050,000)
- Jun 30 – [Devcon discounted ticket](https://devcon.org/en/tickets/) applications close
- Jul 1 – [Data Availability Sampling](https://github.com/ethereum/requests-for-proposals/blob/master/open-rfps/das.md) proposals due
- Jul 6-8 – [ETHBarcelona](https://ethbarcelona.com/)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- **Jul 8 –** [**Staking operator documentation**](https://github.com/ethereum/requests-for-proposals/blob/master/open-rfps/staking-operator-docs.md) **proposals due**
- **Jul 17 –** [**EF Fellowship program**](https://fellowship.ethereum.foundation/) **applications close**
- Jul 18 – [Devcon wave 01 tickets](https://devcon.org/en/tickets/)
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- **Jul 22-24 –** [**EthCC Hackathon**](https://ethcchack.com/) **(Paris)**
- Aug 5-13 – [ETH Seoul](https://2022.ethseoul.org/)
- Aug 8-10 – [ETHToronto](https://www.ethtoronto.ca/)
- **Aug 11-13 –** [**ETH LATAM**](http://ethlatam.org/) **(Buenos Aires)**
- Aug 19-21 – [ETHMexicoCity](https://mexico.ethglobal.com/) (ETH Global)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 27-28 – [HackSummit](https://sf.hacksummit.org/) (San Francisco)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev/) (hackathon & conference)
- Sep 2-28 – [ETHOnline](https://online.ethglobal.com/')
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 8-10 – [ETHSantiago](https://twitter.com/EthereumStgo)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Sep 16-18 - [EthBerlin](https://ethberlin.ooo/)
- Sep 27-29 – [Ethereum SP](https://twitter.com/Ethereum_Brasil/status/1530320916667895808) (São Paulo)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- Oct 10 – [DeFi Bogotá](https://2022.defibogota.org/)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 18-20 – ETHGlobal [Web3 Weekend](https://web3weekend.ethglobal.com/)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

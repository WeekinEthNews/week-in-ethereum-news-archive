---
title: "Week in Ethereum News <br> July 2, 2022"
date: "2022-07-02"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- The second of three public testnets to merge will occur next week, with [Sepolia to turn off PoW forever](https://blog.ethereum.org/2022/06/30/sepolia-merge-announcement/) sometime [between Saturday and Wednesday](https://bordel.wtf/), depending on hashpower
- [Mainnet-shadow-fork-8](https://twitter.com/abcoathup/status/1542417002173992961) merges July 5

**Mainnet execution layer**

- Gray Glacier upgrade (delay difficulty bomb) [successful](https://twitter.com/TimBeiko/status/1542463390475423745);
    - [One block on wrong chain](https://twitter.com/vdWijden/status/1542489519030689795), estimate 0.2% of hash rate didn’t upgrade
    - Reminder: [OpenEthereum (ex-Parity) client](https://twitter.com/koeppelmann/status/1542463408880189442) is deprecated
- Sepolia testnet releases (Besu need to set TTD override):
    - Geth [v1.10.20](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.20)
    - Nethermind [v1.13.4](https://github.com/NethermindEth/nethermind/releases/tag/1.13.4): snap sync now default
    - Erigon [2022.07.01-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.07.01)

**Proof of Stake consensus layer**

- PoS implementers [call video](https://www.youtube.com/watch?v=Fid8hTxkRHM&t=358s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/HJNt57iq5) and [Christine Kim](https://twitter.com/christine_dkim/status/1542947591951769601)
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220701)
- Sepolia testnet releases:
    - Nimbus [v22.6.1](https://github.com/status-im/nimbus-eth2/releases/tag/v22.6.1)
    - Teku [v22.6.1](https://github.com/ConsenSys/teku/releases/tag/22.6.1)
    - Lodestar [v0.39.0](https://github.com/ChainSafe/lodestar/releases/tag/v0.39.0)
    - Lighthouse [v2.3.2-rc.0](https://github.com/sigp/lighthouse/releases/tag/v2.3.2-rc.0)
    - Prysm [v2.1.3-rc.4](https://github.com/prysmaticlabs/prysm/releases/tag/v2.1.3-rc.4)
- [Lido overwhelmingly votes against](https://snapshot.org/#/lido-snapshot.eth/proposal/0x10abedcc563b66b1adee60825e78c387105110fa4a1e7354ab57bc9cc1e675c2) self limiting despite [warning from Danny Ryan](https://notes.ethereum.org/@djrtwo/risks-of-lsd)
- Ben Edgington’s Upgrading Ethereum book [chapter on aggregator selection](https://eth2book.info/altair/part2/building_blocks/aggregator)
- [Prototype validator](https://twitter.com/jcrtp_eth/status/1542681842469437446) using Rock5 ARM board uses 5 watts (8 watts when syncing)
- Vitalik’s [approaches to cap validator set size](https://notes.ethereum.org/@vbuterin/validator_set_size_capping) argues in favor of a variable minimum balance

**Layer2**

- Arbitrum [two-dimensional gas fees](https://medium.com/offchainlabs/understanding-arbitrum-2-dimensional-fees-fd1d582596c9): L1 calldata fees + L2 computational usage
- [Optimism testnet](https://dev.optimism.io/kovan-to-goerli/) migrating from Kovan to Goerli

**EIPs/Standards**

- [EIP5185](https://github.com/ethereum/EIPs/pull/5185/files): NFT updatable metadata extension
- [EIP5187](https://github.com/ethereum/EIPs/pull/5187/files): Extending ERC1155 with rentable usage rights
- [EIP5189](https://github.com/ethereum/EIPs/pull/5189/files): Account Abstraction via Endorsed Operations
- [EIP5192](https://github.com/ethereum/EIPs/pull/5192/files): Minimal Soulbound NFTs

* * *

### **This newsletter is made possible thanks to Starbloom Ventures!**

![Starbloom Ventures](https://weekinethereumnews.com/wp-content/uploads/2021/11/Screenshot-from-2021-11-19-15-25-51.png)

[](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Ffce876fc-5521-4367-aa34-8a2f6fd42fd3_613x313.png)

Starbloom Ventures is a **first round** venture fund founded by [Evan Van Ness](https://twitter.com/evan_van_ness) to invest in the future of web3. 

We pledge 10% of investing profits to support Ethereum public goods.

* * *

**Stuff for developers**

- [Solenv](https://github.com/memester-xyz/solenv#readme): load .env files in Foundry Solidity scripts and tests 
- Nader Dabit: [Foundry cheatsheet](https://github.com/dabit3/foundry-cheatsheet#readme)
- [Deep dive into event logs](https://noxx.substack.com/p/evm-deep-dives-the-path-to-shadowy-16e): topics and Bloom filters
- [NFT contract common patterns](https://www.solidnoob.com/blog/good-nft-contract-patterns): avoid ERC721Enumerable, ERC721A for batch mints, mint not safeMint, Merkle tree allowlists and upgradeable metadata
- [Validate king/knight chess move](https://twitter.com/fiveoutofnine/status/1542274004949647360) in Solidity using bit shifting
- [DeFiVulnLabs](https://github.com/SunWeb3Sec/DeFiVulnLabs#readme): code snippets of common vulnerabilities
- [EVM trivia](https://twitter.com/Zer0dots/status/1541274904712171520): 7 questions and answers
- wagmi [v0.5](https://twitter.com/wagmi_sh/status/1541960443232927744) (Reach Hooks library): connection status callbacks, multicall & batched reads and pagination
- 0xPARC: [on-chain procedural generation](https://0xparc.org/blog/procgen) and Perlin noise to create game worlds

**Security**

- XCarnival [$3.8 million exploit](https://xcarnival-lab.medium.com/xcarnival-has-got-1-467-eth-back-the-security-agencies-have-tentatively-determined-the-hackers-3ea05ad134ae), withdrawn pledged NFT was used as collateral, attacker negotiates [1500 ETH bounty](https://twitter.com/XCarnival_Lab/status/1541226298399653888)
- Quixotic NFT marketplace [$145k exploit](https://twitter.com/quixotic_io/status/1543018810625646593) on Optimism, approved ERC20 tokens stolen, users refunded, Stratos on Arbitrum not affected
- [DNS hijack](https://twitter.com/Mudit__Gupta/status/1542840515292532736) of Polygon & Fantom public RPC gateways provided by Ankr

**Ecosystem**

- ETHGlobal [ETH NYC hackathon finalists](https://twitter.com/ethglobal/status/1541156302780612619)
- Devcon [ticket auction & raffle](https://blog.ethereum.org/2022/06/28/devcon-vi-auction-raffle-speaker/) on Arbitrum, minimum bid 0.25 ETH, refundable minus 2% Sybil resistance fee

**Application layer**

- Arbitrum [Odyssey promotion paused](https://twitter.com/arbitrum/status/1542159105946787840) due to [high gas fees](https://twitter.com/Agusx1211/status/1542459352744955905) from capacity throttling, will resume after Nitro upgrade
- Gitcoin grants [round 14 recap](https://gitcoin.co/blog/gr14-results/), $4.9 million in grants
- Lyra [Avalon](https://blog.lyra.finance/avalon-is-live/) (options trading) live on Optimism
- [Karma](https://twitter.com/showkarma_xyz/status/1542181597377699840) DAO reputation NFT badge minting \[Disclosure: Starbloom portfolio\]
- [Rentable v2](https://medium.com/rentable/rentable-v2-rentals-everywhere-f909256ddb2d) is live: yield on NFTs if someone wants to rent it
- Governance drama at MakerDAO over a disagreement on real world assets between [Rune](https://twitter.com/RuneKek/status/1542969283659153408) (who won) and [Luca Prosperi](https://dirtroads.substack.com/p/-42-valkyrie-makerdao-and-our-side) (who lost), while [Nikolai](https://forum.makerdao.com/t/what-i-do-and-dont-think-about-current-votes-and-how-why-i-plan-to-vote/16059) is generally against all of it

* * *

### **Job Listings**

- [Nexus Mutual: Frontend/Solidity](https://nexusmutual.recruitee.com/): Help build the web3 Risk Marketplace 
- [Status](https://status.im/) is looking for a [Senior Rust Engineer](https://jobs.status.im/?gh_jid=3693623) for [Waku](https://vac.dev/)
- [Hiring Coordinator](https://jobs.lever.co/ethereumfoundation/7f5bf10b-ea68-4364-a378-e34ae345a212?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) wanted by EF
- Taiko ZKRollup: [zkEVM researchers/developers](https://taiko.xyz/career) wanted.
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)
- GridPlus hiring a [Go/protocol dev for the private, scalable PhononDAO](https://gridplus.io/pages/careers#PhononEngineer)

**Job listings: $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet/Arbitrum/Optimism. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- EU agrees: 
    - [Markets in Crypto-Assets framework](https://twitter.com/ernesturtasun/status/1542591815546707970) (MICA): stablecoin regulation requires isolated reserves and cap of 200 million euro transactions a day
    - [Transfer of Funds Regulation](https://twitter.com/ernesturtasun/status/1542217821958115332) (TFR): travel rule requires verification for all transfers between custodial wallets & transfers to non-custodial wallets above 1000 euro; no requirements for transfers between non-custodial wallets 
- CoinFlex announces plan to [tokenize $47m in bad debt via rvUSD](https://twitter.com/MarkDavidLamb/status/1541571519503024129).  Rumors swirl that it’s Roger Ver. RV flatly [denies and says they owe him money](https://twitter.com/rogerkver/status/1541822377461415936).  In response, Coinflex CEO explicitly [names Ver and repeats claims](https://twitter.com/MarkDavidLamb/status/1541831697787928576) of being owed $47m 
- [BlockFi](https://blockfi.com/a-message-from-our-founders-july-2022) agrees to sell to FTX for pennies on the dollar in return for $400m revolving credit line
- [Voyager suspends withdrawals](https://www.investvoyager.com/blog/voyager-update-july-1-2022/) after 3AC defaults on $650 million loan
- US DOJ [charges six people for crypto-related fraud](https://www.justice.gov/opa/pr/justice-department-announces-enforcement-action-charging-six-individuals-cryptocurrency-fraud) \[Editor’s note: never heard of any of the schemes before\]

**General**

- [OpenSea](https://opensea.io/blog/safety-security/important-update-on-email-vendor-security-incident/) email data breach
- [PLONK implementation](https://twitter.com/rel_Aztec/status/1542474186664210432) missed randomization, now fixed

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-2-2022](https://weekinethereumnews.com/week-in-ethereum-news-july-2-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- **Jul 5 –** [**Devcon speaker**](https://devcon.org/en/applications/) **applications close**
- **Jul 5-14 –** [**Devcon ticket auction & raffle**](https://blog.ethereum.org/2022/06/28/devcon-vi-auction-raffle-speaker/)
- Jul 6-8 – [ETHBarcelona](https://ethbarcelona.com/)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 8 – [Staking operator documentation](https://github.com/ethereum/requests-for-proposals/blob/master/open-rfps/staking-operator-docs.md) proposals due
- **Jul 15 –** [**Merge community call #5**](https://github.com/ethereum/pm/issues/564)
- Jul 17 – [EF Fellowship program](https://fellowship.ethereum.foundation/) applications close
- Jul 18 – [Devcon wave 01 tickets](https://devcon.org/en/tickets/)
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Jul 22-24 – [EthCC Hackathon](https://ethcchack.com/) (Paris)
- Aug 5-13 – [ETH Seoul](https://2022.ethseoul.org/)
- Aug 8-10 – [ETHToronto](https://www.ethtoronto.ca/)
- Aug 11-13 – [ETH LATAM](http://ethlatam.org/) (Buenos Aires)
- Aug 19-21 – [ETHMexicoCity](https://mexico.ethglobal.com/) (ETH Global)
- **Aug 20 –** [**Paradigm CTF**](https://twitter.com/paradigm_ctf/status/1542277548670758912) **starts**
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

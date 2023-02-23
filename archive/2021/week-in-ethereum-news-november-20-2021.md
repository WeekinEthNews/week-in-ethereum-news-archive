---
title: "Week in Ethereum News <br> November 20, 2021"
date: "2021-11-20"
---

## **Eth News and Links**

**Mainnet execution layer**

- Trent: miners should plan for [PoW to end in 3-6 months](https://twitter.com/trent_vanepps/status/1460994206223290378)
- PoW switch off [second community call](https://github.com/ethereum/pm/issues/419) December 3, for infrastructure providers, wallet and application developers
- Erigon [v2021.11.03](https://github.com/ledgerwatch/erigon/releases/tag/v2021.11.03): bug fixes, continuing to stabilize beta
- Besu [v21.10.2](https://github.com/hyperledger/besu/releases/tag/21.10.2)
- Erigon [reduced scope of v2](https://twitter.com/ErigonEth/status/1461623643880964098): stopping work on consensus engine separation as PoS testnets can replace PoW and PoA testnets
- Nimbus [creating an execution layer client](https://our.status.im/nimbus-execution-layer/), so that when we turn off proof of work you can run Nimbus for execution and consensus layers
- Piper Merriam’s [Aperture Portal Network update](https://snakecharmers.ethereum.org/the-aperture-vol-3/), focused on getting a live testnet

**EIPs/Standards**

- [EIP NFTs](https://eipnft.io/): authors of finalized EIPs can mint an NFT

**Proof of Stake consensus layer**

- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_211119) (or [What’s New in Consensus Layer](https://consensuslayer.news/) if you prefer, thanks to Proto, but please open both)
- PoS [implementers call](https://www.youtube.com/watch?v=31Jxh9_xXvY&t=142s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/B1Ip90mdt): multi-client devnet started, discussion on total transition difficulty (TTD) override
- Vitalik: [Casper FFG with backoff](https://ethresear.ch/t/casper-ffg-with-backoff/11294)

**Layer2**

- Celer cBridge [v2.0](https://blog.celer.network/2021/11/17/cbridge-2-0-mainnet-launch-the-next-step-to-a-seamless-interoperable-future/) live on mainnet, one click user experience and LPs don’t need to run a cBridge node
- [StarkNet Alpha 4](https://medium.com/starkware/alpha-4-6b572072d80b) (release candidate for mainnet): adds token bridges, block hash, self contract address & updates contract address calculation
- [Polygon Miden](https://blog.polygon.technology/polygon-announces-polygon-miden-a-stark-based-ethereum-compatible-rollup): zk virtual machine in Rust for STARK based zk rollup, led by Bobbin Threadbare (former Facebook's lead ZK researcher & creator of Winterfell), alpha
- [Binance](https://www.binance.com/en/support/announcement/192e0315a7744dcfb8dede7453884c73) adds direct deposit to Arbitrum One rollup with withdrawals to be added later

* * *

### **This newsletter is made possible thanks to [Starbloom Ventures](https://twitter.com/starbloomvent)!**

![Starbloom Ventures](https://weekinethereumnews.com/wp-content/uploads/2021/11/Screenshot-from-2021-11-19-15-25-51.png)

Starbloom Ventures is a new early-stage venture fund by Evan Van Ness and James Fickel to invest in the future of web3. 

Check out our [announcement tweetstorm](https://twitter.com/evan_van_ness/status/1461840784819425288).

We’re pledging 10% of profits to support Ethereum public goods.

* * *

**Stuff for developers**

- Annual [Solidity developer survey](https://docs.google.com/forms/d/e/1FAIpQLSc5iacmGfzHfAAgQK3hQVxIXXKMImYbQ5tzi33BiMwaBvhbFQ/viewform) \[Google form\]
- web3.js [v1.6.1](https://medium.com/chainsafe-systems/web3-js-solid-foundations-create-stable-structures-1674514fe35): breaking change in web3.eth.getBlock output, open discussion on auto fill of gas price if not set in sendTransaction
- eth-sdk [v0.2.2](https://github.com/dethcrypto/eth-sdk/releases/tag/%40dethcrypto%2Feth-sdk%400.2.2) (generate type-safe contract SDK via the address): option to use Sourcify as ABI source
- [Uniswap v3 geometric mean TWAP oracle manipulation](https://twitter.com/euler_mab/status/1459314402059034634), technically possible but under restrictive conditions
- [OpenZeppelin Defender](https://blog.openzeppelin.com/defender-complete-access/) contract automation, now free for teams
- [Gelato Ops](https://medium.com/gelato-network/introducing-gelato-ops-web3s-multi-chain-smart-contract-automation-hub-713dbcf2dad1): contract task automation
- [MultiFaucet](https://faucet.paradigm.xyz/): Ropsten, Kovan, Görli and Optimism Kovan testnet faucet via Twitter sign in, dripping ETH, wETH, DAI and ERC721 NFTs
- [siwe](https://github.com/spruceid/siwe): Sign-In with Ethereum library, alpha with example integration

**Security**

- [ERC1155Supply](https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-wmpv-c2jp-j2xg) low severity OpenZeppelin Contracts vulnerability, total supply lower than circulating tokens during callback when minting
- [Using Flashbots to recover ENS tokens](https://medium.com/@kanewallmann_71759/recovering-assets-from-a-hacked-account-with-flashbots-bfe920435fb6) from a compromised mnemonic

**Ecosystem**

- watchtheburn [v3](https://watchtheburn.com/): insights with real-time historical totals, basefee increasing and net issuance decreasing every month
- Galaxy Digital: [visualization for 100 days of EIP1559](https://docsend.com/view/jngzufksntmpbgej) \[PDF\], miner revenue increased 33% in dollar terms, 56% of ETH issuance burnt
- [Vitalik’s review](https://vitalik.ca/general/2021/11/16/retro1.html) of Optimism’s retroactive public goods funding round: increase number & diversity of voters, 2 layer nomination process, secret ballots, more discussion and change reward formula
- [Flashbots Protect](https://twitter.com/bertcmiller/status/1461754056913862665): view status of pending transactions on Etherscan

**Enterprise**

- [TIME magazine to hold ETH](https://time.com/6121132/time-and-galaxy-digital-partner-to-demystify-the-next-immersive-digital-frontier-the-metaverse-through-a-first-of-its-kind-partnership/) on balance sheet
- [Sotheby’s live auction denominated in Ether](https://twitter.com/sothebys/status/1461492388078268420) for two Banksy paintings
- [Adidas](https://twitter.com/adidasoriginals/status/1461057188529594375) issued POAP via their mobile app
- Yuga Labs (creators of Bored Apes) [trademark application for APE](https://uspto.report/TM/97106855) with US Patent & Trademark Office

**Application layer**

- [Aave Arc](https://aave.mirror.xyz/JcA9DzQHK6o8YYMmxtH43Vqq5HoHvjrTrFnd_UprKWQ): permissioned Aave market with Fireblocks providing KYC/AML and onboarding to institutions
- [Cream Finance](https://creamdotfinance.medium.com/moving-forward-post-exploit-next-steps-for-c-r-e-a-m-finance-1ad05e2066d5) exploit recovery, allocating tokens from the treasury to impacted, uninsured users
- [Paraswap governance token](https://medium.com/paraswap/whats-an-active-user-clarifying-psp-token-distribution-filtering-logic-81df6096d410), ~20k users eligible to claim out of more than 1 million addresses
- [Saddle governance token](https://blog.saddle.finance/introducing-sdl/), initially non-transferrable, after 3 months DAO can make transferrable or after 12 months anyone can
- [AugurDAO](https://augur.net/blog/augurdao/): plan for transition to DAO using a DXdao Guild
- [ConstitutionDAO](https://www.constitutiondao.com/): attempt to buy print of US constitution, outbid at auction by Ken Griffin for $41 million (plus fees & taxes), contributors can claim a pro rata refund and a [POAP](https://poap.delivery/constitution-dao-contributor) \[Disclosure: I contributed\]

* * *

### **Job Listings**

- ethereum.org team is hiring a [Product Designer](https://ethereum.org/en/about/product-designer/)
- [Open Source Developer](https://openzeppelin.com/jobs/opening/?gh_jid=4554917003) at OpenZeppelin
- Ethereum Foundation hiring a [Research Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=48&source=weekinethnews) for PoS consensus layer

**Reach people experienced with Ethereum.**  $420 for two issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Ethereum Foundation grants](https://blog.ethereum.org/2021/11/16/advocacy-grants/) to Coin Center, Electronic Frontier Foundation, Fight for the Future and upcoming Gitcoin advocacy round
- [Fei and Rari](https://twitter.com/jai_bhavnani/status/1460693384549388292) token merger proposal
- Analysis of [COMP liquidity miners participation in governance](https://mirror.xyz/0x7B542178633f16940a131F8F6d670ffdbBe6b2Ab/HoTLzeiTUBn7c-uZoVcZ6PO9AlGrVQI_4WYDSeJFTiA), 7% hold 50% or more of the COMP they claimed, only 1 in top 100 ever voted

**General**

- [Crypto.com buys 20 year naming rights](https://blog.crypto.com/aeg-crypto-com-announce-new-naming-rights-agreement-to-los-angeles-venue-formerly-known-as-staples-center/) for Staples Center in LA
- [npm vulnerability](https://github.blog/2021-11-15-githubs-commitment-to-npm-ecosystem-security/), attacker could publish a new version of any package
- [Amazon UK](https://www.theverge.com/2021/11/17/22786966/amazon-visa-credit-card-ban-alternatives-fees) in 2022 will no longer accept payments from UK issued Visa credit cards due to interchange fee of 1.5%
- Jameson Lopp: Four year journey [tracking down a swatter](https://blog.lopp.net/to-swat-a-swatter/)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-november-20-2021](https://weekinethereumnews.com/week-in-ethereum-news-november-20-2021)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Oct 25 - Dec 13 – [Gitcoin DAO Global hackathon](https://gitcoin.co/hackathon/dao-global/onboard) (virtual)
- Dec 1-16 – [Gitcoin Grants Round 12](https://twitter.com/gitcoin/status/1454244939169214472)
- **Dec 3 – PoW switch off [second community call](https://github.com/ethereum/pm/issues/419)**
- Dec ~8 – [Arrow Glacier](https://blog.ethereum.org/2021/11/10/arrow-glacier-announcement/) upgrade block 13,773,000
- Jan 24-26 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford University)
- Feb 11-20 – [ETHDenver](https://www.ethdenver.com/)
- Mar 28-30 – [ETHDubai](https://www.ethdubai.xyz/)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

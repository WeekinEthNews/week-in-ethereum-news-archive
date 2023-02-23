---
title: "Week in Ethereum News <br> January 22, 2022"
date: "2022-01-22"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest core devs [call video](https://www.youtube.com/watch?v=VffwWtklJvA&t=463s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1484607389164728321):
    - Engine API spec to make executing a payload optional & auth proposal
    - Testnets post PoW switch off likely to be Goerli & Sepolia
    - Discussion of potential EIPs for Shanghai upgrade: EIP2537 BLS precompile, EIP3540 EVM Object Format, EIP3670 EOF code validation and EIP3860 limit & meter initcode
- Erigon [v2022.01.02](https://github.com/ledgerwatch/erigon/releases/tag/v2022.01.02): simplified miner gas limit, trace\_filter intersection mode and bug fixes
- Besu [v21.10.9](https://github.com/hyperledger/besu/releases/tag/21.10.9): bug fixes
- [Empirical analysis of EIP1559](https://arxiv.org/abs/2201.05574): fee estimation is now easier, decreased gas price volatility between blocks, reduced user wait time and MEV larger share of miner revenue due to burn
- Flashbots research: [parallel EVM](https://writings.flashbots.net/research/speeding-up-evm-part-1/), execute transactions with no storage conflicts at the same time and pre-load storage using optional access lists 

**Proof of Stake consensus layer**

- Lighthouse [v2.1.0](https://github.com/sigp/lighthouse/releases/tag/v2.1.0): performance improvements, 5-10x smaller slasher db, improved peer count stability and bug fixes
- Vitalik’s [secret non-single leader election](https://ethresear.ch/t/secret-non-single-leader-election/11789) proposal to avoid DoS attacks on proposer, use randao reveal hash to select, lowest hash wins for conflicts
- proto-EIP: [beacon state root in EVM](https://notes.ethereum.org/@ralexstokes/rke0rQL6F) to support validator withdrawals
- [Insecura](https://notes.status.im/nimbus-insecura-network): long range attack versus weak subjectivity testing

**PoW switch off**

- [Goerli testnet](https://twitter.com/vdwijden/status/1484255125170532358) shadow forked in PoW switch off test

**EIPs/Standards**

- [EIP4675](https://github.com/ethereum/EIPs/blob/72252fec2f091255fe877ecee0927f03d985d017/EIPS/eip-4675.md): Multi-Fractional Non-Fungible Token Standard

**Layer2**

- Connext [Vector v0.1.0](https://medium.com/connext/vector-0-1-0-mainnet-release-9496ae52c422) live, transfer value between Layer 2s using state channels
- [Warp](https://medium.com/nethermind-eth/helm-warp-one-engage-8526233780c4) (Solidity to Cairo transpiler): first major release, write tests in Solidity
- StarkNet Prover code [license discussion](https://community.starknet.io/t/starknet-prover-code-license/371)

* * *

### **This newsletter is made possible thanks to [Kwenta](https://kwenta.io/) by [Synthetix](https://synthetix.io/)!**

![Kwenta](https://weekinethereumnews.com/wp-content/uploads/2021/04/IMG_20210418_190328_618-1024x512.jpg)

[Kwenta](https://kwenta.io/) enables traders to access real-world and derivative assets on-chain using the power of the Synthetix protocol. 

Long or short popular synthetic cryptocurrencies, commodities, forex, and equities without the limits or compromises of a centralized exchange. 

You can now also use [L2 Kwenta on Optimism](https://blog.kwenta.io/everything-you-need-to-know-about-using-kwenta-on-l2/) for low gas fees and blazing fast transactions!

Decentralized Perpetual Futures coming soon.

* * *

**Stuff for developers**

- [Forge](https://w.mirror.xyz/mOUlpgkWA178HNUW7xR20TdbGRV6dMid7uChqxf9Z58) (Foundry testing framework) starter guide \[another one\]
- [Forge replit](https://replit.com/@wilsonc/VanillaForge), run Forge in the browser, vanilla setup
- Ganache [v7](https://trufflesuite.com/blog/introducing-ganache-7/): local blockchain (formerly ganache-cli), 30x faster forking, zero-config mainnet forking
- Hardhat-Vyper [v3.0.0](https://github.com/nomiclabs/hardhat/releases/tag/%40nomiclabs%2Fhardhat-vyper%403.0.0): compilation cache fixed, removed Docker dependency and supports compiling with multiple Vyper versions
- MetaMask [Flask](https://metamask.io/flask/): developer distribution for experimental features, first feature is Snaps to build and plugin APIs
- [ENS Offchain Resolver](https://discuss.ens.domains/t/offchain-resolution-for-ens-is-now-ready-for-devs/9840): starter-kit to resolve names using external services, ready for dev testing, first step for Layer 2/off-chain resolution
- Solidity [functions cheaper with payable modifier](https://twitter.com/mudit__gupta/status/1482643410834300931), non-payable functions add 24 gas check that msg.value is zero
- [evm-codes](https://www.evm.codes/playground): share code links from playground
- [VestedERC20](https://github.com/ZeframLou/vested-erc20): ERC20 wrapped as ERC20 that vests linearly
- [TWAM](https://github.com/abigger87/twam): time weighted minting prices for ERC721
- [MoonCats](https://mooncatcommunity.medium.com/on-chain-generative-art-dd9cfc3e5fb4) deep dive into on-chain generative art NFTs using traits
- [ERC721 with on-mint generation](https://github.com/fiveoutofnine/on-mint-generation) from 7 traits using probabilities
- [Playpen](https://github.com/ZeframLou/playpen): gas optimized staking pool contracts, supports ERC20 & ERC721
- [Web3UIKit](https://github.com/web3ui/web3uikit): lightweight UI components
- [Dune Analytics resources](https://twitter.com/duneanalytics/status/1483071440903680002) to get started
- [Rinkeby social faucet](https://www.rinkeby.io/#faucet) is back! Alchemy’s [Rinkeby faucet](https://www.rinkebyfaucet.com/) requires no auth

**Security**

- Multichain [bridge vulnerability](https://twitter.com/MultichainOrg/status/1483733455296860160), 600 ETH exploited, revoke approvals
- Float Protocol [~$1 million exploit](https://twitter.com/euler_mab/status/1482154663021629440), Uniswap V3 price oracle manipulated
- Redacted [token vulnerability](https://twitter.com/redactedcartel/status/1482497468713611266?s=20), ~$3 million was at risk, funds rescued
- Notional Finance [post mortem](https://medium.com/certora/post-mortem-analysis-of-the-notional-finance-vulnerability-a-tautological-invariant-574d02d6ac15), verification missed vulnerability due to logic error
- Austin Williams: [MasterChefV2](https://mirror.xyz/onewayfunction.eth/J6mp8FmcEPBj3Q4e64GA48zmiqYoB9BobMNFgXdPJXQ) principal freezing and ransom attacks
- Secureum contract auditing [next bootcamp](https://twitter.com/0xrajeev/status/1482743702485614596)

**Ecosystem**

- Josh Stark & Evan Van Ness: [Year in Ethereum 2021](https://stark.mirror.xyz/q3OnsK7mvfGtTQ72nfoxLyEV5lfYOqUfJIoKBx7BG1I)
- Ethereum.org: [20 million visits](https://twitter.com/samonchain/status/1482812310871703553) last year, [Q1 roadmap](https://github.com/ethereum/ethereum-org-website/issues/5105) includes rebrand from ETH2
- ETHGlobal: NFT Hack [recap and finalists](https://ethglobal.medium.com/nfthack-2022-302d2eb468ad)

**Enterprise**

- [Twitter](https://twitter.com/twitterblue/status/1484226494708662273?) adds hexagon NFT profile pics on iOS, requires paid Twitter Blue subscription (US, Canada, Australia & New Zealand), SVG not yet supported
- [Bud Light](https://twitter.com/budlight/status/1483906310647300097) changes Twitter profile pic to Noun NFT in deal to [feature Noun glasses in a Super Bowl commercial](https://nouns.wtf/vote/33)
- [Adidas & Prada](https://www.adidas.com/prada-nft) collaboration with Zach Lieberman on 3000 tile canvas NFT
- [Gucci & SUPERPLASTIC](https://vault.gucci.com/en-GB/story/supergucci) collaboration selling NFTs with ceramic sculptures
- [StockXVault](https://stockx.com/lp/nfts): custodial NFTs of physical products stored at a StockX facility

**Application layer**

- [Curve](https://optimism.curve.fi/) and [Instadapp](https://optimism.instadapp.io/) live on Optimism
- [UMA](https://medium.com/uma-project/uma-launches-hats-finance-vault-with-protected-tokens-2ad4587fcdf) protected tokens, shield underlying token from theft or loss
- [ShapeShift v2](https://medium.com/@ShapeShift.com/shapeshift-dao-launches-an-open-source-v2-platform-2496060b92b7): DeFi gateway
- [Argent zkSync wallet](https://www.argent.xyz/blog/how-to-earn-interest-with-aave-on-layer-2/) adds Aave via pooling
- [Themis](https://blog.themis.exchange/themis-is-live-on-mainnet-heres-what-our-dapp-can-do-6b8b6dfc3378) live on mainnet, borrow and lend against Uniswap v3 LPs
- Radicle [Drips](https://radicle.mirror.xyz/lvf9pxjG4OYZBVzLk5sVkKpfiAONFO69B131y91YOgg): stream funds to an address, split funds, sell memberships & subscriptions, collect from multiple streams with a single transaction
- [Snapshot X](https://mirror.xyz/shot.eth/cUOrwdtEs5PvNh0sqYWWxPjt8GdJWn_Qp3cl7E3_8IU): governance voting on StarkNet & execute transactions on mainnet, work in progress, permissioned from Q2, open access from Q3
- [OpenGSN](https://twitter.com/opengsn/status/1483446098308251650) meta-transactions live on Optimism
- [Lit Protocol](https://blog.litprotocol.com/?p=introducing-lit-protocol): access control for content, airdrops & interactive NFTs
- [Coinbase NFT](https://blog.coinbase.com/coinbase-and-mastercard-partner-to-revolutionize-nft-purchase-experience-8e486a392c55) working with MasterCard to allow credit card purchases
- [gem](https://mirror.xyz/0x4247c65610972d04Ca221bcc64Ff35F50c26E0F6/DYpDOHRrp_ArxADmLX6ADJCtJa5mH8y4C0tzvSQy0kI): NFT marketplace aggregator 
- NFTX [Inventory Staking](https://blog.nftx.io/introducing-nftx-inventory-staking/): staked floor NFTs receive share of vault fees
- [CryptoStats](https://medium.com/crypto-stats/announcing-cryptostats-community-owned-data-metrics-ee47fee3c94d) data metrics, use community created datasets or publish an adaptor

* * *

### **Job Listings**

- Ether Capital is hiring a 👩🏼‍💻 [DevOps Engineer](https://bit.ly/ethcapdevops) 👨🏻‍💻 to stake millions on Eth2
- Kwenta seeks [Frontend Engineer](https://blog.kwenta.io/kwenta-open-position-front-end-developer/), [Solidity Engineer](https://blog.kwenta.io/kwenta-open-position-solidity-engineer/) & [Marketing Lead](https://blog.kwenta.io/kwenta-open-position-marketing-manager/)
- Nethermind 1-3 month [internship program](https://nethermind.notion.site/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)
- Are you a p2p networking whiz? EF research hiring [Networking Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=54&source=weekinethnews)
- Geth team seeks [Senior Technical Writer](https://ethereum.bamboohr.com/jobs/view.php?id=51&source=weekinethnews) to redo the docs & take ownership
- Certora seeks [SR SW Eng](https://www.certora.com/#careers), [Security Res](https://www.certora.com/#careers), [Security Eng](https://www.certora.com/#careers) & [Community Manager](https://www.certora.com/#careers)

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US Fed [CBDC discussion paper](https://www.federalreserve.gov/publications/files/money-and-payments-20220120.pdf) \[PDF\], proposes privacy-protected, intermediated, widely transferable & identity-verified CBDC
- [Bank of Russia](https://www.coindesk.com/policy/2022/01/20/bank-of-russia-calls-for-full-ban-on-crypto/) consultation paper proposes ban on mining & use of crypto
- [Spanish regulator](https://decrypt.co/90545/crypto-influencers-face-300k-fines-spains-advertising-crackdown) to require 10 days notice of crypto ad campaigns
- [UK government](https://www.gov.uk/government/consultations/cryptoasset-promotions) plans for financial promotion regulations to cover crypto
- [Dharma](https://dharma.mirror.xyz/AiAKDL49ChgZmx-D-o_YmP-9zVDl2nqsD4uOwTcXBnI) acquired by OpenSea, Dharma wallet being sunset over 30 days
- [ETH inflation rate](https://twitter.com/biancoresearch/status/1482868840971350020) below that of BTC

**General**

- [Wallets that load centralized NFT metadata directly](https://medium.com/@alxlpsc/critical-privacy-vulnerability-getting-exposed-by-metamask-693c63c2ce94) can be used to identify an IP address from an Ethereum address
- [Hyperstructures](https://jacob.energy/hyperstructures.html): concept of protocols that are unstoppable, free, valuable, expansive, permissionless, positive sum and credibly neutral
- Opera’s [Crypto Browser](https://blogs.opera.com/crypto/2022/01/opera-crypto-browser-project-web3/) with native wallet for Android, Windows & Mac, public beta
- [Crypto.com](https://crypto.com/product-news/crypto-com-security-report-next-steps) $34 million in unauthorized withdrawals from 483 accounts, users refunded, all users migrated to new 2FA infrastructure
- [UK government advertising campaign](https://noplacetohide.org.uk/) against end to end encryption
- [Intel deprecating SGX](https://www.bleepingcomputer.com/news/security/new-intel-chips-wont-play-blu-ray-disks-due-to-sgx-deprecation/) in desktop chips

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-january-22-2022](https://weekinethereumnews.com/week-in-ethereum-news-january-22-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Feb 15 - Apr 5 – [Cryptocurrency Class](https://mirror.xyz/0xaFaBa30769374EA0F971300dE79c62Bf94B464d5/oGqGP2NOK9g7QPl1sMKkzql_Fh0P6hKbpYLZ-EkQTXU) (virtual) 
- Feb 17 – [Schelling Point](https://schellingpoint.gitcoin.co/) (Denver) 
- Feb 18-20 – [ETHDenver](https://www.ethdenver.com/)
- Mar 14-17 – [Eth Rio](https://www.ethrio.org/)
- Mar 17-18 – [ETH Austin](https://2022.ethaustin.org/) summit
- Mar 29-31 – [ETHDubai](https://www.ethdubaiconf.org/)
- Apr 7-9 – [ETH Portland](https://2022.ethportland.com/) hackathon
- **Apr 20-21 – [The Alliance gaming summit](https://medium.com/1kxnetwork/announcing-alliance-summit-7e8732c9fd9d) (Amsterdam)**
- **Apr 21 – [ETHconomics](https://ef-events.notion.site/ETHconomics-Devconnect-676d73f791684e18bfae35bbc9e1fa90) (Amsterdam)**
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- May 3-8 – [spaghettETH](http://spaghett-eth.com/) (Milan)
- **May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline**
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 16-19 – [ETH Miami](https://2022.eth-miami.com/) summit & hackathon
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETHNewYork](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

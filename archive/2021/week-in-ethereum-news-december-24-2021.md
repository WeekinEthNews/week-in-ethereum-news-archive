---
title: "Week in Ethereum News <br> December 24, 2021"
date: "2021-12-24"
---

## **Eth News and Links**

**Mainnet execution layer**

- Tim Beiko’s [Kintsugi testnet announcement](https://blog.ethereum.org/2021/12/20/kintsugi-merge-testnet/); public testnet is running over the next month, help test PoW switch off!
- Getting started on the Kintsugi testnet [video guide](https://www.youtube.com/watch?v=r31aeGPoy1o)
- Geth [v1.10.14](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.14): PoW switch off prototype, Kintsugi testnet spec v3 compatible
- Besu [v21.10.5](https://github.com/hyperledger/besu/releases/tag/21.10.5): update log4j 
- [Gas market analysis of EIP1559](https://pintail.xyz/posts/gas-market-analysis/) with visualizations: users less likely to overpay for transactions
- [ERC4337 account abstraction](https://medium.com/nethermind-eth/erc-4337-account-abstraction-is-already-here-e9588b789e15) proposed implementation live on Goerli testnet using Nethermind

**Proof of Stake consensus layer**

- [Bellatrix](https://github.com/ethereum/consensus-specs/pull/2774) chosen as the name for consensus layer upgrade to switch off PoW
- Consensus specs [v1.1.7](https://github.com/ethereum/consensus-specs/releases/tag/v1.1.7): light-client sync simplification, fork choice rule fixes and new test vectors

**Layer2**

- [Transak](https://twitter.com/transak_finance/status/1473367208474681351) fiat on-ramp to Arbitrum and Optimism (not currently in US)
- [Banxa](https://twitter.com/BanxaOfficial/status/1473887349251604483) fiat on-ramp to Arbitrum
- [DeversiFi](https://deversifi.com/blog/announcing-our-brand-new-integration-with-moonpay/) fiat on-ramp via MoonPay
- [Loopring](https://medium.loopring.io/introducing-l2-counterfactual-wallet-and-fiat-on-ramps-a4b60edf15d6) Layer 2 starter wallet on iOS, pay later to deploy to Layer 1 for mainnet withdrawal and more features, fiat on-ramp via Ramp
- [Across Protocol](https://medium.com/across-protocol/the-fastest-cheapest-and-most-secure-bridge-now-supports-l1-l2-transfers-92d7b2bd6666): bridge now two way, adds mainnet to Arbitrum, Optimism and Boba
- [StarkWare Layer 3 scaling](https://medium.com/starkware/fractal-scaling-from-l2-to-l3-7fe238ecfb4f): application specific layer using recursive proofs, StarkEx Layer 2’s can be ported to Layer 3

* * *

### **This newsletter is made possible thanks to [Kwenta](https://kwenta.io/) by [Synthetix](https://synthetix.io/)!**

![Kwenta](https://weekinethereumnews.com/wp-content/uploads/2021/04/IMG_20210418_190328_618-1024x512.jpg)

[Kwenta](https://kwenta.io/) enables traders to access real-world and derivative assets on-chain using the power of the Synthetix protocol. 

Long or short popular synthetic cryptocurrencies, commodities, forex, and equities without the limits or compromises of a centralized exchange. 

You can now also use [L2 Kwenta on Optimism](https://blog.kwenta.io/everything-you-need-to-know-about-using-kwenta-on-l2/) for low gas fees and blazing fast transactions!

Decentralized Perpetual Futures coming soon.

* * *

**Stuff for developers**

- Solidity [v0.8.11](https://blog.soliditylang.org/2021/12/20/solidity-0.8.11-release-announcement/): Solidity Language Server minimal feature set, native binary only, no autocomplete yet, hook up to favorite IDE and feedback; abi.encodeCall added to check supplied values match expected types
- [Etherscan adds initial Natspec support](https://twitter.com/etherscan/status/1472191164807712768): view notice, parameter & return descriptions in read & write contract tabs
- [WalletConnect v2](https://medium.com/walletconnect/swift-and-kotlin-sdks-are-now-in-beta-436c72eb834f) beta Swift & Kotlin SDKs
- [hardhat-deploy-tenderly](https://github.com/wighawag/hardhat-deploy-tenderly): push deployed contract to Tenderly for debugging
- [Yul-Log](https://github.com/ControlCplusControlV/Yul-Log): write & use Yul+ contracts, supports Truffle, Hardhat in progress
- [sipping-oe (scaffold-eth)](https://github.com/scaffold-eth/scaffold-eth/tree/sipping-oe): starter kit to deploy on-chain SVG NFTs to Optimism \[Disclosure: I was gifted an OΞ40\]
- [ethereum-code-viewer](https://twitter.com/dethcrypto/status/1473001241970159621): adds support for Arbitrum, Optimism and testnets
- [ens2airdrop](https://github.com/iainnash/ens2airdrop): collect addresses from “drop your ENS” Twitter threads
- [Helios](https://github.com/z0r0z/Helios): work in progress ERC1155 based exchange
- [Cairo-jupyter](https://github.com/ankitchiplunkar/cairo-jupyter): Jupyter kernel for Cairo 
- Guide to building an [MEV inspector](https://writings.flashbots.net/writings/the-anatomy-of-an-inspector/) using example CryptoPunk inspector
- [Notion](https://twitter.com/mark_mkzo/status/1472162594077220864) supports Solidity code blocks

**Security**

- Bent Finance ~$1.75 million [exploit](https://bentfi.medium.com/bent-update-12ae69a41dc6), reported rogue developer upgraded contract with hardcoded balances for exploiter account
- Visor Finance 8.8 million VISR [exploit](https://rekt.news/visor-finance-rekt/), staking contract drained, attack contract set owner to be itself 
- Sorbet Finance [vulnerability post mortem](https://medium.com/gelato-network/sorbet-finance-vulnerability-post-mortem-6f8fba78f109), contract could make arbitrary low level calls, $27 million in user funds rescued to escrow, $744k stolen
- Adidas token drop capped to 2 NFTs per address, [custom contract purchased 330 NFTs](https://twitter.com/montana_wong/status/1472023753865396227), 165 subcontracts claimed 2 NFTs each

**Ecosystem**

- Ethereum Foundation teams [Q4 achievements](https://blog.ethereum.org/2021/12/22/ef-supported-teams-research-and-development-update-2021-pt-3/)
- Polygon zk day [recap and videos](https://ethglobal.medium.com/polygon-zk-day-2021-ee257349a4ca)
- [ethOS](https://twitter.com/EthereumPhone/status/1472683474536517635): building mobile OS based on Android fork (LineageOS), running a light client
- [30 days of web3](https://twitter.com/wslyvh/status/1472955969151848456): ship something new (code or no code), first cohort January 2022

**Enterprise**

- [Coca-Cola](https://medium.com/veve-collectibles/coca-cola-snow-globes-ddc7444b6789) snow globe NFTs on VeVe (Immutable X)
- [RadioShack DeFi](https://radioshack.gitbook.io/radioshack-defi/fundamentals/why-radioshack-defi): historic brand reused for DeFi project
- [SAP](https://www.oasis-open.org/2021/12/22/eea-community-projects-governing-body-of-the-baseline-protocol-welcomes-sap-as-sponsor/#baselineprotocol) joins as a sponsor of Enterprise Ethereum Alliance community projects in support of Baseline

**Application layer**

- [Quixotic](https://beta.quixotic.io/): NFT marketplace for Optimism, beta
- [Eth.xyz](https://gen.xyz/blog/ethxyz?utm_source=twitter&utm_medium=post&utm_campaign=2021-12-ethxyz): add “.xyz” to ENS name for URL shareable ENS profile
- [Shaq](https://twitter.com/shaq) changes Twitter handle to ENS & launches 10k NFT collection for his foundation
- [Rarible](https://twitter.com/rarible/status/1473688588789424132?s=20): gift NFTs using Linkdrop, sponsor the transaction for recipients to claim for free
- [Collab.Land](https://twitter.com/collab_land_/status/1474045984783015939) supports Arbitrum
- [Argent](https://www.argent.xyz/blog/gift-crypto/): gift ETH/USDC on zk-sync Layer 2, recipients create an Argent Layer 2 wallet to claim
- [Gnosis Safe](https://twitter.com/gnosisSafe/status/1474039980251041798) deployed to Optimism
- [Kwenta](https://blog.kwenta.io/tradingview-l2-shorting/) shorting live on Optimism
- [Thales](https://thalesmarket.medium.com/thales-l2-deployment-2021-in-review-and-next-steps-975d2374d676) positional markets live on Optimism, with beta AMM
- [dHEDGE](https://app.dhedge.org/competition): 30 day trading competition on Optimism
- [Slingshot](https://twitter.com/slingshotcrypto/status/1474107388760371216) trading live on Optimism
- [Gearbox](https://medium.com/gearbox-protocol/hello-world-source-code-is-open-bug-bounty-and-audits-1673f279b822) composable leverage live on mainnet
- [ZKyber](https://blog.kyber.network/zkyber-a-new-dex-trading-experience-based-on-zk-rollups-6666d52c24cf): Kyber’s zk-rollup and DEX on testnet
- [microETH](https://microeth.io/): 0.000001 ETH wrapped in ERC20, for unit bias

* * *

### **Job Listings**

- The VAC team at Status.im are looking for a [blockchain engineer](https://jobs.status.im/?gh_jid=3712494)
- Geth team is looking for a [Senior Technical Writer](https://ethereum.bamboohr.com/jobs/view.php?id=51&source=weekinethnews)
- Kwenta seeks [Frontend Engineer](https://blog.kwenta.io/kwenta-open-position-front-end-developer/), [Solidity Engineer](https://blog.kwenta.io/kwenta-open-position-solidity-engineer/) & [Marketing Lead](https://blog.kwenta.io/kwenta-open-position-marketing-manager/)
- Ethereum Foundation consensus research team seek [Networking Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=54&source=weekinethnews)
- [Textile](https://textile.io/) is hiring! [Blockchain Eng](https://grnh.se/f093ec154us), [Backend Eng](https://grnh.se/526aef8d4us), and [Partner Manager](https://grnh.se/06c1dfdf4us)
- IoBuilders is hiring: [Enterprise blockchain devs](https://www.linkedin.com/jobs/view/2753213671), [product managers](https://www.linkedin.com/jobs/view/2753213143) & [more](https://www.linkedin.com/company/iobuilders)
- EFF hiring a [Senior Fellow of Decentralization](https://www.eff.org/deeplinks/2021/12/dream-job-alert-senior-fellow-decentralization-eff)
- Bloom Institute of Technology (fka Lambda school) seek [Solidity experts](https://jobs.lever.co/BloomTech/c3ff6acf-c8ad-4957-b1a9-23a5f693598f)

**Reach developers experienced with Ethereum.  $444** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Former US SEC Chair Clayton: [“end-to-end tokenization” of all assets is a “once-in-a-generation opportunity”](https://www.wsj.com/articles/america-future-depends-on-blockchain-crypto-bitcoin-payments-transfers-federal-reserve-11639668586) \[Paywall\]
- [US regulator confirms credit unions](https://www.ncua.gov/regulation-supervision/letters-credit-unions-other-guidance/relationships-third-parties-provide-services-related-digital-assets) can partner with providers to offer crypto services to their members
- [Compound](https://thedefiant.io/compound-dao-open-bidding-security/) governance chose OpenZeppelin’s $1 million a quarter proposal to provide audit and security services, out of three competing proposals 
- Bitwise launch [NFT index fund](https://www.businesswire.com/news/home/20211216005484/en/Bitwise-Launches-Blue-Chip-NFT-Index-Fund-Offering-Broad-Exposure-to-the-Most-Iconic-Digital-Art-Collections), focused on art and collectibles
- [Phonon](https://blog.phonon.network/phonon-dao-launch-overview-resources-and-phonon-token-details-f8369e89f1ea) P2P off-chain transfer protocol being spun off from Grid+, managed by governance token \[Evan is a DAO steward\]
- [Fei & Rari merger](https://www.coindesk.com/tech/2021/12/21/rari-capital-fei-protocol-token-holders-approve-multibillion-dollar-defi-merger/) approved
- Proposal for [updated YFI tokenomics](https://gov.yearn.finance/t/proposal-evolving-yfi-tokenomics/11994): token buy back & reward stakers, vote escrow model, Vault Gauges and rewards for contributing
- [SEBA (Swiss bank)](https://governance.aave.com/t/arc-adding-seba-bank-as-a-whitelister-to-aave-arc/6661) proposal to provide KYC/AML and onboarding to Aave Arc (permissioned Aave market)
- [Web3 renaissance: golden age of content](https://every.mirror.xyz/y_WLA-Tk3VF5uPqHi-glDLVVfHxLUbjXakRI7SMISas), NFTs & scarcity, patronage+, programmable economic models and DAOs & community ownership
- [ETH flips BTC](https://twitter.com/ercwl/status/1473301895104151555) in stock to flow metric 

**General**

- New York Times: Staff from Google, Meta, Amazon and other large companies are [quitting for crypto’s once in a generation opportunity](https://www.nytimes.com/2021/12/20/technology/silicon-valley-cryptocurrency-start-ups.html)
- Vitalik: [bulldozer vs vetocracy political axis](https://vitalik.eth.limo/general/2021/12/19/bullveto.html)
- [Binance’s threshold signature scheme library](https://blog.trailofbits.com/2021/12/21/disclosing-shamirs-secret-sharing-vulnerabilities-and-announcing-zkdocs/) (tss-lib) and forks vulnerability in Shamir’s Secret Sharing implementation
- [ZKDocs](https://www.zkdocs.com/): documentation on zero-knowledge proof systems

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-24-2021](https://weekinethereumnews.com/week-in-ethereum-news-december-24-2021)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Jan 22-23 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Jan 24-26 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford University)
- Feb 17 – [Schelling Point](https://schellingpoint.gitcoin.co/) (Denver) 
- Feb 18-20 – [ETHDenver](https://www.ethdenver.com/)
- Mar 14-17 – [Eth Rio](https://www.ethrio.org/)
- Mar 29-31 – [ETHDubai](https://www.ethdubai.xyz/)
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- **May 3-8 – [spaghettETH](http://spaghett-eth.com/) (Milan)**
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 24-26  – [ETHNewYork](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4) 
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

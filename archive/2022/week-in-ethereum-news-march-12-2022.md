---
title: "Week in Ethereum News <br> March 12, 2022"
date: "2022-03-12"
---

## **Eth News and Links**

**Mainnet execution layer**

- Execution Layer PoW switch off named [Paris](https://twitter.com/timbeiko/status/1502295917206163476), site of first major community organized conference
- Nethermind's [full pruning](https://medium.com/nethermind-eth/netherminds-full-pruning-is-here-cutting-the-gordian-knot-5e3450f02de9), run a pruned node with ~100Gb of storage
- Verkle tree single client [testnet demo video](https://twitter.com/gballet/status/1502321952551280647)

**Proof of Stake consensus layer**

- PoS implementers call [video](https://www.youtube.com/watch?v=SEVY6-Zr2OM&t=396s) \[first 15 mins\]. Notes from [Ben Edgington](https://hackmd.io/@benjaminion/SkYImKP-9)
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220311)
- Kelvin open sources unedited [Eth2 Book](https://eth2.incessant.ink/book/00__introduction/00__forward.html)
- Nimbus [v22.3.0](https://github.com/status-im/nimbus-eth2/releases/tag/v22.3.0): run as a Windows service, config file for command line options and lower CPU, bandwidth & memory usage
- Lodestar [v0.34.1](https://github.com/ChainSafe/lodestar/releases/tag/v0.34.1): make block proposing flow resilient to errors
- Lighthouse [task list](https://lighthouse.sigmaprime.io/update-40.html) before PoW can be switched off
- Prysm [quality approach](https://twitter.com/preston_vanloon/status/1502079385293180939): static analysis checks, unit & fuzz tests, common spec tests and code review; recommends trying a minority client for Kiln
- Wagyu Key Gen [v1.2.0](https://github.com/stake-house/wagyu-key-gen/releases/tag/v1.2.0): supports generating keys for Kiln & Kintsugi testnets
- Paper on [PoS fork choice attacks](https://arxiv.org/abs/2203.01315) results in [spec patch](https://github.com/ethereum/consensus-specs/pull/2845) for an edge case in an equivocation balancing attack; protocol not vulnerable to avalanche attack

**PoW switch off**

- [Kiln testnet](https://kiln.themerge.dev/) launched, transitions to PoS next week.
    - [Help test PoW switch off](https://twitter.com/vdwijden/status/1501853162688421888), the biggest change in Ethereum’s history
    - Get Kiln Ether, deploy contracts and send transactions  
    - The amount of testing impacts when PoW switch off is ready
    - Guide to run [Geth+Teku](https://github.com/chrishobcroft/TestingTheMerge/blob/main/geku.md), [Geth+Lighthouse](https://github.com/remyroy/ethstaker/blob/main/merge-devnet.md), [Geth/Nethermind+Lodestar](https://hackmd.io/@philknows/By5qahdZc) or [Geth+Prysm](https://hackmd.io/@prysmaticlabs/B1Q2SluWq)
- Kiln [v2.1](https://hackmd.io/@n0ble/kiln-spec#v21-change-set) spec: optimistically import any post-merge block, add QoS for transition config endpoint and clarifications of Engine API spec
- Validator withdrawals [meta-spec](https://notes.ethereum.org/@ralexstokes/Skp1mPSb9) proposal using a push architecture
- [merge-devnet-5](https://twitter.com/parithosh_j/status/1500883006571139072) transitioned & switched off PoW, no issues found testing with zombie miners

**EIPs/Standards**

- [EIP4881](https://eips.ethereum.org/EIPS/eip-4881): Deposit Contract Snapshot Interface
- [EIP4885](https://github.com/ethereum/EIPs/blob/275d05e049790836e2df4167c0abb60c4992a550/EIPS/eip-4885.md): Subscription Token Standard for NFTs and Multi Tokens
- [EIP4886](https://github.com/ethereum/EIPs/blob/772b9bbe54b1c6e4db6faa3434af9a2e04e8951c/EIPS/eip-4886.md): Proxy Ownership Register
- [EIP4895](https://eips.ethereum.org/EIPS/eip-4895): Beacon chain push withdrawals as operations 

**Layer2**

- Arbitrum [gas pricing change](https://research.arbitrum.io/t/l2-compute-gas-pricing/22) adds momentum and targets 80% full so gas price changes faster but more gently
- [DefersiFi](https://twitter.com/deversifi/status/1500853979479261185) adds bridge to Arbitrum
- Argent [zkSync mobile wallet](https://twitter.com/argentHQ/status/1500879350677262336) out of beta
- Argent X (StarkNet) [v3](https://github.com/argentlabs/argent-x/releases/tag/v3.0.0): migrate assets such as [briqs](https://twitter.com/briqNFT/status/1502329495528873994) from v2
- StarkNet’s proposed [account abstraction](https://community.starknet.io/t/starknet-account-abstraction-model-part-1/781) design
- Optimism’s proposed [Cannon fault proof](https://medium.com/ethereum-optimism/cannon-cannon-cannon-introducing-cannon-4ce0d9245a03); Norswap’s Cannon [explainer](https://twitter.com/norswap/status/1502085000967061504)
- Optimism [multi-client plan](https://medium.com/ethereum-optimism/our-pragmatic-path-to-decentralization-cb5805ca43c1) to decentralize & remove upgrade keys
- Vitalik’s [explainer of the tradeoffs](https://www.reddit.com/r/ethereum/comments/t7adbt/hows_eip4844_differ_from_eip4488_where_both/hzi63ig) between EIP 4488 (simple calldata gas reduction) and EIP4844 (new data blob transaction type) to drastically lower transaction costs for rollups

* * *

### **This newsletter is made possible thanks to Starbloom Ventures!**

![Starbloom Ventures](https://weekinethereumnews.com/wp-content/uploads/2021/11/Screenshot-from-2021-11-19-15-25-51.png)

Starbloom Ventures is an early-stage venture fund founded by [Evan Van Ness](https://twitter.com/evan_van_ness) to invest in the future of web3. 

Our first [publicly announced investment is Karma](https://twitter.com/evan_van_ness/status/1496909181584084993), which is building an on-chain reputation system for web3 participants.  Check out the reputation leaderboards for [ENS](https://www.showkarma.xyz/dao/delegates/ens) and [Gitcoin](https://www.showkarma.xyz/dao/delegates/gitcoin) delegates. 

* * *

**Stuff for developers**

- [Hardhat for VS Code](https://twitter.com/HardhatHQ/status/1501981504964079621) extension: Solidity code completion, code navigation, formatting and quick fix suggestions; public beta
- ethers.js [update](https://blog.ricmoo.com/highlights-ethers-js-march-2022-f511fe1e88a1) & [v5.6.0](https://github.com/ethers-io/ethers.js/releases/tag/v5.6.0): adds CCIP Read for ENS resolvers, ENS wildcard and Cloudflare Worker support
- WalletConnect [v1.7.4](https://github.com/WalletConnect/walletconnect-monorepo/releases/tag/1.7.4): fix event listener registration
- [Multicall3](https://github.com/mds1/multicall#readme): aggregate results of multiple constant function calls
- PRBProxy [v2.0.0](https://github.com/paulrberg/prb-proxy/releases/tag/v2.0.0) (multiple calls in one transaction): improved gas efficiency
- [Chainalysis oracle](https://go.chainalysis.com/chainalysis-oracle-docs.html) for sanctions screening in Solidity and JavaScript
- [Solwaifu](https://github.com/outdoteth/solwaifu#readme): bytecode ERC20 for minimal gas use, unaudited
- [Ethsig-rs](https://github.com/odyslam/ethsig-rs#readme): Cloudflare worker enables Sign In With Ethereum for services
- Run a [local version](https://twitter.com/kasiazerosiedem/status/1501243828388380674) of StarkNet Voyager block explorer
- [web3-starknet-react](https://github.com/dhruvkelawala/web3-starknet-react#readme): inspired by web3-react
- Damn Vulnerable DeFi (CTF) [Foundry version](https://github.com/nicolasgarcia214/damn-vulnerable-defi-foundry#readme)
- [evm-puzzles](https://twitter.com/fvictorio_nan/status/1500312282567434242): interactive version, improved bytecode display and evm.codes playground links
- [EVM golf](https://twitter.com/the_ethernaut/status/1502405820465795073) challenges by the Ethernaut
- [NFT randomness](https://medium.com/@inner.space/chaos-in-big-nft-collections-63b83aa893d8): algorithms & techniques for less predictable minting
- [Contract memory](https://noxx.substack.com/p/evm-deep-dives-the-path-to-shadowy-d6b) explainer
- [DevPill.me](https://www.devpill.me/docs/introduction/foreword/): blockchain development guide

**Security**

- Bacon Protocol $1 million reentrancy [exploit](https://mirror.xyz/baconcoin.eth/LHaPiX38mnx8eJ2RVKNXHttHfweQMKNGmEnX4KUksk0), bug was found in [patch](https://twitter.com/danielvf/status/1501926505349357576)
- The Idols Marketplace [vulnerability](https://docs.google.com/document/d/1FfeF-epgBUwZBhdwMQ_rtvVjLtQ8f09pukSmZZ-GsI8/edit), rescued ~58 ETH & NFTs that were at risk, reported by samczsun
- EF [vulnerability disclosures](https://github.com/ethereum/public-disclosures#readme) for execution & consensus layer clients
- Optimism self destruct inflation [postmortem](https://github.com/ethereum-optimism/optimism/blob/master/technical-documents/postmortems/2022-02-02-inflation-vuln.md)

**Ecosystem**

- [10 million ETH](https://twitter.com/terencechain/status/1501922526221324289) in staking deposit contract
- Wen Merge?  Superphiz [predicts June](https://www.reddit.com/r/ethstaker/comments/tbql1n/five_indicators_that_the_ethereum_merge_will/)
- [Etherscan](https://etherscan.io/accounts/label/gnosis-safe) labels Gnosis Safe contracts created by proxy factory

**Enterprise**

- [Stripe adds crypto support](https://twitter.com/collision/status/1501961880289480704): on/off ramps, KYC & identity verification, fraud prevention and carbon offsetting

**Application layer**

- [Yuga Labs (BAYC) acquires CryptoPunks & Meebits](https://mirror.xyz/0xEc9f53fA69682833FBd760C104B5D61aE29221E0/Km81y6Mc3O5LzS0wnrghVIV0HnZgLOd4wsnfcGw3_2I), plans to give NFT holders commercial rights
- [Gem](https://twitter.com/gemxyz/status/1500912481035825165) (NFT marketplace aggregator) integrates LooksRare
- [Quixotic](https://twitter.com/quixotic_io/status/1501342408163741699) (Optimism) & [Stratos](https://twitter.com/stratosnft/status/1501674412969369600) (Arbitrum) NFT Launchpad, no-code NFTs for free to mint projects
- [Andre Cronje](https://twitter.com/AntonNellCrypto/status/1500405473337565191) terminating front ends April 3; [Yearn](https://twitter.com/bantg/status/1500416805659201537) unaffected
- DefiSaver’s [automated MakerDAO vault payback to avoid liquidation](https://blog.defisaver.com/automated-strategies-next-era-automation-live/) for mStable, Rari and Yearn yield farming strategies

* * *

### **Job Listings**

- Status is hiring! [Communications Director](https://grnh.se/0a1f0ea71us) & [Creative Strategist](https://grnh.se/315600fd1us). [All jobs](https://grnh.se/9fc6e6fc1us)
- Devcon needs a [front-end web developer](https://ethereum.bamboohr.com/jobs/view.php?id=61&source=weekinethnews)
- EF’s Privacy & Scaling Explorations team seek a [ZKP Security Engineer](https://jobs.lever.co/ethereumfoundation/b80cf733-9a8d-40f1-a85a-635acdc2b1b1?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum%20), [L2 Security Engineer](https://jobs.lever.co/ethereumfoundation/f3148457-ed1e-4659-941d-5f60b49427ca?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) and a [Marketing Ops Manager](https://jobs.lever.co/ethereumfoundation/7a831e7c-1a0d-4e7b-8291-072292e26c0e?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum%20&lever-source%5B%5D=Week%20in%20Ethereum%20)
- eVerse is hiring a [lead blockchain engineer](https://everse.notion.site/Lead-Blockchain-Engineer-Architect-845acc3ef4c64784b19d4f2cede8161c) for its social video platform
- Mark Cuban seeks a [web3 front-end developer](https://forms.office.com/r/M81g5RNgXX). Send a work sample to apply.
- [Nomic Foundation](https://www.notion.so/Nomic-Foundation-jobs-991b37c547554f75b89a95f437fd5056) hiring Rust Tech Lead & Ethereum Tech Lead

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US President Biden’s [crypto executive order](https://www.whitehouse.gov/briefing-room/statements-releases/2022/03/09/fact-sheet-president-biden-to-sign-executive-order-on-ensuring-responsible-innovation-in-digital-assets/): asks Treasury to make policy recommendations, mitigate systemic & illicit use risks, promote US leadership, equitable & safe access and explore CBDC
- [US FINCEN](https://www.fincen.gov/news/news-releases/fincen-provides-financial-institutions-red-flags-potential-russian-sanctions): large scale sanctions evasion using crypto not practicable
- [UK FCA orders shutdown of crypto ATMs](https://www.fca.org.uk/news/news-stories/warning-illegal-crypto-atms-operating-uk) as none are registered
- [Ormeus Coin](https://www.sec.gov/news/press-release/2022-37) promoters charged with fraudulent securities offerings
- [EmpowerCoin, ECoinPlus & Jet-Coin](https://www.justice.gov/usao-edny/pr/owners-and-operators-online-cryptocurrency-companies-indicted-defrauding-investors) owners/operators charged with conspiracy to commit wire fraud and money laundering
- Analysis of [DEX aggregators](https://medium.com/iosg-ventures/dex-aggregators-the-future-of-on-chain-trading-59856515b408)

**General**

- [Twitter](https://twitter.com/AlecMuffett/status/1501282223009542151) available via Tor
- The Verge: [The many escapes of Justin Sun](https://www.theverge.com/c/22947663/justin-sun-tron-cryptocurrency-poloniex)
- Vitalik: [barycentric evaluation tutorial](https://hackmd.io/@vbuterin/barycentric_evaluation)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-march-12-2022](https://weekinethereumnews.com/week-in-ethereum-news-march-12-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Mar 11-20 – [Ethereum Rio](https://www.ethereum.rio/)
- **Mar 15 – deadline for [ETH University student project grants](https://fund.ethuniversity.org/)**
- Mar 15 – [Cryptocurrency Class](https://mirror.xyz/0xaFaBa30769374EA0F971300dE79c62Bf94B464d5/oGqGP2NOK9g7QPl1sMKkzql_Fh0P6hKbpYLZ-EkQTXU) starts (virtual) 
- Mar 16 – submission deadline for [Underhanded Solidity Contest](https://underhanded.soliditylang.org/)
- Mar 17-18 – [ETH Austin](https://2022.ethaustin.org/) summit
- Mar 24 – [Gitcoin Grants Round 13](https://gitcoin.co/grants/) ends (support [Week in Eth News](https://gitcoin.co/grants/2785/week-in-ethereum-news))
- Mar 29-31 – [ETHDubai](https://www.ethdubaiconf.org/)
- Apr 7-9 – [ETH Portland](https://2022.ethportland.com/) hackathon
- Apr 18-25 – [Devconnect](https://devconnect.org/schedule) (Amsterdam)
- Apr 22 – deadline for [EF academic grants round](https://esp.ethereum.foundation/academic-grants)
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETHNewYork](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

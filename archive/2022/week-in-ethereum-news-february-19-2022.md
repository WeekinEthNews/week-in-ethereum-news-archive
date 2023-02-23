---
title: "Week in Ethereum News <br> February 19, 2022"
date: "2022-02-19"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest core devs call [video](https://www.youtube.com/watch?v=Oo_Nnk3CdLA&t=391s) \[audio issue first 8 mins\]. Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1494760753726779394):
    - RANDOM opcode being renamed to PREVRANDAO
    - Kurtosis PoW switch off testing demo with a local multiclient testnet
    - Withdrawals discussion on draft EIPs & execution layer withdrawal contract
    - Proposed EIP4803 cap on gas limit in a transaction
- Geth [v1.10.16](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.16): bug fixes
- mev-geth [v1.10.15-mev0.5.0](https://github.com/flashbots/mev-geth/releases/tag/v1.10.15-mev0.5.0): calculate megabundles when received
- Erigon [v2022.02.03](https://github.com/ledgerwatch/erigon/releases/tag/v2022.02.03): Sepolia testnet support, stability fixes
- Besu [v22.1.0](https://github.com/hyperledger/besu/releases/tag/22.1.0)
- [PluGeth](https://blog.openrelay.xyz/cardinal/plugeth/): fork of Geth designed for plugins, Cardinal plugin for streaming replication system
- Otterscan [Sepolia testnet explorer](https://sepolia.otterscan.io/)
- [Sample block with a Verkle proof](https://github.com/gballet/verkle-block-sample/#readme) and utility to decode & verify

**Proof of Stake consensus layer**

- [Staking pools dashboard](https://pools.invis.cloud/): very high usage of supermajority client by exchanges, estimated usage over 90% for Coinbase & Kraken & over 75% for Binance
- Nimbus [v1.7.0](https://github.com/status-im/nimbus-eth2/releases/tag/v1.7.0): 3-5x faster startup, <1GB memory usage on mainnet, trusted node sync, Keymanager API supports remote keystores 
- Lodestar client setup [video](https://www.youtube.com/watch?v=0xo85F-_fag)
- [Vouch](https://www.attestant.io/posts/helping-client-diversity/) (multi-node validator): avoids client diversity issues by not using supermajority client for attestations
- [Beaconcha.in bug](https://hackmd.io/Bncoj0ilRfi6REyUJPWdiA) believed to be source for claims of uncaught slashings
- Nimbus [Era files](https://twitter.com/jcksie/status/1493524432719073284): early research for storing & retrieving historical data
- Danksharding workshop [video](https://www.youtube.com/watch?v=e9oudTr5BE4&t=9s) & [slides](https://docs.google.com/presentation/d/1-pe9TMF1ld185GL-5HSWMAsaZLbEqgfU1sYsHGdD0Vw/edit#slide=id.p1).  Notes from [Polynya](https://twitter.com/epolynya/status/1492913526964248576)

**PoW switch off**

- [merge-devnet-4](https://twitter.com/parithosh_j/status/1494311072345600004) (precursor to public Kiln testnet) is live, had multiple forks but transitioned to PoS without intervention

**EIPs/Standards**

- [EIP4824](https://github.com/ethereum/EIPs/blob/a757325163ce6ccf8484f744b46bb6415e37eea0/EIPS/eip-4824.md): Decentralized Autonomous Organizations
- [EIP4812](https://github.com/ethereum/EIPs/blob/0f9068accbe1e108a544bd8346383a212c993b78/EIPS/eip-4804.md): Exodus
- [EIP4803](https://github.com/ethereum/EIPs/blob/1b3af5efd7b365b273542621d896b222eac9b7db/EIPS/eip-4803.md): Limit transaction gas to a maximum of 2^63-1
- [EIP4800](https://github.com/ethereum/EIPs/blob/cf59d187fc381a5fa6d2feb347eda57519f2b5dd/EIPS/eip-4800.md): Non-Fungible Token Wrapping Standard

**Layer2**

- [OKX](https://www.okx.com/support/hc/en-us/articles/4426572059661-OKx-supports-Arbitrum-s-network) and [Bitget](https://bitget.zendesk.com/hc/en-us/articles/4419534112665) add Arbitrum support
- [Urbit](https://urbit.org/blog/layer-2-guides) naive rollup is live
- [Optimism fee explainer](https://optimismpbc.medium.com/fancy-numbers-how-we-lowered-fees-for-optimism-users-a3bb80cbc65f), how fees were lowered by 30%, fixed overhead now 2100 gas per transaction with a fee scalar of 1.24

* * *

### **This newsletter is made possible thanks to [Kwenta](https://kwenta.io/) by [Synthetix](https://synthetix.io/)!**

![Kwenta Community Raise](https://weekinethereumnews.com/wp-content/uploads/2022/02/Kwenta-Community-Raise.png)

Kwenta is a derivatives trading platform, live on Optimism, offering real-world and on-chain synthetic assets using the power of the Synthetix protocol. 

The Sovereignty Phase, an 8-week campaign marking the launch of Synthetic Perpetual Futures, Kwenta V2, and the KWENTA token, has just been kicked off and will include a community raise, trading competitions, liquidity mining rewards, and more. 

To start the Sovereignty Phase, Kwenta is hosting a community raise, providing pool contributors with early access to the token. 

The raise is live here on Aelin: [raise.kwenta.io](https://raise.kwenta.io/)

* * *

**Stuff for developers**

- Solidity [v0.8.12](https://blog.soliditylang.org/2022/02/16/solidity-0.8.12-release-announcement/): reduces size of JavaScript/Wasm binaries, solc-js partially ported to TypeScript and bug fixes
- Foundry [fuzzer](https://twitter.com/msolomon44/status/1493638347092234242): improved random uint generation, discard fuzz runs that don’t meet criteria using assume cheatcode
- [Blacksmith](https://github.com/pbshgthm/blacksmith#readme): user contract generator for Foundry, test contract interaction like an EOA user
- [Foundry Rust Monorepo Template](https://github.com/gakonst/foundry-rust-template#readme) for developing Rust applications using Foundry for contract development
- Truffle [v5.5.0](https://github.com/trufflesuite/truffle/releases/tag/v5.5.0): use Truffle Dashboard to deploy with MetaMask, supports hardware wallets and Hardhat
- Brownie [v1.18.0](https://github.com/eth-brownie/brownie/releases/tag/v1.18.0): Ganache v7 support, override storage for eth\_call, config EVM version per language and use latest compiler setting
- Nethereum (.Net library) [v4.2.0](https://github.com/Nethereum/Nethereum/releases/tag/4.2.0): human readable ABI, EIP712 improvements, support for GnosisSafe, MultiSend & Sign-In with Ethereum
- [ctc](https://github.com/fei-protocol/checkthechain#readme): Python package and CLI for historical data analysis of EVM chains
- [Heliaia](https://github.com/GregTheGreek/Heliaia#readme): analyze transactions before broadcasting, sits between wallet & node
- [Detect off-chain evaluation](https://karmacoma.notion.site/Detecting-if-we-re-evaluated-off-chain-aa5fb334f4e640aead68784ea065daf9) using view function values such as msg.sender
- [StealthDrop](https://github.com/nalinbhardwaj/stealthdrop#readme): ERC20 airdrops that can be claimed anonymously using zk proofs, currently has vulnerability
- noble-ed25519 [v1.6.0](https://github.com/paulmillr/noble-ed25519/releases/tag/1.6.0): ZIP-215 support, audited by Cure53
- Map of [ENS](https://twitter.com/avsa/status/1493634935038656519) contracts
- Deep dive into [OlympusDAO](https://norswap.com/olympus/) contracts
- Accounts in Ethereum [explainer](https://dev.to/q9/finally-understanding-ethereum-accounts-1kpe)  

**Security**

- RigoBlock [exploited](https://twitter.com/RigoBlock/status/1494351180713050116), all tokens in Dragos except ETH and USDT at risk, set multiple allowances function missing only owner modifier
- Echidna [v2.0.0](https://github.com/crytic/echidna/releases/tag/v2.0.0) (fuzzer): assertion failure & integer over/underflow detection in Solidity v0.8, contract destruction detection and max value discovery
- [Uniswap oracle attack simulator](https://blog.euler.finance/uniswap-oracle-attack-simulator-42d18adf65af): quantify risks on v3 TWAP price oracles
- Austin Williams: [Chainlink VRF operators](https://email.mg2.substack.com/c/eJwtkM2OhCAMgJ9mOBr5U3vgsJd9DYNQR3YUDZQxvv3iziYNAVr42s9ZwueeLnPsmdi9jHQdaCKeeUUiTKxkTGPwRgxacs28UZ4PemAhj3NC3GxYDaWC7CjTGpylsMe7nrc9Z4tppey1FhxU33UWvO4VWMG5myX0ftYfqC0-YHRo8I3p2iOy1SxER37Ir4f4rkFnuNtp3L7VU6047TWX6G5cvchkqeS64QqUhAGEACE71UEPLBjRihocajdCiEY03WQdSFCopLMdF80E-T39FP5Q7fYUTS5T_dK9bh5Lxkaf8Kw5t1taytFEpHvgsaa3EgNdI0Y7reg_Lugj9M_O-MSIqYr2oyXDO6WF4lpL4P_DV1kKWs473bLK9Xt9Fc2J-AoVs2DCsv0CbY2NEg) can attempt favorable outcomes, **Correction: [VRF operators must control substantial hashpower](https://twitter.com/onewayfunction/status/1495471479391096834) to influence bias randomness**
- [Ice phishing](https://www.microsoft.com/security/blog/2022/02/16/ice-phishing-on-the-blockchain/) could be detected when EOA granted multiple ERC20 approvals

**Ecosystem**

- Dates announced for [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) in Bogotá: October 11-14
- ETHDenver [videos](https://www.youtube.com/playlist?list=PLAy4HNUNlzRmYhKZxvPifaERMYreW_jPu)
- Schelling point [videos](https://www.youtube.com/playlist?list=PLvTrX8LNPbPlryx_S85pZPfH9yD7qcPsg)
- Ethereum Foundation [Q3 & Q4 grantees](https://blog.ethereum.org/2022/02/15/esp-q3-q4-allocation-update/)
- Etherscan [Gas Tracker](https://twitter.com/etherscan/status/1492485388136419328) adds cost estimates for common transactions
- [Gas dashboard](https://twitter.com/hildobby_/status/1493634750430523396) on Dune Analytics

**Enterprise**

- [Twitter](https://twitter.com/TwitterSupport/status/1494008973581856768) adds ETH addresses to Tips feature, ENS not currently supported
- J.P. Morgan: [metaverse opportunities](https://www.jpmorgan.com/content/dam/jpm/treasury-services/documents/opportunities-in-the-metaverse.pdf) \[PDF\] with lounge in Decentraland
- [Battleship](https://www.baseline-protocol.org/blog/battleship-baseline/): simple game implementation using Baseline Protocol
- [Bud Light](https://www.budlight.com/nft/) NFTs sold for flat fee in US, [Nouns glasses](https://twitter.com/budlight/status/1493011386330398720) in Super Bowl commercial
- [Universal Music Group](https://www.universalmusic.com/universal-music-group-partners-with-curio-to-develop-nft-fan-collections-for-its-record-labels-and-artists/) partners with Curio for NFTs

**Application layer**

- Risk Harbor [v2](https://medium.com/riskharbor/risk-harbor-core-v2-launches-core-vault-2-on-arbitrum-with-support-for-tracer-finance-1c365d70026) supports Tracer Finance on Arbitrum
- [Strips Finance](https://strips-finance.medium.com/strips-mainnet-beta-open-832d74bc65f) (interest rate DEX) beta live on Arbitrum
- [Vortex](https://medium.com/akropolis/vortex-is-now-live-on-binance-smart-chain-and-arbitrum-f516577d6d5a) (on-chain basis trading strategy) live on Arbitrum
- [Clipper](https://blog.clipper.exchange/clipper-is-now-live-on-optimism/) (small trade DEX) live on Optimism
- Enzyme [v4 Sulu](https://medium.com/enzymefinance/enzymes-sulu-is-live-62721f3b2bb8) (asset management) live on mainnet
- [Future of MakerDAO](https://hexonaut.medium.com/maker-past-present-and-future-9fd67da4f229): focus on due-diligence of protocols wanting to mint
- Synthetix dynamic exchange fee [explainer](https://blog.synthetix.io/dynamic-exchange-fees-explained/)
- Instadapp [Uniswap staking rewards portal](https://twitter.com/Instadapp/status/1493239700236402699) to create, stake & manage
- [0xSplits](https://mirror.xyz/0x50671995E1ECa15Ca9E807774A814331CabE0F3b/hO97ZEqyE03Qt-3cFcmvsDQuYgr4jLQzBFCG9UiJie0): split incoming funds between recipients using preset percentages 
- [Livepeer](https://medium.com/livepeer-blog/the-confluence-upgrade-is-live-3b6b342ea71e) migrated to Arbitrum
- [OpenSea](https://twitter.com/opensea/status/1494782318619205636) updates contract, NFT listings will expire Feb 25 unless migrated
- [x2y2](https://twitter.com/the_x2y2/status/1493734526610071554): NFT marketplace with airdrop for listings and rewards for staking
- [Propy](https://twitter.com/PropyInc/status/1491919546831286273) sells US house via NFT auction

* * *

### **Job Listings**

- Kwenta seeks [Frontend Engineer](https://blog.kwenta.io/kwenta-open-position-front-end-developer/), [Solidity Engineer](https://blog.kwenta.io/kwenta-open-position-solidity-engineer/) & [Marketing Lead](https://blog.kwenta.io/kwenta-open-position-marketing-manager/)
- Roles at Gnosis [Sr DevRel Eng.](https://grnh.se/3052a2da2us) [Sr Production/Reliability Eng.](https://grnh.se/3345ebe02us) [DevOps Eng.](https://apply.workable.com/blockscout/j/0D9C5798DC/)
- [Nomic Foundation](https://www.notion.so/Nomic-Foundation-jobs-991b37c547554f75b89a95f437fd5056) hiring Rust Tech Lead & Ethereum Tech Lead
- [Internship program](https://nethermind.notion.site/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1) with Nethermind (1-3 month) 
- [Senior Technical Writer](https://ethereum.bamboohr.com/jobs/view.php?id=51&source=weekinethnews) to take ownership & completely redo the Geth docs
- EF research hiring [Networking Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=54&source=weekinethnews)
- [Re7 Capital](https://www.re7.capital/) – a DeFi yield fund – is hiring [analysts and data engineers](https://apply.workable.com/re7-capital/)

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [BlockFi $100 million settlement](https://www.sec.gov/litigation/admin/2022/33-11029.pdf) \[PDF\] with US SEC & states for BlockFi Interest Accounts; SEC Commissioner Pierce’s [statement](https://www.sec.gov/news/statement/peirce-blockfi-20220214)
- [TRUST](https://blog.coinbase.com/introducing-the-travel-rule-universal-solution-technology-trust-232774d76674): Travel Rule compliance solution by US crypto exchanges
- Jake Chervinsky: [US stablecoin regulation update](https://twitter.com/jchervinsky/status/1494041969533853700)
- [Canada using Emergencies Act](https://deputypm.canada.ca/en/news/news-releases/2022/02/15/canada-invokes-emergencies-act-limit-funding-illegal-blockades-and) for financial service providers to freeze accounts believed to be affiliated with protests without a court order
- [US Justice Department](https://www.justice.gov/opa/pr/justice-department-announces-first-director-national-cryptocurrency-enforcement-team) appoints first Director of cryptocurrency enforcement team and reveals FBI’s virtual asset exploitation unit
- [US Federal Reserve](https://www.federalreserve.gov/newsevents/pressreleases/monetary20220218a.htm) prohibits senior officials holding investments in cryptocurrency amongst other investments
- [UK tax authority first seizure of NFTs](https://www.bbc.com/news/business-60369879) in tax fraud investigation
- Packy McCormick’s [tokenomics resource list](https://twitter.com/packym/status/1493990833397325824)

**General**

- Social engineering [scam](https://twitter.com/thomasg_eth/status/1492663192404779013) using token approvals
- [80 column default](https://twitter.com/paintyourdragon/status/1493477940352352257) can be traced back to foolscap paper size from late 1400s 

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-february-19-2022](https://weekinethereumnews.com/week-in-ethereum-news-february-19-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Feb 23 – Mar 11 – [Codeless Conduct](https://codelessconduct.org/) no-code hackathon (virtual)
- Mar 9-24 – [Gitcoin Grants Round 13](https://twitter.com/gitcoin/status/1488231821854740481)
- Mar 11-20 – [Ethereum Rio](https://www.ethereum.rio/)
- Mar 15 – [Cryptocurrency Class](https://mirror.xyz/0xaFaBa30769374EA0F971300dE79c62Bf94B464d5/oGqGP2NOK9g7QPl1sMKkzql_Fh0P6hKbpYLZ-EkQTXU) starts (virtual) 
- Mar 16 – submission deadline for [Underhanded Solidity Contest](https://underhanded.soliditylang.org/)
- Mar 17-18 – [ETH Austin](https://2022.ethaustin.org/) summit
- Mar 29-31 – [ETHDubai](https://www.ethdubaiconf.org/)
- Apr 7-9 – [ETH Portland](https://2022.ethportland.com/) hackathon
- Apr 18-25 – [Devconnect](https://devconnect.org/schedule) (Amsterdam)
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- May 3-8 – [spaghettETH](http://spaghett-eth.com/) (Milan)
- May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETHNewYork](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- **Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)**
- **Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)**
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

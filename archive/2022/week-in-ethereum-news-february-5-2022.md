---
title: "Week in Ethereum News <br> February 5, 2022"
date: "2022-02-05"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest core devs [call video](https://www.youtube.com/watch?v=_kt-r4J8PJc&t=139s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1489710356452675584):
    - Stakers should be [cognizant to have enough disk space](https://notes.ethereum.org/@ExXcnR0-SJGthjz1dwkA1A/BkkdHWXTY) in case of non-finality periods
    - Kiln devnet expected late next week, app devs & infrastructure providers should test on this prior to public testnets
    - Testnets in our post-PoW world: Goerli & Sepolia to continue, Ropsten & Rinkeby to be deprecated
    - Shanghai upgrade discussion on EIPs to include: EVM changes, account abstraction, reduction in rollup fees & removing self destruct
    - Preview of [executable spec](https://ethereum.github.io/execution-specs/) for execution layer
- Vitalik’s proposal for [blob transactions in same format as sharding](https://notes.ethereum.org/@vbuterin/blob_transactions) to provide scaling relief for rollups, along with a [simpler](https://notes.ethereum.org/@vbuterin/blob_transactions_simple) version

**Proof of Stake consensus layer**

- Danny Ryan’s [Finalized PoS update](https://blog.ethereum.org/2022/01/31/finalized-no-33/): engineering progressing for PoW switch off; no progress on client diversity, run a minority client to protect your ETH
- Lighthouse [v2.1.2](https://github.com/sigp/lighthouse/releases/tag/v2.1.2): improves peer stability, Key Manager API support & optimized Docker images
- Prysm [v2.0.6](https://github.com/prysmaticlabs/prysm/releases/tag/v2.0.6): patch release, improved memory usage, JSON API fixes
- Lodestar [v0.34.0](https://github.com/ChainSafe/lodestar/releases/tag/v0.34.0): optimization for non-finality periods, Bellatrix spec upgrades & fixes and remote signer support
- Polynya: Danksharding [explainer](https://polynya.medium.com/danksharding-36dc0c8067fe)
- Ben Edgington’s Upgrading Ethereum book [Simple Serialize (SSZ)](https://upgrading-ethereum.info/altair/part2/building_blocks/ssz) chapter

**PoW switch off**

- Kiln v1 [spec](https://hackmd.io/@n0ble/kiln-spec) (pre-production sprint for PoW switch off): optimistic sync fixes, semantic changes to better handle reorgs
- [Geth](https://twitter.com/peter_szilagyi/status/1489136403376136193) close to being ready for PoW switch off, one major PR awaiting tests

**EIPs/Standards**

- [EIP4762](https://github.com/ethereum/EIPs/blob/ff727b3bda04371a7c4ab6ac3ffcc227745f9ee0/EIPS/eip-4762.md): Statelessness gas cost changes
- [EIP4760](https://github.com/ethereum/EIPs/blob/3b37b6ce5b332d009b871d1205659b9923dcfd92/EIPS/eip-4760.md): SELFDESTRUCT bomb
- [EIP4758](https://github.com/ethereum/EIPs/blob/cc8cd8d86b7e0dfb541caf3a5396ab1687a46d93/EIPS/eip-4758.md): Deactivate SELFDESTRUCT
- [EIP4750](https://github.com/ethereum/EIPs/blob/3ca4f87938f0295a06fa07eb530b4f3cd7774fcd/EIPS/eip-4750.md): EOF Functions
- [EIP4747](https://github.com/ethereum/EIPs/blob/f0e85de590bba2e3b7f3c37a80f05f95585743d9/EIPS/eip-simplify-161.md): Simplify EIP 161
- [EIP4736](https://github.com/ethereum/EIPs/blob/2e35b58f62802fe10f4b0adf494ebdd34e023f13/eip-draft_clwp.md): Consensus Layer Withdrawal Protection

**Layer2**

- [L2Savings](https://www.l2savings.org/): shows Layer 2 transactions and estimated saving if these were made on mainnet
- [Sliding window](https://arxiv.org/abs/2201.09009) for challenge process, allows significant decrease of the deadline for challenge-response and expands the deadline during congestion
- [Secure Asymmetric Frugal Exchange](https://ethresear.ch/t/optimizing-cross-chain-swaps/11924) prototype for optimized batched cross-chain swaps, gas efficient transferring from Layer 2 to mainnet

* * *

### **This newsletter is made possible thanks to [Celer](https://www.celer.network/)!**

![Celer](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

Celer Network is a layer-2 scaling platform that brings fast, secure and low-cost blockchain applications.

Check out our [Inter-chain Message Framework](https://blog.celer.network/2022/01/12/celer-inter-chain-message-framework-the-paradigm-shift-for-building-and-using-multi-blockchain-dapps/), currently **live on testnet**!

Devs can now build inter-chain-native dApps with efficient liquidity utilization, coherent application logic, and shared states.  

With Celer’s IM framework, devs can:

- Bridge assets + make cross-chain calls at the same time 
- Pass arbitrary messages and execution instructions all with a single click

Check out our [developer docs](https://cbridge-docs.celer.network/developer/cbridge-sdk).

* * *

**Stuff for developers**

- [Foundry gas reports](https://twitter.com/brockjelmore/status/1487882666141798406): gas usage report generated when running tests
- Hardhat [roadmap](https://twitter.com/alcuadrado/status/1488164159439220736): opinionated, streamlined default experience, with ability to opt-out of defaults
- Remix [v0.21](https://medium.com/remix-ide/remix-v0-21-0-v0-21-1-released-550dbde6428b): migrated to React, updated backup & restore, added StarkNet plugin, removed Optimism plugin as no longer required
- EthereumJS:
    - VM [v5.7](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs%2Fvm%405.7.0): opcode dynamic gas costs for debugging and easier state manager customization
    - Client [v0.3](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs%2Fclient%400.3.0): added RPC endpoints for logs, transaction receipt & transaction by hash and support for Sepolia testnet
    - TX [v3.5](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs%2Ftx%403.5.0): additional data integrity checks
- Ethers.js [v5.5.4](https://github.com/ethers-io/ethers.js/releases/tag/v5.5.4): support invalid IPFS URI format
- [ExcessivelySafeCall](https://github.com/nomad-xyz/ExcessivelySafeCall): Solidity library to call untrusted contracts and prevent return bombing by specifying maximum bytes to copy
- [Cloaks](https://github.com/abigger87/cloaks#readme): ERC721 with bid commit/reveal scheme, mint price is mean of bids; [SPADES](https://github.com/abigger87/spades#readme) variant: revealers get discounted mint, public mint price increases per mint and decays per block 
- [Cairo Language Server](https://github.com/ericglau/cairo-ls#readme): adds Cairo support to IDEs implementing Language Server Protocol such as VS Code, early preview
- [Cairo Math 64x61](https://github.com/influenceth/cairo-math-64x61#readme): fixed point 64.61 math library
- Sign-In with Ethereum [docs](https://docs.login.xyz/)
- [Single use address](https://twitter.com/ernestognw/status/1487213988408614913) guide, without the need for a private key (Nick’s method)
- Alchemy [NFT API](https://www.alchemy.com/nft-api) on mainnet
- [0x Protocol v4 NFT swaps](https://blog.0x.org/introducing-multi-chain-nft-swaps/), off-chain & on-chain listings, lowers gas costs, on Ropsten testnet
- [3D interactive NFT](https://twitter.com/sayangel/status/1487913266277982212) using gITF (Graphics Language Transmission Format)
- Tweet storm of [building on-chain SVG NFT](https://twitter.com/tom_hirst/status/1489320762926256130) project
- OpenSea’s [guide to creating an NFT](https://docs.opensea.io/docs/creating-an-nft-contract) using Hardhat, IPFS & OpenZeppelin
- [Intro to web3](https://mirror.xyz/dhaiwat.eth/O5CK6Tjfv8uhl6FPbjT0yZ8LUwViDPWGYHdu9khRWpM) for web2 frontend devs

**Security**

- Wormhole’s Solana/Ethereum bridge [~$300 million exploit](https://twitter.com/samczsun/status/1489044939732406275), attacker spoofed guardian signatures after input wasn’t properly validated, 120k Wormhole ETH minted on Solana, 93k ETH bridged back to Ethereum
- Qubit bridge [post-mortem](https://blog.theori.io/news/qubit-post-mortem/), code modified after audit, additional mitigations could have reduced risk
- Index Coop Rari pool [attempted attack](https://twitter.com/NoahCitron/status/1487605582584418305), Uniswap V3 TWAP oracle manipulation prevented by arb bot, attacker lost 68 ETH
- List of [Smart Contract Vulnerabilities](https://github.com/sirhashalot/SCV-List#readme)

**Ecosystem**

- Vitalik’s [reminder on shared security](https://old.reddit.com/r/ethereum/comments/sgd3zt/a_quick_reminder_of_what_shared_security_means/), rollups are just as secure as Ethereum mainnet, Validiums somewhat less secure, sidechains/independent layer 1s much less secure
- NFT marketplaces [should show transfer recipient information](https://twitter.com/punk6529/status/1489387642018050050) such as ENS, account name, previous transfers and NFTs held to prevent transfer errors
- 0xPARC: [ZK-Identity](https://0xparc.org/blog/zk-id-1) should be used to re-architect identity systems putting users in control of their data
- Sign-in with Ethereum: [concept of session keys](https://blog.spruceid.com/from-sign-in-with-ethereum-to-session-keys/), ephemeral keys for a user’s session, stored in the browser with very limited permissions

**Enterprise**

- [GameStop NFT marketplace](https://twitter.com/immutable/status/1489209166010847232) to be powered by Immutable X, marketed as carbon neutral with no gas fees; $100 million for creator grants
- [Nike sues StockX](https://www.reuters.com/technology/nike-cries-foul-over-virtual-shoes-suing-retailer-that-sells-sneaker-nfts-2022-02-04/) for selling NFTs with unauthorized images of sneakers

**Application layer**

- [UMA optimistic oracle](https://twitter.com/UMAprotocol/status/1488334871995072513) live on Optimism, Boba Network & Arbitrum
- [Thales](https://twitter.com/thalesmarket/status/1489252623882461198) migrated to Optimism
- [Rubic](https://cryptorubic.medium.com/the-arbitrum-network-has-been-successfully-integrated-into-rubic-cf1637291d2a) multichain swaps adds Arbitrum
- Mean Finance [v2](https://twitter.com/mean_fi/status/1488248678209007618) Dollar Cost Average protocol for tokens live on Optimism
- [Kuiper](https://medium.com/@Kuiper_Finance/kuiper-a-decentralized-financial-protocol-for-index-tracking-71abf3abcc8f) permissionless index tracking live on mainnet
- [Utopia Core](https://mirror.xyz/utopialabs.eth/nEf_vetIxx7efsqkrk6erqjUFWnuqOxke46My5ICWIQ): DAO payroll, payments & expenses using Gnosis Safe, public beta
- Lit Protocol adds token gated [Zoom](https://litgateway.com/apps/zoom) meetings/webinars and [WordPress](https://litgateway.com/apps/wordpress) 
- [Arcade](https://twitter.com/arcade_xyz/status/1488200348087037952?s=20&t=y8N6sjot1kEcrQJd_9q_4g) NFT lending platform live on mainnet
- [Rarible](https://twitter.com/rarible/status/1489322890650689540) adds floor bids for any NFT in a collection
- Mirror [Plugins](https://dev.mirror.xyz/P0iUQ2DPCcZXLlAcv-akmm5W8UYdSf4PpD2_QeeI3k4): first plugin is minting ERC20 tokens

* * *

### **Job Listings**

- [Re7 Capital](https://www.re7.capital/) – a DeFi yield fund – is hiring [analysts and data engineers](https://apply.workable.com/re7-capital/)
- Wanna build a cutting edge ETH Staking pipeline? [🅐ℙⓅ🄻ʸ for Ether Capital](https://bit.ly/ethcapdevops)
- [Senior Technical Writer](https://ethereum.bamboohr.com/jobs/view.php?id=51&source=weekinethnews) to take ownership & completely redo Geth docs
- EF research hiring [Networking Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=54&source=weekinethnews)
- [Internship program](https://nethermind.notion.site/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1) at Nethermind (1-3 month) 

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [India](https://pib.gov.in/PressReleasePage.aspx?PRID=1794131) to tax transfer of digital asset income at 30%
- [UK tax authority guidance](https://cryptouk.io/2022/02/02/hmrc-defi-guidance-2nd-feb-22/) treats DeFi deposits as asset disposal triggering capital gains
- US [Virtual Currency Tax Fairness bill](https://www.coincenter.org/congress-takes-a-step-toward-a-de-minimis-exemption-for-everyday-cryptocurrency-transactions-2022/) reintroduced to exempt personal crypto transactions where gains are $200 or less
- [Circle runs ads](https://twitter.com/jerallaire/status/1488863139252760579) in US newspapers on how the US can win the digital currency space race
- [ConsenSys acquires MyCrypto](https://consensys.net/blog/press-release/consensys-acquires-mycrypto-to-strengthen-metamask-partnership-and-enhance-web3-experiences/) to join MetaMask team
- [Skepticism of ve-tokenomics](https://forum.makerdao.com/t/signal-request-gbmkr-a-proposal-to-benefit-long-term-mkr-holders/12756/16): reduced investor base, staking derivatives, short term incentives, bribery and prisoners’ dilemma
- Update on the [Triple Halving](https://squish.substack.com/p/the-triple-halving-where-we-stand) thesis
- Visualization of [ETH and BTC percentage share of fees](https://twitter.com/cburniske/status/1488346430271934467) over time

**General**

- Estimating [bit security of pairing-friendly curves](https://research.nccgroup.com/2022/02/03/estimating-the-bit-security-of-pairing-friendly-curves/)
- [EU data protection authorities](https://www.iccl.ie/news/gdpr-enforcer-rules-that-iab-europes-consent-popups-are-unlawful/) find industry bodies consent system violates GDPR and all data collected must be deleted
- German Court rules [embedding Google Fonts violates GDPR](https://thehackernews.com/2022/01/german-court-rules-websites-embedding.html)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-february-5-2022](https://weekinethereumnews.com/week-in-ethereum-news-february-5-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Feb 11 – PoW switch off [community call](https://github.com/ethereum/pm/issues/465)
- Feb 17 – [Schelling Point](https://schellingpoint.gitcoin.co/) (Denver) 
- Feb 18-20 – [ETHDenver](https://www.ethdenver.com/)
- Feb 23 - Mar 11 – [Codeless Conduct](https://codelessconduct.org/) no-code hackathon (virtual)
- **Mar 9-24 – [Gitcoin Grants Round 13](https://twitter.com/gitcoin/status/1488231821854740481)**
- Mar 11-16 – [Ethereum Rio](https://www.ethereum.rio/)
- Mar 15 – [Cryptocurrency Class](https://mirror.xyz/0xaFaBa30769374EA0F971300dE79c62Bf94B464d5/oGqGP2NOK9g7QPl1sMKkzql_Fh0P6hKbpYLZ-EkQTXU) starts (virtual) 
- Mar 17-18 – [ETH Austin](https://2022.ethaustin.org/) summit
- Mar 29-31 – [ETHDubai](https://www.ethdubaiconf.org/)
- Apr 7-9 – [ETH Portland](https://2022.ethportland.com/) hackathon
- **Apr 18-25 – [Devconnect (Amsterdam)](https://blog.ethereum.org/2022/02/01/devconnect-dates-and-details/)**
- **Apr 19-20 – [Layer Two Amsterdam](https://amsterdam.l2beat.com/)**
- Apr 20-21 – [The Alliance (gaming) summit](https://medium.com/1kxnetwork/announcing-alliance-summit-7e8732c9fd9d) (Amsterdam)
- Apr 21 – [ETHconomics](https://ef-events.notion.site/ETHconomics-Devconnect-676d73f791684e18bfae35bbc9e1fa90) (Amsterdam)
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
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

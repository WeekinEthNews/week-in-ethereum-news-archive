---
title: "Week in Ethereum News <br> March 26, 2022"
date: "2022-03-26"
---

## **Eth News and Links**

**Mainnet execution layer**

- Tim Beiko’s [core devs update](https://tim.mirror.xyz/M_3JZXBkvXnr3W1222WIDo1ipMuFymszjH-FP40CO5c): merge testing, difficulty bomb can be pushed back as needed, Shanghai update proposed features, executable spec for execution layer and token compensation for client devs & researchers
- ethereumjs/client [v0.4.0](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs%2Fclient%400.4.0): Kiln v2 support

**Proof of Stake consensus layer**

- Danny Ryan’s [Finalized PoS update](https://blog.ethereum.org/2022/03/23/finalized-no-34/): help test the merge!
- PoS implementers [call video](https://www.youtube.com/watch?v=ThoT6-eLTN0&t=318s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/SybzPe5f5):
    - Goerli testnet was shadow forked, will test endianness fixes
    - merge-devnet-6 next week
    - mainnet shadow fork in two weeks
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220325)
- Teku [v22.3.2](https://github.com/ConsenSys/teku/releases/tag/22.3.2): fixes performance issue when processing blocks containing deposits; [incident review](https://github.com/ConsenSys/teku/wiki/Post-Incident-Review---Deposit-Processing-Performance)
- [DAppNode](https://twitter.com/DAppNode/status/1504809228271296512) now supports Teku, Lighthouse & Prysm clients on Prater testnet
- Vitalik’s EIP4844 proto-danksharding [technical FAQ](https://notes.ethereum.org/@vbuterin/proto_danksharding_faq) 

**PoW switch off (The Merge)**

- Dankrad: [running a majority client](https://dankradfeist.de/ethereum/2022/03/24/run-the-majority-client-at-your-own-peril.html) puts you at serious risk of losing funds
- wat, wen, wy: [stuff Ethereum Reddit should know](https://www.reddit.com/r/ethereum/comments/tijcq1/stuff_rethereum_should_know_proof_of_stake_edition/) about the merge
- [Goerli shadow fork](https://twitter.com/vdWijden/status/1507244702218784770) successfully merged
- [Kiln testnet image for Raspberry Pi](https://twitter.com/ethereumonarm/status/1506212258430476288) updated: adds Erigon execution client; 16 execution & consensus layer combinations
- Setup guide for [ethereumjs client & Lodestar for Kiln testnet](https://twitter.com/efjavascript/status/1507313725996425253)
- [Geth master branch](https://twitter.com/vdwijden/status/1506899633741705217) has all important changes for PoW switch off
- Client teams [adding panda ascii art](https://twitter.com/terencechain/status/1506346434370494465) to display when merged

**EIPs/Standards**

- [EIP4938](https://github.com/ethereum/EIPs/blob/bf97a223017b835ef7f7a7c86f52b98a70b31329/EIPS/eip-4938.md): eth/67: Removal of GetNodeData

**Layer2**

- [Fraud proof attack vectors](https://medium.com/infinitism/optimistic-time-travel-6680567f1864) on optimistic rollups: time-travel attack & reality-distortion attack;  Optimism’s Cannon & Arbitrum’s Nitro expected to reduce attack surface
- [Optimism calldata compression](https://twitter.com/optimismPBC/status/1507077884594241547) live, 40% fee reduction expected next week
- [Huobi](https://twitter.com/huobiglobal/status/1506868755409760259) adds Ether deposits & withdrawals on Optimism
- [Ramp](https://twitter.com/RampNetwork/status/1506211050907131908) adds buying Ether on Arbitrum
- Raiden becoming a [payment network on top of rollups](https://medium.com/raiden-network/the-state-of-the-raiden-network-9aa4b9a9e2fc)
- [Aztec (privacy zk rollup)](https://medium.com/aztec-protocol/privacy-for-pennies-scaling-aztecs-zkrollup-9f2b36615cc6) reducing transaction fees, 30% cheaper proof (with plans to get to 180k gas) and 8x improvement to 896 Aztec transactions per mainnet transaction

* * *

### **This newsletter is made possible thanks to [Nexus Mutual](https://nexusmutual.io/)!**

![Nexus Mutual Protocol Cover](https://weekinethereumnews.com/wp-content/uploads/2022/03/Nexus-Mutual-Protocol-Cover-1024x586.png)

Go where the yield takes you, but don’t let the next hack set you back. Regardless of where you are chasing yield, Protocol Cover can protect your productive crypto assets across L1s, L2s, and scaling solutions. 

Maximize yield. Minimize risk. Enjoy peace of mind knowing Nexus Mutual has you covered. [Become a member](https://nexusmutual.io/) and cover your asse(t)s against the major risks in DeFi.

* * *

**Stuff for developers**

- ethereumjs/vm [v5.8.0](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs%2Fvm%405.8.0): Kiln v2 support, EIP3540 EVM Object Format, EIP3670 EOF - code validation, EIP3860 limit & meter initcode and improved Layer 2 support
- TypeChain [v8](https://github.com/dethcrypto/TypeChain/releases/tag/typechain%408.0.0) (TypeScript typings): supports nested paths, Foundry style artifacts and prefers \`import type\`
- Hardhat VSCode extension [v0.2.0](https://twitter.com/hardhathq/status/1507393377490415617): hover for type info
- Hardhat [v2.9.2](https://github.com/NomicFoundation/hardhat/releases/tag/2.9.2): forking fix
- [EBMP](https://github.com/0xmostima/EBMP#readme): render BMP images in Solidity for on-chain BMP NFTs
- [MagicCounter](https://github.com/0xMisaka/Sol-MagicCounter#readme): Solidity counter, increment/decrement/min/max in O(1)
- [Dapptools](https://twitter.com/gakonst/status/1506669474920886273) passes the torch to Foundry
- Opinionated [Foundry project setup guide](https://www.libevm.com/2022/03/19/opinionated-forge-guide/)
- [Hardhat project template](https://github.com/pcaversaccio/hardhat-project-template-ts#readme) (based on Typescript): adds testing with Foundry
- create-eth-app [v1.8.0](https://github.com/paulrberg/create-eth-app/releases/tag/v1.8.0): integrates useDapp framework in React based templates 
- [StarkNet development](https://medium.com/starknet-edu/the-ultimate-starknet-dev-environment-716724aef4a7) setup guide
- Nile [v0.5.0](https://github.com/OpenZeppelin/nile/releases/tag/v0.5.0): Cairo v0.8.0 support, new Signer for latest Account contract
- [ENS Layer 2/off-chain integration](https://medium.com/the-ethereum-name-service/upgrade-ethers-js-to-5-6-1-to-activate-ens-l2-offchain-integration-40ee1a0fdf2a) with ethers.js v5.6.1
- Alchemy’s [Goerli testnet faucet](https://goerlifaucet.com/)

**Security**

- Umbrella Network ~$700k [exploit](https://twitter.com/peckshield/status/1505495324516782081) on Ethereum & BNB chain, unchecked underflow in withdraw function
- LI.FI ~$600k [exploit](https://blog.li.finance/20th-march-the-exploit-e9e1c5c03eb9), swap function used to transfer approved tokens
- TUSD integration with Compound [post mortem](https://blog.openzeppelin.com/compound-tusd-integration-issue-retrospective/), millions were at risk, token double entry point caused vulnerability when used as collateral, other DeFi protocols were potentially affected, TUSD now patched
- ENS price oracle deployment [post mortem](https://discuss.ens.domains/t/postmortem-ep9-deployment/11662), if vote had passed expired domains could be registered without a premium

**Ecosystem**

- [EIP1559 burnt](https://twitter.com/k06a/status/1506026605063327747) 2 million ETH
- Polynya: [modular execution layers](https://polynya.medium.com/modular-execution-layers-df256768ac2f) and [what everyone gets wrong about modular blockchains](https://polynya.medium.com/updated-thoughts-on-modular-blockchains-ce1b159fa1b3)
- Goerli testnet Ether is being traded, Afri proposes to [inflate Goerli Ether supply](https://github.com/goerli/testnet/issues/97) to prevent it having value

**Enterprise**

- [Baseledger Proxy open-sourced](https://unibrightio.medium.com/baseledger-proxy-open-sourced-7b6d013563d8) by Unibright
- [10KTF Gucci Grail](https://vault.gucci.com/en-US/story/gucci-grail) NFTs revealed
- [10:22PM (Universal Music label) buys Bored Ape](https://www.universalmusic.com/1022pm-buys-bored-ape-5537-and-joins-the-bored-ape-yacht-club-community/) to be the manager of KINGSHIP metaverse group

**Application layer**

- [GameStop NFT marketplace](https://beta.nft.gamestop.com/) on [Loopring](https://medium.loopring.io/gamestop-nft-marketplace-powered-by-loopring-l2-6cdb9289d937) & [Immutable X](https://twitter.com/Immutable/status/1506596126677295108) opens for signups & deposits
- [Universe](https://medium.com/@markwardbro/universe-marketplace-beta-1aca8956407d) NFT marketplace beta
- [LooksRare](https://twitter.com/LooksRareNFT/status/1505924121053757446) (NFT marketplace) zero code NFT collection minting
- [Prop House](https://twitter.com/cryptoseneca/status/1506723837974614027) (Nouns proposal auction house): first community grants round
- The Graph [R&D roadmap](https://thegraph.com/blog/roadmap-2022) 
- [Superfluid Protocol](https://medium.com/superfluid-blog/superfluid-protocol-is-live-on-optimism-and-arbitrum-3a1f09df541) (money streaming) live on Arbitrum & Optimism
- [MakerDAO](https://forum.makerdao.com/t/mip6-huntingdon-valley-bank-loan-syndication-collateral-onboarding-application/14219): US based Huntingdon Valley bank applies for collateral integration

* * *

### **Job Listings**

- EF’s Privacy & Scaling Explorations team: [Technical Project Coordinator](https://jobs.lever.co/ethereumfoundation/78089bc2-125e-47de-af28-e162de149901?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum), [ZKP Security Engineer](https://jobs.lever.co/ethereumfoundation/b80cf733-9a8d-40f1-a85a-635acdc2b1b1?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum%20), [L2 Security Engineer](https://jobs.lever.co/ethereumfoundation/f3148457-ed1e-4659-941d-5f60b49427ca?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) & [Marketing Ops Manager](https://jobs.lever.co/ethereumfoundation/7a831e7c-1a0d-4e7b-8291-072292e26c0e?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum%20&lever-source%5B%5D=Week%20in%20Ethereum%20)
- SideShift.ai is hiring a [Solidity Engineer](https://sideshift.ai/jobs?utm_campaign=hiring&utm_source=weekinethnews). Good job!
- [Hifi](http://hifi.finance/) is hiring a [Senior Solidity Engineer](https://bit.ly/3CMmbSe) & [Community/Social Media Manager](https://bit.ly/36q06g5)
- EF hiring [Test Engineer](https://jobs.lever.co/ethereumfoundation/e6d303e5-168d-447e-a596-e3c2b105ca3f?lever-source%5B%5D=Week%20in%20Ethereum%20) to improve testing infrastructure & coverage
- Devcon needs a [front-end web developer](https://ethereum.bamboohr.com/jobs/view.php?id=61&source=weekinethnews)
- Status is Hiring! [SDET](https://grnh.se/2241310c1us) and [Head of Marketing (Status Network)](https://grnh.se/2e01bc791us). [All jobs!](https://jobs.status.im/)  
- Mark Cuban seeks a [web3 front-end developer](https://forms.office.com/r/M81g5RNgXX). Send a work sample to apply.
- eVerse is hiring a [lead blockchain engineer](https://everse.notion.site/Lead-Blockchain-Engineer-Architect-845acc3ef4c64784b19d4f2cede8161c) for its social video platform

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Indian parliament passes crypto tax law](https://www.coindesk.com/policy/2022/03/25/indias-stiff-crypto-tax-legislation-becomes-law/): 30% capital gains tax, 1% tax deducted at source for buying & selling
- [US DoJ charge Frosties NFT pair](https://www.justice.gov/usao-sdny/pr/two-defendants-charged-non-fungible-token-nft-fraud-and-money-laundering-scheme-0) with wire fraud and money laundering; IRS agent: “You can’t solicit funds for a business opportunity, abandon that business and abscond with money investors provided you”
- [ANZ](https://www.afr.com/companies/financial-services/anz-the-first-bank-to-mint-an-australian-dollar-stablecoin-the-a-dc-20220323-p5a743) bank mints 30 million of Australian dollar stable coin to pilot payment
- [Non-correlated assets in DeFi](https://medium.com/@rysk-finance/rysk-is-the-only-free-lunch-e4f832af0026) via Rysk's dynamic hedging options AMM \[Disclosure: [Starbloom](https://twitter.com/starbloomvent) portfolio\]
- Simon de la Rouviere: [building expansive NFT universes](https://blog.simondlr.com/posts/expansive-nft-universes-cc0-fidelity-on-chain-bundling) using permissive licensing, low fidelity & metadata and bundling
- [Token compensation explainer](https://www.paradigm.xyz/2022/03/token-compensation-a-brief-explainer-for-job-candidates) for job candidates

**General**

- [Ape & Bored Ape holders](https://twitter.com/sniko_/status/1507015430489067521) targeted in phishing campaign
- [Targeted social engineering](https://twitter.com/arthur_0x/status/1506167899437686784) likely used spear-phishing email
- [HubSpot](https://www.hubspot.com/en-us/march-2022-security-incident) employee account compromised, crypto projects targeted
- [Performance improvement for GKR](https://ethresear.ch/t/performance-improvement-for-gkr/12228), 31x speed-up over Groth16 
- [Web3 will be more secure](https://zengo.com/wagmi-web3-will-be-more-secure-than-web2/) than Web2

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-march-26-2022](https://weekinethereumnews.com/week-in-ethereum-news-march-26-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Mar 29-31 – [ETHDubai](https://www.ethdubaiconf.org/)
- **Apr 8-10 – [DAOHacks](https://dao.ethglobal.com/) (hackathon & summit)**
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
- Sep 6-9 – [MCON 2](https://twitter.com/mcon_world/status/1504175505389457410) (Denver)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

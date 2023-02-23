---
title: "Week in Ethereum News <br> July 30, 2022"
date: "2022-07-30"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- [Goerli Merge announcement](https://blog.ethereum.org/2022/07/27/goerli-prater-merge-announcement/), the final testnet to merge, **update your nodes**, last chance to practice going through the Merge before mainnet:
    - Goerli beacon chain (Prater) Bellatrix upgrade at epoch 112260 (August 4 12:24PM UTC)
    - Merge Terminal Total Difficulty (TTD) set to 10,790,000 (August 6-12)
    - Execution layer clients:
        - Besu [v22.7.0-RC3](https://github.com/hyperledger/besu/releases/tag/22.7.0-RC3)
        - Erigon [v2022.07.04-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.07.04)
        - Geth [v1.10.21](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.21)
        - Nethermind [v1.13.5](https://github.com/NethermindEth/nethermind/releases/tag/1.13.5)
    - Consensus layer clients:
        - Lighthouse [v2.4.0](https://github.com/sigp/lighthouse/releases/tag/v2.4.0)
        - Lodestar [v0.41.0](https://github.com/ChainSafe/lodestar/releases/tag/v0.41.0)
        - Nimbus [v22.7.0](https://github.com/status-im/nimbus-eth2/releases/v22.7.0)
        - Prysm [v2.1.4-rc.0](https://github.com/prysmaticlabs/prysm/releases/tag/v2.1.4-rc.0)
        - Teku [v22.7.0](https://github.com/ConsenSys/teku/releases/tag/22.7.0)
    - Rémy Roy’s guide to running [Geth+Lighthouse](https://github.com/remyroy/ethstaker/blob/main/merge-goerli-prater.md) or [Besu+Teku](https://github.com/remyroy/ethstaker/blob/main/merge-goerli-prater-alt.md)
- For stakers: [Merge config tips](https://notes.ethereum.org/@launchpad/merge-configuration-checklist) & common pitfalls
- EF DevOps [checkpoint sync endpoints](https://notes.ethereum.org/@launchpad/checkpoint-sync#EF-DevOps-Endpoints) to quickly sync a beacon node
- Mainnet-shadow-fork-10 [merged successfully](https://twitter.com/abcoathup/status/1552394627998969856), no client compatibility issues

**Execution layer**

- [Akula](https://twitter.com/PaoloRebuffo/status/1550874921496100868) (Rust version of Erigon) synced full archive node in 35.5 hours, almost twice as fast as Erigon

**Proof of Stake consensus layer**

- PoS implementers [call video](https://www.youtube.com/watch?v=XDfNg8mdC10&t=543s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/BJjamMl69) and [Christine Kim](https://docsend.com/view/5jpzhe3z8x2w2mjz):
    - clarify spec on terminal block execution edge case
    - expand optimistic node definition
    - proposed MEV Boost [circuit breaker](https://hackmd.io/@ralexstokes/BJn9N6Thc) if builder network offline
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220729)

**Layer2**

- EIP4844 (proto-danksharding) [call video](https://www.youtube.com/watch?v=t8B7NBRPBfg) and [notes](https://docs.google.com/document/d/1KgKZnb5P07rdLBb_nRCaXhzG_4PBoZXtFQNzKO2mrvc/edit#)
- Draft proposal for [BLS transaction type](https://research.arbitrum.io/t/draft-for-bls-transaction-type-erc/117)
- Layer 2 fixed and variable [actual gas costs](https://twitter.com/sanjaypshah/status/1552679502018478084)
- [Arbitrum Rinkeby testnet](https://twitter.com/arbitrum/status/1552759659139944453) upgraded to Nitro
- [Rainbow mobile wallet](https://twitter.com/rainbowdotme/status/1551978336359890944) adds NFTs on Arbitrum & Optimism
- Send to beginners: [Optimism starter guide](https://app.optimism.io/get-started)

**EIPs/Standards**

- [EIP5320](https://github.com/ethereum/EIPs/pull/5320/files): Harberger tax NFT
- [EIP5341](https://github.com/ethereum/EIPs/pull/5341/files): NFT referral program
- [EIP5344](https://github.com/ethereum/EIPs/pull/5344/files): Soulmates token 

* * *

### **This newsletter is made possible thanks to Starbloom Ventures!**

![Starbloom Ventures](https://weekinethereumnews.com/wp-content/uploads/2021/11/Screenshot-from-2021-11-19-15-25-51.png)

[](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Ffe86a654-d6dc-42fd-b6c0-0153c15a6788_613x313.png)

Starbloom Ventures is a **first round** venture fund founded by [Evan Van Ness](https://twitter.com/evan_van_ness) to invest in the future of web3. 

We pledge 10% of investing profits to support Ethereum public goods.

* * *

**Stuff for developers**

- [Huff](https://twitter.com/huff_language/status/1552368251186716673) released (low level assembly language for gas-optimized contracts), includes compiler, Foundry library, project template, VSCode extension and contract library (Huffmate)
- Vyper language:
    - [v0.3.4](https://github.com/vyperlang/vyper/releases/tag/v0.3.4/): abi decode, enums, uint2str, ERC5202 factory pattern support
    - Vyper [by Example](https://vyper-by-example.org/)
    - [VyperPunk](https://github.com/SupremacyTeam/VyperPunk#readme): CTF using Brownie
- [Verify two numbers are co-prime](https://github.com/hrkrshnn/notes/blob/main/2022/verify-coprime.org) on-chain
- [Verify ed25519 signatures](https://ethresear.ch/t/verify-ed25519-signatures-cheaply-on-eth-using-zk-snarks/13139) using ZK-Snarks, research project
- ganache [v7.4.0](https://github.com/trufflesuite/ganache/releases/tag/v7.4.0): adds Hardhat console.log support and eth\_getProof
- sol2uml [v2](https://twitter.com/naddison/status/1553048037085564929): adds storage slot visualization with contract values
- Guide to using [slither-read-storage](https://blog.trailofbits.com/2022/07/28/shedding-smart-contract-storage-with-slither/) to retrieve storage slots
- Optimism’s [Drippie](https://dev.optimism.io/drippie-how-optimism-automates-ethereum/): on-chain automation run on services such as Gelato
- ethers-rs [v0.17](https://twitter.com/gakonst/status/1552822989162364928): bug fixes and updated docs
- [evm-translator](https://twitter.com/BrennerSpear/status/1552091025887281152) (TypeScript library): human readable transactions, use in social feeds & simulation 
- [evm-trace](https://banteg.mirror.xyz/3dbuIlaHh30IPITWzfT1MFfSg6fxSssMqJ7TcjaWecM) (Python library): transaction tracing
- Ape [v0.4.0](https://github.com/ApeWorX/ape/releases/tag/v0.4.0): (Python contract framework): improves working with logs & traces, adds historical querying
- wagmi [v0.6](https://twitter.com/wagmi_sh/status/1552056222232104960): adds Prepare Hooks to prepare transactions before sending 
- [NFT Embed](https://twitter.com/nftembed/status/1552292725902516229?s=12&t=Ts8-LTlRJrjvz7H46njjAA): iFrame widget for selling NFTs via Universe marketplace
- [eth.limo](https://twitter.com/eth_limo/status/1551658332611649536) supports on-demand ENS subdomain certificates
- Ethernaut DAO CTF [vending machine solution](https://stermi.medium.com/ethernautdao-ctf-vending-machine-solution-b30a74ba4a0f)

**Security**

- Audius [$1 million exploit](https://blog.audius.co/article/audius-governance-takeover-post-mortem-7-23-22), storage conflict in upgradeable contract allowed reinitialization
- Balancer disclosed [DoS vulnerability](https://medium.com/immunefi/balancer-dos-bugfix-review-8a8ba5d971bf) via flash loans on both entry points of a double entry-point ERC20, $50k bounty paid

**Ecosystem**

- [Prioritize proto-danksharding (EIP4844)](https://twitter.com/kaiynne/status/1552726269980479488) over withdrawals for low cost roll-up transactions 
- a16z [Danny Ryan Q&A](https://future.com/what-the-merge-means-for-ethereum-with-danny-ryan/) on the Merge and beyond
- Ethereum.org [Q3 website roadmap](https://github.com/ethereum/ethereum-org-website/issues/7166)
- Wallet devs call [notes](https://twitter.com/_SamWilsn_/status/1553139331195346950) 
- EF Academic Grants Round $2m to [grantees](https://blog.ethereum.org/2022/07/29/academic-grants-grantee-announce/)

**Application layer**

- Nexus Mutual [ETH staking cover](https://medium.com/nexus-mutual/announcing-eth2-staking-cover-comprehensive-protection-against-slashing-b98b64e0c0fd) to hedge against penalties, slashing & missed rewards
- [Maker DAO](https://twitter.com/MakerDAO/status/1553061778363453443) voting to onboard Societe Generale
- Dark Forest [Nightmarket](https://blog.zkga.me/nightmarket): marketplace for planet coordinates
- Mirror [subscriptions](https://dev.mirror.xyz/Jn62zF5n62BfowdaFgm3uIx3Fgp2vIR7b-HTSxKVXqk): subscribe for new content using Ethereum address & email
- [Moloch DAO](https://daohaus.mirror.xyz/9zJrqvsPGwwqrz89Eea6RdsBd8ba9ZG0oCjY05_BXsY) use cases
- [Things to do on mainnet](https://twitter.com/evan_van_ness/status/1552077868536107008) when gas is low

* * *

### **Job Listings**

- ØVIX and GOGO Protocol seeking [Senior DeFi Blockchain Developer](https://bit.ly/3zc7N4o)
- Overlay (backed by Polychain,1kx,ParaFi) hiring a [Senior Solidity Developer](https://www.notion.so/Overlay-Senior-Solidity-Dev-38c9130a01a844b39ef1bb81f82aae16)
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)
- Status is hiring [UI Designer](https://grnh.se/8c816d6b1us) & [Web Developer](https://grnh.se/d64808fa1us). [All jobs!](https://jobs.status.im/)

**Job listings: $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [UK Law Commission](https://twitter.com/craigwarmke/status/1552660043149053952) proposes new “data objects” personal property category in digital assets consultation paper
- [US FDIC & Fed](https://www.federalreserve.gov/newsevents/pressreleases/bcreg20220728a.htm) demand Voyager Digital stop making misleading statements regarding deposit insurance status
- [Turning on Uniswap fees](https://gov.uniswap.org/t/fee-switch-design-space-next-steps/17132) discussion
- An argument that [perpetual futures tilt the advantage to the house](https://efalken.substack.com/p/perp-funding-rate-fraud)
- [CEO of TBIS](https://www.justice.gov/opa/pr/ceo-titanium-blockchain-pleads-guilty-21-million-cryptocurrency-fraud-scheme) pled guilty to US securities fraud involving ICO
- Nic Carter: [redeem & retain NFTs](https://medium.com/@nic__carter/redeem-and-retain-nfts-are-the-future-of-luxury-goods-760f00dbce23) for physical goods
- [Social rules](https://alisha.mirror.xyz/BIymDSUSm_Di9kS1MafI4ct7IWXPd1LVlgYM2C9A-qc) in DAOs

**General**

- [Validity Proofs](https://blog.connext.network/validity-proofs-are-not-effective-for-bridging-blockchains-85b5e3b22a35) are not a stand-alone solution for bridging
- [Inferring contract invariants](https://junrui-liu.github.io/pdfs/cider.pdf) using reinforcement learning \[PDF\]
- [5.4 million Twitter users data](https://restoreprivacy.com/twitter-vulnerability-exposes-5-million-accounts/) allegedly for sale
- Dan Boneh’s [Cryptography II](https://www.coursera.org/learn/crypto2) course starts October 20

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-30-2022](https://weekinethereumnews.com/week-in-ethereum-news-july-30-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Aug 1 – [Devcon Scholars](https://scholars.paperform.co/) applications close
- **Aug 3 –** [**Devcon wave 05 + 06 tickets**](https://devcon.org/en/tickets/)
- Aug 5-13 – [ETH Seoul](https://2022.ethseoul.org/)
- **Aug 6-12 –** [**Goerli testnet merge**](https://blog.ethereum.org/2022/07/27/goerli-prater-merge-announcement/)
- Aug 8-10 – [ETHToronto](https://www.ethtoronto.ca/)
- Aug 11-13 – [ETH LATAM](https://ethlatam.org/) (Buenos Aires)
- Aug 12 – [Merge Community Call #6](https://github.com/ethereum/pm/issues/580)
- Aug 19-21 – [ETHMexicoCity](https://mexico.ethglobal.com/) (ETH Global)
- Aug 20-22 – [Paradigm CTF](https://ctf.paradigm.xyz/)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev/) (hackathon & conference)
- Sep 2-28 – [ETHOnline](https://online.ethglobal.com/')  (ETH Global)
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Sep 16-18 - [EthBerlin](https://ethberlin.ooo/)
- **Sep 23-24 -** [**BUIDL Asia**](https://www.buidl.asia/vietnam) **(Ho Chi Minh)**
- Sep 27-29 – [Ethereum SP](https://www.ethereumbrasil.com/#next) (São Paulo)
- Oct 7-16 – [Devcon week](https://devcon.org/en/devcon-week/) (Bogotá)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- **Oct 7-9 –** [**Infinite hackathon**](https://infinite-hackathons.eth.limo/) **(Bogotá)**
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

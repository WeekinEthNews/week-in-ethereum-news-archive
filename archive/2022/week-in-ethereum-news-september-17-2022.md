---
title: "Week in Ethereum News <br> September 17, 2022"
date: "2022-09-17"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- [Ethereum now secured by Proof of Stake](https://twitter.com/VitalikButerin/status/1570306185391378434), Proof of Work is obsolete
- [12 second blocks](https://twitter.com/natemaddrey/status/1570856077788585984) post-merge
- Recap of [ethresear.ch posts to get to the Merge](https://twitter.com/icebearhww/status/1570085906073391104) and the [panda meme](https://twitter.com/______jpg______/status/1568973769313501185) back story

**Execution layer**

- Latest core devs [call video](https://www.youtube.com/watch?v=DdUt77_eWyc&t=492s). Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1570403039672168448) and [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-call-147/):
    - Merge went extremely smoothly, 1% drop in participation, minor post-merge issues for Besu & Erigon
    - Shanghai planning will be async until next call on October 27
    - Fork ID will be updated as part of Shanghai upgrade
- Geth [v1.10.25](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.25): disables legacy initial sync
- Nethermind [v1.14.2](https://github.com/NethermindEth/nethermind/releases/tag/1.14.2): fix for receipt not available for block 15537393 error in logs
- KZG ceremony [call video](https://www.youtube.com/watch?v=GUhlpYOZ8Lo)

**Proof of Stake consensus layer**

- Somer’s [Lodestar staking guide](https://someresat.medium.com/guide-to-staking-on-ethereum-ubuntu-lodestar-193a2553a161)
- Teku [v22.9.1-RC1](https://github.com/ConsenSys/teku/releases/tag/22.9.1-RC1): improvements for post-merge performance issues, less tested so only upgrade if you are able to rollback
- [MEV-Boost](https://boost.flashbots.net/) is live, relays available from:
    - [Flashbots](https://boost-relay.flashbots.net/)
    - [bloXroute](https://bloxroutelabs.medium.com/mev-relays-for-ethereum-2-0-980016c72563), unfiltered, no front running & US OFAC compliant variants
    - [Blocknative](https://docs.blocknative.com/mev-relay-instructions-for-ethereum-validators), Dreamboat relay [open sourced](https://github.com/blocknative/dreamboat#readme)
- [Curdleproofs](https://twitter.com/asn_d6/status/1570100991084593152): (zk shuffling scheme) protocol specification & Rust implementation to facilitate secret leader election and protect against DDoS attacks

**Layer 2**

- Optimism [Bedrock alpha testnet](https://oplabs.notion.site/External-Optimism-Bedrock-Alpha-Testnet-454a37e469af4658b89a9d766334e331)
- Polynya argues [EIP4488 (calldata gas cost reduction) should be the focus](https://polynya.mirror.xyz/eq4PNsg-ld4V2LDB7HlHuNm-ULFAtvmVH--utaxAAEs) for scaling
- Dankrad: [using KZG commitments in proofs](https://notes.ethereum.org/@dankrad/kzg_commitments_in_proofs)
- Justin Thaler: [SNARK 80 bits of security is too low](https://a16zcrypto.com/snark-security-and-performance/) and should be at least 100 bits

**EIPs/Standards**

- [EIP5601](https://github.com/ethereum/EIPs/pull/5601/files): Extendable pattern
- [EIP5617](https://github.com/ethereum/EIPs/pull/5617/files): Non-transferable token
- [EIP5630](https://eips.ethereum.org/EIPS/eip-5630): New approach for encryption/decryption
- [EIP5633](https://eips.ethereum.org/EIPS/eip-5633): Composable soulbound NFT, ERC1155 extension
- [EIP5635](https://eips.ethereum.org/EIPS/eip-5635): NFT Licensing Agreements
- [EIP5639](https://eips.ethereum.org/EIPS/eip-5639): Delegation Registry
- [EIP5643](https://eips.ethereum.org/EIPS/eip-5643): Subscription NFTs
- [EIP5646](https://eips.ethereum.org/EIPS/eip-5646): Token state fingerprint
- [EIP5656](https://github.com/ethereum/EIPs/pull/5656/files): Memory copying instruction

* * *

### **This newsletter is made possible thanks to** [**SpeedRunEthereum**](https://speedrunethereum.com/)**!**

![SpeedRunEthereum](https://weekinethereumnews.com/wp-content/uploads/2022/04/Screenshot-from-2022-04-01-15-39-52.png)

Are you a web2 dev who wants to get into web3?

The best way to go from _zero_ to **hero** is [SpeedRunEthereum.com](https://speedrunethereum.com/).

Learn how to build on Ethereum; the superpowers and the gotchas.

Then [speed run Ethereum](https://speedrunethereum.com/) by testing your skills in a [series of challenges](https://speedrunethereum.com/challenge/simple-nft-example) and [join web3](https://twitter.com/austingriffith/status/1493688828661432325).

* * *

**Stuff for developers**

- [OpenZeppelin Upgrades Plugins](https://twitter.com/OpenZeppelin/status/1570432196753891328) adds support for storage gaps
- [Etherscan](https://twitter.com/etherscan/status/1569311894279958531?s=20&t=En2v7nT-gO89J7qyuoG_0w) deprecating Rinkeby & Ropsten explorers October 5
- [hardhat-ignore-warnings](https://github.com/frangio/hardhat-ignore-warnings#readme): plugin to convert warnings to errors & ignore unwanted warnings
- web3.js [v1.8.0](https://github.com/ChainSafe/web3.js/releases/tag/v1.8.0): safe & finalized block tags, required for PoS
- [ABIType](https://github.com/wagmi-dev/abitype#readme): strict TypeScript types for ABIs & EIP712 typed data
- [hardhat-vite](https://github.com/projectsophon/hardhat-vite#readme): plugin wrapping Vite to configure & launch dapps
- [p5.js & three.js](https://twitter.com/mathcastles/status/1570675435285151744) deployed on-chain
- [frame.tools](https://twitter.com/zkmcx/status/1569662080592248835?s=20&t=ttGThSGyii5v8BIJRIzVHg): publish web-based on-chain art
- xPARC [circom-batch-ECDSA](https://0xparc.org/blog/batch-ecdsa): proof of concept on top of circom-ECDSA
- [Circomspect](https://blog.trailofbits.com/2022/09/15/it-pays-to-be-circomspect/): static analysis for zk proofs
- [I am the chad v1](https://mirror.xyz/0xbeans.eth/usaKkq6OYzrxHPFTXXD8Lp1ABBQY-bzX-PsSVYIfMC8): gas optimizor king of the hill competition
- [Paradigm CTF files](https://github.com/paradigmxyz/paradigm-ctf-2022/) released
- Ethernaut [Good Samaritan level](https://twitter.com/openzeppelin/status/1570791532491579398) on custom errors

**Security**

- [Profanity vanity address generator](https://blog.1inch.io/a-vulnerability-disclosed-in-profanity-an-ethereum-vanity-address-tool-68ed7455fc8c) vulnerability, private keys can be recovered, [being actively exploited](https://twitter.com/zachxbt/status/1570927217840132097), transfer all assets to a different wallet
- [PoW fork replay attacks possible via EIP712](https://twitter.com/amxx/status/1570441526857138180) for contracts that cache the domain separator
- NFTX [vulnerability](https://blog.nftx.io/postmortem-nftxmarketplace0xzap-vulnerability/) patched, attacker could transfer NFT from a collection approved by a user
- StarkEx v4.5 [double-spend](https://twitter.com/StarkWareLtd/status/1567888940123983874) from a vault in a frozen system vulnerability disclosed
- Compound [cETH price feed](https://www.comp.xyz/t/ceth-price-feed-incident-post-mortem/3578) post-mortem

**Ecosystem**

- [Justin Drake](https://twitter.com/VitalikButerin/status/1570299062800510976): the Merge reduced worldwide electricity consumption by 0.2%, equivalent of [shrinking the height of the Eiffel tower to a plastic toy](https://carbon-ratings.com/eth-report-2022)
- Superphiz: [how to stake](https://www.reddit.com/r/ethstaker/comments/xacc5i/best_practice_for_staking_on_the_ethereum_beacon/)
- finematics: [implications of The Merge](https://twitter.com/finematics/status/1569756503556476928) \[video\]

**Enterprise**

- [Compound Treasury](https://medium.com/compound-finance/compound-treasury-launches-borrowing-for-institutions-432af2cd7e6b) adds borrowing USDC for institutions

**Application layer**

- Degrees of separation from Vitalik using recursive SNARKs, what’s your [ETHdos number](https://ethdos.xyz/blog)?
- [OpenRarity](https://twitter.com/opensea/status/1570179078485082113): NFT rarity standard
- Jonathan Mann [Merge album](https://twitter.com/songadaymann/status/1568741813829369856)
- [Interep](https://mirror.xyz/privacy-scaling-explorations.eth/w7zCHj0xoxIfhoJIxI-ZeYIXwvNatP1t4w0TsqSIBe4): sybil-resistant reputation onramp API using web2 social history
- [Shell v2](https://shellprotocol.io/posts/launch/) AMM live on Arbitrum, guarded launch
- [Wrappr](https://mirror.xyz/kalico.eth/wi5HevVbRWaUqQURy1dzsPsdVf9_QcwLa9YnGH8kfS8): create legal entities such as an LLC or non-profit (UNA)

* * *

### **Job Listings**

- EF’s Privacy & Scaling Explorations team: [Web3 Engineer](https://jobs.lever.co/ethereumfoundation/ece6534a-b946-4996-b7e7-713bd1ec0353?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Bobhub oracle is seeking [Technical content writer](https://bobhub.gitbook.io/bobhub/)
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)

**Job listings: $600** for four issues (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- White House [framework for development of digital assets](https://www.whitehouse.gov/briefing-room/statements-releases/2022/09/16/fact-sheet-white-house-releases-first-ever-comprehensive-framework-for-responsible-development-of-digital-assets/)
- US [OFAC FAQ on Tornado Cash sanctions](https://twitter.com/jchervinsky/status/1569756313718259712), users can apply to withdraw, dusting victims not prioritized for enforcement & publishing code allowed
- [Blockchain Association](https://twitter.com/kmsmithdc/status/1569367263857512448) forming PAC in US
- [Coinbase](https://twitter.com/brian_armstrong/status/1570133078022160384) adding crypto positions of politicians to app
- [South Korean court issued arrest warrant](https://www.coindesk.com/business/2022/09/14/s-korean-court-issues-arrest-warrant-against-terra-co-founder-do-kwon-report/) for Luna founder Do Kwon

**General**

- [Uber security breached](https://www.bleepingcomputer.com/news/security/uber-hacked-internal-systems-breached-and-vulnerability-reports-stolen/) in alleged social engineering attack
- Another [Apple zero-day](https://www.bleepingcomputer.com/news/security/apple-fixes-eighth-zero-day-used-to-hack-iphones-and-macs-this-year/)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-17-2022](https://weekinethereumnews.com/week-in-ethereum-news-september-17-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Sep 22 – [Gitcoin Grants round 15](https://gitcoin.co/grants/) ends **(support** [**Week in Eth News**](https://gitcoin.co/grants/2785/week-in-ethereum-news)**)**
- Sep 23 - [ETH HCMC](https://2022.ethhcmc.com/) summit (Ho Chi Minh)
- Sep 23-24 - [ETHSantiago](https://ethsantiago.com/)
- Oct 6-8 – [Web3 Lagos](https://event.web3bridge.com/)
- Oct 7-16 – [Devcon week](https://devcon.org/en/devcon-week/) (Bogotá)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- Oct 7-9 – [Infinite hackathon](https://infinite-hackathons.eth.limo/) (Bogotá)
- Oct 11-14 – [Devcon 6](https://devcon.org/) (Bogotá)
- Oct 18-22 – [Eth Medellin](https://www.ethmedellin.co/) (Colombia)
- Oct 26-28 – [Eth Panama](https://twitter.com/EthPanama)
- Oct 28-30 – [ETH Lisbon](https://www.ethlisbon.org/)
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 11-13 – [ETHBrno](https://mirror.xyz/ethbrno.eth/6BH9cUVuD85hy5O0L5cOOOE7niSA9Yo5eWsXVzKOlO4) (Czech Republic)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Nov 25-27 – [ETH Vietnam](https://www.eth-vietnam.com/)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

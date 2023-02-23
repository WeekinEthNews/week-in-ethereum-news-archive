---
title: "Week in Ethereum News <br> September 24, 2022"
date: "2022-09-24"
---

## **Eth News and Links**

**Execution layer**

- [Candidate EIPs](https://ethereum-magicians.org/tag/shanghai-candidate) for the next upgrade (Shanghai)
- Erigon [roadmap](https://erigon.substack.com/p/post-merge-release-of-erigon-dropping): alpha/beta designations dropped
- Besu [v22.7.3](https://github.com/hyperledger/besu/releases/tag/22.7.3): fixes for empty block proposals and improvements for missed attestations
- Erigon [v2022.09.03](https://github.com/ledgerwatch/erigon/releases/tag/v2022.09.03): improves sync stability
- [Verkle transition](https://twitter.com/GiulioRebuffo/status/1571125136060977154) prototyped using Erigon at ETHBerlin
- Microsoft research claims 6x EVM execution speed improvement with [Forerunner](https://twitter.com/yorkerhodes/status/1572753966206943232) speculative transaction execution

**Consensus layer**

- [View-merge](https://ethresear.ch/t/view-merge-as-a-replacement-for-proposer-boost/13739) potential replacement for proposer boost, defend against balancing & ex-ante attacks
- [Censorship resistance list](https://notes.ethereum.org/@fradamt/H1ZqdtrBF) (crList) proposal, builders forced to fully use block space otherwise they must include proposer-selected transactions in the unused space
- Consensus layer [call video](https://www.youtube.com/watch?v=_yogw67HxZY&t=298s). Notes from [Christine Kim](https://twitter.com/christine_dkim/status/1573105520080289792), next CL call November 3
- Lodestar [v1.1.0](https://github.com/ChainSafe/lodestar/releases/tag/v1.1.0): stability improvements and configure proposer metadata per validator
- Nimbus [v22.9.1](https://github.com/status-im/nimbus-eth2/releases/tag/v22.9.1): fixes for several reported issues and minor performance improvements
- Teku [v22.9.1](https://github.com/ConsenSys/teku/releases/tag/22.9.1): performance improvements
- consensus-specs [v1.2.0](https://github.com/ethereum/consensus-specs/releases/tag/v1.2.0): mainnet Bellatrix specs, R&D for withdrawals & EIP4844
- MEV [order flow auction options](https://collective.flashbots.net/t/order-flow-auctions-and-centralisation-ii-order-flow-auctions/284) to address exclusive order flow
- [Superlight client](https://twitter.com/dionyziz/status/1572068211465519108) with logarithmic sync time, assumes connected to one honest full node

**Stakers**

- Somer: reasons some [solo-stakers experienced degraded performance](https://twitter.com/SomerEsat/status/1572518098523271170)
- Ben Edgington: [stakers shouldn’t expect a bail out](https://twitter.com/benjaminion_xyz/status/1572657858038177793) if they outsource block building
- MEV-Boost:
    - Anish’s [dashboard](https://www.mevboost.org/): 24% of blocks built by relays, 83% of relayed blocks via Flashbots
    - [Flashbots relay and builder metrics](https://transparency.flashbots.net/) dashboard
    - [MEV-Boost getPayload bug](https://collective.flashbots.net/t/post-mortem-on-the-mev-boost-getpayload-bug-when-deposits-were-included-fixed-in-mev-boost-v1-3-1-on-friday-16-9/311) when deposits included in the block, 3 slots missed
    - [bloXroute relay outage](https://twitter.com/eyalmarkov/status/1572616363054612486), 88 slots missed, refunding validators
- [Zeromev-Geth](https://twitter.com/pmcgoohancrypto/status/1572587801836916742): orders transactions by receive time, mitigates front running, stakers can choose to back run transactions

**Layer 2**

- [Optimism Quests](https://dev.optimism.io/quests/): incentivizes trying dapps with NFTs
- Vitalik: [kinds of layer 3s that make sense](https://vitalik.ca/general/2022/09/17/layer_3.html)

**EIPs/Standards**

- [EIP5659](https://github.com/ethereum/EIPs/pull/5659/files): Social media URI propagation event
- [EIP5679](https://eips.ethereum.org/EIPS/eip-5679): Token minting and burning
- [EIP5700](https://github.com/ethereum/EIPs/pull/5700/files): Bindable token

* * *

### **This newsletter is made possible thanks to** Starbloom Ventures!

![Starbloom Ventures](https://weekinethereumnews.com/wp-content/uploads/2021/11/Screenshot-from-2021-11-19-15-25-51.png)

Starbloom Ventures is a first round venture fund founded by Evan Van Ness to invest in the future of web3.

We pledge 10% of investing profits to support Ethereum public goods.

* * *

**Stuff for developers**

- [execTransaction](https://twitter.com/w1nt3r_eth/status/1572633281094647809): pattern to allow an NFT contract owner to execute any transaction, don’t use if contract manages user funds/allowances
- [Whitenoise CTF](https://twitter.com/vex_0x/status/1572257586656980992) optimize challenge on Optimism
- [Impersonator](https://twitter.com/apoorvlathey/status/1572344831648886784): adds viewing dapps in iFrame to impersonate an address
- [Embed.Art](https://github.com/wighawag/embed-art#readme): shareable NFT pages for social media, supports SVG
- [Mockthereum](https://github.com/httptoolkit/mockthereum#readme): mock a node or proxy to an actual node
- Zerokit [v0.1](https://github.com/vacp2p/zerokit/releases/tag/v0.1): zk library in Rust, RLN Module, use Rust API or C FFI, beta
- [Isokratia](https://nibnalin.me/dust-nib/isokratia.html): trust minimized governance with off-chain voting using recursive SNARKs, proof of concept

**Security**

- Wintermute (market maker) [$160 million exploit](https://twitter.com/evgenygaevoy/status/1572329148411936770), trading address with leading zeroes compromised, likely linked to Profanity address generator vulnerability
- Arbitrum bridge [uninitialized address vulnerability](https://medium.com/@0xriptide/hackers-in-arbitrums-inbox-ca23272641a2) disclosed, 400 ETH bounty paid, bounty hunter [started learning Solidity 6 months ago](https://twitter.com/0xriptide/status/1572936443751702531)
- OpenZeppelin Contracts [TimelockController misconfigured by multiple projects](https://github.com/OpenZeppelin/openzeppelin-contracts/issues/3720), deployer has admin permissions until revoked
- [dYdX malicious npm packages](https://www.mend.io/resources/blog/popular-cryptocurrency-exchange-dydx-has-had-its-npm-account-hacked/) published

**Ecosystem**

- ETHBerlin [hackathon winners](https://ethberlin.devfolio.co/projects?show_winners=true)
- PSE grants to [integrate Semaphore](https://mirror.xyz/privacy-scaling-explorations.eth/g5WjOtK4R3rYfLKyqpSXsbNBcj36jzsjgnV2KT2rthM) anonymous signaling protocol
- Reminder: [Merge data analysis/visualization](https://esp.ethereum.foundation/merge-data-challenge) blog post challenge, [Twitter space recording](https://twitter.com/dannyryan/status/1572987347716939776) for ideas
- [Create a satellite Devcon watch party](https://forum.devcon.org/t/launching-devcon-satellites/1364), for communities who can’t be in Bogotá

**Application layer**

- [OpenSea adds Arbitrum One NFTs](https://twitter.com/opensea/status/1572638029457788929), creators need to setup royalties
- Coinbase NFT [aggregating listings](https://twitter.com/coinbase_nft/status/1572717888557166592) from OpenSea, LooksRare and Coinbase
- [Sound Protocol](https://sound.mirror.xyz/t7GDH8RF6XbHLwbHb_R6QLnDTaln0KdGhExBgul6OXY): permissionless music NFTs with custom metadata, minting formats & metadata
- [Volmex Implied Volatility Index](https://blog.volmex.finance/introducing-viv/): 30-day expected volatility of BTC & ETH options market
- [YieldSpaceTV](https://medium.com/yield-protocol/yieldspacetv-our-next-generation-amm-is-live-5bb57e5a9754): Yield’s token vaults deploy into Euler for additional LP yield
- Tribe DAO voted to [repay Fuse exploit victims](https://twitter.com/joey__santoro/status/1571898748405714947)
- [GasHawk](https://gashawk.io/): saves money by buffering transactions until gas prices are low, beta

* * *

### **Job Listings**

- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)
- EF’s Privacy & Scaling Explorations team: [Web3 Engineer](https://jobs.lever.co/ethereumfoundation/ece6534a-b946-4996-b7e7-713bd1ec0353?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- [Bobhub](https://bobhub.xyz/) multichain oracle is hiring a [Technical writer](https://bobhub.gitbook.io/bobhub/)!
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)

**Job listings: $600** for four issues (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US CFTC fined bZeroX & founders $250k](https://www.cftc.gov/PressRoom/PressReleases/8590-22) and taking action against bZx/Ooki DAO defined as unincorporated association of [token holders who voted on governance proposals](https://www.cftc.gov/PressRoom/SpeechesTestimony/mersingerstatement092222)
- [US SEC settled with Sparkster (no code platform)](https://www.sec.gov/news/press-release/2022-167) for unregistered sale of securities, $35 million to be paid to harmed investor fund; [case against influencer Ian Balina](https://twitter.com/TuurDemeester/status/1572046089888333826) claimed jurisdiction for transactions partly due to cluster of Ethereum nodes in US
- [US Treasury digital assets RFC](https://public-inspection.federalregister.gov/2022-20279.pdf) \[PDF\] on responsible development
- Vitalik: [importance of decentralization for DAOs](https://vitalik.eth.limo/general/2022/09/20/daos.html), making better decisions in concave environments, censorship resistance and credible fairness
- [GitHub re-published as read-only](https://github.com/tornadocash) the Tornado Cash repo and its contributor’s accounts

**General**

- OxPARC: [recursive zkSNARKs](https://0xparc.org/blog/groth16-recursion) implemented in Circom/groth16
- [Zero knowledge proofs](https://eprint.iacr.org/2022/1223) of software vulnerabilities
- [US military bought access to internet monitoring tool Augury](https://www.vice.com/en/article/y3pnkw/us-military-bought-mass-monitoring-augury-team-cymru-browsing-email-data), includes email data, browsing history and cookies
- [Browser enhanced spellcheck](https://www.bleepingcomputer.com/news/security/google-microsoft-can-get-your-passwords-via-web-browsers-spellcheck/) sends passwords to Google/Microsoft
- Python [tarfile path traversal 15 year old bug](https://www.bleepingcomputer.com/news/security/unpatched-15-year-old-python-bug-allows-code-execution-in-350k-projects/) allows overwriting arbitrary files

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-24-2022](https://weekinethereumnews.com/week-in-ethereum-news-september-24-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Oct 6-8 – [Web3 Lagos](https://event.web3bridge.com/)
- Oct 7-16 – [Devcon week](https://devcon.org/en/devcon-week/) (Bogotá)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- Oct 7-9 – [Infinite hackathon](https://infinite-hackathons.eth.limo/) (Bogotá)
- Oct 11-14 – [Devcon 6](https://devcon.org/) (Bogotá)
- **Oct 14 –** [**Semaphore grants**](https://esp.ethereum.foundation/semaphore-grants) **deadline**
- Oct 18-23 – [Eth Medellin](https://www.ethmedellin.co/) (Colombia)
- Oct 26-28 – [Eth Panama](https://twitter.com/EthPanama)
- Oct 28-30 – [ETH Lisbon](https://www.ethlisbon.org/)
- **Oct 31 –** [**Merge data challenge**](https://esp.ethereum.foundation/merge-data-challenge) **deadline**
- **Nov 3 – US Treasury** [**digital assets RFC**](https://public-inspection.federalregister.gov/2022-20279.pdf) **\[PDF\] deadline**
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 11-13 – [ETHBrno](https://mirror.xyz/ethbrno.eth/6BH9cUVuD85hy5O0L5cOOOE7niSA9Yo5eWsXVzKOlO4) (Czech Republic)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Nov 25-27 – [ETH Vietnam](https://www.eth-vietnam.com/)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

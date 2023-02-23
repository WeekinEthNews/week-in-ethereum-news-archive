---
title: "Week in Ethereum News <br> January 8, 2022"
date: "2022-01-08"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest core devs call [video](https://www.youtube.com/watch?v=wCSNMSyJV7Y&t=653s). Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1479481915325440008):
    - [Kintsugi testnet split](https://twitter.com/vdWijden/status/1479414817551261699) due to some clients accepting an invalid block created by fuzz testing
    - EIP1153 (transient storage opcodes) discussion, useful in next version of Uniswap, shout if your app would benefit from this
    - Prioritizing Shanghai upgrade EIPs: withdrawals and some EIPs from backlog, new EIPs need strong rationale to prioritize over backlog
    - [Suggest names](https://ethereum-magicians.org/t/el-merge-client-release-naming/7928) for PoW switch off execution layer upgrade \[e.g. Paris\]
- Geth [v1.10.15](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.15): bug fixes, peer-to-peer eth connections could lock up
- Besu [v21.10.6](https://github.com/hyperledger/besu/releases/tag/21.10.6): update for log4j
- Some exchanges still [haven’t implemented EIP1559](https://twitter.com/0xtrent/status/1476666765111439362) type 2 transactions
- Vitalik’s [multidimensional EIP1559](https://ethresear.ch/t/multidimensional-eip-1559/11651) proposal, create burst limits for each resource starting with EVM execution, transaction calldata, witness data and storage size growth 

**EIPs/Standards**

- [EIP4635](https://github.com/ethereum/EIPs/blob/5b577fee69e4766f028985401e4c1dbf44d97016/EIPS/eip-4635.md): Semi-fungible token standard
- [EIP4626](https://github.com/ethereum/EIPs/blob/295f44225b04050d33e49c8af38cc8055f9375a0/eip-4626.md): Yield bearing vault standard
- [EIP4393](https://eips.ethereum.org/EIPS/eip-4393): Micropayments Standard for NFTs and Multi Tokens

**Proof of Stake consensus layer**

- Stakers should [prepare to run an execution client](https://www.reddit.com/r/ethstaker/comments/rvxdue/stakers_get_ready_to_run_your_own_execution_client/) ready for PoW switch off
- Teku [v22.1.0](https://github.com/ConsenSys/teku/releases/tag/22.1.0): update for log4j, adds Kintsugi network definition
- Lodestar [v0.33.0](https://github.com/ChainSafe/lodestar/releases/tag/v0.33.0): libp2p updates, discv5 to v0.6.6, upgrade to node v16, validator metrics, enable light client to sync to head, Kintsugi updates
- Ben Edgington’s Upgrading Ethereum book [chapter on incentives](https://upgrading-ethereum.info/altair/part2/incentives)

**Layer2**

- [31.7 billion gas spent](https://twitter.com/PaoloRebuffo/status/1476935896553377792) in December to settle Layer 2 transactions on mainnet
- Fuel v2 [Sway](https://twitter.com/fuellabs_/status/1478049212357087232) language, inspired by Rust, repos public for local development
- StarkNet Alpha [transaction fee formula](https://community.starknet.io/t/fees-in-starknet-alpha/286)
- [Polygon Miden VM](https://twitter.com/0xpolygonmiden/status/1478783518800953347) will support unsigned 32-bit integers
- [Formal Lean specification of Yul IR semantics](https://medium.com/nethermind-eth/securing-warp-a-formal-specification-of-the-yul-ir-85bb3bf51c62) for StarkNet Warp transpiler
- [Phonon alpha](https://blog.phonon.network/phonon-alpha-getting-started-f85e107de390) (peer to peer private transfers using hardware enforced security): tools to provision & operate an applet on a smart card

* * *

### **This newsletter is made possible thanks to [Celer](https://www.celer.network/)!**

![Celer](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

Celer Network is a layer-2 scaling platform that brings fast, secure and low-cost blockchain applications.

[cBridge](https://cbridge.celer.network/) is at the $2,000,000,000 mark in volume moving ETH, USDT, and USDC between Ethereum mainnet, Optimism, Arbitrum, Avalanche, Boba, Fantom, BSC and Polygon.

We have the **most chains** and the **most tokens** available to bridge!  [Swap instantly between chains](https://cbridge.celer.network/) - sometimes it is even cheaper than using the native bridge.

Our [liquidity mining is live](https://blog.celer.network/2021/12/10/cbridge-liquidity-mining-session-one-is-launching-on-12-15-2021/) for $ETH, $USDT and $USDC, with rewards paid in $CELR

* * *

**Stuff for developers**

- Solmate [v6](https://twitter.com/transmissions11/status/1477428780045987840) (Solidity library): ERC721 & ERC1155 implementations, fast sqrt, fpow & fdiv, MultiRolesAuthority; audited, AGPL v3 license
- ethers.js [v5.5.3](https://github.com/ethers-io/ethers.js/releases/tag/v5.5.3): adds Kintsugi network and avatar fixes 
- Foundry [cast wallet](https://twitter.com/gakonst/status/1477022693639794698): create new wallet, get address, sign message and verify digital signature
- [wagmi](https://github.com/tmm/wagmi): React Hooks library for working with wallets, ENS, contracts, transactions & signing; MIT License
- web3modal [v1.9.5](https://github.com/Web3Modal/web3modal/releases/tag/1.9.5): Coinbase Wallet support, new injected providers
- solidity-shell [v0.0.10](https://github.com/tintinweb/solidity-shell/releases/tag/v0.0.10): Solidity v0.8.11, basic auto-complete
- hardhat-etherscan [v3.0.0](https://github.com/nomiclabs/hardhat/releases/tag/%40nomiclabs/hardhat-etherscan%403.0.0): supports multiple API keys 
- [lil-web3](https://github.com/m1guelpf/lil-web3): simplified versions of web3 protocols to understand how they work; ENS, OpenSea, Fractional, Juicebox, flash loan and multi-sig
- Why you should use [NatSpec](https://twitter.com/clemlak/status/1478850375419531265) comments with Solidity contracts
- Austin Griffith’s [challenges for web2 devs](https://twitter.com/austingriffith/status/1478760479275175940)
- [FaucETH](https://fauceth.komputing.org/): testnet faucet for Goerli, Rinkeby, Kovan, Kintsugi, Arbitrum Rinkeby and Optimism Kovan
- [cairostarter](https://github.com/a5f9t4/cairostarter): minimal template for StarkNet projects; AGPL v3 license
- [hashtree](https://github.com/prysmaticlabs/hashtree): SHA256 library optimized for Merkle tree computations
- [SuperStruct](https://twitter.com/sproulm_/status/1477505725454635009): Rust library for versioned data

**Security**

- Notional [vulnerability disclosure](https://blog.notional.finance/critical-bug-payout-report/), attacker could borrow without sufficient capital, feature disabled, no funds lost, $1 million bounty paid + 100k NOTE
- Illuvium [vulnerability in staking contracts](https://twitter.com/illuviumio/status/1478191824556621825), minting paused, no funds lost
- YEAR airdrop token 30ETH [rugpull](https://twitter.com/cat5749/status/1476813266462539779), transfers prevented by changing ownership, pool drained
- [SAILFISH](https://arxiv.org/abs/2104.08638) system to find state inconsistency bugs, paper evaluates detection of reentrancy and transaction order dependence in contracts
- Austin Williams’ [pro bono security spot checks](https://github.com/Austin-Williams/pro-bono-spot-checks/) for interesting/important projects

**Ecosystem**

- Ethereum Foundation research team [AMA](https://www.reddit.com/r/ethereum/comments/rwojtk/ama_we_are_the_efs_research_team_pt_7_07_january/) on Reddit, Vitalik’s argument why [future will be multi-chain not cross-chain](https://www.reddit.com/r/ethereum/comments/rwojtk/ama_we_are_the_efs_research_team_pt_7_07_january/hrngyk8/)
- [NFT creators](https://twitter.com/0xstark/status/1479478884072505346) earned estimated $3.5 billion last year
- Proposal for [Protocol Guild](https://stateful.mirror.xyz/mEDvFXGCKdDhR-N320KRtsq60Y2OPk8rHcHBCFVryXY), split contract for core contributors to receive donated tokens over a vesting period for recruitment, retention and reward
- Etherscan adds [NFT tracker](https://twitter.com/etherscan/status/1477986601976283141) and [ERC20 DEX tracker](https://twitter.com/etherscan/status/1476871182850818050)
- [OpenSea sell offers](https://twitter.com/nanexcool/status/1478523957485752320) without expiry, still valid after NFT moved back to wallet

**Enterprise**

- [Samsung’s 2022 TVs](https://news.samsung.com/global/samsung-electronics-unveils-its-2022-micro-led-neo-qled-and-lifestyle-tvs-with-next-generation-picture-quality-and-range-of-cutting-edge-personalization-options) to include NFT platform
- [Skiff](https://www.skiff.org/updates/skiff-ens) decentralized document collaboration adds ENS support for onboarding and sharing

**Application layer**

- [Aave Arc](https://twitter.com/StaniKulechov/status/1478755251905835012) permissioned market launched with 30 institutions onboarded
- [ParaSwap](https://twitter.com/paraswap/status/1476980051690274826) Safety Module live, forked from Aave’s Safety Module
- NFT announcements: Ozzy Osbourne’s [CryptoBatz](https://twitter.com/OzzyOsbourne/status/1478112053223067648), Australian Open [tennis balls](https://twitter.com/AOmetaverse/status/1478952680609366016) and [Lamborghini](https://twitter.com/Lamborghini/status/1478410904836272131)
- [Meebits API](https://github.com/larvalabs/meebitsapi): access model files for Metaverse projects
- [Free NFTs](https://twitter.com/steviepxyz/status/1477348060925763588): set of interrelated NFTs claimable for gas fee; CC0
- [Clock8008](https://www.clock8008.com/): on-chain SVG clock NFTs

* * *

### **Job Listings**

- [Textile](https://textile.io/) is hiring! [Blockchain Eng](https://grnh.se/f093ec154us), [Backend Eng](https://grnh.se/526aef8d4us), and [Partner Manager](https://grnh.se/06c1dfdf4us)
- Certora seeks [SR SW Eng](https://www.certora.com/#careers), [Security Res](https://www.certora.com/#careers), [Security Eng](https://www.certora.com/#careers) & [Community Manager](https://www.certora.com/#careers)
- The VAC team at Status.im are looking for a [blockchain engineer](https://jobs.status.im/?gh_jid=3706505)
- Kwenta seeks [Frontend Engineer](https://blog.kwenta.io/kwenta-open-position-front-end-developer/), [Solidity Engineer](https://blog.kwenta.io/kwenta-open-position-solidity-engineer/) & [Marketing Lead](https://blog.kwenta.io/kwenta-open-position-marketing-manager/)
- Are you a p2p networking whiz? EF research hiring [Networking Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=54&source=weekinethnews)
- Geth team is looking for a [Senior Technical Writer](https://ethereum.bamboohr.com/jobs/view.php?id=51&source=weekinethnews)

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US CFTC fines event market Polymarket](https://www.cftc.gov/PressRoom/PressReleases/8478-22) (Polygon) $1.4 million with order to wind down non-compliant markets
- US IRS requires third-party settlement orgs such as [PayPal and Venmo](https://newsroom.paypal-corp.com/2021-11-04-New-US-Tax-Reporting-Requirements-Your-Questions-Answered) to report goods & services transactions for annual gross sales over $600
- [Fred Wilson](https://avc.com/2022/01/what-is-going-to-happen-in-2022/): ETH market cap will surpass BTC, due to PoW switch off and that productive assets must be worth more than non-productive assets

**General**

- Vitalik’s [reflections on a decade of posts](https://twitter.com/vitalikbuterin/status/1477402749994156036)
- [AMM mathematics](https://idcap.docdroid.com/D9JoW7H/202201-amm-paper-draft-pdf) deep dive \[PDF\]
- [Crypto crime](https://blog.chainalysis.com/reports/2022-crypto-crime-report-introduction/) increased but at all time low in share of all crypto activity
- [Don’t screen share Discord!](https://twitter.com/littlelemonsnft/status/1477923368053706755)  Scammers attempting to obtain your Discord access token
- [Mozilla](https://twitter.com/mozilla/status/1479143340159422468) pauses accepting crypto donations after anti-crypto backlash

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-january-8-2022](https://weekinethereumnews.com/week-in-ethereum-news-january-8-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Jan 13 – [MEV in 2021](https://github.com/flashbots/mev-research/issues/68) (virtual)
- Jan 14-16 – ETHGlobal’s [NFTHack](https://nft.ethglobal.com/) (virtual)
- Feb 15 - Apr 5 – [Cryptocurrency Class](https://mirror.xyz/0xaFaBa30769374EA0F971300dE79c62Bf94B464d5/oGqGP2NOK9g7QPl1sMKkzql_Fh0P6hKbpYLZ-EkQTXU) (virtual) 
- Feb 17 – [Schelling Point](https://schellingpoint.gitcoin.co/) (Denver) 
- Feb 18-20 – [ETHDenver](https://www.ethdenver.com/)
- Mar 14-17 – [Eth Rio](https://www.ethrio.org/)
- **Mar 17 – [ETH Austin](https://2022.ethaustin.org/) summit**
- Mar 29-31 – [ETHDubai](https://www.ethdubaiconf.org/)
- **Apr 7-9 – [ETH Portland](https://2022.ethportland.com/) hackathon** 
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- May 3-8 – [spaghettETH](http://spaghett-eth.com/) (Milan)
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- **Jun 16-19 – [ETH Miami](https://2022.eth-miami.com/) summit & hackathon**
- **Jun 21-23 – [NFT.NYC](https://www.nft.nyc/)**
- Jun 24-26  – [ETHNewYork](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- **Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit**
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- **Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)**
- **Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)**
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

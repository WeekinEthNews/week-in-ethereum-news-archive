---
title: "Week in Ethereum News <br> May 7, 2022"
date: "2022-05-07"
---

## **Eth News and Links**

**PoW switch off (the Merge)**

- Tim Beiko’s [core devs update](https://tim.mirror.xyz/PWFVaHY3Mrx7srarMmuBWya0J5kioR1l2xaH3p5APDk) on final tasks before the Merge:
    - a few mainnet shadow forks without issues 
    - clients passing test suites 
    - smooth upgrades on public testnets
- [Mainnet shadow fork 3](https://twitter.com/vdWijden/status/1522208324661374977) had no major issues
- [Mainnet shadow fork 4](https://twitter.com/abcoathup/status/1522678129063788544) planned for May 12
- [Resource list](https://notes.ethereum.org/@MarioHavel/merge-resources) for the Merge
- Merge testing [leaderboard](https://testingthemerge.notion.site/Testing-the-Merge-d0af826782a34d5ca6ce31aa5e631645)

**Mainnet execution layer**

- [Difficulty bomb](https://ethresear.ch/t/blocks-per-week-as-an-indicator-of-the-difficulty-bomb/12120/17) starting to show
- Erigon [v2020.05.02-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.05.02): improve snapshot download speed, reduce database size by ~120Gb after initial sync
- Nethermind [v1.12.8](https://github.com/NethermindEth/nethermind/releases/tag/1.12.8): reduce CPU usage & sync time when syncing receipts and optimize transaction execution
- Besu [v22.4.0](https://github.com/hyperledger/besu/releases/tag/22.4.0): snapsync fix
- [EIP4444](https://notes.ethereum.org/@ralexstokes/BJWd8saB9) (limit historical data) next steps: continue work on prototype, demo post-merge

**Proof of Stake consensus layer**

- PoS implementers [call video](https://www.youtube.com/watch?v=nnjeqZK7jgU&t=52s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/Hy_VXLb8q) & [Christine Kim](https://twitter.com/christine_dkim/status/1522256793321103360):
    - mainnet shadow fork 3 bug free, with a mere config issue
    - testnet beacon chains to be spun up for Ropsten (permissionless) & Sepolia (permissioned) before end of May to test the Merge
    - IPv6 discussion
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220506)
- Lodestar [v0.35.0](https://blog.chainsafe.io/lodestar-v0-35-0-upgrade-release-d8b636f15091): support consensus-spec v1.1.10 and keymanager API
- Prysm [v2.1.1](https://github.com/prysmaticlabs/prysm/releases/tag/v2.1.1): fixes for regressions found in previous version

**EIPs/Standards**

- Discussion on [splitting ERCs from EIPs](https://twitter.com/TimBeiko/status/1521993235597434880)
- [EIP5075](https://github.com/ethereum/EIPs/pull/5075/files): rateLimit - An outflow limiter for assets
- [EIP5069](https://github.com/ethereum/EIPs/pull/5069/files): EIP editor apprentice handbook 
- [EIP5065](https://github.com/ethereum/EIPs/pull/5065/files): Instruction for transferring ether
- [EIP5058](https://github.com/ethereum/EIPs/pull/5058/files): Lockable ERC721
- [EIP5050](https://github.com/ethereum/EIPs/pull/5050/files): Token interaction

**Layer2**

- [Raiden](https://medium.com/raiden-network/the-raiden-network-now-live-on-arbitrum-3d57fedf7961) live on Arbitrum
- Optimistic rollup [price differences](https://twitter.com/bkiepuszewski/status/1522152595086839808) due to data compression
- Kelvin: potential future [hybrid ZK/Optimistic rollup](https://kelvinfichter.com/pages/thoughts/hybrid-rollups/)
- Polynya: [disaggregated blockchain layers](https://mirror.xyz/polynya.eth/C7pabfX3j8r65w8SWlpT_dem1_JXvQxsQao4V0xjsNY)

* * *

### **This newsletter is made possible thanks to Starbloom Ventures!**

![Starbloom Ventures](https://weekinethereumnews.com/wp-content/uploads/2021/11/Screenshot-from-2021-11-19-15-25-51.png)

[](https://substackcdn.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fa135f262-9467-410d-9db4-b09a0e05c3e5_613x313.png)

Starbloom Ventures is a **first round** venture fund founded by [Evan Van Ness](https://twitter.com/evan_van_ness) to invest in the future of web3. 

What’s missing in DAOs?  Informed delegates.  Why not integrate [Karma's credit scores](https://mirror.xyz/showkarma.eth/xMvT3xIzSAVikzruGXgMvjmADUgeG1EU9Sozhnu1nIs) to help your token holders make better choices on who to delegate to.

* * *

**Stuff for developers**

- Foundry [Anvil](https://twitter.com/gakonst/status/1522282339073597440): local testnet node, written in Rust, drop-in replacement for ganache-cli or hardhat node
- Foundry [shorthand](https://github.com/foundry-rs/foundry/pull/1402#issuecomment-1112095141) for cast and forge commands
- MockProvider [v2](https://twitter.com/cleanunicorn/status/1521776667391234048): updated Solidity mocking library, supports Foundry
- [API3 QRNG](https://medium.com/api3/api3-qrng-web3-quantum-random-numbers-4ca7517fc5bc): quantum random number oracle on mainnet, Arbitrum & Optimism
- [Using EIP2535 (Diamonds)](https://medium.com/@bearded.eth/diamonds-are-a-proxys-best-friends-c302cca82203) with an upgradeable proxy
- [Twitter profile pic support for on-chain SVG NFTs](https://twitter.com/w1nt3r_eth/status/1522240710870663168) using accessories
- [MATT auction](https://twitter.com/danfinlay/status/1520590950916968448): variable-edition NFT auction, uses one transaction; draft
- ETK (EVM bytecode assembler & disassembler) [v0.2.1](https://github.com/quilt/etk/releases/tag/v0.2.1): user defined macros, function selector database
- Web3.py [v5.29.0](https://snakecharmers.ethereum.org/web3-py-patterns-external-modules/): external module support
- [MEV Inspect](https://github.com/Destiner/mev-inspect-js#readme): JavaScript port of mev-inspect-py
- [RainbowKit](https://twitter.com/rainbowdotme/status/1522276598925467649): wallet connection/management library, uses wagmi React hooks
- [Hardhat-deploy](https://github.com/wighawag/hardhat-deploy/pull/276): zkSync deployment support
- OpenZeppelin [Defender](https://forum.openzeppelin.com/t/defender-release-optimism-frame-improved-forta-sentinels-and-full-relayer-crud-api/28293): Optimism support, API to create & manage Relayers and Frame wallet support
- OpenSea [Stream API](https://nft.mirror.xyz/HhXSvsS7ZhVns6FuJB1rUGP53gW-qDVCv5gfx9cDGco): receive marketplace events via websockets; beta

**Security**

- Rari’s Fuse pools [$80 million exploit](https://rekt.news/fei-rari-rekt/) on mainnet & Arbitrum due to missing reentrancy check in exitMarket function
- Saddle Finance [$10.2 million exploit](https://blog.saddle.finance/4-30-2022-post-mortem-of-mainnet-susdv2-metapool-exploit/) due to old version of library, $3.97 million rescued by BlockSec
- NEAR Rainbow bridge unsuccessfully [attacked](https://twitter.com/alexauroradev/status/1520810591803293696), watchdog detected attack & created a challenge transaction
- Aave v3 price oracle manipulation [vulnerability](https://medium.com/@hacxyk/aave-v3s-price-oracle-manipulation-vulnerability-168e44e9e374), fallback oracle missing access controls for set asset price, $2.9 billion across Layer 2s was at risk
- [Multi-block MEV](https://twitter.com/MTorgin/status/1521433474820890624): potential for TWAP oracle manipulation post-Merge

**Ecosystem**

- Tim Beiko’s [Ethereum sustainability todos](https://twitter.com/TimBeiko/status/1520893784556335105): data availability layer for rollups, Proposer/Builder separation and stateless
- CoinDesk: [EIP & ERC explainer](https://www.coindesk.com/learn/what-are-eip-and-erc-and-how-are-they-connected/)
- Etherscan adds account [transaction heatmap](https://twitter.com/etherscan/status/1521813183346151424)
- [MEV Supply Chain](https://flashbots.mirror.xyz/bqCakwfQZkMsq63b50vib-nibo5eKai0QuK7m-Dsxpo): avoid centralized block building

**Application layer**

- Yuga Labs [Otherdeed mint](https://thedefiant.io/yuga-labs-otherside-land-sale-gas-fees/): 55k ETH burnt, gas fees spiked over 5k gwei
- Hop [DAO](https://hop.mirror.xyz/AI5fOUR0X_l0mktShDOx3mwr-hsB24gp8GvTWtS-MBc): governance token airdrop, 25% bounty for Sybil reports, Sybil attackers encouraged to self report
- [Uniswap v3 liquidity for ETH/USD](https://uniswap.org/blog/uniswap-v3-dominance) deeper than centralized exchanges
- [Kwenta](https://mirror.xyz/kwenta.eth/YYQBLaTbk00S8EDCnzMCzBDQjRAmRnnG_XISz6Oo03M) next price orders live (executes order at the next price update)
- [ENS](https://twitter.com/ensdomains/status/1520871974326931456) one million names created

* * *

### **Job Listings**

- Status are hiring [engineers who focus on incentive design](https://jobs.status.im/?gh_jid=3706505)
- Vac @ status are looking for [protocol engineers](https://jobs.status.im/?gh_jid=3693623) 
- Ethereum Foundation need a [People Operations Lead](https://jobs.lever.co/ethereumfoundation/8046bbe5-6343-4ecf-8296-37dc2a5bf915?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Status Waku is hiring: [TypeScript Protocol/Software Engineer & DevRel](https://jobs.status.im/?gh_jid=4143735&gh_src=55c532491us)
- EF’s Privacy & Scaling Explorations team: [Web3 Engineer](https://jobs.lever.co/ethereumfoundation/ece6534a-b946-4996-b7e7-713bd1ec0353?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- EF Ecosystem Support team: [Communications](https://jobs.lever.co/ethereumfoundation/4b0c3305-cf03-4e33-9bfb-63e4ec6f3a68?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum), [Analyst](https://jobs.lever.co/ethereumfoundation/64361391-9a74-49ed-b37c-8ff35931430e?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) & [Admin Assistant](https://jobs.lever.co/ethereumfoundation/5684f7ea-c3ad-4703-b86c-462964f49392?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Trail of Bits [Security Apprenticeship](https://jobs.lever.co/trailofbits/b2d6ce87-6b01-462f-965a-597a273ce26f) (3 months)

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US SEC](https://www.sec.gov/news/press-release/2022-78) doubles the headcount of crypto enforcement unit
- [BitMEX co-founders to pay $10 million each](https://www.cftc.gov/PressRoom/PressReleases/8522-22) to settle US CFTC civil case
- Yuga Labs [Otherside licenses](https://twitter.com/punk6529/status/1520697321167728641): no commercial rights in Otherdeeds, restricted rights in Kodas which are revocable
- Guide to [land value tax](https://www.gamedeveloper.com/design/land-value-tax-in-online-games-and-virtual-worlds-a-how-to-guide) for virtual worlds & games to avoid speculators
- Simon de la Rouviere: [Time-As-Platform](https://blog.simondlr.com/posts/time-as-platform)
- Crypto network effects: [Sarnoff’s Law and Metcalfe’s Law](https://dataalways.substack.com/p/decoding-cryptoasset-network-effects)

**General**

- [Yao's Garbled Circuits](https://cronokirby.com/posts/2022/05/explaining-yaos-garbled-circuits/) explainer
- Remco: [BLS Signatures](https://xn--2-umb.com/22/bls-signatures/index.html)
- 0xPARC: [zk-ECDSA](https://0xparc.org/blog/zk-ecdsa-2) implementation details

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-may-7-2022](https://weekinethereumnews.com/week-in-ethereum-news-may-7-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in_ **_bold_**_)_**:**

- May 8 – deadline for [EF academic grants round](https://esp.ethereum.foundation/academic-grants)
- May 17-20 – [EY Global blockchain summit](https://pub.ey.com/public/2021/2112/2112-3933703/blockchain-summit-2022/index.html)
- May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline
- Jun 10 – [Austin DeFi](https://2022.austindefi.org/) summit
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETH NYC](https://nyc.ethglobal.co/)
- Jul 6-8 – [ETHBarcelona](https://twitter.com/eth_barcelona/status/1516773782538448896)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 5-7 – [ETH Seoul](https://2022.ethseoul.org/)
- **Aug 18-19 –** [**Ethereum SP**](https://twitter.com/EthereumRio/status/1520490449009528832) **(São Paulo)**
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 28 – [DeFi San Francisco](https://2022.defi-sf.com/) summit
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev) (hackathon & conference)
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** [_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive it weekly_**

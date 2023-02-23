---
title: "Week in Ethereum News <BR> July 31, 2021"
date: "2021-07-31"
---

## **Eth News and Links**

**Mainnet execution layer**

- Tim Beiko’s All Core Devs [update](https://hackmd.io/@timbeiko/acd/https%3A%2F%2Fhackmd.io%2F%40timbeiko%2Facd-update-005): update nodes for London, upgrade viewing parties, EIP3675 changes and PoW switch off road map
- [JSON RPC changes for EIP1559](https://hackmd.io/@timbeiko/1559-json-rpc): adds 0x02 transaction type and baseFeePerGas block header field
- Erigon [2021.07.05-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2021.07.05): Docker builds follow XDG spec
- Geth workshop [videos](https://www.youtube.com/playlist?list=PLX_rXoLYCf5GZZK8jF0RDqaNLzU04UbrW)
- [SHA256 optimization](https://hackmd.io/@potuz/rJX9iD30u) for Merkle Roots: ~30% speed up of hashing
- [Erigon on Raspberry Pi 4](https://twitter.com/EthereumOnARM/status/1419560397686951936): full validation node on <$250 hardware

**EIPs/Standards**

- [EIP3675](https://eips.ethereum.org/EIPS/eip-3675): Upgrade consensus to Proof-of-Stake
- [EIP3668](https://eips.ethereum.org/EIPS/eip-3668): Durin: Secure off chain data retrieval

**Proof of stake consensus layer**

- [Lodestar](https://twitter.com/gregthegreek/status/1420758664491720704) validating on mainnet, beacon chain now has 5 mainnet clients
- Danny Ryan’s [Finalized PoS update](https://blog.ethereum.org/2021/07/26/finalized-no-27/): mainnet validators must upgrade their execution clients
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210730)
- PoS implementers call (video not uploaded). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/SyZgz4l1Y)
- Teku [v21.7.0](https://github.com/ConsenSys/teku/releases/tag/21.7.0): optional upgrade, subcommand added to migrate to leveldb without a full resync and fixed file handle leak
- [Lido](https://blog.lido.fi/the-road-to-trustless-ethereum-staking/) staking pool roadmap to trustless staking
- [Measuring staking decentralization](https://shsr2001.github.io/beacondigest/notebooks/2021/07/19/measuring_decentralization.html): 31 parties would need to collude to control 51% of the beacon chain, 8 parties to collude to control 33%
- Proof of concept QT-based block/node [explorer](https://twitter.com/jcksie/status/1419385125540933637)
- [Attacking Gasper](https://ethresear.ch/t/attacking-gasper-without-adversarial-network-delay/10187) without adversarial network delay

**Layer2**

- Synthetix [synth exchanges live on Optimism](https://blog.synthetix.io/synth-exchanges-are-live-on-l2/) using Kwenta [alpha](https://blog.kwenta.io/everything-you-need-to-know-about-using-kwenta-on-l2/)
- [Tenderly adds](https://blog.tenderly.co/optimistic-ethereum-integration-now-available-on-tenderly/) Optimism support
- [Sorare](https://medium.com/sorare/were-live-on-our-scaling-solution-starkware-62438abee9a8) migrated to Starkware for scaling
- StarkEx [v3.0](https://medium.com/starkware/starkex-3-0-now-live-on-mainnet-57174a5f8beb): Layer1 vaults for DeFi pooling & decentralized AMM, single STARK proof for multiple independent dApps

* * *

### **This newsletter is made possible thanks to [Nexus Mutual](https://nexusmutual.io/)!**

![Nexus Mutual](https://weekinethereumnews.com/wp-content/uploads/2021/07/Screenshot-from-2021-07-30-18-52-32.png)

Nexus Mutual’s [Yield Token Coverage](https://medium.com/nexus-mutual/yield-token-cover-nexus-mutuals-defi-protection-for-money-legos-6a92dd8162fd) is now live! 

[Members](https://app.nexusmutual.io/home) can get comprehensive full stack DeFi coverage against smart contract hacks, oracle attacks and even stablecoin depegs, all included in one product. Specifically designed for vault products like Yearn and Idle, all of the underlying risks are covered, regardless of how many strategies the vault uses. 

If you’re looking for protected yield, [Nexus Mutual](https://nexusmutual.io/) has you covered.

* * *

**Stuff for developers**

- Ethers.js [playground](https://playground.ethers.org/)
- Remix IDE [v0.15.0](https://medium.com/remix-ide/remix-ide-v0-15-0-is-released-219845ae51ca): Slither integration, URLs for opening files and Gists in Remix
- web3.js [v1.5.0](https://github.com/ChainSafe/web3.js/releases/tag/v1.5.0): EIP1559 support and documentation updates
- Nethereum (.Net library) [v4.0.0](https://github.com/Nethereum/Nethereum/releases/tag/4.0.0): EIP1559 support
- Fe [v0.7.0-alpha](https://github.com/ethereum/fe/releases/tag/v0.7.0-alpha): runtime checks, custom revert errors, bytes type removed and multi line string support
- MyCrypto’s TypeScript strategy for [EIP1559 fee estimation](https://github.com/MyCryptoHQ/MyCrypto/blob/fb/eip-1559/src/services/ApiService/Gas/eip1559.ts)
- [EthTx](https://ethtx.info/): transaction decoder website and open source Python library
- [Smart-contract-inspector](https://github.com/tintinweb/smart-contract-inspector): state variable viewing library and demo website
- Using [delegatecall](https://eip2535diamonds.substack.com/p/understanding-delegatecall-and-how) safely
- [Contract creation in bytecode](https://monokh.com/posts/ethereum-contract-creation-bytecode) explainer
- [Engineering lessons](https://optimismpbc.medium.com/the-highly-optimistic-dev-blog-01-the-mystery-of-the-missing-message-23b8ce9b9b82) from hunting Optimism L1->L2 deposit bug
- [How to prepare](https://vonnie610.medium.com/how-to-win-an-online-hackathon-and-have-a-good-time-29d50f411e06) to win an online hackathon
- Austin Griffith’s [quick start for developers](https://link.medium.com/PgVAYjBukib) new to Ethereum

**Security**

- [Securing Proof of Personhood services](https://hackmd.io/@RoboTeddy/S1EsAilTO) against puppeteer attack 
- Tincho’s ChainSwap [exploit Proof of Concept](https://github.com/tinchoabbate/chainswap-exploit-poc)
- Sablier [recipient cancellation vulnerability](https://medium.com/sablier/low-severity-recipient-cancellation-bug-post-mortem-f507fea75c95) disclosed
- MyCrypto’s [NFT bugs and exploits](https://blog.mycrypto.com/nft-smart-contract-bugs-exploits/?utm_medium=social&utm_source=reddit&utm_campaign=nft): CryptoPunks v1, Meebits trait minting and MoonCatRescue locked funds 

**Ecosystem**

- Ethereum [launched six years ago](https://twitter.com/LefterisJP/status/1421050318083837956)
- Flashbots bundles were recently included in [⅔ of blocks](https://twitter.com/bertcmiller/status/1421176267051835400)
- [Blockscan](https://twitter.com/etherscan/status/1419985650632122369) by Etherscan: search for an address or transaction hash on mainnet, testnets, layer2 networks and sidechains
- [CryptoFees.info](https://cryptofees.info/) adds protocol grouping to view all their fees
- [Revoke.cash](https://revoke.cash/) adds viewing and revoking of ERC721 allowances

**Enterprise**

- [EY tested TaxGrid](https://www.ey.com/en_lu/news/2021/07/ey-professionals-government-and-industry-representatives-complete-a-blockchain-project-to-tackle-global-tax-challenge) cross-border withholding tax solution, stakeholders included government departments of UK, Netherlands and Norway; uses ZK proofs, ERC20 and ERC721 tokens on a private permissioned network

**Application layer**

- [Thales](https://thalesmarket.medium.com/the-day-has-come-thales-dapp-launches-on-ethereum-mainnet-366b98ed0c71) (Synthetix spin-off) live on mainnet: on-chain binary options
- [Ondo Finance](https://blog.ondo.finance/introducing-ondo-finance-488c6703a9a5): fixed rate managed loans for risk-adjusted exposure to yield, ~$5m capped launch, exercise caution
- [Time-Weighted AMM design](https://www.paradigm.xyz/2021/07/twamm/) for large orders, on-chain equivalent of TWAP order
- [Fractional Art](https://twitter.com/fractional_art/status/1419696688302854146): fractional ownership for high value NFTs using ERC20 tokens
- [Stoner Cats](https://www.stonercats.com/) animated tv series sold ~3k ETH of NFTs with ~1.5k ETH in gas fees; $800k lost on [out of gas errors](https://medium.com/@ilangitter/how-stoner-cats-lost-collectors-800k-in-35-minutes-c23a9072a471) (Disclosure: given a cat for [contract feedback](https://twitter.com/abcoathup/status/1419779607088164873))
- EthBlockArt [minting price discovery mechanism](https://ethblock.art/editorial/price-mechanism-explained)
- [MATT auctions](https://twitter.com/simondlr/status/1417235926820999169) to maximize artist revenue, capped collection size reflects demand and reduces speculation
- JPG: NFT curation protocol live with [Deep Time exhibition](https://jpg.space/gallery/0x08098eb0)
- [Proof of Humanity](https://www.democracy.earth/#/vault/ubi-weth): use yield on ETH to buy and burn UBI tokens

**Regulation/business/tokens**

- [Uniswap.org interface](https://twitter.com/haydenzadams/status/1418961999539712006) removed tokens such as derivatives due to perceived regulatory pressure; Uniswap protocol and alternative interfaces unaffected
- Proposed [US infrastructure bill](https://twitter.com/jchervinsky/status/1421150344051048451) would require KYC for every address
- US Senator Elizabeth Warren said in [committee hearing](https://www.banking.senate.gov/hearings/cryptocurrencies-what-are-they-good-for): “crypto puts the \[financial\] system at the whims of some shadowy faceless group of super coders and miners”
- [DAO Treasury management](https://www.decentralised.co/treasury-management-in-the-age-of-defi/) using options, stablecoins and indices, borrowing against the treasury and range tokens
- Simon de la Rouviere: [NFT economies](https://blog.simondlr.com/posts/exploring-nft-economies), creators vs collectors and collection sizes
- Draft [NFT licences](https://github.com/rariblecom/nft-license), exclusive and non-exclusive variants
- Five [narratives for Ethereum](https://medium.com/electric-capital/from-digital-oil-to-a-digital-nation-narratives-for-ethereum-in-2021-1ae86ad73dae) with valuation models

**General**

- Fortune: [DeFi takes on Wall Street](https://fortune.com/longform/decentralized-finance-crypto-wall-street/); magazine [cover art by pplpleasr](https://twitter.com/tetranode/status/1420972026659889154)
- [Bring Your Own Algorithm](https://twitter.com/ryanberckmans/status/1420858894042255362), choose how you experience the metaverse
- Cloudflare: [AWS’s egregious egress](https://blog.cloudflare.com/aws-egregious-egress/)
- Vitalik: [against overuse of the Gini coefficient](https://vitalik.ca/general/2021/07/29/gini.html) measure of inequality

* * *

## **Job Listings**

- Ethereum Foundation: [Test Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=39) for consensus and execution layers
- [Synthetix](https://twitter.com/kaiynne/status/1415573456146501634): 2 Solidity engineers to work direct with Kain Warwick in Sydney
- Nethermind [internship program](https://www.notion.so/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-july-31-2021/](https://weekinethereumnews.com/week-in-ethereum-news-july-31-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Aug 1 - applications close for [Secureum auditing bootcamp](https://hackmd.io/@secureum/bootcamp-epoch0-announcement)
- Aug 4 (or 5) - [London hard fork](https://blog.ethereum.org/2021/07/15/london-mainnet-announcement/)
- Aug 12 - applications close for [EF small grants for events](https://esp.ethereum.foundation/en/devcon-grants/)
- **Aug 13 - [Sign in with Ethereum RFP](https://notes.ethereum.org/@djrtwo/sign-in-with-ethereum-RFP) extended deadline**
- **Aug 17 - applications close for [written pieces on public goods projects](https://gitcoin.co/blog/seeking-a-new-kind-of-public-good/)**
- Aug 27-29 - [Edcon](https://www.edcon.io/) (Shenzhen/online)
- **Oct 1-3 - [EthAtlanta](https://ethatl.com/) enterprise-focused hackathon & keynotes**
- **Oct 22-24 - [ETH Lisbon](https://ethlisbon.org/)**

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

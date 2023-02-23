---
title: "Week in Ethereum News <BR> August 28, 2021"
date: "2021-08-28"
---

## **Eth News and Links**

**Mainnet execution layer**

- Consensus bug (CVE-2021-39137) [exploited](https://twitter.com/mhswende/status/1431259601530458112) causing a small chain split for those who did not update their Geth nodes as instructed:
    - Most miners had already updated and the incorrect minority chain was short-lived
    - Update now to Geth [v1.10.8](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.8) and Erigon [v2021.08.04](https://github.com/ledgerwatch/erigon/releases/tag/v2021.08.04) (or later)
    - [Exploit explainer](https://twitter.com/kelvinfichter/status/1431336698911338496): pointer to contract's memory was overwritten (pointers are confusing)
    - Impacts Geth based EVM networks (sidechains and Layer2)
- Geth [removing deprecated RPC flags](https://twitter.com/vdWijden/status/1431166626053951492), update command line flags to use http instead
- [100,000 ETH burnt](https://twitter.com/evan_van_ness/status/1430864225178689538) with EIP1559 since London upgrade
- [Execution layer client teams](https://blog.ethereum.org/2021/08/24/building-together/) granted $1.5 million from application layer projects (Compound Grants, Lido, Synthetix, The Graph and Uniswap Grants) and Kraken, in addition to Ethereum Foundation funding

**EIPs/Standards**

- [EIP3772](https://github.com/ethereum/EIPs/blob/e87539550e94ad47315ca2d2227ddf7f10060eb1/EIPS/eip-3772.md): Compressed Integers
- [EIP3770](https://github.com/ethereum/EIPs/blob/2a4baf6cf0958a2fe71cd414c745341fe6f5cc78/EIPS/eip-%23%23%23.md): Chain-specific addresses
- [EIP3756](https://eips.ethereum.org/EIPS/eip-3756): Gas Limit Cap
- [EIP3754](https://github.com/ethereum/EIPs/blob/1206ee802eec3282ca3fe761064a2f2dc1817ac1/EIPS/eip-3754.md): Vanilla Non-Fungible Token Standard
- [EIP3742](https://github.com/ethereum/EIPs/blob/ab637622fce94934a4686d31fb7544501e768564/EIPS/eip-multi_party_contract.md): Multi Party Contract Standard

**Proof of stake consensus layer**

- Stakers: you must update to the latest Geth or Erigon if you run them. Also be prepared for the Altair upgrade coming at the end of September
- Beacon chain minor incident:
    - [Orphaned blocks](https://twitter.com/benjaminion_xyz/status/1429044820383866896) caused small number of dropped attestations, resulting in a 1-2% drop in participation
    - Caused by [Lido](https://blog.lido.fi/lido-20-08-2021-orphaned-blocks-in-ethereum-incident-postmortem/) overreliance on one node serving the queries of 4000 validators
    - Data driven [investigation](https://shsr2001.github.io/beacondigest/notebooks/2021/08/23/beacon_incident.html)
- Danny Ryan’s [Finalized PoS update](https://blog.ethereum.org/2021/08/25/finalized-no-28/): Altair upgrade of Prater testnet on September 2, Beacon chain upgrade targeting end of September
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210827)
- PoS implementers [call](https://www.youtube.com/watch?v=DZiy3RhUgNY&t=35s). Notes from [Alex Stokes](https://twitter.com/ralexstokes/status/1430926107147005952) and [Ben Edgington](https://hackmd.io/@benjaminion/rycc7-HWF)
- Teku [v21.8.2](https://github.com/ConsenSys/teku/releases/tag/21.8.2): Altair upgrade of Prater and reduced CPU and memory usage
- Lighthouse [v1.5.1](https://github.com/sigp/lighthouse/releases/tag/v1.5.1): Altair upgrade of Prater, v1.5.0 improved networking stack and doppelganger protection, downgrade requires resync 
- [Nimbus privacy focus](https://twitter.com/jcksie/status/1430909810669625350?) impacts crawlers as cycles libp2p peerid on restart and doesn’t accept socket connection when peer table is full
- Proposal for committee-driven [MEV smoothing](https://ethresear.ch/t/committee-driven-mev-smoothing/10408) to equally share a block’s MEV among the committee members and the proposer
- Predicted [exit/entry queue clog](https://ethresear.ch/t/exit-entry-queue-clogging-after-withdrawals-are-enabled/10400) once withdrawals enabled due to validators wanting to compound their stake and rotate keys, these use cases should be handled without an exit/entry to avoid clogging
- [Stereum launcher](https://stereum.net/ethereum-node-setup/): beacon chain client installer, supports 4 clients

**Layer2**

- [Optimism](https://optimismpbc.medium.com/arbitrary-token-bridging-d552f6bef694) adds custom ERC20 token deposit and withdrawals
- [Nova](https://twitter.com/transmissions11/status/1431044602287464450): trustless relaying of contract calls between L2 and L1, deployed on Optimism and mainnet, restricted to approved projects for now
- [Hop](https://twitter.com/HopProtocol/status/1430630767042904074) enables fast exits from Optimism to mainnet for USDC and USDT, avoids 7 day optimistic rollup withdrawal time
- [Loopring zkRollup NFTs](https://medium.com/loopring-protocol/loopring-now-supports-nfts-on-l2-29174a343d0d): mint, trade and transfer on L2, deposit to L2, withdraw to L1, supports ERC721 and ERC1155
- L2Beat adds [risk view](https://twitter.com/l2beatcom/status/1431195213113012227): security, data availability, what can be changed and what to do on censorship or system goes offline

* * *

### **This newsletter is made possible thanks to [Streamr](https://streamr.network/)!**

![Streamr](https://weekinethereumnews.com/wp-content/uploads/2021/08/WeekInEth_banner_STREAMR-1024x341.jpg)

The Streamr Network is being built to provide a decentralized real-time messaging protocol for web3. The network is a decentralized, topic-based publish-subscribe system. Each stream or pub-sub topic has its own P2P overlay network that is built and maintained by a set of BitTorrent-like trackers.

Testnets for the current Brubeck milestone of the network are now running. Contribute your idle bandwidth and run a node in the Streamr Network to earn rewards, with 2M DATA tokens up for grabs! DATA is an ERC-20 token, currently trading on most major exchanges, that will power the tokenomics mechanism on the Streamr Network. [Learn how to run a Streamr node here](https://medium.com/streamrblog/how-to-join-the-brubeck-testnet-c8b823c847f8).

For more information about the project, you can talk to the team on the [Streamr Discord server](https://discord.com/invite/xEQWNgYUgA)!

* * *

**Stuff for developers**

- Ganache [v7.0.0 alpha](https://github.com/trufflesuite/ganache/releases/tag/ganache%407.0.0-alpha.0): local blockchain (formerly ganache-cli), significantly faster and more memory efficient, can run in browser
- [Remix tools in VSCode](https://medium.com/remix-ide/remix-in-vscode-compiling-debugging-metamask-remixd-42c4a61817e2): compile, deploy to public chains with MetaMask and debug with Remix's Debugger
- Modern [ERC20 implementation](https://github.com/maple-labs/erc-20/blob/main/src/ERC20.sol) using Solidity over/under flow checks
- Anton Bukov’s [Cumulative Merkle Tree drop](https://github.com/1inch/cumulative-merkle-drop), currently being audited
- [opensea.rs](https://github.com/gakonst/opensea-rs/): Rust CLI for OpenSea, supports Flashbots bundles, so orders don't get frontrun
- Etherscan [Transaction Decoder](https://twitter.com/etherscan/status/1430859570017046529): single view of emitted events, state difference and execution trace
- Etherscan adds [verified contract name to creation transaction](https://twitter.com/kvrncqc/status/1430876939703570434)
- Deep dive of [on chain SVG NFT](https://blog.simondlr.com/posts/flavours-of-on-chain-svg-nfts-on-ethereum) examples
- [ShadowySuperCoder NFT](https://blog.galaxy.eco/project-galaxy-announces-shadowy-super-coder-nft-pack-with-300-million-worth-of-perks-c5cb9ea2d18a) and infrastructure discounts for 100k addresses that deployed 1 or more contracts on mainnet (Disclosure: I claimed)

**Security**

- OpenZeppelin Contracts [TimelockController](https://twitter.com/OpenZeppelin/status/1430999829748932614) had security vulnerability, actor with executor role could escalate privileges, projects should migrate to TimelockController in v4.3.1
- SushiSwap paid [$1 million bounty to samczsun](https://twitter.com/josephdelong/status/1431314816698916865) for Miso vulnerability disclosure where $350 million was at risk and assistance with mitigation

**Ecosystem**

- Guide to [EIP1559 gas fee calculations](https://www.blocknative.com/blog/eip-1559-fees), explains base fee, priority fee and max fee (per gas)
- [Leveraged sandwiching](https://twitter.com/bertcmiller/status/1430169143123353611) using flash swaps
- Discussion on need for a [multi-chain ethereum provider](https://ethereum-magicians.org/t/multi-chain-ethereum-provider/6954)
- [Impersonator](https://twitter.com/apoorvlathey/status/1429212169531396099): log in to dapps impersonating any address via WalletConnect
- Vitalik: [alternatives to selling NFTs at below market prices](https://vitalik.ca/general/2021/08/22/prices.html) to avoid selling out quickly and gas market spikes

**Enterprise**

- Visa buys [CryptoPunk](https://twitter.com/VisaNews/status/1429745230023208969) and shares [NFT whitepaper](https://usa.visa.com/content/dam/VCOM/regional/na/us/Solutions/documents/visa-nft-whitepaper.pdf)
- Head of Gaming at YouTube: [Play-to-earn next major gaming model](https://twitter.com/Fwiz/status/1429108126234546182) along with open market for in-game digital items
- Budweiser buys [Beer.eth](https://twitter.com/dGenNetwork/status/1430330168095264768) and changes profile picture to rocket ship NFT

**Application layer**

- [ENS DNS namespace integration](https://medium.com/the-ethereum-name-service/full-dns-namespace-integration-to-ens-now-on-mainnet-9d37270807d3): domain name owners can import domains (such as weekinethereumnews.com) for use on ENS
- [Lyra](https://blog.lyra.finance/lyra-mainnet-launch/): native options trading on Optimism rollup, starting with single ETH market and liquidity provided by LyraDAO
- [DAI peg mechanics](https://twitter.com/Kurt_M_Barry/status/1429564277329911809) explainer of Vault mechanism, DAI saving rate and Peg Stability Module
- [Uniswap interactive math](https://twitter.com/danrobinson/status/1429972775511408651) demos
- Jonathan Mann deploys [NFT with on chain song](https://twitter.com/songadaymann/status/1430929924043509764)
- Simon de la Rouviere: [NFT fiction, top down vs bottom up](https://blog.simondlr.com/posts/top-down-vs-bottom-up-fiction-using-nfts)

**Regulation/business/tokens**

- [USDC reserves](https://www.centre.io/blog/usdc-reserves-composition) derisking to cash and short duration US Treasuries
- [VanEck](https://www.sec.gov/Archives/edgar/data/1137360/000113736021000522/vvtethereumetfformawaugust.htm) and [ProShares](https://www.sec.gov/Archives/edgar/data/0001174610/000168386321004549/f9483d1.htm) not proceeding with Ethereum ETFs
- Paypal launches [crypto services in UK](https://newsroom.uk.paypal-corp.com/2021-08-20-PayPal-Launches-the-Ability-to-Buy-Hold-and-Sell-Cryptocurrency-in-the-UK) to buy, hold and sell cryptocurrency
- [a16z token delegation open sourced](https://a16z.com/2021/08/26/open-sourcing-our-token-delegate-program/): best practices, criteria for assessing delegates and legal mechanics and template docs
- [ETH daily issuance](https://twitter.com/LucasOutumuro/status/1431133252702674944) lower than BTCs for first time due to EIP1559 and NFT activity

**General**

- 🎂 Week in Ethereum News turned 5, [first issue](https://weekinethereumnews.com/week-in-ethereum-news-august-21-2016/) was August 21, 2016
- [Gartner](https://www.gartner.com/smarterwithgartner/3-themes-surface-in-the-2021-hype-cycle-for-emerging-technologies/): NFTs are at the peak of inflated expectations but DeFi has plenty of room for hype growth
- Analysis of [cross chain bridges](https://medium.com/chainsafe-systems/bridges-in-crypto-space-12e158f5fd1e): security model, incentives and limitations
- Snowden: [Apple declared war on iPhone users privacy](https://edwardsnowden.substack.com/p/all-seeing-i)

* * *

## **Job Listings**

- Futureswap is hiring a [Product Marketing Manager](https://angel.co/company/futureswap/jobs/1509809-product-marketing-manager)
- Vac (Status) is looking for a [smart contracts protocol engineer](https://jobs.status.im/en/jobs/20563) for Waku
- Trail of Bits: [Blockchain Security Apprenticeship](https://jobs.lever.co/trailofbits/b2d6ce87-6b01-462f-965a-597a273ce26f)
- Solidity is [hiring a C++ dev](https://ethereum.bamboohr.com/jobs/view.php?id=40&source=weekinethnews)
- Nethermind [internship program](https://www.notion.so/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-28-2021/](https://weekinethereumnews.com/week-in-ethereum-news-august-28-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- **Sep 2 – [Prater testnet upgrade to Altair](https://github.com/eth2-clients/eth2-networks/pull/58) (epoch 36660)**
- **Sep 8  – [Gitcoin Grants Round 11](https://twitter.com/gitcoin/status/1430284881678962698) starts**
- Sep 15-17 – [MetaCartel MCON Denver](https://www.mcon.fun/)
- Sep 17-Oct 15 – [ETHOnline hackathon](https://online.ethglobal.com/)
- Oct 1-3 – [EthAtlanta](https://ethatl.com/) enterprise-focused hackathon & keynotes
- **Oct 20-21 - [LisCon](https://liscon.org/) (Lisbon)**
- Oct 22-24 – [ETH Lisbon](https://ethlisbon.org/) hackathon

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

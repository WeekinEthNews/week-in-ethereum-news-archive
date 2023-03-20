---
title: "Week in Ethereum News <br> March 18, 2023"
date: "2023-03-18"
---

## Eth News and Links

**Shapella (Shanghai + Capella) upgrade**

- Withdrawals are coming to [mainnet on April 12](https://github.com/ethereum/execution-specs/blob/master/network-upgrades/mainnet-upgrades/shanghai.md#upgrade-schedule) with the Shapella upgrade

- [Goerli testnet successfully upgraded](https://twitter.com/parithosh_j/status/1635795550875336705) to Shapella, testnet finalized after validators updated their clients, [withdrawals & BLS credential changes](https://goerli.beaconcha.in/validators/withdrawals) are being processed

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=ViLwzeIuJUc&t=545s). [Summary](https://twitter.com/abcoathup/status/1636512807725445120) by Tim Beiko.  Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1636410999027953664) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-execution-call-157/):
    - Mainnet Shapella upgrade scheduled, client releases expected in a week
    
    - Discussion on EL suggesting local blocks, consider after Shapella
    
    - Potential Cancun EIPs: SSZ minimal scope, SELFDESTRUCT removal, EVM MAX, BLS, transient storage, beacon state root in EVM, EOF, SWAPN & DUPN opcodes & PAY opcode
    
    - Ethereum Cat Herders [client diversity survey results](https://medium.com/ethereum-cat-herders/exploring-ethereums-client-ecosystem-afc9affa84dd)

**Dencun (Cancun + Deneb) upgrade**

- KZG Ceremony:
    - [First general contribution period is closed](https://twitter.com/trent_vanepps/status/1635311326213070848), people already in the lobby get to contribute
    
    - Special contribution period April 1-16

- consensus-specs [v1.3.0-rc.4](https://github.com/ethereum/consensus-specs/releases/tag/v1.3.0-rc.4): additional Deneb test vectors

- [EIP4844 fee market analysis](https://ethresear.ch/t/eip-4844-fee-market-analysis/15078): data price of 1 wei sets wrong expectations and incentivizes spammy use of blobs

**Layer 1**

- [Slot finder](https://slots.symphonious.net/) to pick time for network upgrades ([on historical roots boundary](https://twitter.com/TimBeiko/status/1636819688952045568))

- [Geth patched transaction pool DoS vulnerability](https://twitter.com/vdWijden/status/1635218368155488262) found on Goerli testnet

- Nimbus [v23.3.0](https://github.com/status-im/nimbus-eth2/releases/tag/v23.3.0) added support for running multiple execution clients

- Draft proposal to [replace SELFDESTRUCT with DEACTIVATE](https://notes.ethereum.org/@ipsilon/HJFA-Bkg2)

- Withdrawals: [Coinbase](https://www.coinbase.com/blog/ethereums-shapella-upgrade-is-coming-heres-what-you-need-to-know) expected ~24 hours after Shapella and [Lido](https://twitter.com/lidofinance/status/1635739580136652825) expected mid May

**Client releases**

- Consensus layer:
    - Nimbus [v23.3.1](https://github.com/status-im/nimbus-eth2/releases/tag/v23.3.1): config handling fixes, improves stability with Besu and fault tolerance when running multiple execution clients

- Execution layer:
    - Nethermind [v1.17.2](https://github.com/NethermindEth/nethermind/releases/tag/1.17.2): fixes bad block production when an empty block was scheduled

**Research**

- [Encrypted transaction pools](https://joncharbonneau.substack.com/p/encrypted-mempools) to address MEV & censorship

- [Transaction auctions](https://ethresear.ch/t/reducing-mev-with-transaction-auction/15057) with same trust assumptions as today to give some MEV back to users

- Idea for [Subgame Credible anti-MEV](https://twitter.com/stephensonhmatt/status/1636097739653259264) mechanism to retroactively penalize harms

**For Stakers**

- [Withdrawals explainer](https://mirror.xyz/rolfy.eth/ZTctOYeO2ZwOHm6ApUTfbh5wvQu1W_jZuvOpnLlsrzg): automated process but withdrawal key needs to be an Ethereum address, no need to rush BLS credential change unless mnemonic compromised

**Layer 2**

- [Arbitrum One & Nova](https://arbitrumfoundation.medium.com/arbitrum-the-next-phase-of-decentralization-e7f8b37b5226) moved to on-chain DAO governance with 9 of 12 security council (for emergency updates), token airdrop next week with 12.75% for users and 1.13% for Protocol Guild & DAOs with treasuries on Arbitrum; Arbitrum Orbit announced: permissionless creation of L3s

- Aztec: [sunsetting Aztec Connect](https://medium.com/aztec-protocol/sunsetting-aztec-connect-a786edce5cae) to focus on their zkEVM rollup

- Patrick McCorry: [defining rollups](https://stonecoldpat.substack.com/p/deconstructing-rollups) both by the community and the validating bridge

**EIPs/Standards**

- EIPs:
    - [EIP6690](https://github.com/ethereum/EIPs/pull/6690/files): EVM modular arithmetic extensions (EVM MAX) decoupled from EOF

- ERCs:
    - [ERC6682](https://github.com/ethereum/EIPs/pull/6682/files): NFT Flashloans

* * *

**This newsletter is made possible thanks to** [**Nexus Mutual**](https://nexusmutual.io/)

![Nexus Mutual](https://weekinethereumnews.com/wp-content/uploads/2023/02/Nexus-Mutual-2-1024x330.png)

What's so special about Nexus Mutual v2?

This upgrade makes the Nexus Mutual protocol an [infrastructure layer enabling an on-chain risk marketplace](https://nexusmutual.io/blog/nexus-mutual-v2-live-on-ethereum-mainnet). 

Now **anyone can build on top of the Nexus Mutual protocol** to _share any risk_ -- and not just crypto-related risks.

Don’t worry, you can still [buy coverage of your DeFi assets](https://nexusmutual.io/cover-products)!

* * *

**Stuff for developers**

- [EVM language design](https://jtriley.substack.com/p/ethereum-virtual-machine-language): overview of Solidity, Vyper, Fe, Huff, ETK and Yul

- [Calldata encoding](https://medium.com/@ljmanini/abi-encoding-deep-dive-fbb750facea9) deep dive

- Gas analysis of [clones vs naive factories](https://twitter.com/PopPunkOnChain/status/1636136500428673024): only use clones for low throughput

- [Function dispatcher optimization](https://philogy.github.io/posts/selector-switches/) using Huff

- [Ganache JSON-RPC reference](https://ganache.dev/), run RPC methods using Ganache in the browser

- web3.py [v6](https://snakecharmers.ethereum.org/web3py-v6-release/): Python v3.10/11 support, [AsyncHTTPProvider](https://snakecharmers.ethereum.org/web3-py-patterns-intro-async/), safe & finalized block identifiers, improved multithreading, improved customization and CCIP Read support

- Sourcify [v2](https://docs.sourcify.dev/blog/sourcify-v2/): reusable lib-sourcify library to verify a contract using the source, chain & address

- BlockSec [Phalcon](https://twitter.com/BlockSecTeam/status/1635282081793314821) transaction explorer adds debugging & improved transaction sharing

- [Pyrometer](https://www.nascent.xyz/idea/introducing-pyrometer): security tool for contract analysis, alpha

- [Paradigm data portal](https://twitter.com/notnotstorm/status/1636768359810498561): public datasets for contract bytecode & metadata, ETH transfers and contract slots, parquet file format

- Worldcoin: [World ID](https://worldcoin.org/blog/announcements/introducing-world-id-and-sdk) protocol & SDK with phone number & privacy-preserving iris verifications

**Security**

- Euler Finance [$197 million exploit](https://www.hacknote.co/17c261f7d8fWbdml/doc/186daaddc4cl77Dj#186daaddc4cl77Dj), lack of health check in donation mechanism

- ParaSpace exploit [blocked by BlockSec](https://twitter.com/ParaSpace_NFT/status/1636679472605982722) with 2.9k ETH rescued

- Immunefi [Proof of Concept templates](https://medium.com/immunefi/immunefi-poc-templates-4345f098ac69) using Foundry: reentrancy, token balance manipulation, flash loan and price manipulation

**Ecosystem**

- Finematics: [withdrawals explainer](https://finematics.com/ethereum-staking-withdrawals-explained/)

- EF’s [Next Billion fellowship](https://blog.ethereum.org/2023/03/16/fellowship-cohort-3-applications) cohort 3, applications close April 28

- Vitalik: [choosing guardians for multisig & social recovery wallets](https://www.reddit.com/r/ethereum/comments/11tijiv/how_i_think_about_choosing_guardians_for_multisig/)

**Enterprise**

- [NAB](https://news.nab.com.au/news/nab-completes-world-first-with-cross-border-stablecoin-transaction/) (Australian bank) pilots intra-bank cross border stablecoin transaction

- Microsoft [Edge browser](https://twitter.com/thebookisclosed/status/1636759487829917698) testing native crypto wallet

- [Meta winding down NFT efforts](https://twitter.com/skasriel/status/1635386565487898624) for now

**Application layer**

- Bank run panic caused USDC to depeg outside banking hours:
    - [Uniswap](https://twitter.com/haydenzadams/status/1634756130776678400) nearly $12 billion in daily volume
    
    - [MEV-Boost](https://twitter.com/bertcmiller/status/1634931226393051136) payments all time high
    
    - $DAI depegged, generally even more than USDC
    
    - [Maker](https://twitter.com/makerdao/status/1636009739329863680) reduced governance execution delay to 16 hours and added PSM circuit breaker

- [Nexus Mutual v2](https://nexusmutual.io/blog/nexus-mutual-v2-live-on-ethereum-mainnet) live on mainnet, cover for crypto-native & real world risks, cover as NFTs

- Sismo [zkConnect](https://twitter.com/sismo_eth/status/1636371873377423361): private single sign-on, beta

- [Stealcam](https://www.stealcam.com/faq): NFT photos only the holder can view, pixelated for everyone else, live on Arbitrum

- POAP [Drops](https://blog.poap.xyz/drops/): streamlined creation, view past drops and manage existing POAPs

- [DAO Drops](https://twitter.com/dao_drops/status/1634287532333584418) (retroactive public goods funding): allocate $250k DAI from EF grant. Voting power given to contract deployers, POAP collectors and DAO voters.  Vote by March 24

* * *

### Job Listings

- [Nimbus](https://nimbus.team/#about) is hiring a [Site Reliability Engineer](https://jobs.status.im/?gh_jid=4797968)

- Frax Finance is expanding their official core developer team. [Apply here!](https://docs.google.com/forms/d/e/1FAIpQLSem7KL-FFgsuxaUMww4OXMxdJ-qXfyWJ_IvGdqVteBSM5FgxA/viewform)

- L2BEAT 💗 is hiring a Senior Software Engineer & Product Owner. [Apply here!](https://l2beat.notion.site/We-are-hiring-Work-at-L2BEAT-e4e637265ae94c5db7dfa2de336b940f)

- [Immutable](https://www.immutable.com/) is hiring a [Principal Product Security Engineer](https://jobs.lever.co/immutable/71ade1b0-3b69-4b85-af79-3c5c223a0e1f)

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [FDIC fully protected deposits](https://home.treasury.gov/news/press-releases/jy1337) at SVB & Signature Bank, which helped restabilize USDC

- [US Fed](https://www.federalreserve.gov/newsevents/pressreleases/orders20230127a.htm) denies Caitlin Long’s Custodia Bank membership application (custodial only, no fractional reserves)

- Blockchain Association [collecting evidence of crypto debanking](https://twitter.com/jchervinsky/status/1636356457770762245)

- [Data visualization on implied versus realized volatility](https://blog.rysk.finance/low-volatility-in-crypto-markets-91446f5cbb28) in crypto options \[[Starbloom](https://twitter.com/starbloomvent) portfolio\]

- [Mint first](https://jacob.energy/mint-first.html): creators should mint content as NFTs and then amplify on social media

**General/crypto**

- PeopleDAO [76 ETH social engineering exploit](https://twitter.com/the_peopledao/status/1634518915668668416), payment added to Google sheet shared in Discord

- [Semacaulk](https://geometry.xyz/notebook/geometry-presents-semacaulk-a-gas-efficient-zero-knowledge-set-membership-protocol): zk set membership protocol, reduces insert gas from 1M to 68k (using KZG commitments instead of Merkle trees), proof of concept

- [CASPER](https://www.bleepingcomputer.com/news/security/casper-attack-steals-data-using-air-gapped-computers-internal-speaker/): secret channel attack via computer's internal speaker to a mobile phone at 20bits/sec

- [Vespass](https://github.com/nalinbhardwaj/Vespass#readme): password manager, uses secret sharing & hardware enclaves, no master password

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-march-18-2023](https://weekinethereumnews.com/week-in-ethereum-news-march-18-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Mar 21 – deadline for [Summer of Protocols](https://efdn.notion.site/Application-5b71c238d6bd44cf9137946ef7767e53)

- **Mar 24 – deadline to vote for** [**DAO drops**](https://twitter.com/dao_drops/status/1634287532333584418)

- Mar 28-30 – [Ethereum Rio](https://www.ethereumbrasil.com/ethereumrio)

- Mar 31 - Apr 2 – [ETHSamba](https://www.ethsamba.org/) (Rio) hackathon & conference

- Mar 31 – deadline for [EF account abstraction grants round](https://esp.ethereum.foundation/account-abstraction-grants)

- **Apr 5-8 –** [**ETH Beijing**](https://www.ethbeijing.xyz/) **hackathon**

- **Apr 12 –** [**Mainnet upgrades to Shapella**](https://github.com/ethereum/execution-specs/blob/master/network-upgrades/mainnet-upgrades/shanghai.md#upgrade-schedule)

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- Apr 13-16 – [Pragma Tokyo](https://ethglobal.com/events/pragma-tokyo) & [ETHGlobal Tokyo](https://tokyo.ethglobal.com/) hackathon

- Apr 14-16 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference & hackathon

- Apr 21-25 – [EthTaipei](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) hackathon & conference

- Apr 27-30 – [Istanbul ETH Privacy](https://www.leadingprivacy.com/istanbul) conference & hackathon

- **Apr 28 – deadline for EF’s** [**Next Billion fellowship cohort 3**](https://blog.ethereum.org/2023/03/16/fellowship-cohort-3-applications)

- May 5-10 – [ETHTallinn](https://ethtallinn.org/) hackathon & [NFT Tallinn](https://nfttallinn.com/) conference

- **May 9-12 –** [**EY blockchain summit**](https://web.cvent.com/event/c066d44d-4e50-4d7e-b6fb-3cc0abdae7ff/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7)

- May 12-14 – [ETHGlobal Lisbon](https://ethglobal.com/events/lisbon)

- May 19-23 – [EDCON](https://edcon.io/) Montenegro (changed from Vienna)

- May 20-21 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 24-26 – [Spaghett ETH](https://naples.spaghett-eth.com/) (Naples) conference

- May 26-28 – [ETHDublin](https://www.ethdublin.io/) hackathon

- Jun 2-4 – [ETH Seoul](https://2023.ethseoul.org/)

- Jun 2-6 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 9-11 – [ETHPrague](https://ethprague.com/) conference & hackathon

- Jun 23–25 – [ETHGlobal Waterloo](https://ethglobal.com/events/waterloo2023) (changed from Toronto)

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Aug 16-19 – [Ethereum Argentina](https://twitter.com/EtherArgentina/status/1625857633260552200) (Buenos Aires)

- Aug 30 - Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- **Sep 15 –** [**Protocol Berg**](https://protocol.berlin/) **(Berlin)**

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–25 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- **Oct 28–30 –** [**ETH Lisbon**](https://www.ethlisbon.org/) **hackathon**

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

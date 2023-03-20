---
title: "Week in Ethereum News <br> March 4, 2023"
date: "2023-03-04"
---

## **Eth News and Links**

**Shapella (Shanghai + Capella) upgrade**

- [Sepolia testnet](https://twitter.com/parithosh_j/status/1630423179687604225) successfully upgraded to Shapella

- [withdrawal-mainnet-shadowfork-2](https://twitter.com/abcoathup/status/1631783236748857344) successfully upgraded to Shapella, circuit breaker to local block building tested

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=GNhrb5txJ4M&t=168s). Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1631371121399562245):
    - Goerli testnet Shapella upgrade scheduled for March 14, 10:25 PM UTC
    
    - Mainnet Shapella upgrade ~4 weeks after Goerli (assuming no issues), date to be selected at next ACDE call
    
    - Cancun planning discussions: SSZ, EIP4788 (beacon state root in EVM), EIP2537 (BLS12-381 precompile) & removing SELFDESTRUCT
    
    - Geth proposals to remove eth/66, pending blocks & pre-merge sync

- Wallet devs: [withdrawals increment account balances without transactions](https://twitter.com/TimBeiko/status/1630693566023598085)

**Dencun (Cancun + Deneb) upgrade**

- KZG Ceremony:
    - [61k+ contributors](https://ceremony.ethereum.org/), 20k+ in the lobby, 9 days left in _first_ general contribution period
    
    - [JavaScript client](https://github.com/dsrvlabs/czg-keremony#readme) implementation

- SSZ breakout [video call](https://www.youtube.com/watch?v=Nl7iwAcqekY): EIP updated with metrics of [Union vs normalized](https://ethereum-magicians.org/t/eip-6404-ssz-transactions-root/12783/17) transaction representation

**Layer 1**

- Execution layer client diversity: [Nethermind client is over 20% of synced nodes](https://twitter.com/ant_sabado/status/1630732757012717570)

- EF [account abstraction grants round](https://esp.ethereum.foundation/account-abstraction-grants), up to $300k available, deadline March 31

- Flashbots:
    - [backrunning private transactions using multi-party computation](https://writings.flashbots.net/backrunning-private-txs-MPC), proof of concept
    
    - [block builder running inside an SGX enclave](https://writings.flashbots.net/block-building-inside-sgx), on Sepolia testnet

- Proposal to [uncouple blobs from the execution payload](https://ethereum-magicians.org/t/uncouple-blobs-from-the-execution-payload/13059)

**Research**

- Proposal for [simple single slot finality](https://ethresear.ch/t/a-simple-single-slot-finality-protocol/14920), synchronous dynamically available protocol plus a finality gadget

- Analysis of [orderflow auctions (OFAs)](https://frontier.tech/the-orderflow-auction-design-space)

**For Stakers**

- Rocket Pool [Rescue Node](https://rescuenode.com/): fallback node for temporary access in case of emergencies or maintenance

**Layer 2**

- Scroll zkEVM [alpha testnet](https://scroll.io/blog/alphaTestnet)

- Arbitrum’s proposed [time boost](https://offchain.medium.com/time-boost-a-new-transaction-ordering-policy-for-arbitrum-5b3066382d62) alternative to first come first served (FCFS) transaction ordering, MEV searchers can buy up to 0.5 second boost for transactions

- Jordi Baylina: [provers are not the bottleneck to zk rollup scalability](https://twitter.com/jbaylina/status/1629352597445394432) as they can run in parallel

- Patrick McCorry: [off-chain systems](https://stonecoldpat.substack.com/p/sharp-superchain-layer-3s-temporary) (Layer 3) on top of rollups

**EIPs/Standards**

- ERCs:
    - [ERC6596](https://github.com/ethereum/EIPs/pull/6596/files): Historical asset metadata JSON schema

* * *

### **This newsletter is made possible thanks to** [**Hardhat**](https://hardhat.org/)**’s VSCode extension!**

![](https://weekinethereumnews.com/wp-content/uploads/2021/06/hardhat-rectangle-1024x325.png)

The Hardhat for Visual Studio Code extension adds comprehensive language support for Solidity to Visual Studio Code and enhances editor integration for Hardhat projects.

Key features include code completion, go to definition, symbol renaming, and inline code validation from compiler errors/warnings. 

The extension also provides helpful code actions, hover help, and support for adding access modifiers and virtual/override keywords to function signatures. 

Get it from the [VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=NomicFoundation.hardhat-solidity)

* * *

**Stuff for developers**

- Hardhat [v2.13.0](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.13.0): ES Modules (ESM) support and improved IR based compilation

- Remix [v0.31](https://medium.com/remix-ide/remix-release-v0-31-0-a-forking-good-time-64dfca5a6a08): fork mainnet/testnets/custom networks, check UUPS contracts for storage layout incompatibilities, backup files/folders, UML zooming and Remixd v0.6.12

- Foundry:
    - forge-std [v1.5.0](https://twitter.com/msolomon44/status/1630729716272447489): StdStyle for console colors/styles, left/right shown for assertion failures, ERC721 & ERC1155 deal cheats, assertEqCall and minimum gas variants of expectCall
    
    - Foundry scripts [base abstract contract](https://twitter.com/PaulRBerg/status/1629480999888273412)

- Trail of Bits [properties](https://blog.trailofbits.com/2023/02/27/reusable-properties-ethereum-contracts-echidna/) for ABDKMath64x64, ERC20 & ERC4626, use with Echidna fuzzing or [Foundry unit tests](https://twitter.com/gakonst/status/1630290323263086594)

- OpenZeppelin [v4.8.2](https://github.com/OpenZeppelin/openzeppelin-contracts/releases/tag/v4.8.2): fix for ERC721Consecutive incorrect balance with batch of 1

- [Unchecked counter](https://github.com/PaulRBerg/unchecked-counter#readme): \`+\` user defined operator to improve readability of unchecked loops

- [Bit shifting and masking](https://medium.com/@mweiss.eth/solidity-and-evm-bit-shifting-and-masking-in-assembly-yul-942f4b4ebb6a) in assembly (Yul)

- [Poseidon-huff](https://github.com/rymnc/poseidon-huff#readme): Poseidon hash function ported to Huff

- Fe (language) [v0.21.0-alpha](https://github.com/ethereum/fe/releases/tag/v0.21.0-alpha): Self type, Max/Min traits with implementations for numeric types

- wagmi [ABIType v0.6](https://twitter.com/wagmi_sh/status/1631017966505541633): adds human-readable ABI type-level & runtime parse utilities

- Starter kits:
    - [Buidl-frontend](https://github.com/District-Labs/buidl-frontend#readme): wagmi, RainbowKit, Next.js; plus message signing, sign in with Ethereum & contract deploy
    
    - [Optimism starter](https://github.com/ethereum-optimism/optimism-starter#readme): wagmi, Foundry, RainbowKit & Vite; plus Optimism’s attestation station

- tx2uml [v1.1.0](https://github.com/naddison36/tx2uml/releases/tag/v1.1.0): adds value transfer diagrams

- [Sybil Form](https://github.com/dabit3/sybil-form#readme): sybil-resistant form using Gitcoin Passport

- [Tenderly Faucet](https://tenderly-faucet.vercel.app/): fork a network and fund addresses via the faucet

- CTFs:
    - [Curta](https://www.curta.wtf/) CTF protocol live
    
    - [Sussy](https://github.com/Philogy/sussy-huff-ctf#readme) Huff challenge
    
    - EKO2022 CTF [Metaverse Supermarket solution](https://stermi.xyz/blog/eko2022-ctf-metaverse-supermarket-solution)
    
    - Damn Vulnerable DeFi v3 [Unstoppable solution](https://bytes032.xyz/Notes/Unstoppable)
    
    - Secureum RACE #15: [8 question Solidity quiz & answers](https://ventral.digital/posts/2023/2/27/race-15-of-the-secureum-bootcamp-epoch-infinity)

- [Fusion zkRollup](https://github.com/leonardoalt/fusion#readme): experimental simple rollup in Rust

**Security**

- [Analysis of exploitable contract bugs](https://www.cs.purdue.edu/homes/zhan3299/res/ICSE23.pdf) \[PDF\] from Code4rena contests, 80% are currently beyond existing detection tools

- [Counter Exploit Toolkit](https://github.com/jtriley-eth/counter-exploit-toolkit#readme): upgradeable contract with arbitrary storage write access, token & ETH withdrawal, ETH deposit honeypot and token transfer from an attacker

**Ecosystem**

- Reminder: [Goerli testnet is deprecated](https://github.com/eth-clients/goerli#readme) with support until the end of the year

- [Devcon 7](https://blog.ethereum.org/2023/02/28/devcon-7-update) coming to South East Asia in 2024, [likely Q3/Q4](https://twitter.com/skylar_eth/status/1630644534605430796).  [Propose](https://forum.devcon.org/c/devcon-7-location-suggestions/14) a city.  [Dev connect](https://twitter.com/EFDevcon/status/1630543193358958592) later in 2023

- [Etherscan address display](https://twitter.com/etherscan/status/1630191302792052736) changed to default to first and last few characters

- Vitalik: [still more to be done to improve the user experience](https://vitalik.eth.limo/general/2023/02/28/ux.html)

**Application layer**

- Account abstraction:
    - ERC4337 [EntryPoint contract](https://twitter.com/erc4337/status/1631087958949531648) deployed on mainnet & Optimism, user operations are sent to a private mempool, bundlers then batch & send to EntryPoint for execution 
    
    - Safe [{Core}](https://safe.mirror.xyz/FLvQQ5J9qXks0izRl73oC6LiFLofbwFNorwzaEj_xL8): account abstraction stack

- [MakerDAO declined](https://vote.makerdao.com/polling/QmRh87bm) Cogent Bank’s $100 million loan proposal

- [Proposal to rescue tokens](https://governance.aave.com/t/bgd-rescue-of-tokens-locked-on-aave-overview-and-phase-1/8150/80) sent to Aave by mistake

- [LlamaZip](https://twitter.com/0xngmi/status/1630367605415444480): UniswapV3 router optimized for Optimism by compressing calldata

- [Ethereum Attestation Service](https://mirror.xyz/0xeee68aECeB4A9e9f328a46c39F50d83fA0239cDF/jmpn9Ykymny7JNCwWKkaDUFCx3MYqykx5phzfrVHHuE) live on Arbitrum

- Analysis of [airdrop impact on NFT marketplaces](https://rabbithole.mirror.xyz/s1BFIgK1oIDAiQnUpyIJtsfx18zvN0U6tWh4fW76DV8)

- POAP [Checkout](https://blog.poap.xyz/checkout/): sell POAPs for Sybil resistance or income on mainnet & Arbitrum

* * *

### Job Listings

- Shell Protocol team is hiring [senior Solidity devs & more](https://shellprotocol.io/posts/now-hiring-for-shell-protocol/), remote or Hawaii

- [Immutable](https://www.immutable.com/) is hiring a [Principal Product Security Engineer](https://jobs.lever.co/immutable/71ade1b0-3b69-4b85-af79-3c5c223a0e1f).

- Frax Finance is expanding their official core developer team. [Apply here!](https://docs.google.com/forms/d/e/1FAIpQLSem7KL-FFgsuxaUMww4OXMxdJ-qXfyWJ_IvGdqVteBSM5FgxA/viewform)

- [Request Network](https://request.network/en/) is hiring a [Community & Communication Manager](https://jobs.lever.co/request/76d0db8a-06bc-42c9-9816-69317c5f8c99)

- Certora is hiring a [Senior Enterprise Sales Rep](https://www.certora.com/#careers).

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- Coinbase [Crypto435 campaign](https://twitter.com/coinbase/status/1630592674020335617) to promote pro-crypto policy in US congress

- Reserve Bank of Australia [piloting 14 CBDC use cases](https://www.rba.gov.au/media-releases/2023/mr-23-06.html)

- Coindesk: [crypto clients suspend business with Silvergate bank](https://www.coindesk.com/business/2023/03/02/silvergate-stock-drops-over-50-as-crypto-clients-flee-beleaguered-bank/)

- [Coinbase](https://twitter.com/CoinbaseAssets/status/1630236377622228994) suspending trading of Binance USD (BUSD)

- Collective DAO [governance library](https://plaid-cement-e44.notion.site/The-Collective-DAO-Archives-Governance-Library-a58c6a2567c34636bc425ac97c7c9a79): DAO policies, programs and processes

**General/crypto**

- [LastPass attack details](https://support.lastpass.com/help/incident-2-additional-details-of-the-attack): keylogger installed on DevOps engineers home computer via vulnerable media software to access corporate vault

- Celer: [benchmark of SHA-256 on SNARK/STARK circuit development frameworks](https://blog.celer.network/2023/03/01/the-pantheon-of-zero-knowledge-proof-development-frameworks/) using metrics of proof generation time, peak memory usage and CPU utilization

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-march-4-2023](https://weekinethereumnews.com/week-in-ethereum-news-march-4-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Mar 10-29 – [Scaling Ethereum](https://ethglobal.com/events/scaling2023) (ETHGlobal) virtual

- Mar 11 – [Ethereum Guatemala](https://www.eventbrite.com/e/ethereum-guatemala-11-de-marzo-tickets-531104466757)

- **Mar 14 –** [**Goerli testnet upgrades to Shapella**](https://github.com/ethereum/execution-specs/blob/master/network-upgrades/mainnet-upgrades/shanghai.md#upgrade-schedule)

- Mar 15-16 – [ETHDubai](https://www.ethdubaiconf.org/)

- Mar 16-18 – [ETH Porto](https://ethporto.org/)

- Mar 28-30 – [Ethereum Rio](https://www.ethereumbrasil.com/ethereumrio)

- **Mar 31 - Apr 2 –** [**ETHSamba**](https://twitter.com/ethsamba/status/1631326304447627265) **(Rio) hackathon & conference**

- **Mar 31 – deadline for** [**EF account abstraction grants round**](https://esp.ethereum.foundation/account-abstraction-grants)

- Apr 12-14 – [NFT NYC](https://www.nft.nyc/)

- Apr 14-16 – [ETHGlobal Tokyo](https://tokyo.ethglobal.com/)

- Apr 14-16 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference & hackathon

- Apr 21-25 – [EthTaipei](https://eth-taipei.notion.site/ETHTaipei-2023-7aba2e9b4d264385ad26cb926639ed3a) hackathon & conference

- Apr 27-30 – [Istanbul ETH Privacy](https://www.leadingprivacy.com/istanbul) conference & hackathon

- May 5-7 – [ETHTallinn](https://ethtallinn.org/) hackathon

- May 9-10 – [NFT Tallinn](https://nfttallinn.com/) conference

- May 19-23 – [EDCON](https://edcon.io/) Montenegro (changed from Vienna)

- May 20-21 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 24-26 – [Spaghett ETH](https://naples.spaghett-eth.com/) (Naples) conference

- **May 26-28 –** [**ETHDublin**](https://www.ethdublin.io/) **hackathon**

- Jun 2-4 – [ETH Seoul](https://2023.ethseoul.org/)

- **Jun 2-6 –** [**ETH Belgrade**](https://ethbelgrade.rs/) **conference & hackathon**

- Jun 9-11 – [ETHPrague](https://ethprague.com/) conference & hackathon

- Jun 23–25 – [ETHGlobal Toronto](https://ethglobal.com/events/toronto)

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Aug 16-19 – [Ethereum Argentina](https://twitter.com/EtherArgentina/status/1625857633260552200) (Buenos Aires)

- **Aug 30 - Sep 3 –** [**ETHWarsaw**](https://www.ethwarsaw.dev/) **conference & hackathon**

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–25 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

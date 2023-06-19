---
title: "Week in Ethereum News <br> June 17, 2023"
date: "2023-06-17"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=ybgQuRcz9sg&t=58s). Notes from [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-consensus-call-111/):
    - Deneb scope: EIP7044 (perpetually valid signed voluntary exits) & EIP4788 (beacon root in EVM); considered for inclusion: EIP7045 (increase max attestation inclusion slot) & EIP6988 (prevent slashed validator being elected block proposer)
    
    - Discussion on reorgs increasing and proposal to [change sub-slot timing](https://github.com/ethereum/consensus-specs/pull/3433) for block production, attestation & aggregation
    
    - Discussion on staking with more than 32 ETH per validator

- EIP4844:
    - Latest EIP4844 implementer [call video](https://www.youtube.com/watch?v=jQ86ItkOfm0). Notes from [Terence](https://twitter.com/terencechain/status/1668332513645977612) 
    
    - Dankrad’s additional [testing to size blobs per block](https://notes.ethereum.org/OZJ90ZlcQtyrtZa6INYixQ?view#Test-day-2-110623)
    
    - [EIP4844 devnet 6](https://4844-devnet-6.ethpandaops.io/) launched
    
    - [KZG ceremony](https://ceremony.ethereum.org/) has over 110k contributions, lobby is empty

- Consensus-specs [v1.4.0-alpha.3](https://github.com/ethereum/consensus-specs/releases/tag/v1.4.0-alpha.3): patch to increase BLOB\_SIDECAR\_SUBNET\_COUNT to 6

**Layer 1**

- [Erigon archive node](https://twitter.com/ethereumonarm/status/1669257232779825153) running on $500 hardware

- Dedaub: [EIP6404/6466 SSZ transition impact](https://docs.google.com/document/d/1p-1VvOGwI5GHkwaGMzJYDL7Affofm6rVLa6cvnmoqGI/edit#heading=h.kqxi3kc5lnoq) on contracts using RLP \[Reminder: SSZ EIPs were already removed from Dencun upgrade\]

- [Beacon API checker](https://github.com/rauljordan/beacon-api-checker#readme): CLI to check API responses across clients, in Rust

**Client releases**

- Consensus layer:
    - Prysm [v4.0.6](https://github.com/prysmaticlabs/prysm/releases/tag/v4.0.6): bug fixes & optimizations to shorten block proposal time for edge cases
    
    - Teku [v23.6.0](https://github.com/ConsenSys/teku/releases/tag/23.6.0): rewards beacon-api endpoints & [how Teku fixed its May non-finality issue](https://mirror.xyz/rolfy.eth/w-hJGapBjnlOaMAjU4Bg8P2N7KyW4QOdaJN2FzBri-o)

- Execution layer:
    - Erigon [v2.45.2](https://github.com/ledgerwatch/erigon/releases/tag/v2.45.2): staged sync fix

**For Stakers**

- Payload’s [block analytics dashboard](https://payload.de/data/), beta

**Research**

- [Data visualization](https://ethresear.ch/t/cascading-network-effects-on-ethereums-finality/15871) on May loss of finality incident

**Layer 2**

- [Optimistic Erigon client](https://github.com/testinprod-io/op-erigon#readme) supports Optimism mainnet

- Arbitrum [sequencer batch posting post-mortem](https://arbitrumfoundation.notion.site/arbitrumfoundation/June-7-2023-Batch-Poster-Outage-d49c50df42864c7b83521fd7aa5897f2)

- [Layer 2 MEV](https://taiko.mirror.xyz/VjNjFws6OOVez5YCDMwjy4BUiDqZBHYDvcW4-JZGDkc) and decentralizing sequencing

- Frax Finance plans [Fraxchain rollup using its LSD as the gas fee token](https://www.theblock.co/post/235110/frax-finance-to-launch-ethereum-layer-2-named-fraxchain) 

**EIPs/Standards**

- ERCs:
    - [ERC7169](https://github.com/ethereum/EIPs/pull/7169/files): Tranche sequence
    
    - [ERC7182](https://github.com/ethereum/EIPs/pull/7182/files): Interface naming conventions: 

**Stuff for developers**

- Foundry:
    - [Pre-v1 updates](https://twitter.com/hievalir/status/1669781947642695680): fuzz-runs CLI flag, 0 basefee, batch transactions on Optimism and readCallers cheatcode
    
    - [Fuzzy DeFi](https://github.com/0xNazgul/fuzzydefi#readme): code properties for Uniswap v2, Olympus DAO & Compound v2 forks
    
    - [Forge-safe](https://github.com/ind-igo/forge-safe#readme): build Safe multisig batch transactions using Forge scripting

- OpenZeppelin Contracts [v4.9.2](https://github.com/OpenZeppelin/openzeppelin-contracts/releases/tag/v4.9.2): MerkleProof library patch, potential issue in multiproof leaf validation

- Uniswap [v4](https://github.com/Uniswap/v4-core#readme): customize liquidity pools using hooks, flash accounting using ERC1153 (transient storage) in Dencun upgrade, work in progress, 4 year business source license
    - [V4-template](https://github.com/saucepoint/v4-template#readme): template for creating Uniswap v4 hooks
    
    - [Huff hooks](https://github.com/jtriley-eth/huff-hooks#readme): Uniswap v4 hooks library in Huff, work in progress

- [Bytecode.zip](https://github.com/merklejerk/bytecode-zip-fe/blob/main/docs/HELP.md): deploy zipped & wrapper contracts from the browser

- Titanoboa (Vyper interpreter) [jupyter notebooks integration](https://twitter.com/big_tech_sux/status/1668305117605662720): sign via browser

- Ethers.js [ENS multicoin provider plugin](https://github.com/ethers-io/ext-provider-plugin-multicoin#readme) 

- [ABIType](https://twitter.com/wagmi_sh/status/1668324730582224898): adds conversion from JSON ABIs to human-readable ABIs at runtime & type-level

- RainbowKit [v1.0.2](https://github.com/rainbow-me/rainbowkit/releases/tag/%40rainbow-me%2Frainbowkit%401.0.2): adds WalletConnect v2 support

- [4byte collider](https://github.com/zobront/4byte-collider#readme): script to find function signatures with colliding 4byte selectors 

- [Wallet Test Framework](https://wtf.allwallet.dev/week-09/): switched to viem and added more tests

- [Passkey based Account Abstraction signer](https://ethresear.ch/t/passkey-based-account-abstraction-signer-for-smart-contract-wallets/15856) for contract wallets

**Security**

- Sturdy Finance, [$800k exploit](https://rekt.news/sturdy-rekt/), price manipulation via read-only reentrancy

- [Signature malleability](https://github.com/pcaversaccio/malleable-signatures#readme): proof of concept showing attack using compact signatures

**Ecosystem**

- [Holešky testnet](https://github.com/ethereum/pm/issues/803#issuecomment-1593108937) (Goerli successor) genesis planned for September 15 (Merge day) with 1.5 million validators, majority run by client teams

- [EF Q1 grantees](https://blog.ethereum.org/2023/06/15/allocation-update-q1-23) share $13 million in funding

- ETHPrague [hackathon winners](https://ethprague2023.devfolio.co/projects?show_winners=true) & [videos](https://www.youtube.com/playlist?list=PLRUSTVWJngidPVV_JC89YsomwtryPGV74)

**Enterprise**

- [BOCI](https://www.ubs.com/global/en/media/display-page-ndp/en-20230609-tokenized-notes.html) (Bank of China) issued CNH 200 million ($28M) in tokenized notes

**Notable at app layer**

- [Maker Dai Savings Rate (DSR)](https://twitter.com/MakerDAO/status/1669710346003808256) increases to 3.49% on June 19

- Uniswap [v4 vision](https://blog.uniswap.org/uniswap-v4): more generalized v3 allowing different tradeoffs via hooks for customized pools

- Uniswap Foundation [bridge assessment](https://uniswap.notion.site/Bridge-Assessment-Report-0c8477afadce425abac9c0bd175ca382)

- [EigenLayer stage 1](https://www.blog.eigenlayer.xyz/eigenlayer-stage-1-mainnet-launch/) live on mainnet, reached guarded launch limits; [restaking dashboard](https://restaking.nethermind.io/)

- [Sound](https://sound.mirror.xyz/eLJe_mQbJJf5_uNUu8AzJTP6VrfT7YIrSNFSeISE8Pc) (music NFTs) live on Optimism

- [The Goose](https://twitter.com/Sothebysverse/status/1669478259489226752) NFT sold for $5.4 million from 3AC collection

- Rough sailing lately for NFT infra projects: [JPG](https://twitter.com/______jpg______/status/1667818270672527363) pausing and [NFF (Backed)](https://twitter.com/backed_xyz/status/1668689845722423314) winding down

* * *

### Job Listings

- [Protocol Engineer](https://github.com/tvl-labs/job-board/blob/main/engineering/protocol_engineer.md) (DeFi) sought by [Tunnel Vision Labs](https://tunnelvisionlabs.xyz/)

- Devconnect Istanbul: [Production Assistant](https://jobs.lever.co/ethereumfoundation/db6e2775-39d3-4eb9-9313-dfb15dfab9bc) and [Volunteer Coordinator](https://jobs.lever.co/ethereumfoundation/401e0af5-f4a2-4e66-a724-4accb003113e)

- Solidity team need a highly skilled [Developer Advocate](https://jobs.lever.co/ethereumfoundation/b9e33c9e-48ee-464f-a672-d51eece2b99d)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US SEC:
    - [Extremely strange circumstances surrounding](https://twitter.com/MattWalshInBos/status/1669061636953366528) “compliant” Prometheum
    
    - [Blockchain Association FOIA request](https://twitter.com/MTCoppel/status/1669358891740860423) for communications about SEC’s suspicious approval
    
    - [Hinman docs](https://www.coindesk.com/policy/2023/06/13/hinman-emails-reveal-2018-speech-on-ether-drew-input-from-multiple-sec-officials/) on 2018 speech that Ether is not a security
    
    - Mark Cuban [eviscerates former SEC staffer](https://twitter.com/mcuban/status/1669338225197072387)

- Coindesk: [Tether heavily backed by Chinese commercial paper](https://www.coindesk.com/policy/2023/06/16/tethers-banking-relationships-commercial-paper-exposure-detailed-in-newly-released-legal-documents/)

- [BlackRock](https://www.reuters.com/business/finance/blackrock-close-filing-bitcoin-etf-coindesk-2023-06-15/) filed for spot Bitcoin ETF

- FT: [Hong Kong regulator pushing banks](https://archive.is/f6U5Q#selection-1575.39-1581.112) to accept more crypto exchanges as clients

- [Wyre](https://twitter.com/sendwyre/status/1669688772844220418) winding down

**General/crypto**

- [Video-based cryptanalysis](https://www.nassiben.com/video-based-crypta): key recovered from smartcard by analyzing video of power LED

- [Zeromorph](https://twitter.com/Zac_Aztec/status/1669751810037542912): speed ups to make Plonk performant  

- [ZachXBT sued by MachiBigBrother](https://twitter.com/zachxbt/status/1669783717236342785) (Jeffrey Huang) for defamation, donate: [zachxbtlegalfund.eth](https://etherscan.io/address/zachxbtlegalfund.eth)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-june-17-2023](https://weekinethereumnews.com/week-in-ethereum-news-june-17-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- **Jun 18** – [Ethereum Protocol Fellowship cohort four](https://blog.ethereum.org/2023/06/01/ethereum-protocol-fellowship-fourth-apps-open) application deadline **extended**

- Jun 20 – EF [run a node grant](https://esp.ethereum.foundation/run-a-node-grants) deadline

- Jun 22–25 – [Pragma Waterloo](https://ethglobal.com/events/pragma-waterloo) & [ETHGlobal Waterloo](https://ethglobal.com/events/waterloo2023) hackathon

- **Jun 26 – Jul 17 –** [**CLRFund round 9**](https://blog.clr.fund/clrfund-round-9-is-coming/)

- Jul 5-9 – [ETHBarcelona](https://ethbarcelona.com/) conference & hackathon

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- **Aug 11-13 –** [**ETHMunich**](https://ethmunich.de/) **hackathon**

- Aug 15-16 – [ETHToronto](https://www.ethtoronto.ca/) & [ETHWomen](https://www.ethwomen.com/)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org/) (Buenos Aires)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 30 – Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 18-21 – [ETH Montréal](https://ethmontreal.xyz/) conference & hackathon

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 6–27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 27–29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://twitter.com/ethbrno/status/1652198745902137344)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 17-19 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

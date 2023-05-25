---
title: "Week in Ethereum News <br>  May 20, 2023"
date: "2023-05-20"
---

## Eth News and Links

**Brief loss of finalization and first inactivity leak** 

- Prysm’s [finality issue postmortem](https://offchain.medium.com/post-mortem-report-ethereum-mainnet-finality-05-11-2023-95e271dfd8b2):
    - Valid attestations with old target checkpoint weren’t processed optimally
    
    - Delay in finalization for 4 epochs & 9 epochs (with inactivity leak)
    
    - 28 ETH in penalties & 55 ETH in missed validator revenue 
    
    - Block space dropped but gas prices weren’t higher than daily highest

- Ben Edgington & Superphiz: [finality issue discussion](https://www.youtube.com/watch?v=Fbhq04dutSc&t=1s) (video)

**Dencun (Cancun + Deneb) upgrade**

- Latest consensus layer devs [call video](https://www.youtube.com/watch?v=Iy5zTJIXhQU&t=235s). Notes from [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-consensus-call-109/):
    - Discussions on PRs for Deneb, removing merge conditions, adding confirmation rule and non-expiring signed voluntary exits

- EIP4844:
    - Latest EIP4844 implementer [call video](https://www.youtube.com/watch?v=IckYm8ZXZtE&t=2s). Notes from [Terence](https://twitter.com/terencechain/status/1658154962625650688)
    
    - [KZG ceremony](https://ceremony.ethereum.org/) available with no waiting to anyone with [32 mainnet transactions](https://twitter.com/CarlBeek/status/1655991868390539264)

- Proposal for [ordering Cancun & Prague opcodes](https://hackmd.io/@shemnon/CancunOpcodeAllocation) in a more coherent layout

**Layer 1**

- Proto’s [consensus.actor](https://github.com/protolambda/consensus-actor#readme): interactive map of attester performance using Nimbus Era files

- [Validator withdrawal/exit](https://github.com/gonlad-x/validator_queue_monitoring) queue monitoring

- [Lambda consensus client planned](https://twitter.com/fede_intern/status/1658484150834442240), to be developed in Elixir by LATAM team

- Geth team [brain dump on implementing light clients](https://gist.github.com/karalabe/184125637d587a16fe038f99a6daefea)

**Client releases**

- Consensus layer:
    - Nimbus [v23.5.1](https://github.com/status-im/nimbus-eth2/releases/tag/v23.5.1): improves 3rd party validator clients/beacon node compatibility and adds incremental pruning
    
    - Prysm [v4.0.4](https://github.com/prysmaticlabs/prysm/releases/tag/v4.0.4): fix for finality issue
    
    - Teku [v23.5.0](https://github.com/ConsenSys/teku/releases/tag/23.5.0): fix for finality issue

- Execution layer:
    - Erigon [v2.43.1](https://github.com/ledgerwatch/erigon/releases/tag/v2.43.1): fixes

**For Stakers**

- [Lido v2](https://blog.lido.fi/lido-v2-launch/) live:
    - Withdrawals; no service should have more than 22% of stake (Lido has ~33%)
    
    - Staking router (allows permissionless onboarding of node operators)

- [Timeserver diversity](https://old.reddit.com/r/ethstaker/comments/13gw7e1/should_i_worry_about_timeserver_diversity/) discussion

- [Lost validator seed phrase on Ledger](https://www.reddit.com/r/ledgerwallet/comments/13kk6iz/successful_recovery_of_70_eth_eip2333_in/) had private keys generated using custom app

**Research**

- Justin Drake: [MEV burn](https://ethresear.ch/t/mev-burn-a-simple-design/15590) add-on to enshrined PBS, smooth & redistribute MEV spikes

**Layer 2**

- [Aztec rollup circuit proving time sped up](https://twitter.com/mike_connor/status/1658533498058326016), Nullifier Tree (used to prevent actions being repeated) reduced from 2^254 leaves to 2^32

**EIPs/Standards**

- EIPs:
    - [EIP7039](https://github.com/ethereum/EIPs/pull/7039/files): Scheme-handler discovery option for wallets
    
    - [EIP7044](https://github.com/ethereum/EIPs/pull/7044/files): Perpetually valid signed voluntary exits
    
    - [EIP7045](https://github.com/ethereum/EIPs/pull/7045/files): Increase max attestation inclusion slot

**Stuff for developers**

- Solidity [immutable variables can be initialized multiple times or left uninitialized](https://twitter.com/solidity_lang/status/1658484463834374154)

- Remix [v0.33](https://medium.com/remix-ide/remix-release-v0-33-0-4fa74d315618): adds scientific notation for input, refactored WalletConnect plugin, updated Etherscan verification plugin, generate docs from file explorer and Sol2UML zoom 

- Foundry:
    - [Scopelint](https://github.com/ScopeLift/scopelint#readme): formatter & linter for Solidity & TOML and spec generation from tests
    
    - [ScopeLift Foundry template](https://github.com/ScopeLift/foundry-template/#readme)
    
    - Tip: [fuzz settings in inline comments](https://twitter.com/paulrberg/status/1657731377662402563)

- [VS Code Solidity](https://twitter.com/juanfranblanco/status/1658869719514972165) plugin: language server rewrite includes code completion, go to definition, find references, hover info; Solparse upgrades; download code & ABI from Etherscan

- Solidity [try/catch edge cases](https://blog.theredguild.org/catch-me-if-you-can/)

- Solc (Solidity compiler) [calling conventions](https://blog.smlxl.io/solc-internals-part-1-calling-conventions-89d62249ccda)

- [Fundraise](https://github.com/409H/fundraise#readme): Solidity contract for memecoin presales with soft/hard caps, unaudited

- [Ether deck](https://github.com/jtriley-eth/ether-deck#readme): extensible multisig in Huff, unaudited

- [Pyrometer](https://www.nascent.xyz/idea/pyrometer-enters-beta): verifies Solidity functions perform as expected via showing how variables change, beta

- [4byte.directory](https://www.reddit.com/r/ethereum/comments/13l7amg/the_4bytedirectory_is_going_to_be_new_management/?context=3) maintenance moving to beaconchain.in team

- [Contract diff](https://x48.tools/diff): mainnet and layer 2 support, multifile support, split & unified modes and summaries

- [Next.js app router + TypeScript + ConnectKit](https://github.com/m1guelpf/nextjs13-connectkit-siwe#readme) Sign in with Ethereum example

- CTFs:
    - Curta [Last One Standing solution](https://twitter.com/fiveoutofnine/status/1658930303019122688)
    
    - Dragonfly CTF [solution](https://twitter.com/merklejerk/status/1658510438512852999)

- [Base Camp](https://docs.base.org/base-camp/docs/welcome): contract development guide for beginners using Remix & deploying to Base testnet

- RareSkills [contract security guide](https://www.rareskills.io/post/smart-contract-security)

**Ecosystem**

- ETHGlobal [Lisbon hackathon finalists](https://twitter.com/ethglobal/status/1657794093802483714)

**Enterprise**

- Visa: [experiments with ERC4337 account abstraction](https://usa.visa.com/solutions/crypto/rethink-digital-transactions-with-account-abstraction.html) on Goerli testnet

**Notable at app layer**

- [Compound v3](https://twitter.com/compoundfinance/status/1658268323556229121) live on Arbitrum

- [Pimlico ERC20 paymaster](https://twitter.com/pimlicoHQ/status/1658597090409209859) for ERC4337 account abstraction live on mainnet, Arbitrum & Optimism

- [DeFiReturns v2](https://medium.com/defireturns/the-new-era-of-defi-investing-introducing-the-relaunched-defireturns-3026d3ed11c4) launches with actual returns, with or without rewards, for ~10 major DeFi protocols

* * *

### Job Listings

- Solidity team need a highly skilled [Developer Advocate](https://jobs.lever.co/ethereumfoundation/b9e33c9e-48ee-464f-a672-d51eece2b99d)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**General/crypto**

- Ledger’s planned KYC’d account recovery leads to a furious blowback during which they [admit that a malicious firmware update can steal](https://www.coindesk.com/business/2023/05/18/ledger-continues-to-defend-recovery-system-says-its-always-technically-possible-to-extract-users-keys/) your crypto despite [prior assurances that they couldn’t](https://twitter.com/CalciumBagel/status/1659340406352429057)

- Argentina [suspending custodial crypto accounts](https://www.msn.com/en-us/money/companies/argentina-moves-to-tighten-grip-on-crypto-transactions/ar-AA1b1on0) as a result of IMF deal

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-may-20-2023](https://weekinethereumnews.com/week-in-ethereum-news-may-20-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- May 24-26 – [Spaghett ETH](https://naples.spaghett-eth.com/) (Naples) conference

- May 26-28 – [ETHDublin](https://www.ethdublin.io/) hackathon

- Jun 2-4 – [ETH Seoul](https://2023.ethseoul.org/)

- Jun 2-7 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 9-11 – [ETHPrague](https://ethprague.com/) conference & hackathon

- Jun 23–25 – [ETHGlobal Waterloo](https://ethglobal.com/events/waterloo2023) (changed from Toronto)

- Jul 5-9 – [ETHBarcelona](https://ethbarcelona.com/) conference & hackathon

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Aug 15-16 – [ETHToronto](https://www.ethtoronto.ca/) & [ETHWomen](https://www.ethwomen.com/)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org/) (Buenos Aires)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 30 – Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 18-21 – [ETH Montréal](https://ethmontreal.xyz/) hackathon & conference

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- **Oct 6-8 –** [**ETHRome**](https://ethrome.org) **hackathon**

- Oct 6–27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 27–29 – [ETH Miami](https://ethmiami.net/) festival + hackathon

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://twitter.com/ethbrno/status/1652198745902137344)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 17-19 – [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

---
title: "Week in Ethereum News <br> April 2, 2022"
date: "2022-04-02"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest core devs [call video](https://www.youtube.com/watch?v=1QU8r9-SJDc&t=322s). Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1509955843654971392) & [Christine Kim](https://twitter.com/christine_dkim/status/1509924174025924615):
    - shadow fork merge testing finds RAM & timeout issues 
    - difficulty bomb will need to be delayed if public testnet upgrades to PoS are not started by late April
    - Shanghai upgrade planning: append withdrawals in block headers, discussed if EIP1153 (transient storage opcodes) should be included
    - Goerli supply inflation discussion
- Besu [v22.1.3](https://github.com/hyperledger/besu/releases/tag/22.1.3): bonsai tries (“super pruning”) no longer experimental, enables faster read & improved storage performance
- Geth [v1.10.17](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.17): prep for merge and upcoming state layout change
- Erigon [v2022.03.02](https://github.com/ledgerwatch/erigon/releases/tag/v2022.03.02): MDBX upgrade, subscribe to events via websockets
- Erigon v2 [video of plans](https://www.youtube.com/watch?v=QqL72qWhF-g) to solve snapshot sync & granularity of history
- [Analysis of selfdestruct usage](https://github.com/jwasinger/eth-selfdestruct-analysis#readme) after London upgrade
- Verkle tree [explainer](https://twitter.com/gballet/status/1508422189216894979) for app devs to understand the gas cost changes

**Proof of Stake consensus layer**

- No more [supermajority staking client](https://twitter.com/superphiz/status/1509006284552654848):
    - Prysm estimated usage down to ~62% 
    - Coinbase, Kraken & Binance estimated usage still over 70%
    - competent staking providers [should run every client](https://twitter.com/technocrypto/status/1508565013094666248) 
- Beacon APIs [v2.2.0](https://github.com/ethereum/beacon-APIs/releases/tag/v2.2.0)
- [Nimbus](https://twitter.com/jcksie/status/1508718929010692098) full sync in 42 hours & trusted node sync in 7 hours

**PoW switch off (the merge)**

- Reminder of [what to expect from the merge](https://twitter.com/trent_vanepps/status/1508478499325202435), fees go to block proposers, withdrawals in Shanghai, 12s block times, no fee reduction, stakers need to run EL client, transition trigger is TTD and don’t need ETH to run a node
- Details of how [withdrawals spec has evolved](https://notes.ethereum.org/@ralexstokes/r1NVzAeQq): push-style withdrawals, managed by the consensus layer, processed by the execution layer
- Alchemy’s [Kiln testnet faucet](https://kilnfaucet.com/)

**EIPs/Standards**

- [EIP4944](https://github.com/ethereum/EIPs/blob/75de4fbbb85d35c73348722f3057c985602ea663/EIPS/eip-4944.md): NFT with wallet
- [EIP4950](https://github.com/ethereum/EIPs/blob/59b0f5ee25b917303c8e6278fb03119923c7cb01/EIPS/eip-entangled.md): Entangled Tokens
- [EIP4955](https://github.com/ethereum/EIPs/blob/8a77afc8bee22064d69b40b431921ca976eb7912/EIPS/eip-4955.md): NFT metadata standard namespaces extension
- [EIP4962](https://github.com/ethereum/EIPs/blob/994a819df180edb1106d3aa111828bd52c615871/EIPS/eip-4962.md): DEST Operation

**Layer2**

- Optimism [calldata compression](https://twitter.com/bkiepuszewski/status/1508740414492323840): how to decompress Layer 2 transactions
- [Rollup centric future](https://twitter.com/pseudotheos/status/1509530981581000705) rather than cross-chain as bridges are single point of failure and introduce contagion risk for the destination chain

* * *

### **This newsletter is made possible thanks to [SpeedRunEthereum](https://speedrunethereum.com/)!**

![SpeedRunEthereum](https://weekinethereumnews.com/wp-content/uploads/2022/04/Screenshot-from-2022-04-01-15-39-52.png)

[](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fae4a93cc-340d-4a7f-a476-c79771e7a0c3_769x208.png)

Are you a web2 dev who wants to get into web3?  

The best way to go from _zero_ to **hero** is [SpeedRunEthereum.com](https://speedrunethereum.com/).

Learn how to build on Ethereum; the superpowers and the gotchas.

Then [speed run Ethereum](https://speedrunethereum.com/) by testing your skills in a [series of challenges](https://speedrunethereum.com/challenge/simple-nft-example) and [join web3](https://twitter.com/austingriffith/status/1493688828661432325).

* * *

**Stuff for developers**

- Foundry [v0.2.0](https://www.paradigm.xyz/2022/03/foundry-02): faster compilation & testing, call traces, gas reports, interactive debugger, more cheatcodes, smarter fuzzer, TOML config and easy installation; [Docker image](https://twitter.com/cryptophinn/status/1508182595627991041)
- [Contract-template](https://github.com/cleanunicorn/ethereum-smartcontract-template#readme): Foundry template with GitHub actions configured
- [Foundry-Yulp-Template](https://github.com/ControlCplusControlV/Foundry-Yulp-Template#readme): Yul+ contracts template, test using Foundry
- [Solve ParadigmCTF's JOP challenge](https://plotchy.substack.com/p/solving-paradigmctfs-jop-) using Foundry call traces, cheatcodes and debugger
- [Forta Hardhat plugin](https://github.com/forta-protocol/hardhat-forta#readme): add security/operational monitoring for contracts
- [Solidity trivia](https://twitter.com/patrickalphac/status/1508415843293700102), a thread by Patrick Collins
- [Sourcify](https://twitter.com/SourcifyEth/status/1509199927225851911) (source code verification) adds Sepolia testnet support
- [Goerli ETH faucet](https://goerli-faucet.pk910.de/) using PoW
- MetaMask Snaps [tutorial](https://github.com/Montoya/gas-fee-snap#readme)
- [Share mnemonics](https://medium.com/nethermind-eth/using-shamirs-secret-sharing-to-share-mnemonics-c40429835117) using Shamir’s secret sharing

**Security**

- Ronin bridge $600 million [exploit](https://roninblockchain.substack.com/p/community-alert-ronin-validators), 5 of 9 keys compromised, reportedly via social engineering, not discovered for 6 days; Kelvin’s [explainer](https://twitter.com/kelvinfichter/status/1508839255996522508)
- Revest Protocol ~$2 million [exploit](https://revestfinance.medium.com/revest-protocol-exploit-recovery-plan-b06ca33fbdf5), reentrancy on ERC1155 minting, protocol soft locked, pause on transfers saved further loss of $1 million
- GearBox protocol [vulnerability disclosed](https://medium.com/@nnez/different-parsers-different-results-acecf84dfb0c), path parsers gave different results, ~$10 million was at risk, fixed, $150k bounty paid
- Rari Capital: Fuse pool [vulnerability disclosed](https://medium.com/@JackLongarzo/rari-capital-fuse-security-upgrade-report-e5d154c16250), cross-asset reentrancy allowed assets to be borrowed for free, pools fixed via upgrade
- Guide to [security incident war rooms](https://twitter.com/storming0x/status/1509769575021178886): document, test, improve, repeat

**Ecosystem**

- Fortune [correcting misconceptions about the merge](https://fortune.com/2022/03/28/3-misconceptions-ethereum-merge/): doesn’t create a new token, doesn’t lower fees and no set date
- Flashbots Protect [fast mode](https://twitter.com/bertcmiller/status/1508818760723050504): frontrunning protection with faster inclusion and more blockspace but can revert
- Vitalik’s [retrospective on decisions not taken](https://vitalik.ca/general/2022/03/29/road.html): simpler Proof of Stake, complex sharding, more EVM features, high level language VM or clone of existing VM and different supply distribution

**Enterprise**

- [Budweiser USA](https://twitter.com/budweiserusa/status/1508231544263131137) hosted NFT Beerfest for token holders, physical Beer.eth cans (only 300 made)
- [Visa creator program](https://usa.visa.com/partner-with-us/info-for-partners/visa-creator-program.html): accelerate creator businesses with NFTs

**Application layer**

- [LooksRare](https://twitter.com/LooksRareNFT/status/1508791295669538818) integrates Etherscan chat for users to message addresses
- [DeFi Saver](https://blog.defisaver.com/makerdao-stop-loss-take-profit/) stop loss options for MakerDAO Vaults
- [Instadapp Lite](https://twitter.com/instadapp/status/1509258038875725824) single click strategies
- [Polynomial Earn](https://medium.com/polynomial-protocol/polynomial-earn-optimism-mainnet-launch-b95874b27ba6) (options vaults) live on Optimism
- [Verse](https://neuroswish.mirror.xyz/i7_5J7vyc-bg7r6pVzUNKH3bw_uQ6I1zPsTEmbiRktc) (NFTs with built-in ERC20 exchange) in beta
- [Element DAO](https://mirror.xyz/0x3fcAf7DDf64E6e109B1e2A5CC17875D4a5993F39/bctuLRkf7oBL4mMJ9lPf0y0blFjBDslTUfUL0CEk1gc): users & [ecosystem contributors](https://twitter.com/jonnyrhea/status/1509928534952796161) can claim non-transferrable governance token, GitHub/Discord claims via zk proofs \[Evan is an advisor\]

* * *

### **Job Listings**

- Status is Hiring! [Libp2p Networking Engineer](https://grnh.se/cbb1921b1us). [All jobs!](https://grnh.se/9fc6e6fc1us)
- SideShift.ai is hiring a [Solidity Engineer](https://sideshift.ai/jobs?utm_campaign=hiring&utm_source=weekinethnews). Good job!
- EF’s Privacy & Scaling Explorations team: [Technical Project Coordinator](https://jobs.lever.co/ethereumfoundation/78089bc2-125e-47de-af28-e162de149901?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum), [ZKP Security Engineer](https://jobs.lever.co/ethereumfoundation/b80cf733-9a8d-40f1-a85a-635acdc2b1b1?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum%20), [L2 Security Engineer](https://jobs.lever.co/ethereumfoundation/f3148457-ed1e-4659-941d-5f60b49427ca?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) & [Marketing Ops Manager](https://jobs.lever.co/ethereumfoundation/7a831e7c-1a0d-4e7b-8291-072292e26c0e?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum%20&lever-source%5B%5D=Week%20in%20Ethereum%20)
- [Hifi](http://hifi.finance/) is hiring a [Senior Solidity Engineer](https://bit.ly/3CMmbSe) & [Community/Social Media Manager](https://bit.ly/36q06g5)
- Devcon needs a [front-end web developer](https://ethereum.bamboohr.com/jobs/view.php?id=61&source=weekinethnews)
- EF hiring [Test Engineer](https://jobs.lever.co/ethereumfoundation/e6d303e5-168d-447e-a596-e3c2b105ca3f?lever-source%5B%5D=Week%20in%20Ethereum%20) to improve testing infrastructure & coverage

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Coinbase](https://www.coindesk.com/business/2022/03/25/coinbase-to-require-recipient-information-for-crypto-transfers-from-users-in-canada-singapore-and-japan/) users in Canada, Singapore and Japan will need to provide recipient info when required by regulations
- [EU committees voted](https://twitter.com/paddi_hansen/status/1509536318585454597) to extend AML requirements to crypto, includes unhosted wallets & remove EUR 1000 floor, not final legislative stage
- US derivatives exchange [CME Group](https://www.cmegroup.com/markets/cryptocurrencies/micro-bitcoin-and-micro-ether-options.html) adds options on Micro Ether futures
- Arthur Hayes: [$10k prediction for ETH](https://cryptohayes.medium.com/five-ducking-digits-cd92a7ab72ce); switches to 75% ETH/25% BTC

**General**

- Vitalik: [defense of maximalism](https://vitalik.ca/general/2022/04/01/maximalist.html) \[posted April 1\]
- Chrome [zero day exploit](https://twitter.com/stocksmencarl/status/1507832895590879243), attackers could inject own JavaScript
- KYC considered harmful: [fake emergency data requests](https://krebsonsecurity.com/2022/03/hackers-gaining-power-of-subpoena-via-fake-emergency-data-requests/) used to subpoena customer data
- [Discord bookmarklet attack](https://twitter.com/v1punks/status/1508863426247995401): JavaScript gets Discord auth token from local storage and sends via a webhook to the attacker
- Remco’s intro to [approximation theory](https://xn--2-umb.com/22/approximation/index.html)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-april-2-2022](https://weekinethereumnews.com/week-in-ethereum-news-april-2-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- **Apr 4 – [DeFi22](https://www.bis.org/events/220404_defi.htm) conference for central bankers (Zurich - livestream only)**
- Apr 7-9 – [ETH Portland](https://2022.ethportland.com/) hackathon
- Apr 8-10 – [DAOHacks](https://dao.ethglobal.com/) (hackathon & summit)
- Apr 18-25 – [Devconnect](https://devconnect.org/schedule) (Amsterdam)
- Apr 22 – deadline for [EF academic grants round](https://esp.ethereum.foundation/academic-grants)
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETH NYC](https://nyc.ethglobal.co/)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 6-9 – [MCON 2](https://twitter.com/mcon_world/status/1504175505389457410) (Denver)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

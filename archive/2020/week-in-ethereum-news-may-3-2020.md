---
title: "Week in Ethereum News<BR> May 3, 2020"
date: "2020-05-03"
---

## **Eth News and Links**

**Eth1**

- Latest [core devs call](https://youtu.be/MOZ7_0Tb95M). Tim Beiko’s [notes](https://twitter.com/TimBeiko/status/1256224860788920320). Updates on EIPs for eth2 curve, EVM subroutines. ProgPoW shelved due to clear lack of consensus. Discussion of migrating to binary trie
- [Analysis of EIP-2315](https://ethereum-magicians.org/t/eip-2315-simple-subroutines-for-the-evm-analysis/4229) simple EVM subroutines
- [DHT+SkipGraph for chain and state data retrieval](https://ethresear.ch/t/explorations-into-using-dht-skipgraph-for-chain-and-state-data-retrieval/7337)
- Notes from the [fee market change call](https://twitter.com/TimBeiko/status/1255874207805837313)
- Vitalik’s EIP[1559 fee market change FAQ](https://notes.ethereum.org/Wjr1SnW-QaST7phX9C5wkg?view)

**Eth2**

- Latest [what’s new in Eth2](https://hackmd.io/@benjaminion/wnie2_200501)
- [Schlesi multi-client testnet launched](https://twitter.com/a4fri/status/1254770383506440195) with Lighthouse and (slightly updated) Prysmatic clients. Then [Nimbus joined Schlesi](https://twitter.com/ethnimbus/status/1255804796961001472) a few days later.
- Bitfly has a [Schlesi explorer](https://schlesi.beaconcha.in/)
- [Nimbus client](https://our.status.im/nimbus-update-may-1/) update - up to date, joining Schlesi testnet, RFP for security audits, and benchmarking Nimbus on a 2018 midrange phone
- Update from ConsenSys’s [TXRX team](https://hackmd.io/@353yQn6WTImF5o12LQXXfQ/H1yRS6tt8): [prkl](https://github.com/prrkl) network monitoring tool, verifiable precompiles, cross-shard tx simulator, fork choice testing, discv5 sim, and work on turning off proof of work.
- A step-by-step guide on joining Prysmatic’s [Topaz testnet for Windows10 and MacOS](https://kb.beaconcha.in/tutorial-eth2-multiclient)
- ConsenSys’s high-level [eth2 FAQ](https://consensys.net/knowledge-base/ethereum-2/faq)

**Layer2**

- [Channels funding channels](https://blog.statechannels.org/channels-funding-channels/): how state channels reduce latency and onchain transactions

### This newsletter is made possible by [Chainlink](https://chain.link/)!

- ![](https://weekinethereumnews.com/wp-content/uploads/2020/05/FE39n5_g.png)

Decentralized oracles are a key capability enabling smart contracts to reach their full potential. Come work with the leading team providing [oracles for Ethereum](http://feeds.chain.link/). Join us to help build the next generation of smart contracts in roles including [Software Engineering](https://careers.chain.link/o/senior-software-engineer-remote-new-york), [Developer Evangelism](https://careers.chain.link/o/developer-evangelist-global), [DevOps](https://careers.chain.link/o/site-reliability-engineer-global), [Product Management](https://careers.chain.link/o/product-manager-blockchain-integrations), and [more](https://careers.chain.link/). 

**Stuff for developers**

- buidler [v1.3](https://github.com/nomiclabs/buidler/releases/tag/v1.3.0) - test time-based cases in Buidler EVM, works with TheGraph
- [Waffle’s plan for making testing better](https://medium.com/ethworks/smart-contracts-testing-still-sucks-how-want-to-make-it-better-7c38d5ce7fc9) with v3
- [Testing with Python and Brownie](https://medium.com/@iamdefinitelyahuman/ethereum-mainnet-testing-with-python-and-brownie-82a61dee0222)
- Typechain [v2](https://github.com/ethereum-ts/TypeChain/releases/tag/v2.0.0) - Typescript bindings. truffle v5 support, natspec
- Solidity docgen [v0.5](https://forum.openzeppelin.com/t/solidity-docgen-0-5/2745) - documentation generation for Solidity project
- [Running async/await scripts in Remix](https://medium.com/remix-ide/running-js-async-await-scripts-in-remix-ide-3115b5dd7687) IDE
- Austin Griffith’s [scaffold-eth](https://medium.com/@austin_48503/building-on-ethereum-in-2020-dca52eda5f00), a toolkit to prototype and win hackathons
- A [linked hashmap in Solidity](https://github.com/cfelde/AKAP-utils/blob/master/contracts/collections/LinkedHashMap.sol)
- How to add [proxy Ethereum addresses to BigQuery](https://medium.com/@ASvanevik/how-to-add-proxy-ethereum-addresses-to-bigquery-d842ed001449)
- Authereum’s [batched transactions API for interest rate arbs](https://medium.com/authereum/how-to-make-your-own-defi-protocol-without-writing-a-smart-contract-a820a90d9124)
- [discv5 feasibility study for Status](https://vac.dev/feasibility-discv5)
- Tutorial to [testing on mainnet fork with Ganache, Jest and Uniswap](https://studydefi.com/testing-on-mainnet/)
- [Etheroll security issue](https://www.reddit.com/r/etheroll/comments/g7zrvz/contract_is_currently_in_lockdown_mode_all_funds/): hacker monitoring for onchain forks and then uses that info to frontrun transactions. Novel (to me!) hack
- Dragonfly releases an [oracles tracker](https://oracles.club/)
- Synthetix CTO [Justin Moses on 10 things they did to improve their Ethereum development experience](https://blog.synthetix.io/the-opsec-and-developer-sprint/). tldr: Buidler, Slither, TheGraph, and Tenderly.

**Ecosystem**

- Contribute to the [TornadoCash trusted setup ceremony](https://ceremony.tornado.cash/). It takes about 5 secs of clicking and requires you to leave the browser tab open a few minutes.
- Multisigs controlling multisigs: [Avsa’s vision for a usable web3](https://medium.com/universal-ethereum/turtles-all-the-way-down-multisigs-owning-multisigs-485a488d571e)
- [Renew your ENS names](https://medium.com/the-ethereum-name-service/the-great-renewal-its-time-to-renew-your-eth-names-or-else-lose-them-afccea4852cb) or you will lose them. Names start to expire May 4th

**Enterprise**

- Hyperledger Besu [v1.4.4](https://github.com/hyperledger/besu/releases/tag/1.4.4), added priv\_getLogs, added Splunk integration

**Governance, DAOs, and standards**

- Governance processes for Maker and Compound add [WBTC to Maker](https://blog.makerdao.com/wtbc-approved-as-collateral-by-maker-governance-generate-dai-now-with-bitcoin) and [USDT to Compound](https://twitter.com/compoundfinance/status/1256319568059838464). [TBTC also proposed for Maker](https://forum.makerdao.com/t/tbtc-proposal-for-collateral-onboarding-tbtc/2328)
- Maker’s [MIPs ratification vote is live](https://blog.makerdao.com/the-maker-improvement-proposals-mips-ratification-vote-is-live/)
- [MetaClan](https://medium.com/metaclan/metaclan-rises-14cf2dad1b79): DAOs for in-game coordination
- [ERC2611](https://github.com/ethereum/EIPs/pull/2619): Geotimeline Contact Tracing Data Standard
- [Last call](https://github.com/ethereum/EIPs/blob/d13308adac628b50234bae656a78f5fba497ac72/EIPS/eip-1363.md): ERC1363 Payable Token
- [Last call](https://github.com/rekmarks/EIPs/blob/94a76302c1ce52697259d04ac3006b941fb66333/EIPS/eip-1193.md): EIP1193 Eth provider Javascript API
- [ERC 2612](https://github.com/ethereum/EIPs/blob/16734786193cee40637f68cabcfcfb5a01ece33e/EIPS/eip-2612.md): permit, 712-signed approvals
- [EIP2357](https://github.com/ethereum/EIPs/pull/2622/files): Total difficult in block header

**Application layer**

- [DeFiZap and DeFiSnap merged to be ZapperFi](https://twitter.com/DeFi_Zap/status/1256170281695162368): now track and trade your DeFi together
- [Gnosis Safe apps](https://blog.gnosis.pm/introducing-gnosis-safe-apps-faef908f69c6): interact with apps straight from the Gnosis Safe interface
- [dforce/lendfme plan post-hack](https://medium.com/dforcenet/lendf-me-resolution-part-ii-dforce-better-future-proposal-76a07b65ca24): user airdrop, dSAFU insurance fund, large bug bounty
- OpenBazaar now [supports Eth](https://twitter.com/brianchoffman/status/1256337841132470273)
- A rough [proposal for a GasToken forward](https://www.reddit.com/r/ethereum/comments/g8uz30/gasevo_embedded_volumetric_optionality_forward/)
- [Everest](https://everest.link/): a project registry from TheGraph and MetaCartel

**Tokens/Business/Regulation**

- UMA did an [Initial Uniswap Offering](https://twitter.com/bramanathan/status/1255898154664263682), and there was a 5-10x spike
- It appears Telegram will have to [return $1.2 billion to investors](https://www.coindesk.com/telegram-caves-to-us-regulators-delays-blockchain-launch-offers-to-return-1-2b-to-investors)
- Ideo’s [Simple Agreement for Future Governance](https://medium.com/ideo-colab/meet-the-safg-defis-emergent-framework-for-participatory-investing-and-protocol-development-62286a576fb5) for DeFi
- Auditing the 10k top Eth addresses: [ETH is better distributed than BTC](https://medium.com/@adamscochran/the-10k-audit-42c100dd32bb) and a bunch of other interesting claims

**General**

- [EtherScan Connect](https://info.etherscan.com/etherscan-connect-a-beginning/): an alpha for mapping addresses with a leaderboard
- a16z raises [$515m crypto fund](https://a16z.com/2020/04/30/crypto-fund-ii/)
- Vitalik’s [review of Gitcoin grants round 5](https://vitalik.ca/general/2020/04/30/round5.html)
- [SuperMarlin](https://medium.com/zengo/supermarlin-adding-transparency-to-marlin-using-1k-lines-of-code-4ed96c514800): no trusted setup with DARK polynomial commitment

* * *

## Housekeeping

[First issue post-ConsenSys](https://twitter.com/evan_van_ness/status/1256336908197732352). As a reminder, this newsletter is and has always been 100% owned by me.

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-may-3-2020/](https://weekinethereumnews.com/week-in-ethereum-news-may-3-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **May 6-20 - Gitcoin’s [virtual hackthon](https://gitcoin.co/hackathon/new-york-blockchain-week/?tab=hackathon:20)**
- May 8-9 - [Ethereal Summit](https://www.etherealsummit.com/) (NYC)
- May 22-31 - [Ethereum Madrid](https://ethereummadrid.com/hackathon-2020-update/) public health virtual hackathon
- May 29-June 16 - [SOSHackathon](https://soshackathon.com/)
- June 17 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

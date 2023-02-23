---
title: "Week in Ethereum News<BR> April 19, 2020"
date: "2020-04-19"
---

## **Eth News and Links**

**Eth1**

- Geth [v1.9.13](https://www.reddit.com/r/ethereum/comments/g2ami2/geth_v1913_drossix_blue_snapshot_format_large_txs/), with dynamic state snapshots if you use the flag
- Nethermind [v.1.8.1](https://github.com/NethermindEth/nethermind/releases/tag/1.8.1) - receipts, bodies and state can be synced in parallel. WebSockets and HTTP run on same port
- Latest [core devs call](https://youtu.be/KlzwFLOj6Bw?t=367). [Beiko’s notes](https://twitter.com/TimBeiko/status/1251143420497719298). Progress and discussion on EIPs for Berlin.
- Quilt doc on [account abstraction implementation plan](https://hackmd.io/y7uhNbeuSziYn1bbSXt4ww?view)

**Eth2**

- Prysmatic launches the [Topaz testnet](https://medium.com/prysmatic-labs/introducing-topaz-testnet-8e8a4e00a700), ready for multi-client testnet
- Chainsafe’s Lodestar client in TypeScript [releases initial audit report](https://medium.com/chainsafe-systems/lodestar-initial-audit-passes-with-flying-colours-397d0ecaee3b) from Least Authority
- Latest [what’s new in Eth2](https://notes.ethereum.org/@ChihChengLiang/Sk8Zs--CQ/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200417?type=book)
- Latest [eth2 call](https://www.youtube.com/watch?v=aEJ9Pw7yFYM&feature=youtu.be&t=57), lots of talk of API standardizations. Ben’s [notes](https://hackmd.io/@benjaminion/HJ-2vo2DU)
- Proto’s [eth2fastspec](https://github.com/protolambda/eth2fastspec), an optimization for transition speed to the spec
- An update to [add atomicity to cross-shard transfers at EE level](https://ethresear.ch/t/atomic-asynchronous-cross-shard-user-level-eth-transfers-over-netted-ee-transfers/7277)

**Layer2**

- When [DeFi meets rollup](https://bankless.substack.com/p/when-defi-meets-rollup), how rollup chains will work together

**Stuff for developers**

- [Writing your first zk proof](https://blog.iden3.io/first-zk-proof.html) with circom and snarkjs from Iden3
- Brownie [v1.7](https://github.com/iamdefinitelyahuman/brownie/releases/tag/v1.7.0) - (python-based dev/testing framework). easy CLI github/EthPM package install. And a quick walkthrough of using [OpenZeppelin contracts with Brownie](https://medium.com/@iamdefinitelyahuman/using-openzeppelin-contracts-with-python-and-brownie-ff7053d63bbe)
- Remix online and desktop IDE [v0.10](https://medium.com/remix-ide/remix-ide-0-10-0-release-88c25d1d997) - more e2e tests, dev node in browser, plugin improvements, publish to IPFS, async/await for script execution 
- OpenZeppelin test environment [v0.1.4](https://forum.openzeppelin.com/t/openzeppelin-test-environment-0-1-4-ganache-fork/2668)
- [dshackle](https://github.com/emeraldpay/dshackle) - Eth API load balancer
- [Flash mintable asset backed tokens](https://forum.openzeppelin.com/t/flash-mintable-asset-backed-tokens-a-new-defi-primitive/2671)
- [Upload to IPFS directly from ENS manager](https://medium.com/the-ethereum-name-service/upload-to-ipfs-directly-from-the-ens-manager-with-new-tool-ac055db5d2fe) with Temporal
- How [MeTokens personalizes with 3Box](https://medium.com/3box/how-stakeonme-uses-3box-to-personalize-metokens-b46a2d049d35) Profiles
- Loopring [launches an API](https://medium.com/loopring-protocol/loopring-exchange-launches-api-ea7dba7f8718) for their dex rollup
- [Patterns for access control](https://medium.com/coinmonks/proposing-future-ethereum-access-control-72e56e14e68e) in Solidity
- [money-legos](https://money-legos.studydefi.com/#/quickstart): tool to build DeFi apps

**Security and ERC777 attacks**

- Sebastian Bürgel finds a [bug cancelling the transaction in the Multis UI](https://medium.com/hoprnet/easterhack-the-unbreakable-gnosis-multisig-with-multis-4eda296500d2)
- Certora on a [Synthetix reentrancy bug](https://www.certora.com/blog/reentrancy.html) they found
- Slither [v0.6.11](https://github.com/crytic/slither/releases/tag/0.6.11) - support for Solidity v0.6, auto-generate properties for unit tests and fuzzer
- Curve found a [vulnerability in the Curve sUSD code](https://twitter.com/CurveFinance/status/1251987199320395781). Funds are safe.
- Two ERC777 re-entrancy attacks this weekend. ERC777 is widely known to be vulnerable to reentrancy attacks, something [ConsenSys Diligence highlighted in the Uniswap audit](https://github.com/ConsenSys/Uniswap-audit-report-2018-12#31-liquidity-pool-can-be-stolen-in-some-tokens-eg-erc-777-29) and on which [OpenZepplin published an exploit](https://blog.openzeppelin.com/exploiting-uniswap-from-reentrancy-to-actual-profit/) on last summer
- Thus a Uniswap market for imBTC (ERC777) got drained for ~1300 ETH with reentrancy and then lendFme also got drained for $25m USD by the attacker tricking the code into believing more had been deposited than actually had. [Peckshield has a solid writeup](https://medium.com/@peckshield/uniswap-lendf-me-hacks-root-cause-and-loss-analysis-50f3263dcc09). The losers are the liquidity providers, and dForce which had the entirety of its liquidity drained.

**Ecosystem**

- [Quarterly update from each EF team](https://blog.ethereum.org/2020/04/14/ef-supported-teams-research-and-development-update-2020-pt-1/)
- What is still lacking to [replace WeChat with web3](https://vac.dev/wechat-replacement-need)?
- [Transaction fees > uncle rewards](https://twitter.com/ankitchiplunkar/status/1250107352323362817) for miners in March 2020. Obviously Black Thursday's transaction fee spike contributed to this

**Enterprise**

- EY releases [OpsChain, v4](https://www.reddit.com/r/ethfinance/comments/g1ap0r/ey_opschain_product_update_notice_opschain/), new SaaS model for public/private chains
- Study of [key management systems for enterprise](https://medium.com/@corgi.desu/a-study-on-blockchain-key-management-systems-part-1-a668eedee058)
- How the [Baseline Protocol synchronizes between different systems of record](https://medium.com/baselineprotocol/say-hello-to-the-baseline-protocol-6f1d6dc9dec7)
- [Using Baseline Protocol](https://medium.com/baselineprotocol/baselining-a-medical-test-covid-19-e24cdf79ac81) for medical tests

**Governance, DAOs, and standards**

- Compound’s [decentralized governance launches](https://medium.com/compound-finance/compound-governance-decentralized-b18659f811e0)
- [EIP2585](https://github.com/ethereum/EIPs/blob/0d7835c4258ad2887f781de1f4f8bd88b5423e21/EIPS/eip-2585.md): Minimal Native Meta Transaction Forwarder
- Austin Williams mentions this [2002 Microsoft Research paper on Sybil resistance](https://twitter.com/onewayfunction/status/1250890427739193350)

**Application layer**

- A guide to the [shutdown of Maker’s SAI](https://blog.makerdao.com/a-guide-to-single-collateral-dai-sai-shutdown/)
- [Play short-deck hold’em with Phil Ivey](https://medium.com/@VirtuePoker/win-a-place-at-iveys-table-3aca09ceaea1) is the new VirtuePoker promo
- Ox opens the [waitlist for Matcha](https://matcha.xyz?id=17V6GD), a “better way to swap tokens”
- First [RocketDAO loan using an ENS name as collateral](https://medium.com/the-ethereum-name-service/the-worlds-first-ens-backed-loan-with-rocket-lp-dao-f24dc4b4019)
- DeFi Saver’s vault protection product [Automation v2](https://medium.com/defi-saver/introducing-automation-v2-now-with-flash-loans-and-next-price-support-433040e6d63b) with flash loans and Maker’s next price
- How MetaCoin is thinking about Nikolai’s [Reflex Bonds idea](https://medium.com/@stefan__ionescu/stability-without-pegs-8c6a1cbc7fbd) for a stablecoin without pegs
- [dYdX crosses 1billion USD](https://twitter.com/dydxprotocol/status/1251349757261262848) in originated loans
- [AtStake](https://atstake.net/), an Eth-based competitor to OpenBazaar. Also: help [test OpenBazaar with Eth](https://twitter.com/brianchoffman/status/1249882656436871170)
- A writeup of [PieDAO’s managed Balancer pools](https://medium.com/piedao/introducing-pie-smart-pools-85a77a2dc22e)
- AtomicLoans lets you [lock up BTC for a Dai/USDC](https://atomic.loans/blog/announcing-public-mainnet-borrowing-launch/) loan. (Get ~9% by lending your Dai/USDC)
- Gnosis launches a [dex protocol with ring trades](https://blog.gnosis.pm/announcing-the-gnosis-protocol-89b3d7794da7) in batch auctions every 5 mins. First app on the protocol is dxDAO’s Mesa, available through mesa.eth

**Tokens/Business/Regulation**

- Another flippening: [value transfer on Ethereum exceeds Bitcoin](https://twitter.com/RyanWatkins_/status/1250427795483684867)
- [7 reasons Eth2 will change the blockchain game](https://medium.com/@adamscochran/7-reasons-eth2-0-will-create-the-next-economic-shift-f689d2f1ec24)
- Swiss Financial Stability Board recommends [heavy stablecoin regulation in response to G20 call](https://www.fsb.org/2020/04/fsb-consults-on-regulatory-supervisory-and-oversight-recommendations-for-global-stablecoin-arrangements/) for stablecoin comments
- Coindesk reports that [China’s Blockchain Service Network will incorporate Ethereum](https://www.coindesk.com/inside-chinas-plan-to-power-global-blockchain-adoption)
- Canada’s [regulatory guidance for crypto exchanges](https://medium.com/coinmonks/canadas-regulatory-guidance-for-cryptocurrency-exchanges-a-good-thing-for-users-and-29ffb9df8841)
- [Bullionix](https://bullionix.io/): mint gold coin NFTs using DGX
- [HashCash v2](https://twitter.com/vaibhavchellani/status/1251261949842649088) - personal token spam protection with auto-decreasing bond
- [me tokens](https://twitter.com/meTokens/status/1249733587479363588), synthetic labor personal tokens on a bonding curve integrated with Moloch/Aragon from Chris Robison. Unfortunately I can’t read the blog post because [Medium censored it](https://twitter.com/evan_van_ness/status/1252012688420614144).
- [DeFi Market Cap](https://defimarketcap.io/), neat way to compare what pools are popular inside of DeFi

**General**

- MyCrypto and PhishFort get [49 malicious Chrome extensions removed](https://medium.com/mycrypto/discovering-fake-browser-extensions-that-target-users-of-ledger-trezor-mew-metamask-and-more-e281a2b80ff9)
- Etherscan’s [ETHProtect](https://info.etherscan.com/ethprotect/), taint inference analysis
- [Shapeshift buys Portis](https://medium.com/shapeshift-stories/making-self-custody-easy-shapeshift-acquires-portis-a9b3bbe63e6b), and will rebrand it as Shapeshift
- Binance is planning a [centralized (DPoS) EVM chain](https://www.binance.com/en/blog/421499824684900520/Binance-Chain-Community-Releases-Whitepaper-for-Enabling-Smart-Contracts)
- [SheFi](https://medium.com/@shefi_org/hello-world-meet-shefi-1f81f01100d8), a DeFi education program aimed at women
- Why so many [South Americans are into DeFi](https://unchainedpodcast.com/the-rise-of-makerdao-a-personal-journey/): “when you believe and know in your heart that nothing is riskier than your government or a bank, any alternative becomes much more enticing”
- The [Eth logo made of Venezuelan bolivars](https://twitter.com/Tompkins_Jon/status/1250901989736644609)

* * *

## **This newsletter is made possible by [ConsenSys](https://consensys.net/)**

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum News. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Apr 21-23 - [EY Global Blockchain Virtual Summit](https://pub.ey.com/public/2019/1911/1911-3312324/global-blockchain-summit/home.html)
- **Apr 24 - EthGlobal’s [HackMoney](https://hackathon.money/) virtual hackathon starts**
- Apr 24-26 - [EthTurin](https://ethturin.com/)
- Apr 29-30 - [SoliditySummit](https://solidity-summit.ethereum.org/) (Berlin)
- May 8-9 - [Ethereal Summit](https://www.etherealsummit.com/) (NYC)
- May 22-31 - [Ethereum Madrid](https://ethereummadrid.com/hackathon-2020-update/) public health virtual hackathon
- June 17 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

---
title: "Week in Ethereum News <BR> August 16, 2020"
date: "2020-08-17"
---

## **Eth News and Links**

**Eth1**

- Geth [v1.9.19](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.19) includes backrunning patch
- Turbogeth [alpha2](https://github.com/ledgerwatch/turbo-geth/releases/tag/v2020.08.02-alpha) release
- [Adding cross-transaction BLS signature aggregation](https://ethresear.ch/t/adding-cross-transaction-bls-signature-aggregation-to-ethereum/7844) to the EVM

**Eth2**

- Medalla experienced instability this weekend as Prysmatic’s client did not [correctly deal with a Cloudflare outage](https://docs.google.com/document/d/11RmitNRui10LcLCyoXY6B1INCZZKq30gEU6BEg3EWfk/edit#heading=h.d5qpimbr9o7y) and then [local storage got deleted in an emergency hotfix](https://twitter.com/terencechain/status/1294637848029585409). If you’re running Prysm, [update to latest version and restart node](https://github.com/prysmaticlabs/prysm/releases/tag/v1.0.0-alpha.22).
    - This is why we testnet - remove unnecessary dependencies like Cloudflare, test failure modes, find bugs.
- This instability showed why Eth2 **needs and incentivizes** client diversity. Here’s some guides to running [Teku (Somer Esat)](https://medium.com/@SomerEsat/guide-to-staking-on-ethereum-2-0-ubuntu-medalla-teku-170e2c52bd23), [Nimbus](https://www.coincashew.com/coins/overview-eth/guide-how-to-stake-on-eth2-with-nimbus) (CoinCashew), [Lighthouse](https://gist.github.com/Larrypcdotcom/fcd4e79c2cf02ce37ec6ed9797beca2c) (larrypc), or [Lodestar](https://www.coincashew.com/coins/overview-eth/guide-how-to-stake-on-eth2-with-lodestar) (CoinCashew).
    - _Editorial reminder: it is a staker’s_ incentivized _duty to run stable clients with minority share of the network_
    - If you’re looking for support as a staker, check out the [Ethstaker subreddit](https://www.reddit.com/r/ethstaker/) or [their discord](https://discord.com/invite/6fJw9qG).
- [Formally verifying the eth2 spec](https://consensys.net/blog/blockchain-development/formally-verifying-the-ethereum-2-0-phase-0-specifications/) in Dafny
- [Nimbus client](https://our.status.im/medalla-update/) update on improving attestation efficiency and switching to blst BLS sigs library
- Danny Ryan’s live [demo of eth1 + eth2 merge](https://youtube.com/watch?v=6iW1MeT-Cug%E2%80%A6)

**EIPs/Standards**

- [EIP2878](https://github.com/ethereum/EIPs/pull/2878): Reduce block reward to 0.5 ETH
- [EIP2872](https://github.com/ethereum/EIPs/blob/5a883ed1d738b8153ac69dc57146492b2596d646/eip-halvening.md): Reduce block reward to 1 ETH
- [ERC2876](https://github.com/junderw/EIPs/blob/bd4195448e2e5067c48c320e8c4abd7c8c37835a/EIPS/eip-2876.md): Deposit contract and address standard

**Layer2**

- Hermez zk rollup [auction to be block producer](https://blog.hermez.io/proof-of-donation-keeping-hermez-permissionless-and-giving-back-to-the-community/) with proceeds funding public goods
- Celer’s [State Guardian Network testnet launch](https://blog.celer.network/2020/08/10/state-guardian-network-beta-testnet-launches/)
- Livepeer’s [probabilistic micropayments as pseudo-layer2](https://forum.livepeer.org/t/how-are-livepeers-probabilistic-micropayments-holding-up-with-these-ethereum-high-gas-prices/1127)
- ENS [exploring optimistic rollup style](https://discuss.ens.domains/t/improving-gas-efficiency-of-dns-domain-claims-with-optimistic-verification/189) for DNS domain claims
- [Rollup replay protection](https://ethresear.ch/t/zkrollup-optimistic-rollup-replay-protection/6999)

* * *

### **This newsletter is made possible thanks to [Matcha by 0x](https://matcha.xyz/)!**

![Matcha](https://weekinethereumnews.com/wp-content/uploads/2020/06/matcha-avatar.png)[](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F6bf41fc7-b9e9-46df-9eaf-049d4c4ca96e_280x280.png)

Matcha aggregates liquidity across decentralized exchange networks to offer you the best price on every token swap. [Trade CRV (Curve), along with 25+ other tokens](https://matcha.xyz/), on Matcha today!

* * *

**Stuff for developers**

- MetaMask to [stop injecting window.web3](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7) in November plus Provider API breaking changes
- Truffle [v5.1.39](https://github.com/trufflesuite/truffle/releases/tag/v5.1.39) more Solidity v0.7 support
- How to make [Solidity libraries have state variables](https://dev.to/mudgen/solidity-libraries-can-t-have-state-variables-oh-yes-they-can-3ke9)
- [MaticVigil](https://medium.com/blockvigil/maticvigil-scalable-blockchain-api-for-everyone-2bc09489e602), an API gateway to make it easier to build on Matic
- [Gas saver deployer](https://twitter.com/emilianobonassi/status/1292788283592912896) - contract to deploy contracts that use Chi gas token
- [Value arrays in Solidity](https://medium.com/coinmonks/value-arrays-in-solidity-32ca65135d5b?source=friends_link&sk=3c2aaf53c7f776cf7d636112d311a48d)
- How to [optimize contract size](https://medium.com/coinmonks/how-to-optimize-eth-smart-contract-size-part-1-a393f444a1df)
- [Connecting APIs and contracts](https://blog.chain.link/apis-smart-contracts-and-how-to-connect-them/) with Chainlink
- [zero knowledge proofs for engineers](https://blog.zkga.me/intro-to-zksnarks)
- Opyn’s [post-mortem on last week’s bug](https://medium.com/opyn/opyn-eth-put-exploit-post-mortem-1a009e3347a8)
- For the functional programmers, Victor Maia on [Formality’s ways to improve](https://medium.com/@maiavictor/thoughts-about-formality-69aa730df481)
- a beginners guide to [safely interacting with erc20 tokens](https://soliditydeveloper.com/safe-erc20)
- an [ERC721 subgraph](https://twitter.com/wighawag/status/1293254549092872197)
- Implementing Eth’s [Merkle Patricia Tree](https://medium.com/@chiqing/merkle-patricia-trie-explained-ae3ac6a7e123) to understand it
- How [OpenRelay beat back DOS attacks](https://blog.openrelay.xyz/dos/thursday) from a Syracuse U lab

**Ecosystem**

- Insane gas prices this week, almost entirely above 100 gwei to get any transaction confirmed and reaching more than 300 gwei. Transaction fees reached over 20k ETH per day compared to 13k ETH in block rewards.
    - Sparkpool’s [GasNow predictor](https://www.gasnow.org/) (with API), using their transaction pool
    - If you’re suggesting gas prices for your users (or programmatically sending many transactions), check out [any.sender to automatically bump up gasprice](https://medium.com/anydot/how-well-does-any-sender-cope-during-events-like-yam-wednesday-ef4d30ed279e) for quick and cheap confirmation
- [Devcon Improvement Proposals](https://blog.ethereum.org/2020/08/14/announcing-devcon-improvement-proposals/)
- Here’s how you can use "decentralized Infura" [Pocket Network to replace Infura in Metamask](https://medium.com/pocket-network/making-metamask-highly-redundant-by-relaying-through-pockets-decentralized-ethereum-api-e556002043ad)
- Videos from the [Randomness Summit](https://www.youtube.com/watch?v=661hUozi9oo) and [Edcon2020](https://www.youtube.com/playlist?list=PL6-IF807eaBEqcWtWkNs0tPNbARehnk_8)

**Enterprise**

- US Postal Service [patent application for blockchain voting on Ethereum](https://pdfaiw.uspto.gov/.aiw?docid=20200258338&PageNum=34&IDKey=7A4F4EA40D1F&HomeUrl=http://appft.uspto.gov/netacgi/nph-Parser?Sect1=PTO1%2526Sect2=HITOFF%2526d=PG01%2526p=1%2526u=/netahtml/PTO/srchnum.html%2526r=1%2526f=G%2526l=50%2526s1=20200258338.PGNR.%2526OS=%2526RS=)
- [Performance enhancements in Hyperledger Besu v1.5](https://www.hyperledger.org/blog/2020/08/06/hyperledger-besu-1-5-performance-enhancements)
- [Interview of Coke bottlers using Baseline Protocol](https://youtu.be/7nQl3Nqr1JI?t=496)
- Paul Brody: [Enterprises Would Use DeFi, if It Weren’t so Public](https://www.coindesk.com/brody-defi)

**Application layer**

- [6 billion in DeFi](https://twitter.com/tayvano_/status/1295020525949878272) (though we’ve always known there is [double counting](https://twitter.com/damirbandalo/status/1295089928901140481)). 1 billion reached by [Aave](https://twitter.com/StaniKulechov/status/1294309152999845888) and [Curve](https://www.theblockcrypto.com/linked/75014/curve-becomes-third-defi-protocol-to-hit-1-billion-in-total-value-locked). [420m+ DAI](https://daistats.com/), [100k eth in Nexus Mutual](https://twitter.com/richardchen39/status/1294320288444948481)
- [Ponzi-like](https://blog.rotki.com/2020/08/13/sustainable-defi/) YAM [launched with unaudited code](https://medium.com/@yamfinance/yam-finance-d0ad577250c7), got to 600m in value, subsequently a bug froze 750k; it went down and is [back to 400m](https://yam.zippo.io/) per the Zippo dashboard. The YAM token went to $160, and is now under a dollar. [Migration to v2](https://medium.com/@yamfinance/yam-migration-faq-57c705688fe6)
- “no premine” similar to YAM became a thing: [based](https://www.coindesk.com/defi-degens-gaming-ethereum-money-legos), [meme](https://decrypt.co/38887/an-anti-meme-coin-joke-just-led-to-a-1-2-million-meme-coin), etc
- CurveDAO had a [performance art type of launch](https://twitter.com/CurveFinance/status/1294089573673455617) which led to pre-mine accusations
- [Aave v2](https://medium.com/aave/aave-v2-the-seamless-finance-d52075d97a70): 1 transaction repayment, governance with AAVE, fixed rate deposits, cheaper gas, etc
- MolochDAO [v2.x](https://medium.com/lexdaoism/introducing-moloch-dao-v2x-mystic-ethereum-contract-upgrades-c7984801d4db) - gas efficiency, wrapped token for voting, accepts ETH
- Status adds [images, audio messages and emoji reactions](https://our.status.im/v1-5-release-keycard-integration-and-notifications-for-android/)
- [Dodoex](https://medium.com/dodoex/dodo-a-revolution-in-on-chain-liquidity-7bc339b9d391), where the market maker curve is flatter near market price
- 1inch [launches Mooniswap](https://medium.com/@1inch.exchange/1inch-revolutionizes-automated-market-maker-amm-segment-with-mooniswap-e068c20d94c), where liquidity providers earn part of the impermanent loss through delayed price updating over 5 minutes

**Tokens/Business/Regulation**

- [cryptofees.info](https://cryptofees.info/) - easy tracker for which chains have any usage (hint: Uniswap v1 and Uniwap v2 both have more usage than any chain other than ETH and BTC)
- Fred Ehrsam: [crypto native insurance](https://www.fehrsam.xyz/blog/crypto-native-insurance-defi)
- Paris Hilton did an [NFT for Cryptograph](https://twitter.com/ParisHilton/status/1293751662536884224)
- [BBC licenses Dr Who](https://www.coindesk.com/doctor-who-to-enter-the-cryptoverse-as-bbc-plans-trading-card-game-on-ethereum-blockchain) for Eth-based trading card game
- Bloxroute [opens service for traders](https://medium.com/bloxroute/announcing-bloxroute-for-eth-defi-7db23e3db4c5)
- Rumored [JPMorgan deal to invest in ConsenSys](https://www.theblockcrypto.com/daily/74687/jpmorgan-consensys-investment-deal)
- BTC [migrating to Ethereum faster than it’s being mined](https://www.coindesk.com/wrapped-bitcoin-tokenized-faster-mined-defi)

**General**

- MyCrypto [launches memberships](https://medium.com/mycrypto/to-a-safer-more-sustainable-mycrypto-c3068bc75259) and protected transactions
- How [malicious Tor relays are exploiting users](https://medium.com/@nusenu/how-malicious-tor-relays-are-exploiting-users-in-2020-part-i-1097575c0cac) to steal BTC
- Everything you need to know about total ETH issuance from [Andreas](https://twitter.com/aantonop/status/1292877311570857990) & [Jay Rush](https://github.com/Great-Hill-Corporation/trueblocks-core/blob/develop/src/other/issuance/README.md)
- Bitmex [adds KYC](https://blog.bitmex.com/announcing-the-bitmex-user-verification-programme/). Dexes everywhere celebrate.
- Andreas Antonopoulos [dexes q&a video](https://www.youtube.com/watch?v=ugPa1r2OdIU)

* * *

## **Job Listings**

- [Dune Analytics](https://careers.duneanalytics.com/): hiring 1st non-founder team members - remote ~CET time zone
- Nethermind is hiring a [Senior .NET Developer](https://justjoin.it/offers/nethermind-senior-net-engineer) (remote)
- The Raiden team is hiring a [comms and growth manager](https://angel.co/company/brainbot-group/jobs/549199-communications-and-growth-manager) in Berlin
- Trail of Bits: [blockchain security engineers](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & [senior software engineers](https://jobs.lever.co/trailofbits/4fec3724-6ecb-4517-a092-5f9c12a60fc6)
- Celer Network: [Android developer](https://www.celer.network/career.html)
- 0x is hiring devs: [full-stack, back-end, and front-end](https://0x.org/about/jobs)
- [Product Managers](https://careers.smartcontract.com/o/product-manager-chainlink-core) wanted to drive Chainlink’s exciting roadmap

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH/DAI/USDC to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **Available Week in Eth News sponsor slots tokenized as $EVAN**

To make my [tokenized available sponsorship slots ($EVAN) for this newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer), you can now buy them directly from me at the spot price on [Balancer](https://balancer.exchange/#/swap/ether/0x89E3aC6Dd69C15e9223BE7649025d6F68Dab1d6a).

Follow me on twitter: [@evan\_van\_ness](https://twitter.com/evan_van_ness) 

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-16-2020/](https://weekinethereumnews.com/week-in-ethereum-news-august-16-2020/)

Did you get **forwarded** this newsletter? **[Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Aug 28-29 - Chainlink’s [Smart Contract Virtual Summit](https://www.smartcontractsummit.io/)
- Oct 2-30 - [EthOnline hackathon](https://www.ethonline.org/)
- Nov 6-7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)
- **Nov 16 - [MetaMask Provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7)**

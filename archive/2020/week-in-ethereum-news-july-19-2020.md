---
title: "Week in Ethereum News <BR> July 19, 2020"
date: "2020-07-19"
---

## **Eth News and Links**

**Eth1**

- [Snapshot acceleration](https://blog.ethereum.org/2020/07/17/ask-about-geth-snapshot-acceleration/) in Geth. Part of Péter Szilágyi’s [Ask about Geth series](http://ask-about-geth.xyz/)
- [KV witness](https://medium.com/@mandrigin/kv-witness-8985168537f9), an alternative block witness proposal

**Eth2**

- An [economic review of eth2](https://medium.com/@thomasborgers/ethereum-2-0-economic-review-1fc4a9b8c2d9): how having less than 1% issuance in proof of stake results in greater chain security than proof of work
- Afri’s updated [benchmarking of eth2 client performance](https://github.com/q9f/eth2-bench-2020-07/blob/master/res/2020-07-eth2-bench.pdf)
- Latest [Prysmatic client](https://medium.com/prysmatic-labs/eth-2-0-dev-update-54-so-close-to-official-multi-client-testnet-e4e1873e7c24) update - better memory management, more test coverage
- Latest [Lodestar client](https://medium.com/chainsafe-systems/lodestar-update-12be7e7d3766) update - syncs to Altona, doesn’t stay synced yet
- [Lodestar tooling](https://lodestar.chainsafe.io/) - BLS keygen, Simple Serialize, ENR decoder
- RuntimeVerification [formally verified safety and liveness with Coq in the beacon chain](https://runtimeverification.com/blog/formally-verifying-finality-in-gasper-the-core-of-the-beacon-chain/)
- A minimum [polynomial commitment scheme](https://ethresear.ch/t/a-minimum-viable-kzg-polynomial-commitment-scheme-implementation/7675) implementation
- How to run the [eth2 fuzzer](https://kb.beaconcha.in/beacon-fuzzer) and make eth2 more secure
- The incentives to [stake your own eth](https://our.status.im/case-for-running-your-own-validator/): don’t need to be online as much, less likely to be slashed

**Layer2**

- [Zkopru](https://ethresear.ch/t/zkopru-zk-optimistic-rollup-for-private-transactions/7717) - an optimistic rollup using zk proofs for 100 private transactions per second. Live on testnet, supports ETH, ERC20, and ERC721 tokens
- Against PoS for [leader election in rollups](https://ethresear.ch/t/against-proof-of-stake-for-zk-op-rollup-leader-election/7698/2)
- [Mass migration to prevent user lockin in rollups](https://ethresear.ch/t/mass-migration-to-prevent-user-lockin-in-rollup/7701)
- Matic does [7200 tps on testnet](https://blog.matic.network/7200-tps-achieved-on-matic-networks-counter-stake-testnet/)

* * *

### **This newsletter is made possible thanks to [Matcha by 0x](https://matcha.xyz/?id=weekinethereum2)!**

![Matcha](https://weekinethereumnews.com/wp-content/uploads/2020/06/matcha-avatar.png)

[](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F6debaee4-eb5a-48b3-89a6-0cc42b9244cb_280x280.png)

Take a sip of Matcha and relax knowing you'll get the best price on every token swap, as [Matcha](https://matcha.xyz/?id=weekinethereum2) aggregates liquidity from 0x, Uniswap, Kyber, Curve, the leading RFQ market makers & more

* * *

**Stuff for developers**

- snarkJS [v3](https://github.com/iden3/snarkjs): native WASM, BN128 and BLS12-381 support, works in nodejs and browser
- Brownie [v1.10](https://github.com/eth-brownie/brownie/releases/tag/v1.10.2) with expanded call traces
- Remix IDE [v0.10.3](https://medium.com/remix-ide/remix-ide-version-0-10-3-release-ff646470d4b7) - unit testing plugin refactored
- Intro to [building with Eth and USDC](https://blog.coinbase.com/introduction-to-building-on-defi-with-ethereum-and-usdc-part-1-ea952295a6e2)
- Factories: [deploy contracts within contracts](https://soliditydeveloper.com/clonefactory) easily and efficiently
- Austin Griffith’s [Scaffold-eth tutorial for beginners](https://www.youtube.com/watch?v=ShJZf5lsXiM): see your frontend with your Solidity code
- Dapphero tutorial on [connecting your frontend with just html](https://www.youtube.com/watch?v=E0guSeAlJFk&feature=youtu.be)
- [OKCoin provides signed price feed as free API endpoint](https://blog.okcoin.com/2020/07/15/supporting-defi-with-the-okcoin-oracle/) conforming to Compound’s Open Price Feed
- [Delegation and voting in Compound](https://medium.com/compound-finance/delegation-and-voting-with-eip-712-signatures-a636c9dfec5e) with EIP712 sigs
- Use the [Diamond proxy standard to get around max contract size limit](https://dev.to/mudgen/ethereum-s-maximum-contract-size-limit-is-solved-with-the-diamond-standard-2189)

**Ecosystem**

- ENS will have a [decaying price premium](https://medium.com/the-ethereum-name-service/new-decaying-price-premium-for-newly-released-names-72080a650c15) for newly released names on Aug 2
- [Fees.wtf](https://fees.wtf/) - frontend that tells you how much you’ve spent on gas
- Camila Russo’s [Infinite Machine](http://www.harperbusiness.com/book/9780062886149/The-Infinite-Machine-Camila-Russo/) book on early Eth history came out this week

**Enterprise**

- Quorum [v2.7](https://github.com/jpmorganchase/quorum/releases/tag/v2.7.0) - add new members to private contracts, protect JSON RPC APIs interface
- Hyperledger Besu [v1.5](https://github.com/hyperledger/besu/releases/tag/1.5.0) - better mining support, better tracing, plugin API block events
- Singapore’s [Project Ubin phase 5](https://www.mas.gov.sg/-/media/MAS/ProjectUbin/Project-Ubin-Phase-5-Enabling-Broad-Ecosystem-Opportunities.pdf?la=en&hash=91091CAD39265C03FF7A4253E70FBEE6D1177714): “successful development of a domestic multi-currency payments network prototype.” Built on Quorum

**Standards**

- [EIP2780](https://github.com/lightclient/EIPs/blob/ea6bc2f911f7eaecfb86cdb48706c5de37577611/EIPS/eip-2780.md) - make ETH send cost 16360 gas instead of 21000
- [ERC725](https://github.com/ethereum/EIPs/blob/49130f7b190edc34f68e887d8485f28e4f987388/EIPS/eip-725.md) v2 - contract based account with attachable key value store

**Application layer**

- [Otoco](https://medium.com/@Otonomos/otoco-is-live-you-can-now-instantly-form-a-real-world-llc-using-your-ethereum-wallet-f31e1b99fa8): instantly form a Delaware LLC from your Eth wallet
- [Understanding pooled staking](https://medium.com/nexus-mutual/understanding-pooled-staking-a32d1bca843d) in Nexus Mutual which led to substantially more cover being available for popular apps
- Request Network [now has DAI invoices](https://request.network/en/2020/07/14/taking-volatility-out-of-crypto-businesses-with-dai-invoice-payments/) (I used it for the job listing below, it was easy)
- Celer launches [Taito’s classic Bust-a-move game](https://blog.celer.network/2020/07/17/bam/)
- DAI passed [200m minted this week](https://daistats.com/#/). Currently at 220m
- Mashable: [DeFi could become the next big thing in finance](https://mashable.com/article/defi-growing-fast/)

**Tokens/Business/Regulation**

- ETH2 staking: [the birth of a digital bond](https://bankless.substack.com/p/ether-the-birth-of-the-digital-bond)
- On [verifying token-based systems](https://blog.oceanprotocol.com/on-verifying-token-based-systems-c33eca757ecf)
- Why [merchants should accept DAI](https://blog.makerdao.com/why-online-merchants-should-accept-dai-for-crypto-payments/)

**General**

- The most prominent [Twitter accounts got hacked this week in a crude BTC phishing](https://medium.com/mycrypto/the-twitterhack-postmortem-423510de54a1) which shines light on the fact that [Twitter DMs are not e2e encrypted](https://www.eff.org/deeplinks/2020/07/after-weeks-hack-it-past-time-twitter-end-end-encrypt-direct-messages)
- [Nim](https://medium.com/better-programming/a-python-substitute-i-tried-out-the-best-programming-language-youve-never-heard-of-9e29cd1893c0): syntax like python and efficiency like C. Language of the eth2 nimbus client
- [Playing with GossipSub](https://adlrocha.substack.com/p/adlrocha-playing-with-gossipsub) and PubSub playground
- Trivial collisions in [IOTA’s hash function](https://soatok.blog/2020/07/15/kerlissions-trivial-collisions-in-iotas-hash-function-kerl/). A recurring theme
- Matthew Green: [Signal’s questionable decision to rely on SGX](https://blog.cryptographyengineering.com/2020/07/10/a-few-thoughts-about-signals-secure-value-recovery/)

* * *

## **Job Listings**

- The Request team is looking for a fully remote [full stack engineer](https://request-network.homerun.co/blockchain-engineer-1)
- Celer Network: [Android developer](https://www.celer.network/career.html)
- [0x is looking for](https://0x.org/about/jobs) all types of devs: full-stack, back-end, and front-end engineers
- Trail of Bits is looking for an elite [blockchain security engineer](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf)
- Build Chainlink as a [Software Engineer](https://careers.smartcontract.com/o/senior-software-engineer-new-york), [Test Engineer](https://careers.smartcontract.com/o/lead-test-engineer-on-chainlink), or [Product Manager](https://careers.smartcontract.com/o/product-manager-blockchain-integrations)!

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH/DAI/USDC to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **Housekeeping**

Follow me on Twitter [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get the **annotated edition of this newsletter** on Monday or Tuesday. Plus I tweet most of what makes it into the newsletter.

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-july-19-2020/](https://weekinethereumnews.com/week-in-ethereum-news-july-19-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- July 20 - [Fork the World](https://metagame.substack.com/p/fork-the-world-hackathon) MetaCartel hackathon
- **July 21 - [Personal Token (online) Summit](https://www.eventbrite.com/e/personal-token-virtual-summit-tickets-112736656374)**
- July 28 - [Augur v2 launch](https://www.augur.net/blog/v2-launch/)
- July 30 - EEA’s [Ethereum in the Enterprise 2020](https://www.conference.entethalliance.org/) virtual conference
- **July 31-Aug 9 - Colorado Lottery & EthDenver [Game Jam hackathon](https://medium.com/ethdenver/colorado-lottery-ethdenver-announce-first-ever-17-500-gamejam-for-new-lottery-games-54422048deba)**
- Aug 2 - [ENS grace period](https://medium.com/the-ethereum-name-service/the-great-renewal-its-time-to-renew-your-eth-names-or-else-lose-them-afccea4852cb) begins to end
- Aug 28-29 - Chainlink’s [Smart Contract Virtual Summit](https://www.smartcontractsummit.io/)
- Jul9 - Aug30 - [EthPlanet’s Summer Camp](https://www.ethplanet.org/ethereum-summer-camp-2020/) virtual event series
- Oct 2-Oct 30 - [EthOnline hackathon](https://www.ethonline.org/)
- Nov 6-Nov 7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)

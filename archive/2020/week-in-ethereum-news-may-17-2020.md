---
title: "Week in Ethereum News<BR> May 17, 2020"
date: "2020-05-18"
---

## **Eth News and Links**

**Eth1**

- Geth [v1.9.14](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.14) - unindex and save disk space
- [OpenEthereum v3](https://blog.gnosis.pm/whats-ahead-for-the-openethereum-client-43da126921c2). Formerly the Parity client. Support for eth/64, breaking database changes to save disk space. Deprecating light client, auto updater, and private transactions
- cross-client consensus tests [v7](https://www.reddit.com/r/ethereum/comments/gk6g5g/v700_preberlin_hf_release_for_ethereum_consensus/)
- Latest [core devs call](https://www.youtube.com/watch?v=bGgzALuyY3w). Beiko’s [notes from the call](https://twitter.com/TimBeiko/status/1261290618078322689), largely around EIPs for next hard fork, eg: 2315 (evm subroutines), 2537 (precompile for curve in eth2), 2046 (reduce gas for static calls to precompiles) and 2565 (repricing the 198 precompile)
- [EVM+384 bit arithmetic](https://notes.ethereum.org/@axic/evm384-preview) as an alternative to EIP2537’s precompile
- Discussion of a second method for resource accounting alongside gas: [oil from Suhabe Bugrara](https://ethresear.ch/t/oil-adding-a-second-fuel-source-to-the-evm-pre-eip-v1-1/7425), separately formulated as [karma](https://gist.github.com/holiman/8a3c31e459ee1bff04256bc214ea7f14) from Martin Swende. Or a counterproposal from Vitalik: [per account gas limits](https://ethresear.ch/t/counter-proposal-to-oil-karma-per-account-gas-limits/7433)
- The case for [Eth-collateralized tokenized gas](https://ethresear.ch/t/free-the-birds-the-case-for-tokenized-gas/7385) at the protocol level

**Eth2**

- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200515), featuring Ben’s thoughts on timelines
- Latest [eth2 implementer call](https://www.youtube.com/watch?v=7uZtEy0nNbw). Notes from [Ben](https://hackmd.io/@benjaminion/rkzVrp958) and [Mamy](https://gist.github.com/mratsim/6e7d4a05c526cdfe64c588bdcab860e1), targeting June for the multi-client testnet
- Schlesi testnet: [Teku is fully participating](https://twitter.com/PegaSysEng/status/1259890067499352065) and [Nimbus is almost fully syncing](https://twitter.com/protolambda/status/1260921727036657665), though there was a [chain split this weekend](https://pbs.twimg.com/media/EYNlZxbWkAAY1_1?format=jpg&name=small)
- [Proof of custody through occasional checks](https://ethresear.ch/t/a-0-001-bit-proof-of-custody/7409) and slashing
- [Stethoscope](https://github.com/lsankar4033/stethoscope): networking test suite
- Idea from Justin Drake on putting [price feed oracles in eth2](https://ethresear.ch/t/enshrined-eth2-price-feeds/7391) via validators, and a [counter-proposal](https://ethresear.ch/t/counter-proposal-to-enshrined-price-feeds-dual-token-oracles/7437/9) from Vitalik Buterin

**Layer2**

- What are the [true finality guarantees of state channels](https://medium.com/statechannels/do-state-channels-exhibit-instant-finality-ec18153136bc)? Depends on liveness of layer 1 chain

### This newsletter is made possible by [Trail of Bits](https://www.trailofbits.com/)!

[![](https://weekinethereumnews.com/wp-content/uploads/2020/05/2314423-1.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F6414b9bf-bcb9-4c15-8963-393e33521ec0_1876x1128.png)

Trail of Bits recently reported and fixed 12 security issues in projects across Ethereum, some of them critical. Read more about what they were and how they found them in [Bug Hunting with Crytic](https://blog.trailofbits.com/2020/05/15/bug-hunting-with-crytic/).

**Stuff for developers**

- Solidity [v0.6.8](https://solidity.ethereum.org/2020/05/14/solidity-068-release-announcement/), some important bugfixes
- Using [immutables in Solidity v0.6.xx](https://solidity.ethereum.org/2020/05/13/immutable-keyword/)
- Austin Griffith tutorial: [build smart contract wallet with social recovery using React](https://medium.com/@austin_48503/programming-decentralized-money-300bacec3a4f)
- If you haven’t watched Austin’s [wtf is eth.build video](https://www.youtube.com/watch?v=30pa790tIIA), you should. It’s under 3 minutes, funny, and informative.
- Running the [Incubed light client with Python](https://blog.slock.it/incubed-for-python-batteries-included-63b79368d58e)
- OpenZeppelin Contracts v3, but [modified to be safe for upgrades](https://forum.openzeppelin.com/t/openzeppelin-contracts-ethereum-package-v3-0/2852)
- [Mainnet testing with your own node](https://medium.com/@matnad/supercharged-ethereum-main-net-testing-on-your-own-node-with-brownie-eb4cb886de7c) using Brownie
- [headlong](https://github.com/esaulpaugh/headlong): ABI v2 and RLP for the JVM
- [EthPM v3](https://medium.com/@nickg_82582/ethpm-v3-is-coming-500d0edd38c4) - spec for v3 of Eth package manager is in last call
- [12 bugs found by Trail of Bits’ Crytic tool](https://blog.trailofbits.com/2020/05/15/bug-hunting-with-crytic/) using 90+ detectors
- [Verifiable randomness on-chain](https://blog.chain.link/verifiable-random-functions-vrf-random-number-generation-rng-feature/) using the Chainlink VRF

**Ecosystem**

- Tornado.cash finished the [largest trusted setup ceremony to date](https://medium.com/@tornado.cash/the-biggest-trusted-setup-ceremony-in-the-world-3c6ab9c8fffa), operator soon to be set to null
- Some interesting findings in [ConsenSys's eth2 staking survey](https://twitter.com/Consensys/status/1260973572916477958)
- A guide to building with [MACI](https://www.youtube.com/watch?v=sKuNj_IQVYI) - an anti-collusion demo using SNARKs

**Enterprise**

- [Visa patent shows they are building on Ethereum](https://twitter.com/econoar/status/1261359936983855105)
- Where to use the Baseline protocol: [sharing business process automation with counterparties](https://medium.com/baselineprotocol/where-to-use-the-baseline-protocol-f32cf4cf31b4)
- Brave releases [Mjolnir](https://brave.com/mjolnir-tooling-for-bat-apollo/) tool for easy deploying and benchmarking permissioned Eth chains

**Application layer**

- Building on ethtrader’s DONUT, [Reddit unveils community points](https://www.reddit.com/community-points/) for r/fortniteBR and r/cryptocurrency subreddits. At the moment, 9000 wallets created for fortnite and just 2100 for r/cryptocurrency. Currently on Rinkeby testnet with plans to move to mainnet.
- Dfinity’s first Swiss employee Robert Lauko now working on [Liquity stablecoin](https://medium.com/liquity/liquity-decentralized-borrowing-5a4b0eb28efc), low collateralization with algorithmic liquidation via stability pool
- “[Augur v2 core contracts are finalized](https://www.augur.net/blog/augur-v2-deployment-update/) and in a code-freeze state, and the trading UI is undergoing performance testing”
- Aave changes its [interest rate model](https://medium.com/aave/aave-borrowing-rates-upgraded-f6c8b27973a7). Inflection point in the curve now 8% and 90% usage.
- [Kyber hit 1 billion](https://twitter.com/KyberNetwork/status/1260923903657963524) USD worth of trades
- Brave at [14m MAU/5m DAU](https://twitter.com/BrendanEich/status/1260388042101022721)
- [Sai successfully shut down on May 12](https://twitter.com/nanexcool/status/1260240861364924417) and now is redeemable for ETH
- Hasu: the [future of cryptomoney is central banking](https://insights.deribit.com/market-research/the-future-of-money-could-be-discretionary/). An analysis of Maker’s options and decisions
- Utah County (Provo) in Utah offering [marriage licenses certified](http://www.utahcounty.gov/Dept/ClerkAud/DigitalCertCopy.html) with the hash on Eth mainnet
- dydx’s [BTC/USDC perpetual with 10x leverage](https://integral.dydx.exchange/btc-perpetual-contract-market-is-live/) is open to the public, and compares [centralized and decentralized perpetual markets](https://integral.dydx.exchange/comparing-perpetual-markets/)

**Tokens/Business/Regulation**

- [ErisX launches ETH futures](https://medium.com/@erisxinsights/erisx-pioneers-first-u-s-based-ether-futures-contract-9d9e0830212f), physically delivered, monthly and quarterly contracts
- Now [~2300 WBTC on Eth versus 900 BTC on Lightning](https://cointelegraph.com/news/1000-wbtc-minted-today-on-ethereum-dwarfs-entire-lightning-network?utm_source=weekinethereumnews)
- [RAC’s $TAPE launched on Zora](https://bankless.substack.com/p/how-to-buy-tape-on-zora) and went from $20 to $1000. $TAPE is a token redeemable for a special edition cassette of RAC’s latest album. Interesting new model for artists to capture value

**General**

- [JPMorganChase decides to bank Coinbase and Gemini](https://www.wsj.com/articles/jpmorgan-extends-banking-services-to-bitcoin-exchanges-11589281201)
- Wired’s [story on MalwareTech/Marcus Hutchins](https://www.wired.com/story/confessions-marcus-hutchins-hacker-who-saved-the-internet/), from stopping WannaCry to FBI arrest
- the [main idea in HALO](https://hackmd.io/@XYwo0oEXTEGRpej1SQVMlg/HJoqBRL9U) snark construction
- Open cryptography problems: [improving stealth addresses](https://ethresear.ch/t/open-problem-improving-stealth-addresses/7438) and [ideal vector commitment](https://ethresear.ch/t/open-problem-ideal-vector-commitment/7421)

* * *

## **Housekeeping**

Follow me on Twitter [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get the annotated edition of this newsletter, usually forthcoming in a day or so, as well as a real-time source of Eth news.

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-may-17-2020/](https://weekinethereumnews.com/week-in-ethereum-news-may-17-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **May 18 - [Book of Swarm launch](https://swarm-gateways.net/bzz:/launch.bookofswarm.eth/)**
- May 22-31 - [Ethereum Madrid](https://ethereummadrid.com/hackathon-2020-update/) public health virtual hackathon
- **May 26 - last day to apply for [Ethereum India fellowship](https://devfolio.co/blog/announcing-the-devfolio-ethereum-india-fellowship/)**
- May 29-June 16 - [SOSHackathon](https://soshackathon.com/)
- June 17 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

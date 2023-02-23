---
title: "Week in Ethereum News<BR> May 24, 2020"
date: "2020-05-24"
---

## **Eth News and Links**

**Eth1**

- Péter Szilágyi’s [snap sync](https://github.com/ethereum/devp2p/blob/3fe9713658f3b3b56e4e99493c54f313e11b43a0/caps/snap.md), and some [benchmarking of snap vs fast sync](https://twitter.com/peter_szilagyi/status/1263668104493662210)
- [Discovery peer advertisement efficiency analysis](https://hackmd.io/@zilm/BJGorvHzL), also applicable to eth2

**Eth2**

- phase 0 spec [v0.12](https://github.com/ethereum/eth2.0-specs/releases/tag/v0.12.0) - added latest IETF standard. This is THE spec for the eth2 launch, barring any updates for bugs
- [Lighthouse client](https://lighthouse.sigmaprime.io/update-25.html) update - BLS key implementation, under Trail of Bits audit, 300mb RAM to run 2000 validators
- [Lodestar client](https://medium.com/chainsafe-systems/lodestar-project-update-c89b15122c57) update - syncing to both Schlesi and Topaz testnets
- [Prysmatic client](https://medium.com/prysmatic-labs/eth-2-0-dev-update-50-multiclient-testnet-restart-slasher-improvements-f1e9339b1922) update - Schlesi fork post-mortem, slashing client and protection
- Fizzy [v0.1](https://github.com/wasmx/fizzy/releases/tag/v0.1.0) - WASM interpreter written in C++
- Carl Beekhuizen’s [Eth2 keys](https://blog.ethereum.org/2020/05/21/keys/) explainer

**Layer2**

- Fuel does a demo of [Reddit’s community points in an optimistic rollup](https://www.reddit.com/r/CryptoCurrency/comments/gonjm3/tldr_moons_and_bricks_go_brrr/) that reduces transaction fees by 60x
- Loopring to pass [1 million trades on its zk rollup](https://medium.com/loopring-protocol/one-millionth-trade-on-loopring-exchange-a-zkrollup-reward-8b8320d359ba) in just 3 months of being live
- Gazelle (formerly Plasma Chamber) [alpha release](https://gzle.io/blog/Alpha_Release) with an API for deposit, transfer and exit

### This newsletter is made possible by [0x](https://0x.org/)!

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F2f99eb49-8111-4f6a-bc77-3ad2702e3236_3083x1500.png)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F2f99eb49-8111-4f6a-bc77-3ad2702e3236_3083x1500.png)

0x is excited to sponsor Week in Ethereum News and invite readers to try out [our new DEX](https://matcha.xyz/?id=weekinethereum1)!

Sign up [here](https://matcha.xyz/?id=weekinethereum1) to get early access to Matcha, your new home for fast, secure token trading.

**Stuff for developers**

- web3js [v1.2.8](https://github.com/ethereum/web3.js/releases/tag/v1.2.8) with Ethers v5 ABI coder integration, ENS’s contenthash, and EIP-1193’s AbstractProvider
- [Mocking Solidity code](https://medium.com/ethworks/mocking-solidity-smart-contracts-with-waffle-55813b22ebf2) with Waffle
- A writeup of [Solhint v3’s features](https://medium.com/protofire-blog/solhint-v3-0-autofix-support-and-new-integrations-8af3f802b99c)
- How to get [randomness onchain using Chainlink’s VRF](https://medium.com/coinmonks/how-to-generate-random-numbers-on-ethereum-using-vrf-8250839dd9e2)
- [Offchain voting for personal tokens](https://medium.com/@austin_48503/personal-token-voting-73b44a598d8e), tutorial from Austin Griffith
- [Gas and circuit constraint benchmarks](https://ethresear.ch/t/gas-and-circuit-constraint-benchmarks-of-binary-and-quinary-incremental-merkle-trees-using-the-poseidon-hash-function/7446) of binary and quinary incremental Merkle trees using Poseidon
- Loopring’s new [approach to generating frontend keys](https://medium.com/loopring-protocol/looprings-new-approach-to-generating-layer-2-account-keys-4a16cc334906) to sign offchain requests
- Hegic had to [shut down again because of an exploit](https://twitter.com/samczsun/status/1263448198057689089) that Sam Sun reported weeks beforehand
- tBTC found a [bug during their rollout;](https://blog.keep.network/details-of-the-tbtc-deposit-pause-on-may-18-2020-38d7dd555663) launch delayed
- [Matic’s mainnet is in the process of going live](https://blog.matic.network/mainnet-is-going-live-announcing-the-launch-sequence/)

**Ecosystem**

- [Tornado.cash non-custodial mixer is now trustless](https://medium.com/@tornado.cash/tornado-cash-is-finally-trustless-a6e119c1d1c2), with the admin function burned and the frontend available at https://tornadocash.eth.link
- Ethereum Foundation [q1 update](https://blog.ethereum.org/2020/05/19/ethereum-foundation-spring-2020-update/), including how EF thinks about funding
- [Intro to dwebsites](http://blog.almonit.eth.link/2020-05-21/Introduction_to_Dwebsitse.html). dweb = ENS + IPFS (and equivalents)
- [Network usage is at an all time high](https://twitter.com/latetot/status/1264385819135148033). With similar use of the Eth2 chain, Ethereum will have [negative issuance of ETH](https://twitter.com/econoar/status/1263254153599451136) because part of every transaction fee is burned

**Enterprise**

- Using Eth mainnet, [Baseline Protocol privately and securely synchronizes data and business logic](https://oasis-open-projects.org/open-source-proof-of-concept-ethereum-mainnet/) across SAP and Microsoft Dynamics
- Hyperledger Fabric founder John Wolpert’s [common sense statement on using blockchain and Ethereum mainnet](https://medium.com/@jwolpert/a-common-sense-statement-on-blockchain-and-the-business-mainnet-10077d969ab1)
- The [Baseline Protocol as lean strategy](https://www.linkedin.com/pulse/baseline-protocol-lean-strategy-machiel-tesser)
- Depository Trust & Clearing Corporation’s [Project Whitney using Ethereum mainnet](https://www.dtcc.com/~/media/Files/Downloads/settlement-asset-services/user-documentation/Project-Whitney-Paper.pdf) to “support private market securities, from issuance through secondary markets”

**DAOs and Standards**

- Aragon [sues to avoid paying grantee a community-voted grant](https://blog.autark.xyz/autarks-response-to-aragons-statement/)
- Exploring [DAOs as a new kind of institution](https://medium.com/commonsstack/exploring-daos-as-a-new-kind-of-institution-8103e6b156d4)
- MetaCartel is [becoming a DAO incubator](https://medium.com/metacartel/metacartel-is-evolving-%EF%B8%8F-350a64b39f3c)
- [ERC2665](https://github.com/ethereum/EIPs/issues/2665): ERC721 transfer fee extension
- [EIP2666](https://github.com/ethereum/EIPs/blob/bfa0f8618e648fd50b0d8a65cbe2f981ba55a2a1/EIPS/eip-2666.md): Repricing of precompiles and Keccak256 function

**Application layer**

- Uniswap v2 [launched](https://uniswap.org/blog/launch-uniswap-v2/), with [more features](https://uniswap.org/blog/uniswap-v2/) - direct token pairs, price oracles, flash swaps, etc
- UMA launches the [ETHBTC synthetic](https://medium.com/uma-project/ethbtc-synthetic-token-is-live-e3fe2242c2fe) token, so you can bet on The Flippening
- [idle v3](https://medium.com/@idlefinance/idle-v3-0-is-a-live-db568c534a09) - stablecoin yield rebalancer adds dydx, USDT, and a risk-adjusted strategy
- Maker changes [USDC stability fee to .75% and WBTC to 1%](https://twitter.com/MakerDaiBot/status/1264433764287029249). Also, how [Dai became a favorite in Latin America](https://blog.makerdao.com/how-dai-became-a-favorite-crypto-in-latin-america/)
- Argent [launches v1](https://www.argent.xyz/blog/argent_v1_launch/) of smart contract wallet with one touch access to TokenSets,  PoolTogether,  Aave,  Uniswap V2, Compound, Maker and Kyber.

**Tokens/Business/Regulation**

- 5 things [crypto can learn from Visa’s struggle for adoption](https://bankless.substack.com/p/5-ways-crypto-is-like-early-visa) in the 1970s
- [WBTC mints another 1500 BTC](https://www.wbtc.network/dashboard/order-book) on May 21. There’s now 5200 [BTC on Ethereum](https://btconethereum.com/) compared to less than 3000 BTC on Lightning and Liquid combined
- [Blockchain code as antitrust](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3597399), Schrepel and Buterin paper
- [ETH to soon surpass BTC on Bitcoiners’ preferred stock-to-flow](https://www.reddit.com/r/ethfinance/comments/gld5d5/i_calculated_ethereums_stocktoflow_value/) metric
- [Staking will turn Ethereum into a functional store of value](https://www.coindesk.com/staking-will-turn-ethereum-into-a-functional-store-of-value)

**General**

- KYC puts lives at risk: [BlockFi hack](https://blockfi.com/wp-content/uploads/2020/05/Incident-Report-05-14-20.pdf) leaks client name, address, and crypto addresses. Similarly, a hacker claims to have exploited [Shopify for Trezor and Ledger databases](https://twitter.com/underthebreach/status/1264460979322138628), though [Ledger says the databases don’t match](https://twitter.com/Ledger/status/1264506360735174657)
- Using [zero knowledge proofs for vulnerability disclosure](https://blog.trailofbits.com/2020/05/21/reinventing-vulnerability-disclosure-using-zero-knowledge-proofs/)
- World Economic Forum’s [principles for a decentralized future](https://www.weforum.org/communities/presidio-principles) (transparency, self-sovereign data, privacy and accountability)
- JK Rowling jokes about [trolling BTC because of her significant ETH holdings](https://twitter.com/jk_rowling/status/1262332956208762881)
- The Winklevosses say they own a [similar amount of ETH and BTC](https://thedefiant.substack.com/p/winklevoss-twins-say-stablecoins-0f3)
- Brave’s [anti-fingerprinting v2](https://brave.com/whats-brave-done-for-my-privacy-lately-episode-4-fingerprinting-defenses-2-0/), available in the beta releases but coming soon in the main releases

* * *

## **Housekeeping**

Follow me on Twitter [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get the annotated edition of this newsletter, usually forthcoming in a day or so, as well as a real-time source of Eth news.

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-may-24-2020/](https://weekinethereumnews.com/week-in-ethereum-news-may-24-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- May 26 - last day to apply for [Ethereum India fellowship](https://devfolio.co/blog/announcing-the-devfolio-ethereum-india-fellowship/)
- **May 28 - [EIP1559 implementation call](https://github.com/ethereum/pm/issues/174)**
- **May 29 - [core devs call](https://github.com/ethereum/pm/issues/172)**
- May 29-June 16 - [SOSHackathon](https://soshackathon.com/)
- **June 16 - deadline to apply for Gitcoin’s [Kernel incubator](https://gitcoin.co/blog/announcing-kernel/)**

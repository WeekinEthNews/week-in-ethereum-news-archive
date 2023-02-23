---
title: "Week in Ethereum News <BR> September 25, 2021"
date: "2021-09-25"
---

## **Eth News and Links**

**Mainnet execution layer**

- December upgrade proposed as [difficulty bomb delay](https://github.com/ethereum/pm/issues/391#issuecomment-924197948) only, named Arrow Glacier
- Erigon [v2021.09.04](https://github.com/ledgerwatch/erigon/releases/tag/v2021.09.04): reimplements [transaction pool](https://twitter.com/realledgerwatch/status/1441009309685530631) as separable (separate process/computer and multiple processes for one node)
- Nethermind [v1.11.3](https://github.com/NethermindEth/nethermind/releases/tag/1.11.3): performance optimization in JSON-RPC and transactions broadcasting

**EIPs/Standards**

- [EIP3978](https://eips.ethereum.org/EIPS/eip-3978): Gas refunds on reverts
- [EIP4200](https://github.com/ethereum/EIPs/blob/08ee4e11f62399b6566cfe857bae0cd2da387992/EIPS/eip-4200.md): Static relative jumps

**Proof of stake consensus layer**

- If [beacon chain consensus fails](https://www.symphonious.net/2021/09/23/what-happens-if-beacon-chain-consensus-fails/), stakers run the risk of incurring large penalties ([~%75 of their balance](https://www.reddit.com/r/ethstaker/comments/ptm04i/the_financial_incentive_to_run_a_minority_client/)) if they use a majority client/cloud provider/staking service and won’t be bailed out!
- [Client diversity estimate](https://twitter.com/sproulM_/status/1440512518242197516) from block proposal data using block attestation fingerprinting, Prysm is ~65%
- Altair upgrade of the beacon chain set for [epoch 74240](https://github.com/ethereum/consensus-specs/pull/2625/files), October 27
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210924)
- PoS implementers [call](https://www.youtube.com/watch?v=DZiy3RhUgNY&t=36s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/rJ8ddAY7t): sync committee issues resolved
- Proto’s [visualization of debugging](https://twitter.com/protolambda/status/1440799521047412739) performance of 200k+ validators on Prater testnet
- [Wagyu](https://twitter.com/wagyutools/status/1440381746688643089): GUI to create and restore validator keys (offline), testnet only
- [Feist-Khovratovich technique](https://alinush.github.io/2021/06/17/Feist-Khovratovich-technique-for-computing-KZG-proofs-fast.html) for computing KZG proofs fast

**Layer2**

- An exhaustive list of [projects on Arbitrum](https://twitter.com/playtern/status/1439224019295752194) (caveat emptor, as always)
- Avoid long optimistic rollup withdrawal delays: use Celer [cBridge 2.0](https://blog.celer.network/2021/09/22/cbridge-2-0-coherent-blockchain-interoperability-powered-by-the-state-guardian-network/) with improved user experience and LPs have option not to run a cBridge node
- Aztec increases caps to [30 ETH, 100k DAI and 2 renBTC](https://medium.com/aztec-protocol/aztec-2-0-updates-100-000-transaction-limits-more-e55c17c0ecf8) for private transactions on its zk rollup
- Bitfinex directly supports [bridge](https://www.bitfinex.com/posts/710) to DeversiFi (StarkWare-based layer2), starting with USDT
- [Solidity to Cairo transpiler](https://medium.com/nethermind-eth/solidity-on-starknet-terminal-velocity-e8df5f63e010) switched from transpiling EVM opcodes to using a combination of Solidity & Yul AST
- [Censorship resistance](https://twitter.com/bkiepuszewski/status/1440553708295577607): Arbitrum and Optimism users can force transactions to layer1 whilst StarkWare layer2s use app specific mechanisms
- Geohot returns: [cannon](https://github.com/geohot/cannon), on chain interactive fraud prover

* * *

### **This newsletter is made possible thanks to [GridPlus](https://gridplus.io/)’s Lattice hardware wallet!**

![GridPlus](https://weekinethereumnews.com/wp-content/uploads/2021/09/grid-rec-1024x768.jpeg)

What good is a hardware wallet if you can’t be sure of what you’re signing?  

The Lattice is the first and only hardware wallet that _securely_ **shows you a human readable version of an Ethereum transaction**.  Anything else is just security theater.

Just as importantly, the Lattice is the only hardware wallet that is **built to be resistant to physical tampering**.  

We can’t leak your data if we don’t have it: we **never store your name or address even a single day longer** than we have to. 

Isn’t your crypto worth securing?  Buy a [Lattice today](http://www.gridplus.io/?afmc=WeekInEthereumNews).

* * *

**Stuff for developers**

- Ganache [v7.0.0 alpha.1](https://github.com/trufflesuite/ganache/releases/tag/ganache%407.0.0-alpha.1): local blockchain (formerly ganache-cli), London EIP1559 support
- web3.js [v1.5.3](https://github.com/ChainSafe/web3.js/releases/tag/v1.5.3): fix for sending legacy transactions on London networks
- [Discussion](https://twitter.com/solidity_lang/status/1440705334650146822) on whether Solidity libraries should behave like contracts
- [Hardhat Ignition](https://medium.com/nomic-labs-blog/hardhat-ignition-5a34a4e3d2de): deployment system for structuring, automating, and distributing contract deployment setups, in development for 2022
- [eth-hooks](https://github.com/scaffold-eth/eth-hooks) (TypeScript): commonly used hooks such as balances, provider, contract loader and ENS resolver, from scaffold-eth
- [gas-estimation](https://github.com/MyCryptoHQ/gas-estimation): MyCrypto EIP1559 library, uses last 10 blocks from an Ethereum node
- [Moloch v3](https://medium.com/@molochmystics/molochv3-8eb732cd0930) proposal (codenamed Baal): adds Compound-style delegation, DAO controlled share and loot transferability
- [nile](https://github.com/martriay/nile) (for Cairo): compile and manage artifacts for StarkNet projects, install Cairo language
- Guide to create [ERC20 payment splitter](https://medium.com/coinmonks/create-an-erc20-token-payment-splitting-smart-contract-c79436470ccc) using OpenZeppelin & Hardhat
- [Full Knowledge User Proofs](https://medium.com/@sblowpckcr/full-knowledge-user-proofs-working-with-storage-without-paying-for-gas-e124cef0c078): pattern using call data with a user proof than paying gas to read from storage
- Guide to using [GitHub with Remix](https://medium.com/remix-ide/github-in-remix-ide-356de378f7da)
- Beginner: [first Solidity contract](https://stermi.medium.com/how-to-deploy-your-first-smart-contract-on-ethereum-with-solidity-and-hardhat-22f21d31096e) using Hardhat with tests & verification
- MyCrypto’s guide to [creating a profile pic NFT](https://blog.mycrypto.com/so-you-wanna-build-your-own-pfp-nft-project) 

**Security**

- Detection of an [NFT drop](https://twitter.com/_anishagnihotri/status/1440359305341923332), using on chain and off chain information, same was detected for [Time NFTs](https://twitter.com/_anishagnihotri/status/1441072865764429825)
- pNetwork bridge $12 million [exploit](https://medium.com/pnetwork/pnetwork-post-mortem-pbtc-on-bsc-exploit-170890c58d5f), event logs for attack contract processed in error by Rust code on pNetwork’s bridge client, only one BSC bridge exploited

**Ecosystem**

- [MEV impact on gas prices](https://twitter.com/hasufl/status/1439938607142277121), increases for priority gas and during high volatility non-priority gas but reduces the waste from pre-Flashbots
- Proposed [Sign-in With Ethereum workflows](https://blog.spruceid.com/sign-in-with-ethereum-proposed-architecture/)
- [Ethereum culture](https://twitter.com/technocrypto/status/1440350136517808129): don't take ourselves too seriously; differentiator is legibility of research for wider understanding and tech/social infrastructure
- Binance, Gemini, Kraken, Bittrex, Bitstamp, Gate and BlockFi wasting money by still sending [legacy transactions](https://twitter.com/trent_vanepps/status/1441490433419329536) rather than EIP1559
- Twitter thread of [common scams in the NFT ecosystem](https://twitter.com/DCLBlogger/status/1440083759928422401) 

**Enterprise**

- Case for enterprise devs to [deploy to public Ethereum](https://blog.infura.io/3-things-enterprise-developers-should-consider-when-deploying-on-ethereum/?utm_content=180846982&utm_medium=social&utm_source=twitter&hss_channel=tw-761372197298528256): faster setup with lower cost, immutable and composable
- [Crosschain Layered Architecture](https://ethresear.ch/t/crosschain-layered-architecture/10813) (work in progress) to better allow for technology and infrastructure reuse, with greater interoperability
- [Quorum Key Manager](https://consensys.net/quorum/key-manager/), consolidates account and private key management
- [TIMEPieces](https://time.com/collection/timepieces-nft/) (sold out in 1 minute): NFTs include digital TIME magazine subscription

**Application layer**

- [DAI](https://forum.makerdao.com/t/official-dai-token-bridge-now-live-on-arbitrum-one/10438) with custom bridge live on Arbitrum
- [Maker adds Gelato Network’s DAI/USDC Uniswap v3 LP](https://twitter.com/hexonaut/status/1440400852385107975) as collateral, test debt ceiling of 10 million.  Replace the PSM while earning fees
- [Uniswap v3 layer2](https://twitter.com/uniswap/status/1440405518623801357) graduates to beta, adds Optimism and Arbitrum network selector
- [1inch](https://blog.1inch.io/the-1inch-network-expands-to-arbitrum-c0e09bfd7ebf) live on Arbitrum
- Synthetix [deprecating selected synths on layer1](https://blog.kwenta.io/deprecating-synths-on-l1/), transitioning to layer2
- Saddle [virtual swaps](https://blog.saddle.finance/low-slippage-trades-across-saddle-btc-eth-and-usd-pools-via-virtual-swap/), low slippage trades for sBTC, sETH and sUSD
- [Argent](https://www.argent.xyz/blog/an-nft-gallery-for-every-user/) adds personal web page with NFT gallery for wallets
- Snoop Dogg reveals [Cozomo de’ Medici](https://twitter.com/SnoopDogg/status/1440038460417474567) as alt NFT account and is launching [metaverse](https://www.sandbox.game/en/snoopdogg/) on the Sandbox
- Twitter adds tip jar for [Ethereum addresses](https://twitter.com/jacksondame/status/1441216811027030018) on iOS with plans to add [authentication of NFT ownership](https://twitter.com/pavtalk/status/1441096873138274306) 
- Proposal for [how RAI could detach from USD](https://community.reflexer.finance/t/completely-detaching-rai-from-fiat/89) to something non-fiat

* * *

### **Job Listings**

- Lambda School hiring [Subject Matter Expert](https://jobs.lever.co/lambdaschool/c3ff6acf-c8ad-4957-b1a9-23a5f693598f) to build Ethereum curriculum
- [Team Lead](https://ethereum.bamboohr.com/jobs/view.php?id=43&source=weekinethnews) for the Ecosystem Support Program at the Ethereum Foundation

**Reach people experienced with Ethereum.**  $345 per line (~75  
character limit), payable in ETH or DAI/USDC to abcoathup.eth.  
Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- US Treasury [moves to regulate stablecoins](https://www.nytimes.com/2021/09/23/us/politics/cryptocurrency-regulators-rules.html)
- Coinbase [not launching USDC lending](https://blog.coinbase.com/sign-up-to-earn-4-apy-on-usd-coin-with-coinbase-cdad79e5f5eb) product after SEC warnings
- [Mainnet speaker](https://thedefiant.io/messari-sec/) served with subpoena by US SEC
- Chris Dixon: [tokens are a new digital primitive](https://cdixon.mirror.xyz/0veLm9KKWae4T6_H3siLpKF933NSdC3F75jhPQw_qWE), whilst still in skeuomorphic era of web3, starting to see native applications that couldn’t have existed before
- Pillars of [decentralized HR](https://medium.com/@loietaylor/the-foundations-of-decent-ralized-hr-3b58f6a52d31): onboarding & offboarding, employee review, decision making, conflict resolution and employee contracts
- [People’s Bank of China](https://www.coindesk.com/policy/2021/09/24/china-tightens-crypto-mining-crackdown-bans-trading/) lists banned activities including crypto currency exchange and provision of services by overseas exchanges
- Sparkpool says it is [banning Chinese miners](https://www.theblockcrypto.com/linked/118640/sparkpool-suspend-china-ethereum-mining-pool)
- JPMorgan: [strong preference for Ethereum versus Bitcoin](https://www.coindesk.com/business/2021/09/23/institutional-investors-preferring-ether-over-bitcoin-now-jpmorgan/) by institutional investors based on CME futures

**General**

- Bloomberg: [Flashbots profile](https://www.bloomberg.com/news/articles/2021-09-23/crypto-trading-how-flashbots-work-to-front-run-ether-and-other-coin-purchases)
- Brave’s [STAR protocol](https://arxiv.org/abs/2109.10074) (distributed Secret Sharing for Threshold Aggregation Reporting): k-anonymity in data collection
- US IRS spending millions to [crack hardware wallets](https://gcn.com/articles/2021/09/17/irs-cryptowallet.aspx)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-25-2021/](https://weekinethereumnews.com/week-in-ethereum-news-september-25-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Sep 30 – [NFT Fest Australia](https://nftfest.com.au/) (virtual)
- Oct 1-3 – [EthAtlanta](https://ethatl.com/) enterprise-focused hackathon & keynotes
- Oct 18 – [ENS online workshop](https://medium.com/the-ethereum-name-service/ens-online-workshop-october-2021-ec1fb049b77f)
- Oct 20-21 – [LisCon](https://liscon.org/) (Lisbon) sold out
- Oct 22-24 – [ETH Lisbon](https://ethlisbon.org/) hackathon
- **Oct 27 – Beacon chain upgrade to Altair [epoch 74240](https://github.com/ethereum/consensus-specs/pull/2625/files)** 
- **Oct 28-29 – [ETH Portland](https://2021.ethportland.com/) hackathon**
- Nov 1-4 – [NFT.NYC](https://www.nft.nyc/) sold out

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

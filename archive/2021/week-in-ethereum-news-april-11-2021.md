---
title: "Week in Ethereum News <BR> April 11, 2021"
date: "2021-04-12"
---

## **Eth News and Links**

**Mainnet**

- **Update your nodes before Berlin fork**: Besu [v21.1.4](https://github.com/hyperledger/besu/releases/tag/21.1.4), EthereumJS VM [v5.3.1](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs%2Fvm%405.3.1), Geth [v1.10.2](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.2), Nethermind [v1.10.56](https://github.com/NethermindEth/nethermind/releases/tag/1.10.56), OpenEthereum [v3.2](https://github.com/openethereum/openethereum/releases/tag/v3.2.0), Turbogeth [04.02 alpha](https://github.com/ledgerwatch/turbo-geth/releases/tag/v2021.04.02)
- [Beam sync in 80 seconds using meta witnesses](https://snakecharmers.ethereum.org/beam-sync-in-80-seconds-using-meta-witnesses/)
- Stateless ideas: [insertion-order Indexed Merkle Tries](https://ethresear.ch/t/statelessness-by-insertion-order-indexed-merkle-tries/9095) and [Bayesian network model of Witness Creation](https://ethresear.ch/t/bayesian-network-model-of-witness-creation-feedback-request/9115)
- [Should storage be priced separately from execution?](https://ethresear.ch/t/should-storage-be-priced-separately-from-execution/9101)

**EIPs/Standards**

- [ERC3473](https://github.com/ethereum/EIPs/blob/c25e033e64dff6f149db21e2518e59118b628ee0/EIPS/eip-3473.md): Multiple Callable Bonds Standard
- [ERC3476](https://github.com/ethereum/EIPs/blob/51fe79aa50a41d38ed422a71cf5ce968ed68ccf6/EIPS/eip-antitoken.md): Antitoken

**Proof of Stake**

- Latest [eth2 call](https://www.youtube.com/watch?v=XLB5HEWdZUE). Notes from [Alex Stokes](https://twitter.com/ralexstokes/status/1380209522447282176) and Ben [Edgington](https://hackmd.io/@benjaminion/SkiD8Y3rd). Altair PoS upgrade targeted for June/July
- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210410)
- The [goal is to turn off PoW in 2021](https://twitter.com/drakefjustin/status/1379052831982956547)
- The [Rayonism spec v0.1 to turn off PoW](https://notes.ethereum.org/@n0ble/rayonism-the-merge-spec) and the [meta-spec](https://notes.ethereum.org/@protolambda/rayonism)
- A [simple approach to incentivizing shard staggering](https://ethresear.ch/t/simple-approach-to-incentivizing-shard-staggering/9149) via checksum incentives
- _Exactly_ [how much can I make as a staker](https://pintail.xyz/posts/beacon-chain-validator-rewards/)? Pintail gets deep into the weeds
- Vitalik’s [why sharding is great](https://vitalik.ca/general/2021/04/07/sharding.html) explainer

**Layer2**

- GodsUnchained launches [ImmutableX zkrollup for free NFT transactions](https://www.immutable.com/blog/immutable-x-alpha-trading-launch). Also running StarkEx: dydx now out of beta with its [cross-margined perpetuals zkrollup](https://dydx.exchange/blog/public).
- StarkWare’s [Caspian l2 AMM](https://medium.com/starkware/caspian-an-l2-powered-amm-f20e93b5421) - batch transactions together and have one layer 1 net transaction. Targeting June
- A [prototype of ENS on Optimism](https://medium.com/the-ethereum-name-service/mvp-of-ens-on-l2-with-optimism-demo-video-how-to-try-it-yourself-b44c390cbd67) with demo
- Celer’s [layer2 finance is on Ropsten testnet](https://blog.celer.network/2021/04/05/the-layer2-finance-testnet-carnival-win-32000-by-helping-us-test-defi-citys-first-subway/) with contest and incentives to test
- [L2beat](https://www.l2beat.com/): tracking the traction of layer2

* * *

### **This newsletter is made possible thanks to [1inch Network](https://1inch.io/?utm_source=evan_van_ness&utm_medium=newsletter&utm_campaign=letter_01)!**

![](https://weekinethereumnews.com/wp-content/uploads/2021/04/1inchbanner-1024x402.png)

The popular DeFi platform [1inch has expanded to the 1inch Network](https://blog.1inch.io/introducing-the-1inch-network-d459c16824a7) by creating multiple protocols, products and teams, all based around the idea of providing instruments for users to maximize their financial opportunities in DeFi.

Currently, the 1inch Network consists of five independent yet interoperable components. In addition to the 1inch Aggregation Protocol and 1inch Liquidity Protocol, which are already admired in the DeFi space, the other three components are the 1inch DAO, 1inch Labs and the 1inch Foundation. For more info check the [1inch.io](https://1inch.io/?utm_source=evan_van_ness&utm_medium=newsletter&utm_campaign=letter_01) and follow the [1inch Network's official Twitter](https://twitter.com/1inchNetwork)!

* * *

**Stuff for developers**

- Understanding [gas costs after Berlin](https://hackmd.io/@fvictorio/gas-costs-after-berlin) - access lists create opportunity for gas golfing but are primarily about making sure no contracts get bricked when eip2929 makes state access opcodes more expensive
- OpenZeppelin [Wizard](https://blog.openzeppelin.com/wizard/): tell it what you want and it generates Solidity for you
- [Testing and using custom hooks](https://medium.com/ethworks/usedapp-deep-dive-into-custom-hooks-and-testing-4a59fbc1769a) with Usedapp
- A complete [guide to full stack Eth dev](https://dev.to/dabit3/the-complete-guide-to-full-stack-ethereum-development-3j13) using React, Ethers.js, and Hardhat

**Security/incidents**

- A [solution to](https://samczsun.com/paradigm-ctf-2021-swap/) _[swap](https://samczsun.com/paradigm-ctf-2021-swap/)_, the most difficult problem from Paradigm’s CTF. You need to overflow memory in the mint function.
- [Fei vulnerability](https://medium.com/immunefi/fei-protocol-vulnerability-postmortem-483f9a7e6ad1) from faulty minting logic

**Ecosystem**

- More attacks on [frontrunning bots](https://twitter.com/bertcmiller/status/1381296074086830091): special behavior for flashbots address, making the token pay the miner, or [freezing the tokens of bots who insta-buy a new Uniswap listing](https://twitter.com/bertcmiller/status/1380866397828440066). It appears that all the attacks on bots have led to bots turning off and gas prices going down to ~65 gwei.
- [58% of hashrate](https://twitter.com/thegostep/status/1381243931841691650) now on Flashbots
- [ETHmerge.com](https://ethmerge.com/) - an open source community effort to educate about Ethereum turning off proof of work
- Reminder: [asset transfer fees are easily avoidable via wrapping](https://www.reddit.com/r/ethereum/comments/mo9mw8/reminder_in_the_long_run_asset_transfer_fees_are/)

**Enterprise**

- Miami wants to explore [putting real estate titles on Ethereum](https://www.theblockcrypto.com/post/100647/miami-ethereum-city-services-blockchain). If you listen to the podcast, the [audio is better on Youtube](https://youtu.be/NcGTAJUHVJE)

**Application layer**

- [Liquity stablecoin live on mainnet](https://medium.com/liquity/liquity-goes-live-on-ethereum-mainnet-203d295d2fc6) - zero interest loans with only 110% collateralization
- Algo stablecoin [Fei has completely lost its peg](https://tribe.fei.money/t/reserve-stabilization/1793) at the moment. There is a vote to allow redemptions at $1, but currently the [vote is for the status quo](https://snapshot.org/#/fei.eth/proposal/QmWYNqr9Rcn8QFiZYyRqjQno3jXTToy3vM4bVKJkuntvoz)
- Kyber [dynamic market maker beta is live](https://blog.kyber.network/kyber-dmm-beta-is-live-b6bdd18d0dde) - fees go up and down with volatility and programmable pricing curve
- [Christie’s to auction nine CryptoPunks](https://twitter.com/ChristiesInc/status/1380236081472364550)
- [WWE is selling Undertaker NFTs](https://www.bitski.com/wwe), chess world champion Magnus Carlsen is [selling NFTs of his games](https://www.bongcloud.art/)
- [GnosisAuction](https://blog.gnosis.pm/announcing-gnosis-auction-launch-390124d56248) for token launches with frontrunning resistance via batch auctions
- 73 Dai [PoolTogether deposit wins ~$44k](https://twitter.com/lay2000lbs/status/1380956604183552002)
- [1inch Network](https://blog.1inch.io/introducing-the-1inch-network-d459c16824a7). 1inch adds a DAO, Foundation, and Labs to the dex aggregator and liquidty pools
- New [TornadoCash pools](https://twitter.com/TornadoCash/status/1380418160327806981): _Dai_ 100, 1k, 10k, 100k. _cDAI_: 5k, 50k, 500k, 5m. _wBtc_: 0.1, 1, 10
- [](https://twitter.com/defipulse/status/1380889501283799042)[Compound is the first protocol over $10b](https://twitter.com/defipulse/status/1380889501283799042) TVL per Defipulse, with DeFi TVL over $50b

**Regulation/business/tokens**

- Paris Hilton: [why I’m excited about NFTs](https://parishilton.com/why-im-excited-about-nfts/)
- Tom Brady is [launching an NFT company](https://www.bostonglobe.com/2021/04/07/business/tom-brady-is-launching-an-nft-company/)
- Mark Cuban: [ETH will dwarf BTC](https://www.forbes.com/sites/billybambrough/2021/04/06/billionaire-mark-cuban-reveals-why-he-thinks-ethereum-will-dwarf-bitcoin-as-crypto-market-price-hits-2-trillion/)

**General**

- [Facebook phone numbers searchable in haveibeenpwned](https://www.troyhunt.com/the-facebook-phone-numbers-are-now-searchable-in-have-i-been-pwned/)
- [CLR fund round 5 is live](https://blog.clr.fund/round-5-launch/), matching but with MACI privacy using SNARKs

* * *

## **Job Listings**

- [Element Finance](https://element.fi/), launching very soon, is hiring a [Solidity engineer](https://docs.google.com/document/d/1D0wxlgnRsd6rQh2s3rC1Lq1fADkcHBtfKAVhepx6wss/edit?usp=sharing)
- Nomic Labs (Hardhat/Buidler) is hiring a [senior dev and an engineering manager](https://www.notion.so/Nomic-Labs-jobs-991b37c547554f75b89a95f437fd5056)
- Junior devs: Nethermind is looking for [junior Solidity, data analysts, nodeJs devs](https://twitter.com/nethermindeth/status/1371830788329779210)
- Status is hiring! [Eng Lead - Go](https://grnh.se/f727dfb01us), [Snr Go Developer](https://grnh.se/01d463ba1us), [see our jobs page](https://status.im/our_team/jobs.html)
- Join Tellor. Backend/solidity/marketing/community - [tellor.io/jobs](https://tellor.io/jobs)

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-april-11-2021/](https://weekinethereumnews.com/week-in-ethereum-news-april-11-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- April 14 - [Berlin upgrade fork](https://github.com/ethereum/pm/issues/248#issuecomment-782069875) (block 12244000)
- **April 14 - [Coinbase public listing](https://blog.coinbase.com/coinbase-announces-effectiveness-of-registration-statement-and-anticipated-listing-date-of-its-1509b281f760)**
- April 16 - [Rollup community grant](https://esp.ethereum.foundation/en/rollup-grants/) applications due
- Apr 16 – May 13 – ETHGlobal’s [Scaling Ethereum](https://scaling.ethglobal.co/) hackathon
- April 20 - deadline for [beacon chain security and testing RFP](https://notes.ethereum.org/@lsankar/security-rfp)
- April 20 - deadline to [comment on FATF anti-DeFi](http://www.fatf-gafi.org/publications/fatfrecommendations/documents/public-consultation-guidance-vasp.html) regulatory proposal
- April 22 - [Ethereum in the Enterprise 2021](https://www.conference2021.entethalliance.org/)
- May 14 - papers due for [WoSCA 2021](https://trailofbits.github.io/WoSCA/)
- May 14 - Jun 2 - [0xHack](https://0xhack.dev/)
- Jul 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

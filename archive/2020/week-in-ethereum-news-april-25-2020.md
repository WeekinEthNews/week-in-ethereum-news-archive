---
title: "Week in Ethereum News<BR> April 26, 2020"
date: "2020-04-26"
---

## **Eth News and Links**

**Eth1**

- Nethermind [v1.8.18](https://github.com/NethermindEth/nethermind/releases/tag/1.8.18) beta enables beam sync by default. Stay on v1.7.x for stable releases
- A very rough transcript from the [latest Stateless Ethereum call](https://notes.ethereum.org/@afhGjrKfTKmksTOtqhB9RQ/HyW2vY6uL). You’ll need to have context for this to make sense.
- An [EIP1559 implementer call](https://github.com/ethereum/pm/issues/167) (predictable transaction fees for users plus ETH burn) on April 30

**Eth2**

- Latest [Lighthouse client](https://lighthouse.sigmaprime.io/update-24.html) update, next public testnet likely this week, working on testnet interop
- Latest [Prysmatic client](https://medium.com/prysmatic-labs/eth-2-0-dev-update-48-eth2-topaz-testnet-going-strong-b7b8cd2fb244) update, Topaz testnet launch, working with Sigma Prime on Lighthouse interop
- Latest [Eth2 implementer call](https://youtu.be/avRcGzfjeIw?t=32), with notes from [Ben](https://hackmd.io/@benjaminion/rkXuXCRd8) and [Mamy](https://gist.github.com/mratsim/b4ae481879c5994be8dd3b17a4cbb91a)
- There was also a call on API standardization. No video, but notes from [Mamy](https://gist.github.com/mratsim/f0ab07dcb6e7c040bec5995b69391210) and [Proto](https://gist.github.com/protolambda/51152013648367e4d9bd1874d0860bc9)
- [Lightweight clock sync protocol](https://ethresear.ch/t/lightweight-clock-sync-protocol-for-beacon-chain/7307)
- An online [eth2 staking calculator](https://ethereumprice.org/eth-2-calculator/), based on the [ConsenSys Codefi spreadsheet](https://docs.google.com/spreadsheets/d/15tmPOvOgi3wKxJw7KQJKoUe-uonbYR6HF7u83LR5Mj4/edit#gid=1548910165)

**Layer2**

- AZTEC releases [code for their zk-zk rollup](https://medium.com/@tompocock/zk-zk-rollup-code-release-i-97216347b3bc), implements recursion for SNARKs over a single curve
- A [spec for account-based anonymous rollup](https://ethresear.ch/t/account-based-anonymous-rollup/6657/12)
- How [state channels fits into layer2](https://blog.statechannels.org/do-we-still-need-state-channels/) post-rollups: immediate finality, no third party necessary, and arbitrary execution.

**Stuff for developers**

- Truffle [v5.1.23](https://github.com/trufflesuite/truffle/releases/tag/v5.1.23) - Solidity stacktraces for debugging
- web3js [v1.2.7](https://github.com/ethereum/web3.js/releases/tag/v1.2.7) - new Websocket provider with auto-reconnect, lots of bugfixes
- OpenZeppelin [Contracts v3](https://forum.openzeppelin.com/t/openzeppelin-contracts-v3-0/2695), migrated to Solidity v0.6
- How to use [accesscontrol.sol](https://medium.com/coinmonks/how-to-use-accesscontrol-sol-9ea3a57f4b15) in OpenZeppelin
- Two posts on inheritance in Solidity from [Sheraz Arshad](https://medium.com/coinmonks/inheritance-in-solidity-debunked-3d8dd32d3a99) and [Igor Yalovoy](https://forum.openzeppelin.com/t/solidity-diamond-inheritance/2694)
- Source [liquidity with the 0x API](https://blog.0xproject.com/managed-liquidity-with-0x-api-403182de0dcf)
- [Coinbase price oracle](https://blog.coinbase.com/introducing-the-coinbase-price-oracle-6d1ee22c7068): signed price feed available via API
- Quick start to building a [governance interface](https://medium.com/compound-finance/building-a-governance-interface-474fc271588c) for Compound
- [Zerion SDK](https://blog.zerion.io/defi-sdk-making-money-lego-work-1dc08b8982cf) - on-chain decoder of complex ERC20 tokens and an onchain registry of protocol metadata
- Real time [front end data with Embark’s Subspace library and Infura](https://blog.infura.io/frontend-dapp-development-2/)
- Using TrailofBits’ [Echidna fuzzer to find transactions with high gas consumption](https://github.com/crytic/building-secure-contracts/blob/master/program-analysis/echidna/finding-transactions-with-high-gas-consumption.md)
- For Pythonistas, a 3 part series to [getting started in Brownie](https://medium.com/@iamdefinitelyahuman/getting-started-with-brownie-part-1-9b2181f4cb99)
- [Getting revert reasons](https://medium.com/authereum/getting-ethereum-transaction-revert-reasons-the-easy-way-24203a4d1844) in an NPM package
- [any.sender transaction relayer is on mainnet](https://medium.com/anydot/any-sender-cyberdice-2-0-3-eth-prize-efacf1419add), with a CyberDice competition ending Monday (showing how to use the any.sender API) to win 3 eth
- [OpenZeppelin to re-focus on security](https://forum.openzeppelin.com/t/doubling-down-on-security/2712), thus deprecating its networkJS library, Gas Station Network libraries, and starter kits. [Gas Station Network](https://www.opengsn.org/) lives on at opengsn.org
- Post-lendfme, a [defense of ERC777 tokens](https://medium.com/@provablethings/is-a-new-token-standard-really-to-blame-for-the-imbtc-uniswap-and-dforce-attacks-31c62e2bc799)
- The lendfme attacker gave all assets (value ~25m USD) back, apparently because the attacker’s [IP address was on a server](https://twitter.com/1inchExchange/status/1252709086803767297) from accessing 1inch’s frontend.
- Hegic Options had a bug, and thus a function can never be called. It will [reimburse its users for over 150 ETH](https://twitter.com/HegicOptions/status/1254276134344314883) that is locked forever

**Ecosystem**

- Videos from [EY Global Blockchain virtual summit](https://www.youtube.com/user/sfpbrody/videos)
- [Cloudflare is now a Rinkeby testnet signer](https://twitter.com/peter_szilagyi/status/1253234216353042432)
- [Ideas for EthGlobal’s Hackathon.money](https://docs.google.com/spreadsheets/d/1fXmwGqMuo1CxRPYN4bD5rb3yAUXMwPaPuLVWO8_ftds)
- a MyCrypto [guide to reading audit reports](https://twitter.com/MyCrypto/status/1254058121342803968). Early adopters beware - you should definitely read audit reports!

**Enterprise**

- [Italy’s ANSA newswire registers a hash](https://www.coindesk.com/italys-leading-wire-service-is-using-ethereum-to-thwart-copycats) of articles to combat fake news, including transparency about updates
- Citing the pandemic, Indian shipping ministry wants to use [CargoX for bills of lading on Ethereum](https://economictimes.indiatimes.com/industry/transportation/shipping-/-transport/covid-19-shipping-min-seeks-govt-intervention-for-recognition-of-electronic-trade-documents/articleshow/75234471.cms)

**Governance, DAOs, and standards**

- [Greg Colvin put ProgPoW](https://github.com/ethereum/pm/issues/165) on the agenda for the next core devs call
- A walkthrough of [TheLAO](https://medium.com/@thelaoofficial/the-end-of-ptsdao-a-walkthrough-of-the-lao-and-proposal-process-265301183ae0), launching April 28. They’re using a TCRParty-fork called [LAOScout](https://medium.com/@thelaoofficial/the-lao-scout-launching-a-token-curated-registry-to-crowdsource-the-best-blockchain-projects-75cc48fda352) to put startups on radar for funding from TheLAO.
- [ERC2615](https://github.com/ethereum/EIPs/blob/2f84770c186b9abfcf681be8ec46ec723e7306d8/EIPS/eip-n.md): Non funglible property standard
- [ERC2612](https://github.com/ethereum/EIPs/blob/8a34d644aacf0f9f8f00815307fd7dd5da07655f/EIPS/eip-2612.md): Permit extension for ERC20

**Application layer**

- Gnosis launches [Corona virus prediction markets](https://blog.gnosis.pm/corona-information-markets-df7cf3582026), subsidized with Gnosis liquidity
- [cent v2](https://beta.cent.co/+nb1vrq). new version of seeding, aimed at monthly subscriptions for content creators. Also a separate tipping feature, and winner-takes-all-bounties
- dYdX [perpetual BTCUSD contracts with 10x leverage](https://medium.com/dydxderivatives/dydx-launches-btc-perpetual-contract-market-68f59b193f7e) is in private alpha (not available on front end in US).
- Futureswap [live on mainnet with perpetual ETHDAI contracts with 20x leverage](https://medium.com/futureswap/futureswap-20x-leverage-on-ethereum-f27a2a9ed59a), a closed source alpha that did over 10m in volume, and is now effectively shut down
- [Opyn gets a front end with an order book](https://opynmonitor.xyz/#/trade/oeth-usdc)
- [Maker stability fees changed](https://twitter.com/MakerDaiBot/status/1254033913623859202), now 6% for USDC, 0% for ETH/BAT, (DSR obviously still 0). 12 hour governance delay
- [rTrees users planted 1541 trees](https://twitter.com/rTreesDapp/status/1253047496084992008) for Earth Day
- Golem [re-writing their codebase](https://blog.golemproject.net/next-milestone/), migrating the token to be ERC20 compliant
- RequestNetwork [hits 1m USD invoiced](https://request.network/en/2020/04/22/milestone-reached-launching-request-create-and-pay/)
- [Signal vs Telegram vs Status](https://our.status.im/the-secure-messaging-app-of-the-future/)
- NexusMutual: [how Solidity cover will evolve](https://forum.nexusmutual.io/t/smart-contract-cover-general-direction/40) to be able to cover the demand for large policies
- [TrustlessFund is live on mainnet](https://medium.com/trustless-fund/trustless-fund-is-live-4e00df17d641) (but unaudited!) - specify a lock date and a beneficiary
- [PoolTogether Pods](https://medium.com/pooltogether/winning-more-prizes-185bad7f6d63) - now you can trustlessly buy your pooltogether tickets as a group
- [Aave updates](https://medium.com/aave/development-update-whats-up-with-aave-b2e18294dc16): adds a UI for manual liquidations, as well as a UI to see burnt LEND, to go with its new risk framework
- 2key: internationally [monetize your calls with an Eth-based paywall Zoom plugin](https://www.2key.network/zoom-smartsession)
- [Dharma social payments](https://twitter.com/Dharma_HQ/status/1252714776448262145): send USD instantly to any Twitter user anywhere around the globe

**Tokens/Business/Regulation**

- [Constant function market makers as a zero-to-one DeFi innovation](https://medium.com/bollinger-investment-group/constant-function-market-makers-defis-zero-to-one-innovation-968f77022159)
- Jacob Horne on [redeemable tokens](https://bankless.substack.com/p/the-democratization-of-value) and Saint Fame
- [Securitize uses white-label AirSwap](https://www.securitize.io/blog/instant-access-easy-secure-and-compliant-peer-to-peer-transactions-of-digital-securities) for US securities transfer
- Token Terminal has an [interesting P/E metric](https://www.tokenterminal.xyz/)
- The [fundamental value proposition of ETH](https://bankless.substack.com/p/the-fundamental-value-proposition)

**General**

- Post-Black Thursday, [is Dai still safe to use](https://medium.com/coinmonks/understanding-the-impact-of-makerdaos-black-thursday-6e338e37c10c)?
- Dappnode makes it [easier to run non-Eth chains (but why!) and prepares for Eth2](https://medium.com/dappnode/faster-lighter-dappnode-er-e4e14f0e45d5)
- Bobbin Threadbare’s [STARK-based VM in Rust](https://ethresear.ch/t/introducing-distaff-a-stark-based-vm-written-in-rust/7318)
- Libra changes to being [multi-fiat stablecoins that will always be permissioned](https://www.forbes.com/sites/michaeldelcastillo/2020/04/16/libra-compromises-undermine-original-facebook-promise/amp/?__twitter_impression=tru)
- How much your new [browser in iOS is spewing data to the world](https://brave.com/ios-browser-first-run/) about you

* * *

## **This newsletter is made possible by [ConsenSys](https://consensys.net/)**

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In [Ethereum News](https://weekinethereumnews.com/). Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit.

Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-april-25-2020/](https://weekinethereumnews.com/week-in-ethereum-news-april-25-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Apr 29-30 - [SoliditySummit](https://solidity-summit.ethereum.org/) (Berlin)
- May 8-9 - [Ethereal Summit](https://www.etherealsummit.com/) (NYC)
- May 22-31 - [Ethereum Madrid](https://ethereummadrid.com/hackathon-2020-update/) public health virtual hackathon
- **May 29-June 16 - [SOSHackathon](https://soshackathon.com/)**
- June 17 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

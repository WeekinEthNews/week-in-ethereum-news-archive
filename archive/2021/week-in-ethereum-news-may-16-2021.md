---
title: "Week in Ethereum News <BR> May 16, 2021"
date: "2021-05-16"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest [core devs call](https://youtu.be/H_T2nNrTuWQ?t=521). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1393230961890906115)
    - [London EIPs](https://github.com/ethereum/eth1.0-specs/blob/master/network-upgrades/mainnet-upgrades/london.md#included-eips): EIP1559: Fee market change, EIP3198: BASEFEE opcode, EIP3554: Difficulty Bomb Delay to December, EIP3529: Reduction in gas refunds, EIP3541: Reject new contracts starting with 0xEF
    - JSON RPC to use same naming as EIP1559
    - Baikal - London devnet for devs to experiment with London until the testnet fork dates
    - London blocks/dates: Ropsten: 10399301 (June 9), Goerli: 4979794 (June 16), Rinkeby: 8813188 (June 23), mainnet aim is July 14
- [Block access list](https://ethresear.ch/t/block-access-list-v0-1/9505)
- [Core dev apprenticeship program](https://blog.ethereum.org/2021/05/13/core-dev-apprenticeship/), an effort by Piper Merriam to find and train more core devs

**EIPs/Standards**

- [EIP3554](https://eips.ethereum.org/EIPS/eip-3554): Difficulty Bomb Delay to December 1st 2021
- [ERC3569](https://github.com/ethereum/EIPs/blob/eca077f7f50584de85385403007a02a457ab1d60/EIPS/eip-draft_sealed_nft_metadata.md): Sealed NFT Metadata
- [ERC3561](https://github.com/ethereum/EIPs/blob/682b83ebff75baa1483abba69d18d4f959fbebad/EIPS/eip-3561.md): Trust Minimized Upgradeability Proxy

**Proof of stake consensus layer**

- Huge milestone on the way to turning off PoW: [Nocturne testnet successfully launched](https://twitter.com/protolambda/status/1392503445714767883) with 12 combinations of consensus and mainnet clients. It's processing transactions and reaching finality.
    - Checkout the [block explorer](https://nocturne.rayonism.io/), live for a couple more days
- Latest [merge implementers call](https://www.youtube.com/watch?v=uzjhLPtvTMQ&t=11s); Nocturne is last merge devnet until post London/Altair
- [Lighthouse v1.4.0](https://twitter.com/sigp_io/status/1393010946025549825) planned for mid-June: 80% Eth1 call reduction, uses 50% less RAM, Altair support, Doppelganger slashing protection, remote signer and beta Windows support

**Layer2**

- [Arbitrum mainnet](https://medium.com/offchainlabs/wen-arbitrum-634969c14713) launches for devs on May 28. Last testnet includes a sequencer for instant transactions.
- [Loopring zkrollup hits $1B in trading volume](https://twitter.com/loopringorg/status/1392676013751078913)
- [Ethhole.link](https://ethhole.link/): token flow visualization from Ethereum to L2 and sidechains

* * *

### **This newsletter is made possible thanks to Synthetix's [Kwenta](https://kwenta.io/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2021/04/IMG_20210418_190328_618-1024x512.jpg)

[Kwenta](https://kwenta.io/) enables traders to access real-world and derivative assets on-chain with zero slippage using the power of the [Synthetix](https://synthetix.io/) protocol.

Trade popular synthetic cryptocurrencies, commodities, forex, and equities, such as TSLA, COIN, and FAANG stocks, without the limits or compromises of a centralized exchange.

Try [Kwenta](https://kwenta.io/) today!

* * *

**Stuff for developers**

- [web3.js v1.3.6](https://github.com/ChainSafe/web3.js/releases/tag/v1.3.6) security patch for underscore and bumps versions of ENS and Ethers
- UMA’s [Optimistic Oracle](https://medium.com/uma-project/introducing-umas-optimistic-oracle-d92ce5d1a4bc) via dispute resolution process. Out of beta; no need to use UMA's financial contracts
- Gnosis Safe [L2/sidechain rollout plan](https://blog.gnosis.pm/gnosis-safes-multichain-future-b676b5b8f431) so you can secure DAO treasuries and privileged smart contract functions such as upgrades on L2/sidechains
- [Alchemy Transfer API](https://blog.alchemy.com/blog/transaction-history) to access historical Eth, ERC20 and ERC721 transfers in single call

**Security**

- [Slither v0.8](https://github.com/crytic/slither/releases/tag/0.8.0) - improved Solidity v0.8 support, better Hardhat support, 3 new detectors
- [xToken exploit](https://medium.com/xtoken/initial-report-on-xbnta-xsnxa-exploit-d6e784387f8e) resulted in $25m loss, due to logic error allowing infinite mint
- yEarn finds a [missing check on a low level call](https://github.com/yearn/yearn-security/blob/master/disclosures/2021-05-13.md); no funds lost
- [Fei awards](https://medium.com/fei-protocol/fei-bonding-curve-bug-post-mortem-98d2c6f271e9) $800k bounty for bonding curve price manipulation vulnerability.

**Ecosystem**

- After [dog memecoins were using over 10%](https://twitter.com/FrankResearcher/status/1392040055133384705) of Ethereum's gas, Vitalik [donated billions (in notional value, it wasn't even nearly liquid) in memecoins](https://www.forbes.com/sites/ninabambysheva/2021/05/12/ethereums-co-founder-vitalik-buterin-donates-over-1-billion-to-india-covid-relief-fund-and-other-charities/?sh=7986ed726548) to India Covid Relief, longevity research, Charter Cities Institute, Gitcoin multisig, etc. Vitalik's trades were getting sandwiched/backrun, so he used [Flashbots via Archerswap](https://twitter.com/bertcmiller/status/1392572952617623553)
- [Flashbots Dashboard](https://twitter.com/bertcmiller/status/1392871268953858057) shows ~$45m miner profit from Flashbots. ~85% of hashpower now uses Flashbots. A third of blocks now have a bundle
- [Etherscan adds ENS names](https://twitter.com/etherscan/status/1392434517571375110) to transaction lists
- [Wallet composability](https://medium.com/coinmonks/1the-importance-of-composable-wallets-for-users-and-developers-accb2aadff49): analyzing the layers of the wallet stack
- ETHGlobal's [Scaling Ethereum hackathon finalists](https://twitter.com/ETHGlobal/status/1392600353628049410)

**Enterprise**

- [Covantis claims 80% decrease in supply chain error rates in 3 months](https://consensys.net/blockchain-use-cases/global-trade-and-commerce/covantis/?utm_content=166176945&utm_medium=social&utm_source=twitter&hss_channel=tw-880544504750764032) since going live with Quorum
- Why [governments and enterprises will move from private chains to Eth mainnet](https://medium.com/blockchangers/permissioned-chains-will-move-over-to-the-ethereum-main-chain-5a8bbe53a4df)

**Application layer**

- Vitalik proposes [UNI should be an oracle token](https://gov.uniswap.org/t/uni-should-become-an-oracle-token/11988) for ETH/USD
- [Balancer V2](https://medium.com/balancer-protocol/the-most-flexible-and-efficient-amm-is-live-meet-balancer-v2-2451a22779b3) is live with 40-53% reduction in gas
- Creating pegged tokens to see if unit bias matters: [Woofy](https://twitter.com/bantg/status/1392231374086676483) is 1 million Woofy per YFI or [Breaker](https://twitter.com/brianmcmichael/status/1393291342248386566) which is 1 billion per MKR
- MerriamWebster sold an [NFT of its NFT definition](https://twitter.com/opensea/status/1392152303419936769)
- Christie's auctioned [9 Cryptopunks for ~$17m](https://www.christies.com/lot/lot-larva-labs-est-2005-9-cryptopunks-2-6316969)

**Regulation/business/tokens**

- A Bitcoiner flips: [why ETH will win the store of value war](https://michaelmcguiness.com/essays/why-eth-will-win-store-of-value)
- Justin Drake [values ETH using EVM fees](https://docs.google.com/spreadsheets/d/1U9cGxGY3_t7m4MEIpjKWtRcA2zRajywaxMCZYqbF9eI/edit#gid=0)
- One more flip: [ETH is more secure than BTC](https://www.flippening.watch/)
- Tesla will no longer accept BTC and will look at [energy efficient cryptocurrencies](https://twitter.com/elonmusk/status/1392602041025843203)
- [Tether discloses the assets backing USDT](https://www.coindesk.com/tether-first-reserve-composition-report-usdt). Half of the assets are commercial paper
- [US DOJ and IRS investigating Binance](https://www.bloomberg.com/news/articles/2021-05-13/binance-probed-by-u-s-as-money-laundering-tax-sleuths-bore-in) for money laundering
- [Rise of micro economies](https://coopahtroopa.mirror.xyz/gWY6Kfebs9wHdfoZZswfiLTBVzfKiyFaIwNf2q8JpgI): enabling a creator middle class

**General**

- [Fragattacks](https://www.fragattacks.com/). WiFi design and implementation security vulnerabilities - be extra sure to update your devices over the next few months
- [Etherscan hits the Alexa top 1000](https://twitter.com/mtbitcoin/status/1392055649601605632)
- [Boring Crypto](https://boringcryptoxyz.medium.com/introducing-boringcrypto-b0850435763f) web3 news aggregator with no price talk
- Palla's noob-friendly [glossary for the Merge, the Flippening, PoW, and PoS](https://twitter.com/smpalladino/status/1391901504752300033)
- Week in Ethereum News has a [new editor](https://twitter.com/abcoathup/status/1392943290681421825)

* * *

## **Job Listings**

- Synthetix are hiring: [Growth Marketer](https://jobs.defialliance.co/companies/synthetix/jobs/4454460-growth-marketer), [Senior Designer](https://jobs.defialliance.co/companies/synthetix/jobs/4538964-senior-designer)
- Ethereum Foundation hiring a [Cryptography Researcher - ZK VMs](https://www.iacr.org/jobs/item/2576)
- Devcon needs a Python developer for [L2 Pretix integration](https://www.notion.so/Python-Developer-for-L2-Pretix-Integration-Devcon-6244954e2bc346b7be18916cd05b34b1)
- OpenZeppelin is hiring [Security Researchers, Devs & Community](https://openzeppelin.com/jobs/)
- [Props](https://www.propsproject.com/): [General Manager/SaaS Division](https://jobs.gohire.io/props-0ds2x7xe/general-manager-saas-division-40616/), [Blockchain Engineer](https://jobs.gohire.io/props-0ds2x7xe/full-stack-blockchain-engineer-40634/) & [Data Analyst](https://jobs.gohire.io/props-0ds2x7xe/data-analyst-paid-internship-40677/).
- BitGo’s WBTC team is hiring [Blockchain Engineers](https://boards.greenhouse.io/bitgo/jobs/5191525002), [Sr. Blockchain Engineers](https://boards.greenhouse.io/bitgo/jobs/5089951002) and [Lead Blockchain Engineers](https://boards.greenhouse.io/bitgo/jobs/5197342002). (You can check out the rest of our jobs [here](https://boards.greenhouse.io/bitgo)!)

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of the workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-may-16-2021/](https://weekinethereumnews.com/week-in-ethereum-news-may-16-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- May 18-21 - [EY Global Blockchain Summit](https://pub.ey.com/public/2021/2101/2101-3679331/blockchain-summit-2021/index.html)
- May 21 - [Linda Xie and Austin Griffith talk Eth dev tooling](https://twitter.com/ljxie/status/1390772688193560581)
- **May 28 - optimistic rollup [Arbitrum launches](https://medium.com/offchainlabs/wen-arbitrum-634969c14713)**
- **May 28-30 - ETHGlobal's [Web3 Weekend](https://web3.ethglobal.co/)**
- **May 31 - deadline to apply for [Eth core dev apprenticeship](https://blog.ethereum.org/2021/05/13/core-dev-apprenticeship/)**
- **June 18 - July 9 - [ETHGlobal - Hack Money 2021](https://hackmoney.ethglobal.co/)**
- **June 25-27 - [Edcon](https://www.edcon.io/) (online)**
- July 14 - [tentative date for London hard fork](https://docs.google.com/spreadsheets/d/1Y3yyTqeqRO1O2UFVkNkHK_V5oRulZd6y-JJbSnKYrb4/edit#gid=0) (Ropsten June 9, Goerli June 16, Rinkeby June 23)
- July 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

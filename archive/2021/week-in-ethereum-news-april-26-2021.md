---
title: "Week in Ethereum News <BR> April 26, 2021"
date: "2021-04-26"
---

## **Eth News and Links**

**Mainnet execution layer**

- Tim Beiko’s [periodic broader overview of mainnet changes](https://hackmd.io/@timbeiko/acd): testnets for the July/Aug London upgrade
- Latest [core devs call](https://youtu.be/C9hzAYkklQM?t=244). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1385613482402275331): London fork in July/Aug will be eip1559, basefee, bomb delay, and eliminating refunds
- OpenEthereum [postmortem for Berlin consensus bug](https://docs.google.com/document/d/18BhIEB7V_f_GkL8NZptxq-xadu5sb8QUzego8YVVMUM/edit#heading=h.nxtmf7qzhoyo)

**EIPs/Standards**

- [ERC3440](https://github.com/ethereum/EIPs/issues/3519): NFT editions standard
- [EIP3520](https://github.com/ethereum/EIPs/blob/8a6f26c5c4929cdbb155fcef2fa5e8ced6d616a7/EIPS/eip-3520.md): transactions destination opcode
- [EIP3529](https://github.com/ethereum/EIPs/blob/5f9d8ea62033890c848e5b363408c82362bc6bcf/EIPS/eip-3529.md): No SELFDESTRUCT refunds, reduce SSTORE refunds, add a max refund per transaction of 20% of gas used
- [EIP3521](https://eips.ethereum.org/EIPS/eip-3521): Reduce access list cost

**Proof of stake consensus layer**

- Our proof of stake network had its first hiccups this week. An issue with eth1data voting and validator deposits led to Prysm nodes being unable to produce blocks. This was relatively minor, leading to an [average of less than a dollar](https://www.reddit.com/r/ethstaker/comments/mxpz57/regarding_the_recent_beacon_chain_incident/) of forgone attestations for individual validators.
    - Prysmatic [released a hotfix](https://github.com/prysmaticlabs/prysm/releases/tag/v1.3.8-hotfix+6c0942)
- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_210424): _it is time for everybody to take client diversity seriously_. Ben reflects on the hiccups. **Running the majority client puts your own money at risk, plus everyone else’s**.
- Turning off PoW testnet: [how to setup a multi-client ethereum merge testnet](https://github.com/protolambda/mergenet-tutorial). An ephemeral multi-client testnet is planned for late this upcoming week.
- Nethermind floats [October](https://twitter.com/nethermindeth/status/1385699335355125766) as an aggressive target to turn off PoW
- When we turn off PoW, [staking rewards will likely be multiples higher](https://twitter.com/drakefjustin/status/1384124998084792324) than they are now
- Latest [proof of stake implementation](https://youtu.be/D9Aqr8thF9c?t=225) call. Notes from [Alex Stokes](https://twitter.com/ralexstokes/status/1385295236885204997) and [Ben Edgington](https://hackmd.io/@benjaminion/rJUzAo0Id). The first upgrade (named Altair) may get pushed back a couple weeks, roughly around the London fork upgrade.
- We hit [1 million PoS blocks this week](https://beaconcha.in/block/1000000), the milestone block proposed by Validator\_McValid\_ETH
- [Visualizing Ethereum’s sharded, rollup-centric future](https://barnabe.substack.com/p/eth2?s=09), secured by proof of stake

**Layer2**

- Celer’s [layer2 finance is live](https://blog.celer.network/2021/04/22/the-layer2-finance-v0-1-mainnet-launches-democratize-defi-simple-and-zero-fees/): transfer your DAI, USDC, USDT or BUSD to Celer’s optimistic rollup and then you can deposit gas-free to Aave, Compound or Curve
- StarkEx’s [oracle price feed](https://medium.com/starkware/oracle-price-feed-on-starkex-2b15a3ca122)
- [Scalar](https://thegraph.com/blog/scalar): Connext’s state channel microtransactions powering TheGraph

* * *

### **This newsletter is made possible thanks to Celer!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

[Celer](http://celer.network/) recently launched [Layer2.finance](https://app.l2.finance/) on Ethereum mainnet.

Layer2.finance tackles the two biggest challenges preventing DeFi from reaching mass adoption: the extraordinarily high transaction fees and being very difficult to navigate and use. Layer2.finance is a novel solution that allows people to access all existing DeFi protocols at a fraction of the cost by acting like a “[DeFi Public Transportation System](https://blog.celer.network/2021/04/02/eli5-layer2-finance-the-modern-subway-of-the-defi-city/)”. With Celer’s [advanced layer-2 rollup technology](https://blog.celer.network/2021/02/18/layer2-finance-get-defi-mass-adoption-today-scaling-layer-1-defi-in-place-with-zero-migration/), multiple people split the cost of individual layer1DeFi transactions in a completely trust-free and non-custodial way.

Users can use Aave, Compound and Curve now completely for free via layer2.finance.

Follow Celer on [twitter](https://twitter.com/CelerNetwork), [blog](https://blog.celer.network/), [discord](https://discord.com/invite/Trhab5w) and [telegram](https://t.me/celernetwork).

* * *

**Stuff for developers**

- Solidity [v0.8.4](https://blog.soliditylang.org/2021/04/21/solidity-0.8.4-release-announcement/) - [custom errors](https://blog.soliditylang.org/2021/04/21/custom-errors/) and an ABI decoder v2 bugfix
- [PRBMath](https://twitter.com/PaulRBerg/status/1384179308978085889) - fixed point math Solidity library from Paul Berg
- An [Ethernal plugin](https://github.com/tryethernal/hardhat-ethernal) for Hardhat, an easy blockchain explorer for local networks
- Torus launches [Face/TouchID logins](https://medium.com/toruslabs/openlogin-by-torus-911c56526e33)
- zoKrates [v0.7](https://github.com/Zokrates/ZoKrates/releases/tag/0.7.0) - SNARKs on Ethereum library. breaking release with constant generics
- A prototype for [VDF in Solidity](https://github.com/kilic/evmvdf)
- Rivet’s [Bolt](https://medium.com/@designheretic/introducing-rivet-bolt-5a757cbeb7e3) for transaction data with no requests per second cap
- [Learn SQL and ETH at the same time](https://towardsdatascience.com/your-guide-to-intermediate-sql-while-learning-ethereum-at-the-same-time-7b25119ef1e2?gi=3dd064e47b17) tutorial
- [`Debug` commands with archivenode.io and IPFS](https://chasewright.com/ethereum-and-ipfs/)

**Security**

- New [Ethernaut level](https://twitter.com/OpenZeppelin/status/1384907280521519110)
- MakerDAO discloses patched [vulnerabilities in ESM and End modules](https://forum.makerdao.com/t/esm-end-module-upgrades-and-disclosures/7569)
- EASY (on Polygon) treasury was [controlled by one EOA](https://www.rekt.news/easyfi-rekt/) which got compromised
- [Pancake v2 bug](https://twitter.com/nipun_pit/status/1385531250073427968) (on BSC obviously, but in Solidity)
- Samczsun: [uncovering a 4 year old EToken2 bug](https://samczsun.com/uncovering-a-four-year-old-bug/)

**Ecosystem**

- This week, the [gas limit went up to 15m](https://etherscan.io/chart/gaslimit), fees low got down close to 30 gwei at off-peak periods
- [EF supported teams R&D update](https://blog.ethereum.org/2021/04/26/ef-supported-teams-research-and-development-update-2021-pt-1/): compendium of progress from EF teams
- [HoneybadgerSwap](https://medium.com/initc3org/honeybadgerswap-making-mpc-as-a-sidechain-364bebdb10a5): MPC as a sidechain, with a Uniswap-style demo running on Kovan testnet
- Messari notes that [Ethereum settled $1.5m trillion worth of transactions](https://twitter.com/RyanWatkins_/status/1384676842045681664) in just q1 2021

**Enterprise**

- Cartier, LVMH and Prada launch [Aura consortium chain](https://twitter.com/VanessaGrellet_/status/1384681019077496840) on Quorum

**Application layer**

- NexusMutual launches [expanded protocol cover](https://medium.com/nexus-mutual/nexus-is-growing-protocol-cover-is-live-56752446ec57): covers you against all protocol risks (rug pulls excepted!) even across different chains
- [Stock trading is live](https://blog.kwenta.io/stocks-are-now-live-on-kwenta/) on Synthetix’s Kwenta, starting with 6 big US tech stocks, with extra yield on afterhours pools
- UMA [synthetic CryptoPunk](https://medium.com/uma-project/ulabs-cryptopunks-synthetic-token-upunk-25d9d97600c3) index token
- DeFiSaver’s [Recipe Creator](https://twitter.com/DeFiSaver/status/1384158771623055375) build transactions in English or by clicking, and you can simulate it in the UI with Tenderly
- [Archer swap](https://twitter.com/calebsheridan/status/1384811452402442240): PoC frontend for 0 slippage fee “only execute if successful” Uniswap transactions
- Uniswap breaks [$10b weekly volume](https://twitter.com/haydenzadams/status/1384534770214916097)
- Centrifuge’s [real world assets live](https://medium.com/centrifuge/defi-2-0-first-real-world-loan-is-financed-on-maker-fbe24675428f) in MakerDAO with NewSilver’s real estate loans

**Regulation/business/tokens**

- [Ethereumcashflow.com:](https://ethereumcashflow.com/) a store of value with cash flow
- 3 [Canadian Ethereum ETFs](https://www.msn.com/en-us/money/other/3-ethereum-etfs-will-start-trading-today-in-canada-as-crypto-fever-continues/ar-BB1fQZbi) launch
- Venmo launched [crypto buying and selling](https://newsroom.paypal-corp.com/2021-04-20-Introducing-Crypto-on-Venmo)
- [Wyoming recognizes DAOs](https://twitter.com/CaitlinLong_/status/1384991490531729410) as type of LLC
- Beware of [NFT sleepminting](https://timdaub.github.io/2021/04/22/nft-sleepminting-beeple-provenance/): tricking frontends to make it look like artists created NFTs that they did not

**General**

- Dexes are superior to centralized exchanges reminder: [Turkish exchange Thodex founder](https://www.msn.com/en-us/money/other/thodex-cryptocurrency-exchange-chief-allegedly-goes-on-the-run-with-242bn-in-client-funds/ar-BB1g3IBO) apparently absconds with $2 billion
- [Bitmain says they’ll launch a new ASIC](https://twitter.com/OhGodAGirl/status/1386042625443078145), not sure who’s buying given that we’re turning off PoW
- [Practical SNARK aggregation](https://eprint.iacr.org/2021/529) without trusted setup

* * *

## **Job Listings**

- Matter Labs is hiring [engineering, operational & community roles](https://www.notion.so/matterlabs/Career-at-Matter-Labs-4a69ed0f7acb45c89f662cf12dbc2464) for zkSync
- Join our team to help [bring Ethereum into governments as a dApp developer](https://www.notion.so/symfoni/Symfoni-jobs-0c2bdc029d2a4cf7b91864a5e68ed00f)
- BitGo's WBTC team is hiring [Blockchain Engineers](https://boards.greenhouse.io/bitgo/jobs/5191525002), [Sr. Blockchain Engineers](https://boards.greenhouse.io/bitgo/jobs/5089951002) and [Lead Blockchain Engineers](https://boards.greenhouse.io/bitgo/jobs/5197342002). (You can check out the rest of our jobs [here](https://boards.greenhouse.io/bitgo)!)
- [Enzyme](https://enzyme.finance/) is hiring. [Solidity dev](https://www.notion.so/Senior-Smart-Contract-Developer-to-work-on-Enzyme-641aef0d89cc419cba792445354f835b), [data engineer](https://www.notion.so/Data-Engineer-a412646a06a046bfaac26085b4695857), [UX/UI designer](https://www.notion.so/UX-UI-Designer-e115c94e193b4e98b98283fa1bcaf3b8) & [growth eng](https://www.notion.so/Growth-Engineer-d682408e8500447888859f9d47bc4a79).
- 90 day apprenticeships to be an [auditor with Trail of Bits](https://twitter.com/dguido/status/1385636916620582922)
- Want to work on stateless/EVM? [EF JavaScript team is hiring several developers](https://twitter.com/EFJavaScript/status/1382292102348935168)

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue:

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **April 26-30 - [DAO Rush Week](https://daorushweek.com/)**
- **May 7 - [Building on Ethereum](https://twitter.com/dabit3/status/1386696929770283010) with Austin Griffith and Nader Dabit**
- May 14 - papers due for [WoSCA 2021](https://trailofbits.github.io/WoSCA/)
- May 14 - Jun 2 - [0xHack](https://0xhack.dev/)
- Jul 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

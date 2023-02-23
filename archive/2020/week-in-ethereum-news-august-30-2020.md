---
title: "Week in Ethereum News <BR> August 30, 2020"
date: "2020-08-31"
---

## **Eth News and Links**

**Eth1**

- Geth [v1.9.20](https://www.reddit.com/r/ethereum/comments/igdeid/geth_v1920_paragade_new_geth_bugfix_release/) bugfix release - new blockchain database layout, Go v1.15
- There was a kerfuffle about OpenEthereum this week: as [announced Aug 14](https://twitter.com/OpenEthereumOrg/status/1294187926432227328), the next release in a week or two is backporting features to v2.5 codebase because current release has stability issues. The new release [might not require resyncing](https://twitter.com/OpenEthereumOrg/status/1298163468948905985).
- Turbogeth [weekly alpha release](https://github.com/ledgerwatch/turbo-geth/releases/tag/v2020.08.04), fixes memory leak and stability improvements
- Where [Regenesis fits in the eth1 roadmap](https://blog.ethereum.org/2020/08/25/the-1x-files-tech-tree-regenesis/)
- Fee market reform: [a question of fairness](https://medium.com/@pintail/ethereum-fee-market-reform-eip-1559-as-a-question-of-fairness-567c52dac017)?
- Notes from the latest [1559/fee market reform call](https://twitter.com/TimBeiko/status/1299397735171280896)

**Eth2**

- Eth1 merged into eth2: [demo of an Eth1 transfer inside an eth2 client](https://twitter.com/mkalinin2/status/1299038199591862274). It’s dockerized, so you can run it yourself
- What [hardware should I buy to stake](https://kb.beaconcha.in/staking-and-hardware) my Eth?
- Client diversity matters: Bankless guide to [get started staking on the Medalla testnet](https://bankless.substack.com/p/guide-becoming-a-validator-on-the)
- A script for [easy Nimbus deployment](https://github.com/gravityblast/nimbus-deploy)
- Attestant opensources its [distributed remote keymanager](https://www.attestant.io/posts/introducing-dirk/)
- Barnabé Monnot: [agent based validator modeling](https://github.com/barnabemonnot/beaconrunner/blob/master/notebooks/thunderdome.ipynb) with new strategies and behaviors. Python notebook

* * *

### **This newsletter is made possible thanks to [Celer](https://www.celer.network/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/05/Screenshot-from-2020-05-10-16-13-18.jpg)

[Celer](http://celer.network/) is a coherent layer-2 scaling platform on Ethereum powered by [Generalized State Channel Network](https://www.celer.network/docs/celercore/index.html) and [Hybrid Rollup](https://medium.com/celer-network/adding-hybrid-pos-rollup-sidechain-to-celers-coherent-layer-2-platform-d1d3067fe593) technology. Real money games, such as [Arcade Win](https://apps.apple.com/us/app/arcade-win/id1459895768) and [Daub Cash](https://apps.apple.com/us/app/daub-cash/id1513396754), built using [Celer's gaming-focused SDK](http://developer.celerx.app/) just reached top #10 ranking in App Store.

We are hosting [a campaign to expand state channel network on Ethereum with $20,000 prizes](https://blog.celer.network/2020/08/20/light-up-the-world-with-celer-network-state-channel-phase-2/).

We have also just launched [State Guardian Network beta testnet.](https://blog.celer.network/2020/08/10/state-guardian-network-beta-testnet-launches/) Follow us on [twitter](https://twitter.com/CelerNetwork), [blog](https://blog.celer.network/), [discord](https://discord.com/invite/Trhab5w) and [telegram](https://t.me/celernetwork).

* * *

**Stuff for developers**

- [Improving Eth dev ex](https://medium.com/nomic-labs-blog/nomic-labs-devx-prioritizing-projects-9db6659cbed6): faster compiling/testing, better debugging, better editors/IDEs and more
- [ethers-contract-hook](https://www.npmjs.com/package/@govtechsg/ethers-contract-hook): package to generate hooks from Ethers contract functions
- A buidler [plugin to easily verify on Etherscan](https://github.com/nomiclabs/buidler/tree/development/packages/buidler-etherscan)
- Using [scaffold-eth to build an NFT art sales](https://medium.com/@austin_48503/nifty-ink-%EF%B8%8F-alpha-release-c860a4904cb2) app on xdai
- create-eth-app [v1.4](https://github.com/PaulRBerg/create-eth-app/releases/tag/v1.4.0) adds IPFS deployment
- A [strongly typed fixed point math library](https://github.com/albertocuestacanada/DecimalMath) to prevent the YAM bug
- [YFV pool exploit](https://medium.com/@yfv.finance/yfv-update-staking-pool-exploit-713cb353ff7d)
- [Solidity bugs compiled to Yul](https://github.com/Mikerah/solidity-bugs-and-vulns-in-yul)
- [10 points about the Diamond proxy standard](https://twitter.com/mudgen/status/1297920437415010304)
- Identifying [orchestration patterns in Solidity](https://hackernoon.com/identifying-smart-contract-orchestration-patterns-in-solidity-pd223x20): simple (Uniswap), more complicated (Yield) and…Maker.

**EIPs/Standards**

- [ERC2917](https://github.com/skardas/EIPs/blob/8458979ad6885709eff929eed2dcab52803cb3cc/EIPS/eip-2917.md): Staking Reward Calculation

**Ecosystem**

- Beware of [generalized frontrunners](https://medium.com/@danrobinson/ethereum-is-a-dark-forest-ecc5f0505dff): the transaction pool is a dark forest
- [EthGas.watch](https://ethgas.watch/): an aggregator of gasprice predictions that will email you when gas prices drop
- [EthVM](https://medium.com/myetherwallet/introducing-mews-ethereum-blockchain-explorer-ethvm-beta-78e5b849e2fc): an opensource block explorer from MyEtherWallet
- Uniswap frontend now [requires that you pick a token list](https://uniswap.org/blog/token-lists/)

**Enterprise**

- [Quorum moves to ConsenSys](https://consensys.net/blog/news/consensys-acquires-jpm-quorum). As part of the deal, JPMorgan invests in ConsenSys
- Video demo of [OpenLaw integration with Microsoft Office](https://twitter.com/awrigh01/status/1299338807960113155)
- Baseline Protocol [v0.1](https://oasis-open-projects.org/baseline-protocol-v01/), set of standard interfaces for privately using Eth mainnet as the source of truth between enterprises

**Application layer**

- Uniswap [flipped Coinbase](https://twitter.com/haydenzadams/status/1300034164830408704) for transaction volume and [flipped Bitcoin](https://twitter.com/nanexcool/status/1299943708478115840) for transaction fees
- [Aave #1 on DefiPulse for TVL](https://twitter.com/defipulse/status/1298290438827212800). Aave company also got a UK [license to provide payment services](https://www.theblockcrypto.com/post/75845/aave-uk-fca-emi-license-defi).
- [Goodghosting](https://medium.com/goodghosting/boo-goodghosting-launches-f3842b173909) is live: multiple people save regularly using Aave, those who don’t miss a payment get the interest of those who miss a payment
- [Sushiswap](https://medium.com/sushiswap/the-sushiswap-project-c4049ea9941e): deposit your uniswap LP tokens and get SUSHI back (10% for anonymous team) then after 2 weeks it becomes a Uniswap competitor with fees accruing to Sushi holders. More than 500m locked in less than a week
- Aragon has a [conviction funding](https://aragon.org/blog/introducing-the-conviction-funding-pilot) pilot
- [Meme](https://medium.com/@dontbuymeme/announcing-the-meme-protocol-yield-farming-meets-nfts-1a9820f7058b): it began as a [joke](https://twitter.com/JordanLyall/status/1294466755692081152), now it’s NFT farming
- TokenBrice on understanding the [rules of vegetable meme ponzis](https://tokenbrice.xyz/posts/2020/defi-moneygames/)

**Tokens/Business/Regulation**

- SEC slightly relaxes [accredited investor standards](https://www.sec.gov/news/press-release/2020-191)
- [FTX acquires Blockfolio](https://blockfolio.com/ftx) for $150 million
- [USDC v2](https://medium.com/centre-blog/centre-consortium-announces-release-of-usd-coin-version-2-0-37ee8b27e09b): adds permit for gasless transactions and more multisigs for administration
- Tokenized BTC (there’s now [more than 52000 BTC on ETH](https://btconethereum.com/)): [1 click to turn BTC to WBTC](https://medium.com/imtoken/the-new-btc-wbtc-1click-conversion-127ac51ce379) on imToken
- 0x’s new [request for quote system](https://blog.0xproject.com/growing-defi-with-the-help-of-professional-market-makers-0xs-new-request-for-quote-system-8d5fb08594bf) for professional market makers
- [Fairlaunch capital](https://twitter.com/fairlaunchcap/status/1298670543961329664) experiment in funding networks owned by their community from outset
- The [bear case for yield farming](https://bankless.substack.com/p/the-bear-case-for-yield-farming)
- Valuing ETH as [privately owned public infrastructure](https://medium.com/ether-capital-blog/the-ethereum-toll-road-aff45c1f15a7)

**Crypto/General**

- Three “[Obfuscation August](https://twitter.com/sweis/status/1298844185999454208)” papers: [Indistinguishability Obfuscation from Well-Founded Assumptions](https://eprint.iacr.org/2020/1003), [Indistinguishability Obfuscation from Circular Security](https://eprint.iacr.org/2020/1010), [Factoring and Pairings are not Necessary for iO: Circular-Secure LWE Suffices](https://eprint.iacr.org/2020/1024)
- Coinbase: [understanding accumulators by implementing](https://blog.coinbase.com/zksnarks-and-cryptographic-accumulators-f840da0b61c6) in Rust
- Hermez zk rollup on their [process of using multi-party ceremonies](https://blog.hermez.io/zero-knowledge-proofing-hermez-a-quick-guide-to-our-cryptographic-setup/)
- ETC 51% [attacked again with a reorg of 2 days](https://twitter.com/etherchain_org/status/1299822510607917056)

* * *

## **Job Listings**

- BnkToTheFuture is hiring a high performance dev team! Come [create the future](https://app.bnktothefuture.com/careers)!
- Celer Network is seeking Solidity and Go devs. Email: hiring@celer.network
- 0x is hiring [full-stack, back-end, front-end or Solidity](https://0x.org/about/jobs) devs
- Help Chainlink foster a security culture as a [security engineer](https://careers.smartcontract.com/o/senior-software-security-engineer)
- Trail of Bits: [blockchain security engineer](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & [cryptography analyst](https://jobs.lever.co/trailofbits/56af8506-3205-4c7b-b28d-ba8292bd1a47)[senior software engineers](https://jobs.lever.co/trailofbits/b9c65cdc-3fb9-4493-9073-73a4400f0e23)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH/DAI/USDC to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **If you want to sponsor newsletter, read this:**

The available sponsorship slots [were tokenized ($EVAN) for this newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer). You can now buy enough for a newsletter OTC from me at the spot price, or directly on [Balancer](https://balancer.exchange/#/swap/ether/0x89E3aC6Dd69C15e9223BE7649025d6F68Dab1d6a) - but you’ll likely get a better price from me.

Follow me on twitter: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-30-2020/](https://weekinethereumnews.com/week-in-ethereum-news-august-30-2020/)

Did you get **forwarded** this newsletter? **[Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **Sep 1 - BlockVigil’s free [online Eth developer bootcamp](https://medium.com/blockvigil/hackfs-results-remote-developer-bootcamp-announcement-cd3263757fe5) starts**
- Oct 2-30 - [EthOnline hackathon](https://www.ethonline.org/)
- Nov 6-7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)
- Nov 16 - [MetaMask Provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7)

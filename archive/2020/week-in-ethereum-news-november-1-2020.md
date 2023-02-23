---
title: "Week in Ethereum News <BR> November 1, 2020"
date: "2020-11-02"
---

## **Eth News and Links**

**Eth1**

- Retesteth [v0.9](https://github.com/ethereum/retesteth/releases/tag/v0.0.9-berlin), test suite for the Berlin hard fork
- Latest [core devs call](https://youtu.be/GOWSrHtNZOQ?t=239). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1322176445825736706). The BLS12-381 precompile (eip2537) is likely not going to be in the next hard fork, which is due in q1 2021. Fork tentatively is: EIP2315 (evm subroutines), EIP2929 (state access gas increase), EIP2718 (typed transaction envelope), EIP2930 (optional access lists) and EIP2565 (modexp precompile gas repricing)
- Turbogeth [weekly alpha release](https://twitter.com/realLedgerwatch/status/1321787473157083136), faster log storage
- Barnabé Monnot’s [1559 fee market/escalator jupyter notebook](https://nbviewer.jupyter.org/github/barnabemonnot/abm1559/blob/master/notebooks/floatingEscalator.ipynb) and [tweetstorm](https://twitter.com/barnabemonnot/status/1321797297529778176)

EIPs/standards

- [EIP3074](https://eips.ethereum.org/EIPS/eip-3074): Sponsored Transaction Precompile
- [ERC3076](https://eips.ethereum.org/EIPS/eip-3076): Validator client interchange standard
- [EIP3068](https://eips.ethereum.org/EIPS/eip-3068): precompile for BN256 HashToCurve Algorithms

**Proof of Stake launch**

- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_201031)
- Latest [eth2 call](https://youtu.be/_4Ry2AEzXGU?t=45). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/BJOIcBd_w)
- Open problem: [sub-second transaction latency using staggering](https://ethresear.ch/t/open-problem-incentive-compatible-sub-second-latency-via-staggering/8171)
- [Performance improvements](https://twitter.com/jcksie/status/1321366361348673536) in Nimbus from Medalla’s non-finality period
- Loredana’s [ewasm VM and debugger](https://www.reddit.com/r/ethereum/comments/jhst1g/ewasm_virtual_machine_and_debugger_for_ethereum_20/)
- [Armiarma](https://github.com/leobago/BSC-ETH2/blob/master/Armiarma/Armiarma.md) network crawler
- Medalla [exit tool](https://twitter.com/superphiz/status/1322165640006901761)
- “[all the things you wish you knew about staking](https://www.youtube.com/watch?v=tpkpW031RCI),” superphiz’s EthOnline talk

**Layer2**

- Nick Johnson: a general [bridge for eth layer2](https://medium.com/the-ethereum-name-service/a-general-purpose-bridge-for-ethereum-layer-2s-e28810ec1d88)

* * *

### **This newsletter is made possible thanks to [Trail of Bits!](https://www.trailofbits.com/)**

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F51a18ac3-6243-4bb9-8107-53cf06a46b26_1876x1128.png)](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F51a18ac3-6243-4bb9-8107-53cf06a46b26_1876x1128.png)

[Good idea, bad design: How the Diamond standard falls short](https://blog.trailofbits.com/2020/10/30/good-idea-bad-design-how-the-diamond-standard-falls-short/). We audited an implementation of the Diamond upgradeability proposal and can’t recommend it in its current form. It’s a laudable undertaking, but the Diamond proposal and its implementation raise many concerns. Still, there’s plenty to learn from it.

* * *

**Stuff for developers**

- OpenZeppelin’s [Defender](https://blog.openzeppelin.com/defender/), with contract administration, transaction relayer, autotask service to call contracts and guides for security best practices. [Andre Cronje is a fan](https://andrecronje.medium.com/keep3r-network-openzeppelin-defender-f320cfefd3d4)
- Solidity [v0.8.x preview](https://solidity.ethereum.org/2020/10/28/solidity-0.8.x-preview/). checked arithmetic operations by default
    - A [solidity team AMA](https://www.reddit.com/r/ethdev/comments/jigz5o/ask_the_solidity_team_anything_1/)
- Lightweight framework for [executing multi-step onchain workflows](https://omarish.com/2020/10/28/react-workflow.html)
- A [react hook Hardhat](https://www.npmjs.com/package/@symfoni/hardhat-react) plugin (fka Buidler)
- Multi-file verification in [Truffle via Rosco’s plugin](https://www.reddit.com/r/ethdev/comments/jizlj3/multifile_verification_in_trufflepluginverify_v050/)
- web3J [open API](https://blog.web3labs.com/web3j-open-api): generate API from your Solidity code
- Write a [call option in Solidity](https://blog.chain.link/defi-call-option-exchange-in-solidity/) with a Chainlink oracle
- The new [ethereum.org dev portal](https://blog.ethereum.org/2020/10/22/introducing-the-new-developer-portal/) - help make Eth dev easier to learn

**Security**

- Harvest attacked for 18m via [oracle depegging using flashloans](https://medium.com/harvest-finance/harvest-flashloan-economic-attack-post-mortem-3cf900d65217)
- Attacks as advertising: MakerDAO governance got “[friendly attacked” using flash loans](https://forum.makerdao.com/t/urgent-flash-loans-and-securing-the-maker-protocol/4901) by B protocol
- Trail of Bits finds [issues in Diamond implementation](https://blog.trailofbits.com/2020/10/30/good-idea-bad-design-how-the-diamond-standard-falls-short/). Nick Mudgen’s [response](https://dev.to/mudgen/addressing-josselin-feist-s-concern-s-of-eip-2535-diamond-standard-me8)
- a [yearn security disclosure](https://github.com/iearn-finance/yearn-security/blob/master/disclosures/2020-10-30.md)
- Nansen analyzes whale-heavy [SushiSwap farming](https://research.nansen.ai/sushiswap-farming/) and finds an exploit
- [Fuzzing your Solidity code with Echidna](https://medium.com/coinmonks/smart-contract-fuzzing-d9b88e0b0a05) tutorial

**Ecosystem**

- A [visualization of the Ethereum roadmap](https://twitter.com/trent_vanepps/status/1321936246332104705/photo/1)
- [Token allowances](https://cryptotesters.com/blog/token-allowances) and understanding them as a user
- ETHOnline [winners](https://twitter.com/ETHGlobal/status/1321898728198934528) and [submissions](https://hack.ethglobal.co/ethonline/showcase)

**Enterprise**

- Central bank digital currencies on Ethereum: ConsenSys selected by [Bank of Thailand](https://consensys.net/blog/press-release/consensys-selected-as-technology-partner-by-the-bank-of-thailand-for-cbdc-project/), [Societe General’s work with Banque de France,](https://consensys.net/blog/press-release/consensys-selected-by-societe-generale-forge-to-provide-technology-and-expertise-for-its-central-bank-digital-currency-experiments/) and the [Reserve Bank of Australia](https://consensys.net/blog/press-release/reserve-bank-of-australia-partners-with-commonwealth-bank-national-australia-bank-consensys-perpetual-on-wholesale-cbdc-project/)
- Paul Brody: [DeOps blockchain apps take the benefits of ERP for individual companies and spread it to entire supply chains](https://www.coindesk.com/how-blockchains-replace-erp-systems)
- JPMorganCoin (built on Quorum) “[being used commercially for the first time this week](https://www.cnbc.com/2020/10/27/jpmorgan-creates-new-unit-for-blockchain-projects-as-it-says-the-technology-is-close-to-making-money.html)”

**Application layer**

- [B.Protocol](https://medium.com/b-protocol/b-protocol-is-live-8d0971b77ef9) (of the [Maker flash loan incident](https://forum.makerdao.com/t/urgent-flash-loans-and-securing-the-maker-protocol/4901)) live on mainnet with its Maker liquidator that returns 50% of liquidations to users
- [dhedge live](https://medium.com/dhedge-org/dhedge-mainnet-is-live-72ed2c356d32) on mainnet, a social trading platform built on Synthetix
- [Autonomous lawyering](https://openlawesq.medium.com/autonomous-lawyering-using-openlaw-dad9c604975b) using OpenLaw (writing a memo for a network)
- ResearchCoin is giving away [1 million per week of its token to those who post or discuss academic research](https://medium.com/researchhub/were-giving-away-1m-researchcoin-every-week-to-accelerate-science-6b9da6c73da9)
- Augur adds [ETH trading](https://www.augur.net/blog/augur-ce/);
    - [Catnip.exchange](http://catnip.exchange/) nears 1m USD in daily volume on Trump or Biden market
- [](https://blog.oceanprotocol.com/ocean-v3-is-now-live-b47c0e73f52a)[Ocean v3](https://blog.oceanprotocol.com/ocean-v3-is-now-live-b47c0e73f52a) live on mainnet, with tokens representing access to the data set (and its value) and a data market built on balancer
- ReflexerLabs’ [Proto Rai stablecoin](https://medium.com/reflexer-labs/introducing-proto-rai-c4cf1f013ef) using PID controller has an unaudited demo on mainnet

**Regulation/business/tokens**

- Federal Reserve proposes [lowering Bank Secrecy Act transaction threshold to $250](https://www.federalreserve.gov/newsevents/pressreleases/bcreg20201023a.htm) from 3000; makes explicit that it applies to stablecoins
- [Anti-encryption EARN IT bill](https://act.eff.org/action/stop-the-earn-it-bill-before-it-breaks-encryption-a7904e20-2083-4d5e-88ae-44ee5fef7a5d) may get US Senate vote soon
- Michael del Castillo reports [Binance’s 2018 plan to evade US regulators](https://www.forbes.com/sites/michaeldelcastillo/2020/10/29/leaked-tai-chi-document-reveals-binances-elaborate-scheme-to-evade-bitcoin-regulators/#7805ba8d2a92)
- Iran [quasi-nationalizes crypto miners in attempt to thwart sanctions](http://www.irandaily.ir/News/275899.html)
- [Evolution of funding and organization](http://www.divraj.com/posts/evolution-of-funding-and-organization-in-crypto) in crypto
- [LexToken](https://lexdao.substack.com/p/launch-on-lextoken): cheap to deploy erc20, cheap batch mint/transfer, uses permit, adds details and resolver strings for real world assets

**General**

- [Deanonymizing the Kucoin hacker](https://medium.com/@weijiek/deanonymising-the-kucoin-hacker-418fa5e9911d)
- Singaporean bank [DBS deleted a new digital assets exchange page](https://www.coindesk.com/singapore-bank-dbs-looks-to-be-planning-a-digital-asset-exchange) on its website when crypto twitter found it
- Cypherpunks video series, [final part](https://youtu.be/HDKQulqVCQg)
- Be careful: there has been a sustained [Ledger impersonation phishing attempt](https://twitter.com/Ledger/status/1318294484208279556)

* * *

## **Job Listings**

- Join Status and help drive the [JS implementation of Waku and Integrations](https://status.im/our_team/open_positions.html?gh_jid=2385338)
- Mainframe is hiring a [Solidity Smart Contract Engineer](https://cryptocurrencyjobs.co/engineering/mainframe-solidity-smart-contract-engineer/)
- Celer hiring Solidity and Go devs. Email: hiring@celer.network
- 0x looking for [Matcha marketing manager](https://boards.greenhouse.io/0x/jobs/4923909002) and [all flavors of developers](https://0x.org/about/jobs)
- Chainlink has [30+ openings at the moment](https://jobs.lever.co/chainlink/) across marketing, ops, & devs
- Trail of Bits hiring [cryptography analyst](https://jobs.lever.co/trailofbits/56af8506-3205-4c7b-b28d-ba8292bd1a47) & [blockchain security engineers](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **Download The Crypto News Podcast**

Episode 1: [Taylor Monahan](https://thecryptonewspodcast.com/mycrypto-ceo-taylor-monahan)

It’s no secret that I think podcasts are (much) better businesses than newsletters. So if you want to support the newsletter, download and subscribe to my podcast!

[Taylor and I had a fun chat](https://thecryptonewspodcast.com/mycrypto-ceo-taylor-monahan) about the latest in DeFi, please check it out and leave a review on your podcasting app of choice. I think you'll like it.

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow the newsletter on twitter: [@WeekinEthNews](https://twitter.com/WeekInEthNews)

Permalink for this week’s issue:  [https://weekinethereumnews.com/week-in-ethereum-news-november-1-2020/](https://weekinethereumnews.com/week-in-ethereum-news-november-1-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Nov 6-7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)
- **Nov 12-13 - [Baseline Protocol Summit](https://www.eventbrite.com/e/baseline-protocol-summit-2020-registration-125941465313)**
- Nov 16 - [MetaMask Provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7)
- Nov 19 - EthBerlin 2.5: [Talk Show](https://medium.com/ethberlin/move-over-netflix-theres-a-new-zoom-talk-show-in-town-db48c75d35af)
- Dec 3 - [Ethereum in the Enterprise - Asia Pacific](https://twitter.com/EntEthAlliance/status/1314652848655872000)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

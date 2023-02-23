---
title: "Week in Ethereum News <BR> November 15, 2020"
date: "2020-11-15"
---

## **Eth News and Links**

**Eth1**

- Geth [found a Golang bug](https://blog.ethereum.org/2020/11/12/geth_security_release/) (the [second Golang bug found by Ethereum](https://twitter.com/drakefjustin/status/1326996515416576005) in a few months), so:
    - Immediately update to geth [v1.9.24](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.24)
    - In the future, update your node (at least) every time a release says “security”
- On Wednesday, [Infura went down](https://blog.infura.io/infura-mainnet-outage-post-mortem-2020-11-11/) for a few hours because it hadn’t updated some geth versions for a few months. Apparently some tiny percent of mining hash power also hadn’t updated and produced a few blocks on a different chain over a few hours
- The Optimism team [sparked the issue](https://twitter.com/jinglanW/status/1326651349912719360) because they’d found the bug that had led the geth team to update.
- Deep into the [technical weeds of the issue](https://twitter.com/lightclients/status/1326947036961239042)
- Geth team post mortem explains [why it does what it does](https://gist.github.com/karalabe/e1891c8a99fdc16c4e60d9713c35401f).
- Latest [core devs call](https://www.youtube.com/watch?v=5-614J9qNvY). Beiko’s [notes](https://twitter.com/TimBeiko/status/1327249352205615106): working through issues to get to consensus for the Berlin fork
- Latest [update on 1559](https://hackmd.io/@timbeiko/1559-updates/https%3A%2F%2Fhackmd.io%2F%40timbeiko%2F1559-update-003): testnets, tools, simulations
- [Alexandria state relayer p2p network](https://snakecharmers.ethereum.org/alexandria-dev-update-1/) update: use SSZ to transmit via UDP

**Proof of Stake launch**

- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_201113)
- Latest [eth2 quick update](https://blog.ethereum.org/2020/11/13/eth2-quick-update-no-20/) from Danny Ryan; Toledo and Pyrmont testnets pre-launch
- [Staking community grants](https://ethereum.org/en/eth2/get-involved/staking-community-grants/) for tools, documentation and education
- Latest [eth2 call](https://youtu.be/yFjs_tB6I-Y?t=147). Notes from [Mamy](https://gist.github.com/mratsim/6c3ced507236af7d2995fa74f1a1a380) and [Ben](https://hackmd.io/@benjaminion/B1GPwjcKP). Roadmap priorities: data shards, light clients, end PoW.
- The SigmaPrime fuzzer finds [2 prysm consensus bugs and 1 very minor Teku bug](https://blog.sigmaprime.io/beacon-fuzz-09.html)
- proof of stake [forkmon](https://eth2-fork-mon.stokes.io/) (fork monitoring tool)
- Barcelona Super Computer [client benchmarking](https://github.com/leobago/BSC-ETH2/blob/master/report/Clients_behaviour_report.pdf)
- Client updates: [Lighthouse](https://lighthouse.sigmaprime.io/update-32.html), [Nimbus](https://our.status.im/nimbus-update-november-10/), [Prysm](https://medium.com/prysmatic-labs/upcoming-prysm-v1-release-afea046d7ea1), [Teku](https://github.com/ConsenSys/teku/releases/tag/0.12.14). The gist is to watch for mainnet releases for the chain launch.
- a [FAQ for those considering staking](https://www.reddit.com/r/ethstaker/comments/ju61pf/ethstaker_faq/) and some [staking best practices](https://docs.google.com/document/d/1WZuP-K0S4RKlwH4GQVcGpgzVYPdpZF0WiHsawnmOKxM/edit)

**Layer2**

- Celer’s [State Guardian Network first phase launch](https://blog.celer.network/2020/11/09/celer-state-guardian-network-launches-on-mainnet/)
- Fuel: layer2 will turn the [Eth basechain into an asset creation & settlement layer](https://fuellabs.medium.com/the-future-of-l1-ethereum-5ec5d9a01c10)

* * *

### **This newsletter is made possible thanks to Chainlink!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/05/FE39n5_g.png)

The Chainlink community grant program provides substantial financial support to teams and individuals who are developing critical tools, infrastructure, and services that increase the usefulness and accessibility of smart contracts. [Explore our open grants.](https://chn.lk/grants)

* * *

**Stuff for developers**

- [EthereumNodes](https://ethereumnodes.com/) - dashboard of public RPC endpoints
- [Miao](https://kndrck.co/posts/miao-evm-tx-decoder/): Kendrick Tan’s EVM tx decoder with no external data processing
- toolkit for TheGraph with [functions commonly used by subgraph mappings](https://github.com/Amxx/graphprotocol-utils)
- [Railroad diagrams for Solidity and Vyper](https://www.reddit.com/r/ethdev/comments/jr65tk/railroad_diagrams_of_solidity_and_vyper_antlr4/)
- [OpenZeppelin Contracts Upgradable](https://forum.openzeppelin.com/t/first-release-of-openzeppelin-contracts-upgradeable/4548)
- [Testing Eth code](https://blog.chain.link/testing-chainlink-smart-contracts/) with Chainlink
- [Speculative execution via GraphQL endpoint](https://dfuse.io/en/announcing-speculative-execution-for-ethereum/) from dfuse

**Security**

- Samczsun’s [using price oracles](https://samczsun.com/so-you-want-to-use-a-price-oracle/) opus
- Perez, Livshits paper: [“vulnerable” Eth code does not mean exploited](https://arxiv.org/pdf/1902.06710)
- Slither [v0.6.14](https://github.com/crytic/slither/releases/tag/0.6.14), improves Solidity v0.7 support, works with Hardhat
- Certora finds [ABIencoder bug](https://www.certora.com/blog/confusedABI.html)
- Akropolis [reentrancy bug hacked for 2m Dai](https://medium.com/@peckshield/akropolis-incident-root-cause-analysis-c11ee59e05d4)
- ValueDefi (formerly yfv) tweets that it has the “highest security,” then gets an [oracle attack a few hours later for $7.4m](https://medium.com/@peckshield/value-defi-incident-root-cause-analysis-fbab71faf373) hack peckshield

**Ecosystem**

- Solidity code in [Ariana Grande’s latest video](https://twitter.com/jzlegion/status/1325993150238793728)
- [Umbra stealth payments](https://www.scopelift.co/blog/umbra-update) still coming; some funding issues
- Petkanics: [observations after 4 years building web3 apps](https://petkanics.medium.com/observations-at-the-four-year-mark-of-a-web3-protocol-build-fad1df5e1728)

**Enterprise**

- [Accenture, Splunk, and others join Baseline Protocol](https://www.einpresswire.com/article/530331948/accenture-splunk-and-others-back-baseline-protocol-for-public-blockchains)
- ETHOnline [enterprise panel featuring EY, Microsoft, and BP](https://www.youtube.com/watch?v=6yj4Rt927n0)

**Application layer**

- Maker hit [one billion dai](https://twitter.com/MakerDAO/status/1327335078477774848) this week
- Synthetix offers [oil derivatives](https://blog.synthetix.io/soil-ioil/) using Brent Crude (ICE)
- Enjin makes its token/game item [platform free](https://blog.enjin.io/free-platform/) of subscription fees
- Etherisc offering [crop insurance in Kenya](https://blog.etherisc.com/etherisc-teams-up-with-chainlink-to-deliver-crop-insurance-in-kenya-137e433c29dc)
- [Aave v2 is on Kovan](https://medium.com/aave/aave-v2-is-available-on-public-testnet-dc13e3dca2b) testnet

**Regulation/business/tokens**

- UK Treasury publishes [draft of stablecoin regulations](https://www.theblockcrypto.com/linked/84148/uk-treasury-to-publish-draft-stablecoin-regulations)
- US House left wingers criticize [Comptroller Brian Brooks for too much crypto focus](https://www.coindesk.com/us-representatives-blast-occ-crypto)

**General**

- [BDoS](https://twitter.com/aklamun/status/1326199789978066946) - incentive manipulation to stop Bitcoin liveness with just 21% of hashpower
- “Computer scientists achieve “[Crown jewel” of cryptography](https://www.quantamagazine.org/computer-scientists-achieve-crown-jewel-of-cryptography-20201110/)”
- Non-interactive [threshold ECDSA signatures](https://dl.acm.org/doi/10.1145/3372297.3423367)
- Another week, [another SGX hack](https://www.usenix.org/system/files/sec21summer_chen-zitai.pdf)
- Brave fighting [CNAME cloaking](https://brave.com/privacy-updates-6/)
- [Macs send (unencrypted!) to Apple](https://sneak.berlin/20201112/your-computer-isnt-yours/) every app you use, your IP address, etc

* * *

## **Job Listings**

- [Blocknative](https://www.blocknative.com/) is hiring [Front-end, Back-end, and DevOps engineers](https://jobs.lever.co/blocknative?lever-origin=applied&lever-source=thisweekinETH). (Remote)
- Live for DeFi? [mStable](https://mstable.org/) seeks experienced [Smart Contract/Protocol Dev](https://cryptocurrencyjobs.co/engineering/mstable-protocol-developer-defi/)
- Chainlink Labs is looking for a [Director of BD & Sales](https://jobs.lever.co/chainlink/d35cff18-ffc6-41fe-98b2-b86f960e2f88?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Celer hiring Solidity and Go devs. Email: hiring@celer.network
- 0x looking for [Matcha marketing manager](https://boards.greenhouse.io/0x/jobs/4923909002) and [all flavors of developers](https://0x.org/about/jobs)
- Trail of Bits is hiring [cryptography analyst](https://jobs.lever.co/trailofbits/56af8506-3205-4c7b-b28d-ba8292bd1a47) & [blockchain security engs](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **Download The Crypto News Podcast**

Episode 3: ZapperFi’s [DefiDad](https://thecryptonewspodcast.com/defidad)

How’d he gain more than 25,000 Twitter followers in less than a year?

If you want to support Week in Ethereum News, download and subscribe to my podcast!

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow the newsletter on twitter: [@WeekinEthNews](https://twitter.com/WeekInEthNews)

Permalink for this week’s issue:  [https://weekinethereumnews.com/week-in-ethereum-news-november-15-2020/](https://weekinethereumnews.com/week-in-ethereum-news-november-15-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Nov 16 - [MetaMask Provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7)
- **Nov 18 - [Pyrmont testnet](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_201113) launch**
- Nov 19 - EthBerlin 2.5: [Talk Show](https://twopointfive.online/)
- Nov 24 - last day to deposit to be in proof of stake genesis block
- Dec 1 - [Proof of stake launch](https://blog.ethereum.org/2020/11/04/eth2-quick-update-no-19/) (if enough deposits by Nov 24)
- **Dec 2 - [Gitcoin CLR matching](https://gitcoin.co/grants) round starts**
- Dec 3 - [Ethereum in the Enterprise - Asia Pacific](https://twitter.com/EntEthAlliance/status/1314652848655872000)
- **Dec 22 - Deadline to apply for [proof of stake community grants](https://ethereum.org/en/eth2/get-involved/staking-community-grants/)**
- **Mar 2-4 - [EthCC4](https://ethcc.io/) (Paris)**

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

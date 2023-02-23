---
title: "Week in Ethereum News <BR> November 22, 2020"
date: "2020-11-22"
---

## **Eth News and Links**

**Eth1**

- How to have a lightweight [Nethermind node for eth2 staking](https://twitter.com/nethermindeth/status/1329931101268283392)
- The [current hard fork planning](https://medium.com/ethereum-cat-herders/shedding-light-on-the-ethereum-network-upgrade-process-4c6186ed442c) process as it goes into the Berlin fork/upgrade
- Account abstraction [community call](https://www.youtube.com/watch?v=0hAIjLFe38Y)
- An [account abstraction technical explainer](https://our.status.im/account-abstraction-eip-2938/) from Status

**Proof of Stake launch**

- We have over [50% of the ETH in the deposit contract necessary to launch the chain](https://etherscan.io/address/0x00000000219ab540356cbb839cbe05303d7705fa).
- [Eth research AMA](https://www.reddit.com/r/ethereum/comments/jvkoat/ama_we_are_the_efs_eth_20_research_team_pt_5_18/): explicit statement that data shards (“phase 1”) and swapping out PoW for PoS (commonly called “the merge” or “phase 1.5”) are getting spec’d independently and are not dependent on each other. That means ending PoW _could_ happen before data shards, though it probably will not.
- [Data availability sampling](https://hackmd.io/@HWeNw8hNRimMm2m2GH56Cw/r1XzqYIOv) proposal
- [Medalla data challenge results](https://blog.ethereum.org/2020/11/17/medalla-data-challenge-results/) - top prize to Jim McDonald’s [chaind](https://github.com/wealdtech/chaind) and Pintail
- Eth2 deposit CLI [v1.1](https://github.com/ethereum/eth2.0-deposit-cli/releases/tag/v1.1.0), adds Pyrmont testnet
- [Ledger Nano X now supports eth2](https://www.ledger.com/blog/ledger-is-ready-for-ethereum-2) (but not Ledger Nano S)
- Somer Esat’s guides to staking updated for Pyrmont testnet:
    - [Lighthouse](https://someresat.medium.com/guide-to-staking-on-ethereum-2-0-ubuntu-pyrmont-lighthouse-a634d3b87393), [Prysm](https://someresat.medium.com/guide-to-staking-on-ethereum-2-0-ubuntu-pyrmont-prysm-a10b5129c7e3), [Teku](https://someresat.medium.com/guide-to-staking-on-ethereum-2-0-testnet-ubuntu-pyrmont-teku-3da74372910)
- Running an [eth validator for the barely motivated](https://bankless.substack.com/p/running-an-eth-validator-for-the)
- Dankrad: [staking on a Raspberry Pi](https://dankradfeist.de/ethereum/2020/11/20/staking-on-raspi.html)

**Layer2**

- Connext’s [cross-layer 2 via channels](https://medium.com/connext/instant-cross-l2-transfers-are-now-on-testnet-2f1295530c22) on testnet
- Zk [rollups with data shards](https://ethresear.ch/t/rollups-on-a-data-sharded-ethereum-2-linking-the-data-availability-with-the-execution/8237): linking the data availability with the execution

* * *

### **This newsletter is made possible thanks to [Celer](https://www.celer.network/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

We are excited to announce that [Phase One of the Celer State Guardian Network (SGN) mainnet](https://blog.celer.network/2020/11/09/celer-state-guardian-network-launches-on-mainnet/) is now up and running! Staking will start from December 1, 2020. SGN is the last piece of Celer Network’s coherent layer-2 scaling platform. This launch marks another significant milestone of the Celer layer-2 blockchain scaling platform after our [State Channel Network](https://www.celer.network/docs/celercore/index.html), which was successfully launched more than a year ago and supports hundreds of thousands of users today. 

Real money games, such as [Arcade Win](https://apps.apple.com/us/app/arcade-win/id1459895768) and [Daub Cash](https://apps.apple.com/us/app/daub-cash/id1513396754), built using [Celer’s gaming-focused SDK](http://developer.celerx.app/) just reached top #10 ranking in App Store.

Follow us on [twitter](https://twitter.com/CelerNetwork), [blog](https://blog.celer.network/), [discord](https://discord.com/invite/Trhab5w) and [telegram](https://t.me/celernetwork).

* * *

**Stuff for developers**

- Nomic Labs on a [year massively improving the Eth dev experience](https://medium.com/nomic-labs-blog/nomic-labs-devx-1-year-working-on-ethereum-developer-experience-66ed0a43bbed)
- Solidity [v0.7.5](https://blog.soliditylang.org/2020/11/18/solidity-0.7.5-release-announcement/) - switch between ABI encoder v1 and v2, also experimental Yul-based compiler pipeline
- Prettier Solidity plugin gets a [first beta release](https://github.com/prettier-solidity/prettier-plugin-solidity/releases/tag/v1.0.0-beta.1)
- If you can open a terminal, you can [create an ERC20 token with scaffold-eth](https://www.linumlabs.com/articles/create-an-open-zeppelin-erc20-in-scaffold-eth-with-great-ease) and OpenZeppelin contracts
- Update on [Fe Python-like language development](https://snakecharmers.ethereum.org/fe-development-update-1/)
- web3j [v4.8](https://www.reddit.com/r/ethdev/comments/jter2r/web3j_v48_release_updates/)
- [Ette](https://github.com/itzmeanjan/ette): block, transaction and event indexing in PostgreSQL, query via REST API
- Quiknode’s [Etherflow](https://blog.quiknode.io/introducing-etherflow-by-quiknode/) node debugging tool, supports web3js and ethersjs

**Security**

- Pickle [attacked for 19.8m Dai](https://github.com/banteg/evil-jar/blob/master/readme.md) by deploying evil jars.
- Samczsun finds [attack-in-process on 88mph](https://medium.com/88mphapp/88mph-mphminter-contract-issue-6365dbcacb4f). 88mph thwarts the attack and will distribute the attacker’s $100k to users
- Attacker finds [re-entrancy in Origin Protocol to steal](https://medium.com/originprotocol/urgent-ousd-has-hacked-and-there-has-been-a-loss-of-funds-7b8c4a7d534c) $8m
- Cheesebank got hit in a [flashloan oracle depegging for 3.3m](https://cheesebank2020.medium.com/cheese-bank-detailed-statement-a765372dd84f)
- Consensys Diligence [token interaction checklist](https://consensys.net/diligence/blog/2020/11/token-interaction-checklist/)
- An explanation of [challenge #1 of DamnVulnerableDefi](https://medium.com/@iphelix/damn-vulnerable-defi-setup-and-challenge-1-walkthrough-1ea16ea09709)

**Ecosystem**

- Why has decentralized proof of stake taken 6 years? [Jeff Coleman answers](https://twitter.com/technocrypto/status/1330150362427387910)
- Circle, AirTM, and the US federal government work with Juan Guaido’s dissident government to [provide aid to Venezuela using USDC](https://www.circle.com/blog/circle-partners-with-bolivarian-republic-of-venezuela-and-airtm-to-deliver-aid-to-venezuelans-using-usdc).

**Application layer**

- Post-Uniswap farming ending, Maker back on top for most value locked (no link)
- In response, competitors like [1inch](https://1inch-exchange.medium.com/liquidity-mining-update-1inch-announces-stage-2-of-liquidity-mining-program-43352f32d868) and dxDAO’s [Swapr](https://medium.com/swapr/dxdao-announces-swapr-becoming-the-first-dao-to-launch-a-defi-protocol-on-ethereum-d45c291ae86a) offering incentives. Uniswap governance [discussing whether to offer more incentives](https://gov.uniswap.org/t/discussion-uniswap-liquidity-incentive-plan/8590)
- 0x’s Matcha dex [aggregator adds 1000+ tokens](https://matcha.xyz/blog/trade-any-token)
- How Livepeer’s [decentralized transcoding is better than centralized](https://livepeer.com/blog/livepeer-always-on-transcoding-network): no bootup time means no need to reserve transcoding server 24/7
- Streamr’s [data union framework is live](https://blog.streamr.network/data-union-concept-ideas/)
- Quadratic funding experiments: Austin Griffith’s [build guild](https://medium.com/@austin_48503/buidl-guidl-round-1-unaudited-4e1d9456e43d) (donate to support next generation of Eth devs!) and [CLR fund](https://blog.clr.fund/round-0-review-round-1-launch/) (uses MACI so donations are private!)

**Regulation/business/tokens**

- SEC [no action letter](https://www.sec.gov/corpfin/imvu-111920-2a1) for IMVU social network emphasizes that the network is usable on day 1 and the token has a fixed price.
    - tldr: SEC will still only issue no action letters if it’s ridiculously far away from being a security and breaks just about every prong of the _Howey_ test
- [OCC proposes banning Obama’s Operation Chokepoint](https://www.occ.treas.gov/news-issuances/news-releases/2020/nr-occ-2020-156.html). This would mandate fair banking access for legal products like crypto
- AirBnB explicitly mentions [tokenization as a future possibility](https://www.sec.gov/Archives/edgar/data/1559720/000119312520294801/d81668ds1.htm) in IPO paperwork

**General**

- Github [restores youtube-dl](https://github.blog/2020-11-16-standing-up-for-developers-youtube-dl-is-back/) reversing a DMCA takedown and donates $1m to DMCA defense fund
- Godaddy employees get [social engineered to attack crypto sites](https://krebsonsecurity.com/2020/11/godaddy-employees-used-in-attacks-on-multiple-cryptocurrency-services/)

* * *

## **Job Listings**

- Nexus Mutual: [experienced Solidity dev](https://angel.co/company/nexus-mutual-1/jobs/967538-smart-contract-engineer) in Euro timezones
- Celer hiring Solidity and Go devs. Email: hiring@celer.network
- 0x looking for [Matcha marketing manager](https://boards.greenhouse.io/0x/jobs/4923909002) and [all flavors of developers](https://0x.org/about/jobs)
- Join Chainlink Labs as a [Developer Advocate](https://jobs.lever.co/chainlink/b5cfde5c-4a1f-42dd-869f-87bd1010fb4e?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Trail of Bits is hiring [cryptography analyst](https://jobs.lever.co/trailofbits/56af8506-3205-4c7b-b28d-ba8292bd1a47) & [blockchain security devs](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow the newsletter on twitter: [@WeekinEthNews](https://twitter.com/WeekInEthNews)

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-november-22-2020/](https://weekinethereumnews.com/week-in-ethereum-news-november-22-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Nov 24 - **last day to deposit** to be in proof of stake genesis block
- Dec 1 - [Proof of stake launch](https://blog.ethereum.org/2020/11/04/eth2-quick-update-no-19/) (if enough deposits by Nov 24)
- Dec 2 - [Gitcoin CLR matching](https://gitcoin.co/grants) round starts
- Dec 3 - [Ethereum in the Enterprise: Asia Pacific 2020](https://entethalliance.org/ethereum-in-the-enterprise-asia-pacific-2020/)
- Dec 22 - Deadline to apply for [proof of stake community grants](https://ethereum.org/en/eth2/get-involved/staking-community-grants/)
- **Feb 5-12 - [ETHDenver](https://twitter.com/EthereumDenver/status/1328367230707396609) (virtual)**
- **Mar 2-4 - [EthCC4](https://ethcc.io/) (Paris)**

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

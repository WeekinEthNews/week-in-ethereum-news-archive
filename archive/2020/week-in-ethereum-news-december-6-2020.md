---
title: "Week in Ethereum News <BR> Dec 6, 2020"
date: "2020-12-06"
---

## **Eth News and Links**

**Eth1**

- Leading game theorist Tim Roughgarden [publishes his positive analysis of 1559](http://timroughgarden.org/papers/eip1559.pdf)
- Latest [eip1559 implementation](https://www.youtube.com/watch?v=dopljpI59Rw&feature=youtu.be) call. [Beiko’s notes](https://twitter.com/TimBeiko/status/1334571129671806976), with a path to mainnet
- A [code merkleization explainer](https://blog.ethereum.org/2020/11/30/the-1x-files-code-merkleization/)

**Proof of Stake launches successfully**

- The Beacon chain launched, with the first block graffiti reading “Mr F was here” ([beaconscan](https://beaconscan.com/slot/1), [beaconchain](https://beaconcha.in/block/1)) and the network participation rate quickly reaching an astonishing 98-99% ([beaconchain](https://beaconcha.in/charts/participation_rate), [beaconscan](https://beaconscan.com/stat/networkparticipation))
- Meanwhile the deposit contract is [over 1m ETH](https://etherchain.org/account/0x00000000219ab540356cbb839cbe05303d7705fa), so now more than 1% of all ETH is locked for staking. That number is only going to go up, right now that puts annual staking rewards at 14.6%. That means the network is [continually increasing its decentralization](https://twitter.com/VitalikButerin/status/1333738057162362880)
- There have been [3 slashing events](https://twitter.com/benjaminion_xyz/status/1334881186003492864), all by stakers (and a pool known as Ankr) running their keys on multiple machines. This was already a known bad idea! Slashing is bad, going offline is very insignificant in comparison
- Before genesis, Prysmatic published [slashing prevention tips](https://medium.com/prysmatic-labs/eth2-slashing-prevention-tips-f6faa5025f50). It emphasized that you should never run your key in multiple places.
- Pre-launch [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_201130)
- Superphiz: hold off on [staking with trusted pools/exchanges](https://www.youtube.com/watch?v=qh4q8B2GSds&feature=youtu.be)

**Proof of Stake plans**

- Latest [eth2 call](https://youtu.be/8mE--yxMZtk?t=23). Notes from [Ben](https://hackmd.io/@benjaminion/SJphODIiv) and [Mamy](https://gist.github.com/mratsim/d35a5171c52d3b998b492e9512f6cee7)
- Shift [computing costs from end of epoch to mid-epoch](https://hackmd.io/@HWeNw8hNRimMm2m2GH56Cw/HkTzLKOov)

**Layer2**

- Loopring’s [AMM is live on their zkrollup](https://medium.com/loopring-protocol/looprings-zkrollup-amm-is-live-2f8251cd0fcd) (though limited to LRC/ETH for now)
- Golem’s latest release uses [Zksync zkrollup for transfers](https://blog.golemproject.net/new-golem-alpha-iii-reveal/)
- Deversifi’s validium (off-chain data held by committee) upgrades to [StarkEx v2](https://medium.com/starkware/starkex-2-0-is-now-live-on-mainnet-d8768b860bd4) which includes fast withdrawals and a Turing-complete STARK proof language, though non-conformant ERC20 tokens (OMG, USDT) won’t [work for another month](https://blog.deversifi.com/a-tale-of-intrigue-non-standard-erc20-tokens-and-platform-upgrades/)

* * *

### **This newsletter is made possible thanks to [Matcha](https://matcha.xyz/?id=wien) by [0x](https://0x.org/)!**

![Matcha](https://weekinethereumnews.com/wp-content/uploads/2020/06/matcha-avatar.png)

Matcha aggregates liquidity across decentralized exchange networks to offer you the best price on every token swap. 

Now you can [trade 1000+ DeFi tokens](https://matcha.xyz/?id=wien) on Matcha!

* * *

**Stuff for developers**

- [Solidity Underhanded Contest winners](https://blog.soliditylang.org/2020/12/03/solidity-underhanded-contest-winners/)
- Exploring [eth2 attestation rates with chaind](https://www.symphonious.net/2020/12/04/exploring-eth2-attestation-inclusion-rates-with-chaind/)
- [4byte.directory now has event signatures](https://www.4byte.directory/event-signatures/)
- Video from latest [dev onboarding call](https://www.youtube.com/watch?v=ipFJeK0M5ks&feature=youtu.be)
- Infura buys [anysender and releases it as Infura transactions](https://blog.infura.io/announcing-our-acquisition-of-any-sender-and-the-alpha-release-of-infura-transactions) (relayer that auto-bumps gasprice) on testnet
- “Decentralized Github” [Radicle’s first public release](https://twitter.com/radicle/status/1333403629961797635)
- A (non-audited) package of [code for using different oracles](https://www.npmjs.com/package/usm-oracles)
- RicMoo’s [ethersJS update](https://blog.ricmoo.com/highlights-ethers-js-december-2020-2e2db8bc800a); eip712, React native testing

**Security and incidents**

- [Ethernaut updated](https://ethernaut.openzeppelin.com/) to Solidity v0.6 and web3js v1.2.7
- Rari had a [logic error leading to an overflow](https://medium.com/rari-capital/rari-capital-11-29-2020-bug-resolved-and-deployed-acaecc6a313b); fixed and no funds lost
- Saffron had a bug where [SFI got locked for 8 weeks](https://medium.com/saffron-finance/saffron-epoch-1-recovery-d10b84c95940)
- [15k hacked from Sushiswap](https://rekt.ghost.io/sushiswap-saved-0xmaki-speaks-out/)
- CP3R [rug pulls for $11m](https://rekt.ghost.io/deathbed-confessions-c3pr/)

**Ecosystem**

- Vitalik updates [his version of Ethereum’s roadmap](https://twitter.com/VitalikButerin/status/1333922620857745408) with progress bars
- Johoe’s “mempool statistics” now [includes the Ethereum transaction pool](https://jochen-hoenicke.de/queue/#2,24h)
- [Ethereum passes Bitcoin in node count](https://twitter.com/etherchain_org/status/1333173744089640960)

**Enterprise**

- [Visa partners with Circle](https://www.forbes.com/sites/michaeldelcastillo/2020/12/02/visa-partners-with-ethereum-digital-dollar-startup-that-raised-271-million/) to help card issuers integrate USDC so you can spend USDC with your card
- [Baseline as a service demo day](https://medium.com/unibrightio/baseline-as-a-service-demo-day-b5ceb2fadb8d) on Dec 10
- [Layer2 knocks down barriers for enterprise](https://entethalliance.org/how-ethereum-layer-2-scaling-solutions-address-barriers-to-enterprises-building-on-mainnet/) to use mainnet

**Application layer**

- [Aave v2](https://medium.com/aave/the-aave-protocol-v2-f06f299cee04) is live. Native credit delegation, gas optimizations, swap collateral, fixed and variable rate borrowing
- Nexus Mutual unveils [cover for some centralized custodians](https://medium.com/nexus-mutual/custody-cover-is-now-live-7737c45367b8)
- 1inch now [submits your transactions directly to miners](https://twitter.com/1inchExchange/status/1334992381242961930) to avoid some frontrunners
- this week’s yearn m&a: [Sushi](https://medium.com/iearn/yearn-x-sushi-%E8%A1%8C%E3%81%A3%E3%81%A6%E3%81%8D%E3%81%BE%E3%81%99-41b2f78b62e9) and [Akropolis](https://medium.com/iearn/%CE%BC%CE%B1-%CF%84%CE%BF%CE%BD-%CE%B4%CE%B9%CE%B1-yearn-x-akropolis-16f5351af35e)
- Paradigm’s Uniswap problems: [liquidity providers can beat impermanent loss](https://research.paradigm.xyz/uniswaps-alchemy)
- A [gas futures token](https://medium.com/uma-project/ulabs-gas-futures-token-9f51682778dd) launches on UMA so you can hedge gasprices going up

**Regulation/business/tokens**

- Messari report: [Eth2 is the evolution of the cryptoeconomy](https://twitter.com/RyanWatkins_/status/1334327593827504130)
- Canada’s Ether Cap becomes [first public company to stake ETH](https://www.businesswire.com/news/home/20201201005696/en/Ether-Capital-Corporation-Announces-Initial-Commitment-to-Staking-on-Ethereum-2.0)
- S&P to issue [Dow Jones branded crypto indexes](https://www.spglobal.com/spdji/en/corporate-news/article/sp-dow-jones-indices-builds-crypto-indexing-capabilities-with-lukka/) next year
- A [fund buys OmiseGo](https://gbv.capital/gbv-omg-synqa/) from Omise/Synqa
- Congressional Democrats all-in against crypto this week: 1) left-wingers propose STABLE Act [regulations against stablecoins and running a node](https://tlaib.house.gov/media/press-releases/tlaib-garcia-and-lynch-stableact). 2) House Banking Committee chair Maxine Waters asks Biden to [repeal OCC’s crypto-friendly rules](https://financialservices.house.gov/uploadedfiles/120420_cmw_ltr_to_biden.pdf)

**General**

- [MyCrypto Winter](https://winter.mycrypto.com/) returns; an advent calendar with security tips (and prizes!)
- Shapeshift’s [FoxCrypt](https://foxcry.pt/): one time message encyption
- Phone [apps sell your location data](https://www.vice.com/en/article/epdpdm/ice-dhs-fbi-location-data-venntel-apps) to everyone

* * *

## **Job Listings**

- Circle is hiring! **Please check us out**: [https://www.circle.com/en/careers](https://www.circle.com/en/careers)
- Linum Labs is hiring a [CTO & a Fullstack developer](https://angel.co/company/linum-labs/jobs) (Remote)
- 0x looking for [devs of all types](https://0x.org/about/jobs) and a [Matcha marketing manager](https://boards.greenhouse.io/0x/jobs/4923909002)
- Expand Chainlink Labs’ presence as the [Head of Sales](https://jobs.lever.co/chainlink/6bb12110-439a-4033-9b7c-d5e0baaf33ed?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Trail of Bits is hiring [blockchain security devs](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & [cryptography analyst](https://jobs.lever.co/trailofbits/56af8506-3205-4c7b-b28d-ba8292bd1a47)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow the newsletter on twitter: [@WeekinEthNews](https://twitter.com/WeekInEthNews)

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-dec-6-2020/](https://weekinethereumnews.com/week-in-ethereum-news-dec-6-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **Dec 17 - [Gitcoin grants matching](https://gitcoin.co/grants) ends (here’s [Week in Eth News](https://gitcoin.co/grants/237/week-in-ethereum-news))**
- Dec 22 - Deadline to apply for [proof of stake community grants](https://ethereum.org/en/eth2/get-involved/staking-community-grants/)
- Feb 5-12 - [ETHDenver](https://twitter.com/EthereumDenver/status/1328367230707396609) (virtual)
- Mar 2-4 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

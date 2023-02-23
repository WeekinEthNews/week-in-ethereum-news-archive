---
title: "Week in Ethereum News <BR> November 29, 2020"
date: "2020-11-29"
---

## **Eth News and Links**

**Eth1**

- Nethermind [v1.9.39](https://github.com/NethermindEth/nethermind/releases/tag/1.9.39) - update if you’re [using Nethermind for your eth2 staking](https://medium.com/nethermind-eth/an-important-announcement-from-the-nethermind-team-c31ce785b7f1)
- A writeup of some [Nethermind (written in .NET core) performance improvements](https://blog.scooletz.com/2020/11/23/improving-Nethermind-performance)
- [EthereumJS VM v5](https://blog.ethereum.org/2020/11/26/ethereumjs-vm-v5-release/) - now a monorepo, supports all forks, all written in TypeScript, all APIs work with JavaScript Promises
- Latest [core devs call](https://youtu.be/UGyqRoLwq1o?t=244). Beiko’s [notes](https://twitter.com/TimBeiko/status/1332324209649885184): hashing through what goes in Berlin fork; SSZ out. In line with the past, most likely Berlin will be EIPs 2929, 2930, 2718, 2565, 2315.
- [EVM384 update](https://notes.ethereum.org/@poemm/evm384-update4): 384-bit arithmetic in EVM. Final pairings done, runtime better than wasm and almost as fast as Rust.
- [Alexandria state network update](https://snakecharmers.ethereum.org/alexandria-dev-update-2/): PoC ready by end of year to serve the header chain
- [Code merkleization benchmarks](https://ethereum-magicians.org/t/eip-2926-chunk-based-code-merkleization/4555/13)

**EIPs/Standards**

- [ERC3135](https://github.com/ethereum/EIPs/pull/3135): exclusive claimable token

**Proof of Stake launch**

- We are way over the minimum stake necessary to launch (60% more at time of writing). [Proof of stake chain launches Dec 1 at 12pm UTC](https://blog.ethereum.org/2020/11/27/eth2-quick-update-no-21/)
- if you’re staking, make sure you have the latest release: [Lighthouse](https://github.com/sigp/lighthouse/releases/tag/v1.0.2), [Nimbus](https://github.com/status-im/nimbus-eth2/releases/tag/v1.0.0), [Prysm](https://github.com/prysmaticlabs/prysm/releases/tag/v1.0.2), [Teku](https://github.com/ConsenSys/teku/releases/tag/20.11.0) (the latest release could change between now and then!) and join the discord for your client. [Discord links](https://blog.ethereum.org/2020/11/27/eth2-quick-update-no-21/) to make sure you stay up to date
- Somer Esat’s staking guides with Ubuntu updated for mainnet: [Lighthouse](https://someresat.medium.com/guide-to-staking-on-ethereum-2-0-ubuntu-lighthouse-41de20513b12?sk=ac7477fd99b6648a5745a3e327f2701c), [Nimbus](https://someresat.medium.com/guide-to-staking-on-ethereum-2-0-ubuntu-nimbus-e86bdee8c550?sk=6d2d96e714d0ec41c702b94bddec5040), [Prysm](https://someresat.medium.com/guide-to-staking-on-ethereum-2-0-ubuntu-prysm-56f681646f74?sk=b61691b713d37802b8345855dc356b02), [Teku](https://someresat.medium.com/guide-to-staking-on-ethereum-2-0-ubuntu-teku-e4247e7c75a1?sk=6d63b55ebe821bd18788c99fa81e437c).
- [Staking with docker](https://github.com/eth2-educators/eth2-docker)
- Some [security best practices](https://www.coincashew.com/coins/overview-eth/guide-or-security-best-practices-for-a-eth2-validator-beaconchain-node)
- Use ["ntp" with the setting "tinker panic 5"](https://twitter.com/dankrad/status/1332427232766255108) in ntp.conf
- Vitalik’s stats on [genesis block validators](https://twitter.com/VitalikButerin/status/1331231955787030528)
- Given the genesis block we can now calculate the [absolute minimum return stakers will receive](https://twitter.com/AlexanderFisher/status/1331242944314085379) (because there’s a 4 validators per epoch limit to how quickly new stakers can join)

**Proof of Stake plans**

- A proposal to put [mainnet state (“eth1) on the beacon chain](https://ethresear.ch/t/executable-beacon-chain/8271)
- Ideas around withdrawal: [dirt simple withdrawal](https://ethresear.ch/t/dirt-simple-withdrawal-contract/8218), [simple withdrawals](https://ethresear.ch/t/simple-eth1-withdrawals-beacon-chain-centric/8256), [excess balance transfers](https://ethresear.ch/t/simple-transfers-of-excess-balance/8263)

**Layer2**

- Loopring [zkrollup smart contract wallet](https://medium.com/loopring-protocol/loopring-wallet-ethereum-unleashed-ac4173f940a5), available in an Android app and with rewards for holding balances on their rollup
- Hermez’s [massive migrations mechanism](https://blog.hermez.io/hermez-massive-migrations-mechanism/) to prevent rollup centralization

* * *

### **This newsletter is made possible thanks to [Trail of Bits](https://www.trailofbits.com/)!**

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F90416e8c-9f60-429a-b5b1-b5beeec0a967_1876x1128.png)](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F90416e8c-9f60-429a-b5b1-b5beeec0a967_1876x1128.png)

The means and tools for securing your contracts are available today. Use the latest releases of [Slither](https://github.com/crytic/slither/releases/tag/0.6.14), [Echidna](https://github.com/crytic/echidna/releases/tag/v1.6.0), and the [Building Secure Contracts](https://github.com/crytic/building-secure-contracts) guidebook to level up your security knowledge.

* * *

**Stuff for developers**

- Using [redwoodjs to create an Eth app](https://patrickgallagher.dev/blog/2020/11/18/web3-redwood-intro/using-redwoodjs-to-create-an-ethereum-app) because redwood is built for graphQL
- [Random number generation](https://blog.chain.link/random-number-generation-solidity/) in Solidity with Chainlink’s VRF tutorial
- OpenZeppelin [Contracts v3.3](https://forum.openzeppelin.com/t/openzeppelin-contracts-3-3/4804), adds timelock, supports Solidity v0.6 and v0.7
- A [guide for devs new to Ethereum](https://www.linumlabs.com/articles/a-guide-for-developers-interested-in-learning-blockchain-development). Also check out the Eth [dev onboarding session on Dec 4](https://www.reddit.com/r/ethereum/comments/k086iv/dec_4_ethereum_dev_onboarding_2_feat_linda_xie/)

**Security**

- [Answers and explanations for all Damn Vulnerable DeFi](https://drdr-zz.medium.com/write-ups-and-lessons-learned-from-damn-vulnerable-defi-caa95d2678ec) challenges
- More [Damn Vulnerable DeFi walkthroughs](https://medium.com/@iphelix) (#2-4) from Peter Kacherginsky
- A full [postmortem from 88mph](https://medium.com/88mphapp/the-88mph-wild-ride-e09ec56ed079) on the bug that let an attacker steal 100k, and the bug that allowed them to steal it back using [Taichi](https://taichi.network/) to avoid getting frontrun

**Ecosystem**

- [Flashbots](https://medium.com/flashbots/frontrunning-the-mev-crisis-40629a613752): an org gaimed at democratizing miner-extractable value. They’re building tools to [understand MEV](https://github.com/flashbots/mev-inspect-rs) and a [geth fork PoC](https://github.com/flashbots/mev-geth) to auction transaction ordering
- Ethereum Foundation gives [$2.4m to q3 grant recipients](https://blog.ethereum.org/2020/11/25/esp-q3-updates/)
- Vids from [EthOnline](https://www.youtube.com/playlist?list=PLXzKMXK2aHh5K68HuJR8fKFuGFXCBQg0T) and [EthBerlin](https://twitter.com/_franzihei/status/1331286181259120644)
- Twitter [bot of text messages found in calldata](https://twitter.com/EtherText)
- [Eth123](https://eth123.org/), an ecosystem portal from Sparkpool

**Enterprise**

- Polish city concludes [trial with SmartKey’s Ethereum-enabled locks](https://cointelegraph.com/news/polish-city-becomes-first-to-adopt-ethereum-blockchain-for-emergency-services) so emergency services can enter without permission
- Svensson: [blockchain to simplify complex business processes](https://blog.web3labs.com/how-blockchain-simplifies-complex-business-processes)

**Application layer**

- Coinbase's Dai price got pushed upward causing $85m in [liquidations from Compound farmers who were overleveraged](https://www.comp.xyz/t/dai-liquidation-event/642)
- Aave hits a [billion in flashloans](https://twitter.com/twobitidiot/status/1332399827771068418), all in 2020
- [Ideamarket](https://rinkeby.ideamarket.io/) is on rinkeby testnet; Twitter accounts on bonding curves where the interest from deposits goes to the owner of the twitter account
- [GnosisDAO](https://blog.gnosis.pm/announcing-gnosisdao-a7102fcf9224) to govern Gnosis's treasury and products that will incorporate futarchy as its governance mechanism
- 2020 American presidential election? [Prediction markets were right](https://www.charlesrubenfeld.com/the-prediction-markets-were-right/)
- Week in Andre Cronje: [Deriswap](https://andrecronje.medium.com/deriswap-capital-efficient-swaps-futures-options-and-loans-ea424b24a41c), an attempt to consolidate liquidity. To that end, a blizzard of mergers and acquisitions: [Cream v2](https://medium.com/iearn/yearn-cream-v2-merger-e9fa6c6989b4), [Pickle](https://medium.com/iearn/pickle-yearn-ferment-co-operation-dill-eec43b93d0ea), [Cover](https://medium.com/iearn/yearn-cover-merger-651142828c45). Andre’s [explanation of each of those](https://andrecronje.medium.com/merger-acquisition-partnership-collaboration-nomenclature-in-the-decentralized-space-ca24370d6f27) three

**Regulation/business/tokens**

- Ehrsam: [governance minimization](https://www.fehrsam.xyz/blog/governance-minimization)
- Mintable doing [NFT-governed DAO](https://mintable.medium.com/mint-nft-dao-100-governed-by-nfts-18c99421230) to thwart flashloans
- Chinese [federal government seizes billions](https://www.theblockcrypto.com/post/85873/china-seize-billion-cryptos-from-plustoken-crackdown) from Plustoken scam
- Trump’s [spy chief asks SEC to be more crypto-friendly](https://www.washingtonexaminer.com/news/trump-spy-chief-seeks-sec-scrutiny-of-chinese-dominance-in-cryptocurrency) to counter China
- SEC [proposal to let web2 network participants get equity](https://ca.reuters.com/article/idUSL4N2IA3ON)

**General**

- Cloudflare [post mortem on the Byzantine fault that caused cascading failures](https://blog.cloudflare.com/a-byzantine-failure-in-the-real-world/) and substantial outage
- [Ziggy](https://twitter.com/EliBenSasson/status/1332057808611708951): a quantum-secure STARK signature scheme

* * *

## **Job Listings**

- [Aztec's hiring](https://medium.com/aztec-protocol/were-hiring-5cd7cf5b0667)! Join ZK’s cutting edge with the private L2 from PLONK’s creators
- 0x looking for [devs of all types](https://0x.org/about/jobs) and a [Matcha marketing manager](https://boards.greenhouse.io/0x/jobs/4923909002)
- Chainlink Labs has [40+ openings](https://www.chainlinklabs.com/careers#open-roles) across all departments
- Nexus Mutual: [experienced Solidity dev](https://angel.co/company/nexus-mutual-1/jobs/967538-smart-contract-engineer) in Euro timezones
- Trail of Bits is hiring [blockchain security devs](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & [cryptography analyst](https://jobs.lever.co/trailofbits/56af8506-3205-4c7b-b28d-ba8292bd1a47)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow the newsletter on twitter: [@WeekinEthNews](https://twitter.com/WeekInEthNews)

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-november-29-2020/](https://weekinethereumnews.com/week-in-ethereum-news-november-29-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Dec 1 - [Proof of stake launch](https://blog.ethereum.org/2020/11/04/eth2-quick-update-no-19/) 
- Dec 2 - [Gitcoin CLR matching](https://gitcoin.co/grants) round starts
- Dec 3 - [Ethereum in the Enterprise: Asia Pacific 2020](https://entethalliance.org/ethereum-in-the-enterprise-asia-pacific-2020/)
- **Dec 4 - [New to Ethereum dev onboarding](https://www.reddit.com/r/ethereum/comments/k086iv/dec_4_ethereum_dev_onboarding_2_feat_linda_xie/)**
- Dec 22 - Deadline to apply for [proof of stake community grants](https://ethereum.org/en/eth2/get-involved/staking-community-grants/)
- Feb 5-12 - [ETHDenver](https://twitter.com/EthereumDenver/status/1328367230707396609) (virtual)
- Mar 2-4 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

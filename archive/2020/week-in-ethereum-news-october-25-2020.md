---
title: "Week in Eth News <BR> October 25, 2020"
date: "2020-10-25"
---

## **Eth News and Links**

**Eth1**

- Latest [Turbogeth weekly release](https://github.com/ledgerwatch/turbo-geth/releases/tag/2020.10.02)
- [Sponsored transaction precompile](https://hackmd.io/@SamWilsn/rkmD5l8Pw) draft
- Piper’s [state availability](https://notes.ethereum.org/e8VFLDiUSPSn2v7VVM1CXw) doc

**Proof of Stake launch**

- [Deposit contract at least 2 weeks away](https://youtu.be/JOgowAlKSqw?t=2487), pending audit report of blst BLS sig library
- Context: Justin Drake writes the history of [BLS sigs and Eth2](https://www.reddit.com/r/ethfinance/comments/jghide/daily_general_discussion_october_23_2020/g9sz7jm/)
- [Mass-slashable unavailability faults](https://ethresear.ch/t/mass-slashable-unavailability-faults/8129)

**Layer2**

- StarkWare’s plans for [layer2 interoperability](https://medium.com/starkware/the-road-to-l2-interoperability-718ff69ec822), aiming at q1 2021

* * *

### **This newsletter is made possible thanks to [Celer](https://www.celer.network/)!**

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F18e1fc5a-eab4-4869-9b9d-135dff1fabaa_950x400.png)](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F18e1fc5a-eab4-4869-9b9d-135dff1fabaa_950x400.png)

[Celer](http://celer.network/) is a coherent layer-2 scaling platform on Ethereum powered by [Generalized State Channel Network](https://www.celer.network/docs/celercore/index.html) and [Hybrid Rollup](https://medium.com/celer-network/adding-hybrid-pos-rollup-sidechain-to-celers-coherent-layer-2-platform-d1d3067fe593) technology. Real money games, such as [Arcade Win](https://apps.apple.com/us/app/arcade-win/id1459895768) and [Daub Cash](https://apps.apple.com/us/app/daub-cash/id1513396754), built using [Celer's gaming-focused SDK](http://developer.celerx.app/) just reached top #10 ranking in App Store. We have [completed the last State Guardian Network testnet](https://blog.celer.network/2020/10/04/sgn-beta-testnet-community-event-successfully-completed/) and will be launching SGN on mainnet soon.

Follow us on [twitter](https://twitter.com/CelerNetwork), [blog](https://blog.celer.network/), [discord](https://discord.com/invite/Trhab5w) and [telegram](https://t.me/celernetwork).

* * *

**Stuff for developers**

- Solidity [v0.7.4](https://solidity.ethereum.org/2020/10/19/solidity-0.7.4-release-announcement/) bugfix when copying empty byte arrays from memory/calldata to storage
- [B̶u̶i̶d̶l̶e̶r̶ is now Hardhat](https://medium.com/nomic-labs-blog/buidler-has-evolved-introducing-hardhat-4bccd13bc931); much easier mainnet forking, better support for multiple solc versions in production
- [Tenderly’s deep integration with Hardhat](https://blog.tenderly.co/level-up-your-smart-contract-productivity-using-hardhat-and-tenderly/), with accompanying guide
- Truffle [v5.1.50](https://github.com/trufflesuite/truffle/releases/tag/v5.1.50), now with web3js v1.2.9
- [Chainlink VRF now providing randomness](https://blog.chain.link/chainlink-vrf-now-live-on-ethereum-mainnet/) on mainnet
- Prestwich’s [memview-sol](https://github.com/summa-tx/memview-sol): memory access with runtime typechecking in Solidity
- [Falsehoods that Ethereum devs believe](https://gist.github.com/spalladino/a349f0ca53dbb5fc3914243aaf7ea8c6)
- [Detecting ownership takeovers](https://diligence.consensys.net/blog/2020/09/detecting-ownership-takeovers-using-mythril) using Mythril
- Trail of Bits intern on using [n-grams in SlithIR and machine learning on their audit reports](https://blog.trailofbits.com/2020/10/23/efficient-audits-with-machine-learning-and-slither-simil/); data prep is hard!
- A story of [saving 200m in DeFi cover from getting bricked](https://medium.com/armorfi/saving-200m-in-defi-cover-ffe492f9459b)
- How Argent upgraded to [Solidity v0.6](https://www.argent.xyz/blog/argent-upgrading-to-solidity-0-6/)
- 3box’s [IDX](https://medium.com/3box/idx-a-devkit-for-open-identity-48edc88e8e85), an SDK for decentralized identities (DIDs)
- A more [gas efficient version of WETH](https://twitter.com/acuestacanada/status/1319581439831298048)
- Autoconnect your [Unity game to MetaMask](https://medium.com/coinmonks/unity-engine-metamask-wallet-6797d4699e45)
- Learning [Solidity for attorneys](https://lexdao.substack.com/p/learning-solidity-for-attorneys)
- Austin Griffith’s eth.build [course for web devs new to eth on BlockGeeks](https://courses.blockgeeks.com/course/eth-build/)

**Ecosystem**

- Ethereum is on pace to [settle over 1 trillion USD in 2020](https://twitter.com/MessariCrypto/status/1318985292347543552) eth tx volume
- [Mamba](https://twitter.com/vasa_develop/status/1318337690828369921): Cicada 3301 for web3
- Vitalik’s [round 7 gitcoin matching review](https://vitalik.ca/general/2020/10/18/round7.html)
- Some Medalla data challenge submissions:
    - Splunk [dashboard with health score](https://www.splunk.com/en_us/blog/tips-and-tricks/attesting-the-health-of-ethereum-2-0.html)
    - Some [whale data viz](https://medium.com/coinmonks/visualizing-whales-in-the-rough-seas-of-medalla-the-ethereum-2-testnet-f748592fc08a) over time
    - Elias Simos and Sid Shekhar [plethora of stats](https://eth2data.github.io/)

**Enterprise**

- Provide and Unibright merging into a “[low-code, end-to-end Baseline integration suite](https://medium.com/unibrightio/provide-incorporates-the-unibright-framework-to-create-unified-service-for-corporate-data-sharing-e0f0a57b7f25)”
- [Baselining the end consumer](https://medium.com/@a.freundhaskel/baselining-the-end-consumer-9349a8e0ed7e), how people use mainnet without knowing it
- Villanova sending [private Ethereum chain into space on a satellite](https://www.coindesk.com/villanova-test-ethereum-blockchain-space)
- Interact with the chain using [Curvegrid’s Google Sheets add-on](https://www.curvegrid.com/blog/2020-10-20-multibaas-for-google-sheets/)

**Application layer**

- Defi now has a yield curve: [Yield Protocol is live](https://medium.com/yield-protocol/yield-protocol-is-live-e6e8ebf2537b) with beta launch. Fixed-term, fixed-rate lending/borrowing, or add liquidity.
    - Quick [visualization of the yield curve](https://curve.is/)
- [pooltogether v3](https://medium.com/pooltogether/the-new-pooltogether-891d94858588) is live, removed admin control, randomness via VRF, rewards for deposits and referrals
- [Novel Air Pollution Measurement System](https://www.mdpi.com/2224-2708/9/4/49/htm) on Ethereum
- a [synthetic token for impermanent loss](https://medium.com/hakkafinance/impermanent-gain-the-antimatter-of-impermanent-loss-8d4d6c513d09) via prediction market
- DeFiSaver’s [loan shifter](https://medium.com/defi-saver/introducing-loan-shifter-change-your-collateral-or-debt-asset-and-shift-between-protocols-using-cf03ec3c225f) to easily move between protocols and assets
- Opolis Employment Commons [unveils tokenization system](https://medium.com/opolis/opolis-announces-upcoming-rewards-token-which-members-can-earn-for-consumption-of-payroll-2eb45f88874e) for processing payroll or getting health insurance through the commons
- Music streaming platform [Audius on mainnet](https://medium.com/audius/welcome-audio-to-mainnet-409009bc130c); airdrop to 10k most popular artists

**Regulation/business/tokens**

- Federal bank regulator Brian Brooks compares [banks in the age of DeFi to the post office in the age of email](https://cointelegraph.com/news/mainstream-defi-is-inevitable-us-currency-comptroller)
- Kik [settles with the SEC](https://www.courtlistener.com/docket/15722539/89/2/us-securities-and-exchange-commission-v-kik-interactive-inc/) by paying $5m and freezing their 3 trillion tokens
- de la Rouviere: [seasons & longevity of community tokens](https://blog.simondlr.com/posts/seasons-longevity-in-community-tokens)
- web3 [ownership will eat the software](https://medium.com/@etm612/ownership-will-eat-the-software-thats-eaten-the-world-82030c8b6a14) that’s eaten the world

**General**

- PayPal adds [ETH and BTC](https://newsroom.paypal-corp.com/2020-10-21-PayPal-Launches-New-Service-Enabling-Users-to-Buy-Hold-and-Sell-Cryptocurrency) in the US, held by Paxos. Venmo to follow.
- GridPlus’s [Lattice1 hardware wallet ships pre-orders](https://blog.gridplus.io/from-idea-to-reality-the-first-lattice1-hardware-wallets-have-shipped-5e9672e89c32)
- Reason’s [cypherpunk series, video 3](https://youtu.be/lv8OFSWZkGs)
- Build a [high performance fuzzer with GPUs](https://blog.trailofbits.com/2020/10/22/lets-build-a-high-performance-fuzzer-with-gpus/) for 10x performance in the cloud

* * *

## **Job Listings**

- Want a new challenge? [mStable](https://twitter.com/mstable_) seeks experienced [Smart Contract/Protocol Dev](https://cryptocurrencyjobs.co/engineering/mstable-protocol-developer-defi/)
- DeFi devs! Yield is hiring for Solidity and front-end – contact@yield.is
- 0x hiring a [Matcha marketing manager](https://boards.greenhouse.io/0x/jobs/4923909002) and [all flavors of developers](https://0x.org/about/jobs)
- Chainlink has [30+ openings at the moment](https://jobs.lever.co/chainlink/) across marketing, ops, & devs
- Trail of Bits hiring [blockchain security engineers](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & [cryptography analyst](https://jobs.lever.co/trailofbits/56af8506-3205-4c7b-b28d-ba8292bd1a47)
- Celer hiring Solidity and Go devs. Email: hiring@celer.network

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH (or 250 DAI or 250 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **Wanton self-promotion section**

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Follow the newsletter on twitter: [@WeekinEthNews](https://twitter.com/WeekInEthNews)

Permalink for this week’s issue:  [https://weekinethereumnews.com/week-in-eth-news-october-25-2020/](https://weekinethereumnews.com/week-in-eth-news-october-25-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Oct 29 - [ETHBKK](https://pages.atato.com/ethbkk)
- **Oct 30 - [Ethereum’s Impact on the World](https://ethonline.org/impact/) - ETHOnline summit**
- Oct 31 - [submission deadline for Underhanded Solidity Contest](https://underhanded.soliditylang.org/)
- Nov 6-7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)
- Nov 16 - [MetaMask Provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7)
- Nov 19 - EthBerlin 2.5: [Talk Show](https://medium.com/ethberlin/move-over-netflix-theres-a-new-zoom-talk-show-in-town-db48c75d35af)
- Dec 3 - [Ethereum in the Enterprise - Asia Pacific](https://twitter.com/EntEthAlliance/status/1314652848655872000)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

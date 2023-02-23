---
title: "Week in Ethereum News <BR> August 24, 2019"
date: "2019-08-25"
---

## **Eth News and Links**

**Layer 1**

- Paper [analyzing Eth’s gas prices](https://arxiv.org/abs/1905.00553), which largely mirrors the upcoming Istanbul gas repricing
- Wei Tang: what if we designed a [versionless EVM](https://that.world/~essay/nevm/)
- [Lighthouse eth2 client fuzzing update](https://lighthouse.sigmaprime.io/fuzzing-01.html)
- [Prysmatic eth2 client](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-33-prysmatic-labs-5ce8c2baafcf) update - swappable database backend, now running disc v5
- A [finalization delay attack on LMD Ghost](https://ethresear.ch/t/decoy-flip-flop-attack-on-lmd-ghost/6001)
- [Secret single-leader election](https://ethresear.ch/t/low-overhead-secret-single-leader-election/5994) with per block overhead of one SNARK plus 32 bytes

**Layer 2**

- The [Optimistic Virtual Machine loves state channels](https://medium.com/plasma-group/the-ovm-%EF%B8%8Fs-your-scaling-solution-state-channel-edition-ed13de56e249)

**Stuff for developers**

- [Efficient ECC in zkSNARKs using ZoKrates](https://medium.com/zokrates/efficient-ecc-in-zksnarks-using-zokrates-bd9ae37b8186)
- [Bringing privacy to NFTs](https://medium.com/centrifuge/bringing-privacy-to-non-fungible-tokens-a-recap-from-the-zokrates-workshop-at-zcon1-6d9ea8a74b7f) using ZoKrates
- [Circom snarks compiler ported to Rust](https://github.com/iden3/rust-circom-experimental)
- 0x [Asset Swapper](https://blog.0xproject.com/contract-fillable-liquidity-made-simple-8b9cf1b2f2f2) integration to source liquidity
- A guide to deploying [Alethio and Ethstats](https://medium.com/alethio/a-guide-to-deploying-alethios-free-open-source-products-18216617722e)
- [MythX Pro](https://medium.com/consensys-diligence/announcing-mythx-pro-c8ea5ecc9c59) - Mythril/MythX security scan API subscription paid in Dai using [Daisy Payments](https://www.daisypayments.com/)
- The intersection of [formal verification and agent-based incentive simulation](https://medium.com/gauntlet-networks/formal-verification-and-incentive-simulation-as-necessary-complements-in-smart-contract-security-67a571ebcce8)
- Academic [survey paper on EVM security](https://arxiv.org/pdf/1908.04507.pdf)
- Compound’s [Open Oracle System](https://medium.com/compound-finance/announcing-compound-open-oracle-development-cff36f06aad3) for price feeds. Running on Rinkeby.
- [Solidity2UML class diagram generation v1 release](https://github.com/naddison36/sol2uml#solidity-2-uml)
- [Eventeum event listener v0.7](https://github.com/ConsenSys/eventeum)
- [OpenZeppelin SDK v2.5.3](https://github.com/OpenZeppelin/openzeppelin-sdk/releases/tag/v2.5.3) with Gas Station Network
- [Manage tokens in Java with web3j](https://kauri.io/article/d13e911bbf624108b1d5718175a5e0a0/manage-erc20-tokens-in-java-with-web3j) tutorial
- How I [used 3box to build a full stack dapp](https://medium.com/@pedrouid/how-i-used-3box-to-build-a-full-stack-dapp-49d3ef9365cb)
- [How to design modular smart contracts in Solidity](https://liamz.co/blog/how-to-design-modular-smart-contracts-in-solidity-using-the-target-pattern/)
- Zeppelin’s Santi Palladino releases [Ethereum for web devs](https://www.apress.com/us/book/9781484252772) book
- You no longer have to [Etherscan verify every cloned contract](https://medium.com/etherscan-blog/eip-1167-minimal-proxy-contract-on-etherscan-3eaedd85ef50) if it is EIP1167 compliant

**Ecosystem**

- Large-scale [translation program underway starting with the Ethereum website](https://blog.ethereum.org/2019/08/20/Translating-Ethereum-for-our-Global-Community/) to make sure everyone can learn about Ethereum in their native language
- You can now [donate to MolochDAO](https://twitter.com/MolochDAO/status/1162338964122021890) without being a member
- Onchain [auction for Devcon tickets](http://ethercards.devcon.org/), Aug 25-27
- A [majority of r/ethtrader mods quit and started r/ethfinance](https://www.reddit.com/r/ethfinance/), so Eth holders now have two large Reddit price-talking communities
- EthBerlin [hackathon submissions](https://zwei.devpost.com/submissions).

**Enterprise**

- [Pantheon poised to join Hyperledger](https://www.coindesk.com/ethereum-could-become-first-public-blockchain-with-official-hyperledger-project) and become first public chain
- [Deployment with Kubernetes and Pantheon](https://pegasys.tech/accelerate-blockchain-deployment-with-kubernetes-pantheon/)
- [Deploying a full stack app to Azure](https://kauri.io/article/d37518870cba4caeab6a95624254a6b8/v1/deploying-a-full-stack-dapp-to-microsoft-azure) tutorial
- Kaleido: Using [rotating signers to scale IBFT](https://kaleido.io/using-rotating-signers-to-scale-ibft-consensus-algorithm/)
- [World Bank sells $50m AUD (~35m USD) in bonds](https://www.worldbank.org/en/news/press-release/2019/08/16/world-bank-issues-second-tranche-of-blockchain-bond-via-bond-i) on private Ethereum chain
- ING executes [first commodity transaction on Komgo](https://www.ingwb.com/themes/distributed-ledger-technology-articles/ing-executes-first-commodity-trade-transaction-on-komgo)

**Governance and Standards**

- Latest [core devs call](https://www.youtube.com/watch?v=yO0WdT-J64w). [Notes](https://github.com/ethereum/pm/blob/48d690ba04ab1a09c3ec4b98d22b0f4cc7d254df/All%20Core%20Devs%20Meetings/Meeting%2069.md). Istanbul finalized EIPs: 152, 1108, 1344, 1884, 2028 and 2200. Clients to finish implementations in next 2 weeks, then pick a hard fork date.
- Lots of core dev discussion about setting expectations for app developers: expect some breaking changes.
- Also lots of core dev discussion on how to do 1884 gas repricing: the “correct” way to do it \_may\_ break some things, but want to try that before a “hacky” way that may be unnecessary. Listen to the call or read the notes for more.
- [Client tracker for Istanbul](https://notes.ethereum.org/@holiman/SyT_rGjNr)
- [Opinionator](https://blog.slock.it/introducing-the-opinionator-1d0bf0438aab) - votes weighted by gas usage

**Live on mainnet**

- [Clovers Network](https://medium.com/@billyrennekamp/launching-clovers-network-2bbe76acaa37) is live on mainnet. “mine” clover and then buy your collectibles with the in-game currency on a bonding curve.
- [Panvala](https://medium.com/@Panvala/batch-four-and-the-astrotrope-6fddd573322a) is live on mainnet. Anyone can recommend who deserves Panvala tokens for work on public goods, and then token holders vote on recommendations.
- [RequestNetwork v2](https://request.network/en/2019/08/19/request-version-2-0-mainnet-released/) is on mainnet. IPFS storage with Eth hash, and invoicing features.
- [Centrifuge’s Tinlake](https://medium.com/centrifuge/centrifuges-tinlake-goes-live-with-the-financing-of-more-than-usd180k-2cc6ce176a1b) is live on mainnet. 180k USD in tokenized real world assets like invoice factoring and mortgages.

**Application layer**

- Augur [v2 transition update](https://www.augur.net/blog/v2-transition-update/)
- [Yolorekt](https://medium.com/yolorekt/meet-yolorekt-ethereums-newest-dapp-9a9173f8eaef) - a 3 minute ETHUSD price prediction game using Abridged
- You can now [tip BAT on Reddit and Vimeo with Brave](https://twitter.com/AttentionToken/status/1164283113112924160) desktop
- [Escrow and arbitration](https://medium.com/@rosscampbell9/digital-escrow-and-arbitration-on-openlaw-and-ethereum-9e2c498c6495) on OpenLaw

**Tokens / Business / Regulation**

- The [road to futarchy](https://medium.com/level-k/the-road-to-futarchy-87edc282c2b)
- NYTimes headline: “[Terrorists turn to Bitcoin](https://www.nytimes.com/2019/08/18/technology/terrorists-bitcoin.html)…” These tend to be harbingers of regulatory overreaction.
- A bunch of [crazy BTC maximalists have been investing](https://www.coindesk.com/crypto-and-security-token-exchange-inx-to-raise-130-million-in-landmark-ipo) in an IPO that builds on Ethereum. A bullish thing for Ethereum: how often haters have to build on ETH

**General**

- [PLONK](https://eprint.iacr.org/2019/953.pdf): universal and updatable trusted setup with better performance than Sonic
- [Efficient zero-knowledge arguments in the discrete log setting](https://eprint.iacr.org/2019/944)
- Comprehensive survey paper [deconstructing blockchains](https://arxiv.org/pdf/1908.08316.pdf)
- Toronto Star [Q&A with Vitalik](https://www.thestar.com/business/2019/08/19/ethereums-vitalik-buterin-on-reducing-cryptocurrencys-risks.html)
- BigTech literally [tracks you with every thing you do](https://www.nytimes.com/interactive/2019/08/23/opinion/data-internet-privacy-tracking.html). All you even have to do is open up [any browser, even a fresh install](https://twitter.com/jonathansampson/status/1165353213308129281). Switch [to Brave](https://brave.com/wee307) (referral link).

* * *

## 🎂 **3 year anniversary** 🎂

For the three year anniversary, we’re going to try a small experiment. 🥼

Next week I’m going to do two versions of the newsletter. One will be the normal edition, and one will be the gated “annotated edition.” People often tell me they would be willing to pay money to get an edition with more commentary and with more robust summaries.

Partnering with [Unlock Protocol](https://unlock-protocol.com/), you can [buy the NFT for 0.11 Eth](https://weekinethereumnews.com/three-year-anniversary-edition/) which will unlock next week’s annotated edition. There are 200 Week in Ethereum 3 year anniversary NFTs available.

All proceeds will be back into Ethereum somehow, likely donated to a public good, at my discretion. And who knows, maybe there will be future benefits for the 200 NFT holders?

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- Aug 28-Sep11 - [Ethereal Blocks](https://hackathons.gitcoin.co/ethereal-blocks/) virtual hackathon
- Aug 29-30 - [ERC1400 security token hackathon](https://medium.com/@ramvi/invitation-to-hackathon-in-oslo-29-30-august-1d8ec54a26ad) (Oslo)
- **Sep 1 - [ENS 3-6 character auction](https://medium.com/the-ethereum-name-service/timeline-for-3-6-character-name-reservation-auction-and-instant-registrations-e39aa2f89dc9) starts**
- Sep 2-16 - [Decentraland SDK virtual hackathon](https://hack.decentraland.org/?with=weekinethereum) (250k USD in prizes. There’s a referral code on that link that gets both you and me something extra)
- Sep 3 - Deadline to [apply for EU Horizon Prize](https://ec.europa.eu/info/funding-tenders/opportunities/portal/screen/opportunities/topic-details/blockchain-eicprize-2019). 1m € each to 5 "Blockchains for Social Good" projects
- Sep 6-8 - [ETHBoston](https://eth.boston/)
- Sep 10-11 - [DeFi Summit](https://defisumm.it/) (London)
- Sep 15 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff/)
- Sep 15 - [Ethereal Tel Aviv](https://etherealsummit.com/events/ethereal-tel-aviv/)
- Sep 16 - [Tachyon accelerator application](https://labs.consensys.net/tachyon/) deadline
- Sep 15-16- [StarkWare sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- Sep 22 - [IDEO virtual hackathon](https://coinlist.co/build/ideo) ends
- Oct 7 - [ENS workshop](https://medium.com/the-ethereum-name-service/ens-workshop-applications-are-now-open-f46db6c63384) (Osaka)
- Oct 8-11 - [DeVcon](https://devcon.org/) (Osaka) and [Devcon social events calendar](http://osaka.kickback.events/events/)
- Nov 8-10 - [ETHWaterloo](https://ethwaterloo.com/)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I own 100% Week In Ethereum. Editorial control has always been me.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **This headline stays as long as so many people continue to link to old URL and not the right one: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/week-in-ethereum-news-august-24-2019/](https://weekinethereumnews.com/week-in-ethereum-news-august-24-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

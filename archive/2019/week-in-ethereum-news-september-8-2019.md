---
title: "Week in Ethereum News <BR> September 8, 2019"
date: "2019-09-09"
---

## **Eth News and Links**

**Eth1**

- Geth [v1.9.3](https://github.com/ethereum/go-ethereum/releases/tag/v1.9.3) - maintenance release with Istanbul upgrade finalized
- Least Authority’s [ProgPow security audit](https://github.com/ethereum-cat-herders/progpow-audit/blob/master/Least%20Authority%20-%20ProgPow%20Algorithm%20Initial%20Audit%20Report.pdf), later discussed on core devs call. “We found no major issues and the design appears to function as intended.”
- First call for the [finality gadget working group](https://youtu.be/ot_io5Xi13M?t=16) that will use the eth2 chain to finalize the eth1 chain and then drastically reduce mining rewards.
- Latest [core devs call](https://www.youtube.com/watch?v=6m0So81_j2Q). Live [tweeted notes](https://twitter.com/TimBeiko/status/1169976701302054913). Oct 2 testnet fork, mainnet in Nov. Lots of [blake2b discussion](https://github.com/ethereum/EIPs/issues/152). Next hard fork after this one named “Berlin.”

**Eth2**

- A [Casper FFG explainer](https://medium.com/unitychain/intro-to-casper-ffg-9ed944d98b2d). How it adapts PBFT
- It’s [Eth2 networking lockin week](https://github.com/ethereum/eth2.0-pm/blob/master/interop/lockin/goals-exercises.md)
- [Games for evaluating liveness in Casper CBC](https://ethresear.ch/t/games-for-evaluating-liveness-in-cbc-and-other-dag-protocols/6070)
- Bouncing attack [analysis](https://ethresear.ch/t/analysis-of-bouncing-attack-on-ffg/6113) and [prevention](https://ethresear.ch/t/prevention-of-bouncing-attack-on-ffg/6114)
- [Lighthouse client](https://lighthouse.sigmaprime.io/update-15.html) update - interop with Nimbus, networking to official spec, 50ms slot times with 8 validators
- [Prysmatic client](https://medium.com/prysmatic-labs/ethereum-2-0-development-update-34-prysmatic-labs-7937061af3a7) update - like Lighthouse, prepping for Eth2 networking lockin

**Layer 2**

- Vitalik: [layer 1 techniques on layer 2](https://ethresear.ch/t/cases-where-the-same-thing-can-be-done-with-layer-1-and-layer-2-techniques/6111)
- A [gentle guide to the OVM](https://medium.com/cryptoeconomics-lab/a-gentle-guide-to-the-ovm-934035646942), and where CEL is building.
- Latest [Plasma implementer call](https://www.youtube.com/watch?v=eT2a3HrENFM)
- IACR paper on [lightweight watchtowers](https://eprint.iacr.org/2019/986)

**Stuff for developers**

- [Eth2 developer experience survey](https://hwwhww.typeform.com/to/McUlt8)
- [Write your first zk snark using Iden3’s circom and snarkjs libraries](https://docs.iden3.io/#/guides/circom-and-snarkjs)
- [babyJubJub in Rust](https://github.com/arnaucube/babyjubjub-rs)
- [Groth16 verifier](https://github.com/snjax/groth16batchverifier/blob/master/contracts/Groth16Verifier.sol)
- [Zac Williamson video on PLONK](https://www.youtube.com/watch?v=NqrVcDuQ8hM), Aztec’s new snark construction
- [Remix IDE v0.8.6](https://twitter.com/EthereumRemix/status/1169587816680103936)
- [web3Connect v1.0.0-beta.20](https://gist.github.com/pedrouid/d1bbba594ec679fa16c85fce37c24a2c) - 92% smaller bundle size, some breaking changes
- Chainshot’s [intro to ethers.js tutorial](https://www.chainshot.com/intro/5c36bf15143eed0017f579755d6e7a3847e43837b005c4d7)
- [filestorage.js](https://github.com/skalenetwork/filestorage.js) for storage on SKALE sidechains
- [First time Eth developing on Windows](https://medium.com/@filzatariq92/build-your-ethereum-dapp-on-windows-with-truffle-ganache-and-metamask-beginners-guide-8c62b55ef556) guide
- Build a [text notification app with IPFS, Twilio and Eth address](https://medium.com/simpleid-dev-tools/tutorial-how-to-build-an-ipfs-text-notification-app-d7e1a89c784b) for authentication
- Runtime Verification announces work on [bounded model checker](https://runtimeverification.com/blog/the-rv-bounded-model-checker-a-lightweight-semantics-based-tool/), a symbolic execution tool as a component of K’s Haskell backend.
- [Stop using Solidity’s transfer](https://diligence.consensys.net/posts/2019/09/stop-using-soliditys-transfer-now/). Christian Reitwießner’s [response](https://twitter.com/ethchris/status/1169684628208259074): “We have not yet reached a conclusion on that”

**Ecosystem**

- [Mixers and beyond: Semaphore](https://medium.com/coinmonks/to-mixers-and-beyond-presenting-semaphore-a-privacy-gadget-built-on-ethereum-4c8b00857c9b) and the MicroMix eth and token mixer (live on Kovan testnet). An outline on making a [private DAO with Semaphore](https://ethresear.ch/t/private-dao-with-semaphore/6110)
- [State of mixers](https://github.com/tvanepps/State-of-the-Mixers-Summer-2019/blob/master/README.md) - a report on the tradeoffs and progresses of mixers in our ecosystem
- [Mixicles](https://chain.link/mixicles.pdf) - Juels, Breidenbach, et al paper with Chainlink. Input payments and decide payouts based on oracle results. two or more parties and yield payouts that are conditioned on oracle reports.
- A [coin mixer built on Enigma](https://blog.enigma.co/salad-coin-mixing-with-enigma-1c565adee79c)
- [Evolution of Dharma](https://blog.dharma.io/the-evolution-of-dharma-2017-present-64b841d9eac2) - engaging chronicle of how Dharma has navigated the idea maze
- [EthBoston submissions](https://ethboston.devpost.com/submissions) and [winners](https://twitter.com/ETHBoston/status/1170774191504674816). Also two great videos from EthBoston to watch: Albert Ni’s “[Ethereum from multiple perspectives](https://www.youtube.com/watch?v=QndfwZF8YeY)” and Raul Jordan’s “[Paving the path for the future of Ethereum](https://www.youtube.com/watch?v=iaWJp3ioTdc)”

**Standards and governance topics**

- [The LAO](https://medium.com/openlawofficial/the-lao-a-for-profit-limited-liability-autonomous-organization-9eae89c9669c): an LLC+TheDAO mashup to be a US-compliant DAO for profit. Ross Campbell’s code for [how TheLAO extends Moloch](https://medium.com/@rosscampbell9/venturing-into-the-lao-comparing-molochdao-and-vmlao-solidity-designs-81da2361dba5)
- Since everyone is launching a DAO: [how to launch a (moloch fork) DAO](https://molochdao.discourse.group/t/how-to-launch-a-dao/82)
- [ERC2258](https://github.com/ethereum/EIPs/issues/2258): Custodial ownership standard

**Application layer**

- [Maker’s oracles v2](https://blog.makerdao.com/introducing-oracles-v2-and-defi-feeds/): 0x, dYdX, Set, Gnosis to be oracles and get fees. Also [Dai Stability Fee now at 14.5%](https://twitter.com/MakerDaiBot/status/1170436478188568577)
- DeFi Saver: [automatic CDP liquidation protection](https://medium.com/defi-saver/automatic-liquidation-protection-and-leverage-increase-is-now-live-in-defi-saver-beta-e53b6194b35a)
- [pooltogether v2](https://www.reddit.com/r/ethereum/comments/czsz5u/no_loss_lottery_on_ethereum_launching_today/) is live
- [PoolDai](https://twitter.com/boredGenius/status/1168441905950015488) also live: donate the interest from your cDai to a good cause
- With any DeFi product, you should be aware of what risks you’re taking. Ameen writes up the [risks to using Compound](https://medium.com/@ameensol/what-you-should-know-before-putting-half-a-million-dai-in-compound-fafdb2645f77). Compound CEO Leshner’s [response](https://twitter.com/rleshner/status/1169274512900124672).
- More money markets: [Outlet](https://medium.com/outlet-finance/outlet-the-defi-bank-the-consumer-decentralized-finance-app-for-crypto-and-non-crypto-people-f2046fe36f4), a wallet aiming to abstract away using the protocols using Plaid as the fiat onramp
- [Podcrypt](https://www.reddit.com/r/ethereum/comments/d115ic/podcrypt_beta_has_been_released/): podcast discovery webapp with recurring Eth donations
- [Majority Report](https://medium.com/@sheehan_95/the-majority-report-af46c6743213): cataloging Augur’s decisions by REP holders, ie LexisNexis/WestLaw for Augur.
- A [text based RPG/MUD](https://www.reddit.com/r/ethereum/comments/d0kyze/earn_ether_next_weekend_playtesting_worlds_first/)
- [Decentraland gets first casino](https://ryanschultz.com/2019/09/03/decentraland-gets-its-first-casino-and-slot-machines-soon-you-will-be-able-to-gamble-using-mana-and-ethereum-at-chateau-satoshi/)
- Austin Griffith’s latest DAOG version: [Three Queens](https://medium.com/@austin_48503/three-queens-b3760c33ab4b)
- Guesser markets are [competitive for NFL games](https://medium.com/guesser/sports-fans-can-get-the-best-odds-for-every-sport-using-ethereum-2d7481170eab)
- [SingularDTV](https://medium.com/@SingularDTV/singulardtv-the-sngls-dao-sngls-2-0-and-breaker-6f23f473911c)’s SNGLS DAO to incentivize content curation
- [Gitcoin hits 2m GMV](https://twitter.com/gitcoin/status/1168533339466129408)

**Tokens / Business / Regulation**

- Joel Monegro: [Ethereum and the 77 dwarfs](https://www.placeholder.vc/blog/2019/8/31/ethereum-and-the-seven-dwarfs). Nobody in blockchain ever got fired for choosing to build on Ethereum.
- [Information asymmetry in crypto](https://medium.com/@jonathanjoseph/information-asymmetry-in-crypto-e7d17da04066). web3 moves fast, some aren’t keeping up.
- Mougayar’s [PIB framework](http://startupmanagement.org/2019/09/04/pulse-impact-and-breadth-pib-a-simple-framework-of-metrics-for-evaluating-cryptocurrencies-and-tokens/) for comparing crypto tokens
- Paxos launches a [gold-backed token that takes a fee at the contract layer](https://twitter.com/arvanaghi/status/1169713013705912326) on transfer. It’ll be interesting to see if this [gets wrapped](https://twitter.com/gakonst/status/1170045064829177856)
- Dan Robinson’s [yTokens idea](https://twitter.com/danrobinson/status/1169689525536215040), collateralized fixed-term lending. Zero coupon bonds for a yield curve.

**General**

- “[ETH goes where no Bitcoin has gone before](https://twitter.com/WilliamShatner/status/1168597678185275393)” - William Shatner
- [80k Hours Podcast talks to Vitalik](https://80000hours.org/podcast/episodes/vitalik-buterin-new-ways-to-fund-public-goods/) for a few hours (with transcript!). Lots of “what are blockchains good for” conversation.
- [China’s digital currency](https://www.reuters.com/article/us-china-cryptocurrency-cenbank/china-says-new-digital-currency-will-be-similar-to-facebooks-libra-idUSKCN1VR0NM), in the works for 5 years, will be somewhat similar to Libra
- LedgerLive finally [supports ERC20 tokens](https://www.ledger.com/ledger-live-securely-supporting-erc-20-tokens/)
- Eric Wall says [no to Hedera/Hashgraph](https://medium.com/@ercwl/hedera-hashgraph-time-for-some-fud-9e6653c11525)/whatever it’s called. [Followup](https://medium.com/@ercwl/counter-counter-fud-afed13a378c9).
- Missed this back then: in June, Jeffrey Berns closed the [deal to buy Kirkwood Bank of Nevada](https://thenevadaindependent.com/article/blockchains-ceo-charts-future-course-for-company-through-purchase-of-local-bank). So we should get another crypto-friendly bank, as promised at Devcon.
- For the 2nd straight week, I did an annotated version of the newsletter. Anyone who has bought the NFT can read it. Same link, you can still buy the NFT. See immediately below:

* * *

## **🎂 3 year anniversary 🎂**

Just to repeat the advertisement immediately above: you can [buy the limited edition NFT for 0.11 Eth](https://weekinethereumnews.com/three-year-anniversary-edition/) which will unlock the annotated edition.

All proceeds will be back into Ethereum somehow, likely donated to a public good, at my discretion. And who knows, maybe there will be future benefits for the 200 NFT holders?

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- **Sep 9-Oct 21 - [Kyber DeFi virtual hackathon](https://blog.kyber.network/kyber-defi-virtual-hackathon-620cdbe67c9f)**
- Sep 10-11 - [DeFi Summit](https://defisumm.it/) (London)
- Sep 15 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff/)
- Sep 15 - [Ethereal Tel Aviv](https://etherealsummit.com/events/ethereal-tel-aviv/)
- Sep 16 - [Tachyon accelerator application](https://labs.consensys.net/tachyon/) deadline
- Sep 15-16- [StarkWare sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- Sep 27 - [ErasureCon](https://erasure.xxx/con) (password: information) (SF)
- Oct 7 - [ENS workshop](https://medium.com/the-ethereum-name-service/ens-workshop-applications-are-now-open-f46db6c63384) (Osaka)
- Oct 8-11 - [DeVcon](https://devcon.org/) (Osaka) and [Devcon social events calendar](http://osaka.kickback.events/events/)
- Oct 19-20 - [Crosslink](https://crosslink.taipei/) (Taipei)
- **Nov 5-6 - [Decentralized insurance D1Conf](https://blog.etherisc.com/d1conf-2019-to-focus-on-blockchain-adoption-november-5-6th-in-malta-3b8b582ac7b4) (Malta)**
- Nov 8-10 - [ETHWaterloo](https://ethwaterloo.com/)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

I own 100% Week In Ethereum. Editorial control has always been me.

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then here’s a hint: don’t email me. Do put it on Reddit. It’s amazing to me how many people email me when every issue has a link at the bottom saying not to email me to get in the newsletter.

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **This headline stays as long as so many people continue to link to old URL and not the right one: [weekinethereumnews.com](https://weekinethereumnews.com/)**

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/week-in-ethereum-news-september-8-2019/](https://weekinethereumnews.com/week-in-ethereum-news-september-8-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

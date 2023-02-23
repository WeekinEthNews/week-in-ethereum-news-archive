---
title: "Week in Ethereum News <BR> August 23, 2020"
date: "2020-08-23"
---

## **Eth News and Links**

**Eth1**

- Latest [Turbogeth alpha release](https://github.com/ledgerwatch/turbo-geth/releases/tag/v2020.08.03-alpha)
- Notes from latest [Stateless Ethereum call](https://ethresear.ch/t/stateless-ethereum-call-8-digest/7869)
- Latest [core dev call](https://youtu.be/q6bIeSu7r9o?t=235). Beiko’s [notes](https://twitter.com/TimBeiko/status/1296808958842122245).
- [Increase gas price for SLOAD to 2300; CALL family, EXT\* family and BALANCE to 2500](https://notes.ethereum.org/@vbuterin/BkrNbeAfD)
- [EVM384](https://notes.ethereum.org/@axic/evm384): can we do fast crypto in the EVM?
- [eip2666 benchmarking](https://github.com/ethereum/pm/issues/200#issuecomment-678115862)
- EIP1559 [decreases the risk of 51% attacks](https://medium.com/@MicahZoltu/eip-1559-51-attacks-should-you-live-in-fear-d817be3759dc)
- Tim Roughgarden [contracted to simulate eip1559 and escalator algo](https://d24n.org/tim-roughgarden-will-work-on-eip-1559/)

**Eth2**

- This week, the Medalla testnet recovered from a catastrophic event and is finalizing again. Prysmatic’s [catalog of events](https://medium.com/prysmatic-labs/eth2-medalla-testnet-incident-f7fbc3cc934a) and Ben Edgington’s shorter [writeup](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200817)
- **Shout it from the rooftops**: [client diversity matters](https://blog.ethereum.org/2020/08/21/validated-why-client-diversity-matters/)**.** If you prefer to hear that in video form, I made a [short video on why the incident shows](https://youtu.be/dEYzsolkxd0) we need client diversity (and why the incident is great for eth2!)
- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200822)
- SigmaPrime’s [BeaconFuzz update](https://blog.sigmaprime.io/beacon-fuzz-07.html) on bug finding - you can help fuzz eth2 clients using the dockerized fuzzer
- [Lighthouse client](https://lighthouse.sigmaprime.io/update-28.html) update, nailing attestation inclusion
- [Lodestar client](https://medium.com/@colinrileyschwarz/lodestar-medalla-update-59865a5cce1a) update, lessons learned from Medalla and browser ready light client
- [Nimbus client](https://our.status.im/medalla-update-august-21/) update, performance and stability fixes
- Tutorial to [using rumor](https://notes.ethereum.org/@protolambda/rumor-tutorial) for client debugging
- an [eth2 clock](https://stokes.io/eth2-dashboard)
- A list of [eth2 tooling](https://notes.ethereum.org/@protolambda/eth2_tooling)
- Latest [eth2 call](https://youtu.be/g3fKTfBXArU?t=272). Notes from [Ben](https://hackmd.io/@benjaminion/S1b2sJhzv) and [Mamy](https://gist.github.com/mratsim/370f96bd0e50f3bc8bce4a7e4010f887)
- ZenGo initial results on [VDF design cryptanalysis](https://zengo.com/vdf-alliance-zengo-secure-eth-2-design/)

**Layer2**

- [USDT live on OMG](https://tether.to/tether-usdt-integration-live-on-omg-network/)
- [Golem picks zk sync](https://blog.golemproject.net/zksync/)
- dYdX announces they’re planning a [q4 StarkWare rollup](https://integral.dydx.exchange/scaling-with-starkware/)

* * *

### **This newsletter is made possible thanks to [Chainlink](https://chain.link/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/05/FE39n5_g-1.png)

Come learn about the leading ideas in DeFi from top teams building the next wave of smart contracts at the [Smart Contract Summit](https://www.smartcontractsummit.io/?utm_campaign=SmartCon-general&utm_medium=banner&utm_source=weekinethereumnews) (Aug 28 - 29th). Synthetix, Aave, SetProtocol, Nexus Mutual, Kyber and 70+ other DeFi project speakers are sharing what they’re building next at SmartCon.

* * *

**Stuff for developers**

- [Test your Solidity code](https://blog.trailofbits.com/2020/08/17/using-echidna-to-test-a-smart-contract-library) with the Echida fuzzer
- Sam Sun [finds a xSNXa bug](https://medium.com/xtoken/xsnxa-false-start-post-mortem-f26a7a735383)
- OpenZeppelin upgrades for [Buidler](https://forum.openzeppelin.com/t/openzeppelin-buidler-upgrades/3580) and [Truffle](https://forum.openzeppelin.com/t/openzeppelin-truffle-upgrades/3579)
- [Golem wasm and VM payloads alpha](https://blog.golemproject.net/alpha-reveal-new-golem/) release for devs
- [Dynamic value arrays](https://www.linkedin.com/pulse/dynamic-value-arrays-solidity-julian-goddard/) in Solidity
- For new web3 devs, remember: Ethereum [code is not a database](https://hackernoon.com/smart-contracts-are-not-databases-t43532qc)
- Debug and profile together with [Tenderly Organizations](https://blog.tenderly.co/tenderly-organizations/)

**Ecosystem**

- MetaMask restricts [commercial use forks with more than 10k users](https://medium.com/metamask/evolving-our-license-for-the-next-wave-of-metamask-users-81b0b494c09a)
- How to [get your old ENS deposit back](https://medium.com/the-ethereum-name-service/how-to-get-back-an-old-deposit-1e2b1767b930) and we’re now halfway through the [decaying price premium for expired ENS domains](https://medium.com/the-ethereum-name-service/halfway-through-the-decaying-price-premium-after-releasing-280k-names-analysis-414452cd51e)
- Ethereum Foundation: [beyond just ecosystem grants](https://blog.ethereum.org/2020/08/19/esp-beyond-grants/)

**Enterprise**

- SAP.com: [SAP integration with Ethereum mainnet](https://blogs.sap.com/2020/08/21/sap-integration-with-ethereum-mainnet/)
- AWS: [mint tokens with BurnerFactory and monitor them with BlockScout](https://aws.amazon.com/blogs/awsmarketplace/build-and-monitor-custom-ethereum-tokens-with-blockscout-from-aws-marketplace/)
- TheBlock [research report on CBDCs](https://www.theblockcrypto.com/post/75022/a-global-look-at-central-bank-digital-currencies-full-research-report) (central bank digital currencies)

**Application layer**

- More than [10b USD on ethereum](https://usdonethereum.com/) (now 11.3b) after [1b migrated from Tron to ETH](https://www.theblockcrypto.com/linked/75411/tether-1-billion-usdt-tron-ethereum-blockchain)
- A primer on [Synthetix futures](https://blog.synthetix.io/synthetic-futures-primer/)
- [YieldSpace](https://twitter.com/yield/status/1296143989444423681), an automated liquidity provider using time to maturity as an input
- Opium’s [credit default swaps](https://medium.com/opium-network/first-credit-default-swap-on-aave-credit-delegation-launched-5e3efc961317) using Aave credit delegation
- Andre Cronje is [now going to do yinsure](https://medium.com/iearn/yinsure-finance-a-new-insurance-primitive-77d5d4217896)
- Arbol goes live with [parametric rainfall insurance](https://www.arbolmarket.com/businesses-and-farmers-can-now-hedge-weather-risk-through-the-arbol-platform-and-chainlink-data/)
- [DeFi Safety](https://defisafety.com/elementor-255/): a score based on “process quality”
- POAP doing [Merkle AirDrops and tool to create raffles](https://medium.com/poap/poap-recap-h1-2020-fb71af56ecd7)
- Multis using Unlock for [monthly automatic subscription fees](https://multis.co/post/how-multis-automates-monthly-subscription-fees-using-unlock-protocol)
- Yield [farming with Set](https://medium.com/set-protocol/yield-farming-deep-dive-532a14cb4022)

**Tokens/Business/Regulation**

- A [framework for token value flows](https://bankless.substack.com/p/a-framework-for-token-value-flows)
- Haseeb Qureshi: [Unbundling Uniswap](https://medium.com/dragonfly-research/unbundling-uniswap-the-future-of-on-chain-market-making-1c7d6948d570)
- Preparing your ERC20 [token to list on Coinbase](https://blog.coinbase.com/securing-an-erc-20-token-for-launch-on-coinbase-68313652768f)
- [Proof of personhood](https://arxiv.org/pdf/2008.05300.pdf) paper, a review of sybil-resistance
- Hasu: YAM is a [Nakamoto scheme](https://insights.deribit.com/market-research/why-yam-is-a-nakamoto-scheme/)

**General**

- MyCrypto: [10 steps to avoid getting hacked](https://medium.com/mycrypto/the-10-best-things-you-can-do-to-not-lose-your-crypto-dba4f5c05c7) in crypto
- Binance on collaborating with governments [to thwart ransomware ring](https://www.binance.com/en/blog/421499824684900882/The-Bulletproof-Exchanger-Project-How-Binance-Helped-Take-Down-a-Cybercriminal-Group-Laundering-$42M)
- Elaine Shi’s [Foundations of Distributed Consensus & Blockchains](https://twitter.com/ElaineRShi/status/1295411007393796099) textbook is available for free
- Brave research on using [AZTEC confidential payments on a Quorum POA sidechain](https://brave.com/themis-smart-contracts-and-sidechains/)
- Sergio Demian Lerner: [Satoshi had an optimized miner](https://bitslog.com/2020/08/22/the-patoshi-mining-machine/) he didn’t release publicly
- Vitalik on [philosophy of blockchain coordination](https://vitalik.ca/general/2020/08/17/philosophy.html) and the accompanying [X of n trust models](https://vitalik.ca/general/2020/08/20/trust.html) in blockchains

* * *

## **Job Listings**

- MyCrypto's hiring [frontend wizards](https://mycrypto.bamboohr.com/jobs/view.php?id=22&source=aWQ9Ng%3D%3D…). Remote. ~UTC-7. Go all in this bull run.
- Celer Network: [Android developer](https://www.celer.network/career.html)
- Trail of Bits: [blockchain security engineers](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & [senior software engineers](https://jobs.lever.co/trailofbits/b9c65cdc-3fb9-4493-9073-73a4400f0e23)
- Drive global Chainlink adoption as an [Ecosystem Marketer](https://careers.smartcontract.com/o/marketing-director-ecosystem) & [Head of Growth](https://careers.smartcontract.com/o/head-of-growth)
- If you’re a dev, 0x is hiring [full-stack, back-end, front-end or Solidity](https://0x.org/about/jobs) devs

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH/DAI/USDC to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **I’m making daily crypto videos**

Every day, I’m making [5 minute videos on YouTube](https://www.youtube.com/channel/UCHp-CVlamUCjl3z0KBivHmg).

The available sponsorship slots [were tokenized ($EVAN) for this newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer). You can now buy enough for a newsletter OTC from me at the spot price, or directly on [Balancer](https://balancer.exchange/#/swap/ether/0x89E3aC6Dd69C15e9223BE7649025d6F68Dab1d6a).

Follow me on twitter: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-august-23-2020/](https://weekinethereumnews.com/week-in-ethereum-news-august-23-2020/)

Did you get **forwarded** this newsletter? **[Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- Aug 28-29 - Chainlink’s [Smart Contract Virtual Summit](https://www.smartcontractsummit.io/)
- Oct 2-30 - [EthOnline hackathon](https://www.ethonline.org/)
- Nov 6-7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)
- Nov 16 - [MetaMask Provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7)

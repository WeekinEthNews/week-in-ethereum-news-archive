---
title: "Week in Ethereum News <BR> June 14, 2020"
date: "2020-06-14"
---

## **Eth News and Links**

**Eth1**

- [Analysis of EIP1559](https://insights.deribit.com/market-research/analysis-of-eip-1559/) (fee market change) from Hasu and Georgios Konstantopoulos
- Latest [core devs call](https://youtu.be/c_JmTqeQkU4?t=245). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1271428329875353601): STATICCALL likely to be repriced to 40 gas, account abstraction prototype, option 2 for EIP2565, discussion of eth2 deposit proxy contract, YOLO ephemeral testnet issues
- Geth [v1.9.15](https://www.reddit.com/r/ethereum/comments/gywkuc/geth_v1915_berlin_eips_merged_and_exposed_for/) includes implementations of Berlin fork EIPs

**Eth2**

- Latest [what’s new in Eth2](https://hackmd.io/@benjaminion/wnie2_200612), Witti multi-client testnet quite stable, next testnet in a week called Altona
- Latest [Eth2 call](https://youtu.be/WmU3k2v4UA8?t=55). Notes from [Ben](https://hackmd.io/@benjaminion/SkfYVnJ68), discussion of validator key hygiene
- Prysmatic successfully [launched their Onyx testnet](https://medium.com/prysmatic-labs/introducing-the-onyx-testnet-6dadbd95d873). An updated guide to [staking on Onyx](https://medium.com/@steve.berryman/installing-and-running-an-ethereum-2-prysm-validator-on-the-testnet-c004dd7eece8)
- [Lighthouse client](https://lighthouse.sigmaprime.io/update-26.html) update - getting to the final spec, discv5 rewrite for CPU optimization, tiny RAM use
- [Updating and generating Kate witnesses in amortized sqrt(n) time](https://ethresear.ch/t/updating-and-generating-kate-witnesses-in-amortized-sqrt-n-time/7520)
- An explainer for [phase zero of eth2](https://quantstamp.com/blog/understanding-phase-0-the-current-stage-of-eth-2-0-development)
- IvanOnTech’s [eth2 explainer](https://academy.ivanontech.com/blog/breaking-down-eth-2-0-the-next-generation-of-ethereum)
- [Protecting withdrawal keys](https://www.attestant.io/posts/protecting-withdrawal-keys/)

**Layer2**

- A framework to compare and [evaluate layer2 solutions](https://medium.com/matter-labs/evaluating-ethereum-l2-scaling-solutions-a-comparison-framework-b6b2f410f955)
- Formally verifying [state channels with TLA+](https://blog.statechannels.org/breaking-state-channels/)
- [Volition](https://medium.com/starkware/volition-and-the-emerging-data-availability-spectrum-87e8bfa09bb): hybrid onchain/offchain data decision by users at the transaction level from StarkWare

### This newsletter is made possible by [Trail of Bits](https://www.trailofbits.com/)!

![](https://weekinethereumnews.com/wp-content/uploads/2020/05/2314423.jpeg)

Contract upgrades are not as safe as you think. Trail of Bits has [catalogued 17 different ways that upgrades can go wrong](https://blog.trailofbits.com/2020/06/12/upgradeable-contracts-made-safer-with-crytic/), and built tools that help validate upgrades before you run them. Use [Crytic](https://crytic.io/) to keep your contracts safe from these flaws.

* * *

**Stuff for developers**

- ethers [v5 is on npm](https://www.npmjs.com/package/ethers), though RicMoo is still updating documentation
- web3js [v1.2.9](https://www.reddit.com/r/ethereum/comments/gzwxi2/web3js_129_with_an_extended_transaction_event_api/) - better transaction submission tracking
- [Brownie and React](https://medium.com/@matnad/a-cooking-lesson-with-brownie-and-react-building-dapp-front-ends-on-ethereum-f19e22f7430e) starter tutorial
- [Querying your eth2 validator balance](https://blog.infura.io/checking-your-eth-2-0-validator-balance) with Infura
- [Async event-driven app architecture](https://medium.com/blockvigil/design-pattern-of-developing-ethereum-applications-on-ethvigil-api-gateway-b56337b0086a) with EthVigil
- 17 checks to make [upgradeable contracts safer](https://blog.trailofbits.com/2020/06/12/upgradeable-contracts-made-safer-with-crytic/) with Crytic
- [Diamond Setter](http://joeyzacherl.com/2020/06/diamond-setter-ethereum-smart-contract-manager/) manager for your Diamond Standard upradeable contracts

**Ecosystem**

- [Transaction pool analyzer tool](https://www.reddit.com/r/ethereum/comments/h10zl7/johoes_mempool_analyser_is_now_available_for/)
- [Deanonymization using transaction time and gas price analysis](https://arxiv.org/pdf/2005.14051.pdf). Use [good privacy hygiene](https://medium.com/@tornado.cash/how-to-stay-anonymous-with-tornado-cash-and-similar-solutions-efdecdbd7d37) and this isn’t a problem
- 3 transactions with massive transaction fees ([1](https://etherscan.io/tx/0xca8f8c315c8b6c48cee0675677b786d1babe726773829a588efa500b71cbdb65), [2](https://etherscan.io/tx/0xc215b9356db58ce05412439f49a842f8a3abe6c1792ff8f2c3ee425c3501023c), [3](https://etherscan.io/tx/0xfd10c9a4507c4ebf1db9f71e05ba8ea09f3603c9012c24195d731a1fadfa14d9)). First 2 paid over 10k ETH each for a transaction fee. Lots of speculation about who screwed up and how.
- Trueblocks: [how accurate is Etherscan?](https://medium.com/@tjayrush/how-accurate-is-etherscan-83dab12eeedd)

**Enterprise**

- [Baseline protocol explained](https://limechain.tech/blog/the-baseline-protocol-explained/)
- [Baselining business process across Microsoft Dynamics and Google Sheets](https://www.youtube.com/watch?v=JDQmatMZrr8) video

**DAOs and Standards**

- TheLAO is extending [Moloch v2 with Raid Guild’s Minion (programmatic proxy) framework](https://medium.com/@thelaoofficial/the-path-to-unaccredited-daos-with-minion-8113213f7195) for non-accredited investor baby DAOs
- DAOs: [governance as a service](https://medium.com/@ingamar/governance-as-a-service-a-new-business-model-for-daos-e59ed0a660b3)
- [EIP2711](https://github.com/MicahZoltu/EIPs/blob/274638c066be95fdd02cfeb139921029efc9526a/EIPS/eip-2711.md): Separate gas payer from msg.sender
- [EIP2718](https://github.com/MicahZoltu/EIPs/blob/35d61f1882ee499cd40758e3988d5928edc60aed/EIPS/eip-2718.md): Typed Transaction Envelope

**Application layer**

- Unstoppable Domains launches [blogs on the dweb](https://www.coindesk.com/unstoppable-domains-launches-censorship-resistant-blogging-platform) using 3Box and IPFS. Etherscan launches [BlockScan](https://medium.com/etherscan-blog/blockscan-the-search-engine-for-a-decentralized-web-20b4d3d20efb), a dweb search engine
- Use [Balancer pools as swing trading](https://medium.com/balancer-protocol/high-fee-balancer-pools-for-swing-trading-8bc1c169a4c2)
- a [Foundation Markets technical primer](https://withfoundation.com/blog/we-are-empowering-creators-to-build-their-own-markets-on-ethereum), automated market makers for artists
- Austrian post office returns with [CryptoStamps v2](https://crypto.post.at/)
- LexDAO’s [personal token factory](https://medium.com/lexdaoism/introducing-lexdao-org-and-the-first-legal-engineer-certified-personal-token-factory-2e97f7b2106c) with dispute resolution via their DAO vote
- Opyn now has [call options](https://twitter.com/opyn_/status/1271255781791289345)
- [TokenSets upgraded](https://medium.com/set-protocol/upgraded-robo-sets-now-live-on-tokensets-99810f8c6ae5) with better rebalancing for less slippage (ahem: higher returns!)
- PodsFinance: [Money legos with options](https://medium.com/podsfinance/money-legos-with-options-f7cb917facb5), lock aUSDC as collateral when selling American put options. Live on testnet

**Tokens/Business/Regulation**

- Bank Frick lets customers [replace SWIFT with USDC](https://www.bankfrick.li/en/about-bank-frick/media/bank-frick-adds-first-stablecoin-to-its-range-of-tradable-and-custodial-crypto-assets-with-usdc) for faster processing
- ConsenSys starts [KYC/AML compliance](https://consensys.net/blog/press-release/consensys-launches-codefi-compliance/) service
- Ontario Securities Commission [report on Quadriga](https://www.osc.gov.on.ca/quadrigacxreport/web/files/QuadrigaCX-A-Review-by-Staff-of-the-Ontario-Securities-Commission.pdf): Gerald Cotten lost 143m trading
- Tim Swanson: [40 crypto controversies to look into](https://www.ofnumbers.com/2020/06/08/40-cointroversies-to-look-into-over-the-summer/)
- [Dove Mountain Data](https://www.dovemountaindata.com/) - crypto venture investor directory and their deals
- [Opolis](https://twitter.com/opolis/status/1270687154344091650) live - HR/benefits solution for the US

**General**

- [Crypto data breaches so far in 2020](https://medium.com/mycrypto/2020-so-far-personal-information-dumps-and-cryptocurrency-9e639ac357bf)
- Crosstalk: [Cross side channel attack on Intel CPUs](https://www.vusec.net/projects/crosstalk/); can exploit SGX
- SGAxe: [Cacheout attack targeting SGX](https://cacheoutattack.com/)
- [Lamphone](https://www.zdnet.com/article/lamphone-attack-lets-threat-actors-recover-conversations-from-your-light-bulb/): measure light bulb variations from up to 80 ft away to record audio conversations
- Gavin Andresen: [Ethereum can scale Bitcoin](https://twitter.com/gavinandresen/status/1271561026199261185)
- **Checkout the job listings below!**

* * *

## **Job Listings**

- Reflexer Labs (RAI): [smart contract dev lead](https://angel.co/company/reflexer-labs/jobs/856024-smart-contract-lead-developer-ethereum), [fullstack JS dev](https://angel.co/company/reflexer-labs/jobs/856033-backend-javascript-web3-developer), [python/devops lead](https://angel.co/company/reflexer-labs/jobs/856049-python-devops-lead-web3-ethereum)
- Aave: Solidity Rockstar? let's build the future of DeFi together wecare@aave.com
- Nomic Labs (Buidler): join our [dev experience & tooling engineering](https://www.notion.so/nomiclabs/Systems-Programming-Engineer-efc1c3006d3f4dd29121489377b19e9e) team!
- Chainlink: [Lead Test Engineer](https://careers.smartcontract.com/o/lead-test-engineer-on-chainlink) and [Senior Software Security Engineer](https://careers.smartcontract.com/o/senior-software-security-engineer)
- [0x is hiring](https://0x.org/about/jobs) full-stack, back-end, front-end engineers + 1 data scientist
- OpenZeppelin is hiring! To apply, visit: [https://openzeppelin.com/jobs](https://openzeppelin.com/jobs/)
- Celer Network: [Android developer](https://www.celer.network/career.html)
- Trail of Bits is looking for masters of low-level security. [Apply here](https://jobs.lever.co/trailofbits/8b7f7fc1-efb0-4e89-b406-784c3a2d77e4).

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH/DAI/USDC to evan.ethereum.eth. Questions? thecryptonewspodcast -at-gmail

* * *

## **Housekeeping**

Follow me on Twitter [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get the **annotated edition of this newsletter** on Monday or Tuesday. Plus I tweet most of what makes it into the newsletter.

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-june-14-2020/](https://weekinethereumnews.com/week-in-ethereum-news-june-14-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- June 15 - Gitcoin [CLR matching grants](https://gitcoin.co/grants/) begins
- June 16 - deadline to apply for Gitcoin’s [Kernel incubator](https://gitcoin.co/blog/announcing-kernel/)
- **June 17 - [Stateless Ethereum](https://github.com/ethereum/pm/issues/181) call**
- **June 29 - [Swarm first public event](https://swarm-gateways.net/bzz:/alpha.swarm.eth/)**
- **Aug 2 - [ENS grace period](https://medium.com/the-ethereum-name-service/the-great-renewal-its-time-to-renew-your-eth-names-or-else-lose-them-afccea4852cb) begins to end**
- Oct 2-Oct 30 - [EthOnline hackathon](https://www.ethonline.org/)

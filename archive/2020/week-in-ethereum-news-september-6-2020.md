---
title: "Week in Ethereum News <BR> September 6, 2020"
date: "2020-09-06"
---

## **Eth News and Links**

**Eth1**

- Turbogeth [weekly alpha release](https://github.com/ledgerwatch/turbo-geth/releases/tag/v2020.09.01), upgrade to latest geth, experimental hdd sync, more RPC APIs
- [Getting started with Turbogeth](https://chasewright.com/getting-started-with-turbo-geth-on-ubuntu/) on Ubuntu (~700 gigs storage for archive node)
- Latest [core devs call](https://youtu.be/-Jefyrs4f70). Beiko’s [notes](https://twitter.com/TimBeiko/status/1301880286959947777), lots of discussion about EIPs below (gas cost increases!)
- [Alexandria](https://notes.ethereum.org/mh6eVBRIScagdTG4Jx4XUg?view), a sketch of state network over latest version of discovery protocol

**EIPs/Standards**

- EIP suggested process changes: [change abandoned to withdrawn](https://github.com/ethereum/EIPs/issues/2941) and [removing implementation as a core requirement](https://github.com/ethereum/EIPs/issues/2940)
- [EIP2926](https://eips.ethereum.org/EIPS/eip-2926): Chunk-Based Code Merkleization
- [EIP2929](https://eips.ethereum.org/EIPS/eip-2929): Gas cost increases for state access opcodes
- [EIP2930](https://eips.ethereum.org/EIPS/eip-2930): Optional access lists
- [EIP2935](https://eips.ethereum.org/EIPS/eip-2935): Save historical block hashes in state
- [EIP2936](https://eips.ethereum.org/EIPS/eip-2936): EXTCLEAR Opcode For SELFDESTRUCTed contracts
- [EIP2937](https://github.com/ethereum/EIPs/blob/1864f7134a08358d2242fbfb8200cee2e8bae543/EIPS/eip-2937.md): SET\_INDESTRUCTIBLE opcode
- [EIP2938](https://github.com/ethereum/EIPs/pull/2938/files): Account abstraction ([Evaluating account abstraction DoS vectors](https://ethresear.ch/t/dos-vectors-in-account-abstraction-aa-or-validation-generalization-a-case-study-in-geth/7937))
- [ERC2942](https://github.com/ethereum/EIPs/blob/a47f4df6401748177cc92a36e438f84b80c1e610/EIPS/eip-draft_title_abbrev.md): EthPM URI Specification

**Eth2**

- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200905)
- Danny Ryan’s [quick update](https://blog.ethereum.org/2020/09/01/eth2-quick-update-no-15/) - Medalla testnet is stable but eth2 _needs client diversity and_ you _are incentivized to pick a non-majority client_
- Images and guide to [validating on Raspberry Pi4 with Lighthouse/ Nimbus/ Prysm/ Teku](https://www.reddit.com/r/ethereum/comments/ikgp1z/ethereum_on_arm_new_eth20_raspberry_pi_4_image/)
- Latest [eth2 call](https://youtu.be/FhFIog9D0II?t=79). Notes from [Ben](https://hackmd.io/@benjaminion/S1bUH_R7w) and [Mamy](https://gist.github.com/mratsim/a4e733f8801d7c30861d89cb66b6f38d)
- [Shuffling in eth2](https://hackmd.io/@benjaminion/shuffling)
- An overview of [attestation](https://kb.beaconcha.in/attestation)
- Phase1: understanding [shards as “data availability layer](https://www.lakshmansankar.com/#/shards-as-data-availability-layers)”
- Fizzy wasm interpreter [v0.4](https://github.com/wasmx/fizzy/releases/tag/v0.4.0)
- [Shargri-la](https://ethresear.ch/t/shargri-la-a-transaction-level-sharded-blockchain-simulator/7936): shard simulator with an analysis of eth2 transaction fees

**Layer2**

- StarkWare’s [Cairo](https://medium.com/@StarkWare/hello-cairo-3cb43b13b209) STARK prover for generalized computation
- [Rollup diff compression](https://ethresear.ch/t/rollup-diff-compression/7933)
- Using that compression, optimistic rollup Fuel [benchmarks 2500 tps](https://twitter.com/fuellabs_/status/1300468388695810050) for token transfers

* * *

### **This newsletter is made possible thanks to [Trail of Bits](https://www.trailofbits.com/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/05/2314423.jpeg)

Conduct your own [minimum viable security audit](https://github.com/crytic/building-secure-contracts/blob/master/development-guidelines/workflow.md). Follow this process from Trail of Bits to invest in your own security, particularly when time is short and help may not be available.

* * *

**Stuff for developers**

- Solidity [v0.7.1](https://solidity.ethereum.org/2020/09/02/solidity-0.7.1-release-announcement/): functions can be defined at file level, copy calldata structs to storage
- New maintainer Chainsafe’s roadmap (TypeScript) for web3JS, [now with a v1.3 release candidate](https://medium.com/@colinrileyschwarz/chainsafe-receives-grant-from-ethereum-foundation-b7217065065d)
- Truffle [v5.1.43](https://github.com/trufflesuite/truffle/releases/tag/v5.1.43), better Solidity v0.7 support
- [CompoundJS](https://medium.com/compound-finance/compound-js-9d1e3e5742d8)
- rDai’s [library to track interest](https://patrickgallagher.dev/blog/2020/09/01/rtoken-project-utils-library)
- [Using external adapters](https://blog.chain.link/build-and-use-external-adapters/) in Chainlink
- Trail of Bits recommended [process for developing secure Eth code](https://github.com/crytic/building-secure-contracts/blob/master/development-guidelines/workflow.md)
- [Unique sorting in Solidity using value arrays](https://medium.com/coinmonks/unique-sorting-in-solidity-using-value-arrays-519546c84092)
- [BLS sigs](https://ethresear.ch/t/bls-signatures-in-solidity/7919) in Solidity

**Ecosystem**

- Crazy gas fees this week: Matcha has [free limit orders](https://matcha.xyz/blog/how-to-trade-defi-tokens-when-ethereum-gas-prices-spike) during this time of gas spikes. Dharma app has [free trades](https://twitter.com/Dharma_HQ/status/1299433888926687232) as well
- Remco Bloemen’s detailed tour through [scaling layer1](https://blog.0xproject.com/scaling-defi-layer-one-7eeb24aca4f0)
- Livepeer’s analysis of [how to deal with crazy gas prices](https://medium.com/livepeer-blog/livepeer-protocol-scaling-during-times-of-high-ethereum-gas-prices-f13614562d6a)

**Application layer**

- [Uniswap hit #1 on DefiPulse](https://twitter.com/defipulse/status/1300911921936433152) because of SushiSwap
- SushiSwap cashes out all of the accrued [“10% to themselves” tokens for 38k ETH](https://etherscan.io/tx/0x419a835b33eb03481e56a5f964c1c31017ab196cb7bb4390228cabcf50dfd6f1) (Irony: they used Uniswap via ZapperFi). Many [call it an exit scam](https://twitter.com/search?q=sushiswap%20scam&src=typed_query). Sushi founder [says](https://twitter.com/NomiChef/status/1302222318618308609) he will stay involved, and has now [transferred control to FTX’s Sam Bankman-Fried](https://twitter.com/NomiChef/status/1302509536943640577). There are rumors of who the Sushi founder is; he denies it.
- A few Uniswap/Sushiswap clones. No link necessary.
- An attempt to [put a token on top of Uniswap v2](https://medium.com/unipool-finance/unipool-the-uniswap-union-7bd927044cd8)
- [Swerve](https://swerve.fi/), a new fork of Curve, reached almost $500m in total value locked in under a week.
- [Pine is live on mainnet](https://medium.com/@pine_eth/pine-finance-an-amm-orders-engine-525fe1f1b1eb) (formerly UniswapEx) limit orders on Uniswap v1 and v2
- Brave at [18m+ monthly active users](https://twitter.com/BrendanEich/status/1300849501410701318)

**Tokens/Business/Regulation**

- the [web3 sustainability loop](https://blog.oceanprotocol.com/the-web3-sustainability-loop-b2a4097a36e)
- a [yearn/YFI yield harvesting explainer](https://medium.com/@finematics/yearn-finance-and-yfi-token-explained-229d66106b69)

**Crypto/General**

- [Explaining Halo2](https://electriccoin.co/blog/explaining-halo-2/), a SNARK without trusted setup (replaces SONIC with PLONK)
- ZenGo’s [DogByte attack](https://medium.com/zengo/dogbyte-attack-playing-red-team-for-eth2-0-vdf-ea2b9b2152af) on VDF’s mpc ceremony
- [Man in the middle ransom](https://www.coindesk.com/trezor-keepkey-wallets-attack) attack on Trezor/KeepKey
- CipherTrace announces [product to track Monero transactions](https://ciphertrace.com/ciphertrace-announces-worlds-first-monero-tracing-capabilities/)
- [Understanding Ethereum by studying](https://gisli.hamstur.is/2020/08/understanding-ethereum-by-studying-the-source-code/) Geth

* * *

## **Job Listings**

- Want to work in DeFi? [mStable](https://mstable.org) is hiring a [Protocol](https://cryptocurrencyjobs.co/engineering/mstable-protocol-developer-defi/) Developer
- Props is hiring [full-stack](https://propsproject.com/careers/?gh_jid=2295299), [Product Manager](https://propsproject.com/careers/?gh_jid=2295035), [Finance Lead](https://propsproject.com/careers/?gh_jid=2295034) and [Marketing Lead](https://propsproject.com/careers/?gh_jid=1276877).
- DAIswaps@gmail.com - Seeking skilled eth devs for DEX/DeFi. fulltime 🧙🤑🤖
- Trail of Bits is looking for [blockchain security engineers](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf) & an [R&D engineer](https://jobs.lever.co/trailofbits/94f47428-7c88-43dd-846d-93e3d3059337)
- 0x is hiring devs! [Full-stack, back-end, front-end or Solidity](https://0x.org/about/jobs)
- Inspire Chainlink's community as a [Head of DevRel](https://careers.smartcontract.com/o/head-of-developer-relations) & [Dev Evangelist](https://careers.smartcontract.com/o/developer-evangelist)
- Celer Network: hiring Solidity and Go devs. Email: hiring@celer.network

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH/DAI/USDC to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **My [Nifty.ink](https://nifty.ink/) artwork on sale (and newsletter sponsorships)**

I drew the Eth rainbow logo using nifty.ink \[very noob friendly; send to your artist friends!\] and put in on sale. You can buy it or watch how I made it here: [https://nifty.ink/QmeYK5yHCoZ1Upe1cHcoQvi7hPVvwmAxfZFtUd3DB5K2iS](https://nifty.ink/QmeYK5yHCoZ1Upe1cHcoQvi7hPVvwmAxfZFtUd3DB5K2iS)

The available sponsorship slots have been [for this newsletter have been tokenized](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer) as $EVAN. You can now buy enough for a newsletter OTC from me at the spot price, or directly on [Balancer](https://balancer.exchange/#/swap/ether/0x89E3aC6Dd69C15e9223BE7649025d6F68Dab1d6a) - but you’ll likely get a better price from me.

Follow me on twitter: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-6-2020/](https://weekinethereumnews.com/week-in-ethereum-news-september-6-2020/)

Did you get **forwarded** this newsletter? **[Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **Sep 17 - [Q&A for devs new to Ethereum](https://twitter.com/ljxie/status/1301588925006319618)**
- Oct 1-30 - [EthOnline hackathon](https://www.ethonline.org/)
- Nov 6-7 - virtual [Trufflecon](https://www.trufflesuite.com/trufflecon2020)
- Nov 16 - [MetaMask Provider breaking changes](https://medium.com/metamask/breaking-changes-to-the-metamask-provider-its-happening-eebc91fff1a7)

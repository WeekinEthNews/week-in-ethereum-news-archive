---
title: "Week in Ethereum News<BR> May 31, 2020"
date: "2020-05-31"
---

## **Eth News and Links**

**Eth1**

- Latest [core devs call](https://youtu.be/UJ1jK73rKdk?t=219), discussion of EIPs for inclusion in Berlin hard fork, whether or not to include 2046 (static call to precompile gas reduction) and 2565 (modexp reprice). Working toward an ephemeral testnet for Berlin.
- Latest [fee market change (1559) call](https://www.youtube.com/watch?v=MVjHEIdgaRo). Notes from the [EIP1559 call](https://twitter.com/TimBeiko/status/1265989911225798662)
- Discussion thread on [meta transactions, oil, opcode repricing](https://ethresear.ch/t/meta-transactions-oil-and-karma-megathread/7472)
- [Snap sync mainnet benchmarking](https://twitter.com/peter_szilagyi/status/1264801013174845442), single peer on AWS

**Eth2**

- Latest [what’s new in eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_200530), features a Schlesi testnet postmortem
- The new [multi-client testnet is Witti](https://witti.beaconcha.in/). Here’s a [guide to staking](https://medium.com/@SomerEsat/guide-to-staking-on-ethereum-2-0-ubuntu-prysm-witti-2b972e697918)
- Latest [eth2 implementer call](https://www.youtube.com/watch?v=xvIk22HvTVE). Notes from [Ben](https://hackmd.io/@benjaminion/H1h7zHTiL) and [Mamy](https://gist.github.com/mratsim/813c041b58bfc2f2f34722c3cdcffac2)
- [Cross-shard transaction simulation](https://ethresear.ch/t/cross-shard-transaction-probabilistic-simulation/7474)
- [8 things you should consider before staking](https://medium.com/chainsafe-systems/8-things-every-eth2-validator-should-know-before-staking-94df41701487)
- RocketPool is going to [wrap the ETH locked up in Eth2 staking](https://medium.com/rocket-pool/rocket-pool-2-5-tokenised-staking-48601d52d924), thus giving liquidity to eth2 stakers

**Layer2**

- [Raiden v1](https://medium.com/raiden-network/alderaan-mainnet-release-announcement-7f701e58c236) is live on mainnet for DAI and WETH, with some token limits
- [Deconstructing a state channel app](https://blog.statechannels.org/deconstructing-a-state-channel-application/) and how a dev interacts with a state channel wallet
- A [zk-rollups to scale blockchain](https://bankless.substack.com/p/can-fancy-new-cryptography-scale) explainer
- [Understanding optimistic rollups](https://gourmetcrypto.substack.com/p/optimistic-rollups-from-the-bottom) by building one
- Dharma and Interstate open source their [Tiramisu optimistic rollup](https://blog.dharma.io/introducing-tiramisu-dharma-l2/) for token transfers

### This newsletter is made possible by [Chainlink](https://chain.link/)!

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fac0a39e0-62f4-4c16-a069-82b479b231f9_925x285.png)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fac0a39e0-62f4-4c16-a069-82b479b231f9_925x285.png)

Connect your smart contract to decentralized oracles that provide the most tamper-proof and [accurate market price data](http://defi.chain.link/), as well as [on-chain verifiable randomness](https://docs.chain.link/docs/chainlink-vrf) that’s provably fair. 

**Stuff for developers**

- [Array slices](https://solidity.ethereum.org/2020/05/26/array-slices) in Solidity v0.6
- Truffle [v5.1.27](https://github.com/trufflesuite/truffle/releases/tag/v5.1.27) - debugger support for Solidity inline assembly
- [Upgradeable contracts](https://hiddentao.com/archives/2020/05/28/upgradeable-smart-contracts-using-diamond-standard) using diamond standard
- [web3j now includes abi v2](https://blog.web3labs.com/abiv2-comes-to-web3j)
- Typescript [types for Solidity AST](https://forum.openzeppelin.com/t/solidity-ast-types/2883)
- [i18n translation strings for Defi](https://defi18n.com/), available as npm package
- [Build your first Harberger tax app](https://dev.to/wildcards/build-your-first-harberger-tax-app-part-1-3gdd) tutorial
- [eth95](https://github.com/adrianmcli/eth95): retro UI for calling contract functions
- [secp256k1 twist attacks](https://github.com/christianlundkvist/blog/blob/master/2020_05_26_secp256k1_twist_attacks/secp256k1_twist_attacks.md)
- [BLS12-381 pairing-friendly curve](https://github.com/paulmillr/noble-bls12-381) in JavaScript, now with hash-to-curve v7 and 50 pairings/sec

**Ecosystem**

- [Devcon6 will be in Bogota in 2021](https://blog.ethereum.org/2020/05/28/devcon-hacia-colombia-en-2021/)
- All the projects from EthGlobal’s [Hack Money](https://hack.ethglobal.co/online/showcase)

**Enterprise**

- [First Central Bank Digital Currency public blockchain transaction](https://www.societegenerale.com/en/newsroom-first-financial-transaction-settled-with-a-digital-currency) is on Ethereum: Societe General issued €40m of covered bonds as security tokens and paid with Banque de France digital euros. While the press release does not make it clear, the [transaction was on Ethereum](https://www.fitchratings.com/research/banks/sg-covered-bonds-issued-settled-with-blockchain-technology-21-05-2020) mainnet

**DAOs and Standards**

- [Summoning the spirit of DAO ops](https://medium.com/abridged-io/summoning-the-spirit-of-dao-ops-5928ee26b9d5)
- [ERC2680](https://github.com/ethereum/EIPs/blob/d11bf27bdac54155b6a7047f85050bac0937e42c/EIPS/eip-2680.md): eth2 standard wallet layout and naming format 
- [ERC2678](https://github.com/ethereum/EIPs/blob/9e80aae10133e15c248610dbbe5c0e14f01628d4/EIPS/eip-2678.md): EthPM v3
- [EIP2681](https://github.com/ethereum/EIPs/blob/9432fa173cd6f107555de43bbd3debe57dc57861/EIPS/eip-2681.md): Limit account nonce to 2^64-1
- [EIP2677](https://github.com/ethereum/EIPs/blob/07d834a2f7a607b097bad2b024333ea39083b0f7/EIPS/eip-2677.md): Limit initcode size

**Application layer**

- [Enjin plugin for Minecraft](https://blog.enjin.io/enjincraft-plugin-for-minecraft/) to tokenize Minecraft items on your server
- [Umbra](https://www.scopelift.co/blog/introducing-umbra): stealth payments to ENS names, running on Ropsten testnet
- How does [NexusMutual become an efficient version of Lloyd’s of London](https://forum.nexusmutual.io/t/towards-new-risks/50)?
- Maker’s Oasis now [makes it easy to leverage up](https://blog.oasis.app/introducing-multiply-on-oasis-trade/) with ETH
- [DeFi777](https://medium.com/@dmihal/introducing-defi777-decentralized-finance-for-everyone-dc3f87bea70d) - wrap your erc20 tokens as erc777 tokens, then swap through ENS names
- [RenVM brings BTC, BCH, and ZEC](https://medium.com/renproject/renvm-mainnet-release-98cac4c6fa8e) to Ethereum as ERC20 tokens
- [Mstable basket of stablecoins](https://medium.com/mstable/mstable-now-live-on-mainnet-c9f55f748ac7) live on mainnet, includes yield from Compound/Aave plus swap fees - there’s a zero slippage stablecoin trade with 30 basis points of fees
- [Centrifuge](https://medium.com/centrifuge/introducing-decentralized-asset-finance-onboarding-the-world-to-defi-f400ad906546)’s Tinlake asset factoring is on mainnet, with factoring for freight shipping and Spotify payments

**Tokens/Business/Regulation**

- Liquidity mining: now you earn [Balancer tokens](https://medium.com/balancer-protocol/balancer-liquidity-mining-begins-6e65932eaea9) for supplying liquidity or [Compound tokens](https://medium.com/compound-finance/expanding-compound-governance-ce13fcd4fe36) for supplying/borrowing
- [Zap your liquidity around in one transaction](https://defitutorials.substack.com/p/defragmenting-liquidity-with-pool)
- Ryan Sean Adams: [Eth is doubly undervalued](https://bankless.substack.com/p/eth-is-doubly-undervalued-market-7ae)
- Gavin Andresen: [crypto markets take a long time to reflect reality](http://gavinandresen.ninja/it-s-not-about-the-tech-yet)

**General**

- [LadderLeak and ECDSA](https://soatok.blog/2020/05/26/learning-from-ladderleak-is-ecdsa-broken/) explainer
- [Hundreds of thousands of Thai users switching to Minds](https://qz.com/1860804/thai-users-ditch-twitter-for-crypto-social-network-minds/), a Twitter/Facebook hybrid social network incentivized through an ERC20 token

* * *

## **Housekeeping**

Follow me on Twitter [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get the **annotated edition of this newsletter** on Monday or Tuesday. Plus I tweet most of what makes it into the newsletter.

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-may-31-2020/](https://weekinethereumnews.com/week-in-ethereum-news-may-31-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **June 1-6 - [DAO Rush Week](https://daorushweek.com)**
- **June 3 - BlockVigil’s free [remote developer bootcamp](https://medium.com/blockvigil/announcing-the-blockvigil-remote-developer-bootcamp-2nd-edition-27f3d4c21eee) begins**
- June 16 - deadline to apply for Gitcoin’s [Kernel incubator](https://gitcoin.co/blog/announcing-kernel/)
- **Oct 2-Oct 30 - [EthOnline hackathon](https://www.ethonline.org/)**

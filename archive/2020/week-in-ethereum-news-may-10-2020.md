---
title: "Week in Ethereum News<BR> May 10, 2020"
date: "2020-05-10"
---

## **Eth News and Links**

**Eth1**

- Step by step guide to [running a Hyperledger Besu node on mainnet](https://pegasys.tech/running-a-hyperledger-besu-node-on-the-ethereum-mainnet-benefits-requirements-and-setup/)
- Nethermind [v1.18.30](https://github.com/NethermindEth/nethermind/releases/tag/1.8.30) query the chain and trace transactions within minutes with Beam sync
- A [primer on block witnesses](https://blog.ethereum.org/2020/05/04/eth1x-witness-primer/)
- Installation guide to [running eth1 nodes (or eth2 testnet) on RaspberryPi4](https://www.reddit.com/r/ethereum/comments/gf3nhg/ethereum_on_arm_raspberry_pi_4_images_release/)

### This newsletter is made possible by [Celer](https://www.celer.network/)!

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F78edba42-79f2-4d84-840c-20a93fb42aaa_950x400.png)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F78edba42-79f2-4d84-840c-20a93fb42aaa_950x400.png)

[Celer](http://celer.network/) has just released a new state channel [mainnet upgrade](https://blog.celer.network/2020/05/08/celer-launches-orion-mainnet-upgrade-ready-for-large-scale-node-expansion-on-ethereum-layer-2/) enabling everyone to easily [run a layer-2 state channel node](https://github.com/celer-network/goCeler-oss) and to utilize the low-cost and real-time transactions enabled by Celer. Game developers with no blockchain knowledge today monetize their games through [CelerX gaming SDK](http://developer.celerx.app/) that leverages the underlying layer-2 scaling technology with ease. Celer has also released the world’s first [skill-based real money game apps](http://celerx.app/) where players can join multi-player game tournaments and [win cryptocurrency prizes](https://apps.apple.com/us/app/arcade-win/id1459895768), Follow us on [twitter](https://twitter.com/CelerNetwork), [blog](https://blog.celer.network/), [discord](https://discord.com/invite/Trhab5w) and [telegram](https://t.me/celernetwork).

**Eth2**

- Danny Ryan’s latest [quick eth2 update](https://blog.ethereum.org/2020/05/06/eth2-quick-update-no-11/) - bug bounties doubled, latest IETF BLS standard
- PegaSys’s [Teku client is now syncing the Schlesi testnet](https://twitter.com/cemozer_/status/1258189567624196099) - which has been much more stable than expected
- Latest [Prysmatic client](https://medium.com/prysmatic-labs/eth-2-0-dev-update-49-multiclient-testnet-security-audit-741ae1049ebf) update - reducing RAM usage, slashing protection
- SigmaPrime’s [Beacon fuzzer](https://blog.sigmaprime.io/beacon-fuzz-04.html) update, struct-aware, bugs found in Teku and Nimbus
- Latest [Eth2 networking call](https://www.youtube.com/watch?v=VPgMe6CVf5Q), gossipsub v1.1. Ben’s [notes](https://hackmd.io/@benjaminion/rJkuZ4e5I)
- Python notebook to [simulate a network partition](https://github.com/ethereum/rig/blob/master/eth2economics/code/beaconrunner2049/beacon_runner_2049.ipynb)
- [Apostille](https://ethresear.ch/t/eth1x64-variant-1-apostille/7365), an Eth1x64 variant
- Scoping what is necessary to [port eth1 to an eth2 shard and turn off proof of work](https://ethresear.ch/t/the-scope-of-eth1-eth2-merger/7362)

**Layer2**

- [Demo of Synthetix on the OVM](https://blog.synthetix.io/synthetix-exchange-l2-demo/) includes paper trading competition with 50k SNX prizepool. The details of how the [Optimistic Virtual Machine enables EVM-in-EVM](https://medium.com/ethereum-optimism/ovm-deep-dive-a300d1085f52)
- [Gods Unchained building an NFT exchange with StarkWare](https://blog.godsunchained.com/2020/05/08/introducing-immutable-x/)
- [Exit games in state channels](https://blog.statechannels.org/state-channel-exit-games/)
- Celer Network’s Orion upgrade makes it [easy to run a state channel node](https://blog.celer.network/2020/05/08/celer-launches-orion-mainnet-upgrade-ready-for-large-scale-node-expansion-on-ethereum-layer-2/)

**Stuff for developers**

- Solidity [v0.6.7](https://github.com/ethereum/solidity/releases/tag/v0.6.7), EIP165 (standard interface detection) support. Also [survey results on what devs love and hate](https://twitter.com/solidity_lang/status/1258432533286584322) about Solidity
- [Solhint v3](https://github.com/protofire/solhint/releases/tag/v3.0.0) - Solidity linter removes styling rules and recommends [prettier Solidity](https://github.com/prettier-solidity/prettier-plugin-solidity) instead
- [Open Zeppelin ethers.js based console](https://github.com/pooltogether/oz-console)
- [Etherplex](https://github.com/pooltogether/etherplex): batch multiple JSON RPC calls into single call
- [Time-based Solidity tests](https://medium.com/@adrian_g/back-to-the-future-testing-solidity-through-time-with-brownie-5da4f257e2cb) with Brownie
- [MythX now has 46 detectors](https://medium.com/consensys-diligence/mythx-smart-contract-security-api-update-revamped-vulnerability-detection-and-new-property-4b4ab8194198)
- Quiknode has an [online tool to test endpoints](https://www.quiknode.io/compare)
- Reading Eth [price from Maker’s medianizer v1](https://studydefi.com/read-maker-medianizer/)
- [Build an app with Sablier’s constant streaming](https://medium.com/sablier/how-to-build-a-sablier-powered-dapp-cee47eb648dc) tutorial
- [Building a bot using MelonJS](https://medium.com/melonprotocol/building-a-melonbot-1cdea583fb88) to automate your Melon fund
- [StarkWare found a vulnerability](https://medium.com/starkware/looprings-frontend-vulnerability-explained-106df1aa17db) in Loopring’s frontend where passwords were being hashed to only 32 bit integers

**Ecosystem**

- A chart of [ETH issuance over time](https://www.attestant.io/posts/charting-ethereum-issuance/). The best I’ve seen
- Ethereum Foundation’s [q1 grants list](https://blog.ethereum.org/2020/05/07/ecosystem-support-program-allocation-update-q1/)
- A guide to [bulk renewing your ENS names](https://medium.com/the-ethereum-name-service/step-by-step-guide-to-bulk-renewals-of-eth-names-daeb043124c1)
- ethereum.org looking for [Vietnamese, Thai, Danish, Norwegian, Hungarian, Finnish, or Ukranian translators](https://blog.ethereum.org/2020/05/05/ethereum.org-development-update-3/)
- A review of [hardware for eth staking](https://old.reddit.com/r/ethstaker/comments/ggmbvd/a_comprehensive_look_at_hardware_for_staking/)

**Enterprise**

- PegaSys’s [Hyperledger Besu suite available on Azure Marketplace](https://consensys.net/blog/press-release/consensys-and-microsoft-collaborate-to-bring-ethereum-to-enterprises-with-the-pegasys-ethereum-suite/) and Microsoft’s blockchain devkit now supports Besu
- Quorum [v2.6](https://github.com/jpmorganchase/quorum/releases/tag/v2.6.0) - breaking database schema changes, update to geth v1.9.x

**Governance, DAOs, and standards**

- [How to start a MolochDAO](https://bankless.substack.com/p/how-to-start-a-moloch-dao)
- Options for [delegated voting in KyberDAO](https://blog.kyber.network/kyberdao-options-for-pool-operators-d2ea050c76c5)
- [EIP2633](https://github.com/ethereum/EIPs/blob/92473a28bc09cb189c2efd57cb924406347b3f2c/EIPS/eip-2633.md): Formalized upgradable governance
- [EIP2628](https://github.com/ethereum/EIPs/blob/4c85bc1098e7b1e1c22c43e2c1c324b552f27b35/EIPS/eip-2628.md): Header in StatusMessage

**Application layer**

- [Use POAP](https://medium.com/poap/poaps-next-chapter-6be604961261) for sybil-resistant voting or to determine Discord channel access
- [Yield](https://twitter.com/niemerg/status/1258488654437195779): a revised implementation of Dan Robinson’s yTokens for fixed rate, fixed term loans that give a yield curve
- Comparing [total value locked in DeFi to unique active addresses](https://thecontrol.co/defi-usage-numbers-7e5e2cd5ab2e)
- [75 interesting uses of social money](https://twitter.com/sidkal/status/1258381746464346114) by Roll
- Personal tokens were the topic du jour, check out this [overview from Dan Finlay](https://twitter.com/danfinlay/status/1258008200126664705)
- [Strike](https://medium.com/@strikeprotocol/introducing-strike-decentralized-perpetual-swaps-for-every-asset-9acfc52c3ec8): perpetual swaps with 20x leverage

**Tokens/Business/Regulation**

- Nic Carter: [are stablecoins parasitic or beneficial](https://bankless.substack.com/p/crypto-fiat-mutualistic-or-parasitic)?
- [OpenRaise](https://medium.com/bitfwd/distributed-capital-formation-with-openraise-3af9a601ad63): a continuous offering fundraiser for DAOs
- dxDAO’s [kickstarter using OpenRaise](https://daotalk.org/t/dxdao-dxtrust-and-dxd/1304) sold out before public announcement - though the curve is still live, plus a secondary Uniswap market

**General**

- [Aggregatable Subvector Commitments](https://eprint.iacr.org/2020/527), the future may not involve Merkle trees
- This week, Ethereum mined its [10 millionth block](https://twitter.com/etherchain_org/status/1257300024259641344).
- Here’s MyCrypto’s [history of Eth hard forks](https://medium.com/mycrypto/the-history-of-ethereum-hard-forks-6a6dae76d56f) to celebrate 10m blocks
- [IPFS releases Testground suite](https://blog.ipfs.io/2020-05-06-launching-testground/) for p2p networking tests
- [PayPal blocked tokenized real estate startup RealT](https://realt.co/paypal-axed-us/) despite a lack of chargebacks, so they’re switching to Wyre

* * *

## **Housekeeping**

Follow me on Twitter [@evan\_van\_ness](https://twitter.com/evan_van_ness) for a one-stop source for real-time Ethereum news.

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-may-10-2020/](https://weekinethereumnews.com/week-in-ethereum-news-may-10-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **May 11 - [RAC’s $TAPE](https://twitter.com/ourZORA/status/1257293995035602944)**
- **May 12 - [MakerDAO Sai shutdown deadline](https://twitter.com/MakerDAO/status/1255186078505422848)**
- May 22-31 - [Ethereum Madrid](https://ethereummadrid.com/hackathon-2020-update/) public health virtual hackathon
- May 29-June 16 - [SOSHackathon](https://soshackathon.com/)
- June 17 - [EthBarcelona](https://ethbarcelona.github.io/) R&D workshop

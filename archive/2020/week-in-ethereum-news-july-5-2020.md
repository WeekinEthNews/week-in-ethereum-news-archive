---
title: "Week in Ethereum News <BR> July 5, 2020"
date: "2020-07-05"
---

## **Eth News and Links**

**Eth1**

- Nethermind [v1.8.60](https://github.com/NethermindEth/nethermind/releases/tag/1.8.60) memory usage during sync reduced 70%
- [Ethereum without block limits](https://medium.com/@MicahZoltu/a-world-without-block-limits-f3ecc926cd68)
- Igor Mandrigin explains the [ReGenesis](https://medium.com/@mandrigin/regenesis-explained-97540f457807) proposal for curbing state growth with transaction witnesses
- a proposed [binary trie format](https://ethresear.ch/t/binary-trie-format/7621) - no more RLP?

**Eth2**

- [Altona multiclient testnet](https://altona.beaconcha.in/) launched almost a week ago with Lighthouse, Nimbus, Prysmatic and Teku clients and (so far) is stable. One more testnet after Altona until launch.
- Step by step [guide to run an Altona validator](https://hive.blog/ethereum/@tarekadam/altona-test-net-validator-using-raspberry-pi4b-8-gb) on Raspberry Pi4B 8 GB
- [Prysmatic client](https://medium.com/prysmatic-labs/eth-2-0-dev-update-53-altona-testnet-launched-bf41173a8513) update
- [Weak subjectivity](https://notes.ethereum.org/@adiasg/weak-subjectvity-eth2) in eth2
- [Deanonymization using time sync](https://ethresear.ch/t/de-anonymization-using-time-sync-vulnerabilities/7610)
- [Public single leader election](https://ethresear.ch/t/public-single-leader-election-psle-secret-probabilistic-backup-election-spbe/7633) with secret probabilistic backup

**Layer2**

- IvanOnTech [rollups explainer](https://academy.ivanontech.com/blog/breaking-down-eth-2-0-zk-snarks-and-zk-rollups)
- [Brick](https://arxiv.org/abs/1905.11360) async payment channels implemented in Solidity (revised arxiv paper)

* * *

### **This newsletter is made possible thanks to [Celer Network](https://www.celer.network/)!**

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F0ebc70fd-ff68-4d9b-879b-76e9cea3b2af_950x400.png)](https://cdn.substack.com/image/fetch/c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F0ebc70fd-ff68-4d9b-879b-76e9cea3b2af_950x400.png)

[Celer](http://celer.network/) is a coherent layer-2 scaling platform on Ethereum powered by [Generalized State Channel Network](https://www.celer.network/docs/celercore/index.html) and [Hybrid Rollup](https://medium.com/celer-network/adding-hybrid-pos-rollup-sidechain-to-celers-coherent-layer-2-platform-d1d3067fe593) technology. Real money games, such as [Arcade Win](https://apps.apple.com/us/app/arcade-win/id1459895768) and [Daub Cash](https://apps.apple.com/us/app/daub-cash/id1513396754), built using [Celer's gaming-focused SDK](http://developer.celerx.app/) just reached top #10 ranking in App Store. You can [easily set up](https://github.com/celer-network/goCeler-oss) and join Celer's [growing layer-2 State Channel Network](http://explorer.celer.network/) to support Ethereum's layer-2 scalability. Follow us on [twitter](https://twitter.com/CelerNetwork), [blog](https://blog.celer.network/), [discord](https://discord.com/invite/Trhab5w) and [telegram](https://t.me/celernetwork).

* * *

**Stuff for developers**

- [Gelato automation protocol](https://medium.com/@gelatonetwork/ethereums-automation-protocol-gelato-network-launches-on-mainnet-88647aa10d65) is live on mainnet, an IFTTT-like way to automate Eth contract execution
- Hack on [eth2+libp2p at HackFS](https://twitter.com/dannyryan/status/1279443288756416512)
- [buidler deploy](https://github.com/wighawag/buidler-deploy). Buidler plugin to deploy contracts to any network with same testing environment
- seth now lets you [step through the transaction in debugging](https://twitter.com/MartinLundfall/status/1276559264098721792)
- [Debugging your transaction](https://ethereumdev.io/debugging-your-ethereum-transactions-with-tenderly/) with Tenderly
- A [simple ABI decoder](https://cleanunicorn.github.io/santoku/#/)
- Build [Ethereum apps on Python with EthVigil SDK](https://medium.com/blockvigil/build-ethereum-apps-on-python-with-ethvigil-sdk-517abdb25979)
- Vyper [v0.2](https://vyper.readthedocs.io/en/latest/release-notes.html) - breaking changes release
- [State machines](https://medium.com/coinmonks/state-machines-in-solidity-9e2d8a6d7a11) in Solidity
- [Class features](https://medium.com/coinmonks/class-features-provided-by-solidity-84ee97840666) provided by Solidity
- 1inch writeup of [Balancer deflationary’s token issue](https://medium.com/@1inch.exchange/balancer-hack-2020-a8f7131c980e) which BalancerLabs chose to [cover for affected users](https://medium.com/balancer-protocol/update-2-incident-with-non-standard-erc20-deflationary-tokens-f3a7cedf6292)

**Ecosystem**

- Transaction fees on Ethereum in [first half of 2020 (44m) exceed 2019 (34m)](https://twitter.com/0xstark/status/1278369273640091648)
- [the plan for Waku v2](https://vac.dev/waku-v2-plan) private p2p messaging
- Austin Griffith’s [xmoon exchange](https://twitter.com/austingriffith/status/1279078134349025281): get your Reddit MOONs onto mainnet
- [Quadratic matching with MACI](https://www.maxgrok.com/posts/clrfund) (anti-collusion) explainer
- [MetaMask v8](https://medium.com/metamask/announcing-metamask-version-8-9126dc2df98) - better privacy, better onboarding, erc1193 provider api

**DAOs and Standards**

- [ERC2767](https://github.com/ethereum/EIPs/blob/dfbfbef9f728cdb55b527b417d9c4f416fafa048/EIPS/eip-2767.md): Contract Ownership Governance
- [Democracy Earth is now a DAO explorer](https://democracy.earth/), starting with Moloch v1 and proof of personhood score
- [TornadoCash forming a Moloch DAO](https://medium.com/@Tornado_Fund/decentralizing-tornadocash-the-launch-of-tornado-fund-and-the-path-towards-tornadodao-a6d4ffc6c800) with OpenLaw
- [KyberDAO goes live July 7](https://blog.kyber.network/katalyst-and-kyberdao-go-live-on-07-07-2020-d67ac075d95a)

**Application layer**

- Synthetix [launches binary options](https://blog.synthetix.io/how-binary-options-work/)
- 0x’s [Matcha](https://matcha.xyz/blog/say-hello-to-matcha) dex aggregator is live with a focus on non-hardcore traders
- MCDex launches [10x ETH perpetual](https://medium.com/@montecarlodex/mcdex-officially-launches-its-perpetual-contracts-with-up-to-10x-leverage-e9464cfcbc60) with the funding rate coming from the automated market maker
- It’s now easier to host on [IPFS the latest Uniswap frontend](https://uniswap.org/blog/ipfs-uniswap-interface/)
- MakerDAO is exploring [Peg Stabilization Modules](https://forum.makerdao.com/t/peg-stabilization-modules-a-pre-mip-discussion/3045), ie stablecoin to stablecoin trading
- Augur v2 [launches July 28](https://www.augur.net/blog/v2-launch/)
- dxDao launches [Omen prediction markets](https://medium.com/@ingamar/omen-eth-has-officially-launched-67eb51c249c8) using Realit.IO and Kleros as oracles and available atomen.eth or omen.eth.link

**Tokens/Business/Regulation**

- [USDC hit 1 billion in circulation](https://etherscan.io/token/0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48) on Eth
- A new [Flippening tracker](https://www.blockchaincenter.net/flippening/)
- Common Stack’s [trusted seed token](https://medium.com/commonsstack/cstk-the-token-of-the-commons-stack-trusted-seed-931978625c61)

**General**

- Swarm released [Bee client v0.1](https://github.com/ethersphere/bee/releases/tag/v0.1.0) and announced a future token sale
- [Staking is now live](https://twitter.com/maticnetwork/status/1277515494141030401) on Matic Network
- [Skale sidechains](https://skale.network/blog/3-2-1-blast-off-skale-mainnet-is-live/) launches with POA and no transfers
- [Attacking less than 85 Lightning Network channels](https://medium.com/@jonahar/flood-loot-a-systemic-attack-on-the-lightning-network-5c3dac7bba24) will result in a successful attack
- [Harry Denley rescued a victim’s 5k](https://medium.com/mycrypto/intercepting-and-saving-5-000-worth-of-phished-crypto-9d2d6db6c527) from a fake TrustWallet app in the GooglePlay store by DOSing the Telegram API

* * *

## **Job Listings**

- [GridPlus is hiring](https://gridplus.io/careers) US remote firmware engineers.
- [Donut](https://www.donut.app/about) is looking for a CTO to bring DeFi to the masses. Interested?
- [0x is hiring](https://0x.org/about/jobs) full-stack, back-end, front-end engineers + 1 data scientist
- Trail of Bits is looking for masters of low-level security. [Apply here](https://jobs.lever.co/trailofbits/8b7f7fc1-efb0-4e89-b406-784c3a2d77e4).
- Celer Network: [Android developer](https://www.celer.network/career.html)
- Chainlink: [Senior Software Engineer](https://careers.smartcontract.com/o/senior-software-engineer-new-york) and [Lead Test Engineer](https://careers.smartcontract.com/o/lead-test-engineer-on-chainlink)

**Want your job listing here**? $250 per line (~75 character limit including spaces), payable in ETH/DAI/USDC to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

## **Housekeeping**

Follow me on Twitter [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the newsletter as it happens.

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive it weekly**

Permalink: [https://weekinethereumnews.com/week-in-ethereum-news-july-5-2020/](https://weekinethereumnews.com/week-in-ethereum-news-july-5-2020/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- July 6-Aug 6 - [HackFS](https://hackfs.com/) Filecoin/IPFS and Ethereum hackathon
- July 10 - next [core dev call](https://github.com/ethereum/pm/issues/192)
- **July 10 - [eth2 research team Reddit AMA](https://twitter.com/drakefjustin/status/1278038062405169154)**
- July 20 - [Fork the World](https://metagame.substack.com/p/fork-the-world-hackathon) MetaCartel hackathon
- **July 28 - [Augur v2 launch](https://www.augur.net/blog/v2-launch/)**
- July 30 - EEA’s [Ethereum in the Enterprise 2020](https://www.conference.entethalliance.org/) virtual conference
- Aug 2 - [ENS grace period](https://medium.com/the-ethereum-name-service/the-great-renewal-its-time-to-renew-your-eth-names-or-else-lose-them-afccea4852cb) begins to end
- Oct 2-Oct 30 - [EthOnline hackathon](https://www.ethonline.org/)

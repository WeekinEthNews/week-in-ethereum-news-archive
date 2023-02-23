---
title: "Week in Ethereum News <BR> May 3, 2021"
date: "2021-05-03"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest [core devs call](https://youtu.be/_QLDhNMwoe4?t=221). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1388185926149435399)
    - Decided: EIP3529 (getting rid of gas refunds) included in London fork, difficulty bomb postponed to q2 2022, including EIP3541 in London to be decided next call, also timing for London to be decided next call
- [EIP3074 community call](https://www.youtube.com/watch?v=pUJlZMXrVEI)
- Idea: [charge gas to access each individual contiguous 31-byte segment](https://notes.ethereum.org/@vbuterin/code_chunk_gas_cost) of code, to put a ceiling on witness size
- Updated [EVM384 Geth benchmarking](https://hackmd.io/Ou0SkcLPQNOx3qAgGnaZgQ)

**EIPs/Standards**

- [EIP3540](https://github.com/ethereum/EIPs/blob/fc03ae17e9f93d7aa372122892205839dcaa1e54/EIPS/eip-3540.md): Ethereum Object Format
- [EIP3541](https://github.com/ethereum/EIPs/blob/8aa8b36070c28808f32d1e6465e71e9d0f2b8d2f/EIPS/eip-3541.md): Reject new contracts starting with the 0xEF byte (a stepping stone to 3540)
- [EIP3534](https://github.com/whilei/EIPs/blob/b61b3563a154de1d6f568ab22dc611eb25172231/EIPS/eip-3534.md): Restricted Chain Context Type Transactions
- [ERC3525](https://github.com/ethereum/EIPs/blob/ce3d6bdc14d277c39ec5785a52701739068308f8/EIPS/eip-vnft.md): Versatile NFT
- [ERC3549](https://github.com/ethereum/EIPs/blob/8e3591e986e01490b61abb8205e03bd0e3bb8907/EIPS/eip-3549.md): Anti-sleepminting ERC721 Metadata sig

**Proof of stake consensus layer**

- First ephemeral [multi-client testnet to turn off PoW](https://twitter.com/protolambda/status/1388093072936951811) with 12 different client combinations; a surprising amount of consensus.
    - A longer lasting testnet coming in next week or so
- Client diversity matters: [switch to Lighthouse](https://lighthouse.sigmaprime.io/switch-to-lighthouse.html) (or another minority client) for your own good and the good of the network. They have a neat feature I didn’t know about: use Teku for redundancy even if Lighthouse node has a bug.
    - Reminder: we have four fantastic consensus clients: Lighthouse, Nimbus, Prysm, Teku
- Prysmatic [post-mortem on last week’s staking hiccups](https://medium.com/prysmatic-labs/eth2-mainnet-incident-retrospective-f0338814340c) coming from an invalid Eth deposit root hash in the cache initialization for deposits
- What would’ve happened [if the staking hiccups had occurred after](https://bisontrails.co/eth2/014/) we turn off PoW
- Barnabé Monnot: [graphical view of staking hiccup event](https://barnabe.substack.com/p/a-data-driven-view-of-the-beacon).
    - Chain never stopped finalizing, “strong evidence for the robustness of the protocol”
- A demo of [Teku’s sync](https://twitter.com/benjaminion_xyz/status/1388182493510131719) in a minute
- Latest [turning off PoW call](https://www.youtube.com/watch?v=KAm718N_bvA), notes from [Shane Lightowler](https://github.com/ethereum/pm/blob/3432ee86f8987b2c2139024eef07f4a9d4961901/Merge/Meeting%2003.md)
- [Add ability to change staking key](https://ethresear.ch/t/adding-pos-validator-key-changes/9264)
- Work in progress [design for stakers to withdraw](https://hackmd.io/@zilm/withdrawal-spec)
- There’s now [more than 4 million ETH](https://etherscan.io/address/0x00000000219ab540356cbb839cbe05303d7705fa) in the staking contract
- Vitalik on some [underappreciated PoS benefits](https://www.reddit.com/r/ethereum/comments/mxo151/some_lessappreciated_benefits_of_ethereums_pos/): regular blocks every 12 seconds, much better confidence after same amount of confirmations, better light clients, easier to detect attacks

**Layer2**

- Deversifi’s [layer2 ecosystem map](https://twitter.com/deversifi/status/1387379996713439237/photo/1)
- Truebit offchain computation verification [announces it is live](https://truebit.substack.com/p/truebit-early-access) on mainnet
- Vitalik sketches an [optimistic rollup using offchain computation verifier](https://ethresear.ch/t/evm-optimistic-rollup-using-truebit/9318)

* * *

### **This newsletter is made possible thanks to [NEAR](https://near.org/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2021/05/rainbow-bridge-1024x538.png)

[NEAR](https://near.org/) is rapidly scaling the Creator Economy and DeFi with a trustless, secure Rainbow Bridge to Ethereum. Check out [NEAR Protocol](https://docs.near.org/) and see why thousands of devs are taking advantage of NEAR's usability and developer experience. Top ecosystem projects like [Collab.Land](https://collab.land/) and [Mintbase.io](https://mintbase.io/) are already using NEAR to empower creators and communities with smooth user onboarding to crypto.

Sign up for a NEAR Wallet using a faucet hosted by [Paras](https://faucet.paras.id/), a trading card NFT marketplace, and try the [Rainbow Bridge](https://ethereum.bridgetonear.org/)!

Don’t forget to follow NEAR on [Twitter](https://twitter.com/NEARProtocol) and join us on [Discord](https://near.chat/).

* * *

**Stuff for developers**

- OpenZeppelin Contracts [v4.1](https://blog.openzeppelin.com/openzeppelin-contracts-4-1), cheaper UUPS proxies, flashmint functionality, multicall batch transactions, plus EIP2098 and SignatureChecker
- [OCaml-Solidity](https://github.com/OCamlPro/ocaml-solidity): Solidity parser and typechecker library
- [Circom & SnarkJS snark plugin](https://www.npmjs.com/package/hardhat-circom) for Hardhat
- ZoKrates [v0.7.1](https://github.com/Zokrates/ZoKrates/releases/tag/0.7.1), constant declaration, constant range checks, and now includes poseidon hash function
- Call state overrides in lates [web3.py v5.19 release](https://snakecharmers.ethereum.org/web3-py-patterns-eth_call-overrides/)
- [ENS integration best practices](https://medium.com/the-ethereum-name-service/ens-integration-best-practices-313d6fbd358)
- Remix IDE [v0.11.5](https://medium.com/remix-ide/remix-release-v0-11-5-a840d0444acb) adding Solidity’s new “custom errors” feature
- Is your node giving you [accurate gas prices from eth\_estimateGas](https://twitter.com/gregthegreek/status/1387936480375582724)?
- $100 in ETH [incentive for the first 5 CryptoZombies lessons](https://twitter.com/balajis/status/1387263302351216644)
- Eric Wall argues [Chainlink v2 is less secure than v1](https://ercwl.medium.com/whats-wrong-with-the-chainlink-2-0-whitepaper-for-simpletons-d50f27049464)

**Security**

- Samczsun finds a [tokenlon vulnerability](https://tokenlon.medium.com/tokenlon-4-0-fee-incident-disclosure-9ee8b5fad564)
- Two big BSC hacks:
    - [Uranium for $51m](https://twitter.com/FrankResearcher/status/1387347025742557186) in code that didn’t need to be changed
    - [Spartan for $31m](https://www.rekt.news/spartan-rekt/) because apparently they [didn’t understand what they forked](https://twitter.com/FrankResearcher/status/1388860919694782466)

**Ecosystem**

- Worried about PoW’s massive energy waste? [Ethereum proof of stake is green](https://our.status.im/ethereum-is-green/)
    - Miners should conservatively [plan for mining to end in 2021](https://twitter.com/trent_vanepps/status/1387837123756240898)
- Several [mining pools are mining gastokens to sell](https://compassmining.io/education/empty-blocks-gas-chi-tokens-ether-pools-mining/); they don’t have to pay miners transaction fees for gas tokens
- Gas fees in [20 gwei range](https://www.gasnow.org/) this weekend
- Metamask surpasses [5 million monthly active users](https://consensys.net/blog/metamask/metamask-surpasses-5-million-monthly-active-users/)

**Enterprise**

- [European Investment Bank issues 100m euro, 2 year bond](https://www.eib.org/en/press/all/2021-141-european-investment-bank-eib-issues-its-first-ever-digital-bond-on-a-public-blockchain) on mainnet Ethereum. This bond is the first “first multi‑dealer led, primary issuance of digitally native tokens.” EIB exec calls Ethereum “[revolutionary](https://finance.yahoo.com/news/european-debt-pioneer-trumpets-revolution-112630196.html).”
- Project (L)Ubin continues: [DBS, JPMorgan, and Temasek](https://www.jpmorgan.com/news/dbs-jpmorgan-and-temasek-to-establish-platform) working together on interbank transfers

**Application layer**

- LarvaLabs’ [Meebits](https://meebits.larvalabs.com/), 20000 generative 3d voxel characters
- [NFT perpetually programmable song](https://async.art/music/master/0xb6dae651468e9593e4581705a09c10a76ac1e0c8-1597/player) from RAC
- [Etherplay Konquest-style alpha](https://etherplay.medium.com/get-ready-for-conquest-eth-first-alpha-84f72efdd73d) on goerli testnet
- General Mills is [auctioning NFTs for Dunkaroos](https://www.marketingdive.com/news/general-mills-auctions-nfts-to-promote-return-of-chocolate-dunkaroos/599239/) re-release. Hasbro floats [Magic: the Gathering NFTs](https://www.polygon.com/22406490/magic-the-gathering-nft-tokens-hasbro-ceo-quarterly-earnings)
- USDC upgrades to [v2.1](https://www.centre.io/blog/centre-consortium-announces-release-of-usd-coin-version-2.1) to prevent users from sending to contract

**Regulation/business/tokens**

- JPMorgan note on why [ETH is outperforming BTC](https://twitter.com/santiagoroel/status/1387417522777956354)
- ETH is a [better treasury reserve asset](https://twitter.com/investindigital/status/1388164681228029952) than BTC, a summary of TwoPrime’s the [rise of institutional Ethereum investors](https://twoprime.io/the-rise-of-institutional-ethereum-investors/)
- Ethereum, the [Triple Halving](https://twitter.com/SquishChaos/status/1387074107217436675): flows based $ETH analysis
- Justin Drake calculates [peak ETH supply](https://twitter.com/drakefjustin/status/1386670011742306310)

**General**

- Gemini to launch [Mastercard credit card](https://www.mastercard.com/news/press/2021/april/gemini-partners-with-mastercard-to-launch-new-crypto-rewards-credit-card-this-summer/) with crypto cashback
- Pete Rizzo chronicles [Satoshi’s final days](https://bitcoinmagazine.com/technical/what-happened-when-bitcoin-creator-satoshi-nakamoto-disappeared)
- Facebook is working on a [STARK prover](https://github.com/novifinancial/winterfell)
- Brave browser over [30m MAUs and 10m DAUs](https://twitter.com/BrendanEich/status/1389256491991846915)

* * *

## **Job Listings**

- [Join Zerion as Product Manager](https://jobs.lever.co/zerion/02a3d561-3367-48c0-9e50-eef8db11d5dc?lever-origin=applied&lever-source%5B%5D=WeekInEthereum) and take DeFi to the next level
- Giveth is [hiring experienced Solidity Devs](https://cryptojobslist.com/jobs/lead-solidity-smart-contract-developer-at-giveth-remote) interested in #Defi4good
- Join our team to help [bring Ethereum into governments as a dApp developer](https://www.notion.so/symfoni/Symfoni-jobs-0c2bdc029d2a4cf7b91864a5e68ed00f)
- [Enzyme](https://enzyme.finance/) is hiring. [Solidity dev](https://www.notion.so/Senior-Smart-Contract-Developer-to-work-on-Enzyme-641aef0d89cc419cba792445354f835b), [data engineer](https://www.notion.so/Data-Engineer-a412646a06a046bfaac26085b4695857), [UX/UI designer](https://www.notion.so/UX-UI-Designer-e115c94e193b4e98b98283fa1bcaf3b8) & [growth eng](https://www.notion.so/Growth-Engineer-d682408e8500447888859f9d47bc4a79).
- Want to work on stateless/EVM? [EF JavaScript team is hiring several developers](https://twitter.com/EFJavaScript/status/1382292102348935168)
- BitGo's WBTC team is hiring [Blockchain Engineers](https://boards.greenhouse.io/bitgo/jobs/5191525002), [Sr. Blockchain Engineers](https://boards.greenhouse.io/bitgo/jobs/5089951002) and [Lead Blockchain Engineers](https://boards.greenhouse.io/bitgo/jobs/5197342002). (You can check out the rest of our jobs [here](https://boards.greenhouse.io/bitgo)!)

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-may-3-2021/](https://weekinethereumnews.com/week-in-ethereum-news-may-3-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **May 6 - OpenZeppelin’s [ECDSA/ERC712 sigs to build NFT Merkle Drop](https://twitter.com/OpenZeppelin/status/1388177065493426176) workshop**
- May 7 - [Building on Ethereum](https://twitter.com/dabit3/status/1386696929770283010) with Austin Griffith and Nader Dabit
- **May 7 - [EIP1559 social coordination](https://twitter.com/trent_vanepps/status/1388153403432480769) call**
- May 14 - papers due for [WoSCA 2021](https://trailofbits.github.io/WoSCA/)
- May 14 - Jun 2 - [0xHack](https://0xhack.dev/)
- **May 18-21 - [EY Global Blockchain Summit](https://pub.ey.com/public/2021/2101/2101-3679331/blockchain-summit-2021/index.html)**
- Jul 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

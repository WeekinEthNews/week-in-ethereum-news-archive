---
title: "Week in Ethereum News <BR> April 18, 2021"
date: "2021-04-19"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest [core devs call](https://youtu.be/-H8UpqarZ1Y?t=452). [Notes](https://twitter.com/TimBeiko/status/1383054611506864133) from Tim Beiko. Discussion of future avoidance of OpenEthereum’s bug, plus finalizing what goes into the London release.
- OpenEthereum had a bug a few hours into Berlin and thus it went down. Here’s the [detailed version of the bug](https://twitter.com/ralexstokes/status/1382750001026146304) involving access lists and an address reserved for the bls12-381 precompile which is planned but vacant
- OpenEthereum [v3.2.4](https://github.com/openethereum/openethereum/releases/tag/v3.2.4) is the latest version with the bugfix
- Why [did we need to increase gas costs for state access](https://www.reddit.com/r/ethereum/comments/mrl5wg/a_quick_explanation_of_what_the_point_of_the_eip/) in the Berlin fork?
- [Turbogeth’s mining functionality](https://twitter.com/realLedgerwatch/status/1382674673239011328) will have a devnet launch with a 1 billion gas limit (!)

**EIPs/Standards**

- [EIP3508](https://github.com/ethereum/EIPs/blob/64ff371102eadac8980f63cd4a1e3dc155de359d/EIPS/eip-3508.md): Transaction Data Opcodes

**Proof of stake consensus layer**

- Latest [turning off PoW call](https://www.youtube.com/watch?v=ODcNpWiLASk). Protolambda’s [notes](https://notes.ethereum.org/@protolambda/merge_impl_call_2): going through the spec
- SigmaPrime’s [Lighthouse client update](https://lighthouse.sigmaprime.io/update-35.html): getting ready for the Altair network upgrade, wrestling with memory allocators
- A twitter thread about [turning off Pow (“the Merge”) explainer](https://twitter.com/yulesa/status/1382429264683925504)

**Layer2**

- MatterLabs is planning an [offchain data availability](https://medium.com/matter-labs/zkporter-a-breakthrough-in-l2-scaling-ed5e48842fbf) security model as well as its zksync zk-rollup

* * *

### **This newsletter is made possible thanks to [Kwenta](https://kwenta.io/)!**

![](https://weekinethereumnews.com/wp-content/uploads/2021/04/IMG_20210418_190328_618-1024x512.jpg)

[Kwenta](https://kwenta.io/) offers derivatives trading on a vast range of assets with infinite liquidity and zero slippage, and is powered by the [Synthetix](https://synthetix.io/) protocol.

Trade synthetic cryptocurrencies, forex, commodities, and equities both long and short, without the limits or compromises of a centralised exchange. Try [Kwenta](https://kwenta.io/) today!

* * *

**Stuff for developers**

- Hardhat [v2.2](https://github.com/nomiclabs/hardhat/releases/tag/hardhat-core-v2.2.0), ready for Berlin
- [Migrating files to workspaces](https://medium.com/remix-ide/migrating-files-to-workspaces-8e34737c751c) in Remix, plus [Remix now available in VSCode](https://medium.com/remix-ide/remix-plugin-engine-plugs-ahead-6b3d89872926)
- Vyper [v0.2.12](https://vyper.readthedocs.io/en/latest/release-notes.html#v0-2-12) is out, also updated for Berlin, plus a medium and low security vulnerability report
- Blocknative’s [Simulation Platform](https://www.blocknative.com/blog/simulation-platform): simulate via API function calls & net balance changes for what’s in the transaction pool
- [EVM opcode list](https://github.com/wolflo/evm-opcodes) updated for Berlin

**Ecosystem**

- Phil Daian: [MEV wat do](https://pdaian.com/blog/mev-wat-do/)? Argues that MEV must be extracted for security and what you should do about it
- Ed Felten’s [five theses for transaction ordering](https://medium.com/offchainlabs/five-theses-about-transaction-ordering-mev-and-front-running-5ebf52bc0cbe): resistance to frontrunning is good, and we’ll be working at it a long time, so we should be careful not to make it worse
- [Sandwiching an uncled sandwicher](https://twitter.com/bertcmiller/status/1382673604085698567)
- Flashbots monthly update: [93 searchers landed ~5500 bundles](https://medium.com/flashbots/flashbots-transparency-report-march-2021-d3930b4b98a9); they’re probably moving to mev-sgx
- [Flashbots fair market principles](https://hackmd.io/@flashbots/fair-market-principles) proposal
- The history of [Synthetix’s fight against frontrunners](https://blog.synthetix.io/frontrunning-synthetix-a-history/): impending implementations are TWAP oracles and lower latency on Optimism

**Enterprise**

- JP Morgan testing a [Quorum-based product with Taiwanese banks](https://www.coindesk.com/jpmorgan-testing-blockchain-solution-to-improve-transfers-with-taiwanese-banks)
- Videos from JP Morgan’s [demo of space-based machine to machine payments](https://www.jpmorgan.com/onyx/payments-in-space.htm?source=wp_os_li_wpiTL0421) using satellites

**Application layer**

- [Gelato v2](https://medium.com/gelato-network/introducing-gelato-v2-the-most-reliable-way-to-automate-your-ethereum-smart-contracts-73cd0010599e) is live: bots that execute automatically. Now doesn’t need proxy contracts, and data generated offchain
- [Whether Rai is a stable asset](https://ameensol.medium.com/rai-narrative-strategy-guide-901acdd6bfc4) depends on narrative and market participants
- Edward [Snowden auctions NFT for ~2200 ETH (~$5.5m)](https://twitter.com/Snowden/status/1383155552793026560) to benefit Freedom of Press Foundation, purchased by PleasrDAO
- [DisasterGirl meme](https://foundation.app/DisasterGirl/disaster-girl-25046) goes for 180 ETH (~$400k)
- [Etherfreakers update](https://observablehq.com/@jflatow/etherfreakers): NFT characters with gameplay (rules in post), some players already deployed a DAO to protect their characters, and 0age has entered the chat
- [Maker votes against writing a letter asking a16z](https://vote.makerdao.com/polling/QmPWEpBB?network=mainnet#poll-detail) to participate in Maker governance

**Regulation/business/tokens**

- SEC Commissioner Hester Peirce’s [Token Safe Harbor v2](https://www.sec.gov/news/public-statement/peirce-statement-token-safe-harbor-proposal-2.0) proposal
- The [perils of progressive decentralization](https://thewayofthedao.substack.com/p/daos-and-the-pitfalls-of-progressive): an argument for community first, product-market fit second
- ConsenSys announces [$65m fundraising round from JPMorgan, UBS, Mastercard](https://www.mastercard.com/news/press/2021/april/partnership-with-consensys-supports-the-future-of-multi-blockchain-commerce/) and Filecoin’s ProtocolLabs
- Andre Cronje: [scams pumping during bull markets is demotivating for builders](https://andrecronje.medium.com/bull-market-bear-development-b6ede96d4c82)
- Justin Drake calculates that 1559 and turning off PoW will produce [more buy pressure per year](https://twitter.com/drakefjustin/status/1383325832467214337) than the eth2 deposit contract and Grayscale trust combined
- Arthur Hayes says [price/revenue models have ETH massively undervalued](https://cryptohayes.medium.com/yes-i-read-the-whitepaper-59cfa2ea9c2c)

**General**

- Is [Google FLoC’ing you](https://adalytics.io/blog/google-chrome-floc)? By default Chrome now gives your browsing history to advertisers and websites
- How to [beat a sweeper and recover your assets](https://blog.mycrypto.com/how-to-beat-an-ethereum-based-sweeper-and-recover-your-assets/) from a compromised private key
- r/WallStreetBets now [allowing ETH and memecoin (BTC/DOGE) talk](https://www.reddit.com/r/wallstreetbets/comments/mqveqc/on_crypto/)

* * *

## **Job Listings**

- bZx is hiring a Lead Developer. 400k/year total comp. Apply [here](https://angel.co/company/bzx-1/jobs/1181110-senior-full-stack-developer).
- [Enzyme](https://enzyme.finance/) is hiring. [Solidity dev](https://www.notion.so/Senior-Smart-Contract-Developer-to-work-on-Enzyme-641aef0d89cc419cba792445354f835b), [data engineer](https://www.notion.so/Data-Engineer-a412646a06a046bfaac26085b4695857), [UX/UI designer](https://www.notion.so/UX-UI-Designer-e115c94e193b4e98b98283fa1bcaf3b8) & [growth eng](https://www.notion.so/Growth-Engineer-d682408e8500447888859f9d47bc4a79).
- [Element Finance](https://element.fi/), launching very soon, is hiring a [Solidity engineer](https://docs.google.com/document/d/1D0wxlgnRsd6rQh2s3rC1Lq1fADkcHBtfKAVhepx6wss/edit?usp=sharing)
- Nomic Labs (Hardhat/Buidler) is hiring a [senior dev and an engineering manager](https://www.notion.so/Nomic-Labs-jobs-991b37c547554f75b89a95f437fd5056)
- Want to work on stateless/EVM? [EF JavaScript team is hiring several developers](https://twitter.com/EFJavaScript/status/1382292102348935168)

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-april-18-2021-thanks-to-synthetixs-kwenta-for-making-this-issue-possible/](https://weekinethereumnews.com/week-in-ethereum-news-april-18-2021-thanks-to-synthetixs-kwenta-for-making-this-issue-possible/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- April 20 - deadline for [beacon chain security and testing RFP](https://notes.ethereum.org/@lsankar/security-rfp)
- April 20 - deadline to [comment on FATF anti-DeFi](http://www.fatf-gafi.org/publications/fatfrecommendations/documents/public-consultation-guidance-vasp.html) regulatory proposal
- **April 20 - [OG NFT](https://ognft.club/) conference**
- April 22 - [Ethereum in the Enterprise 2021](https://www.conference2021.entethalliance.org/)
- **April 22 - OpenZeppelin [managing upgrades](https://twitter.com/OpenZeppelin/status/1383178388425293827) workshop**
- **April 23 - submissions due for [network crawler RFP](https://notes.ethereum.org/@timbeiko/crawler-rfp)**
- May 14 - papers due for [WoSCA 2021](https://trailofbits.github.io/WoSCA/)
- May 14 - Jun 2 - [0xHack](https://0xhack.dev/)
- Jul 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

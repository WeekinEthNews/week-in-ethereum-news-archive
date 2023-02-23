---
title: "Week in Ethereum News <BR> June 12, 2021"
date: "2021-06-12"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest [core devs call](https://www.youtube.com/watch?v=XYhN26UrJ5o&t=268s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1403390897614561282): 
    - London mainnet upgrade block to be chosen after Ropsten testnet upgrade, clients to be updated with chosen block
    - Working through EIP1559 JSON RPC standards
    - EIP3607 prevents transactions from senders with deployed code, clarifies how transactions are validated,  doesn’t require hard fork
    - Update on EIP3074 AUTH and AUTHCALL opcodes audit and [impact study](https://twitter.com/dedaub/status/1403083441772638211)
- Tim Beiko’s overview of [EIPs included in London](https://medium.com/ethereum-cat-herders/london-upgrade-overview-8eccb0041b41)
- [Erigon 2021.06.03-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2021.06.03): nodes using the old [LMDB](https://twitter.com/realLedgerwatch/status/1402967620639395840) database will need to resync after next release
- Vitalik’s proposal to use [a single layer Verkle tree](https://www.reddit.com/r/ethereum/comments/nve036/ethmag_proposed_scheme_for_encoding_ethereum/) rather than the current two-layer trie inside a trie structure when moving Ethereum state to a Verkle tree
- Proposal to use [precompiles to abstract verifying history and shard proofs](https://ethresear.ch/t/future-proof-shard-and-history-access-precompiles/9781) to allow formats to be changed in future
- Proposal for [account abstraction](https://notes.ethereum.org/@vbuterin/alt_abstraction) via alternative mempool such as Flashbots
- [Piper’s proposal to replace the inscrutable Yellow Paper](https://ethereum-magicians.org/t/replace-the-yellow-paper-with-executable-markdown-specification/6430) with an executable markdown spec as used in the Beacon chain specs

**EIPs/Standards**

- [EIP3607](https://eips.ethereum.org/EIPS/eip-3607): Reject transactions from senders with deployed code
- [Proto-EIP](https://notes.ethereum.org/4BPLDyGnQ0WY12kVbOuvxw): Witness gas cost reform for Verkle trees
- [Proto-EIP](https://notes.ethereum.org/@vbuterin/state_expiry_eip): State expiry

**Proof of stake consensus layer**

- [Exploring MEV in PoS](https://hackmd.io/@flashbots/mev-in-eth2): MEV will still exist and increase validator rewards, may amplify inequalities between validators, exchanges may possibly control largest amount of validator slots
- [Lighthouse v1.4.0](https://github.com/sigp/lighthouse/releases/tag/v1.4.0): 1/3rd the RAM and 1/5th the execution layer calls
- [Teku v21.6.0](https://github.com/ConsenSys/teku/releases/tag/21.6.0): report current peer count API, eth1 requests metric
- [Beaconcha.in mobile app v2.0](https://twitter.com/etherchain_org/status/1402909186913153024): Monitor staking device performance (Lighthouse & Prysm - alpha)

**Layer2**

- [Raiden Bespin](https://medium.com/raiden-network/bespin-mainnet-release-announcement-87f5d5ede018): stability release, users will need to close and settle Alderaan channels
- [ArbRinkeby](https://twitter.com/arbitrum/status/1403102638699433984): stable Arbitrum testnet
- [Arbitrum in 10 minutes](https://tracer.finance/radar/arbitrum-in-under-10/) explainer 

* * *

### **This newsletter is made possible thanks to Synthetix’s [Kwenta](https://kwenta.io/)!**

![Kwenta](https://weekinethereumnews.com/wp-content/uploads/2021/04/IMG_20210418_190328_618-1024x512.jpg)

[Kwenta](https://kwenta.io/) enables traders to access real-world and derivative assets on-chain with zero slippage using the power of the [Synthetix](https://synthetix.io/) protocol.

Trade popular synthetic cryptocurrencies, commodities, forex, and equities, such as TSLA, COIN, and FAANG stocks, without the limits or compromises of a centralized exchange.

Try [Kwenta](https://kwenta.io/) today!

* * *

**Stuff for developers**

- [Solidity v0.8.5](https://blog.soliditylang.org/2021/06/10/solidity-0.8.5-release-announcement/): bytes to bytesNN conversion and verbatim builtin function to inject arbitrary bytecode in Yul for new opcodes or projects like Optimism
- [bytes.concat(bytes(s1), bytes(s2))](https://docs.soliditylang.org/en/v0.8.5/types.html#bytes-and-string-as-arrays): concatenate strings since Solidity v0.8.4
- New [Fe website](https://fe.ethereum.org/): download binaries, read docs and examples
- [Remix v0.12.0](https://medium.com/remix-ide/remix-ide-0-12-0-released-7301b3b3f35d): Hardhat integration via Remixd, DGIT - Git in the browser, easy GIST creation and custom error reporting
- [VS Code Solidity extension v0.12](https://twitter.com/juanfranblanco/status/1402176611051524096)
- [Instadapp Terminal](https://terminal.instadapp.io/): browser based interaction via SDK and web3 wallet
- [Bondzier](https://github.com/bluedotdao/bondzier): experimental bezier bonding curves for ERC1155 tokens

**Security**

- [Path-based IPFS gateways](https://consensys.net/diligence/blog/2021/06/ipfs-gateway-security) disable same-origin policy
- DeFiSafety calls for projects to be [transparent on admin functions including upgrades](https://rex2.medium.com/upgradeability-in-defi-7b6828e9e6df)
- [Reproduce Fei exploit](https://medium.com/immunefi/a-guide-to-reproducing-ethereum-exploits-fei-protocol-224b30b517d6): setup environment, test exploit and fix

**Ecosystem**

- [Sign-In with Ethereum](https://twitter.com/BrantlyMillegan/status/1402388133086367751) is the future of login for the web
- Josh Stark: alternative history if [Pong was invented before computers](https://stark.mirror.xyz/8VPxOqJu1UZDDBTn4sxctshFdaZPTFuFRGoat2UJOw8)
- Anthony Sassano: [Ethereum is freedom](https://thedailygwei.substack.com/p/ethereum-is-freedom-the-daily-gwei)
- [r/ethereum crosses 1 million](https://twitter.com/0xMidnight/status/1402476244055302150) subscribers 

**Enterprise**

- [Tracking cattle](https://brownfieldagnews.com/news/nebraska-ranch-first-to-use-new-cattle-supply-chain-tracking-technology/) in Nebraska, USA

**Application layer**

- [Curve v2](https://curve.substack.com/p/june-9-2021-curve-v2-live): non-pegged volatile asset pool which uses an internal price oracle that adjusts when the loss becomes smaller than the system’s profit, initially USDT+wBTC+WETH
- [Livepeer processes 1 million minutes of video](https://medium.com/livepeer-blog/livepeer-processes-1-million-minutes-of-video-in-a-single-week-c320186256b3) in a single week 
- [Visualisation of lending protocols volumes](https://twitter.com/tokenterminal/status/1401901076903776260) over the last 12 months
- Sotheby’s auctions masked alien [CryptoPunk for $11.8m](https://twitter.com/Sothebys/status/1402996062474760193)
- [Doge meme](https://very.auction/doge/doge) sold for 1,696.9 ETH to @pleasrdao

**Regulation/business/tokens**

- [US Commodity Futures Trading Commissioner speech](https://www.cftc.gov/PressRoom/SpeechesTestimony/opaberkovitz7): can’t see how DeFi markets for derivative instruments are legal and untenable to allow them to compete with regulated derivatives market
- World Economic Forum: [DeFi Policy-Maker Toolkit](http://www3.weforum.org/docs/WEF_DeFi_Policy_Maker_Toolkit_2021.pdf)
- Trent McConaghy: [using ERC721 for base IP & ERC20 for IP sub-licenses](https://blog.oceanprotocol.com/nfts-ip-3-combining-erc721-erc20-b69ea659115e)

**General**

- [Bitcoin becomes legal tender](https://twitter.com/nayibbukele/status/1402446890466217985) in El Salvador
- [Chain-specific addresses](https://ethereum-magicians.org/t/chain-specific-addresses/6449) discussion
- [FundOSS](https://fundoss.org): Gitcoin Grants for open source

* * *

## **Job Listings**

- [Chorus One](https://chorus.one/careers) has open engineering & business positions
- Kwenta open position: [UI/UX Designer](https://blog.kwenta.io/kwenta-open-position-ui-ux-designer/)
- Sourcify looking for an [experienced TypeScript developer](https://twitter.com/SourcifyEth/status/1401917871710736385)
- Nethermind [internship program](https://www.notion.so/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)
- [Argent is hiring](https://apply.workable.com/argenthq/) Layer 2 Solidity Engineers, JS Full Stack, iOS & Android
- Quant (DeFi Options): [Solidity Eng](https://jobs.lever.co/QuantLabs/e5178731-3101-477b-b1b0-73b455f149fa?lever-origin=applied&lever-source%5B%5D=week%20in%20ethereum), [Designer](https://jobs.lever.co/QuantLabs/e9b98ca2-c37c-41ff-938c-93f8a6a4c5cc?lever-origin=applied&lever-source%5B%5D=week%20in%20ethereum), [Marketing Lead](https://jobs.lever.co/QuantLabs/9730189f-65ec-4f91-86db-b92a5c5be29d?lever-origin=applied&lever-source%5B%5D=week%20in%20ethereum), [DevOps](https://jobs.lever.co/QuantLabs/ef7fd355-cc6b-4921-b2f6-1ed6664d86e0?lever-origin=applied&lever-source%5B%5D=week%20in%20ethereum)
- [Prysmatic Labs](https://prysmaticlabs.com/careers) are hiring: Frontend, Go Security, Q/A

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please post your news to an Ethereum subreddit; emails/DMs are not part of our workflow.

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-june-12-2021/](https://weekinethereumnews.com/week-in-ethereum-news-june-12-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- June 16 - July 1 - [Gitcoin Grants Round 10](https://gitcoin.co/grants/explorer/)
- June 16 - July 7 - [Gitcoin Grants Round 10 Hackathon](https://gitcoin.co/hackathon/gr10/onboard)
- June 18 – July 9 – [ETHGlobal – Hack Money 2021](https://hackmoney.ethglobal.co/)
- June 23 - [Ethereum Foundation Research team AMA](https://twitter.com/drakefjustin/status/1398375498342977544)
- June 25-27 – [Edcon](https://www.edcon.io/) (Shenzhen/online)
- July 10 - Road to Devcon Quest: [Devcon Trivia Game](https://ethstaker.cc/road-to-devcon/)
- July 28 – [tentative date for London hard fork](https://docs.google.com/spreadsheets/d/1Y3yyTqeqRO1O2UFVkNkHK_V5oRulZd6y-JJbSnKYrb4) (Ropsten June 24, Goerli June 30, Rinkeby July 7)
- July 20-22 – [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

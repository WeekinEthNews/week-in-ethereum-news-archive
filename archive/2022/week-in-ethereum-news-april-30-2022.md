---
title: "Week in Ethereum News <br> April 30, 2022"
date: "2022-04-30"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest core devs [call video](https://www.youtube.com/watch?v=SWWoniO6rZc&t=63s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1520106955003424768) & [Christine Kim:](https://twitter.com/christine_dkim/status/1520087529139019779)
    - Focus on 2 more mainnet shadow forks, clients passing hive tests & fixing outstanding bugs
    - Difficulty bomb not delayed, review in two weeks
    - [Testnets post-merge](https://ethereum-magicians.org/t/og-council-post-merge-testnets/9034) are Goerli & Sepolia, plan to deprecate Rinkeby & Ropsten but other orgs may want to maintain
    - Discussion on RPC safe/unsafe/latest labeling
    - MEV boost: validators/proposers to set gas limit rather than builders
- Erigon [v2022.04.04-alpha](https://github.com/ledgerwatch/erigon/releases/tag/v2022.04.04): workaround to improve snapshot download speed via BitTorrent 
- Rough sketch of [Verkle tree migration](https://notes.ethereum.org/@XwIwCeCIQMeAl00PUAbEDw/verkle-migration-sketch)
- [NiceNode](https://mirror.xyz/johnsgresham.eth/BqQ92jtwu3hl6Ri2-giRLd0hequOt8Ya6ULAyCR-3ls): alpha interface to run a Geth node on Linux, Mac or Windows

**Proof of Stake consensus layer**

- Prysm [v2.1.0](https://github.com/prysmaticlabs/prysm/releases/tag/v2.1.0): support for the Merge, Web3Signer, experimental weak subjectivity sync and vectorized sha256 optimizations
- [12 million ETH deposited](https://twitter.com/ultrasoundmoney/status/1519640238381060097), 10% of supply
- Proposal for [withdrawal credentials exits using a generalized message bus](https://ethresear.ch/t/withdrawal-credentials-exits-based-on-a-generalized-message-bus/12516)

**PoW switch off (the merge)**

- [mainnet-shadow-fork-2](https://twitter.com/parithosh_j/status/1517816757884538881) successful with every single client combination, mild deposit processing issues (now patched) in two consensus clients
- mainnet-shadow-fork-3 [merge planned for May 5](https://twitter.com/evan_van_ness/status/1520214112264990725)

**EIPs/Standards**

- [EIP5058](https://github.com/ethereum/EIPs/pull/5058/files): Lockable ERC721
- [EIP5027](https://github.com/ethereum/EIPs/pull/5027/files): Unlimit contract code size

**Layer2**

- [Optimism Collective](https://optimism.mirror.xyz/gQWKlrDqHzdKPsB1iUnI-cVN3v0NvsWnazK7ajlt1fI): $OP governance token with first airdrop in Q2.  Bicameral governance for the network and public goods funding
- [Celer inter-chain messaging framework](https://blog.celer.network/2022/04/25/celer-im-launches-on-mainnet-a-new-era-for-inter-chain-dapps-begins/) live on mainnet 
- [Taiko](https://taikochain.github.io/l2design/): early draft of decentralized zk-rollup design
- [KZG commitments explainer](https://twitter.com/bkiepuszewski/status/1518163771788824576) (danksharding commitment scheme), more efficient than Merkle trees but requires trusted setup

* * *

### **This newsletter is made possible thanks to** [**SpeedRunEthereum**](https://speedrunethereum.com/)**!**

![SpeedRunEthereum](https://weekinethereumnews.com/wp-content/uploads/2022/04/Screenshot-from-2022-04-01-15-39-52.png)

[](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F1d7f63ca-4af0-4c6e-be64-fbdad99a56e0_769x208.png)

Are you a web2 dev who wants to get into web3?  

The best way to go from _zero_ to **hero** is [SpeedRunEthereum.com](https://speedrunethereum.com/).

Learn how to build on Ethereum; the superpowers and the gotchas.

Then [speed run Ethereum](https://speedrunethereum.com/) by testing your skills in a [series of challenges](https://speedrunethereum.com/challenge/simple-nft-example) and [join web3](https://twitter.com/austingriffith/status/1493688828661432325).

* * *

**Stuff for developers**

- OpenZeppelin Contracts [v4.6.0](https://twitter.com/OpenZeppelin/status/1519757750569418755): cross chain abstraction to receive messages, Governor parameterized voting, reinitializer modifier for upgrades and governance contracts security improvements
- Ganache [v7.1.0](https://github.com/trufflesuite/ganache/releases/tag/v7.1.0): override address state with eth\_call
- [ERC4626Votes](https://github.com/devanonon/ERC4626Votes#readme): extension for governance voting based on underlying asset
- [Fuzzing for memory bugs](https://ventral.digital/posts/2022/4/28/fuzzing-for-memory-bugs-in-solidity) in Solidity
- wagmi [v0.3.0](https://twitter.com/awkweb/status/1518607778209751041) (React hooks): caching, React 18 support and vanilla JS client
- [EIP712 Codegen](https://github.com/danfinlay/eip712-codegen#readme): generate Solidity for EIP712 decoding
- [IntelliJ](https://blog.web3labs.com/web3development/solidity-debugging-intellij) Solidity debugger plugin
- [MetaMask Snaps tutorial](https://github.com/Montoya/address-book-snap-tutorial#readme) to manage state in a Snap and add an API
- [dEth Tools](https://tools.deth.net/): online unit conversion, decoders and encoders 
- [Dune](https://dune.com/blog/flashbots-data) adds Flashbots data; query arbitrages, liquidations & sandwiches
- 0xPARC: [ZK Machine Learning](https://0xparc.org/blog/zk-mnist) tutorial and demo
- [GitHub Copilot suggested a private key](https://twitter.com/0xmuse/status/1519324793723568128), configure copilot so your key isn’t suggested

**Security**

- Akutar NFTs [$34 million locked in contract](https://twitter.com/0xInuarashi/status/1517674505975394304), team funds can’t be withdrawn due to faulty logic & dutch auction refunds initially blocked by a contract bid 
- Rari’s Fuse pool #45 [Uniswap v3 oracle manipulation vulnerability](https://medium.com/@hacxyk/we-rescued-4m-from-rari-capital-but-was-it-worth-it-39366d4d1812) due to low liquidity, $4 million was at risk 
- Review of [EIP4337 account abstraction](https://blog.openzeppelin.com/eth-foundation-account-abstraction-audit/) spec & reference implementation, one critical & several high-severity issues discovered

**Ecosystem**

- ETHAmsterdam [finalists](https://twitter.com/ETHGlobal/status/1518234859323408384)
- Ethereum.org [Q2 website roadmap](https://github.com/ethereum/ethereum-org-website/issues/6161)
- 0xPARC: [technical work required to build zk-identity](https://0xparc.org/blog/zk-id-2)
- Proposal for [simplified version of MACI](https://ethresear.ch/t/saci-simplified-anti-coliusion-infrastructure/12494) designed for voting

**Application layer**

- [ENS daily fees](https://twitter.com/MrWhiplash_eth/status/1519214063087194112) surpassed alt-layer 1s, mostly due to purchases of [four digit names](https://twitter.com/0xQuit/status/1519385101192237058) 
- [Ex0t1c Markets](https://medium.com/@exoticmarkets.xyz/exotic-markets-create-the-markets-you-want-to-participate-in-6aa7e9e7bba2) (on-chain positional markets) live on Optimism
- [DeFi Saver](https://blog.defisaver.com/automated-strategies-for-liquity-stop-loss-is-now-available/) stop loss options for Liquidity
- [Backed](https://twitter.com/backed_xyz/status/1517883906678312960): NFT-backed loans
- Bored Apes Instagram [hacked](https://twitter.com/zachxbt/status/1518609171796611072), NFTs stolen using phishing airdrop site
- [ENS expired names](https://twitter.com/nicksdjohnson/status/1519979007152095232) now use exponential curve for premium pricing
- Celer’s [layer2.finance](https://blog.celer.network/2022/04/27/celers-layer2-finance-launches-in-zk-proofs-mode-built-with-starkex-from-starkware/) (batched ETH/USDC/USDT deposits into Compound) launches with zk-proofs 
- Maker [proposal for Basepool Curve pool](https://twitter.com/MonetSupply/status/1520094314789056514) (DAI, USDC, USDP & GUSD)

* * *

### **Job Listings**

- Status Waku is hiring: [TypeScript Protocol/Software Engineer & DevRel](https://jobs.status.im/?gh_jid=4143735&gh_src=55c532491us)
- Ethereum Foundation need a [People Operations Lead](https://jobs.lever.co/ethereumfoundation/8046bbe5-6343-4ecf-8296-37dc2a5bf915?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Status are hiring [engineers who focus on incentive design](https://jobs.status.im/?gh_jid=3706505)
- Vac @ status are looking for [protocol engineers](https://jobs.status.im/?gh_jid=3693623) 
- Trail of Bits [Security Apprenticeship](https://jobs.lever.co/trailofbits/b2d6ce87-6b01-462f-965a-597a273ce26f) (3 months)
- OpenZeppelin are hiring a [Director of Development - Contracts](https://openzeppelin.com/jobs/opening/?gh_jid=5078928003)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- [Internship program](https://nethermind.notion.site/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1) at Nethermind (1-3 month) 
- EF’s Privacy & Scaling Explorations team: [Web3 Engineer](https://jobs.lever.co/ethereumfoundation/ece6534a-b946-4996-b7e7-713bd1ec0353?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- EF Ecosystem Support team: [Communications](https://jobs.lever.co/ethereumfoundation/4b0c3305-cf03-4e33-9bfb-63e4ec6f3a68?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum), [Analyst](https://jobs.lever.co/ethereumfoundation/64361391-9a74-49ed-b37c-8ff35931430e?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) & [Admin Assistant](https://jobs.lever.co/ethereumfoundation/5684f7ea-c3ad-4703-b86c-462964f49392?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Ethereum Q1 financial results](https://newsletter.banklesshq.com/p/state-of-ethereum-q1-2022) by Bankless
- Richard Chen’s [counterintuitive lessons](https://showerthoughts.substack.com/p/three-counterintuitive-lessons-from) from a crypto fund
- Balaji: [case for a Twitter airdrop](https://balajis.com/elondrop/) and tokenization of Twitter handles

**General**

- Zcash ceremony [sixth participant was Edward Snowden](https://www.youtube.com/watch?v=8qSA29vWWds&t=360s) \[video\] 
- Cloudflare says largest https [DDoS attack](https://blog.cloudflare.com/15m-rps-ddos-attack/) ever targeted a crypto site
- [A6 claims ability to track ~3 billion devices](https://theintercept.com/2022/04/22/anomaly-six-phone-tracking-zignal-surveillance-cia-nsa/) in real time using GPS location data leaking from apps

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-april-30-2022](https://weekinethereumnews.com/week-in-ethereum-news-april-30-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in_ **_bold_**_)_**:**

- May 1 – application deadline for [yAcademy’s auditor fellowship](https://yacademy.dev/fellowship-program/)
- May 3-5 – [Spaghett ETH](https://spaghett-eth.com/) (Milan)
- May 6-27 – ETHGlobal [Hack Money](https://defi.ethglobal.com/)
- May 8 – deadline for [EF academic grants round](https://esp.ethereum.foundation/academic-grants)
- May 17-20 – [EY Global blockchain summit](https://pub.ey.com/public/2021/2112/2112-3933703/blockchain-summit-2022/index.html)
- May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline
- Jun 10 – [Austin DeFi](https://2022.austindefi.org/) summit
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETH NYC](https://nyc.ethglobal.co/)
- **Jul 6-8 –** [**ETHBarcelona**](https://twitter.com/eth_barcelona/status/1516773782538448896)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 5-7 – [ETH Seoul](https://2022.ethseoul.org/)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 28 – [DeFi San Francisco](https://2022.defi-sf.com/) summit
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev) (hackathon & conference)
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** [_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive it weekly_**

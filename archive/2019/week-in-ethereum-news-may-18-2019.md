---
title: "May 18, 2019"
date: "2019-05-19"
---

## **Ethereum News and Links**

**Layer 1**

- Using [Eth2 as an Eth1 finality gadget](https://medium.com/@ralexstokes/the-finality-gadget-2bf608529e50)
- [Everything you need to know about Eth2 through phase 2](https://medium.com/@william.j.villanueva/a-journey-through-phase-2-of-ethereum-2-0-c7a2397a36cb)
- My phase 0 roadmap summary: individual clients already have testnets to varying degrees. Spec freeze end of June, networking this summer, longstanding cross-client testnet early Q4, auditing/testing, go live around end of q4 or q1
- [Exploration of discouragement attacks](http://hackingresear.ch/discouragement-attacks/)

**Layer 2**

- Matter doing over “[100 TPS of ZK transactions on ETH mainnet](https://twitter.com/the_matter_labs/status/1129439834819440641)” but couldn’t test higher because they crashed Digital Ocean
- [Separating the role of signatures in transaction validity vs slashing](https://ethresear.ch/t/separating-the-role-of-signatures-in-transaction-validity-vs-slashing/5453)
- [Mainnet sneak peak of Celer Network at EthNY](https://medium.com/celer-network/celer-ethny-2d8faa48d669)
- [Decentraland adopts Matic](https://decentraland.org/blog/technology/decentralands-path-toward-scaling-transactions) for fast and cheap layer2 sales of Estates
- Raiden [light client SDK and app](https://medium.com/raiden-network/public-project-launch-raiden-light-client-sdk-and-dapp-140a546c63a0), live on Rinkeby

**Client releases**

- [Parity v2.5.1-beta](https://github.com/paritytech/parity-ethereum/releases/tag/v2.5.1) or v[2.4.6-stable](https://github.com/paritytech/parity-ethereum/releases/tag/v2.4.6)

**Stuff for developers**

- [Solidity Hot Reloading using Zepkit](https://blog.zeppelinos.org/solidity-hot-reloading-using-zepkit/)
- [Pocketh](https://forum.zeppelin.solutions/t/new-pocket-knife-tool-for-developers-pocketh/655): a “pocket knife for auditing smart contracts” from Zeppelin
- Skale explainer on using their [sidechain storage as an IPFS alternative](https://skalelabs.com/blog/skale_decentralized_storage/)
- An [sbt-ethereum tutorial](https://medium.com/quiknode/creating-ethereum-smart-contracts-via-command-line-e817aa4ef8a)
- [Sandcastle](https://twitter.com/shahankhatch/status/1129427879262138369), an Eth SQL language pre-alpha available in Remix.
- Slither [v0.6.4](https://github.com/crytic/slither/releases/tag/0.6.4)
- Drizzle [v1.3.0](https://github.com/trufflesuite/drizzle-react/releases/tag/1.3.0)
- [Build a simple insurance Etherisc product](https://blog.etherisc.com/gif-tutorial-part-1-dc595057c1b9) with role-based actors
- Enjin’s Java SDK to integrate a [blockchain economy into your Minecraft server](https://blog.enjincoin.io/announcing-enjins-open-source-java-sdk-minecraft-plugin-minecraft-server-af7a34fa1d65)

**Ecosystem**

- [Swarm v0.4.0 released](https://www.reddit.com/r/ethswarm/comments/bpqxeu/swarm_v040_released/)
- POA Network is [picking up the Kovan testnet](https://forum.poa.network/t/kovan-testnet-upgrade-featuring-four-new-validators/2486) and changing it to 4 second block times.

**Enterprise**

- EEA [enterprise client spec v3](https://entethalliance.org/wp-content/uploads/2019/05/EEA_Enterprise_Ethereum_Client_Specification_V3.pdf). Plus EEA released [trusted compute spec v1.0](https://entethalliance.org/enterprise-ethereum-alliance-releases-dff-chain-trusted-compute-specification-1-0/)
- World Bank and Commonwealth Bank of Australia [trade 9 figure secondary bond](https://www.finextra.com/newsarticle/33825/world-bank-and-cba-record-secondary-bond-trading-on-a-blockchain/blockchain) built on Ethereum
- GE Aviation to [track aircraft engine parts maintenance](https://www.coindesk.com/codename-truengine-ge-aviation-and-microsoft-reveal-aircraft-parts-certification-blockchain) an use with a consortium chain built on Ethereum
- [Aura](https://content.consensys.net/wp-content/uploads/AURA_ConsenSys_Press-Release_May-16-2019-2.pdf): a product tracking consortium chain for the luxury industry from LVMH, ConsenSys and Microsoft
- [Element implementation](https://medium.com/transmute-techtalk/introducing-element-328b4260e757) of Decentralized Identity Foundation’s Sidetree Protocol

**Governance and Standards**

- Proposed [list of EIPs](https://github.com/ethereum/EIPs/blob/f8ffe537c1c684863570ee27527c01334517be9a/EIPS/eip-1679.md) for Istanbul hard fork
- [EIP2028](https://github.com/ethereum/EIPs/blob/77aa54f578b13e15c45d22dc1d5f9d93e231366c/EIPS/eip-2028.md): Calldata gas cost reduction
- [ERC2009](https://github.com/ethereum/EIPs/pull/2009/files): Compliance service
- [EIP2029](https://github.com/ethereum/EIPs/blob/7f770499088e402aa7db7c336361f063a4157e30/EIPS/eip-2029.md): State Rent A - State counters contract
- [EIP2031](https://github.com/ethereum/EIPs/blob/b5c02ae35481fbf96315ba36018a8e7779a5a887/EIPS/eip-2031.md): State Rent B - Net transaction counter
- [EIP2027](https://github.com/ethereum/EIPs/blob/bf8055e7faa512ed8237df2696c77cf8c666d319/EIPS/eip-2027.md): State Rent C - Net contract size accounting
- [EIP2026](https://github.com/ethereum/EIPs/blob/3be640ba18841c0ebc6f2f4e3526656a0ecfb5b1/EIPS/eip-2026.md): State Rent H - Fixed Prepayment for accounts
- [EIP2035](https://github.com/ethereum/EIPs/blob/76ece359ecec2feb51571adb114cf5378d4af566/EIPS/eip-2035.md): Stateless Clients - Repricing SLOAD and SSTORE to pay for block proofs
- [ERC2015](https://github.com/pedrouid/EIPs/blob/5101cc053161824c5d4b031e823c7bed35cefec6/EIPS/eip-2015.md): Wallet Update Chain JSON-RPC Method (\`wallet\_updateChain\`)
- Nexus Mutual: [digital cooperatives are the future](https://medium.com/nexus-mutual/digital-cooperatives-are-the-future-2b0772c1e03a)

**Application layer**

- [iExec v3](https://medium.com/iex-ec/v3-iexec-releases-data-wallet-for-enterprises-to-rent-data-and-ai-models-using-blockchain-e773a6bab69a): secure “data renting,” particularly aimed at enterprises. Massive [French utility company EDF to use it](https://www.coindesk.com/the-worlds-fifth-largest-electrical-company-is-using-an-ethereum-dapp).
- [Sell your personal Firefox info](https://medium.com/streamrblog/crowdselling-your-personal-data-through-firefox-c4f8bf9b8a96) through Streamr
- The CryptoKitties folks debut a [new game called CheezeWizards](https://medium.com/dapperlabs/cheeze-wizards-the-worlds-first-blockchain-battle-royale-with-cheese-756ec102f9ab)
- Cryptocup [returns for CopaAmerica](https://cryptocup.io/) - predict South America’s cup
- [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff/) on September 15th. Also interesting: Veil [forked Augur](https://twitter.com/joeykrug/status/1128732458193752065), though they say they’re coming back for v2
- 100m USD in [loans outstanding on DeFi](https://twitter.com/bloqboard/status/1128335007506927617)
- Maker Stability Fee [lowered to 17.5%](https://blog.makerdao.com/executive-vote-stability-fee-17-5/)
- [District0x launches MemeFactory](https://blog.district0x.io/introducing-meme-factory-4aba7925dcdd). Curation markets, TCRs. Memes.

**Interviews, Podcasts, Videos, Talks** 

- [Ethereal videos](https://www.youtube.com/playlist?list=PLJ8kQp5OiaEN6PALiLvOl1rcn3C7zoxRi)
- [Fluidity Summit vidos](https://www.youtube.com/playlist?list=PL8PE6YyYo5OIA5bzcLPAcVnZl_gjx8IyQ)
- Gitcoin’s [Kevin Owocki](https://www.zeroknowledge.fm/77) on Zero Knowledge
- Argent’s [Itamar Lesuisse](https://ethhub.substack.com/p/argent-the-immense-benefits-of-smart) on Into the Ether
- [Aya Miyaguchi](https://epicenter.tv/episode/287/) on Epicenter

**Tokens / Business / Regulation**

- Katie Haun: [what’s going on in the fight between Kik and the SEC](https://a16z.com/2019/05/15/kik-and-the-sec-whats-going-on-and-what-does-it-mean-for-crypto/)
- [Farewell words from outgoing CFTC Chair Giancarlo](https://www.coindesk.com/christopher-giancarlo-cftc-future-of-blockchain)

**General**

- [Fast Fourier Transforms](https://vitalik.ca/general/2019/05/12/fft.html) explainer
- Flexa and Gemini announce some major [retails chains to accept ETH and BTC](https://medium.com/flexa/the-flexa-network-is-open-for-business-8673c50c3d9d)
- [Stellar crashed for 2 hours and no one noticed](https://thenextweb.com/hardfork/2019/05/16/stellar-blockchain-cascading-failure-crash-nobody-noticed-cryptocurrency-xlm/)
- [A cryptocurrency wallet is not a wallet](https://medium.com/@zigguratt/a-cryptocurrency-wallet-is-not-a-wallet-97fa6eb29e48)! If you didn’t know this, click the link.

* * *

## **Dates of Note**

_Upcoming dates of note (new in **bold**)_**:**

- May 23-25 - [Swarm Orange Summit](https://www.eventbrite.com/e/swarm-orange-summit-madrid-2019-tickets-57378034245) (Madrid)
- May 24-26 - [Ethereum Madrid Hackathon](https://ethereummadrid.com/hackathon-2019/)
- May 27-28 - [EthCon Korea](https://ethcon.kr/) (Seoul)
- June 8-9 - [WASM in blockchains](https://avive.github.io/wasm_on_the_blockchain/#/) (Berlin)
- June 10-11 [Blockchain for Social Impact conference](https://conference.blockchainforsocialimpact.com/) (NYC)
- June 22-24 - [Zcon1](https://www.zfnd.org/zcon/) (Split, Croatia)
- July 3-5 - [WindingTree’s HackTravel](https://windingtree.com/hacktravel-lisbon-2019) (Lisbon)
- July 19 - [BuildETH](https://www.buildeth.io/) (San Francisco)
- Aug 2-4 - [ETHIndia](https://ethindia.co/) (Bangalore)
- Aug 2-4 - [TruffleCon](https://www.truffleframework.com/trufflecon2019) (Redmond)
- Aug 21-23 - [Dappcon](https://dappcon.io/) (Berlin)
- Aug 23-25 - [ETHBerlin](https://ethberlinzwei.com/)
- **September 15 - [Augur v1 cutoff](https://www.augur.net/blog/v1-cutoff/)**
- Sep 16-17 - [Starkware sessions](https://www.starkware.co/sessions/) (Tel Aviv)
- Oct 8-11 - [DeVcon](https://devcon.org/) (Osaka)

* * *

## **If you appreciate this newsletter, thank ConsenSys**

This newsletter is made possible by [ConsenSys](https://consensys.net/).  

[![](https://cdn.substack.com/image/fetch/w_1100,c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)](https://cdn.substack.com/image/fetch/c_limit,q_auto:good,f_auto/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F08f1b2fd-57e2-4d4b-bd42-730c769114be_240x240.jpeg)

  
I own Week In Ethereum. Editorial control has always been 100% me. 

If you're unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

* * *

## **It’s annoying how many link to the old URL. This is the new one: [weekinethereumnews.com](https://weekinethereumnews.com/)** 

Archive on the web if you’re linking to it: [https://weekinethereumnews.com/may-18-2019/](https://weekinethereumnews.com/may-18-2019/)

* * *

**Follow me on Twitter**, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter)?”

* * *

**Did you get forwarded this newsletter?  [Sign up](https://weekinethereum.substack.com/subscribe#about) to receive the weekly email**

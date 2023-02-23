---
title: "Week in Ethereum News <br> February 26, 2022"
date: "2022-02-26"
---

## **Eth News and Links**

**Mainnet execution layer**

- Erigon [v2022.02.04](https://github.com/ledgerwatch/erigon/releases/tag/v2022.02.04): optimization for getStorageAt & getBalance, auto detect latest, poke function to rebroadcast a transaction
- Otterscan [v2022.02.03](https://github.com/wmitsuda/otterscan/releases/tag/v2022.02.03-otterscan): address page adds ETH balance & contract creation info
- Besu [v22.1.1](https://github.com/hyperledger/besu/releases/tag/22.1.1): PoW switch off support; QBFT consensus algorithm is production ready for enterprise chains 

**Proof of Stake consensus layer**

- [Superphiz calls out the two largest staking pools](https://twitter.com/superphiz/status/1495397371466944523) (Coinbase & Kraken) for risking their funds and the network by running over 90% supermajority validators
    - Kraken [pledges greater client diversity](https://twitter.com/krakensupport/status/1495590333085798400)
    - Coinbase to [merely add Lighthouse remote signing](https://twitter.com/CoinbaseCloud/status/1496256008552960003) in the future
- [Rocket Pool](https://twitter.com/Rocket_Pool/status/1495571529819901954) now runs 1% of validators
- PoS implementers [call video](https://www.youtube.com/watch?v=fqPk576t5iw&t=231s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/r1nwpZHe9):
    - Kiln public testnet expected next week
    - push vs pull withdrawal designs
    - Discussed [safe block confirmation rule](https://notes.ethereum.org/@adiasg/safe-head) (safe against reorgs)
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220225)
- [Mini-danksharding prototype](https://twitter.com/protolambda/status/1495538286332624898) (data blob transactions): hacked together at ETHDenver, next steps are devnets & draft EIP
- [Nimbus migration guide](https://twitter.com/ethnimbus/status/1496404992575610880) using checkpoint sync
- Vouch [v1.4.0](https://github.com/attestantio/vouch/releases/tag/v1.4.0) (multi-node validator) adds Nimbus support
- Vitalik: [data availability sampling with inner product arguments](https://ethresear.ch/t/what-would-it-take-to-do-das-with-inner-product-arguments-ipas/12088) rather than KZG commitments

**PoW switch off**

- Kiln spec [v2](https://hackmd.io/@n0ble/kiln-spec#v2-change-set): EIP4399 renaming, Engine API auth and heartbeat
- Setup [local multiclient testnets](https://notes.ethereum.org/@ExXcnR0-SJGthjz1dwkA1A/H11OzhRAK) using Kurtosis; Kurtosis breakout [call](https://www.youtube.com/watch?v=yMe4RG5emx8&t=175s)
- Beacon chain withdrawals (will happen post-PoW switch off):
    - Draft EIP for [withdrawals on EVM](https://notes.ethereum.org/@ipsilon/H1lC5OAJ5)
    - [Pull style prototype](https://twitter.com/ralexstokes/status/1496991439938633733) on Geth, work in progress

**EIPs/Standards**

- [EIP4841](https://github.com/ethereum/EIPs/blob/501cf92b2f8fd7d61203e64a2fb5808107765680/EIPS/eip-4841.md): Expandable Onchain SVG Images Storage Structure
- [EIP4399](https://eips.ethereum.org/EIPS/eip-4399): Supplant DIFFICULTY opcode with PREVRANDAO

**Layer2**

- [zkSync v2.0](https://matterlabs.medium.com/zksync-2-0-public-testnet-is-live-de870ba9632a) EVM compatible zk-rollup public testnet
- [Optimism](https://twitter.com/optimismPBC/status/1496241118077505536) reduces timestamp update interval to 15 seconds
- Barnabé: [rollup economics](https://barnabe.substack.com/p/understanding-rollup-economics-from), framework for discussions on fees & economic designs
- Norswap’s optimistic perspective of [optimistic vs zk rollups](https://twitter.com/norswap/status/1494763568843132931)
- Polynya’s [state of chains](https://polynya.medium.com/optimistic-rollups-are-brilliant-and-the-state-of-blockchains-a57bc4799dca): optimistic rollups will scale faster but zk-rollups will catch up, every chain without validity, fraud & data proofs is dead
- Fran (OpenZeppelin maintainer): idea for [ERC20 bridge-mintable tokens](https://ethereum-magicians.org/t/idea-erc20-bridge-mintable-tokens/8422)

* * *

### **This newsletter is made possible thanks to [NEAR](https://near.org/)!**

![NEAR](https://weekinethereumnews.com/wp-content/uploads/2021/10/near_logo_stack.jpg)

NEAR has [launched Simple Nightshade sharding](https://near.org/blog/near-launches-nightshade-sharding-paving-the-way-for-mass-adoption/) to pave the way for greater throughput!

Recently [NEAR launched stake farming](https://medium.com/nearprotocol/near-launches-stake-farming-to-unlock-ecosystem-rewards-e09ae94d8218) for apps to work with staking pools to integrate apps’ tokens into their rewards.  The first launch was with Aurora EVM, so you can now stake $NEAR and be paid in $AURORA.

Learn more about what’s going on in NEAR in the community-driven [NEARweek](https://nearweek.com/) newsletter.

* * *

**Stuff for developers**

- Solidity development with [Replit](https://blog.replit.com/getting-started-with-solidity-on-replit) (web based IDE)
- [foundry deploy](https://github.com/joshieDo/foundrydeploy#readme): deployment script for Foundry, work in progress
- [Remix beta testers](https://twitter.com/EthereumRemix/status/1496971220905910275) wanted for v0.22 and UX research for product roadmap
- Guide for [Remix DGit plugin](https://medium.com/remix-ide/securing-you-file-in-remix-how-to-clone-and-push-f1350111aa13) to push files to GitHub
- [Deploy via MetaMask using Truffle Dashboard](https://trufflesuite.com/blog/introducing-truffle-dashboard/), supports Truffle & Hardhat
- [Cacheable Beacon Proxy](https://github.com/frangio/cacheable-beacon-proxy#readme): upgradeable proxy with 100 gas overhead
- [Shrines](https://github.com/Astrodrop/shrine#readme): ERC20 distribution to weighted list of addresses for fixed gas cost
- [ETH-Hentai](https://github.com/tradingstrategy-ai/eth-hentai#readme): library for Python of common contracts and utilities
- [w3](https://github.com/lmittmann/w3#readme): Go package, modular JSON RPC client with ABI support
- Sign-In with Ethereum [Ruby library](https://blog.spruceid.com/sign-in-with-ethereum-ruby-library-release-and-rails-examples/) (alpha) with Rails examples
- [Ethereum & StarkNet Data Warehouses](https://tokenflow.live/blog/edw-open): public beta, uses Snowflake cloud
- Getting started with [TrueBlocks](https://chasewright.com/getting-started-with-trueblocks/)
- [Dark Forest game](https://blog.zkga.me/dark-forest-and-the-diamond-standard) replaced upgrade system with EIP2535 (Diamonds)
- [Dynamic SVG NFT](https://twitter.com/austingriffith/status/1497031722591944708): mint NFT & set SVG, prototype built with scaffold-eth
- [ethernaut-x-foundry](https://github.com/ciaranmcveigh5/ethernaut-x-foundry#readme): Ethernaut CTF run locally with Foundry

**Security**

- Polygon PoS [consensus bypass vulnerability](https://medium.com/immunefi/polygon-consensus-bypass-bugfix-review-7076ce5047fe), required open validator spot with high capital costs, $75k bounty paid
- Harry Denley: [malicious tokens can abuse events](https://blog.mycrypto.com/bad-actors-abusing-etherscan-to-trick-you) for display on block explorers
- NFT [phishing attack](https://twitter.com/NadavAHollander/status/1495509511179755530) targeted OpenSea users

**Ecosystem**

- Laura Shin book: [The Cryptopians](https://www.publicaffairsbooks.com/titles/laura-shin/the-cryptopians/9781541763005/), inside look at the founding of Ethereum, [names likely hacker of The DAO](https://www.forbes.com/sites/laurashin/2022/02/22/exclusive-austrian-programmer-and-ex-crypto-ceo-likely-stole-11-billion-of-ether/?sh=72132ff37f58)
- [Ethereum Foundation grantees in Japan](https://blog.ethereum.org/2022/02/24/japan-local-grants-round/): zkCREAM, Ryodan, Startrail, w3aio & Famiee
- ETHDenver [hackathon submissions](https://hackerlink.io/hackathon/ethdenver22/)

**Application layer**

- [Yearn](https://twitter.com/iearnfinance/status/1496577884802060288) live on Arbitrum
- Hegic [HardCore](https://medium.com/hegic/hegic-hardcore-beta-release-2573a2d4cb3d) (options) beta live on Arbitrum
- [Ooki](https://blog.ooki.com/ooki-is-live-on-arbitrum/) (margin trading) live on Arbitrum
- [Request Finance](https://www.request.finance/post/arbitrum-powers-cheaper-faster-crypto-invoicing-and-payroll-in-request-finance) (invoicing & payroll) adds Arbitrum support
- Moloch [v3](https://decrypt.co/93196/dao-framework-builder-moloch-launches-v3-at-ethdenver) (Baal)
- DAOhaus [v3](https://daohaus.mirror.xyz/SKzS-s85EeEICZHjXLkpwN1UueAZMrvgFbI2tB0zkMc) early preview
- [MakerDAO discussion](https://forum.makerdao.com/t/against-the-burn/13412) against burning Maker in favor of growth
- Sound [Song Splits](https://twitter.com/soundxyz_/status/1495443379676717059): artists define collaborator splits when minting tracks
- [Isotile](https://twitter.com/isotile/status/1496580249865314305) (NFT metaverse) adds support for NFTs on Arbitrum

* * *

### **Job Listings**

- EF research hiring [Networking Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=54&source=weekinethnews)
- [Nomic Foundation](https://www.notion.so/Nomic-Foundation-jobs-991b37c547554f75b89a95f437fd5056) hiring Rust Tech Lead & Ethereum Tech Lead
- Roles at Gnosis [Sr DevRel Eng.](https://grnh.se/3052a2da2us) [Sr Production/Reliability Eng.](https://grnh.se/3345ebe02us) [DevOps Eng.](https://apply.workable.com/blockscout/j/0D9C5798DC/)
- Kwenta seeks [Frontend Engineer](https://blog.kwenta.io/kwenta-open-position-front-end-developer/), [Solidity Engineer](https://blog.kwenta.io/kwenta-open-position-solidity-engineer/) & [Marketing Lead](https://blog.kwenta.io/kwenta-open-position-marketing-manager/)
- [Internship program](https://nethermind.notion.site/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1) with Nethermind (1-3 month) 
- [Senior Technical Writer](https://ethereum.bamboohr.com/jobs/view.php?id=51&source=weekinethnews) to take ownership & completely redo the Geth docs

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Flexpool](https://www.reddit.com/r/ethereum/comments/t0hxqq/announcement_flexpoolio_is_halting_all_service_to/) halting services in Russia
- [Ontario Securities Commission](https://leaderpost.com/the-logic/osc-flags-emergencies-act-tweets-by-kraken-coinbase-ceos-to-rcmp) (Canada) contacted police over tweets from Coinbase & Kraken CEOs advocating non-custodial wallets
- [BitMex founders plead guilty](https://www.justice.gov/usao-sdny/pr/founders-cryptocurrency-exchange-plead-guilty-bank-secrecy-act-violations) in exchange for each paying $10 million fine

**General**

- Coinbase [vulnerability disclosed](https://blog.coinbase.com/retrospective-recent-coinbase-bug-bounty-award-9f127e04f060), API allowed trade submission with mismatched source account, $250k bounty paid to [Tree of Alpha](https://twitter.com/tree_of_alpha/status/1495014902582362112)
- Samsung Galaxy phones [keystore design](https://eprint.iacr.org/2022/208) found vulnerable to downgrade attack & IV reuse
- [Remote access via a browser](https://mrd0x.com/bypass-2fa-using-novnc/) is attack vector to steal credentials & bypass 2FA
- [Short-lived](https://eprint.iacr.org/2022/190) non-interactive zk proofs

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-february-26-2022](https://weekinethereumnews.com/week-in-ethereum-news-february-26-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Mar 9-24 – [Gitcoin Grants Round 13](https://twitter.com/gitcoin/status/1488231821854740481)
- Mar 11-20 – [Ethereum Rio](https://www.ethereum.rio/)
- Mar 15 – [Cryptocurrency Class](https://mirror.xyz/0xaFaBa30769374EA0F971300dE79c62Bf94B464d5/oGqGP2NOK9g7QPl1sMKkzql_Fh0P6hKbpYLZ-EkQTXU) starts (virtual) 
- Mar 16 – submission deadline for [Underhanded Solidity Contest](https://underhanded.soliditylang.org/)
- Mar 17-18 – [ETH Austin](https://2022.ethaustin.org/) summit
- Mar 29-31 – [ETHDubai](https://www.ethdubaiconf.org/)
- Apr 7-9 – [ETH Portland](https://2022.ethportland.com/) hackathon
- Apr 18-25 – [Devconnect](https://devconnect.org/schedule) (Amsterdam)
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- May 3-8 – [spaghettETH](http://spaghett-eth.com/) (Milan)
- May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETHNewYork](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

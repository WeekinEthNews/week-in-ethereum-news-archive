---
title: "Week in Ethereum News <BR> September 18, 2021"
date: "2021-09-18"
---

## **Eth News and Links**

**Mainnet execution layer**

- Upgrade Nethermind nodes to [v1.11.2](https://github.com/NethermindEth/nethermind/releases/tag/1.11.2)! [Unsuccessful attack](https://twitter.com/vdwijden/status/1437712249926393858) publishing ~550 blocks with invalid PoWs, small number of Nethermind nodes switched to invalid chain, all affected nodes reorged back to good chain
- Latest [core devs call video](https://www.youtube.com/watch?v=NorHRk5fFZU&t=523s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1438916709000253440):
    - PoW switch off difficulty to be hardcoded rather than computed
    - EIPs to include with difficulty bomb delay to be decided on next call; candidates: EIP3860 limit initcode, EIP3855 PUSH0 opcode and EIP3756 gas cap limit
- Erigon [v2021.09.03](https://github.com/ledgerwatch/erigon/releases/tag/v2021.09.03): fixes and tx pool improvements
- [Postmortem](https://github.com/ethereum/go-ethereum/blob/master/docs/postmortems/2021-08-22-split-postmortem.md) on August 27 minority chain split
- [Geth sunsetting fast sync](https://twitter.com/peter_szilagyi/status/1438503255126929408), in favor of snap sync

**Proof of stake consensus layer**

- Modelling [impact of Altair upgrade](https://pintail.xyz/posts/modelling-the-impact-of-altair/), how staking rewards change
- Teku [v21.9.1](https://github.com/ConsenSys/teku/releases/tag/21.9.1): stops including redundant attestations in blocks, fixes rare block creation exception.  [Fully sync with Teku](https://twitter.com/benjaminion_xyz/status/1438093650513235970) in less than 12 seconds
- Lighthouse [v1.5.2](https://github.com/sigp/lighthouse/releases/tag/v1.5.2): improves head vote rewards and on testnets improves Altair block processing times
- Lodestar client now [capable of 100% effectiveness](https://twitter.com/dapplion/status/1438882897260425217)
- Security of [BLS batch verification](https://ethresear.ch/t/security-of-bls-batch-verification/10748)

**Layer2**

- [Arbitrum grew $1.5 billion TVL](https://twitter.com/l2beatcom/status/1437100464005427211) in two weeks (now $2.6 billion at time of publishing)
- [Arbitrum Sequencer offline](https://medium.com/offchainlabs/arbitrum-one-outage-report-d365b24d49c) for ~45 minutes due to large burst of transactions, new transaction submission stopped, though [Arbitrum never went down](https://twitter.com/DZack23/status/1437923828391424005)
- The [validator strategies (active, defensive and watchtower)](https://medium.com/offchainlabs/fraud-proofs-and-validators-how-you-or-anyone-can-keep-arbitrum-honest-d68add3f6c5d) that keep Arbitrum trustless
- [Optimism EVM equivalence](https://medium.com/ethereum-optimism/the-future-of-optimistic-ethereum-7f22d987331) coming in October, so you can deploy your existing Solidity contracts on Optimism with same tooling
- [Throughput limit](https://twitter.com/optimismpbc/status/1437437368303329289) doubled on Optimism to 200k transactions per day
- Protolambda’s [Optimistic brainf\*\*\*](https://twitter.com/protolambda/status/1436806120249729026): experiment with alternative VMs in an open rollup infrastructure
- Blockchains as [layers of specialization](https://polynya.medium.com/the-lay-of-the-modular-blockchain-land-d937f7df4884): execution (rollups), security (Ethereum) and data availability (data shards)
- [Hop](https://twitter.com/HopProtocol/status/1438612133776867330) supports Arbitrum for USDC & USDT transfers between L2 and mainnet
- Why rollups are a [superior long-term execution layer](https://polynya.medium.com/addressing-common-rollup-misconceptions-eba9d758707e)

* * *

### **This newsletter is made possible thanks to [Celer Network](https://www.celer.network/)!**

![Celer](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png)

Celer Network is a layer-2 scaling platform that brings fast, secure and low-cost blockchain applications. Celer cBridge 1.0 is now live on mainnet. Users are now able to use cBridge to [instantly transfer tokens across 10 different chains and optimistic rollups](https://cbridge.celer.network/). 

Since launch, cBridge has witnessed doubling weekly volume growth and reached $120M total transaction volume today. Use at [cbridge.celer.network](https://cbridge.celer.network/)

* * *

**Stuff for developers**

- Remix IDE [v0.18.0](https://medium.com/remix-ide/remix-ide-v0-18-0-is-released-d6605c50817e): GitHub integration, plugins activate other plugins
- OpenZeppelin Contracts [v4.3.2](https://github.com/OpenZeppelin/openzeppelin-contracts/releases/tag/v4.3.2): security patch for UUPSUpgradeable
- web3.js potential [upcoming breaking change](https://twitter.com/web3_js/status/1438608789306023936): web3.eth.getBlock baseFeePerGas changing from hex to BigNumber  
- [Add and switch networks](https://twitter.com/liamihorne/status/1437168861846069254) programmatically for your users
- [Consolerr](https://github.com/AztecProtocol/consolerr) (Solidity library): log runtime variables in error messages
- Otterscan [v2021.09.02](https://twitter.com/wmitsuda/status/1437502826649997313): early access to Sourcify integration
- Guide to [storing NFT metadata and SVG images](https://andyhartnett.medium.com/solidity-tutorial-how-to-store-nft-metadata-and-svgs-on-the-blockchain-6df44314406b) on chain
- [EmbeddedMultiCall](https://github.com/Defi4Bitcoin/EmbeddedMultiCall): similar to Maker’s Multicall but without onchain deployment, written in Yul
- Beginner tutorial: [create and sell/buy an ERC20](https://stermi.medium.com/how-to-create-an-erc20-token-and-a-solidity-vendor-contract-to-sell-buy-your-own-token-8882808dd905)
- [CryptoHack courses](https://cryptohack.org/courses/): introduces players to modern cryptography fundamentals via curated challenges
- [ENS looking for dapps](https://twitter.com/brantlymillegan/status/1438906449854353408) to implement NFT as avatar for ENS names

**Security**

- SushiSwap’s [Miso ~860 ETH exploit](https://www.coindesk.com/tech/2021/09/17/3m-was-stolen-but-the-real-steal-is-these-kia-sedonas-say-anonymous-developers/) changed recipient of Kia Sedona NFT proceeds, supply chain attack of front end; funds were returned
- OpenZeppelin UUPS proxy [post mortem](https://forum.openzeppelin.com/t/uupsupgradeable-vulnerability-post-mortem/15680), uninitialized implementation contracts could be self destructed bricking any proxy using it
- Yearn Vesting Escrow [bug](https://twitter.com/0xbunnygirl/status/1438632697929158656), escrow could be reinitialized and bricked after ownership renounced
- Yam Finance [post mortem](https://yamfinance.medium.com/yam-minting-incident-postmortem-b76afd1aef45) from minting 20 billion YAM in error
- [Privacy in DeFi](https://arxiv.org/abs/2109.06836), many trackers on DeFi websites can record Eth addresses and can trivially link to Personally Identifiable Information
- [Air dropped tokens with apparent high value](https://twitter.com/sniko_/status/1438643879851528199) revert on approve, directing to a website that sweeps highest held ERC20
- OpenZeppelin [security guidelines](https://blog.openzeppelin.com/smart-contract-security-guidelines/) for contract development
- Guide to using linear programming to [calculate optimal parameters](https://medium.com/immunefi/how-to-get-a-bigger-bounty-by-optimizing-attack-parameters-a51b144f5cc2) so as to determine maximum funds at risk when disclosing vulnerabilities
- Babel, Daian, Kelkar [paper on quantifying economic security](https://twitter.com/phildaian/status/1438532084130275334), including tool for doing so

**Ecosystem**

- SpruceID selected to [develop Sign-in with Ethereum](https://blog.spruceid.com/sign-in-with-ethereum/)
- [80% of MetaMask users](https://twitter.com/timbeiko/status/1437857299473653760) never make it to the edit gas screen
- [Update Ledger firmware to v2](https://twitter.com/MetaMaskSupport/status/1438609003928555527) to use with latest MetaMask
- [Eth.limo](https://blog.fleek.co/posts/eth-limo-alternative-eth-link), alternative to eth.link to resolve .eth names on browsers

**Enterprise**

- [Infura Transactions](https://consensys.net/blog/press-release/infura-transactions-itx-simplifies-transaction-management-on-ethereum/) public release: meta transactions allow enterprises not to hold Ether, transaction management auto bumps gas fees 
- [ConsenSys Quorum Proof of Authority network](https://consensys.net/blog/codefi/codefi-activate/over-32000-users-from-130-countries-applied-to-purchase-damien-hirsts-nfts-on-the-palm-network/?utm_content=180233221&utm_medium=social&utm_source=twitter&hss_channel=tw-1156973517264625665) used for Palm NFTs

**Application layer**

- [OpenSea iOS and Android app](https://twitter.com/opensea/status/1438936921066164225), view only, no SVG support yet
- [OpenSea implements staff policies](https://opensea.io/blog/announcements/employee-information-use-at-opensea/) to not buy/sell promoted NFTs or use confidential information after staff member traded promoted NFTs
- [Smol Puddle](https://smolpuddle.io/): ERC721 marketplace on Arbitrum, decentralized order book using Waku, unaudited alpha with no tests
- [NFT Chain rule](https://twitter.com/zoink/status/1437236693413744641): a meme’s value is proportional to number of derivatives
- Uniswap [Auto Router](https://uniswap.org/blog/auto-router/), splits trades across multiple pools, uses more data, factors gas costs and switches to V2 if better to get best trade
- [Curve](https://twitter.com/charlie_eth/status/1437543305169063940) on Arbitrum
- [Tracer Perpetual Pools](https://tracer.finance/radar/perpetual-pools-launch/) on Arbitrum
- [Ribbon v2 Vaults](https://twitter.com/ribbonfinance/status/1437529366100066307): decentralized and autonomous, [comparable to v1 Vaults performance](https://twitter.com/ribbonfinance/status/1438904003526631426)
- Gnosis Guild’s [Zodiac toolsuite](https://gnosisguild.mirror.xyz/OuhG5s2X5uSVBx1EK4tKPhnUc91Wh9YM0fwSnC8UNcg) for DAOs: Exit (rage quit), Bridge, (time) Delay and Reality (formerly SafeSnap)  
- [BrightDAO](https://medium.com/brightid/brightdao-is-here-bdcb198393e): token drop per person rather than per address using BrightID with ongoing faucets
- [Myco](https://m.mirror.xyz/6UxMOPMAnCZr8XSkhIM2Xx47bZ7X5rColwpnwIDbx5s) digital social clubs as LLCs co-owned by contributors
- [Dope Wars](https://github.com/dopedao/RYO) on a StarkNet zkRollup

**Regulation/business/tokens**

- [Update of Gnosis Safe iOS app](https://twitter.com/SchorLukas/status/1437728066218958850) blocked by Apple due to NFT display
- [Coinbase filed to register as a Futures Commission Merchant](https://twitter.com/coinbase/status/1438247595877416962) in the US, to allow it to offer futures and derivatives trading
- US infrastructure bill includes [digital asset recipients to verify senders info](https://twitter.com/abesutherland/status/1438881314871156736) and report to the government within 15 days
- Franklin Templeton [raising for first blockchain fund](https://www.coindesk.com/business/2021/09/15/franklin-templeton-seeks-20m-for-first-blockchain-venture-fund/)
- [Rolling SAFE](https://blog.fairmint.co/a-new-era-of-high-resolution-fundraising-the-rolling-safe-1fb67eee68ab): ongoing startup funding, and why Fairmint thinks it fulfills Paul Graham’s high resolution fundraising vision

**General**

- [The Economist](https://www.economist.com/leaders/2021/09/18/the-beguiling-promise-of-decentralised-finance): Bitcoin is now a distraction, Ethereum upon which most DeFi applications are built, is reaching critical mass
- [Vitalik](https://time.com/collection/100-most-influential-people-2021/6095980/vitalik-buterin/) in Time 100 most influential people of 2021
- [Leave Travis CI](https://twitter.com/peter_szilagyi/status/1437646118700175360): secure env variables injected into PR builds, no security disclosure
- Apple patches [zero click iMessage bug](https://citizenlab.ca/2021/09/forcedentry-nso-group-imessage-zero-click-exploit-captured-in-the-wild/), update iOS immediately
- CNBC duped into [Litecoin pump and dump through fake press release](https://www.reuters.com/business/retail-consumer/press-release-walmarts-litecoin-partnership-is-fake-cnbc-2021-09-13/) which @Litecoin tweeted
- [Decentralised CloudFlare](https://ethresear.ch/t/decentralised-cloudflare-using-rln-and-rich-user-identities/10774) using RLN and rich user identities
- Google and Apple cave to Russia and [remove pro-Navalny app](https://www.nytimes.com/2021/09/17/world/europe/russia-navalny-app-election.html) after threats to prosecute local employees
- [Fflonk](https://eprint.iacr.org/2021/1167) a Plonk variant, greatly reduces verifier cost by using Kate commitments to allow multiple polynomials in a commitment

* * *

## **Job Listings**

- OpenZeppelin hiring [Open Source Developer](https://openzeppelin.com/jobs/opening/?gh_jid=4554917003)
- Rarible is hiring: [VP of Product](https://jobs.lever.co/Rarible/47ed8db0-2161-420c-9321-4ade80e8dece) and [Product Manager](https://jobs.lever.co/Rarible/06d88504-b740-434e-87c0-72846b9ddeeb)
- yAcademy 1 month [internships](https://yacademy.github.io/internships/)
- Nethermind 1-3 month [internship program](https://www.notion.so/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)

**Want to reach people experienced with Ethereum? List your job here.** $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to abcoathup.eth. Questions? abcoathup at-gmail

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-18-2021/](https://weekinethereumnews.com/week-in-ethereum-news-september-18-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Sep 24  – [Gitcoin Grants Round 11](https://gitcoin.co/grants/) ends (support [Week in Eth News](https://gitcoin.co/grants/2785/week-in-ethereum-news))
- Sep 30 – [NFT Fest Australia](https://nftfest.com.au/) (virtual)
- Oct 1-3 – [EthAtlanta](https://ethatl.com/) enterprise-focused hackathon & keynotes
- **Oct 18 – [ENS online workshop](https://medium.com/the-ethereum-name-service/ens-online-workshop-october-2021-ec1fb049b77f)**
- Oct 20-21 – [LisCon](https://liscon.org/) (Lisbon) **sold out**
- Oct 22-24 – [ETH Lisbon](https://ethlisbon.org/) hackathon

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

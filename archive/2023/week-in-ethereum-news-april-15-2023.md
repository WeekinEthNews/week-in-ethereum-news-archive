---
title: "Week in Ethereum News <br> April 15, 2023"
date: "2023-04-15"
---

## Eth News and Links

**Shapella (Shanghai + Capella) upgrade**

- [Mainnet upgraded](https://twitter.com/TimBeiko/status/1646264219019407360) to Shapella:
    - Staking withdrawals are being processed (view on [beaconcha.in](https://beaconcha.in/validators/withdrawals))
    
    - Christine Kim: [withdrawal misconceptions](https://twitter.com/christine_dkim/status/1646916343952703488)
    
    - [Prysm validators using MEV-Boost](https://arbitrum.notion.site/17-relayers-are-failing-with-the-prysm-client-post-Capella-Shanghai-2023-04-12-mainnet-0ef5ccd795e54ae4894fa695f1a3e70b) failed to propose blocks
    
    - [~100 validators with double deposits](https://twitter.com/lefterisjp/status/1646274484817522689) can retrieve their extra ETH
    
    - first [transaction using new PUSH0 opcode](https://twitter.com/vex_0x/status/1646281317925920769)

- Hot fixes:
    - Lighthouse [v4.0.2-rc.0](https://github.com/sigp/lighthouse/releases/tag/v4.0.2-rc.0): fix for high CPU when missed blocks & high volume of exits
    
    - Prysm [v4.0.2](https://github.com/prysmaticlabs/prysm/releases/tag/v4.0.2): fix for interacting with MEV-Boost

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=u8Nm8AGyCQM&t=142s). Summary by [Tim Beiko](https://twitter.com/timbeiko/status/1646550211580264452).  Notes from [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-execution-call-159/):
    - Shapella went relatively smoothly: Prysm MEV-Boost bug caused missed blocks which triggered Lighthouse high CPU, Teku investigating slow block import
    
    - Dencun scope to be discussed at next ACDE call
    
    - Discussions on EIP4788 design, starting testnets with Capella genesis state, payload IDs and Execution API addition for MEV-Boost

- [Zhejiang testnet](https://twitter.com/parithosh_j/status/1646851561224654848) being taken down April 19

**Dencun (Cancun + Deneb) upgrade**

- KZG ceremony special contributions:
    - Mr. Moloch's [Ephemeral album II](https://twitter.com/trent_vanepps/status/1645532615137693703) made & destroyed in one day
    
    - [Random dog walk](https://twitter.com/saint_rat/status/1645550341692194816) from eating dropped dog biscuits
    
    - [Improvised theater](https://twitter.com/thomasdenh/status/1645911736896110594) with music

- [Nimbus](https://github.com/status-im/nimbus-eth2/pull/4803) added Blobfish ASCII art for when Deneb activates

- Proposal to [rename danksharding to dankscaling](https://twitter.com/adietrichs/status/1646402410708094976)

**Layer 1**

- [Mevboost.pics](https://twitter.com/nero_eth/status/1645056071889813504) added average MEV payment per relay/builder/validator in boxplots

- [Bootnode diversity discussion](https://ethresear.ch/t/execution-consensus-client-bootnodes/14588/21): client teams could run geo diverse bootnodes on bare metal

- Terence: [single slot PBS using attester committee](https://hackmd.io/@vianq8jgSjC9fiZvnjcAvw/ryKYUjbf3) notes & open questions

**For Stakers**

- [Staking pool](https://twitter.com/evan_van_ness/status/1646903790111522817) execution client diversity

- Somer’s [configuring withdrawal credentials guide](https://someresat.medium.com/guide-to-configuring-withdrawal-credentials-on-ethereum-812dce3193a) & updated [staking guides](https://github.com/SomerEsat/ethereum-staking-guides)

**Research**

- Barnabé Monnot: [protocol credibility = introspection + agency + community defense of last resort](https://barnabe.substack.com/p/seeing-like-a-protocol)

- [Sync committee slashing](https://github.com/ethereum/consensus-specs/issues/3321) to deter against signing non-canonical beacon block roots

**Layer 2**

- Intro to [MEV on Layer 2 sequencers](https://twitter.com/francescoglt/status/1646875996925333504)

**EIPs/Standards**

- EIPs:
    - [EIP6873](https://github.com/ethereum/EIPs/pull/6873/files): Preimage retention

- ERCs:
    - [ERC6864](https://github.com/ethereum/EIPs/pull/6864/files): Upgradable fungible token
    
    - [ERC6865](https://github.com/ethereum/EIPs/pull/6865/files): Onchain EIP712 visualization

* * *

### **This newsletter is made possible thanks to the funding received from Optimism’s** [**RetroPGF**](https://optimism.mirror.xyz/Upn_LtV2-3SviXgX_PE_LyA7YI00jQyoM1yf55ltvvI?rpgf)**!**

![Optimism's RetroPGF: Week in Ethereum News](https://weekinethereumnews.com/wp-content/uploads/2023/04/RetroPGF-WiEN-1024x546.png)

Thank you to [Optimism’s RetroPGF round 2](https://optimism.mirror.xyz/Upn_LtV2-3SviXgX_PE_LyA7YI00jQyoM1yf55ltvvI?rpgf) which generously funded Week in Ethereum News for “months, not weeks.”

* * *

**Stuff for developers**

- Hardhat [v2.13.1](https://github.com/NomicFoundation/hardhat/releases/tag/hardhat%402.13.1): added Shanghai support

- [Foundry-devops](https://github.com/ChainAccelOrg/foundry-devops#readme): get most recent deployment, requires ffi

- [Difftastic](https://community.thecreed.xyz/c/tools/difftastic-a-next-level-diff-tool) (diff tool) supports Solidity using tree-sitter parser

- [Rolling dutch auction](https://github.com/deomaius/rolling-dutch-auction#readme) in Solidity: perpetual auction with composite decay

- [Property-based testing](https://medium.com/@jat9292/building-a-smart-contracts-fuzzer-for-fun-and-profit-1f73323c2b4d) using Hypothesis Python library

- [Dedaub contract library](https://twitter.com/dedaub/status/1645930929729273857) (mainnet) added decompile to Yul

- [Titanoboa (Vyper interpreter) cheats](https://twitter.com/big_tech_sux/status/1646148954709544964) can be written as Python functions

- [HuffBoa](https://github.com/z80dev/HuffBoa#readme): example repo for using Huff contracts with titanoboa

- Alchemy [Spearmint](https://twitter.com/alchemyplatform/status/1646605943965368320): allowlist platform, low-code

- [Create T3 App](https://codingwithmanny.medium.com/combine-sign-in-with-ethereum-with-create-t3-app-8f54604caeeb) (NextJS, NextAuth, Prisma, tRPC, Tailwind & TypeScript) with Sign-In With Ethereum

- Create a [Council Voting Vault](https://twitter.com/delv_tech/status/1645487258617643008)

- [Indexed.xyz](https://goldsky.com/blog/introducing-indexed-xyz): raw blocks, transactions & event logs and decoded event logs for mainnet

**Security**

- iEarn [$10 million exploit](https://twitter.com/iearnfinance/status/1646644624314757120), yUSDT misconfigured, multiple pools drained

- SushiSwap [~$3.3 million exploit](https://rekt.news/sushi-yoink-rekt/), didn’t check for a genuine Uniswap v3 pool, attempted whitehat copied by MEV bots

- Paribus [~$100k exploit](https://twitter.com/peckshield/status/1645742296904929280) on Arbitrum, reentrancy of Compound v2 fork

- [Pretend hack](https://twitter.com/haydenzadams/status/1646937025210195968) to trick users into using fake revoke sites

**Ecosystem**

- Etherscan:
    - [Zero-value token transfers hidden](https://twitter.com/etherscan/status/1645406189692526593) by default
    
    - [EthValidate](https://twitter.com/etherscan/status/1646485065520775168): verify explorer data on using data from other nodes

**Notable at app layer**

- Ondo [OMMF](https://www.prnewswire.com/news-releases/ondo-finance-announces-new-token-ommf-providing-tokenized-exposure-to-us-money-market-funds-targeting-100-billion-stablecoin-market-301796332.html) (money market funds token): KYC & 100k USDC minimum 

- [Gandalf](https://alpha.gandalf.page/): tokengate Typeform, Notion, Substack, Medium, Gitbook & Google Docs, alpha

- Metropolis [podarchy explorer](https://pod.xyz/): visualize account relationships, permissions & multisig signers

* * *

### Job Listings

- EF Ecosystem Support Program seek a [Grant Analyst & Liaison](https://jobs.lever.co/ethereumfoundation/92306cf4-1a7d-4e32-bc23-9762383522b1)

**Job listings: $600 for four issues** (75 character limit), payable to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Commissioner Peirce calls out Chairman Gensler's clandestine power grab](https://www.sec.gov/news/statement/peirce-rendering-inovation-2023-04-12) to expand the SEC's reach and push all DeFi out of the US

- Tether [blacklisted 3 million USDT](https://twitter.com/peckshieldalert/status/1645702939498135552) from MEV bot exploiter

- NYTimes reports on [debanking of the current disfavored](https://www.nytimes.com/2023/04/08/your-money/bank-account-suspicious-activity.html)

- [Wallets should be invisible](https://mirror.xyz/sylve.eth/A8VnNvBVbc0aXmW2FlG58ysI8oZUnH0HGwwjIsQGHUk), using WebAuthn

**General/crypto**

- Summer of Protocols [researchers](https://paragraph.xyz/@protocolized/introducing-the-summer-of-protocols-cohort)

- [PLONKish ZK-SNARK](https://taiko.mirror.xyz/9kGUby8h_dyu-t8jcPkDADfbWUMJw3mlGxvZAZk9sV0) explainer

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-april-15-2023](https://weekinethereumnews.com/week-in-ethereum-news-april-15-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Apr 21-25 – [EthTaipei](https://ethtaipei.org/) hackathon & conference

- Apr 25 - May 9 – [Gitcoin Program Beta Round](https://gitcoin.notion.site/Gitcoin-Grantee-Portal-6adfc92627474bd48a5dfcd1e8438d20)

- Apr 27-30 – [Istanbul ETH Privacy](https://www.leadingprivacy.com/istanbul) conference & hackathon

- Apr 28 – deadline for EF’s [Next Billion fellowship cohort 3](https://blog.ethereum.org/2023/03/16/fellowship-cohort-3-applications)

- May 5-10 – [ETHTallinn](https://ethtallinn.org/) hackathon & [NFT Tallinn](https://nfttallinn.com/) conference

- May 9-12 – [EY blockchain summit](https://web.cvent.com/event/c066d44d-4e50-4d7e-b6fb-3cc0abdae7ff/websitePage:34e89f81-7647-4dff-b5f8-cd05d75a1ea7)

- May 12-14 – [ETHGlobal Lisbon](https://ethglobal.com/events/lisbon)

- May 19-23 – [EDCON](https://edcon.io/) Montenegro (changed from Vienna)

- May 20-21 – [ETHDam](https://www.ethdam.com/) (Amsterdam) conference & hackathon

- May 24-26 – [Spaghett ETH](https://naples.spaghett-eth.com/) (Naples) conference

- May 26-28 – [ETHDublin](https://www.ethdublin.io/) hackathon

- Jun 2-4 – [ETH Seoul](https://2023.ethseoul.org/)

- Jun 2-7 – [ETH Belgrade](https://ethbelgrade.rs/) conference & hackathon

- Jun 9-11 – [ETHPrague](https://ethprague.com/) conference & hackathon

- Jun 23–25 – [ETHGlobal Waterloo](https://ethglobal.com/events/waterloo2023) (changed from Toronto)

- Jul 5-7 – [ETHBarcelona](https://ethbarcelona.com/)

- Jul 15-16 – [DeFi Security Summit](https://defisecuritysummit.org/) (Paris)

- Jul 17-20 – [EthCC](https://ethcc.io/) (Paris)

- Jul 21–23 – [ETHGlobal Paris](https://ethglobal.com/events/paris2023)

- Aug 13-16 – [ETHToronto](https://www.ethtoronto.ca) & [ETHWomen](https://www.ethwomen.com/)

- Aug 16-19 – [Ethereum Argentina](https://ethereumargentina.org) (Buenos Aires)

- Aug 28-30 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc23/) (Stanford University)

- Aug 30 - Sep 3 – [ETHWarsaw](https://www.ethwarsaw.dev/) conference & hackathon

- Sep 1-3 – [Ethcon Korea](https://ethcon.kr/) hackathon

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 18-21 – [ETH Montréal](https://ethmontreal.xyz/) hackathon & conference

- Sep 22–24 – [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 6–27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 27–29 – [ETH Miami](https://ethmiami.net/) festival + hackathon

- Oct 28–30 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- November – Devconnect

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

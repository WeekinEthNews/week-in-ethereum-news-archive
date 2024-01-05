---
title: "Week in Ethereum News <br> December 9, 2023"
date: "2023-12-09"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade (meta** [**EIP7569**](https://eips.ethereum.org/EIPS/eip-7569)**)**

- Latest all core devs – execution (ACDE) [call video](https://www.youtube.com/watch?v=5KMvtxiSbow&t=212s). Recap by [Tim Beiko](https://mirror.xyz/abcoathup.eth/e3VlsWAgzqo4bDsPVzPyVOu3qQ6ithZxKXxB_fy5Aac).  Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1732813652536009115) and [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-execution-call-176/):
    - Devnet-12: issues being found & fixed; Prysm expect to join in 1-2 weeks
    
    - Goerli ~300 node shadow fork planned before end of December
    
    - Goerli upgrade to be scheduled in January to test 3/6 (target/max) blobs
    
    - Community can [propose EIPs for next upgrade](https://ethereum-magicians.org/t/prague-electra-network-upgrade-meta-thread/16809), to be discussed in January

- Consensus-specs [v1.4.0-beta.5](https://github.com/ethereum/consensus-specs/releases/tag/v1.4.0-beta.5): clarifies when clients can serve blocks & sidecars byRoot

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 32.03%**](https://twitter.com/lidodominance/status/1733124269368877152) **is far too close to** [**33.3% threshold**](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=1050s)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth ~84% supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm 41% & Lighthouse 34%, any client bug over 33.3% could mean loss of finality

- Better [geographic diversity is optimal](https://nodewatch.io/), particularly outside of North America & Europe

**Layer 1**

- [Reth (node) crawler](https://etherclients.com/): ~19k active nodes found using [UDP & inbound TCP](https://twitter.com/0xprames/status/1732250192655618222)

- [Erigon](https://erigon.tech/erigons-roadmap-to-2024/) 2024 roadmap: Erigon++ (evmone, SilkRPC C++ components), Caplin full archive node, Erigon v3 & Otterscan (enhanced with Erigon v3 & Beacon Chain capability via Caplin)

- Lightclients: [EIP3074](https://hackmd.io/@matt/note-on-3074) (AUTH & AUTHCALL opcodes) would allow EOAs to be used within ERC4337 (Account Abstraction using alt transaction pool)

**For Stakers**

- [Rescue Node](https://twitter.com/Rescue_Node/status/1732533290127499317) adds support for solo stakers, fallback node for temporary access in emergencies/maintenance

**Client releases**

- Execution layer:
    - Erigon [v2.55.1](https://github.com/ledgerwatch/erigon/releases/tag/v2.55.1): patch
    
    - Nethermind [v1.23.0](https://github.com/NethermindEth/nethermind/releases/tag/1.23.0): OP Stack support (Canyon upgrade not yet supported), initialize DB using snapshot and reduced memory consumption when overloaded with CL requests
    
    - Reth [v0.1.0-alpha.13](https://github.com/paradigmxyz/reth/releases/tag/v0.1.0-alpha.13): fix block commit times for full node & heavy RPC tracing users

**Research**

- [Timing games](https://ethresear.ch/t/timing-games-implications-and-possible-mitigations/17612): implications of proposers delaying block publication to increase MEV and pros & cons of possible mitigations

- [CEX<>DEX arbitrage](https://ethresear.ch/t/empirical-analysis-of-cross-domain-cex-dex-arbitrage-on-ethereum/17620) empirical analysis

**Layer 2**

- L2BEAT [liveness dashboard](https://twitter.com/l2beat/status/1731988273839407168) adds intervals of proof submissions for zk rollups

**EIPs/Standards**

- ERCs (application layer):
    - [ERC7570](https://github.com/ethereum/ERCs/pull/143/files): Security token interface for confidentiality & legal status transparency
    
    - [ERC7571](https://github.com/ethereum/ERCs/pull/151/files): Shadow events
    
    - [ERC7572](https://github.com/ethereum/ERCs/pull/150/files): Contract-level metadata via contractURI

**Stuff for developers**

- [Solidity developer survey 2023](https://soliditylang.org/blog/2023/12/08/solidity-developer-survey-2023-announcement/): feedback to the Solidity team

- [Shadow](https://blog.shadow.xyz/introducing-shadow/) logs: add custom events for contracts to offchain shadow fork, access via RPC

- [Foundry Go differential fuzzing](https://github.com/kjr217/foundry-go-template) template to compare Solidity & Go implementations

- [Wagmi-permit](https://github.com/vacekj/wagmi-permit#readme): sign ERC2612/DAI permits with viem/wagmi

- Guide to [web3.py typed data message signing](https://snakecharmers.ethereum.org/typed-data-message-signing/)

- EF Python team: [Ethereum Python user survey](https://forms.gle/a5EedxU5FtWv1pQq5)

- OpenZeppelin [access manager explorer](https://twitter.com/openzeppelin/status/1732448662230356110) for contract permissions

- Protolambda’s [Grug wallet](https://twitter.com/protolambda/status/1731104505918288233) design

**Security**

- [OpenZeppelin](https://blog.openzeppelin.com/arbitrary-address-spoofing-vulnerability-erc2771context-multicall-public-disclosure): contracts integrating both Multicall & ERC2771 vulnerable to address spoofing
    - Thirdweb [vulnerability](https://blog.thirdweb.com/security-vulnerability/), impacted pre-built contract deployers need to mitigate

**Ecosystem**

- Blocknative [Ethernow](https://www.ethernow.xyz/) transaction explorer (including live transaction pool), desktop only

- [Parsec](https://parsec.finance/blog/explorer) block explorer, supports mainnet & L2s, transaction heat map and custom layouts for address types

- MEV searching strategy: [blind arbs on private orderflow](https://twitter.com/bertcmiller/status/1732530082558931119)

- EF [run a node grantees](https://blog.ethereum.org/2023/12/06/run-a-node-grantee): 35 recipients from 23 countries

- Optimism’s [RetroPGF3 voting ended](https://twitter.com/retropgf/status/1733116557482504324), [502 projects](https://app.powerbi.com/view?r=eyJrIjoiNGM0YjEyYjEtMzc2ZS00NDBiLTgxNjItOTgzZDY0MGQxNmNmIiwidCI6IjRjYThhMzQ5LThiMmEtNDY1Yy05MTdlLWM1ZThhMjdjMzhjNCIsImMiOjN9) qualified for share of 30M OP

**Enterprise**

- [Societe Generale](https://www.societegenerale.com/en/news/press-release/first-inaugural-digital-green-bond-public-blockchain) issued EUR 10M green bond onchain

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 21.4 to 144.2 gwei, with 45.2 gwei average
    - Zero net issuance currently at 21.8 gwei 
    
    - 17.6k ETH net burn this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $2,086 - $2,385, currently $2,361

- [ETHBTC](https://ratiogang.com/): currently 0.053 (Flippening at ~0.16)

**Notable at app layer**

- Safe [RecoveryHub](https://safe.mirror.xyz/WxKSxD9J1bRI-SDOuDvAAIezwVrvWWkpuwuzcLDPSmk): set multisig recoverer(s), recovery attempt can be canceled within review window

- Coinbase Wallet [links](https://www.coinbase.com/blog/with-coinbase-wallet-sending-money-is-now-as-easy-as-sending-a-text): send USDC via a shareable link, returned if not claimed within 2 weeks

- Matcha [cross chain swaps](https://blog.matcha.xyz/article/cross-chain-swaps) live on mainnet, L2s & sidechains

- [Proof of P2P](https://twitter.com/zkp2p/status/1730646286523584677): soulbound NFT, zk proof of unique human with P2P account, requires Venmo

- Optimism [We ❤️ the Art](https://twitter.com/optimismFND/status/1732159055420854732) (NFT creator contest) extended to January 8

* * *

### Job Listings

- Enya Labs: [Lead Security Engineer](https://enyalabs.applytojob.com/apply/vkSNxMxgCT/Founding-Security-Engineer?source=weekinethereumnews), [Sr. Fullstack Dev](https://enyalabs.applytojob.com/apply/FlzWnQ2S7G/Senior-Full-Stack-Developer?source=weekinethereumnews) (with Go exp), [BizDev](https://enyalabs.applytojob.com/apply/eIiMobirGL/Business-Development?source=weekinethereumnews)

- [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db) wanted by EF

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

**Job listings: $600 for four issues** (75 character limit).  [**Pay**](https://3cities.xyz/#/pay?c=CAEaDWFiY29hdGh1cC5ldGgiAgIBKgIGFDoRV0VUSCBFVEggREFJIFVTRENKCgEACgQCAQYBCgFaQ1dlZWsgaW4gRXRoZXJldW0gTmV3cyBKb2IgTGlzdGluZzogZm91ciBpc3N1ZXMgKDc1IGNoYXJhY3RlciBsaW1pdCmSAY8Cfm1haWx0bzphYmNvYXRodXBAZ21haWwuY29tP3N1YmplY3Q9Sm9iJTIwTGlzdGluZyUyMFB1cmNoYXNlZCZib2R5PUhpJTJDJTBEJTBBJTBEJTBBSSUyMHB1cmNoYXNlZCUyMGElMjBXZWVrJTIwSW4lMjBFdGhlcmV1bSUyME5ld3MlMjBKb2IlMjBMaXN0aW5nJTNBJTIwJTI0NjAwJTIwZm9yJTIwZm91ciUyMGlzc3VlcyUyMCg3NSUyMGNoYXJhY3RlciUyMGxpbWl0KS4lMEQlMEElMEQlMEFNeSUyMHBheW1lbnQlMjByZWNlaXB0JTNBJTIwflJ-JTBEJTBBJTBEJTBBVGhhbmtzIZoBNUFjdGlvbiBSZXF1aXJlZDogQ2xpY2sgdG8gRW1haWwgV2VlayBpbiBFdGhlcmV1bSBOZXdz) **using 3cities.**  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Russian owner of Bitzlato exchange](https://www.justice.gov/usao-edny/pr/founder-and-majority-owner-cryptocurrency-exchange-pleads-guilty-unlicensed-money) pleaded guilty to unlicensed money transmitting \[back in January [US DoJ pre-announced enforcement action](https://twitter.com/thejusticedept/status/1615740967939674116)\]

- [Platypus hackers acquitted](https://content.wrappr.wtf/ipfs/QmRsaTeKrf7QiSS2BhMGGFPFjpiBMbo7MidFRv6jh1FX3b) by Paris court, as deemed smart contract interaction

**General**

- [Governments obtained push notification metadata](https://www.reuters.com/technology/cybersecurity/governments-spying-apple-google-users-through-push-notifications-us-senator-2023-12-06/) from Apple (subpoena) & Google (court order)

- Security self audit: [Telegram](https://securityalliance.notion.site/Telegram-Security-Self-Audit-863507aa2ea84360be8e6f30c61e6b0d) and [Google account](https://securityalliance.notion.site/Google-Security-Self-Audit-6718ff76812f4be5a0e62141c66fa5ec) 

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-9-2023](https://weekinethereumnews.com/week-in-ethereum-news-december-9-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Jan 15 – EF’s [Next Billion fellowship cohort 4](https://fellowship.ethereum.foundation/) deadline

- Feb 2-4 – [ETH Cinco de Mayo](https://ethcincodemayo.com/) hackathon (Cholula, Puebla)

- Feb 23-Mar 3 – [ETHDenver](https://www.ethdenver.com/) BUIDLWeek & hackathon

- Mar 13-14 – [ETHLatam](https://ethlatam.org/) (San Pedro Sula, Honduras)

- Mar 15-17 – [ETHGlobal London](https://ethglobal.com/events/london2024)

- **Mar 19-21 –** [**ETH Canal**](http://ethcanal.xyz) **(Panama City, Panamá)**

- Mar 21-24 – [ETHTaipei](https://ethtaipei.org/) conference & hackathon

- **Mar 27-30 –** [**ETH Bucharest**](https://www.ethbucharest.xyz/) **hackathon & conference**

- Apr 5-26 – ETHGlobal [Scaling Ethereum](https://ethglobal.com/events/scaling2024) (virtual)

- Apr 5-7 – [EthereumZuri.ch](https://ethereumzuri.ch/) conference & hackathon

- May 3-5 – [ETHGlobal Sydney](https://ethglobal.com/events/sydney)

- May 21-23 – [DappCon](https://www.dappcon.io/) (Berlin)

- May 24-26 – [ETHBerlin](https://ethberlin.org/)

- Jul 8-11 – [EthCC](https://www.ethcc.io/) (Brussels)

- Jul 12-14 – [ETHGlobal Brussels](https://ethglobal.com/events/brussels)

- Aug 23-Sep 13 – ETHGlobal [ETHOnline](https://ethglobal.com/events/ethonline2024) (virtual)

- Sep 20-22 – [ETHGlobal Singapore](https://ethglobal.com/events/singapore2024)

- Oct 18-20 – [ETHGlobal San Francisco](https://ethglobal.com/events/sanfrancisco2024)

- Nov – [ETHGlobal DevCon](https://ethglobal.com/events/devcon2024)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

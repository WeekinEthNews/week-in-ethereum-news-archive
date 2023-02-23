---
title: "Week in Ethereum News <br> January 29, 2022"
date: "2022-01-29"
---

## **Eth News and Links**

**Mainnet execution layer**

- Tim Beiko’s [Core Devs Update](https://tim.mirror.xyz/RXwf30VB-Lr4_56w7Kbe-CVXi-L5DuN0Vpfr06Ww5Cs). Apps should prepare for PoW switch off by testing on Kintsugi testnet, EIPs being prioritized for Shanghai upgrade
- Erigon [v2022.01.03](https://github.com/ledgerwatch/erigon/releases/tag/v2022.01.03): improved classification of transactions in the pool, experimental issuance tracking & bug fixes
- Proposal to [charge rollup gas for mainnet to Layer 2 messages](https://ethereum-magicians.org/t/charging-rollup-gas-for-l1-to-l2-messages-extractgas-or-payfromorigin/8104)

**Proof of Stake consensus layer**

- PoS implementers [call video](https://www.youtube.com/watch?v=Bi2qZ2epaPM&t=278s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/rk1gRzgCK): 
    - PoW switch off target of June based on difficulty bomb, focus is on getting switch off right, difficulty bomb can be delayed
    - Kiln (Kintsugi v2) testnet mid-Feb, Engine API & optimistic sync updates
    - Aim for client releases for public testnets mid-March
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220128)
- consensus-specs [v1.1.9](https://github.com/ethereum/consensus-specs/releases/tag/v1.1.9): update for Engine API, full optimistic sync spec, minor refactors & new tests
- Latest Message Driven fork choice [Balancing Attack](https://ethresear.ch/t/balancing-attack-lmd-edition/11853)
- Vitalik: [single-slot proposer/builder separation](https://ethresear.ch/t/single-slot-pbs-using-attesters-as-distributed-availability-oracle/11877) using attesters as distributed availability oracle, alternative to two-slot PBS
- Teku [v22.1.1](https://github.com/ConsenSys/teku/releases/tag/22.1.1): key management API, avoid timeouts in event stream, sync committee optimizations & bug fixes
- Lighthouse [v2.1.1](https://github.com/sigp/lighthouse/releases/tag/v2.1.1): fix for missed attestations with InsufficientPeers error
- Eth-wizard [v0.8.0](https://github.com/stake-house/eth-wizard/releases/tag/v0.8.0): update clients with a single click
- Vitalik: [paths to single-slot finality](https://notes.ethereum.org/@vbuterin/single_slot_finality) (~16 seconds), via super-committees or supporting large number of attesters

**PoW switch off**

- [Super majority client with a consensus bug](https://upgrading-ethereum.info/altair/part2/incentives/diversity#4-client-x-approaches-or-exceeds-two-thirds-of-the-stake) would quickly finalize a broken version of the chain with no chance to intervene, possibly in 13 minutes, leading to all super majority stakers getting slashed
- [Client diversity](https://clientdiversity.org/): stats & client specific instructions on how to switch
- [Community call #3](https://github.com/ethereum/pm/issues/465), Feb 11, for infrastructure providers & app developers
- Guide to setup a [Kintsugi node with Besu+Teku](https://luisnaranjo733.hashnode.dev/want-to-help-test-the-merge-run-a-node-on-kintsugi)

**EIPs/Standards**

- [EIP4721](https://github.com/ethereum/EIPs/blob/fac7ec6ec1ff6c1e25821c7d7ef2b1e8490b73cd/EIPS/eip-draft_tx_expir.md): Transaction Expiration

**Layer2**

- [Arbitrum update](https://twitter.com/bfreshhb/status/1486057303224856578) lowers transaction fees
- [Bybit](https://twitter.com/Bybit_Official/status/1486640127627743235) and [MEXC Global](https://twitter.com/MEXC_Global/status/1485780322176225282) adds support for Arbitrum deposits & withdrawals
- Arbitrum anti-censorship [explainer](https://twitter.com/bkiepuszewski/status/1486416315799769097), transactions can be forced to mainnet after 6545 blocks and 24 hour timeout
- [MoonPay](https://twitter.com/immutable/status/1486869212295360512) adds support for Immutable X ETH purchases with credit cards
- Polygon Hermez documents their [zkEVM opcode-based approach](https://blog.hermez.io/zkevm-documentation/)

* * *

### **This newsletter is made possible thanks to [NEAR](https://near.org/)!**

![NEAR](https://weekinethereumnews.com/wp-content/uploads/2021/10/near_logo_stack.jpg)

NEAR has [launched Simple Nightshade sharding](https://near.org/blog/near-launches-nightshade-sharding-paving-the-way-for-mass-adoption/) to pave the way for greater throughput!

Recently [NEAR launched stake farming](https://medium.com/nearprotocol/near-launches-stake-farming-to-unlock-ecosystem-rewards-e09ae94d8218) for apps to work with staking pools to integrate apps’ tokens into their rewards.  The first launch was with Aurora EVM, so you can now stake $NEAR and be paid in $AURORA.

Learn more about what’s going on in NEAR in the community-driven [NEARweek](https://nearweek.com/) newsletter.

* * *

**Stuff for developers**

- [Models for token deployment](https://hexonaut.medium.com/layer-2-bridges-tokens-and-fungibility-d154986731d3), deploy token root to either mainnet or Layer 2
- ethereum-cryptography [v1.0](https://medium.com/nomic-labs-blog/a-safer-smaller-and-faster-ethereum-cryptography-stack-5eeb47f62d79): 15x smaller, 5 dependencies; [fun details](https://gist.github.com/paulmillr/bff927eb421457c9e2efddd26082cc7a)
- Solidity [gas optimizations](https://gist.github.com/hrkrshnn/ee8fabd532058307229d65dcd5836ddc): use v0.8.4+, calldata function parameters, immutable variables, short revert strings/custom errors & optimize for loops
- [Minimal constructor bytecode](https://twitter.com/k06a/status/1485784061285126145) in a tweet
- [ClonesWithImmutableArgs](https://github.com/wighawag/clones-with-immutable-args): reduces cost of creation & use by replacing storage loads, proxy appends arguments to calldata of delegate call
- [EC20Wrapper](https://forum.openzeppelin.com/t/erc20-wrapper-tutorial/23536) guide, wrap existing ERC20 to add on-chain governance
- [ZKP Private Airdrop](https://github.com/a16z/zkp-merkle-airdrop-contracts): users provide public commitment to later claim using a zk proof that they belong in the Merkle tree 
- [Twitter Airdrop](https://www.polychain.tech/twitter): extract addresses & ENS from drop address Twitter replies
- [Constant Rate Issuance Sales Protocol](https://www.paradigm.xyz/2022/01/constant-rate-issuance-sales-protocol/): increase/decrease NFT sale price to meet target rate, collaboration with Justin Roiland (Rick & Morty co-creator)
- [Solidity Metadata Playground](https://twitter.com/SourcifyEth/status/1487005088975671298): decode metadata hash, view verified contracts on Sourcify/Etherscan, open in Remix if verified
- [c4udit](https://github.com/byterocket/c4udit): simple Solidity analyzer, regular expressions for low severity issues
- Tenderly [Simulator](https://blog.tenderly.co/mempool-simulated/): access any pending transaction with expected outcomes
- [Group signature primitive using zkSNARKs](https://0xparc.org/blog/zk-group-sigs), proof of concept message board where identity of poster can’t be narrowed beyond the group

**Security**

- [OpenSea uncanceled listings](https://thedefiant.io/opensea-listing-bug/) used to buy NFTs below market rates, listings valid until canceled by a transaction, listing [cancels](https://twitter.com/dingalingts/status/1486654437548773376) are being front run
- Multichain bridge [post mortem](https://media.dedaub.com/phantom-functions-and-the-billion-dollar-no-op-c56f062ae49f), relied on a tokens permit function reverting but WETH doesn’t have permit & the fallback function doesn’t revert
- Qubit Ethereum BSC Bridge $80 million [exploit](https://certik.medium.com/qubit-bridge-collapse-exploited-to-the-tune-of-80-million-a7ab9068e1a0), insufficient checks allowed withdraw of tokens on BSC using a 0 ETH deposit with malicious data
- ZORA [fixed price sale vulnerability](https://zora.mirror.xyz/JeFZXnWb6jfJPon1rruXW-XJcoUVfgeNhu4XTYO3yFM), seller could increase price & front run purchase, no funds lost, fix uses explicit buy price
- Austin Williams: [two contracts from BoringSolidity](https://mirror.xyz/onewayfunction.eth/-ctBALK2996RmFHCtBrE0joVKT774gaihGBD8gTZVJM) when imported together allow ETH to be drained; safe contracts may become unsafe when combined 

**Ecosystem**

- [Ethereum.org](https://blog.ethereum.org/2022/01/24/the-great-eth2-renaming/) removed all uses of ETH2 terminology, Ethereum is execution layer + consensus layer, renaming doesn’t change Ethereum roadmap
- [Blockscan chat](https://chat.blockscan.com/), off-chain instant messaging, Etherscan address view shows unread message count, not currently end-to-end encrypted, beta

**Application layer**

- Aave [v3](https://aave.mirror.xyz/MwzcAtfUn2OeHyGZ9Ma4ah5LNM3te3OpG8OUMTIRdKw) on testnets (Rinkeby, Arbitrum Rinkeby and Optimism Kovan)
- Opyn Squeeth [crab strategy](https://medium.com/opyn/automated-squeeth-strategies-the-crab-strategy-is-now-live-b92281ebe701) live, for sideways market (narrow range price fluctuation)
- Rari Capital [Fuse](https://twitter.com/RariCapital/status/1485661611838877699) live on Arbitrum
- Maple [Loans v2](https://maplefinance.medium.com/introducing-loans-v2-a-more-flexible-and-capital-efficient-maple-finance-54ac1c1fa9), refinancing & liquidation tools for capital efficiency and reduced gas costs
- [Pika Protocol](https://pikaprotocol.medium.com/pika-protocol-is-officially-launched-on-optimism-mainnet-116eedb9cb01) perpetual swap exchange live on Optimism, gradual rollout with increasing cap
- Syndicate [Web3 Investment Clubs](https://syndicate.mirror.xyz/4p6a0nKpBYMSxoAfN6KpjcUwJSD2t68Dq7zgoliB4pk), each club can have 99 members, invite-only, can’t charge carry, public beta 
- Risk Harbor [v2](https://medium.com/riskharbor/risk-harbor-core-v2-now-live-on-ethereum-mainnet-7411e58bc328) live on mainnet, includes levered vaults, AMM & risk engine
- Suggestion to [replace USDC blacklist](https://alexkroeger.mirror.xyz/RJ1gZ8tAfqXOmfA3MJz0AkD082c-3hwr2lba-F1j3uw) with admin function to freeze balances, save 2100 gas for each check
- ZORA [v3](https://zine.zora.co/zora-v3): NFT marketplace protocol adds instant royalties, finder’s fee, non-custodial listings and fee governance right as an NFT
- [Reservoir](https://reservoir.mirror.xyz/cW3-xUuLpqpfYmTMZhfTowOrJssEL_iSThuNoUmMpxE): NFT order book protocol
- [MoonPay NFT Checkout](https://www.moonpay.com/business/nfts) supports card purchases
- [OpenSea reversed 50 item limit](https://twitter.com/opensea/status/1486843201352716289) for their free minting tool after backlash, 80% of items created are plagiarized works, fake collections or spam
- [ENS voted](https://discuss.ens.domains/t/ep5-executable-set-the-temporary-premium-start-price-to-100-000/9336) to set expired name start price premium to $100k to prevent names being snapped up by bots, premium decays to $0 over 28 days
- [on-chain art](https://www.0xchain.art/): NFT showcase, rated by how data is stored and rendered

* * *

### **Job Listings**

- [Re7 Capital](https://www.re7.capital/) – a DeFi yield fund – is hiring [analysts and data engineers](https://apply.workable.com/re7-capital/)
- Ether Capital is hiring a 👩🏼‍💻 [DevOps Engineer](https://bit.ly/ethcapdevops) 👨🏻‍💻 to stake millions on Eth2
- Geth team seeks [Senior Technical Writer](https://ethereum.bamboohr.com/jobs/view.php?id=51&source=weekinethnews) to redo the docs & take ownership
- Nethermind 1-3 month [internship program](https://nethermind.notion.site/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1)
- Are you a p2p networking whiz? EF research hiring [Networking Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=54&source=weekinethnews)

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US proposed America COMPETES Act](https://www.coincenter.org/new-bill-would-hand-treasury-blank-check-to-ban-crypto-at-exchanges/) would allow US Treasury to prohibit types of transactions deemed a money laundering concern without public notice or comment
- [US SEC proposed amendments](https://lexnode.substack.com/p/urgent-considerations-of-impact-on) to Exchange Act expand definition of securities exchange
- [Diem](https://www.coindesk.com/business/2022/01/27/diem-to-sell-assets-to-silvergate-bank-for-200m-report/) reported to be selling their tech to Silvergate Capital for $200 million
- [Wonderland/Abracadabra/FrogNation CFO](https://thedefiant.io/frog-nation-cfo-quadrigacx/) found to be QuadrigaCX co-founder Michael Patryn

**General**

- [Trezor](https://blog.trezor.io/a-decision-on-aopp-789540c2930b) backtracks and removes Address Ownership Proof Protocol
- Joe Grand [hacked Trezor wallet](https://www.theverge.com/2022/1/24/22898712/crypto-hardware-wallet-hacking-lost-bitcoin-ethereum-nft) to rescue $2 million in funds
- Vitalik: [soulbound items](https://vitalik.eth.limo/general/2022/01/26/soulbound.html), limit transferability of NFTs by binding to an ENS name or proof of humanity, non-transferable items can be private
- PwnKit: [Linux local privilege escalation exploit](https://blog.qualys.com/vulnerabilities-threat-research/2022/01/25/pwnkit-local-privilege-escalation-vulnerability-discovered-in-polkits-pkexec-cve-2021-4034) in polkit’s pkexec
- [Download of a users Amazon data](https://twitter.com/AlinaUtrata/status/1485194962027388929), includes audio speaking to Alexa 

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-january-29-2022](https://weekinethereumnews.com/week-in-ethereum-news-january-29-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- **Feb 11 – PoW switch off [community call](https://github.com/ethereum/pm/issues/465)**
- Feb 15 - Apr 5 – [Cryptocurrency Class](https://mirror.xyz/0xaFaBa30769374EA0F971300dE79c62Bf94B464d5/oGqGP2NOK9g7QPl1sMKkzql_Fh0P6hKbpYLZ-EkQTXU) (virtual) 
- Feb 17 – [Schelling Point](https://schellingpoint.gitcoin.co/) (Denver) 
- Feb 18-20 – [ETHDenver](https://www.ethdenver.com/)
- **Feb 23 - Mar 11 – [Codeless Conduct](https://codelessconduct.org/) no-code hackathon (virtual)**
- Mar 11-16 – [Ethereum Rio](https://www.ethereum.rio/)
- Mar 17-18 – [ETH Austin](https://2022.ethaustin.org/) summit
- Mar 29-31 – [ETHDubai](https://www.ethdubaiconf.org/)
- Apr 7-9 – [ETH Portland](https://2022.ethportland.com/) hackathon
- Apr 20-21 – [The Alliance (gaming) summit](https://medium.com/1kxnetwork/announcing-alliance-summit-7e8732c9fd9d) (Amsterdam)
- Apr 21 – [ETHconomics](https://ef-events.notion.site/ETHconomics-Devconnect-676d73f791684e18bfae35bbc9e1fa90) (Amsterdam)
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- May 3-8 – [spaghettETH](http://spaghett-eth.com/) (Milan)
- May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 16-19 – [ETH Miami](https://2022.eth-miami.com/) summit & hackathon
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETHNewYork](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

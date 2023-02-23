---
title: "Week in Ethereum News <br> October 23, 2021"
date: "2021-10-23"
---

## **Eth News and Links**

**Mainnet execution layer**

- PoW switch off [community call](https://github.com/ethereum/pm/issues/402) November 5, for infrastructure providers and application developers
- Geth [v1.10.11](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.11): fixes pending transaction retrieval RPC and snapshot corruption bug
- [Stateless Ethereum cheat sheet](https://notes.ethereum.org/@gballet/Sy-a6T5St): current state of verkle trees, address space extension and state networks
- Piper Merriam’s [Aperture Portal Network update](https://snakecharmers.ethereum.org/the-aperture-vol-2/): State Network testnet coming, agreed on a wire protocol, considering using libp2p and an ultra light client in the browser

**EIPs/Standards**

- Summary of EIPs for [signing and identity](https://blog.spruceid.com/ethereum-identity-review-of-eips-over-time/), informing EIP4361 Sign-in with Ethereum

**Proof of Stake consensus layer**

- **UPDATE YOUR NODES BEFORE OCT 27**.   
    Danny Ryan’s [Finalized](https://blog.ethereum.org/2021/10/19/finalized-no-30/) reminder: if you don’t update, you’ll get penalties
    - Teku [v21.10.1](https://github.com/ConsenSys/teku/releases/tag/21.10.1): support different ports for TCP and UDP, fixes Windows incompatibility introduced in v21.10.0
    - Lighthouse [v2.0.1](https://github.com/sigp/lighthouse/releases/tag/v2.0.1): fix for discovery that could cause unexpected shutdown
    - Prysm [v2.0.2](https://github.com/prysmaticlabs/prysm/releases/tag/v2.0.2): bug fixes
    - Nimbus [v1.5.2](https://github.com/status-im/nimbus-eth2/releases/tag/v1.5.2): fixes and optimizations
- 46% nodes ready for Altair upgrade ([nodewatch.io](https://www.nodewatch.io/))
- Visualization of [client diversity](https://twitter.com/sproulM_/status/1451065804183662592) change over time.  It got worse in the last year, but is now slowly improving.
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_211022)
- [PoS implementers call](https://youtu.be/5vGxLoTUqaQ?t=68). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/HyjI-xy8K): teams working on issues and stability of Pithos testnet, Prysm can now sync with Pithos, beacon chain upgrade as part of PoW switch off needs a name
- Pithos testnet [consensus monitor](https://pithos.consensus-monitor.stokes.io/)
- Three [reorg and liveness attacks](https://arxiv.org/abs/2110.10086) on staking fork choice rule

**Layer2**

- [Optimism upgrade](https://twitter.com/optimismpbc/status/1451339513964359682) to EVM equivalence delayed until November 11
- Celer cBridge [v2.0 testnet](https://twitter.com/celernetwork/status/1450249124331155458): improved user experience and LPs have option not to run a cBridge node, mainnet mid November
- [Springrollup](https://ethresear.ch/t/springrollup-a-zk-rollup-that-allows-a-sender-to-batch-an-unlimited-number-of-transfers-with-only-6-bytes-of-calldata-per-batch/11033) proposal for zk rollup where sender can batch unlimited number of transfers with only 6 bytes of calldata
- [Private AMM](https://ethresear.ch/t/why-you-can-build-a-private-uniswap-with-weak-secrecy-in-zkrollup/11031) proposal with weak secrecy using a zkRollup
- Comparison of [Arbitrum and Optimism’s fraud proofs](https://medium.com/@cpbuckland88/fraud-proofs-and-virtual-machines-2826a3412099) 
- Systematisation of knowledge of [validating bridges](https://stonecoldpat.github.io/images/validatingbridges.pdf) \[PDF\]

* * *

### **This newsletter is made possible thanks to [Nexus Mutual](https://nexusmutual.io/)!**

![Nexus Mutual](https://weekinethereumnews.com/wp-content/uploads/2021/07/Screenshot-from-2021-07-30-18-52-32.png)

Yield farming or deploying on L2? Nexus Mutual's Protocol Cover keeps you protected. Coverage includes all L2 deployments in addition to the regular main chain coverage. What about multi-chain? We've got you covered for that as well.

Sleep without worrying.  [Get coverage](https://app.nexusmutual.io/cover) today. 

* * *

**Stuff for developers**

- js-ethereum-cryptography [v0.2.0](https://github.com/ethereum/js-ethereum-cryptography/releases/tag/v0.2.0): cryptographic primitives, 15x smaller with 3 dependencies, experimental, awaiting security audit
- [prb-proxy](https://github.com/paulrberg/prb-proxy): execute multiple calls in one transaction, modern DSProxy with deterministic proxy addresses and 3rd party permissions
- [smart-batched-auction](https://github.com/FrankieIsLost/smart-batched-auction) for ERC721, implementation of Paradigm's NFT launch design
- [template-ethereum-contracts](https://github.com/wighawag/template-ethereum-contracts): Solidity template with Hardhat deploy, updated with dapptools tests
- [starkex-clientlib-js](https://github.com/starkware-industries/starkex-clientlib-js): JavaScript wrapper of StarkEx API
- [starknet-devnet](https://github.com/Shard-Labs/starknet-devnet/): Flask wrapper of Starknet dummy network
- [Ethernal](https://blog.tryethernal.com/ethernal-is-going-open-source/) block explorer for private chains, open sourced, adds free and paid ($20/mo) hosted tiers
- [pool-sniper](https://github.com/Anish-Agnihotri/pool-sniper): Uniswap v2 pool creation sniper
- [13 lessons](https://ethresear.ch/t/13-dev-takeaways-from-developing-the-usm-stablecoin/11020) from developing USM stable token

**Security**

- Polygon Plasma bridge [double spend vulnerability](https://medium.com/immunefi/polygon-double-spend-bug-fix-postmortem-2m-bounty-5a1db09db7f1):
    - $2 million bounty paid
    - Exit transaction could be resubmitted 223 times
    - ~$850 million was at risk
- Unlock Protocol’s [UDT vulnerability](https://unlock-protocol.com/blog/udt-disclosure), token could be burnt for any address, contract has since been upgraded
- [Indexed Finance](https://hackmd.io/@d1ll0n/Hyd-uCuBK) identified attacker, details being provided to law enforcement after expiry of request to return 90% of funds
- Hot wallet [private key committed to Git](https://steviep.xyz/txt/compromised): NFTs rescued via gasless private zero ETH sales and using Flashbots

**Ecosystem**

- [gasprice.io](https://www.gasprice.io/): gas price estimates with visualizations of recent and monthly prices and transaction pool analysis
- ETHOnline [finalists](https://twitter.com/ethglobal/status/1449883260457209857)
- LisCon [videos](https://vimeo.com/user155155490)
- Parity 2017 multisig hack of 153k ETH now worth ~$600 million, [hacker asked to return 90%](https://medium.com/parity-hack-trace/a-message-to-the-ethereum-community-and-parity-multisig-wallet-hacker-3596bbc4fd38) of funds

**Enterprise**

- [Associated Press](https://www.ap.org/press-releases/2021/ap-chainlink-to-bring-trusted-data-onto-leading-blockchains) providing economic, sports and election data via Chainlink
- Facebook’s [Novi](https://scontent.fmel14-2.fna.fbcdn.net/v/t39.2365-6/245645778_229514682497390_5814575696636412345_n.pdf?_nc_cat=102&ccb=1-5&_nc_sid=ad8a9d&_nc_ohc=vMfQUa02-cIAX8jNxEr&_nc_ht=scontent.fmel14-2.fna&oh=318c76fab87d62faa88d1a9dfe135627&oe=61744796) \[PDF\] wallet piloting in US and Guatemala with USDP (Paxos) held in [Coinbase Custody](https://blog.coinbase.com/coinbase-to-power-crypto-custody-for-facebooks-novi-90dc8d3f5830)

**Application layer**

- DeFi has [$100 billion in TVL](https://twitter.com/defipulse/status/1450846435688202248)
- [PoolTogether v4](https://twitter.com/PoolTogether_/status/1449050529146064904): single prize pool across Ethereum and sidechains, rather than siloed
- [Worldcoin](https://worldcoin.org/how-it-works): iris scans using zk proofs (Semaphore) on Hubble optimistic rollup 
- Kwenta testnet [futures trading competition](https://blog.kwenta.io/kwenta-decentralized-perpetual-futures-competition-is-now-live/)
- [Decentralized Gitcoin Grants](https://grants.gtcdao.net): quadratic funding grants protocol
- [Sismo](https://blog.sismo.io/what-is-sismo-part-1-zk-badges-73e7031bacda): aggregate reputation on public profile without giving away all your accounts using zk attestations
- [Paperhands](https://twitter.com/iblamenfts/status/1450769400370384899): check current floor price of NFTs you sold
- [Tellie](https://www.producthunt.com/posts/tellie): creator sites with token gated content
- [DAO](https://medium.com/lexdaoism/when-daos-get-real-managing-real-property-on-a-blockchain-83f43f55da53) owning and managing a real life farm

* * *

### **Job Listings**

- [Team Lead](https://ethereum.bamboohr.com/jobs/view.php?id=43&source=weekinethnews) for the Ecosystem Support Program at the Ethereum Foundation
- [Senior Engineer @Gitcoin](https://angel.co/company/gitcoin/jobs) - build the future of public goods funding!
- Solidity is [hiring a C++ dev](https://ethereum.bamboohr.com/jobs/view.php?id=40&source=weekinethnews)
- Nomic Labs hiring a [Tech Lead for Hardhat VSCode](https://nomiclabs.notion.site/Senior-Software-Engineer-Hardhat-VSCode-23cfe4ccf56846ada207c83e3a2830c3)

**Reach people experienced with Ethereum.**  $420 for two issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [New York Attorney General](https://ag.ny.gov/press-release/2021/attorney-general-james-directs-unregistered-crypto-lending-platforms-cease) directs two lending platforms to cease activities in New York and three others to provide info on their activities; [failure to redact names](https://twitter.com/lefterisjp/status/1450121889368641537) suggests Nexo was sent a cease letter and Celsius was sent an info request
- Australian Senate committee [crypto regulation recommendations](https://www.aph.gov.au/Parliamentary_Business/Committees/Senate/Financial_Technology_and_Regulatory_Technology/AusTechFinCentre/Final_report/section?id=committees%2freportsen%2f024747%2f78047) covering regulatory structure for DAOs, capital gains tax events and CDBCs
- [Epic](https://twitter.com/TimSweeneyEpic/status/1449146317129895938) welcomes games making use of blockchain (unlike Steam)
- NFTs more efficient at [signaling cultural fluency](https://twitter.com/sershokunin/status/1450477846590332929?s=20) than traditional art
- PleasrDAO purchased [Wu-Tang Clan’s unreleased album](https://pleasr.mirror.xyz/PTzSIYe6LbNW55i_Jo4S_fgqIiDp3d7YblpikQ1iRks) from US DoJ

**General**

- ECFFT on the BN254 base field [implemented in Rust](https://solvable.group/posts/ecfft-bn254/)
- [Google Threat Analysis Group](https://blog.google/threat-analysis-group/phishing-campaign-targets-youtube-creators-cookie-theft-malware/): phishers target YouTube creators with cookie theft non-persistent malware in a smash-and-grab
- New York Times: [Sneaker flippers](https://www.nytimes.com/interactive/2021/10/15/style/sneaker-bots.html) using bots
- Argentina’s [National Registry of Persons](https://therecord.media/hacker-steals-government-id-database-for-argentinas-entire-population/) allegedly hacked, identity data of entire country could be at risk
- 3.1 million [email addresses from CoinMarketCap](https://twitter.com/haveibeenpwned/status/1451650181552750594) were being traded

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-october-23-2021/](https://weekinethereumnews.com/week-in-ethereum-news-october-23-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Oct 25 - Dec 13 – [Gitcoin DAO Global hackathon](https://gitcoin.co/hackathon/dao-global/onboard) (virtual)
- Oct 27 – Beacon chain upgrade to Altair [epoch 74240](https://blog.ethereum.org/2021/10/05/altair-announcement/); **EthStaker viewing [party](https://twitter.com/superphiz/status/1450528521391157251)** 
- Oct 28-29 – [ETH Portland](https://2021.ethportland.com/) hackathon
- Nov 1-4 – [NFT.NYC](https://www.nft.nyc/)
- **Nov 5 – PoW switch off [community call](https://github.com/ethereum/pm/issues/402)**
- **Nov 11 – [Optimism upgrade](https://twitter.com/optimismPBC/status/1451339513964359682)**
- Dec ~8 – [Arrow Glacier](https://github.com/ethereum/execution-specs/blob/master/network-upgrades/mainnet-upgrades/arrow-glacier.md) upgrade block 13,773,000
- **Jan 24-26 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford University)**
- Mar 28-30 – [ETHDubai](https://www.ethdubai.xyz/)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

---
title: "Week in Ethereum News <br> December 3, 2022"
date: "2022-12-03"
---

## **Eth News and Links**

**Layer 1**

- Discussion of [upgrade naming schemes](https://ethereum-magicians.org/t/rfc-post-merge-network-upgrade-naming-schemes/11977)
- Latest consensus layer [call video](https://www.youtube.com/watch?v=KFc1sWYlVZ4&t=106s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/Sk2SWNLPs) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-consensus-layer-call-99-writeup/):
    - EIP4844 is not in the same readiness as withdrawals, so is being worked on in parallel & specified separately from Capella upgrade, to not delay withdrawals
- EIP4844 implementer call [notes](https://twitter.com/terencechain/status/1597640854742917121): CL teams working on passing spec tests & sync protocol, EL teams rebasing on top of fork by timestamp, devnet 3 now expected next week
- [EOF v1 checklist](https://notes.ethereum.org/@ipsilon/eof1-checklist) with summary of EIP implementations
- [Shandong testnet](https://twitter.com/efjavascript/status/1598323497939378180) deprecated

**For stakers**

- New MEV-Boost non-censoring relays: 
    - [ultra sound](http://relay.ultrasound.money) by ultra sound money
    - [agnostic](http://agnostic-relay.net) by GnosisDAO
    - (instructions from Flashbots on how to [run a relay](https://flashbots.notion.site/Running-mev-boost-relay-at-scale-4040ccd5186c425d9a860cbb29bbfe09))
- [Ephemery project](https://ethereum-magicians.org/t/ephemery-project-an-ephemeral-testnet/11955) to create an ephemeral testnet for testing staking setups
- [Full node on $365 hardware](https://twitter.com/EthereumOnARM/status/1597889744821944320) using Rock 5B board

**Research**

- [Optimal attestation packing](https://lighthouse-blog.sigmaprime.io/optimising-attestation-packing.html), existing Lighthouse greedy approximation algorithm produced optimal solution 52.3% and within 5% of optimal 99.97%

**Client releases**

- Consensus Layer:
    - Nimbus [v22.11.0](https://github.com/status-im/nimbus-eth2/releases/tag/v22.11.0): production ready separate validator client
- Execution Layer:
    - Besu [v22.10.1](https://github.com/hyperledger/besu/releases/tag/22.10.1): performance improvements via database caching, sync fixes & logging improvements, reduced memory consumption and RPC additions

**Layer 2**

- Christine Kim: [overview of zkEVMs](https://www.galaxy.com/research/whitepapers/zkevms-the-future-of-ethereum-scalability/)

**EIPs/Standards**

- [EIP6046](https://github.com/ethereum/EIPs/pull/6046/files): Replace SELFDESTRUCT with DEACTIVATE
- [EIP6047](https://github.com/ethereum/EIPs/pull/6047/files): Balance accountable via event for ERC721
- [EIP6049](https://eips.ethereum.org/EIPS/eip-6049): Deprecate SELFDESTRUCT
- [EIP6051](https://github.com/ethereum/EIPs/pull/6051/files): Private key encapsulation
- [EIP6059](https://github.com/ethereum/EIPs/pull/6059/files): Parent-governed nestable NFTs
- [EIP6065](https://github.com/ethereum/EIPs/pull/6065/files): Real estate token
- [EIP6066](https://github.com/ethereum/EIPs/pull/6066/files): Signature validation method for NFTs

* * *

### **This newsletter is made possible thanks to Starbloom Ventures!**

![Starbloom Ventures](https://weekinethereumnews.com/wp-content/uploads/2021/11/Screenshot-from-2021-11-19-15-25-51.png)

Starbloom Ventures is a first round venture fund founded by Evan Van Ness to invest in the future of web3.

* * *

**Stuff for developers**

- [Ropsten testnet](https://blog.ethereum.org/2022/11/30/ropsten-shutdown-announcement) is shutting down, Rinkeby is next; app devs should use Sepolia
- PRBMath [v3](https://twitter.com/PaulRBerg/status/1597645509094649856): user defined value types SD59x18 & UD60x18, free functions (defined outside of contracts), typed assertions for use in Foundry tests, MIT license
- [Blacksmith](https://github.com/blacksmith-eth/blacksmith#readme): generates front end for interacting with contracts in Foundry projects
- [Foundry <> Python differential fuzz testing template](https://twitter.com/Jib0xD/status/1596878625105592321): useful for quantitative finance contract development
- [RareSkills](https://www.rareskills.io/test-yourself) 40 question timed Solidity test; [Tincho got 77.5%](https://www.youtube.com/watch?v=tpekiuASieo) \[video\]
- Guide to [how contracts are constructed](https://blog.smlxl.io/evm-contract-construction-93c98cc4ca96) & deployed
- [EVM storage diagram](https://twitter.com/blainemalone/status/1597352375593078784) of how it is structured & accessed
- [evmc](https://github.com/joshstevens19/evmc#readme): fetch verified Solidity from Etherscan and load in IDE
- [interface.fyi](http://interface.fyi): UI for mainnet contracts including unverified & without ABI
- [Sample contract deployment pipeline](https://github.com/spalladino/sample-contract-deploy-pipeline#readme) using GitHub Actions, Hardhat & OpenZeppelin Defender; proof of concept
- [Basement API](https://mirror.xyz/0x25B2B8458BAB283d465996df38305333C75982B6/uYsldHeef7FxVcBI233QSYzje4ejiQu0SMVdY74vf1s): fetch contracts, wallet and NFT data
- [Liberte](https://github.com/michael1011/liberte#readme): replace Infura with your own node

**Security**

- 88mph [vulnerability disclosed](https://medium.com/immunefi/88mph-theft-of-unclaimed-mph-rewards-bugfix-review-1dec98b9956b), unclaimed rewards could be drained from vesting contract

**Ecosystem**

- Despite Twitter jokes, [WETH (wrapped Ether) cannot depeg](https://twitter.com/eulerfinance/status/1597280990770376705), unlike other wrapped assets
- Chainlist reports [RPC privacy](https://twitter.com/0xngmi/status/1596586588448116736)
- [ETHGasStation](https://twitter.com/ETHGasStation/status/1597341610777317376) is shutting down; [gasprice.io](https://www.gasprice.io/) is a decent alternative

**Enterprise**

- [Stripe fiat onramp](https://stripe.com/en-au/blog/crypto-onramp), US only initially
- [Maersk discontinuing TradeLens](https://www.maersk.com/news/articles/2022/11/29/maersk-and-ibm-to-discontinue-tradelens) (built on Hyperledger Fabric) after 4 years 

**Application layer**

- [Compound set borrowing caps](https://twitter.com/rleshner/status/1598123050301788160) on 10 assets in response to CRV-borrowing attack against Aave
- Maker [Dai Savings Rate (DSR)](https://twitter.com/MakerDAO/status/1598350198383656960) increasing to 1%
- [Eth.co](https://eth.co/): add .co to .eth ENS to view links, NFTs, ENS domains and profile
- [Set ENS avatar](https://twitter.com/gregskril/status/1598384620646850560): mint an image and set the profile pic NFT as your avatar
- Uniswap [NFT marketplace aggregator](https://uniswap.org/blog/uniswap-nft-aggregator-announcement) live on mainnet
- [Coinbase Wallet forced to remove NFT transfers on iOS](https://twitter.com/CoinbaseWallet/status/1598354819735031809) as Apple wanted transaction fees paid via in-app purchase (to collect their 30%)

* * *

### Job Listings

- [Code integration tester](https://jobs.lever.co/ethereumfoundation/6feeb8cb-bd05-4f24-9fda-9ba3be98e5a4) wanted by Ethereum Foundation
- EF Robust Incentives Group seek a [research scientist](https://jobs.lever.co/ethereumfoundation/cd2382ec-abbd-493b-b942-b5e2a61a6c0a)

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [BlockFi](https://blockfi.com/November28-ClientUpdate) filed for bankruptcy
- US Senate [committee hearing on FTX](https://twitter.com/adamscochran/status/1598332447241998337); Blockchain Association sent [FTX failure memo](https://theblockchainassociation.org/wp-content/uploads/2022/11/The-Failure-of-FTX-International-Nov-30-2022-1.pdf) \[PDF\]
- [Kraken settled with OFAC](https://home.treasury.gov/policy-issues/financial-sanctions/recent-actions/20221128) for $360k after geoblocking onboarding but not transactions
- [Proposal to pilot Uniswap fee switch](https://gov.uniswap.org/t/fee-switch-pilot-update-vote/19514), with input from Uniswap Foundation
- Vitalik calls out [governance rights as a token value](https://twitter.com/vitalikbuterin/status/1597570120456769536) narrative
- Alex Van de Sande: [instant run-off voting](https://mirror.xyz/avsa.eth/4pvULeQRqWCS8mMnk_UY1THYt3p6tEQNL0JkCzflcd0) is hard to visualize, with chaotic results
- [Overview of digital fashion](https://medium.com/1kxnetwork/augmenting-culture-the-emerging-field-of-digital-fashion-bead627c8dcd): digiphysical, AR & direct-to-avatar wearables

**General**

- [Intel SGX attacks](https://sgx.fail/): Secret Network vulnerability disclosed, past transactions may not be private
- [LastPass customer info accessed](https://blog.lastpass.com/2022/11/notice-of-recent-security-incident/) in second security incident

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-december-3-2022](https://weekinethereumnews.com/week-in-ethereum-news-december-3-2022)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Dec 5 – [EF Layer 2 grants](https://esp.ethereum.foundation/layer-2-grants) deadline
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)
- **Mar 15-16 –** [**ETHDubai**](https://www.ethdubaiconf.org/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

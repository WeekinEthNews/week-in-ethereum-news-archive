---
title: "Week in Ethereum News <BR> March 7, 2021"
date: "2021-03-07"
---

## **Eth News and Links**

**Mainnet**

- Geth [v1.10](https://blog.ethereum.org/2021/03/03/geth-v1-10-0/) - snap sync is shipped, though not yet enabled as nodes need to build the structure necessary for snap sync. That structure makes pruning relatively quick and gets you back to a database size of a fresh sync. Snapshots also make DOS attacks harder and increase database read capacity of node. Adds eth/66 and will drop eth/64 soon and eth/65 in the summer
- [EIP1559 scheduled for the London hard fork](https://hackmd.io/@timbeiko/1559-updates/https%3A%2F%2Fhackmd.io%2F%40timbeiko%2F1559-update-008), likely in July when the difficulty bomb goes off.
- Latest [core devs call](https://youtu.be/xWfR-WxjmYg?t=137), Beiko’s [notes](https://twitter.com/TimBeiko/status/1367836983628824576). Removed EIP2315 (EVM subroutines) for Berlin
- Proposal for increasing [address size from 20 to 32 bytes](https://ethereum-magicians.org/t/increasing-address-size-from-20-to-32-bytes/5485)
- [Weak statelessness and/or state expiry coming soon](https://www.reddit.com/r/ethereum/comments/lw7ug3/weak_statelessness_andor_state_expiry_coming_soon/)
- Better [bidding with EIP1559](https://barnabe.substack.com/p/better-bidding-with-eip1559)
- An [econ analysis of EIP1559](https://medium.com/coinmonks/economic-analysis-of-eip-1559-a-summary-afac46533928), a blog post summary of Tim Roughgarden’s paper

**EIPs/Standards**

- [ERC3085](https://eips.ethereum.org/EIPS/eip-3085): Wallet add Eth chain RPC method (‘wallet\_addEthereumChain’)
- [EIP3322](https://eips.ethereum.org/EIPS/eip-3322): Account gas storage opcodes
- [EIP3332](https://github.com/ethereum/EIPs/blob/17a68f2c1ce94319253ca52f54a83b9cf59e31d2/EIPS/eip-3332.md): `MEDGASPRICE` Opcode
- [ERC3338](https://eips.ethereum.org/EIPS/eip-3338): Limit account nonce to 2^52
- [EIP3336](https://eips.ethereum.org/EIPS/eip-3336): Paged memory allocation for the EVM
- [EIP3337](https://eips.ethereum.org/EIPS/eip-3337): Frame pointer support for memory load and store operations

**Proof of Stake**

- [Commit to pre-state](https://ethresear.ch/t/commit-to-pre-state-instead-of-post-state-on-the-executable-beacon-chain/8802) instead of post-state when we turn off PoW
- A toy example of calculating [data recovery](https://hackmd.io/@benjaminion/data_recovery)
- [Mousse](https://medium.com/@ethereum-mousse/mousse-an-ethereum-2-0-emulator-for-local-testing-of-eth2-applications-19af727519ce), an eth2 emulator for local testing

**Layer2**

- Hermez [zk-rollup is on Rinkeby testnet](https://blog.hermez.io/hermez-testnet-is-now-public/)
- [Cross-rollup dex design](https://ethresear.ch/t/cross-rollup-dex-with-smart-contracts-only-on-the-destination-side/8778) even if only the destination rollup has EVM support

* * *

### **This newsletter is made possible thanks to Chainlink!**

![](https://weekinethereumnews.com/wp-content/uploads/2020/05/FE39n5_g.png)

Chainlink’s biggest hackathon yet is right around the corner! Join us from March 15 to April 11 to compete for $80k+ in prizes, learn from industry-leading mentors, and build with others across the community. 

[Register today to secure your spot.](https://chain.link/hackathon?utm_source=this-week-in-eth&utm_medium=newsletter&utm_campaign=hackathon)

* * *

**Stuff for developers**

- [Expectations for breaking changes for Eth devs](https://www.reddit.com/r/ethereum/comments/lx32kv/expectations_for_backwardsincompatible_changes/)
- Solidity [v0.8.2](https://blog.soliditylang.org/2021/03/02/solidity-0.8.2-release-announcement/), inliner from post immediately below, custom NatSpec and exported documentation
- Saving [gas with simple inlining](https://blog.soliditylang.org/2021/03/02/saving-gas-with-simple-inliner/)
- Hardhat [v2.1](https://medium.com/nomic-labs-blog/increased-mining-flexibility-in-hardhat-network-1fa2707ebd38), a transaction pool implementation that fully mimics geth
- Zero configuration for [Hardhat and Typechain](https://twitter.com/krzKaczor/status/1368276886959263745)
- [Load balancing freemium Ethereum endpoints](https://chasewright.com/load-balancing-freemium-ethereum-endpoints/) with Dshackle
- A walkthrough of [ERC3156 flash loan standard](https://soliditydeveloper.com/eip-3156)
- [WETH10](https://twitter.com/r_ross_campbell/status/1366535538300379136) is on mainnet

**Security/incidents**

- Avoiding npm attacks with Metamask’s [Lavamoat](https://medium.com/metamask/how-metamasks-latest-security-tool-could-protect-smart-contract-developers-from-theft-e12da346aa53)
- Finding [evil go packages](https://michenriksen.com/blog/finding-evil-go-packages/), npm-style
- A security framework for [SNARKy ceremonies](https://eprint.iacr.org/2021/219)
- [PaidNetwork rugpull](https://twitter.com/FrankResearcher/status/1367905172798795777), founders claim that admin address was hacked
- There was a [BSC rugpull](https://www.rekt.news/meerkat-finance-bsc-rekt/) as well for 31m, also with ex-post dubious founder claims
- The blow-by-blow of warroom events to [save Primitive finance](https://medium.com/immunefi/inside-the-war-room-that-saved-primitive-finance-6509e2188c86), and the big bounties paid in return
- Fiona Kobayashi’s [guide to troubleshooting Flashbots](https://fifikobayashi.medium.com/beginners-guide-to-troubleshooting-mev-on-flashbots-aee175048858)
- [Curve v1](https://twitter.com/CurveFinance/status/1367576697122525191) pools have a bug, please withdraw liquidity
- A [browser-based side channel attack via CSS](https://orenlab.sise.bgu.ac.il/p/PP0)

**Ecosystem**

- MetaMask’s [custom networks API](https://consensys.net/blog/metamask/connect-users-to-layer-2-networks-with-the-metamask-custom-networks-api) for layer2 and EVM sidechains
- You can use [Chainlist](https://chainlist.org/) to easily add a new chain to MetaMask, though it is a [trusted 3rd party](https://twitter.com/danfinlay/status/1367513890599309313)
- Rate-limiting nullifiers in [Waku v2 messaging (eg, Whisper replacement) for spam protection](https://vac.dev/rln-relay) without compromising privacy
- Ethereum Foundation [rollup grant applications](https://esp.ethereum.foundation/en/rollup-grants/) are due April 16.

**Enterprise**

- AWS Managed Blockchain now has [Eth node general availability](https://aws.amazon.com/about-aws/whats-new/2021/03/announcing-general-availability-of-ethereum-on-amazon-managed-blockchain/)
- [Aon pilot of tokenized “placement of insurance”](https://btcmanager.com/global-insurance-heavyweight-blockchain-pilot/)
- PayPal CEO says they’re [experimenting with building on Ethereum](https://decrypt-co.cdn.ampproject.org/c/s/decrypt.co/60086/paypal-ceo-schulman-talks-new-crypto-unit?amp=1)
- HK public company [Meitu buys $22m ETH and $18m BTC](https://www.coindesk.com/software-firm-meitu-buys-22m-of-ether-17-9m-bitcoin-for-its-treasury)

**The NFT application layer**

- Indie band Kings of Leon [issuing an NFT for new album](https://www.rollingstone.com/pro/news/kings-of-leon-when-you-see-yourself-album-nft-crypto-1135192/)
- Jack Dorsey is [selling his first tweet](https://v.cent.co/tweet/20) on Cent
- Grimes sells [NFTs for $6-7m](https://niftygateway.com/profile/grimes)
- Even the Associated Press is selling an [NFT of its US presidential call](https://opensea.io/assets/0x9fc4e38da3a5f7d4950e396732ae10c3f0a54886/1)
- Burning a [Banksy artwork to sell it as an NFT](https://twitter.com/BurntBanksy)

**Regulation/business/tokens**

- 1400 Florence, 1920 Paris, 2021 Ethereum: a [new framework for art](https://felipether.medium.com/%EF%B8%8F-ethereums-artistic-renaissance-77de62df1a69)
- Coinbase’s “[rise of the Ethereum economy](https://www.coinbase.com/learn/market-updates/deep-dive-ethereum-economy)”
- Nobody cares about [decentralization until they need it](https://defited.medium.com/my-centralized-experience-dapper-3d3e3a99cbd7), a user’s story of getting locked out of his TopShot account
- McAfee [indicted on fraud and money laundering](https://www.justice.gov/usao-sdny/pr/john-david-mcafee-and-executive-adviser-his-cryptocurrency-team-indicted-manhattan) in pump and dumps
- JP Koning: is [DeFi undoing Tether’s network effects](https://jpkoning.blogspot.com/2021/03/tether-bigger-badder-paypal.html)?

**General**

- Nick Johnson hacks [Cobo Vault hardware wallet](https://weka.medium.com/defeating-the-cobo-vault-pros-self-destruct-mechanism-abf321e2f5b5), something easily possible on Ledger and Trezor as well
- [Brave Search](https://brave.com/brave-search/): buys Tailcat to make privacy-first search engine
- Adler: cryptoeconomic [blockchain bridges are not trust-minimized](https://talk.lazyledger.org/t/on-the-trustedness-of-cryptoeconomic-bridges/44)

* * *

## **Job Listings**

- [Switchain](https://www.switchain.com/) is looking for a [VP of Business Development](https://cryptocurrencyjobs.co/sales/switchain-vp-of-business-development/). Remote, full-time
- At the edge of blockchain R&D. [Rust](https://chainsafe.io/careers/openpositions/rust-developer), [Golang](https://chainsafe.io/careers/openpositions/lead-golang-developer), [Solidity](https://chainsafe.io/careers/openpositions/solidity-engineer). [Join ChainSafe](https://chainsafe.io/careers/openpositions)!
- Trail of Bits is looking for a [blockchain security engineer](https://jobs.lever.co/trailofbits/4f459855-3299-462f-9e73-299a840d5baf)
- 0x: [devs of all types](https://0x.org/about/jobs) and a [data analyst](https://boards.greenhouse.io/0x/jobs/4220949002)
- ethereum.org is [hiring a front end dev](https://ethereum.bamboohr.com/jobs/view.php?id=32)

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-march-7-2021/](https://weekinethereumnews.com/week-in-ethereum-news-march-7-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **Mar 8 - [Statelessness and state expiry](https://github.com/ethereum/pm/issues/268) call**
- Mar 10-25 - [Gitcoin CLR matching grants](https://gitcoin.co/grants/) round
- Mar 19-21 - ETHGlobal’s [NFT Hack](https://nft.ethglobal.co/)
- Apr 9 - May 14 - ETHGlobal’s [Scaling Ethereum](https://scaling.ethglobal.co/) hackathon
- April 14 - [Berlin upgrade fork](https://github.com/ethereum/pm/issues/248#issuecomment-782069875) (testnets: Ropsten Mar 10, Goerli Mar 17, Rinkeby Mar 24)
- **April 16 - [Rollup community grant](https://esp.ethereum.foundation/en/rollup-grants/) applications due**
- **April 22 - [Ethereum in the Enterprise 2021](https://www.conference2021.entethalliance.org/)**
- May 14 - papers due for [WoSCA 2021](https://trailofbits.github.io/WoSCA/)
- Jul 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

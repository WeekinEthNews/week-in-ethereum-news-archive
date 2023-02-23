---
title: "Week in Ethereum News <br> October 8, 2022"
date: "2022-10-07"
---

## **Eth News and Links**

**Execution layer**

- [Account abstraction](https://twitter.com/vitalikbuterin/status/1576199517434949634) via ERC4337 + EIP3074 + EIP5003 + [transaction inclusion lists](https://notes.ethereum.org/@vbuterin/account_abstraction_roadmap#Transaction-inclusion-lists)
- EIP4844 (proto-danksharding): [arithmetic hash alternatives to KZG](https://ethresear.ch/t/arithmetic-hash-based-alternatives-to-kzg-for-proto-danksharding-eip-4844/13863) are possible but with a lot of tradeoffs
- Besu [v22.7.5](https://github.com/hyperledger/besu/releases/tag/22.7.5): fix for empty block proposals & RPC defect
- Erigon [v2.27.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.27.0): experimental [embedded consensus layer client](https://giulioswamp.substack.com/p/erigon-embedded-consensus-module), change to [semantic versioning](https://erigon.substack.com/p/big-release-and-renaming-of-erigon)
- Nethermind [v1.14.3](https://github.com/NethermindEth/nethermind/releases/tag/1.14.3): reduces missed attestations; [upcoming features](https://twitter.com/m25marek/status/1578057260248465408)
- Proposal to [add blockTimestamp to logs](https://ethereum-magicians.org/t/proposal-for-adding-blocktimestamp-to-logs-object-returned-by-eth-getlogs-and-related-requests/11183) returned by eth\_getLogs
- [Second stage findings](https://github.com/imapp-pl/gas-cost-estimator/blob/master/docs/gas-cost-estimator.md) of gas cost estimation research using marginal execution cost

**Consensus layer**

- Mitigate centralization risks by [constraining builder power](https://ethresear.ch/t/how-much-can-we-constrain-builders-without-bringing-back-heavy-burdens-to-proposers/13808) and minimize proposer responsibilities via partial block auctions (inclusion lists or proposer suffixes)
- MEV-Boost development process [discussion](https://collective.flashbots.net/t/toward-an-open-research-and-development-process-for-mev-boost/464)
- Flashbots [plan towards decentralized block building](https://twitter.com/bertcmiller/status/1577482296629739520)
- Jon Charbonneau: [Flashbots could reduce censorship](https://joncharbonneau.substack.com/p/censorship-wat-do) by open sourcing their builder or adding a cap
- Nimbus [v22.10.0](https://github.com/status-im/nimbus-eth2/releases/tag/v22.10.0): faster block production, added metrics
- ethStaker [Goerli testnet validator deposit](https://goerli.launchpad.ethstaker.cc/en/) updated to only require 0.0001 GoETH

**EIPs/Standards**

- [EIP5744](https://github.com/ethereum/EIPs/pull/5744/files): Latent fungible token
- [EIP5748](https://github.com/ethereum/EIPs/pull/5748/files): Approval expiration for ERC20 tokens
- [EIP5749](https://eips.ethereum.org/EIPS/eip-5749): The 'window.evmproviders' object
- [EIP5750](https://github.com/ethereum/EIPs/pull/5750/files): Extra data parameter in methods
- [EIP5753](https://github.com/ethereum/EIPs/pull/5753/files): Lockable extension for ERC721
- [EIP5757](https://github.com/ethereum/EIPs/pull/5757/files): Process for approving external resources

**Layer 2**

- Norswap compares [Optimism Bedrock and Arbitrum Nitro](https://norswap.com/bedrock-vs-nitro/)
- Polynya: [rollups can offer higher throughput than Layer 1s](https://polynya.mirror.xyz/zYV0g6II0iREbcaph8362sRBC2_a2hm6NlKj1-yuh6Q) as rollups need fewer nodes

### **This newsletter is made possible thanks to** [**Nexus Mutual**](https://nexusmutual.io/)**!**

![Nexus Mutual Protocol Cover](https://weekinethereumnews.com/wp-content/uploads/2022/03/Nexus-Mutual-Protocol-Cover-1024x586.png)

The yield is still out there.  When you discover the next opportunity make sure you don’t get rekt. 

Protect yourself against: 

- hacks with Protocol Cover 
- depegging with Yield Token Cover
- CeFi blow-ups with Custody Cover 

Maximize yield. Minimize Risk. Enjoy peace of mind knowing Nexus Mutual has you covered. Become a member and [protect your assets](https://app.nexusmutual.io/cover) against the major risks in crypto.

* * *

**Stuff for developers**

- [Reminder](https://twitter.com/TimBeiko/status/1577301427051167748): Rinkeby & Ropsten testnets are deprecated, use Goerli & Sepolia
- Remix [v0.27.0](https://medium.com/remix-ide/remix-ide-v0-27-0-release-77ea40f9914b): sync HardHat/Truffle/Foundry compilation with Remixd, OpenZeppelin template customization, autocomplete import statements and code formatting
- [Foundry Canary](https://github.com/ZeframLou/foundry-canary#readme): example deploy script
- Remco [exp & ln](https://xn--2-umb.com/22/exp-ln/index.html): exponential function & natural logarithm in Solidity
- 0age tip: [view Yul assembly of your Solidity](https://twitter.com/z0age/status/1578443864217554945) using compiler irOptimized setting
- [Useful Solidity patterns](https://github.com/dragonfly-xyz/useful-solidity-patterns#readme): self contained examples with Foundry tests
- [CREATE3 Factory](https://github.com/ZeframLou/create3-factory#readme): deploy a contract with the address based on deployer & salt
- [HyVM](https://github.com/oguimbal/HyVM#readme): EVM Hypervisor in Huff, allows arbitrary bytecode execution
- samczsun’s [transaction viewer](https://tx.eth.samczsun.com/#txhash=0x3443cd8f0c722fa9d83e12033f29eb590b177804ae625f2072625dfb79b329c2); front end [open sourced](https://github.com/samczsun/ethereum-transaction-viewer-frontend#readme)
- [Ethereum utils](https://eth-utils.com): unit conversion, checksum, hex & Keccak256
- Guide to [fuzzing with Echidna](https://blog.pessimistic.io/fuzzing-solidity-smart-contracts-with-echidna-die-hard-level-tips-9ab7033fa893), attempts to break user-defined invariants
- Transpose [SQL](https://www.transpose.io/blogs/introducing-transpose-sql): direct SQL access to indexed blockchain data
- [MEV Template](https://github.com/DeGatchi/mev-template-rs#readme): MEV bot in Rust
- Slither [v0.9.0](https://github.com/crytic/slither/releases/tag/0.9.0): adds arbitrary-send-erc20, arbitrary-send-erc20-permit & domain-separator-collision detectors and reduces false positives
- [Noir](https://medium.com/@aztecnetwork/ff43f38d86d9): Aztec’s Rust-based language for creating and verifying zk proofs
- [Circom-Next-Starter](https://github.com/Darlington02/circom-next-starter#readme): zk app starter kit using Hardhat, Circom, Snarkjs & Nextjs

**Security**

- [$566 million exploit of BSC token hub](https://www.bnbchain.org/en/blog/bnb-chain-ecosystem-update/) (bridge between BNB beacon chain & BSC):
    - 2 million BNB minted using [forged messages verified by the bridge](https://twitter.com/samczsun/status/1578167198203289600)
    - [$110 million bridged](https://twitter.com/certikalert/status/1578300670544936960) to other chains
    - BSC chain halted then [upgraded to freeze accounts](https://github.com/bnb-chain/bsc/releases/tag/v1.1.15) & disable BSC token hub transfers
- Transit Swap cross-chain DEX [$28.9 million exploit](https://rekt.news/transit-swap-rekt/), approved tokens were transferred using arbitrary external call, attacker was [front run for $1 million by arb bot](https://twitter.com/SlowMist_Team/status/1576488479357214721)

**Ecosystem**

- Devcon [manual](https://blog.ethereum.org/2022/10/04/devcon-manual), [passport app](https://app.devcon.org/) (mobile friendly PWA) and [schedule](https://app.devcon.org/schedule)
- clr.fund [LatAm quadratic funding round](https://ethcolombia.clr.fund/) during Devcon

**Application layer**

- [Maker DAO $1 million bond investment pilot](https://twitter.com/MakerGrowth/status/1578093187016822784); aims to invest $500 million, 80% in US Treasury & 20% in corporate bonds
- [DeFi Saver Compound v3 support](https://blog.defisaver.com/compound-v3-support-live-defisaver-automation-notifications/) with automation and notifications
- [Aztec integrates Euler](https://twitter.com/aztecnetwork/status/1576997493987868672) using ERC4626 bridge
- Liquity [Chicken Bonds](https://www.chickenbonds.org/blog-posts/chicken-bonds-is-live) live on mainnet, dynamic NFT represents bond
- [Adrastia oracle](https://blog.adrastia.io/introducing-adrastia-833c83006412) live on mainnet, Optimism & Arbitrum; price aggregated from DEXs weighted by liquidity
- Endaoment [v2](https://twitter.com/endaomentdotorg/status/1578126164064960518) adds portfolios and composability
- Etherscan’s [Blockscan chat](https://twitter.com/etherscan/status/1577667362744020992) adds end-to-end encryption (for signed in addresses), contract address sign-in, browser notifications and alpha recipes SDK

* * *

### **Job Listings**

- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)
- [Join Llama](https://zenith-caboc-8a4.notion.site/Join-Llama-ad66be1cb28541f5b5346aa37d192b79) to help build the future of protocol DAOs: [Solidity](https://zenith-caboc-8a4.notion.site/Smart-Contract-Engineer-ef9426f7cfef4f0d90b596aaeff216e0) and [Backend](https://zenith-caboc-8a4.notion.site/Senior-Backend-Engineer-6a096e7937c248f4a90fba08c3bf14ae)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)

**Job listings: $600** for four issues (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US CFTC allowed to serve notice to Ooki DAO](https://www.coindesk.com/policy/2022/10/05/second-crypto-group-objects-to-cftcs-use-of-chat-bot-to-serve-legal-papers/) via help bot & forum post, LeXpunK & DeFi Education Fund filed to submit amicus briefs
- [EU Commission Russian sanctions](https://twitter.com/EU_Commission/status/1577951963781767168) adds ban on all crypto wallets & custody services
- [Kim Kardashian $1.26 million settlement with US SEC](https://www.sec.gov/news/press-release/2022-183) for promoting a token on Instagram without disclosing payment received
- [Celsius filing](https://twitter.com/sniko_/status/1578320508021374977) included users full name and deposit/withdrawal amounts
- [Cloudflare IPFS gateway](https://twitter.com/liamzebedee/status/1577525264963100674) blocks Tornado Cash
- DeFiLlama [dashboard of project raises](https://defillama.com/raises)

**General**

- [Chromium application mode](https://mrd0x.com/phishing-with-chromium-application-mode/) allows for creation of phishing applications
- Australian telco [Optus confirms 2.1 million customers](https://www.bleepingcomputer.com/news/security/optus-confirms-21-million-id-numbers-exposed-in-data-breach/) had identity document numbers exposed

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-october-8-2022](https://weekinethereumnews.com/week-in-ethereum-news-october-8-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Oct 11-14 – [Devcon 6](https://devcon.org/) (Bogotá)
- **Oct 14 –** [**Flashbots MEV workshop**](http://flashbots.net/devcon)
- Oct 14 – [Semaphore grants](https://esp.ethereum.foundation/semaphore-grants) deadline
- Oct 18-23 – [Eth Medellin](https://www.ethmedellin.co/) (Colombia)
- **Oct 21 – Clr.fund** [**LatAm round**](https://ethcolombia.clr.fund/) **ends**
- Oct 26-28 – [Eth Panama](https://www.ethpanama.com/)
- Oct 28-30 – [ETH Lisbon](https://www.ethlisbon.org/)
- Oct 31 – [Merge data challenge](https://esp.ethereum.foundation/merge-data-challenge) deadline
- Nov 3 – US Treasury [digital assets RFC](https://public-inspection.federalregister.gov/2022-20279.pdf) \[PDF\] deadline
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 11-13 – [ETHBrno](https://mirror.xyz/ethbrno.eth/6BH9cUVuD85hy5O0L5cOOOE7niSA9Yo5eWsXVzKOlO4) (Czech Republic)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Nov 25-27 – [ETH Vietnam](https://www.eth-vietnam.com/)
- **Nov 26-30 –** [**ETH Miami**](https://ethmiami.net/)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

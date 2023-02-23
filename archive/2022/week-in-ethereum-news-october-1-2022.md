---
title: "Week in Ethereum News <br> October 1, 2022"
date: "2022-10-01"
---

## **Eth News and Links**

**Execution layer**

- Besu [v22.7.4](https://github.com/hyperledger/besu/releases/tag/22.7.4): fix for memory leak
- EIP4844 (proto-danksharding) [call video](https://www.youtube.com/watch?v=Oc_e7YJQl-I&t=13s), [notes](https://docs.google.com/document/d/1KgKZnb5P07rdLBb_nRCaXhzG_4PBoZXtFQNzKO2mrvc/edit) and [readiness checklist](https://github.com/ethereum/pm/blob/master/Breakout-Room/4844-readiness-checklist.md)

**Consensus layer**

- Lighthouse [v3.1.2](https://github.com/sigp/lighthouse/releases/tag/v3.1.2): optional payload pruning to reduce execution node timeouts and optimizations to attestation & block processing
- bloXroute's ethical MEV-Boost relayer [produced invalid blocks](https://twitter.com/blink_labs_xyz/status/1575022763232075778)
- Danny Ryan’s notes on [not coupling Beacon blocks & blobs](https://notes.ethereum.org/RLOGb1hYQ0aWt3hcVgzhgQ?view) for EIP4844

**EIPs/Standards**

- [EIP5719](https://github.com/ethereum/EIPs/pull/5719/files): Signature replacement interface
- [EIP5725](https://github.com/ethereum/EIPs/pull/5725/files): Transferable vesting NFT
- [EIP5727](https://github.com/ethereum/EIPs/pull/5727/files): Semi-fungible soulbound token
- [EIP5732](https://github.com/ethereum/EIPs/pull/5732/files): Simple commit interface

* * *

### **This newsletter is made possible thanks to** [**Hardhat**](https://hardhat.org/)**!**

![](https://weekinethereumnews.com/wp-content/uploads/2021/06/hardhat-rectangle-1024x325.png)

The Hardhat for Visual Studio Code extension adds language support for Solidity to Visual Studio Code, and provides editor integration for Hardhat projects.

It supports:

- Code completion
- Go to definition, type definition and references
- Symbol renames
- Solidity code formatting
- Inline code validation from compiler errors/warnings for Hardhat projects
- Hover help for variables, function calls, errors, events etc.
- Code actions (quick fixes) suggested from compiler errors/warnings for Hardhat projects
- Implement missing functions on interface with stubs
- Constrain mutability by adding view/pure to function signature
- Meet inheritance requirements by adding virtual/override on function signature
- Provide accessibility by adding public/private to function signature

Get it from the [VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=NomicFoundation.hardhat-solidity)

* * *

**Stuff for developers**

- [Solbase](https://github.com/Sol-DAO/solbase#readme) (Solidity library): adds ERC2612 permit extensions to ERC20/721/1155
- [Solidity Array Generators](https://github.com/mds1/solidity-generators#readme): Solidity functions to generate evenly spaced arrays, linspace, arange & logspace, designed for testing, not optimized
- [Bit Magic](https://saxenism.com/web3/solidity/language-tricks/bit-magic/intermediate/2022/09/06/Bit-Magic-Solidity.html): guide to bit manipulation in Solidity
- Paul R Berg’s Solidity tip: [function calls with named parameters](https://docs.soliditylang.org/en/latest/control-structures.html#function-calls-with-named-parameters)
- [GitHub Action to run Solidity unit tests](https://medium.com/remix-ide/solidity-unit-tests-via-a-github-action-9fd129b89349) using Remix
- Vyper [v0.3.7](https://github.com/vyperlang/vyper/releases/tag/v0.3.7): isqrt & epsilon built-ins, block.prevrandao, public constant & immutable variables
- [Serpentor](https://github.com/yearn/serpentor#readme): Vyper on-chain voting and governance contracts
- Huffmate [v1](https://github.com/pentagonxyz/huffmate/releases/tag/v1): Huff contract library, unaudited
- [evm2](https://github.com/hananbeer/evm2#readme): EVM that runs inside EVM
- ctc [v0.3.0](https://twitter.com/notnotstorm/status/1574214692834115585): Python package & CLI for historical data analysis
- [WhatsABI](https://github.com/shazow/whatsabi#readme): guesses ABI from an address via 4-byte JUMPI instructions; [web app](https://abi.w1nt3r.xyz/)
- Heimdall [v0.1.5](https://github.com/Jon-Becker/heimdall-rs/releases/tag/0.1.5): adds decompile, generates ABI for functions, events & errors, beta
- Vitalik’s [Py\_plonk](https://github.com/ethereum/research/tree/master/py_plonk#readme): SNARK (PLONK) compiler, prover and verifier in Python
- Raul Jordan: [intro to functional programming](https://rauljordan.com/2022/09/25/blog-series-functional-programming-for-blockchain.html)
- Ethernaut DAO CTF [vulnerable NFT solution](https://stermi.xyz/blog/ethernautdao-ctf-vnft-solution)

**Security**

- MEV bot 0xbaD [1,101 ETH exploit](https://twitter.com/bertcmiller/status/1574852628030361609) after ~800 ETH arbitrage, attacker used flash loan callFunction implementation to set WETH allowance
- [Wintermute private key reconstructed](https://medium.com/amber-group/exploiting-the-profanity-flaw-e986576de7ab) on a 16GB Macbook M1 in less than 48 hours

**Ecosystem**

- [Core developers based in 18 countries](https://cointelegraph.com/news/7-ethereum-developers-would-like-to-sell-you-on-the-merge): 20.7% USA, 9.1% Germany, 7.4% UK
- [MEV Stats](https://mev.metablock.dev/1/dashboard) grouped by type & protocol, search & MEV leaderboards
- ETHOnline [finalists](https://ethglobal.medium.com/ethonline-2022-5fbb126ed72c)
- Vitalik’s [Proof of Stake book](https://twitter.com/vitalikbuterin/status/1574837986633682949) released

**Enterprise**

- [Christie’s](https://twitter.com/ChristiesInc/status/1574794644642304007?s=20&t=Qurl59eH10h-zdGpg7LM4Q) v3.0: on-chain NFT auction platform
- [Facebook users in US](https://about.fb.com/news/2022/05/introducing-digital-collectibles-to-showcase-nfts-instagram) can post their NFTs
- Reserve Bank of Australia [piloting CBDC on Quorum private Ethereum](https://www.rba.gov.au/payments-and-infrastructure/central-bank-digital-currency/pdf/australian-cbdc-pilot-for-digital-finance-innovation-white-paper.pdf) \[PDF\]

**Application layer**

- [OpenSea adds Optimism NFTs](https://twitter.com/opensea/status/1574799977649422339), creators need to setup royalties
- [Public Nouns](https://twitter.com/publicnouns/status/1575408052064305152): Nouns derivative supporting public goods
- [Skiff ethereum.email address](https://skiff.com/blog/ethereum-wallet-email) for wallets and ENS
- [delegate.cash](https://0xfoobar.substack.com/p/delegatecash): on-chain registry of delegations from cold wallets to hot wallets
- [Safe](https://safe.mirror.xyz/p1aonqM1NSZeOFN8iY2_Ms8y6Ikuz5E76HRiEPKnCEA) (formerly Gnosis Safe) to be governed by SafeDAO, token now claimable
- [Gemini proposal](https://forum.makerdao.com/t/gusd-makerdao-partnership-announcement/18140) for MakerDAO to hold GUSD

* * *

### **Job Listings**

- [Join Llama](https://zenith-caboc-8a4.notion.site/Join-Llama-ad66be1cb28541f5b5346aa37d192b79) to help build the future of protocol DAOs: [Solidity](https://zenith-caboc-8a4.notion.site/Smart-Contract-Engineer-ef9426f7cfef4f0d90b596aaeff216e0) and [Backend](https://zenith-caboc-8a4.notion.site/Senior-Backend-Engineer-6a096e7937c248f4a90fba08c3bf14ae)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Remix: [frontend React/Typescript dev](https://jobs.lever.co/ethereumfoundation/2c293808-48ed-4994-b0e0-14a8986e6ff3)
- [Bobhub](https://bobhub.xyz/) multichain oracle is hiring a [Technical writer](https://bobhub.gitbook.io/bobhub/)!

**Job listings: $600** for four issues (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Ooki DAO forum post](https://forum.ooki.com/t/cftc-v-ooki-dao-case-no-3-22-cv-05416-tsh/453) attempts to serve notice in US CFTC case, [DAO has 21 days to respond or risk default judgment](https://twitter.com/lex_node/status/1574903583132327951)
- [US SEC charges Hydrogen Technology & former CEO](https://www.sec.gov/news/press-release/2022-175) for market manipulation
- [Reversible tokens](https://mirror.xyz/kaili.eth/gB-rx89sNAT3CVuxWo6xVFS5ptNcllW7cVWVCfcFa6k) proposal using decentralized judiciary to reverse or reject; foobar [argues for finality](https://0xfoobar.substack.com/p/why-finality-matters)
- [History of gaming](https://www.galaxy.com/research/whitepapers/history-of-gaming-and-web3-future/) and future for web3

**General**

- [zkBridge paper](https://rdi.berkeley.edu/zkp/zkBridge/zkBridge.html): uses zk-SNARKs to prove validity of block headers on remote chains
- [Construct an efficient zk-proof for keccak](https://blog.polygon.technology/zk-white-paper-efficient-zk-proofs-for-keccak/) using arithmetization

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-october-1-2022](https://weekinethereumnews.com/week-in-ethereum-news-october-1-2022)

* * *

## **Upcoming Dates of Note**

_(new/changes in_ **_bold_**_)_

- Oct 6-8 – [Web3 Lagos](https://event.web3bridge.com/)
- Oct 7-16 – [Devcon week](https://devcon.org/en/devcon-week/) (Bogotá)
- Oct 7-9 – [ETHBogotá](https://bogota.ethglobal.com/) (ETH Global)
- Oct 7-9 – [Infinite hackathon](https://infinite-hackathons.eth.limo/) (Bogotá)
- Oct 11-14 – [Devcon 6](https://devcon.org/) (Bogotá)
- Oct 14 – [Semaphore grants](https://esp.ethereum.foundation/semaphore-grants) deadline
- Oct 18-23 – [Eth Medellin](https://www.ethmedellin.co/) (Colombia)
- Oct 26-28 – [Eth Panama](https://www.ethpanama.com/)
- Oct 28-30 – [ETH Lisbon](https://www.ethlisbon.org/)
- Oct 31 – [Merge data challenge](https://esp.ethereum.foundation/merge-data-challenge) deadline
- Nov 3 – US Treasury [digital assets RFC](https://public-inspection.federalregister.gov/2022-20279.pdf) \[PDF\] deadline
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 11-13 – [ETHBrno](https://mirror.xyz/ethbrno.eth/6BH9cUVuD85hy5O0L5cOOOE7niSA9Yo5eWsXVzKOlO4) (Czech Republic)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Nov 25-27 – [ETH Vietnam](https://www.eth-vietnam.com/)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive this newsletter weekly_**

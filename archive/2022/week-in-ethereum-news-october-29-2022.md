---
title: "Week in Ethereum News <br> October 29, 2022"
date: "2022-10-29"
---

## **Eth News and Links**

**Layer 1**

- Latest core devs [call video](https://www.youtube.com/watch?v=oQfEW8LdE88&t=445s). Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1585406583278047235) & [Christine Kim](https://www.galaxy.com/research/insights/ethereum-all-core-developers-call-148/):
    - Shanghai upgrade scope to be finalized over the next month, could be split into two upgrades
    - Shanghai will include [withdrawals + EIP3651 (warm COINBASE), EIP3855 (PUSH0) & EIP3860 (limit & meter initcode)](https://github.com/ethereum/execution-specs/pull/633/files)
    - EIP4844 (proto-danksharding) & EOF being worked on in parallel, may be included in Shanghai depending on specs being finalized & implementation complexity
    - EIP1153 (transient storage) & EIP4758 (deactivate SELFDESTRUCT) are potential inclusions
    - Timestamp as upgrade trigger to be tested on Shanghai devnet
    - Discussion on eth/68 (announce transactions with type & size rather than gossip them)
- Consensus specs [v1.3.0-alpha.0](https://github.com/ethereum/consensus-specs/releases/tag/v1.3.0-alpha.0): adds withdrawal test vectors
- EIP4844 proto-danksharding:
    - EIP4844 implementers [call video](https://www.youtube.com/watch?v=hAa1b4m7tsI&t=9s) and [notes](https://docs.google.com/document/d/15EatedrJanNxBZGPVASvwq9xgbTs5UxjsDfjpM6ppSY/edit)
    - [Blobscan](https://www.blobscan.com/): testnet blob explorer
    - Protolambda: [blobspace](https://twitter.com/protolambda/status/1584105020697432064), history of sharding design
    - [.oO](https://twitter.com/adietrichs/status/1585465506370408448): danksharding meme; blobs will get bigger over time
- Jim McDonald: [impact of MEV-Boost relays](https://www.attestant.io/posts/exploring-the-impact-of-mev-relays/), 3% decrease in correct attestations for relayed blocks versus locally built blocks
- Flashbot’s [sync-proxy](https://collective.flashbots.net/t/open-sourcing-sync-proxy/626): beacon node requests proxied to multiple execution layer clients

**Research**

- Proposal to [burn MEV](https://ethresear.ch/t/burning-mev-through-block-proposer-auctions/14029) via block proposer auctions; Hasu [argues](https://collective.flashbots.net/t/to-burn-or-not/647) that it isn’t viable

**Client releases**

- Consensus Layer:
    - Lighthouse [v3.2.1](https://github.com/sigp/lighthouse/releases/tag/v3.2.1): patch for v3.2.0 to fix ~80ms increase in block import times
    - Prysm [v3.1.2](https://github.com/prysmaticlabs/prysm/releases/tag/v3.1.2): bug fixes & improvements
    - Teku [v22.10.2](https://github.com/ConsenSys/teku/releases/tag/22.10.2): fixes & optimisations

**Layer 2**

- zkSync [v2.0](https://blog.matter-labs.io/baby-alpha-has-arrived-5b10798bc623) deployed; apps will be able to deploy later this year, opens to users next year
- EF $750k [Layer 2 grants round](https://esp.ethereum.foundation/layer-2-grants) to support applications, analytics and education
- Arbitrum Nova [Etherscan block explorer](https://nova.arbiscan.io/)
- Scroll: [KZG and polynomial commitment schemes](https://scroll.io/blog/kzg) explainer

**EIPs/Standards**

- [EIP5827](https://github.com/ethereum/EIPs/pull/5827/files): Auto-renewable allowance extension
- [EIP5843](https://github.com/ethereum/EIPs/pull/5843/files): EVM modular arithmetic extensions

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
- Constrain mutability by adding view/pure to function signature
- Meet inheritance requirements by adding virtual/override on function signature
- Provide accessibility by adding public/private to function signature

Get it from the [VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=NomicFoundation.hardhat-solidity)

* * *

**Stuff for developers**

- Foundry: [guide to add a cheat code](https://twitter.com/gakonst/status/1584000626010165248) (in a single tweet)
- ERC4626 (tokenized vaults) [property tests](https://a16zcrypto.com/generalized-property-tests-for-erc4626-vaults/) to check for conformance, using Foundry
- Nethereum [v4.11.0](https://github.com/Nethereum/Nethereum/releases/tag/4.11.0) (.NET) adds EVM simulator to preview state changes
- RareSkills [Distribute gas optimizor CTF solution](https://mirror.xyz/vicnaum.eth/gZPBJoJm4Ne3eXhxR-x7bbh8oFLnJ2JyVzczq2n9H8M)
- WalletConnect [Sign v2.0](https://medium.com/walletconnect/walletconnect-sign-v2-0-the-final-release-is-here-864b21e8d1ca) production release, [v1 will be deprecated](https://twitter.com/walletconnect/status/1585297184102047744) March 1, 2023; [Auth](https://medium.com/walletconnect/introducing-walletconnect-auth-one-click-wallet-login-to-simplify-web3-ux-9cc11fd18aba): one-click login
- [0xShip](https://twitter.com/nazar_ilamanov/status/1585055440123359232): contract vs contract battleship game, Goerli testnet, similar to 0xMonaco

**Security**

- Team Finance [$15.8 million exploit](https://rekt.news/teamfinance-rekt/), via Uniswap v2 to v3 migrate function
- Layer2DAO [exploit](https://twitter.com/llamaintern/status/1583935286332911616), 50 million tokens stolen from Optimism address of multisig
- FriesDAO [$2.3 million exploit](https://twitter.com/CertiKAlert/status/1585764826025975809?s=20&t=AEGqQtd4d_DGyMp5ldqM4w), deployer private key generated using Profanity

**Ecosystem**

- Discussion to [fix Goerli testnet supply issues](https://ethereum-magicians.org/t/testnet-workgroup-paths-out-of-the-goerli-supply-mess/11453)
- Ethereum.org [Q4 roadmap](https://github.com/ethereum/ethereum-org-website/issues/8399)
- OpenSea [old Wyvern approvals](https://twitter.com/PocketUniverseZ/status/1585793457385140225) can be used to steal NFTs in malicious transactions

**Enterprise**

- Google offers managed [Eth node hosting](https://cloud.google.com/blog/products/infrastructure-modernization/introducing-blockchain-node-engine)

**Application layer**

- MakerDAO ratification vote was in favor (pending executive vote) of [custodying up to $1.6b of USDC at Coinbase for 1.5% annual interest](https://www.coinbase.com/blog/coinbase-launches-usdc-institutional-rewards-program-with-makerdao)
- [Uniswap v3 TWAP oracles in PoS](https://uniswap.org/blog/uniswap-v3-oracles) research: mitigate risk with wide-range liquidity
- 0xSplits [liquid splits](https://0xsplits.mirror.xyz/vTrce7rS1odZPOvtBfrxqNWluu2h9cJoIyUZ7nqhvNw): split ownership represented with transferable NFTs
- [LooksRare](https://twitter.com/LooksRare/status/1585647538635689985) NFT marketplace replaced creator royalties with 0.5% fee
- [Sound Market](https://sound.mirror.xyz/X3hChH1-Ipu2OXaZL4vrcgd9JrwMOEznu2-SuagiJlY): dedicated music NFT marketplace, aggregates listings
- [Llamalend](https://twitter.com/0xngmi/status/1585709182807744512) NFT lending protocol live

* * *

### Job Listings

- EF are hiring a [code integration tester](https://jobs.lever.co/ethereumfoundation/6feeb8cb-bd05-4f24-9fda-9ba3be98e5a4)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- [Research scientist](https://jobs.lever.co/ethereumfoundation/cd2382ec-abbd-493b-b942-b5e2a61a6c0a) wanted for EF Robust Incentives Group

**Job listings: $600 for four issues** (75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet or Layer 2. [Pay with one click](https://3cities.xyz/#/pay?c=H4sIAHqco2IAAyXOMU6EQBSA4atMqVbAgGjJuqzGmI3JrrHcDMODnQAz5L03ERsTLey9gtJop8bGUk-xt5HE4m-__A_vPbreEZRZjQAdWH58ZZeVJQLR7iAYQglFKeNYVipJ0mQR5EWYSpCRnB_F4fEijZPopJqFz5v-Z9xg3_-O1jHsTq8BGmGsyHkLCL4TS7ghce4KcWGIja1F5XDKozBEHkjs3aWJ0FuFSjOgaE1neP-jdbXRqs2IgNdGN4AvV6v5t-qct5zRzNRL3xWAZzCsGCf3LRgiqWV8GASfxKgY6ttLhGq6sBro_otdA_afygfdejLO0tM4qes_d-LI2xABAAA) using 3cities.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Apple app store guidelines](https://twitter.com/wongmjane/status/1584609845570768897) allows NFT sales but must pay Apple’s 30%
- [ARCx token going private](https://arcx.substack.com/p/the-next-phase-of-arcx), token holders can be bought out otherwise the token will be frozen
- [Music NFTs shouldn’t link to music](https://scarceobjects.substack.com/p/keep-music-out-of-music-nfts), they should focus on non-copyright revenues

**General**

- Matt Levine’s [40,000 word _Bloomberg Businessweek_ cover story](https://www.bloomberg.com/features/2022-the-crypto-story/) on why crypto is interesting
- Vitalik’s [Revenue-evil Curve](https://vitalik.eth.limo/general/2022/10/28/revenue_evil.html) argues that subsidies for public goods should focus on reducing the pressure to monetize where the marginal monetization most hurts the user experience
- [Flookup](https://eprint.iacr.org/2022/1447.pdf): gets closer to when complex >32 bit operations can be done directly via lookup in snarks
- [Hashing](https://geometry.xyz/notebook/Hashing-to-the-secp256k1-Elliptic-Curve) to the secp256k1 Elliptic Curve
- [Isomorphic elliptic curves](https://hackmd.io/@dJO3Nbl4RTirkR2uDM6eOA/Bk0NvC8Vo) on the secp256k1/secq256k1 cycle
- PayPal reintroduces controversial terms allowing them to take [$2500](https://twitter.com/GayRepublicSwag/status/1585151345610600448) if they don’t like what you say

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-october-29-2022](https://weekinethereumnews.com/week-in-ethereum-news-october-29-2022)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Oct 31 – [Merge data challenge](https://esp.ethereum.foundation/merge-data-challenge) deadline
- Oct 31-Nov 10 – Clr.fund [LatAm round](https://ethcolombia.clr.fund/)
- **Nov 1 –** [**Fixing Goerli**](https://github.com/eth-clients/goerli/issues/129) **community call**
- Nov 3 – US Treasury [digital assets RFC](https://public-inspection.federalregister.gov/2022-20279.pdf) \[PDF\] deadline
- Nov 4-6 – [ETHSanFrancisco](https://sf.ethglobal.com/) (ETH Global)
- Nov 11-13 – [ETHBrno](https://ethbrno.cz/) (Czech Republic)
- Nov 18-20 – [Web3 Weekend](https://web3weekend.ethglobal.com/) (ETH Global)
- Nov 25-27 – [ETH Vietnam](https://www.eth-vietnam.com/)
- Dec 1 – [Columbia cryptoeconomics workshop](https://bit.ly/columbiacryptoeconomics) (New York)
- Dec 2-4 – [ETHIndia](https://ethindia.co/) (ETH Global)
- **Dec 5 –** [**EF Layer 2 grants**](https://esp.ethereum.foundation/layer-2-grants) **deadline**
- Mar 2-5 – [ETHDenver](https://www.ethdenver.com/)

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

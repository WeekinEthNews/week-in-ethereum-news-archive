---
title: "Week in Ethereum News <br> November 13, 2021"
date: "2021-11-13"
---

## **Eth News and Links**

**Mainnet execution layer**

- Update your clients for [Arrow Glacier upgrade](https://blog.ethereum.org/2021/11/10/arrow-glacier-announcement/) (difficulty bomb delay) before December 5:
    - Geth [v1.10.12](https://github.com/ethereum/go-ethereum/releases/tag/v1.10.12): native Go call tracing (2.5x faster)
    - Erigon [v2021.11.02](https://github.com/ledgerwatch/erigon/releases/tag/v2021.11.02): official beta suffix
    - Nethermind [v1.11.7](https://github.com/NethermindEth/nethermind/releases/tag/1.11.7): TxPool optimization, trace\_callMany and tracing improvements
    - Besu [v21.10.1](https://github.com/hyperledger/besu/releases/tag/21.10.1)
    - EthereumJS VM [v5.6.0](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs%2Fvm%405.6.0)
- Latest [core devs call video](https://www.youtube.com/watch?v=Kk-kZXazi18&t=227s). Notes from [Tim Beiko](https://twitter.com/TimBeiko/status/1459240133752856577): 
    - Multi-client devnet to switch off PoW expected late next week
    - Discussion of how execution layer clients will identify network upgrade for PoW switch off
    - EIP4396 to update EIP1559 to use time rather than blocks won’t be included in PoW switch off as don’t want to delay
    - EIP4444 proposal to limit historical data over p2p to 1 year
- Initial PoW switch off [execution layer spec](https://github.com/ethereum/execution-specs/pull/390)
- [Geth todo list](https://mariusvanderwijden.github.io/blog/2021/11/07/GethTODO/) to switch off PoW
- [JSON-RPC spec has great first issues](https://twitter.com/lightclients/status/1458806187638411270) for devs looking to contribute and break into core development

**EIPs/Standards**

- [EIP editors wanted](https://notes.ethereum.org/@timbeiko/eip-editors): volunteer a few hours per week, focus on your area of expertise, ensure EIPs are well-formatted, technically complete and meet minimum quality bar
- [EIP4430](https://github.com/ethereum/EIPs/blob/165dde6dda401a0f4ca8bfd7f0c1a8b01f18a5ec/EIPS/eip-4430.md): Described Transactions
- [EIP4444](https://eips.ethereum.org/EIPS/eip-4444): Bound Historical Data in Execution Clients

**Proof of Stake consensus layer**

- [Kintsugi testnet (PoW switch off) v2 spec](https://hackmd.io/@n0ble/kintsugi-spec): engine API forkchoiceUpdated returns payloadId rather than both layers calculating it
- [Optimistic sync research](https://twitter.com/sigp_io/status/1458210054557954048) (post PoW switch off): sync Beacon Chain without verifying execution components, once execution client synced then inform consensus client of validity of transactions
- Teku [v21.11.1](https://github.com/ConsenSys/teku/releases/tag/21.11.1): fixed blocks endpoints compliance, support for Apple silicon and LevelDB on Linux/arm64, improved performance when running large number of validators
- Nimbus [v1.5.4](https://github.com/status-im/nimbus-eth2/releases/tag/v1.5.4): hotfix for rare issue leading to loss of attestations and sync committee messages
- Beacon chain [light client design](https://notes.ethereum.org/@ralexstokes/HJxDMi8vY)
- Rocket Pool (staking pool) is [live](https://twitter.com/rocket_pool/status/1457893042367582209), users can run a node or provide liquidity for stakers, capacity will be raised again on November 15

**Layer2**

- [$5 billion locked](https://twitter.com/evan_van_ness/status/1457903605541920771) in Layer2
- [Optimism upgrade to EVM equivalence](https://twitter.com/optimismpbc/status/1458953238867165192) is live; [MetaMask v10.5.1](https://twitter.com/optimismpbc/status/1459296690045796353) supports new fee scheme
- [StarkNet (zk rollup)](https://twitter.com/StarkWareLtd/status/1457707282238738448) opens project onboarding for Alpha mainnet
- [Across Protocol](https://medium.com/across-protocol/across-protocol-is-live-and-you-can-be-a-co-founder-43d848a969d1): bridge from Arbitrum to mainnet built to showcase UMA’s Optimistic Oracle 
- [DAI Wormhole](https://forum.makerdao.com/t/introducing-maker-wormhole/11550): teleport DAI between L2s and mainnet, burn DAI on one network, provide an oracle attestation of the burn, then mint DAI on another network; no need for counterparty liquidity
- [How rollups scale Ethereum](https://hackmd.io/@norswap/rollups): rollups need less validators than mainnet for security and state growth can be spread across multiple rollups

* * *

### **This newsletter is made possible thanks to [Celer](https://www.celer.network/)’s [cBridge](https://cbridge.celer.network/) cross-chain transfer exchange!**

![Celer](https://weekinethereumnews.com/wp-content/uploads/2020/11/Screenshot-from-2020-11-22-15-36-32.png "Celer")

Celer Network is a layer-2 scaling platform that brings fast, secure and low-cost blockchain applications.

Celer cBridge 1.0 has processed $920M total volume and [a major upgrade, cBridge 2.0](https://blog.celer.network/2021/09/22/cbridge-2-0-coherent-blockchain-interoperability-powered-by-the-state-guardian-network/), is launching soon in November. Use at [cbridge.celer.network](https://cbridge.celer.network/).

Celer is also hosting a [cBridge 2.0 testnet campaign with $20,000 in reward](https://blog.celer.network/2021/11/08/cbridge-2-0-testnet-upgrade-with-a-brand-new-state-guardian-network-ui-ux/). 

* * *

**Stuff for developers**

- Solidity [v0.8.10](https://blog.soliditylang.org/2021/11/09/solidity-0.8.10-release-announcement/): external function call optimizations, EVM code generator for pure Yul mode and SMTChecker reports contract invariants & reentrancy properties
- [ENSTools](https://github.com/alexvansande/ENSTools): use ENS instead of an address including DNS not yet claimed as ENS; onlyENSOwner modifier, push & pull funds/NFTs to ENS
- [xdeployer](https://github.com/pcaversaccio/xdeployer): Hardhat plugin to deploy contracts with deterministic address (uses CREATE2), beta, currently only selected testnets
- Intro to [DappTools testing](https://eattheblocks.com/dapptools-supercharge-your-smart-contracts/): write tests in Solidity, fuzz testing and symbolic execution
- Nile [v0.2.0](https://medium.com/@martriay/manage-your-starknet-deployments-with-nile-%EF%B8%8F-e849d40546dd): Python development environment for StarkNet contracts, supports Cairo v0.5.0, uses starknet-devnet as default local network
- [Nethereum explorer](https://github.com/Nethereum/Nethereum-Explorer-Wallet-Template-Blazor) (.NET explorer & simple wallet template): migrated to Blazor & Maui
- Etherscan adds [more support for ERC1155](https://twitter.com/etherscan/status/1456967310237863940) multi token standard
- WalletConnect [v2.0 explainer](https://medium.com/walletconnect/walletconnect-v2-0-protocol-whats-new-3243fa80d312): multi-chain support, pairing & session separation, JSON-RPC permissions, improved session management and decentralized message relaying (using Waku v2.0)

**Security**

- samczsum’s [pinball CTF](https://www.paradigm.xyz/2021/11/hiding-in-plain-sight/) used Etherscan source verification 0day, anything between solc metadata markers was ignored; [solution to CTF](https://medium.com/@kanewallmann_71759/an-untrustworthy-pinball-machine-d9dcd07882c)
- [Smart Contract Security Registry](https://blog.openzeppelin.com/smart-contract-security-registry/): register to receive info on known incidents or threats for OpenZeppelin Contracts & selected libraries 

**Ecosystem**

- Trent’s [updated Ethereum roadmap](https://newsletter.banklesshq.com/p/ethereum-roadmap-update-end-of-2021): PoW switch off in 5-8 months, Shanghai upgrade in 10-12 months and ongoing research for data sharding, state expiry & weak statelessness
- [Energy use of the network will be reduced by ~99.95%](https://twitter.com/0xstark/status/1457823831360368640) when Proof of Work is switched off forever
- [Sandwiching that benefits users](https://twitter.com/bertcmiller/status/1459175377591541768): provide Just in Time liquidity on Uniswap v3 to frontrun a large trade and then backrun the trade to remove liquidity, gives better execution price to traders
- [Gas fees during NFT launches](https://twitter.com/blocknative/status/1458887789030764557?s=20): base fee & priority fee combine to create tabletop around 2000 gwei
- [Etherscan](https://twitter.com/etherscan/status/1457678536982994949): review and revoke NFT and ERC20 approvals

**Enterprise**

- [KINGSHIP metaverse group formed by 10:22PM](https://www.universalmusic.com/1022pm-forms-kingship-the-first-ever-group-consisting-of-nft-characters-from-bored-ape-yacht-club/) (Universal Music label), 3 Bored Apes & 1 Mutant to release music, NFTs and experiences
- Discord [hints at Ethereum integration](https://twitter.com/jasoncitron/status/1457841222995693570) but then [announces no plans to ship](https://twitter.com/jasoncitron/status/1458607550677405699) after backlash
- [CDBCgo from ConsenSys and Visa](https://finance.yahoo.com/news/mas-announces-winners-global-cbdc-115100065.html) one of three winners of Monetary Authority of Singapore’s Global CDBC Challenge

**Application layer**

- [Curve ended USDM gauge](https://thedefiant.io/curve-wars-mochi-turned-off-rewards/) after alleged governance attack, turning off Mochi’s pool CRV rewards
- 1inch Router [v4](https://blog.1inch.io/the-1inch-router-v4-is-rolled-out-320f291f995f): separate routers added to lower gas costs and DAI permit support
- [SongADAO](https://twitter.com/songadaymann/status/1457807950756683792): co-op to own Song A Day catalog copyright and royalties (Disclosure: I own a Song A Day NFT)
- [Sign-in with Ethereum](https://twitter.com/BrantlyMillegan/status/1458902877708107780) demo implementation, integrates with ENS to display ENS name and avatar

* * *

### **Job Listings**

- Ethereum Foundation hiring a [Research Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=48&source=weekinethnews) for PoS consensus layer
- OpenZeppelin hiring a [Open Source Developer](https://openzeppelin.com/jobs/opening/?gh_jid=4554917003)
- Toucan: [Solidity dev](https://toucan-protocol.notion.site/Join-the-Flock-c5782edb754b48e598a8cdd74a4dc93c) to build web3 infrastructure to reverse climate change

**Reach people experienced with Ethereum.**  $420 for two issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [US infrastructure bill passed](https://twitter.com/jerrybrito/status/1456823501529260033), crypto provisions take effect Jan 1, 2024 
- [Mastercard](https://www.mastercard.com/news/ap/en/newsroom/press-releases/en/2021/november/mastercard-partners-with-leading-digital-currency-companies-across-asia-pacific-to-launch-the-region-s-first-crypto-linked-payment-cards/) launching crypto-funded payment cards in Asia Pacific
- Gnosis propose [xDAI sidechain merger](https://forum.gnosis.io/t/gip-16-gnosis-chain-xdai-gnosis-merge/1904) to become Gnosis Chain
- A post-EIP1559 [flows-based Ethereum price](https://dataalways.substack.com/p/a-flows-based-ethereum-price-model) model

**General**

- [Visualization of crypto vs internet adoption](https://twitter.com/crypto_fruit/status/1458354467452198916): crypto is where the internet was in 1998
- [16% of US adults](https://www.pewresearch.org/fact-tank/2021/11/11/16-of-americans-say-they-have-ever-invested-in-traded-or-used-cryptocurrency) have used, invested or traded crypto
- [Robinhood](https://blog.robinhood.com/news/2021/11/8/data-security-incident) customer support social engineering incident, unauthorized access to 5m email addresses, 2m names, ~300 personal info and ~10 extensive account details
- [2FA bots](https://www.vice.com/en/article/y3vz5k/booming-underground-market-bots-2fa-otp-paypal-amazon-bank-apple-venmo) used to gain access to centralized accounts
- Cloudflare: [performance of TLS with drop-in post-quantum signatures](https://blog.cloudflare.com/sizing-up-post-quantum-signatures/)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-november-13-2021](https://weekinethereumnews.com/week-in-ethereum-news-november-13-2021)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Oct 25 - Dec 13 – [Gitcoin DAO Global hackathon](https://gitcoin.co/hackathon/dao-global/onboard) (virtual)
- Nov 16 – [Formal Verification in the Ethereum Ecosystem](https://runtimeverification.com/events/formalverificationeth/)
- **Nov 19 – Applications close for [Applied ZK learning group](https://twitter.com/0xparc/status/1458908334069727235)**
- Dec 1-16 – [Gitcoin Grants Round 12](https://twitter.com/gitcoin/status/1454244939169214472)
- Dec ~8 – [Arrow Glacier](https://blog.ethereum.org/2021/11/10/arrow-glacier-announcement/) upgrade block 13,773,000
- Jan 24-26 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford University)
- Feb 11-20 – [ETHDenver](https://www.ethdenver.com/)
- Mar 28-30 – [ETHDubai](https://www.ethdubai.xyz/)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

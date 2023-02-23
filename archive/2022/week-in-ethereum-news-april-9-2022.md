---
title: "Week in Ethereum News <br> April 9, 2022"
date: "2022-04-09"
---

## **Eth News and Links**

**Mainnet execution layer**

- [Erigon stabilizing alpha version](https://twitter.com/erigoneth/status/1511664827839782916) with merge support, full sync required as DB layout not compatible with beta version
- Verkle tree [Condrieu testnet relaunched twice](https://notes.ethereum.org/@gballet/verkle-testnet-updates/%2Fs%2FSksmVxpb5) for continued stress-testing
- [Predicting access lists](https://ethresear.ch/t/predicting-access-list-a-potential-way-to-speed-up-the-evm-for-portal-clients/12355) to reduce state retrieval time for Portal network clients 

**Proof of Stake consensus layer**

- PoS implementers [call video](https://www.youtube.com/watch?v=rYWF7N8tS0g&t=25s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/H1U6EPnXq) & [Christine Kim](https://twitter.com/christine_dkim/status/1512100564586348549):
    - Timing of forking public testnets to be decided at Core Devs call on April 29, clients to be feature complete or need to delay difficulty bomb
    - Goerli shadow fork #3 had issue impacting small subset of Geth nodes
    - mainnet shadow fork switches to PoS on April 11;  
        **warning**: txs could be replicated to mainnet costing ETH
    - Builder API & MEV-Boost discussion
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220408)
- Proposer boost upgrade to mitigate attacks involving delayed publishing of blocks & attestations:
    - Lighthouse [v2.2.0](https://github.com/sigp/lighthouse/releases/tag/v2.2.0)
    - Teku [v22.4.0](https://github.com/ConsenSys/teku/releases/tag/22.4.0)
- [Activation/exit queue rate-limit](https://twitter.com/terencechain/status/1509923504841392129) increased to 5 each epoch after reaching 327,680 active validators
- [Visualization of staking pools](https://hackmd.io/vCxX0WgoQEW3dZ-k_oZgBg?view), open source analytics of known pools
- Vitalik: [simplified version of single secret leader election](https://ethresear.ch/t/simplified-ssle/12315) (SSLE) using size-2 swaps, less perfect guarantees but much simpler

**PoW switch off (the merge)**

- [clientdiversity.org](https://clientdiversity.org/): dashboard with consensus & execution client distribution;
    - **Reminder**: execution client diversity also required
    - Currently Prysm at 56% and Geth at 87%
- [EthereumJS client](https://twitter.com/efjavascript/status/1510176850873626627) (with Lodestar) proposed a block on Kiln testnet
- [Transaction fees can be stolen](https://www.symphonious.net/2022/04/09/exploring-eth2-stealing-inclusion-fees-from-public-beacon-nodes/) if you don’t run your own staking nodes

**EIPs/Standards**

- [EIP4974](https://github.com/ethereum/EIPs/blob/8e8709bfa55c6357e6022ca4f886a59f5dc7c148/EIPS/eip-4974.md): Experience (EXP) token standard
- [EIP4972](https://github.com/ethereum/EIPs/blob/30ca715aa9b0e4946f4b428f2bf03dc8ca283cab/EIPS/eip-4972.md): Name Owned Account
- [EIP4966](https://github.com/ethereum/EIPs/blob/9754700b44b8e63d5503b563d16c99a2552b8c2e/EIPS/eip-4966.md): Non-Transferable NFTs (Soulbound Tokens)

**Layer2**

- Arbitrum [Nitro devnet](https://medium.com/offchainlabs/its-nitro-time-86944693bf29): fraud prover using core Geth on WASM, calldata compression, code uses Business Source License; Twitter faucet
- Polynya: [rollup types](https://twitter.com/poiynya/status/1511623759786307586), regular, immutable, enshrined and sovereign

* * *

### **This newsletter is made possible thanks to Starbloom Ventures!**

![Starbloom Ventures](https://weekinethereumnews.com/wp-content/uploads/2021/11/Screenshot-from-2021-11-19-15-25-51.png)

[](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F9bf9946e-747e-4db0-b217-2e99b2b307af_613x313.png)

Starbloom Ventures is an early-stage venture fund founded by [Evan Van Ness](https://twitter.com/evan_van_ness) to invest in the future of web3. 

What’s missing in DeFi?  How about [non-correlated assets](https://medium.com/@rysk-finance/rysk-is-the-only-free-lunch-e4f832af0026) - coming soon™️ via [Rysk](https://www.rysk.finance/)’s dynamic hedging options AMM

* * *

**Stuff for developers**

- [Foundry fork mode test traces](https://twitter.com/gakonst/status/1512177380160274432) decoded using source/ABI from Etherscan
- [Experiment with EIP3540 EVM Object Format](https://twitter.com/EFJavaScript/status/1511656097932881921) using EthereumJS 
- Formal verification of [BokkyPooBah's DateTime library](https://github.com/Zellic/publications/tree/master/BokkyPooBahsDateTimeLibrary#readme)
- [StreamPie](https://github.com/ameensol/streampie#readme): tokenized Sablier stream that token holders can RageStream to fork their own pro-rata Sablier stream
- [Bit twiddling techniques](https://hackmd.io/@fiveoutofnine/Skl9eRbX9) in Solidity, applied to tic-tac-toe game
- [solvm](https://github.com/brockelmore/solvm#readme): stripped down EVM implemented using Yul & Solidity
- [Trustus](https://github.com/ZeframLou/trustus#readme): provide contracts with off-chain data from trusted servers
- [EVM draw contract](https://github.com/DanielVF/evm-contract-draw#readme): draws bytes of a contract for overview of its shape
- [GateRepo](https://github.com/anish-agnihotri/gaterepo#readme): ERC20 token gated private GitHub repositories
- Deep dive into [web3.py internals](https://snakecharmers.ethereum.org/web3py-internals-json-rpc-round-trips/): JSON-RPC round trips
- Echidna [v2.0.1](https://github.com/crytic/echidna/releases/tag/v2.0.1): adds Foundry support, bug fixes
- OpenZeppelin [Contracts for Cairo v0.1.0](https://blog.openzeppelin.com/announcing-openzeppelin-contracts-for-cairo/): account abstraction, ERC20 & ERC721 implementations, Ownable, Pausable, SafeMath and Proxy
- [GitPOAP](https://medium.com/gitpoap/gitpoap-is-live-ca736f33fa0b): POAPs for contributing to open source

**Security**

- Inverse Finance $15.6 million [exploit](https://medium.com/inverse-finance/inv-price-manipulation-incident-55ea0433f4fc), price oracle manipulation due to TWAP with short window
- Starstream [exploit](https://twitter.com/CertiKAlert/status/1512155452217479171) on Metis Andromeda Layer 2, public execution function allowed Stars tokens to be drained from the treasury
- Convex Finance [vulnerability disclosed](https://blog.openzeppelin.com/15-billion-rugpull-vulnerability-in-convex-finance-protocol-uncovered-and-resolved/), multi-sig owners could potentially gain control of staked LP tokens, $15 billion was at risk, patched

**Ecosystem**

- Tim Beiko’s [roadmap FAQ](https://github.com/timbeiko/eth-roadmap-faq) covering the merge, withdrawals & sharding
- [Fake revoke approvals site](https://twitter.com/0xquit/status/1511773105705783296) used to get holders to approve NFTs
- [VaynerSports](https://twitter.com/cr0sseth/status/1511446814196572161): $8 million in NFT sales but $26 million spent on gas, [record 106 ETH burnt in one block](https://twitter.com/ultrasoundmoney/status/1511433534036189184) by EIP1559
- EF’s client incentive program updated with [technical details](https://blog.ethereum.org/2021/12/13/client-incentive-program/) 

**Enterprise**

- [Proof of concept usage of Baseline pattern](https://medium.com/unibrightio/unibright-presents-study-on-the-usage-of-the-baseline-pattern-at-european-investment-fund-97376b1afc01) at European Investment Fund

**Application layer**

- [Umbra](https://www.scopelift.co/blog/umbra-launches-on-optimism-and-polygon) (stealth address payments) live on Arbitrum & Optimism
- Index Coop [icETH](https://indexcoop.com/blog/understanding-interest-compounding-eth-index-iceth): leverage liquid staking using Set Protocol & Aave
- [Gem](https://twitter.com/gemxyz/status/1512104464563515392) (NFT marketplace aggregator): adds listing analytics, filter by traits/price/rarity
- [Pando](https://forum.makerdao.com/t/mip73-pando-investment-grade-climate-assets-collateral-onboarding/14484) applies to onboard solar loans with Maker
- Curve wars: [Luna and FRAX propose 4pool](https://avgjoescrypto.substack.com/p/the-curve-wars-go-hot) (UST, FRAX, USDC & USDT) in attempt to undercut DAI’s spot in 3pool (USDT, USDC & DAI)
- [Gradual Dutch Auctions](https://www.paradigm.xyz/2022/04/gda): sell tokens without liquid markets, discrete GDA for selling NFTs & continuous GDA for selling fungible tokens
- [veDAO](https://medium.com/@vedao.alt/on-optimism-9d81f56bbdd3) announces plans to bring Solidly v2 to Optimism

* * *

### **Job Listings**

- EF ecosystem support hiring for [Communications](https://jobs.lever.co/ethereumfoundation/4b0c3305-cf03-4e33-9bfb-63e4ec6f3a68?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum), [Analyst](https://jobs.lever.co/ethereumfoundation/64361391-9a74-49ed-b37c-8ff35931430e?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) & [Admin Assistant](https://jobs.lever.co/ethereumfoundation/5684f7ea-c3ad-4703-b86c-462964f49392?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- [Hifi](http://hifi.finance/) is hiring a [Senior Solidity Engineer](https://bit.ly/3CMmbSe) & [Community/Social Media Manager](https://bit.ly/36q06g5)
- EF’s Privacy & Scaling Explorations team: [Technical Project Coordinator](https://jobs.lever.co/ethereumfoundation/78089bc2-125e-47de-af28-e162de149901?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum), [ZKP Security Engineer](https://jobs.lever.co/ethereumfoundation/b80cf733-9a8d-40f1-a85a-635acdc2b1b1?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum%20), [L2 Security Engineer](https://jobs.lever.co/ethereumfoundation/f3148457-ed1e-4659-941d-5f60b49427ca?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) & [Marketing Ops Manager](https://jobs.lever.co/ethereumfoundation/7a831e7c-1a0d-4e7b-8291-072292e26c0e?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum%20&lever-source%5B%5D=Week%20in%20Ethereum%20)
- EF hiring [Test Engineer](https://jobs.lever.co/ethereumfoundation/e6d303e5-168d-447e-a596-e3c2b105ca3f?lever-source%5B%5D=Week%20in%20Ethereum%20) to improve testing infrastructure & coverage
- Devcon needs a [front-end web developer](https://ethereum.bamboohr.com/jobs/view.php?id=61&source=weekinethnews)
- SideShift.ai is hiring a [Solidity Engineer](https://sideshift.ai/jobs?utm_campaign=hiring&utm_source=weekinethnews). Good job!

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [UK government plans](https://www.gov.uk/government/news/government-sets-out-plan-to-make-uk-a-global-cryptoasset-technology-hub): regulate stablecoins for payment use, legislate financial market infrastructure sandbox & explore tax treatment of DeFi loans and make UK a global crypto hub
- US SEC Chair: [potential areas for regulation](https://www.axios.com/sec-head-has-four-new-questions-about-crypto-cfbd989f-1ab2-46d8-9cab-1662d03dac46.html), protect retail traders, work with CFTC, separate exchange & custody and separate market making 
- [Worldpay](https://www.circle.com/en/pressroom/worldpay-from-fis-becomes-first-global-merchant-acquirer-to-offer-direct-usdc-settlement-driving-digital-currency-adoption-to-businesses) to allow merchants to receive settlement in USDC
- [Wyre acquired](https://blog.sendwyre.com/setting-a-new-standard-bdc7842b9ba6) by Bolt for $1.5 billion
- Christine Kim (Galaxy Digital Research): [what to expect from the merge](https://docsend.com/view/padamxd8qsg56459)

**General**

- Contribute to [Semaphore’s trusted setup ceremony](https://twitter.com/PrivacyScaling/status/1511291645920219140)
- [Trezor users targeted in phishing attacks](https://blog.trezor.io/ongoing-phishing-attacks-on-trezor-users-edd840b17304) after MailChimp compromised
- Jameson Lopp: [how to backup a seed phrase](https://blog.lopp.net/how-to-back-up-a-seed-phrase/)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-april-9-2022](https://weekinethereumnews.com/week-in-ethereum-news-april-9-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in_ **_bold_**_)_**:**

- Apr 18-25 – [Devconnect](https://devconnect.org/schedule) (Amsterdam)
- Apr 22 – deadline for [EF academic grants round](https://esp.ethereum.foundation/academic-grants)
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- May 3-5 – [Spaghett ETH](https://spaghett-eth.com/) (Milan)
- **May 6-27 – ETH Global** [**Hack Money**](https://defi.ethglobal.com/)
- **May 17-20 –** [**EY Global blockchain summit**](https://pub.ey.com/public/2021/2112/2112-3933703/blockchain-summit-2022/index.html)
- May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETH NYC](https://nyc.ethglobal.co/)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- **Sep 1-4 –** [**ETHWarsaw**](https://ethwarsaw.dev) **(hackathon & conference)**
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** [_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive it weekly_**

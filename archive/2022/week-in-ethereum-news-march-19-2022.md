---
title: "Week in Ethereum News <br> March 19, 2022"
date: "2022-03-19"
---

## **Eth News and Links**

**Mainnet execution layer**

- Latest core devs [call video](https://www.youtube.com/watch?v=Lbsjw-lzMIw). Notes from [Tim Beiko](https://twitter.com/timbeiko/status/1504913092420931584):
    - Kiln testnet transition to PoS successful, some implementation issues, more testing needed including devnets and live network shadow forks
    - EIP4895 push withdrawals as operations selected for Shanghai
    - EIP4844 data blob transaction type update
    - Proposal to [harmonize Core EIP process with executable specs](https://notes.ethereum.org/@timbeiko/executable-eips)
- Erigon [v2022.03.01](https://github.com/ledgerwatch/erigon/releases/tag/v2022.03.01): bug fixes
- Besu [v22.1.2](https://github.com/hyperledger/besu/releases/tag/22.1.2): Kiln v2.1 spec support, tracing API improvements
- PluGeth [Parity tracing plugin](https://blog.openrelay.xyz/parity-trace/): 4 tracing methods equivalent to OpenEthereum
- EIP4844 data blob transaction type [meta-spec](https://hackmd.io/@protolambda/eip4844-meta) and [promotional website](https://www.eip4844.com/)
- Dankrad’s EIP1559 exponential version [explainer](https://dankradfeist.de/ethereum/2022/03/16/exponential-eip1559.html), proposed for data blob transactions

**Proof of Stake consensus layer**

- [Loss risk model](https://docs.google.com/spreadsheets/d/12R8wkuv62hZyajrhhlkNrskkwH2-zjYZjXKkHJuxGQc/edit#gid=1446351392) for providers running a supermajority client
- Lighthouse [v2.1.4](https://github.com/sigp/lighthouse/releases/tag/v2.1.4): Kiln testnet support, networking optimizations;  
    [v2.1.5](https://github.com/sigp/lighthouse/releases/tag/v2.1.5): address DoS vulnerability in OpenSSL used for https
- Teku [v22.3.1](https://github.com/ConsenSys/teku/releases/tag/22.3.1): Kiln testnet support, reduced CPU & memory usage when processing gossip
- Ben Edgington’s Upgrading Ethereum book [chapter on BLS signatures](https://eth2book.info/altair/part2/building_blocks/signatures)
- [Priority fee analysis](https://www.attestant.io/posts/exploring-execution-block-rewards/) with projected returns for validators
- Rocket Pool [smoothing pool proposal](https://dao.rocketpool.net/t/a-candidate-design-for-the-smoothing-pool/346) for MEV & priority fees
- [Stakers should prune Geth node](https://www.reddit.com/r/ethstaker/comments/tgs9qy/if_you_are_running_your_node_on_a_2tb_ssd_its_a/) if running on a 2TB SSD

**PoW switch off**

- Ethereum Foundation’s [Kiln testnet](https://blog.ethereum.org/2022/03/14/kiln-merge-testnet/) announcement: 
    - App & tooling devs should [test now](https://kiln.themerge.dev/)
    - PoW switch off date will be set once existing public testnets transition to PoS successfully
- Prysm [block proposal bug](https://hackmd.io/@prysmaticlabs/HyZqgTA-c) on Kiln testnet, caused by big vs little endian handling in base fee per gas, not detected previously as base fee of 7 used has same value in big/little endian
- [Video](https://www.youtube.com/watch?v=caaV4oMmWe8) guide to join Kiln testnet using Geth+Lighthouse
- Join Kiln testnet with a [Raspberry Pi or on AWS](https://twitter.com/EthereumOnARM/status/1503662463778271237)

**EIPs/Standards**

- [EIP4906](https://github.com/ethereum/EIPs/blob/f400ed4823ff547e789111adbdd90c83f4aedce5/EIPS/eip-4906.md): ERC721/ERC1155 Metadata Update Extension
- [EIP4907](https://github.com/ethereum/EIPs/blob/692afba71b6b2cee2e48c6c729597c2f025da732/EIPS/eip-4907.md): ERC721 User And Expires Extension
- [EIP4910](https://github.com/ethereum/EIPs/blob/a32f465175f0509781b52615b1e29bed03a5fed5/EIPS/eip-4910.md): Royalty Bearing NFTs

**Layer2**

- StarkNet Alpha [v0.8.0](https://medium.com/starkware/starknet-alpha-0-8-0-16e046e0f94b) on testnet, adds fees, optional until v.0.9.0
- Design for [partially anonymous rollup](https://ethresear.ch/t/partially-anonymous-rollups-a-new-rollup-design/12206), operator creating a batch has transaction details, account activity leaked via updated account state hashes

* * *

### **This newsletter is made possible thanks to the [Uniswap Grants Program](https://unigrants.org/)!**

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fbdb3fefa-2a1b-4624-9893-cda1453bf527_1600x429.png)](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fbdb3fefa-2a1b-4624-9893-cda1453bf527_1600x429.png)

[Uniswap Grants Program](https://unigrants.org/) - If you’ve ever wanted to work on TWAP oracles, better DeFi devtools, had ideas on optimizing LP strategies, or just wanting to improve the Uniswap protocol, [apply for a grant from UGP today](https://airtable.com/shrWrSFRs6t1q1s9v)!

For more grant ideas, check out our [list of RFPs](https://www.notion.so/RFPs-Challenges-3be614ba4e504b5caeee7b0159e64a42)!

* * *

**Stuff for developers**

- Solidity [v0.8.13](https://blog.soliditylang.org/2022/03/16/solidity-0.8.13-release-announcement/): fix for abi.encodeCall bug, Yul IR pipeline production ready, optimizer can avoid stack too deep, using for at file level & global and adds go to definition for language server
- Remix [v0.22](https://medium.com/remix-ide/remix-v0-22-0-v0-22-1-released-359f7e02f693): increased browser storage capacity, JavaScript unit testing with Mocha and debugger searches Sourcify & Etherscan for verified code
- Foundry seminar [video](https://www.youtube.com/watch?v=Rp_V7bYiTCM): setup, testing, call-tracing, debugger and preview of invariant tests & smarter fuzzer
- Chainlink [Foundry starter kit](https://github.com/smartcontractkit/foundry-starter-kit#readme): VRFv2, MockOracle and prompt-based deployment scripts
- ethers js [v5.6.1](https://github.com/ethers-io/ethers.js/releases/tag/v5.6.1): fix for CCIP Read using wrong sender
- [Solidity trivia](https://twitter.com/the_ethernaut/status/1502748198301011969) by the Ethernaut
- [Gas optimizations for regular devs](https://m1guelpf.blog/d0gBiaUn48Odg8G2rhs3xLIjaL8MfrWReFkjg8TmDoM): bump Solidity version, use immutable variables, unchecked, custom errors, avoid Counters and avoid copy to memory
- [ERC4626.sol](https://github.com/Rari-Capital/solmate/blob/main/src/mixins/ERC4626.sol): solmate implementation of tokenized vault
- [Revenue distribution token](https://github.com/maple-labs/revenue-distribution-token#readme): ERC4626 with linear revenue issuance, not audited, unit/fuzz tests in Foundry & invariant tests in dapptools
- hardhat-circom [v3.0.0](https://github.com/projectsophon/hardhat-circom/releases/tag/v3.0.0): uses circom2 compiler as default
- Dune dashboard to [get contracts by deployer address](https://dune.xyz/msilb7/Get-Contracts-by-Creator-Address-Ethereum-Optimism) on Ethereum & Optimism

**Security**

- Agave (Aave fork) & Hundred Finance (Compound fork) $5.5 & $6.2 million [exploits on Gnosis chain](https://rekt.news/agave-hundred-rekt/) (formerly xDAI) using reentrancy via native token
- Bored Apes from NFTX vault used to [claim APE airdrop](https://twitter.com/wilburforce_/status/1504437189979119622) before being returned to the vault in the same transaction
- Parity wallet 2017 hacker [moved 990 ETH](https://twitter.com/PeckShieldAlert/status/1503359286692704267) to Tornado Cash

**Ecosystem**

- Sign-In with Ethereum [Discourse plugin](https://blog.spruceid.com/sign-in-with-ethereum-to-discourse/) for self-hosted forums, enabled on [ENS forum](https://discuss.ens.domains/t/sign-in-with-ethereum-is-now-enabled/11498)
- [Tally Ho](https://blog.tally.cash/sign-in-with-ethereum-support/) (browser wallet) adds native support for Sign-In With Ethereum
- Etherscan’s [spoof token explainer](https://medium.com/etherscan-blog/spoof-tokens-on-ethereum-c2ad882d9cf6): token transfer event has a different from address than the transaction from address
- Vitalik [trusted setup explainer](https://vitalik.ca/general/2022/03/14/trustedsetup.html); a trusted ceremony is needed for KZG commitments

**Enterprise**

- [DC Comics hybrid trading cards](https://www.dccomics.com/blog/2022/03/11/cartamundi-launches-dc-hybrid-physical-and-nft-trading-cards): physical cards with connected NFTs on Hro (Immutable X)
- [Pixar NFTs](https://medium.com/veve-collectibles/disney-pixar-pals-25c6da53ab8e) via blind boxes on VeVe (Immutable X)
- [HSBC](https://sandboxgame.medium.com/hsbc-to-become-the-first-global-financial-services-provider-to-enter-the-sandbox-c066e4f48163) acquires virtual real estate in The Sandbox metaverse
- Aya: [ESG systems can learn from Ethereum’s principles](https://www.weforum.org/agenda/2022/03/blockchain-principles-improve-esg-systems/)

**Application layer**

- Aave [v3](https://aave.mirror.xyz/2TnHYHQRnNhSG56Y4CcssulFArSVqrFbmAdYfU7Kxp0) live on Optimism & Arbitrum; adds portals, high efficiency mode, isolation mode, gas optimization & risk management
- Alchemix [v2](https://twitter.com/scupytrooples/status/1503751703019110410) (self-repaying loans): mix and match collateral & strategies 
- Kwenta [synthetic perpetual futures](https://blog.kwenta.io/futures-beta/) beta live on Optimism
- [Sablier](https://medium.com/sablier/sablier-expands-to-optimism-arbitrum-and-avalanche-b0889fb8d3ac) (money streaming) live on Optimism & Arbitrum
- [Backd](https://blog.backd.fund/backd-is-live-c90e8dc08f34) (reactive liquidity) live on mainnet
- [Vovo Finance](https://vovofinance.medium.com/vovo-finance-is-live-on-arbitrum-mainnet-695974f92b32) (principal protected products) live on Arbitrum
- [Stargate bridge](https://medium.com/stargate-official/stargate-a-farewell-to-bridges-28831d0f9439) between mainnet, Optimism & Arbitrum 
- [Epic space saga](https://twitter.com/wiiichang/status/1503751757834379270) in latest round of Dark Forest game
- [Larva Labs hid a Meebit](https://twitter.com/andrewbadr/status/1503436760239464449) with clues in Grails #11 and Meebit artwork
- [Sound](https://twitter.com/soundxyz_/status/1503376318649438209) onboards Snoop Dogg with Death Row Mix Vol. 1 NFT
- [CyberBrokers](https://twitter.com/cybourgeoisie/status/1503130085993459722) SVG layers & metadata on mainnet, uses custom renderer with images cached on IPFS, deployment cost 91 ETH
- [Guild](https://twitter.com/guildxyz/status/1504817786685693998) adds NAND (can’t hold competing) & NOR (can’t hold any) token gating
- [ApeCoin DAO](https://twitter.com/apecoin/status/1504201556165644298): token airdrop for Bored Ape holders

* * *

### **Job Listings**

- [Hifi](http://hifi.finance/) is hiring a [Senior Solidity Engineer](https://bit.ly/3CMmbSe) & [Community/Social Media Manager](https://bit.ly/36q06g5)
- SideShift.ai is hiring a [Solidity Engineer](https://sideshift.ai/jobs?utm_campaign=hiring&utm_source=weekinethnews). Good job!
- EF hiring [Test Engineer](https://jobs.lever.co/ethereumfoundation/e6d303e5-168d-447e-a596-e3c2b105ca3f?lever-source%5B%5D=Week%20in%20Ethereum%20) to improve testing infrastructure & coverage
- Status is Hiring! [SDET](https://grnh.se/2241310c1us) and [Head of Marketing (Status Network)](https://grnh.se/2e01bc791us). [All jobs!](https://jobs.status.im/)  
- Devcon needs a [front-end web developer](https://ethereum.bamboohr.com/jobs/view.php?id=61&source=weekinethnews)
- EF’s Privacy & Scaling Explorations team seek a [ZKP Security Engineer](https://jobs.lever.co/ethereumfoundation/b80cf733-9a8d-40f1-a85a-635acdc2b1b1?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum%20), [L2 Security Engineer](https://jobs.lever.co/ethereumfoundation/f3148457-ed1e-4659-941d-5f60b49427ca?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) and a [Marketing Ops Manager](https://jobs.lever.co/ethereumfoundation/7a831e7c-1a0d-4e7b-8291-072292e26c0e?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum%20&lever-source%5B%5D=Week%20in%20Ethereum%20)
- eVerse is hiring a [lead blockchain engineer](https://everse.notion.site/Lead-Blockchain-Engineer-Architect-845acc3ef4c64784b19d4f2cede8161c) for its social video platform
- Mark Cuban seeks a [web3 front-end developer](https://forms.office.com/r/M81g5RNgXX). Send a work sample to apply.

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [Analysis of US proposed bill](https://www.coincenter.org/new-crypto-sanctions-bill-targets-publishing-code-facilitating-transactions/) for secondary sanctions on crypto providers
- [Russia’s Central bank](https://www.reuters.com/article/russia-cenbank-sberbank-crypto-currency-idUSL5N2VK540) licensed Sberbank to issue and exchange crypto
- [Ukraine](https://www.coindesk.com/policy/2022/03/16/ukraines-zelensky-signs-virtual-assets-bill-into-law-legalizing-crypto/) legalizes crypto
- [EU parliamentary committee](https://twitter.com/paddi_hansen/status/1503383993391194115) voted to reject proposal limiting Proof of Work
- dYdX’s [Guernsey purpose trust](https://dydx.foundation/blog/en/legal-framework-non-us-trusts-in-daos) framework for DAOs: limit liability for DAO participants, enable off-chain activities and clarify US tax reporting
- [Soulbound tokens](https://gov.gitcoin.co/t/how-soulbound-tokens-can-make-gitcoin-grants-more-pluralistic/10077) can make GitCoin grants more pluralistic
- [The Space](https://matterslab.medium.com/radical-markets-can-work-on-blockchain-our-web3-experiment-the-space-shows-how-1b5d49b91d27): experiment with UBI & Harberger tax on a graffiti wall
- [veRev](https://uxdprotocol.medium.com/introducing-verev-a-yield-distribution-mechanism-c9243fbbfe3e): yield distribution using periodic reverse dutch auction for buy back and semi-liquid veTokens
- Risk of buying licensed NFTs: [F1 Delta Time](https://f1deltatime.medium.com/f1-delta-time-to-cease-operations-announces-rewards-for-supporters-2fbf307fe89f) F1 license not renewed, NFTs to be replaced with generic versions

**General**

- Time Magazine puts [Vitalik on the cover](https://time.com/6158182/vitalik-buterin-ethereum-profile)
- [Browser in the browser attack](https://mrd0x.com/browser-in-the-browser-phishing-attack): phishing via simulated browser window to spoof a legitimate domain
- [Node-ipc supply chain attack](https://twitter.com/lefterisjp/status/1504219196590280704), protestware wrote files for users with a Russian IP address

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-march-19-2022](https://weekinethereumnews.com/week-in-ethereum-news-march-19-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Mar 24 – [Gitcoin Grants Round 13](https://gitcoin.co/grants/) ends (support [Week in Eth News](https://gitcoin.co/grants/2785/week-in-ethereum-news))
- Mar 29-31 – [ETHDubai](https://www.ethdubaiconf.org/)
- Apr 7-9 – [ETH Portland](https://2022.ethportland.com/) hackathon
- Apr 18-25 – [Devconnect](https://devconnect.org/schedule) (Amsterdam)
- Apr 22 – deadline for [EF academic grants round](https://esp.ethereum.foundation/academic-grants)
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETHNewYork](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- **Sep 6-9 – [MCON 2](https://twitter.com/mcon_world/status/1504175505389457410) (Denver)**
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- **Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)**
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

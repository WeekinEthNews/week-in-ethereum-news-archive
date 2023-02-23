---
title: "Week in Ethereum News <br> February 12, 2022"
date: "2022-02-12"
---

## **Eth News and Links**

**Proof of Stake consensus layer**

- PoS implementers [call video](https://www.youtube.com/watch?v=DtwTZWZrZMY&t=62s). Notes from [Ben Edgington](https://hackmd.io/@benjaminion/S1YGF9Gk9):
    - Public Kiln testnet to be setup once sufficient milestones hit
    - Vitalik’s blob transactions more complex version favored to lessen work on execution layer; to be prototyped at EthDenver
- Latest [What’s New in Eth2](https://hackmd.io/@benjaminion/eth2_news/https%3A%2F%2Fhackmd.io%2F%40benjaminion%2Fwnie2_220211)
- Lighthouse [v2.1.3](https://github.com/sigp/lighthouse/releases/tag/v2.1.3): improves peer stability using fork of rust-libp2p

**PoW switch off**

- Kiln [milestone tracker](https://notes.ethereum.org/@timbeiko/kiln-milestones#Milestone-tracker) (pre-production sprint for PoW switch off)
    - Kiln will be last testnet before existing public testnets like Goerli are upgraded
- Not many unchecked boxes remain in PoW switch off [readiness checklist](https://github.com/ethereum/pm/blob/master/Merge/mainnet-readiness.md)
- [Draft EIP to add beacon state roots into the EVM](https://twitter.com/ralexstokes/status/1491950188944056320) for beacon chain withdrawals, aiming for Shanghai upgrade after PoW switch off
- [Client diversity risk scenarios](https://mirror.xyz/jmcook.eth/S7ONEka_0RgtKTZ3-dakPmAHQNPvuj15nh0YGKPFriA): 3-4 weeks to resolve a consensus bug in a client with half the ETH staked, compared with 13 minutes for a client with 67% or more ETH staked; examples of past attacks and bugs
- Community call #3 [video](https://www.youtube.com/watch?v=65Pt6oS3kDM&t=5s)
- [Kintsugi testnet PnP image](https://twitter.com/EthereumOnARM/status/1490624310792400897) for Raspberry Pi

**EIPs/Standards**

- [EIP4788](https://github.com/ethereum/EIPs/blob/109829c5aff5c8c687dbbaf4df16980601a93fb0/EIPS/eip-beacon_state_root_in_evm.md): Beacon state root in the EVM
- [EIP4786](https://github.com/ethereum/EIPs/blob/11066d3ac3a576089d1d4045031f985aa226745a/EIPS/eip-4786.md): Link Common Token to ERC721
- [EIP4742](https://github.com/ethereum/EIPs/blob/527902042b4f84952199bcd2c9ed60f87e6c19ac/EIPS/eip-4742.md): NONCE opcode

**Layer2**

- [L2 Fees](https://l2fees.info/l1-fees): adds fees paid to Layer 1 by Layer 2s for security
- [FTX](https://twitter.com/FTX_Official/status/1490903050269396992) supports Arbitrum
- [Argent zkSync wallet](https://www.argent.xyz/blog/how-to-fund-your-argent-l2-account-from-an-exchange/) deposits from exchanges via LayerSwap
- [Proof of Efficiency](https://ethresear.ch/t/proof-of-efficiency-a-new-consensus-mechanism-for-zk-rollups/11988): Polygon Hermez consensus proposal for zk-rollups

* * *

### **This newsletter is made possible thanks to Starbloom Ventures!**

![Starbloom Ventures](https://weekinethereumnews.com/wp-content/uploads/2021/11/Screenshot-from-2021-11-19-15-25-51.png)

Starbloom Ventures is an early-stage venture fund by [Evan Van Ness](https://twitter.com/evan_van_ness) to invest in the future of web3.

We believe that the Ethereum ecosystem should have a cultural norm that VCs help fund public goods, that’s why we pledge [10% of profits to support Ethereum public goods](https://twitter.com/evan_van_ness/status/1461840784819425288).

* * *

**Stuff for developers**

- OpenZeppelin Contracts [v4.5.0](https://github.com/OpenZeppelin/openzeppelin-contracts/releases/tag/v4.5.0): Base64 encoding, NFT royalties, NFT voting, governance minimum voting duration and ERC20 infinite approval
- [Underhanded Solidity Contest](https://blog.soliditylang.org/2022/02/09/underhanded-solidity-contest-2022-announcement/): build a DEX with unexpected trades
- [Solidity developer survey 2021](https://blog.soliditylang.org/2022/02/07/solidity-developer-survey-2021-results/) results
- Feedback wanted on support for [catching Solidity custom errors](https://forum.soliditylang.org/t/feedback-wanted-catching-custom-errors-default-catch-clause/810)
- [Nomic Foundation](https://medium.com/nomic-foundation-blog/introducing-the-nomic-foundation-an-ethereum-public-goods-organization-31012af67df9): non-profit public goods organization building Hardhat, [Rethnet & Slang](https://medium.com/nomic-foundation-blog/slang-rethnet-2ad465fd7880); $15m of $30m already raised
- Forge: [guide](https://mirror.xyz/susheen.eth/bRCzT2QLdNINMVk8251udkfjHW_T9ascCQ1DV9hURz0) to forking mainnet/testnets in tests
- Use [Forge Standard Library](https://mirror.xyz/brocke.eth/PnX7oAcU4LJCxcoICiaDhq_MUUu9euaM8Y5r465Rd2U) to set token balances for an address
- [Incentivize bots to call your contract](https://twitter.com/onewayfunction/status/1491632390564823044?s=20&t=RJtHuBozERcdm-74qksxZw): pay in ETH/WETH, no inputs, no bond/registration, no unsafe external calls & only call when meaningful
- [Slither Action](https://github.com/marketplace/actions/slither-action): run Slither static analyzer in GitHub Actions workflow
- Yield’s approach to [calculating prices](https://hackernoon.com/getting-prices-right) from oracles
- [Token Gate](https://github.com/marcusmolchany/tokengate#readme): TypeScript module for ERC20/721/777/1155 balance gating
- [Flashbots Proxy](https://github.com/Arachnid/flashbots-proxy#readme): interactively compose and submit Flashbots bundles
- [Choosing which wallets](https://twitter.com/fitzeth/status/1491531485509144577) to support for projects on Layer 2
- [StarkNet React](https://github.com/auclantis/starknet-react#readme): React hooks using starknet.js
- [Full-stack guide to Starknet](https://hackmd.io/@sambarnes/BJvGs0JpK) using Nile, Starknet.py and cairopal
- [circom-ecdsa](https://0xparc.org/blog/zk-ecdsa-1): proof of concept zkSNARK circuits for ECDSA in circom
- [EVM symbolic execution engine](https://github.com/leonardoalt/dl_symb_exec_sol#readme) in Solidity with a Difference Logic solver, for study purposes only 
- [Guide to web3 data](https://ath.mirror.xyz/w2cxg5OP1OEcqvSgsEjSSyKRJhPmam0w-fXGogiG-8g) for web2 data analysts

**Security**

- Optimism [critical vulnerability disclosed](https://optimismpbc.medium.com/disclosure-fixing-a-critical-bug-in-optimisms-geth-fork-a836ebdf7c94), self destruct created additional ETH, Optimism & forks fixed, $2 million bounty paid to [saurik](https://www.saurik.com/optimism.html)
- Dego Finance ~$10 million [exploit](https://rekt.news/dego-finance-rekt/), reportedly compromised keys
- Tecra $639k [exploit](https://twitter.com/mauricio_0218/status/1490082073096462340), logic error in token burn, Uniswap v2 pool drained
- Yearn [vulnerability disclosed](https://github.com/yearn/yearn-security/blob/master/disclosures/2022-01-30.md), SingleSidedBalancer strategy could be attacked, $200k bounty paid

**Ecosystem**

- Polynya: [how Ethereum scales](https://old.reddit.com/r/ethereum/comments/skb5h6/how_ethereum_scales_eli12/), first with rollups, then EIP4488 or blob transactions, followed by danksharding and finally statelessness & zk EVM
- Ethereum ecosystem [$585 billion total market cap](https://mirror.xyz/brunny.eth/-0Jn0dD5868h_WshCirxJPyjBD6hQvqPL18blZrEbsU) in January; $310B Ether, $240B ERC20s, $25B synthetic assets and $9B NFTs
- Vitalik: [why Ethereum chose 12 second block times for PoS](https://old.reddit.com/r/ethereum/comments/slzfsd/why_wouldnt_proof_of_stake_drastically_reduce/hvu9ekc/) 

**Enterprise**

- [OnlyFans](https://www.reuters.com/article/onlyfans-nft-idUSKBN2KF2CZ) adds NFT profile pics
- [Ubisoft’s Rabbids](https://medium.com/sandbox-game/the-sandbox-partners-with-ubisoft-to-bring-rabbids-to-the-metaverse-c7c08fd1360e) to be used in the Sandbox

**Application layer**

- Maker crosses[10 billion DAI](https://twitter.com/makerdao/status/1491141179932491776)
- BarnBridge [SMART Alpha](https://medium.com/barnbridge/barnbridge-partners-with-optimism-to-launch-smart-alpha-pools-for-synthetix-and-chainlink-388bd207802e) live on Optimism, new 1-day pools
- [Set Protocol](https://medium.com/set-protocol/introducing-the-perpetual-protocol-v2-set-protocol-integration-on-optimism-ad527051875) integrates Perpetual Protocol v2 on Optimism
- [Aboard Exchange](https://blog.aboard.exchange/decentralized-derivative-exchange-aboard-is-live-on-arbitrum-mainnet-980b4c33acd7) (order book derivatives exchange) live on Arbitrum
- [Vesta Finance](https://twitter.com/vestafinance/status/1491290559025401857) live on Arbitrum
- Element Finance [Voting Vaults](https://medium.com/element-finance/voting-vaults-a-new-defi-and-governance-primitive-b4b2f6289d48): assign voting power to any contributor or value, such as locked positions
- Mirror [midwit](https://midwit.vercel.app/N4IgLgngDgpiBcIAmB7AxiANCNKB2YMBCA2qJLAiABYwCGSAlngOZYh1hgBOAzgqAA2MAG4xBCAIwBfbLgJEwpctDiJCADyXZNSxAFlGSAO6Ml0gLqyVlRFDrc6LR1Grt5hYvDLhVVXewBiAC2RqZgAASMvBF0eBEwGrDcjMGKEQBmKNwRuMEARszMLBF4Do5gjGIR4dQRvMEOkR6OaGC8AHQRAOoplayxMQCuvEN0ghFDBIwTEChDERQwESDWvrbgidogjdwA1vzeNmo4KEhwljpbVAD0LXRtq5jH-tdXWlQRANwAlBEAKtwIBEoCgoFBilF4nRSkMCjAcvlxChjF0ni91G8dg4Dsp1idBMw9uxODxDqBqNwYBkqNQuFBePAbjd+hAhtxBB08jcAExQAAcSAAnNwAMw0nQOFgwPQgAD6+UEcWJ0kumw+iAAYtk9hEAGQRACiTHMz3xrw+71li2o0RBTmWYBQiyBUUic3ZvHEGQ6qysZqWVHubU1UzajHwJK4fAEHCQSCpvEOIAADBoMhkhWhJPlJABWXMANh5hdFaELkiQKckAHYYDAhRlC3m0HmUzAACx0GDVySipA19zUOjMACSSCkchGTuCAEFCgg8ENBIJsIl7HhzhP4Blxl7sBkw5V8ABpGAQfwoPZEACqACVRwBhDswYySFhQFhIFh7FgAKT2WdVjWQM7AcJwXDcOR8E8PQfFA9VtiCEAAAkEWWBxll4FA0giUITDMCIWCGIwYBiJ1cloNBdXmMBEEsEC-EQfJl2EMAABlom2DxFDxBDCV4MBR0IYJ3Bg3ijnNMDHGcOhXDEhQvHgpjEPYXZcUk-iiSjMlY0palaXpRlmVZdlOW5Pl+TAOgAC8GUCKUZSoBUlTwFU1WQwwCFiHpsgnBj-QxEABKEkSFNgviVPsGTIPCiTlI2AJsHUw4EoJbTsFJGN4ApKkaUQOkwAZJkWWYNkOS5HDeRrDRuCmYweQc7hpVlFzlWAiwrSodiUBQSIAAoshyWckDEAh2TIn4-QYgMVJC4SYFE6DFLgoLooguSoNOFbIsSrEUt29K3J07LcoMgqjJK0yKosqAhQ0flRTzC9JWapzEDa47VU61TEAAZVtcQkH4AKZrW8DZPk5aIs0lSkt+kBujMOp8PCTAIg9XI4giKkGFiTcaj6ZYkE4GEMm4HDchg1p2nRuIkBxohzhyfAAFo0GHZg8JgJg6C6Q0kkEbIYHRobdQNHmzHR3hhypABCabZo2dbIa2nilKC+HkMAPg3ADy99EpNU5KcVSoLCWOzLo3JGg8sMorjNKvByvMqqIHyUUACtCwgDQXvARzWsVdrvq6gxGG4CmcjtW0UlYaarCAA): generate contract UI in a document, alpha, supports mainnet, Arbitrum & Optimism
- briq [alpha 1.0](https://twitter.com/briqnft/status/1491411425863954433) (building blocks to create NFTs on StarkNet): redesigned as semi-fungible tokens, resizable canvas, claim 1000 briqs
- [Looksmutable](https://looksmutable.com/): analyze mutability of NFT metadata by ENS or OpenSea link
- [RAC.fm](https://rac.fm/): web3 enabled music portal for RAC holders
- [Gummy](https://chrjentzsch.medium.com/lets-get-physical-nfts-59c7edc81998): link a physical object to an NFT using a verifiable anti-counterfeit sticker, available for beta testers

* * *

### **Job Listings**

- Roles at Gnosis [Sr DevRel Eng.](https://grnh.se/3052a2da2us) [Sr Production/Reliability Eng.](https://grnh.se/3345ebe02us) [DevOps Eng.](https://apply.workable.com/blockscout/j/0D9C5798DC/)
- [Nomic Foundation](https://www.notion.so/Nomic-Foundation-jobs-991b37c547554f75b89a95f437fd5056) hiring Rust Tech Lead & Ethereum Tech Lead
- [Re7 Capital](https://www.re7.capital/) – a DeFi yield fund – is hiring [analysts and data engineers](https://apply.workable.com/re7-capital/)
- Wanna build a cutting edge ETH Staking pipeline? [🅐ℙⓅ🄻ʸ for Ether Capital](https://bit.ly/ethcapdevops)
- [Senior Technical Writer](https://ethereum.bamboohr.com/jobs/view.php?id=51&source=weekinethnews) to take ownership & completely redo the Geth docs
- EF research hiring [Networking Engineer](https://ethereum.bamboohr.com/jobs/view.php?id=54&source=weekinethnews)
- [Internship program](https://nethermind.notion.site/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1) with Nethermind (1-3 month) 

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- [KPMG Canada adds Ether to balance sheet](https://www.newswire.ca/news-releases/kpmg-in-canada-adds-bitcoin-and-ethereum-to-its-corporate-treasury-851778842.html), along with carbon offsets
- RAC: why [NFTs matter to artists](https://twitter.com/rac/status/1490431018792226817)
- [BlackRock](https://www.coindesk.com/business/2022/02/09/blackrock-planning-to-offer-crypto-trading-sources-say/) plans to offer crypto trading

**General**

- [Couple arrested in relation to Bitfinex 2016 hack](https://www.justice.gov/opa/pr/two-arrested-alleged-conspiracy-launder-45-billion-stolen-cryptocurrency) for alleged conspiracy to launder $4.5 billion in Bitcoin
- [Binance $200m investment](https://www.forbes.com/sites/forbespr/2022/02/10/forbes-announces-200-million-strategic-investment-from-binance) in Forbes
- [US Senator reveals secret CIA bulk data collection](https://www.wyden.senate.gov/news/press-releases/wyden-and-heinrich-newly-declassified-documents-reveal-previously-secret-cia-bulk-collection-problems-with-cia-handling-of-americans-information) without oversight
- Proposal for [trustless BTC bridge creation](https://ethresear.ch/t/trustless-bitcoin-bridge-creation-with-witness-encryption/11953) with witness encryption
- [SHA256](https://sha256algorithm.com/): visually step through the algorithm
- Least Authority discloses [security vulnerabilities in Atomic Wallet](https://leastauthority.com/blog/disclosure-of-security-vulnerabilities-in-atomic-wallet/)

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-february-12-2022](https://weekinethereumnews.com/week-in-ethereum-news-february-12-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in **bold**)_**:**

- Feb 17 – [Schelling Point](https://schellingpoint.gitcoin.co/) (Denver) 
- Feb 18-20 – [ETHDenver](https://www.ethdenver.com/)
- Feb 23 – Mar 11 – [Codeless Conduct](https://codelessconduct.org/) no-code hackathon (virtual)
- Mar 9-24 – [Gitcoin Grants Round 13](https://twitter.com/gitcoin/status/1488231821854740481)
- Mar 11-20 – [Ethereum Rio](https://www.ethereum.rio/)
- Mar 15 – [Cryptocurrency Class](https://mirror.xyz/0xaFaBa30769374EA0F971300dE79c62Bf94B464d5/oGqGP2NOK9g7QPl1sMKkzql_Fh0P6hKbpYLZ-EkQTXU) starts (virtual) 
- **Mar 16 – submission deadline for [Underhanded Solidity Contest](https://underhanded.soliditylang.org/)**
- Mar 17-18 – [ETH Austin](https://2022.ethaustin.org/) summit
- Mar 29-31 – [ETHDubai](https://www.ethdubaiconf.org/)
- Apr 7-9 – [ETH Portland](https://2022.ethportland.com/) hackathon
- Apr 18-25 – [Devconnect (Amsterdam)](https://devconnect.org/schedule)
- Apr 22-24 – [ETHAmsterdam](https://amsterdam.ethglobal.com/)
- May 3-8 – [spaghettETH](http://spaghett-eth.com/) (Milan)
- May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
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

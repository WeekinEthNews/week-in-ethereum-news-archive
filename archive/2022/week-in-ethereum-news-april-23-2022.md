---
title: "Week in Ethereum News <br> April 23, 2022"
date: "2022-04-23"
---

## **Eth News and Links**

**Mainnet execution layer**

- Erigon [v20220402-alpha](https://erigon.substack.com/p/erigon-alpha-release-20220402-alpha): adds support for the merge & upgrade 1 for Erigon v2; need to sync from scratch as alpha not compatible with beta database 
- [Erigon architecture](https://erigon.substack.com/p/architecture-of-erigon-separable): components are separable and can run in same process

**Proof of Stake consensus layer**

- [$350k staking quadratic funding round](https://blog.clr.fund/350k-eth-staking-qf-round/) to fund open source public goods

**PoW switch off (the merge)**

- [mainnet shadow fork 2](https://github.com/eth-clients/merge-testnets/tree/main/mainnet-shadow-fork-2#mainnet-shadow-fork-2) transitions to PoS on April 23

**EIPs/Standards**

- [EIP5023](https://github.com/ethereum/EIPs/pull/5023/files): Shareable non-transferable NFT
- [EIP5022](https://github.com/ethereum/EIPs/pull/5022/files): Increase price of SSTORE from zero to non-zero to 40k gas
- [EIP5018](https://github.com/ethereum/EIPs/pull/5018/files): Directory standard
- [EIP5006](https://github.com/ethereum/EIPs/pull/5006/files): ERC1155 usage rights extension
- [EIP4931](https://github.com/ethereum/EIPs/pull/4931/files): Generic token upgrade standard

**Layer2**

- [KuCoin](https://www.kucoin.com/news/en-optimism-is-now-supported-on-kucoin-20220416) adds deposits to Optimism
- [EIP4844 reduces rollup data availability costs](https://medium.com/@cpbuckland88/4844-it-aint-all-gravy-fbae93bacf2) but assumes single honest party with access to recent rollup state
- [Proof of Validity Proof](https://ethresear.ch/t/a-design-of-decentralized-zk-rollups-based-on-eip-4844/12434) decentralized zk-rollup design based on EIP4844

* * *

### **This newsletter is made possible thanks to** [**Nexus Mutual**](https://nexusmutual.io/)**!**

![Nexus Mutual Protocol Cover](https://weekinethereumnews.com/wp-content/uploads/2022/03/Nexus-Mutual-Protocol-Cover-1024x586.png)

[](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fbcce9084-9c1f-408c-b907-a39fb47fd2ab_1600x915.png)

Go where the yield takes you, but don’t let the next hack set you back. Regardless of where you are chasing yield, Protocol Cover can protect your productive crypto assets across L1s, L2s, and scaling solutions. 

Maximize yield. Minimize risk. Enjoy peace of mind knowing Nexus Mutual has you covered. [Become a member](https://nexusmutual.io/) and cover your asse(t)s against the major risks in DeFi.

* * *

**Stuff for developers**

- [Guide to writing ERC20 tests](https://soliditydeveloper.com/foundry) in Foundry
- [Truffle for VS Code extension](https://trufflesuite.com/blog/build-on-web3-with-truffle-vs-code-extension/): deploy & debug contracts and run Ganache
- [Solidity square root](https://twitter.com/GaussianProcess/status/1516147690735738880): based on Solmate, ~50 gas cheaper on average
- [web3 cheatsheet](https://www.web3cheatsheet.xyz/): front end snippets using React, TypeScript and wagmi
- [Token gated image gallery tutorial](https://medium.com/pinata/how-to-use-sign-in-with-ethereum-and-nfts-to-build-a-token-gated-instagram-bb3752ccf597) using Sign-In with Ethereum
- [Semgrep](https://github.com/Raz0r/semgrep-smart-contracts#readme) (static analysis) rules for contracts based on DeFi exploits
- [Solidity Fuzzing Boilerplate](https://github.com/patrickd-/solidity-fuzzing-boilerplate#solidity-fuzzing-boilerplate): run fuzz tests with Echidna and Foundry
- Slither [v0.8.3](https://github.com/crytic/slither/releases/tag/0.8.3): Foundry support, markup contracts for Slither with custom natspec and tool to read storage values on-chain
- Vyper [v0.3.2](https://twitter.com/vyperlang/status/1515719040978857984): dynamic arrays & full ABI type support; 3 vulnerabilities disclosed
- OpenZeppelin [Contracts Wizard for Cairo](https://wizard.openzeppelin.com/cairo): ERC20 & ERC721 support
- [Amarna](https://blog.trailofbits.com/2022/04/20/amarna-static-analysis-for-cairo-programs/): Cairo static analyzer and linter
- [Livepeer](https://camiinthisthang.hashnode.dev/the-developers-guide-to-getting-started-with-livepeer) starter guide
- [Testnet reminder](https://twitter.com/trent_vanepps/status/1516716106467229699): Ropsten will be upgraded to PoS; Ropsten & Rinkeby will be deprecated; use Goerli & Sepolia testnets

**Security**

- Beanstalk $76 million [exploit](https://twitter.com/kelvinfichter/status/1515735674703470595), flash loan used to execute malicious governance proposal that drained liquidity pools

**Ecosystem**

- [Ethereum Foundation report](https://ethereum.foundation/report-2022-04.pdf) \[PDF\]: 
    - philosophy of long term thinking, subtraction and values stewardship
    - supports ecosystem via EF teams, grants, delegated domain allocators and third party funding
    - spent $48 million in 2021, treasury of $1.6 billion with 80.5% in ETH
- [Project Sunshine](https://ethsunshine.com/) decentralization dashboard; consensus & execution client diversity; overall health rated at 61%
- [Apple ID phishing scam](https://twitter.com/Serpent/status/1515545806857990149) obtained secret recovery phrase from MetaMask password encrypted vault in iCloud backup
- Rarible [wormable cross-site scripting vulnerability](https://palisade.consulting/blog/rarible-vulnerability) disclosed and patched
- [NFT arbitrage searcher](https://twitter.com/bertcmiller/status/1517278228918018049) bought Moonbird for 44 ETH then sold for 240 ETH in the same transaction
- [Etherscan filters](https://twitter.com/etherscan/status/1515689467117461507): filter transactions by function name, block & age
- Barry Whitehat: proposal for [private binding negotiations](https://ethresear.ch/t/private-binding-negotiations/12426) using decentralized dark pool and advanced MPC & ZKP tooling

**Enterprise**

- [Budweiser using ENS subdomain](https://twitter.com/budweiserusa/status/1517151154978705414) on Twitter, shares Budverse roadmap
- [Jimmy Fallon](https://twitter.com/ethleaderboard/status/1516518590932946945) adds ENS to Twitter, tops leaderboard with most followers

**Application layer**

- [Coinbase NFT](https://blog.coinbase.com/gm-coinbase-nft-is-now-in-beta-25e6c052aa43): beta, trading by invite code only, no marketplace fee initially
- LooksRare [Listing Rewards](https://docs.looksrare.org/blog/looksrare-listing-rewards-list-nfts-earn-looks) for listing top 25 NFTs within 1.5x of floor price
- Index Coop [JPG](https://indexcoop.com/blog/announcing-the-launch-of-jpg-an-nft-index): NFT index token
- [Bored Brothers](https://www.sound.xyz/boredbrothers/drip): two Apes in animated band release single on Sound
- Moonbirds NFT [explainer](https://fortune.com/2022/04/18/moonbird-nft-collection-surge/)
- [MISO v2](https://medium.com/sushiswap-org/its-here-miso-v2-a-permissionless-multi-chain-launchpad-da7e840da397) (permissionless token launchpad) live on mainnet and Arbitrum
- [Pegasus Finance](https://twitter.com/0xPegasusFi/status/1516478741265862657) (interest rate perpetual) live on Optimism
- [Fiat](https://medium.com/fiat-dao/let-there-be-light-fiat-is-live-85b90fe210b4) (fixed income collateral stablecoin) live on mainnet
- Zodiac [Exit app](https://gnosisguild.mirror.xyz/6CnO4NQYqpF_gPTj3XWJeSmXG3InaTSg-MpgNtaHE0s): interface to DAO Exit module

* * *

### **Job Listings**

- Status Waku is hiring: [TypeScript Protocol/Software Engineer & DevRel](https://jobs.status.im/?gh_jid=4143735&gh_src=55c532491us)
- Ethereum Foundation need a [People Operations Lead](https://jobs.lever.co/ethereumfoundation/8046bbe5-6343-4ecf-8296-37dc2a5bf915?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- Status are hiring [engineers who focus on incentive design](https://jobs.status.im/?gh_jid=3706505)
- Vac @ status are looking for [protocol engineers](https://jobs.status.im/?gh_jid=3693623) 
- OpenZeppelin are hiring a [Director of Development - Contracts](https://openzeppelin.com/jobs/opening/?gh_jid=5078928003)
- Ethereum Foundation seek a generalist [ecosystem developer](https://jobs.lever.co/ethereumfoundation/6b80a26f-7db3-4415-8339-a3543a967998?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- [Internship program](https://nethermind.notion.site/Nethermind-Internship-Program-4eb494969aa24afa9181223e958522d1) at Nethermind (1-3 month) 
- EF’s Privacy & Scaling Explorations team: [Web3 Engineer](https://jobs.lever.co/ethereumfoundation/ece6534a-b946-4996-b7e7-713bd1ec0353?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)
- EF Ecosystem Support team: [Communications](https://jobs.lever.co/ethereumfoundation/4b0c3305-cf03-4e33-9bfb-63e4ec6f3a68?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum), [Analyst](https://jobs.lever.co/ethereumfoundation/64361391-9a74-49ed-b37c-8ff35931430e?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum) & [Admin Assistant](https://jobs.lever.co/ethereumfoundation/5684f7ea-c3ad-4703-b86c-462964f49392?lever-origin=applied&lever-source%5B%5D=Week%20in%20Ethereum)

**Reach developers experienced with Ethereum.  $600** for four issues (~75 character limit), payable in ETH/DAI/USDC to abcoathup.eth on mainnet, Arbitrum or Optimism.  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- To comply with EU sanctions [Binance restricts Russian accounts](https://www.binance.com/en/support/announcement/4887e569afdf4b1e89e024371d3a49b9) over 10k EUR value to withdrawal only
- [a16z announces Crypto Research](https://a16z.com/2022/04/21/announcing-a16z-crypto-research/) lab headed by Tim Roughgarden
- [Atari terminates license](https://www.globenewswire.com/news-release/2022/04/18/2423873/0/en/Atari-Announces-Planned-Creation-of-New-Token-and-Termination-of-Joint-Venture.html) for Atari token, plans another token

**General**

- US CISA [Cybersecurity Advisory](https://www.cisa.gov/uscert/ncas/alerts/aa22-108a): North Korean groups targeting crypto
- [Stripe pilots crypto payouts](https://stripe.com/blog/expanding-global-payouts-with-crypto) with Twitter
- [Java ECDSA vulnerability](https://neilmadden.blog/2022/04/19/psychic-signatures-in-java/): signature based security mechanisms could be bypassed
- [Mine for malicious domains](https://twitter.com/sniko_/status/1516163027527254020) by checking new SSL certificates
- [Candiru spyware used zero-day vulnerabilities](https://catalonia.citizenlab.ca/) to spy on Catalan citizens
- George Hotz: [how to vampire attack Twitter](https://geohot.github.io//blog/jekyll/update/2022/04/16/vampire-attack-twitter.html) using a token

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) and [@abcoathup](https://twitter.com/abcoathup) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-april-23-2022](https://weekinethereumnews.com/week-in-ethereum-news-april-23-2022)

* * *

## **Dates of Note**

Upcoming dates of note _(new/changes in_ **_bold_**_)_**:**

- May 1 – application deadline for [yAcademy’s auditor fellowship](https://yacademy.dev/fellowship-program/)
- May 3-5 – [Spaghett ETH](https://spaghett-eth.com/) (Milan)
- May 6-27 – ETHGlobal [Hack Money](https://defi.ethglobal.com/)
- May 8 – deadline for [EF academic grants round](https://esp.ethereum.foundation/academic-grants)
- May 17-20 – [EY Global blockchain summit](https://pub.ey.com/public/2021/2112/2112-3933703/blockchain-summit-2022/index.html)
- May 20 – US Fed CBDC discussion paper [feedback](https://www.federalreserve.gov/apps/forms/cbdc) deadline
- **Jun 10 –** [**Austin DeFi**](https://2022.austindefi.org/) **summit**
- Jun 10-12 – [ETHPrague](https://ethprague.com/)
- Jun 20-23 – [NFT.NYC](https://www.nft.nyc/)
- Jun 24-26 – [ETH NYC](https://nyc.ethglobal.co/)
- Jul 8 – [ETH Seattle](https://2022.ethseattle.org/) summit
- Jul 19-21 – [EthCC 5](https://ethcc.io/) (Paris)
- **Aug 5-7 –** [**ETH Seoul**](https://2022.ethseoul.org/)
- Aug 19-21 – [ETHMexicoCity](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Aug 27-28 – [DeFi Security Summit](https://defisecuritysummit.org/) (Stanford)
- **Aug 28 –** [**DeFi San Francisco**](https://2022.defi-sf.com/) **summit**
- Aug 29-31 – [Science of Blockchain Conference](https://cbr.stanford.edu/sbc22/) (Stanford)
- Sep 1-4 – [ETHWarsaw](https://ethwarsaw.dev) (hackathon & conference)
- Sep 6-9 – [MCON 2](https://www.mcon.fun/) (Denver)
- Sep 12-14 – [DappCon](https://www.dappcon.io/) (Berlin)
- Oct 11-14 – [Devcon 6](https://blog.ethereum.org/2022/02/18/colombia-in-2022-redux/) (Bogotá)
- Nov 4-6 – [ETHSanFrancisco](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)
- Dec 1-4 – [ETHDownUnder](https://ethdownunder.com/) (Sydney)
- Dec 2-4 – [ETHTaipei](https://ethglobal.medium.com/announcing-the-ethglobal-2022-season-51a7906bb3a4)

**Did you get forwarded this newsletter?** [_Sign up_](https://weekinethereum.substack.com/subscribe#about) **_to receive it weekly_**

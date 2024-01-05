---
title: "Week in Ethereum News <br> September 9, 2023"
date: "2023-09-09"
---

## Eth News and Links

**Dencun (Cancun + Deneb) upgrade**

- Latest all core devs – consensus (ACDC) [call video](https://www.youtube.com/watch?v=zODMnGxQBG0&t=438s). Notes from [Christine Kim](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-117/):
    - Testing continues on devnet-8
    
    - Devnet-9 planned for Tuesday September 19
    
    - EIP4844 blobs per block: [big block analysis](https://docs.google.com/presentation/d/1glx__evliifIRyS3GnbzADd0rVPV4CFPh92INEsRdX8) presented, no changes to 3/6 (target/max) yet
    
    - Proposed addition to Dencun (open for community input): [max epoch churn limit](https://twitter.com/philngo_/status/1699805844748030383) as a short term fix to validator set size growth, discuss on ACDE whether to include in Dencun

**Centralization watch: threatening the value of your ETH**

- **🚨** [**Lido at 32.4%**](https://dune.com/hildobby/eth2-staking) **is very close to breaching risky** [**33% threshold**](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

- Client diversity (via [clientdiversity.org](https://clientdiversity.org/#distribution)):
    - Execution layer: Geth supermajority, could possibly cause a chain split
    
    - Consensus layer: Prysm & Lighthouse over 33%, a bug could mean loss of finality

- Need more [geographic diversity for both stakers and nodes](https://nodewatch.io/), particularly outside of US/Can/EU

**Layer 1**

- [Mempool dumpster](https://github.com/flashbots/mempool-dumpster#readme): exports transactions from EL node transaction pools in Parquet & CSV format

- MEV-Boost:
    - [Strong builder identity](https://ethresear.ch/t/strong-builder-identity-for-combating-builder-imposter-attacks/16550): proposal to combat imposter attacks (Titan had an imposter)
    
    - Prestwich: [proposers & builders could collude](https://prestwich.substack.com/p/has-anyone-checked-on-eip-1559-recently) on gas limit to minimize base fees

- [Whisk devnet](https://twitter.com/dapplion/status/1700222295719952534): proof of concept Single Secret Leader Election (SSLE) on fork of Lighthouse + Geth

**For Stakers**

- [Staking directory](https://twitter.com/stakedirectory/status/1699346477598843269): adds info for liquid staking on network share & self-limit pledges

**Client releases for Holešky testnet**

- Consensus layer:
    - Lighthouse [v4.4.1](https://github.com/sigp/lighthouse/releases/tag/v4.4.1)
    
    - Lodestar [v1.11.1](https://github.com/ChainSafe/lodestar/releases/tag/v1.11.1)
    
    - Teku [v23.9.0](https://github.com/Consensys/teku/releases/tag/23.9.0)

- Execution layer:
    - Besu [v23.7.2](https://github.com/hyperledger/besu/releases/tag/23.7.2)
    
    - Erigon [v2.49.0](https://github.com/ledgerwatch/erigon/releases/tag/v2.49.0)
        - Otterscan [v2.0.0 alpha](https://github.com/otterscan/otterscan/releases/tag/v2.0.0): adds in-node token indexers

**Research**

- Terence’s [EIP4844+](https://hackmd.io/@ttsao/ByhnIFXR2) (ideas for extending blobs after Dencun upgrade): erase code to increase target/max blobs to 6/12 and apply data availability sampling

- [PeerDAS](https://ethresear.ch/t/peerdas-a-simpler-das-approach-using-battle-tested-p2p-components/16541): data availability sampling approach reusing p2p components to scale without DHT

- Barnabe: [inclusion list games](https://ethresear.ch/t/fun-and-games-with-inclusion-lists/16557), builders may be incentivised to stuff blocks and proposers may try to bribe/extort each other

**Layer 2**

- Base [delay in block production](https://status.base.org/incidents/n3q0q4z24b7h) for 45 minutes

- Barry Whitehat’s [Plasma Free](https://ethresear.ch/t/plasma-free/16570) proposal: free transactions but if data is unavailable users need to make a forced transaction (users online assumption)

**EIPs/Standards**

- EIPs
    - [EIP7514](https://github.com/ethereum/EIPs/pull/7668/files): Add max epoch churn limit

- ERCs (application layer):
    - [ERC7507](https://github.com/ethereum/EIPs/pull/7634/files): Multi-user NFT extension (ERC721 extension)
    
    - [ERC7508](https://eips.ethereum.org/EIPS/eip-7508): Dynamic onchain token attributes repository
    
    - [ERC7509](https://github.com/ethereum/EIPs/pull/7651/files): Entity component system
    
    - [ERC7510](https://github.com/ethereum/EIPs/pull/7638/files): Cross-contract hierarchical NFT (ERC721 extension)
    
    - [ERC7511](https://eips.ethereum.org/EIPS/eip-7511): Minimal proxy contract with PUSH0
    
    - [ERC7512](https://eips.ethereum.org/EIPS/eip-7512): Onchain representation for audits
    
    - [ERC7513](https://github.com/ethereum/EIPs/pull/7656/files): NFT-bound modularized contract (ERC1155 extension)

* * *

### **Check out** [**web3 Builders Podcast**](https://podcasters.spotify.com/pod/show/web3builderspodcast) 

![Web3 Builders](https://weekinethereumnews.com/wp-content/uploads/2023/08/Web3-Builders.webp)

Check out Will and Evan’s interviews with the [honest actors](https://twitter.com/evan_van_ness/status/1699825569041350744) of Ethereum: [Austin Griffith](https://podcasters.spotify.com/pod/show/web3builderspodcast/episodes/Stealing-Web2s-Developers-With-Austin-Griffith-e280fvo), [Ameen Soleimani](https://podcasters.spotify.com/pod/show/web3builderspodcast/episodes/Tornado-Devs-Jailed-for-Writing-Code--With-Ameen-Soleimani-e28ghir), and [Vitalik Buterin](https://podcasters.spotify.com/pod/show/web3builderspodcast/episodes/Vitalik-Buterin-On-Twitter--Cryptos-Main-Characters--and-Making-Ethereum-Apps-Censorship-Resistant-Part-1-e291foq) (part 1).  

Or listen to our weekly news show. On [this week’s episode](https://podcasters.spotify.com/pod/show/web3builderspodcast/episodes/Evan-vs--Everybody--MakerDAOs-Solana-Pivot-and-Fixing-Bitcoins-Security-Budget-e292sep): Lido attempting to add backdoor onchain governance to Ethereum, Bitcoin mining adjustment and declining security budget, and Rune’s announcement of a far-off Maker appchain.

* * *

**Stuff for developers**

- Foundry:
    - Forge-std [v1.6.1](https://github.com/foundry-rs/forge-std/releases/tag/v1.6.1): new cheat codes to get keys of a mapping, filesystem cheats & JSON parsing 
    
    - [Catapulta](https://www.reddit.com/r/ethdev/comments/16d3jma/meet_catapulta_your_automation_tool_for_foundry/) (Foundry deployment automation): abstracts RPC config & Etherscan keys, free during alpha
    
    - [Solpretty](https://github.com/devtooligan/solpretty#readme): Solidity library for pretty printing numbers

- RareSkills: [gas optimization](https://www.rareskills.io/post/gas-optimization) guide

- Guide to [Vyper compilation pipeline](https://hackmd.io/@pcaversaccio/how-vyper-compiles-into-bytecode)

- [Ape-roll](https://github.com/fp-crypto/ape-roll#readme): weiroll (operation-chaining/scripting language) client for Ape Framework

- ApeWorX [cHaOSneT](https://twitter.com/ApeFramework/status/1700221649084129644) (beta): paid testnet service with simulated activity using bots

- Heimdall-rs [v0.5.3](https://github.com/Jon-Becker/heimdall-rs/releases/tag/0.5.3): increased decoding accuracy and adds flag to help decode transactions with non-standard byte sizes

- [Privacy playgrounds](https://tonk.notion.site/Eternal-Privacy-Playgrounds-6cb0ebb4042b42888a15a112a7040cbe) (wiki): hidden information mechanics for onchain games

**Security**

- Stake (gambling) [$41 million stolen](https://rekt.news/stake-rekt/) from mainnet & sidechain hot wallets; [FBI blames Lazarus](https://www.fbi.gov/news/press-releases/fbi-identifies-lazarus-group-cyber-actors-as-responsible-for-theft-of-41-million-from-stakecom)

- GMBL Computer on Arbitrum [~$1 million exploit](https://gmblcomputer.medium.com/gmbl-computer-exploit-postmortem-a09aa3297405) via referral system

- FloorDAO [40 ETH exploit](https://twitter.com/FloorDAO/status/1699078468678377679) via backlog of rebases

**Ecosystem**

- Paper on [privacy pools](https://twitter.com/ameensol/status/1699424914229321966) (authors include Vitalik & Ameen Soleimani): users can prove regulatory compliance without revealing their entire transaction history

- [ERC4337](https://mirror.xyz/erc4337official.eth/hRn_41cef8oKn44ZncN9pXvY3VID6LZOtpLlktXYtmA) (account abstraction) grant recipients

- Hackathon projects: [ETHWarsaw](https://ethwarsaw-2023.devpost.com/project-gallery) and [Ethcon Korea](https://ethcon-korea.devfolio.co/projects)

**Onchain stats**

- Gas fees (via [ultrasound.money](https://ultrasound.money/#gas)): 7.8 to 88.9 gwei, with 15.7 gwei average
    - Negative issuance currently at 20.4 gwei 
    
    - 3.6k ETH net issuance this week

- [ETHUSD](https://www.coingecko.com/en/coins/ethereum): $1615-1653, currently $1635

- [ETHBTC](https://ratiogang.com/): 0.0627-0.0636, currently 0.0631 (Flippening at ~0.16)

**Notable at app layer**

- [USDC](https://twitter.com/circle/status/1699045142429319321) native on Optimism & Base

- Kain proposes [Synthetix experiment with expansion](https://mirror.xyz/kain.eth/tAXGVKMTYM8K2gUOQq9JDQ1wyV_5Msdlrn_AtmiCGEI), on Base with ETH collateral

- [Kevin Owocki](https://twitter.com/owocki/status/1699056199445221437) returning to Gitcoin

- Nouns DAO [fork #0](https://nouns.wtf/fork/0) started (fork [explainer](https://mirror.xyz/verbsteam.eth/iN0FKOn_oYVBzlJkwPwK2mhzaeL8K2-W80u82F7fHj8): enables 20%+ to exit their share of the treasury together)

- [TryENS](https://twitter.com/mailchain_xyz/status/1699052271022363079): create a temporary ENS subdomain, expires after 48 hours

- [Hashmarks](https://hashmarks.deafbeef.com/): fading SVG NFTs that require refreshing using the physical sculpture

- [Vaults.FYI](https://www.vaults.fyi/): find the best yield (with or without farming incentives) for your assets 

* * *

### Job Listings

- [Product Manager - L2 Blockchain Effort](https://grnh.se/48614a711us) @ Status: [All jobs](https://grnh.se/9fc6e6fc1us)

- EF are hiring a [Senior Operations Security Expert](https://jobs.lever.co/ethereumfoundation/10923b49-c76a-47b9-bd27-96ee71a460db)

- [ZK circuits engineer](https://jobs.lever.co/ethereumfoundation/7a7da3a9-a080-40a9-8aed-9e81641650a4) sought by EF Privacy & Scaling Explorations team

**Job listings: $600 for four issues** (75 character limit).  Questions? abcoathup at-gmail

* * *

**Regulation/business/tokens**

- CFTC:
    - [DeFi regulation by enforcement](https://www.cftc.gov/PressRoom/PressReleases/8774-23) against Opyn (despite blocking US IP addresses), Deridex & 0x
        - [Commissioner Mersinger](https://www.cftc.gov/PressRoom/SpeechesTestimony/mersingerstatement090723) dissent
    
    - [Commissioner Pham](https://www.cftc.gov/PressRoom/SpeechesTestimony/opapham9) calls for a US regulatory sandbox

- [International Organization of Securities Commissions](https://www.iosco.org/news/pdf/IOSCONEWS706.pdf) (IOSCO) DeFi policy recommendations

- [IMF and FSB](https://www.fsb.org/2023/09/imf-fsb-synthesis-paper-policies-for-crypto-assets/) policies for crypto assets, warns against blanket bans

- [Ark Invest & 21Shares](https://www.sec.gov/Archives/edgar/data/1992508/000119312523229449/d450565ds1.htm) apply for spot Ether ETF

**General**

- [Crypto wealth report](https://www.henleyglobal.com/publications/crypto-wealth-report): 22 billionaires, 182 centi-millionaires & 88,200 millionaires

- [Google’s Threat Analysis Group](https://blog.google/threat-analysis-group/active-north-korean-campaign-targeting-security-researchers/) warns North Korea targeting security researchers

- [Blastpass](https://citizenlab.ca/2023/09/blastpass-nso-group-iphone-zero-click-zero-day-exploit-captured-in-the-wild/): iPhone zero-click exploit, update your Apple devices

- [Proton mail](https://www.sonarsource.com/blog/code-vulnerabilities-leak-emails-in-proton-mail/) vulnerability disclosed, fixed

* * *

Follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked links are. Follow [@abcoathup](https://twitter.com/abcoathup) and [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week’s news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-september-9-2023](https://weekinethereumnews.com/week-in-ethereum-news-september-9-2023)

* * *

## Upcoming Dates of Note

_(new/changes in_ **_bold_**_)_

- Sep 10-12 – [Ethereum Singapore](https://www.ethereumsingapore.com/) hackathon & conference

- Sep 11-13 – [DappCon](https://www.dappcon.io/) (Berlin)

- Sep 15 – [Protocol Berg](https://protocol.berlin/) (Berlin)

- Sep 15-17 – [ETHChicago](https://www.ethchicago.xyz/) conference & hackathon

- Sep 15 – [Holešky testnet](https://github.com/eth-clients/holesky#readme) genesis

- Sep 18-23 – [ETHSafari](https://ethsafari.xyz/) (Kilifi Kenya)

- Sep 21–24 – [Pragma](https://ethglobal.com/events/pragma-newyork) & [ETHGlobal New York](https://ethglobal.com/events/newyork2023)

- Oct 5-6 – [ETHMilan](https://www.ethmilan.xyz/) conference

- Oct 6-8 – [ETHRome](https://ethrome.org) hackathon

- Oct 6-27 – [ETHOnline](https://ethglobal.com/events/ethonline2023) (ETHGlobal) virtual

- Oct 13-15 – [Ethereum Kuala Lumpur](https://hack.ethkl.org/) conference & hackathon

- Oct 21 – [Ethereum México](https://twitter.com/ethereum_mexico/status/1684649652639924224)

- Oct 22-24 – [ETH Hong Kong](https://www.ethhongkong.co/)

- Oct 27-29 – [ETH Miami](https://ethmiami.net/) festival & hackathon

- Oct 27-29 – [ETH Vietnam](https://www.eth-vietnam.com/)

- Oct 27-29 – [ETH London](https://www.encode.club/eth-london) hackathon

- Oct 28-30 – [Paradigm CTF](https://ctf.paradigm.xyz/)

- Oct 31 – [Road to Devcon grants](https://blog.ethereum.org/2023/06/29/road-to-devcon7-grants) deadline (max $1k for local meetups)

- Nov 3-5 – [ETH Lisbon](https://www.ethlisbon.org/) hackathon

- Nov 3-5 – [ETHBrno](https://ethbrno.cz)

- Nov 13-19 – [Devconnect](https://devconnect.org/) (Istanbul)

- Nov 16-19 – [Pragma](https://ethglobal.com/events/pragma-istanbul) & [ETHGlobal Istanbul](https://ethglobal.com/events/istanbul)

- Dec 4-5 – [ETHVenice](https://ethvenice.com/)

- Dec 8-10 – ETHGlobal [ETHIndia](https://ethindia.co/) (Bangalore) 

[_Sign up_](https://weekinethereum.substack.com/subscribe#about) _to receive this newsletter weekly_

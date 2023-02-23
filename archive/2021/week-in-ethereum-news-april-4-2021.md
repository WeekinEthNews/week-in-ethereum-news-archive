---
title: "Week in Ethereum News <BR> April 4, 2021"
date: "2021-04-04"
---

## **Eth News and Links**

**Mainnet**

- Latest [core devs call](https://www.youtube.com/watch?v=V-Qz4UN6Z88&t=710s). Beiko’s [notes](https://twitter.com/TimBeiko/status/1378025331605434369): Berlin on track for [April 14 or 15](https://goto.etherscan.com/block/countdown/12244000) (block 12244000).
    - London testnet [Aleut](https://github.com/ethereum/eth1.0-specs/blob/master/client-integration-testnets/aleut.md) to include EIP1559 and EIP3198 (BASEFEE opcode). EIP3238 (difficulty bomb delay) must also be in London.
    - Potential London/Shanghai EIPs include: EIP3403 (disable gas refunds), EIP3074 (AUTH and AUTHCALL) and EIP2537 (BLS precompile)
- EthereumJS VM [v5.3.0](https://github.com/ethereumjs/ethereumjs-monorepo/releases/tag/%40ethereumjs%2Fvm%405.3.0) with EIP-2930 Access List generation + a new Block Builder API
- Dan Finlay on [safety of EIP3074 AUTH and AUTHCALL opcodes](https://ethereum-magicians.org/t/eip-3074-auth-and-authcall-opcodes/4880/61?u=danfinlay) and Alexey’s response
- [EIP2537 and EVM384](https://docs.google.com/document/d/1DdA1IxSDK5ppC1C2W9uvMW66Y8VToc-vPV5B68ZQvOg) paths for enabling BLS12-381 support
- [EVM384 update](https://notes.ethereum.org/--JjliY8T_-qIdvAQKQlcg?view): benchmarks vs precompile
- Proposed opcode [GASMETER](https://ethresear.ch/t/new-opcode-gasmeter-as-a-step-towards-removing-gas-and-gas-observability/9067) to allow removing GAS opcode
- [Make eip1559 more like an AMM curve](https://ethresear.ch/t/make-eip-1559-more-like-an-amm-curve/9082) (this is for the future; not going into the 1559/London upgrade)
- Stateless Ethereum [updated roadmap](https://ethresear.ch/t/an-updated-roadmap-for-stateless-ethereum/9046): prioritizing allowing stateless stakers and constraining state growth

**EIPs/Standards**

- [EIP3447](https://github.com/ethereum/EIPs/issues/3447): New transaction parameter for latest block number inclusion
- [EIP3448](https://github.com/ethereum/EIPs/pull/3448): MetaProxy Factory Standard
- [EIP3450](https://github.com/ethereum/EIPs/pull/3450): Shamir + BIP-39

**Proof of Stake**

- Danny Ryan’s [Finalized](https://blog.ethereum.org/2021/04/02/finalized-no-25/) PoS update: the effort to turn off PoW is making progress, plus a reminder of RfP for PoS security and testing.
- Guido Vranken’s fuzzing found a [bug in the blst library’s inverse function](https://github.com/supranational/blst/security/advisories/GHSA-x279-68rr-jp4p). **Update your staking clients to latest version** (just to be on the safe side).
- What’s necessary to [turn off PoW from a mainnet client perspective](https://hackmd.io/@n0ble/ethereum_consensus_upgrade_mainnet_perspective)
- [Turning off PoW (“Merge”) implementer call](https://www.youtube.com/watch?v=b3hfgLa_GHw)
- Prysm’s [merge demo](https://hackmd.io/@prysmaticlabs/prysm-catalyst-interop) using Catalyst (Geth fork)
- Vitalik: [cap active validators](https://www.reddit.com/r/ethereum/comments/mgq07y/capping_the_number_of_actively_attesting) so that devs can safely make assumptions about non-finalizing edge cases
- [Rayonism](https://rayonism.io/): an ambitious Scaling Eth hackathon project to create testnets to turn off PoW AND add data shards with rollup integrations

**Layer2**

- [Understanding Arbitrum's design](https://developer.offchainlabs.com/docs/inside_arbitrum)
- zkSync [roadmap update](https://medium.com/matter-labs/zksync-2-0-roadmap-update-zkevm-testnet-in-may-mainnet-in-august-379c66995021): EVM on zkrollup, plan public testnet in May. They’ll also have NFTs on their mainnet in May
- [ELI5 of Celer’s layer2.finance](https://blog.celer.network/2021/04/02/eli5-layer2-finance-the-modern-subway-of-the-defi-city/): move your money to rollup and the rollup batches DeFi transactions

* * *

### **This newsletter is made possible thanks to [Uniswap](https://app.uniswap.org/)!**

[![](https://weekinethereumnews.com/wp-content/uploads/2021/04/2021-04-04-1024x355.png)](https://airtable.com/shrEXXxXB1humz7VS)

[Uniswap grants](https://twitter.com/uniswapgrants): Whether it’s enhancing the TWAP Oracle (V3 oracles provide time-weighted average prices on demand for any period within the last ~9 days!) or making V3 even more usable upon launch, submit your application and get in touch!

For more ideas for grants [check out our list of RFPs](https://www.notion.so/RFPs-Challenges-3be614ba4e504b5caeee7b0159e64a42)

* * *

**Stuff for developers**

- Compound's new [governance code (Bravo)](https://twitter.com/compoundfinance/status/1376905836539355142) is live, more tunable and with more features
- Slither [v0.7.1](https://github.com/crytic/slither/releases/tag/0.7.1), solc version recommendations increased to 0.7.6
- Prepare smart contracts for Berlin Hardfork with [Tenderly](https://blog.tenderly.co/prepare-your-smart-contracts-for-the-berlin-hardfork-with-tenderly/), now includes Access List Tool
- [Solar](https://blog.trailofbits.com/2021/04/02/solar-context-free-interactive-analysis-for-solidity/): interactive analysis tool
- Making [Flashbots work in the browser](https://kndrck.co/posts/making_flashbots_work_in_browser/)
- [4byte](https://www.npmjs.com/package/4byte) npm: look up an Ethereum function sig from its 4 byte hash
- [dharmaOS](https://github.com/dharmaprotocol/dharmaOS): an SDK to connect any EVM protocol action to Dharma’s (currently US only) payment rails.

**Security/incidents**

- [Solutions to Paradigm’s CTF](https://github.com/paradigm-operations/paradigm-ctf-2021)
- Blocksec [list of security incidents](https://github.com/openblocksec/blocksec-incidents)
- samczsun: Importance of client consensus via a [bug in uncle validation](https://samczsun.com/the-block-mined-in-january-584942419325/)

**Ecosystem**

- [Flashbots.tools](https://flashbots.tools/): a Flashbots frontend to easily execute a gasless ERC20 token transfer from your browser
- [27% of Eth hashpower](https://twitter.com/thegostep/status/1377312654507773958) is now in Flashbots, so remember to be [careful when providing liquidity](https://twitter.com/epheph/status/1376934206547271685)
- Is [Oracle Extractable Value](https://twitter.com/haydenzadams/status/1377431421573234689) the new Miner Extractable Value? [Maker’s strategies to thwart malicious oracles](https://twitter.com/nanexcool/status/1377449453553082368)
- Devcon [Attendee Survey](https://docs.google.com/forms/d/e/1FAIpQLSffvoFeaada3u2n6mGKOy7hIJjbnwPUB-N-USCxCYmKcyehFw/viewform) with POAP for completion
- Vitalik's [review of Gitcoin Grants round 9](https://vitalik.ca/general/2021/04/02/round9.html); make bribes and retroactive airdrops cryptographically impossible using [MACI](https://github.com/appliedZKP/maci)
- [Astrodrop](https://whalerdao.github.io/astrodrop/): Merkle tree airdrop for just 212k gas
- [Traffic to ethereum.org is up 4x](https://twitter.com/samonchain/status/1378034008529858564) since December

**Enterprise**

- Visa [transactions settled with USDC](https://usa.visa.com/visa-everywhere/blog/bdp/2021/03/26/digital-currency-comes-1616782388876.html) on Eth mainnet

**Application layer**

- Algo stablecoin [Fei launched on mainnet](https://medium.com/fei-protocol/what-you-should-know-about-fei-3ccffd4a4bb6), got oversubscribed with ~$1.2b in ETH (eg meaning Fei launched at $1.01) [leading to some instability](https://twitter.com/jonwu_/status/1378534945900134400)
- RAC’s NFT sale makes ~$700k “[more than I've received for 3 albums / 10yrs of work](https://twitter.com/RAC/status/1375630706479558658)” as a musician
- Ex-Ujo Jack Spallone’s [31 ideas for music and crypto](https://twitter.com/JackSpallone/status/1377423491746557955)
- ConsenSys announced an [NFT sidechain](https://consensys.net/blog/press-release/palm-a-new-nft-ecosystem-and-studio-for-creators-announces-launch-of-first-project-with-damien-hirst/) which will feature Damien Hirst
- After last weekend’s skit, of course [Saturday Night Live sells an NFT](https://opensea.io/collection/saturday-night-live) this week
- [Overly Attached Girlfriend meme](https://twitter.com/laina622/status/1378511072080982016) goes for 200 Eth (~$400k)
- What is [fungibility in tokens](https://blog.oceanprotocol.com/on-difficult-to-explain-fungibility-sightings-in-nfts-26bc18620f70)?
- [Ether Freakers](https://twitter.com/jmflatow/status/1375543196013490180), like CryptoKitties but with a game. No frontend yet.

**Regulation/business/tokens**

- Coinbase [listing set for April 14](https://blog.coinbase.com/coinbase-announces-effectiveness-of-registration-statement-and-anticipated-listing-date-of-its-1509b281f760)
- [Tether assurance opinion](https://tether.to/assurance-opinion-mar-21/) from Cayman accounting firm
- Burniske: the [original sin of many crypto projects](https://www.placeholder.vc/blog/2021/4/1/the-original-sin) is unequal distribution
- List of the biggest DAO [war chests](https://open-orgs.info/)

**General**

- Participate in the [multi-party computation ceremony for zkopru](https://thore-hildebrandt.medium.com/zkopru-trusted-setup-ceremony-f2824bfebb0f). It’s very easy!
- [Dharma](https://twitter.com/Dharma_HQ/status/1376660977735794689) wallet adds $25k fiat into DeFi with a tap and massive gas savings via batching (fiat rails sadly US only at the moment)
- PayPal launches [checkout with crypto](https://newsroom.paypal-corp.com/2021-03-30-PayPal-Launches-Checkout-with-Crypto)
- Vitalik [critiques the anti-PoS arguments](https://www.reddit.com/r/ethereum/comments/mf31ia/a_brain_dump_on_pos_vs_pow_arguments/) from Bitcoiners
- Auction of 23 TLDs (eg .lol and .link) [includes the ENS version and NFT](https://medium.com/the-ethereum-name-service/nfts-of-ens-tlds-to-be-auctioned-alongside-dns-versions-by-unr-9a23af828f9c)
- _The Onion_: priceless [NFT vandalized](https://www.theonion.com/priceless-nft-artwork-vandalized-with-spray-paint-tool-1846574103) with MSPaint
- [Wormhole](https://twitter.com/feross/status/1377528461464645633): send files end-to-end encrypted, based on Webtorrent

* * *

## **Job Listings**

- Mark Cuban is [hiring a Solidity developer](https://forms.office.com/pages/responsepage.aspx?id=eXzVWmTuiUmTrcjxzHRKl4CqH2xfzK5LnnIqG9Y7LxlURVc5ODdUUVhIVUxPUEQyNzA0NU9ESlRPNC4u). Send a code sample to apply. 
- Showtime, the NFT social network, is [hiring for more roles](https://angel.co/company/showtime-technologies/jobs/1282540-founding-mobile-engineer)
- Status are hiring! [Protocol Engineer](https://status.im/our_team/jobs.html?gh_jid=2162520), [Mobile UI Engineer](https://status.im/our_team/jobs.html?gh_jid=3022408), [Security Engineer](https://status.im/our_team/jobs.html?gh_jid=2973159)
- 3Box Labs is hiring! [Backend, FS + Protocol Devs](https://jobs.lever.co/3box) for [Ceramic Network](http://ceramic.network/)

**Want your job listing here**? $345 per line (~75 character limit including spaces), payable in ETH (or 345 DAI or 345 USDC) to evan.ethereum.eth. Questions? thecryptonewspodcast at-gmail

* * *

If you’re wondering “[why didn’t my post make it into Week in Ethereum News](https://www.evanvanness.com/post/179914035841/why-didnt-my-post-make-the-newsletter),” then please put it on an Ethereum subreddit; emails/DMs are not part of my workflow.

Please click the following if you’re interested in sponsoring the [newsletter](https://www.evanvanness.com/post/625741875743227904/evan-is-live-on-balancer).

Twitter: follow [@WeekinEthNews](https://twitter.com/WeekInEthNews) to find out what the most clicked are. Follow [@evan\_van\_ness](https://twitter.com/evan_van_ness) to get most of the week's news in real time.

Permalink for this week’s issue: [https://weekinethereumnews.com/week-in-ethereum-news-april-4-2021/](https://weekinethereumnews.com/week-in-ethereum-news-april-4-2021/)

* * *

## **Dates of Note**

Upcoming dates of note _(_new/changes in **bold**_)_**:**

- **April 8 - OpenZeppelin’s [Solidity access control workshop](https://twitter.com/OpenZeppelin/status/1377349984937418754)**
- April 9 - May 14 - ETHGlobal’s [Scaling Ethereum](https://scaling.ethglobal.co/) hackathon
- April 14 - [Berlin upgrade fork](https://github.com/ethereum/pm/issues/248#issuecomment-782069875) **(block 12244000)**
- April 16 - [Rollup community grant](https://esp.ethereum.foundation/en/rollup-grants/) applications due
- April 20 - deadline for [beacon chain security and testing RFP](https://notes.ethereum.org/@lsankar/security-rfp)
- April 20 - deadline to [comment on FATF anti-DeFi](http://www.fatf-gafi.org/publications/fatfrecommendations/documents/public-consultation-guidance-vasp.html) regulatory proposal
- April 22 - [Ethereum in the Enterprise 2021](https://www.conference2021.entethalliance.org/)
- May 14 - papers due for [WoSCA 2021](https://trailofbits.github.io/WoSCA/)
- **May 14 - Jun 2 - [0xHack](https://0xhack.dev/)**
- Jul 20-22 - [EthCC4](https://ethcc.io/) (Paris)

**Did you get forwarded this newsletter?** _[Sign up](https://weekinethereum.substack.com/subscribe#about) **to receive it weekly**_

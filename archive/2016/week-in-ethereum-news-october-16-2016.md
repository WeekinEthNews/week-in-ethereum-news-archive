---
title: "Week in Ethereum News <BR> October 16, 2016"
date: "2016-10-16"
---

## News and Links

**Top**

- Yogi Berra’s aphorism “when you come to a fork in the road, take it” has never been more apropos.  As predicted last week, we came to the fork in the road.
- So we’re going to take it. Twice.
    - Just like we have a few times before.  
        

**Fork for Freedom (from spam)**

- This week’s spam attacks were about cheaply creating many new accounts and bloating the blockchain.
    - Consequences: at one point, thousands of pending transactions and thus blockchain bloat.  
        
- Fork 1: At [block 2463000](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.ethereum.org%2F2016%2F10%2F13%2Fannouncement-imminent-hard-fork-eip150-gas-cost-changes%2F&t=M2I3ZmIyN2NkNzc3NjU3NDUxN2RlMTZhNTllNGFmMzY3YTcxYTY3OCxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0) to reprice opcodes in the Ethereum virtual machine. That block should happen early afternoon Tuesday in Europe.
    - Update your clients beforehand: [Geth](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2Fgo-ethereum%2Freleases%2Ftag%2Fv1.4.18&t=ODkyYzE3ZDJmYjQyOGMxNTEzZjdkNWQ3ZDc1ODZkOTYzZDE4OGM3YyxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0). [Parity](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethcore%2Fparity%2Freleases%2Ftag%2Fv1.3.8&t=NzI3OWM2YTBjOGVjODI1ZjEzMTc2NjA2NTVlYWQwZDVjZDEwODI3YixOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0).  
        
- Fork 2: Un-bloat the state.
- Vitalik on how the [re-pricing will affect existing contracts](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F57p0bv%2Fa_quick_note_on_how_the_call_gas_cost_increase%2F&t=NTE5ZTkzYjU3ODFhN2M5ZTVmMGQ1NzQ3NTliM2M5MjRkZDQ2MWJmZCxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0) – likely only extreme edge cases.  Or in Vitalik’s words, “the size of that set is possibly nonzero.”
- More Vitalik: [On Gas Price Markets](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F572n4q%2Fon_gas_price_markets%2F&t=ZjRkNTJjZTgzMDM0MzFkY2E5ZDI0NDI3NTNkYzg5ZTIwZjIxZjk0NCxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0). Short version: static re-pricing in the near-term; more flexibility long-term.

**Tech**

- Yoichi Hirai’s [smart contract verification](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fpirapira%2Fethereum-formal-verification-overview%2Fblob%2Fmaster%2FREADME.md&t=ZjJhMTc1Mzk0Zjg4MmNjNzE1ZDc1ZGU1NDYzMjA4M2UwNjlmMWNiYixOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0) overview
- [Upgrading to Solidity 0.4.0](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2Fsolidity%2Fblob%2Fdevelop%2FChangelog.md&t=OWJmYjE2MWUyYTA0ODMwMDkwYjhmNWJhMjg5YzFlMGM3YzRhMmY0NSxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0)
- [Wallet/Mist 0.8.5](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2Fmist%2Freleases%2Ftag%2Fv0.8.5&t=OWY0ZmEyM2I1ZTY3NjJlN2Y2MDVmYTY0MTVjNDAyOWQ0OTgyNTA3OCxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0) release.
- Nick Johnson [updated his EVM disassembler](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Farachnid%2Fevmdis%2F&t=ZjU1ZmUxOTEzMWNlZmFiNTI1ZDQ1NDE5NGIxMGI1OGZlMTI5ODU0NCxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0).
- [Truffle v 2.1](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F574rvr%2Ftruffle_v210_now_with_solc_04x_support%2F&t=Yzc1M2VhMTQ5OGZhNzVhYTM3YWJlZTgxNWVmOTYxMTJlZmFkYmI2NixOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0) is out.
- [Could zk-snarks scramble the Proof-of-Individuality (POI) tokens?](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F57j3zp%2Fcould_zksnarks_scramble_the_proofofindividuality%2F&t=OTNlNjMwMTJhNzA0ZTJmOGFiY2Y1YjgyNTA1ZDNkZjg3YzU3MmIxNCxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0)
- Péter Szilágyi’s “[Immutability in Go](https://t.umblr.com/redirect?z=https%3A%2F%2Fethereum.karalabe.com%2Ftalks%2F2016-dotgo.html&t=MGJiOGViMjk5YjI0NmQ4NjNhZTdkYjM3MzdjNWZjNDk0ZGQ4Nzc4YyxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0)” slides from presenting at a Go conference.

**Ecosystem**

- [DevCon2 talks are finally being released](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.youtube.com%2Fchannel%2FUCNOfzGXD_C9YMYmnefmPH0g&t=ZjE2MGNiMDZiN2I4MzZmY2Y3ZDY2YWE2N2QxZjgxZjdhNjU4MTIzZSxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0)!  Currently there are 5 videos of Day 1 talks, and the slides are now on the [Decvon2 page](https://t.umblr.com/redirect?z=https%3A%2F%2Fethereumfoundation.org%2Fdevcon&t=YWRhZDJkZjdjYmMzZTdhZTQ5YzliYTk4YzM3NWZhN2M0ZDhjMTFiNyxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0).
    - Or you can check out [raw footage](https://t.umblr.com/redirect?z=http%3A%2F%2Flist.youku.com%2Falbumlist%2Fshow%3Fid%3D28368456%26ascending%3D1%26page%3D1&t=NzNjNDAxZTJhZWZjYjIxMmFkNDZjN2VhMTBjOTA1YjY1ZGIwNjE2NSxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0).  
        
- [Weiwardit](https://t.umblr.com/redirect?z=http%3A%2F%2Fwww.weiwardit.com%2F&t=YzgzY2IzMDE4NjgwYTk1MWI5ZTYwYjU4YTA2OTc5YTRhZWNhMzBkOSxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0) live on testnet – A combination of Quora and Reddit on Ethereum.  Lots of [Q&A on Reddit thread](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F56rkrs%2Fi_built_a_new_dapp_ethereum_quora_reddit_steemit%2F&t=MjdkYjdhZjY2Y2M5MWMyYzllYWU5OWU4Mzk4YmUwOTAzMWQ4MmU2ZixOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0).
- Chronicled’s video of a [drone delivery access system](https://t.umblr.com/redirect?z=http%3A%2F%2Fchronicled.org%2Fdrone-case-study.html&t=ZWM2MTAxZTM1ODU5ODRkNzljMjBkZjk4N2U3ZDYzZGQ1ZGM5M2I4MCxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0) via blockchain is beyond cool.  It feels like seeing the future – as long as politicians don’t mess strangle it with regulations.
- [MakerDAO’s Annual Update](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.makerdao.com%2F2016%2F10%2F11%2Fmaker-annual-update%2F&t=ZDk2ZjVmODExMzg3ODQ2MzYxZTI5YTM2ZDI3NzFlODNjZGJlMzE2ZixOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0).
- [Colony Q4 update](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.colony.io%2Fcolony-q4-update-77f7661a9e00&t=ODYxMjM5MTY0NTY0MmFkMmU3ZTc2ZDg5ZWMwZDA5Y2VmY2UzYzZlOSxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0).
- Piper Merriam on the [Ethereum Ethos](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F57hqyg%2Fthoughts_on_our_values_as_a_community%2F&t=MTA5ZWIzY2ZkNWNiMDhmNzkzYmQzYWY5MjY5NmVjY2EzMzRlZDQ1YSxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0)
- Taylor from MyEtherWallet’s rants are [sometimes just awesome](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F56wgd7%2Fsecurity_of_jaxx%2Fd8myta8%3Fcontext%3D3&t=YTNkOGMwYTZmOWNmOTE0MTQ0ZDE1NDE1ZTY5MThmMTU3ODdhYTU2OCxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0).
- Dwarfpool explains why it is [mostly mining empty blocks](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F57c1yn%2Fwhy_dwarfpool_mines_mostly_empty_blocks_and_only%2F&t=MDZkMGIxYWE0MTdkOTRmYTllYThiMWUxYjJjNjEwMTI4ZDViYTE5YSxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0).
- RexMLS [raises a seed round](https://t.umblr.com/redirect?z=http%3A%2F%2Fwww.rexmls.com%2Fblog%2Funcategorized%2Fsuccessful-seed-objectives%2F&t=ZTM4ODg0MzAwZGY5MTliZmUxODdhMjkwZDE1ZjhhMDllNTliN2FiZixOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0).
- Navelgazing: Jeremiah Nichol’s post of the newsletter to [EthTrader](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethtrader%2Fcomments%2F56p3h8%2Fthis_guy_has_a_very_clean_newsletter_and_a_great%2F&t=YTZjOWJmNjI2YzFkNTEzNzdhM2UzMzVhZDJlOGE2NjM5ZjE1ZGE1ZixOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0) got more new subscribers than most of my own posts.  Thanks Jeremiah!

**Token Sales**  

- [Golem releases a draft whitepaper](https://t.umblr.com/redirect?z=http%3A%2F%2Fgolemproject.net%2Fdoc%2FDraftGolemProjectWhitepaper.pdf&t=Y2RiY2ZkYjE0YmFlNWNlNWZjOGQ0NmQ0Y2YwMWMzMDQ4NDU4N2Q4NyxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0).  Definitely will be commenting on this in the future.
- Decent bit of ether.camp kerfuffle this week.
    - Lots of sockpuppet accounts.  So many there needed to be a post about [banning them](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F57fcef%2Fbanned_sockpuppet_accounts_promoting_projects_are%2F&t=ZmZmNmNkNDBjY2Q4MGMyYWI1MjRmZDI2NjFkMDc5YTdiNzhhY2NkNixOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0).  
        
    - $50m crowdsale cap  
        
    - In general, the announcement of their crowdsale didn’t feel well thought out or explained. Technologists often seem to forget (or simply disregard) business in favor of technology. That doesn’t incline me to want to put value at risk in their business.  
        
- Gnosis [promises](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F56urcg%2Fethereum_community_needs_a_more_rigorous_tools_to%2Fd8nmsyj%3Fcontext%3D3&t=NTU1MDg4MWVhOGY4N2Q2YjJlZWE5NDNhODNjNDY4MTJlNTRhY2ZjOSxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0) to release its code at least a month before their crowdsale begins.

**Media**

- Augur’s Joey Krug on the state of crypto journalism: “[What happens when a VC + institutional trading firm acquires a news publication](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F%40joeykrug%2Fjournalism-bcd76ab28484&t=MzEzZWY2YjliMDFhNGI2Nzg0ZDJjNjFkNmIwN2ZkZDZjOGU5NzIyMCxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0)?”
- Dun & Bradstreet [announces](https://t.umblr.com/redirect?z=http%3A%2F%2Fblogs.wsj.com%2Fcio%2F2016%2F10%2F14%2Fdun-bradstreet-tests-blockchain-for-trade-finance%2F&t=ZGRhMTA4YWYyNjI0MmVmNTVkNTFiNzAzMjE1OGQ3MDU0YjMzMTUwZixOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0) Ethereum based project in the Wall Street Journal.
- [Central banks consider blockchains](https://t.umblr.com/redirect?z=http%3A%2F%2Fwww.nytimes.com%2F2016%2F10%2F12%2Fbusiness%2Fdealbook%2Fcentral-banks-consider-bitcoins-technology-if-not-bitcoin.html%3F_r%3D0&t=ZTZlZjRiODBiOTNhM2Q5ODQzODI5ODBlMGVmY2Y4NzQzYTAxOGU5YSxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0), from the NYTimes.

## Dates of note      

- Oct 20 – ether.camp [ICO begins](https://t.umblr.com/redirect?z=https%3A%2F%2Fforum.ether.camp%2Fc%2FHackerGold&t=NzBkMWQ4NThlMmViZjgzYjU0YjdiOGI5NTFhMzcxZTYxNWEyMWVjZCxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0)
- Oct 26 – [Inchain](https://t.umblr.com/redirect?z=http%3A%2F%2Fico.inchain.io&t=MGExMDIwYzM0ZmY1OTNkYzZlNDljYTZiYzZiZTk0OWRmNDZiYTFlOSxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0) crowdsale begins.
- Nov 1 – [Beyond the Void](https://t.umblr.com/redirect?z=http%3A%2F%2Fbeyond-the-void.net%2F&t=MmIwZmU5ZDI0N2RjYzUwOTA5ZDAwMDQ4Zjg2NjE3MGJiNWUxNjlhOCxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0) game crowdsale begins
- Nov 14 – SEC has a fintech/blockchain meeting
- Nov 15 – [vDice](https://t.umblr.com/redirect?z=http%3A%2F%2Fcrowdsale.vdice.io%2F&t=ZWUwZTRjZTZlY2JhZTg5NTQzZDA2Y2NlMGVmNzMxMTM5OWYwMDk5MixOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0) crowdsale begins
- November TBA – .ETH name system goes live
- Dec 7 – Inchain crowdsale ends
- Dec 15 – vDice crowdsale ends

## Token Sale Standards  

Plenty of activity this week:

1. [Raising money only on the basis of intent](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F57ctky%2Fico_raising_money_on_the_only_basis_of_the_intent%2F&t=MGEzZDJjM2ZkYzZjNDJjMDIwOTI0YTIwOTQ4ZDdjNDJjZTRkZjIxYyxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0)
2. Dennis Peterson proposes [pro-rata portions of an ICO that goes over its cap](https://t.umblr.com/redirect?z=http%3A%2F%2Fwww.blunderingcode.com%2Ffairtokensales%2F&t=YTE2NDM2NTk5YWZmNzQ5MWU0MGIxZjQzYmNiNjI5ODQzZjRiNzg0NyxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0), possibly by using security deposits.
3. Reddit thread: [We should create minimum viable ICO standards](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F57j8uk%2Fwe_should_create_a_set_of_guidance_that_defines_a%2F&t=MDYwNGM2OTE1NWE5NGFhNTRjNjVlY2M0MDg0OWM4NmU1YzI5NTgyYSxOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0)
4. Nick Tomaino: [Discussing cryptotoken best practices](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F%40ntmoney%2Fdiscussing-cryptotoken-best-practices-5ff4b9184933&t=YzFiNDViOTFiNWI0NzVhYWQxMWMwMmEwODNhN2I2ZGZlODA4ZjEyYixOSnB1em1ESA%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155176171838%2Foctober-16-2016&m=0)

_**To cap or not to cap?**_

_Where I’m at right now_: I feel like the best two crowdsales have been Ethereum and Augur.  Both of which were uncapped, with relatively low early bonuses. Later funders could calculate what percent they would get, knowing that further dilution could occur and that the early funders got a better deal than they did.

I’m also tempted towards the idea that founders should get more % of a project as more money is raised.  That way the marginal incentive to fund another dollar/ether decreases as more money is raised.

There are downsides to this model, however.  To name just a few: funders have no influence once a crowdsale has finished, raising money as a one-shot deal encourages over-estimation, no vesting schedule for founders, no lockup period, etc etc.

As a community, we should try to find a way to fix those downsides.

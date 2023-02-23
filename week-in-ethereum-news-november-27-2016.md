---
title: "Week in Ethereum News <BR> November 27, 2016"
date: "2016-11-27"
---

##  News and Links  

**Top**

- The Spurious Dragon hard fork went off without a hitch at first.  But then it didn’t at block 2686351, when the two main clients disagreed with each other on a rather trivial issue. Consensus lost, unintentional fork.
    - Why? The spam clearing account (eg [old](https://t.umblr.com/redirect?z=https%3A%2F%2Fetherscan.io%2Faddress%2F0xe9c9068240d8450da314f60804debfc194b72309&t=MzE4OGEyMDkzZDg2Y2QxM2VjYmU1Zjc1MzIxZmE3MjUxZGYzZjgxZSx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) or [current](https://t.umblr.com/redirect?z=https%3A%2F%2Fetherscan.io%2Faddress%2F0x388383dae4f910faa943df42ee2a80642916481e&t=NmY3ODdmN2Y5OTUzZGRhMjM2NzFjMzJmY2ZjNGNkMTY2YzcwNjcxNyx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)) ran out of Ether, so the Geth client deleted the spam but the Parity client did not.  Either would be correct, but both clients must do the same thing.  
        
    - There was some snarking between the dev teams on Twitter but the [Yellow Paper](https://t.umblr.com/redirect?z=http%3A%2F%2Fpaper.gavwood.com%2F&t=ZjE1NTk5MGZjMWYxY2NiMGM1YTQ1YTE0MWMxODgzYjIzYTNjMTJjNSx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) spec was ambiguous.  \[The Yellow Paper is quite dense and a [reference version](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F5eqggd%2Ffolks_gav_gave_you_a_spec_use_it%2Fdaeno6b%2F%3Fcontext%3D3&t=NmFiMzRlOTFjYjllZDA3NjkyMjM3MTgyY2VmNTg4MGU1NzdkMjYxZSx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) might be useful\]   
        
    - In the end, Geth [updated](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.ethereum.org%2F2016%2F11%2F25%2Fsecurity-alert-11242016-consensus-bug-geth-v1-4-19-v1-5-2%2F&t=NDk0N2M0ZjI2Y2U5NWMzYWY0ZmFhMTcwZDVhODdkNDg0YTUxMDllNix3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) with a fix in a mere ~10 hours.  Transactions weren’t lost – the losers are the Geth miners on the abandoned chain.    
        
    -  Lessons will be [learned](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F5eohlm%2Fgeth_dev_team_needs_to_improve_their_testing%2Fdaeecap%2F&t=OWRmZTIxMmQxYWQ2NjZhNTJiMmIwMzFhODMzNjc5NmE1MzJkYjljYSx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) and processes will be improved  
        
- Vitalik’s FAQ on [cleaning the state of spam](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F5es5g4%2Fa_state_clearing_faq%2F&t=OTFiYjdhZTBmZDJjNjNmYTc0OTc2ZmFhMjBmZTAwNDYzYmJjZWEzMCx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0).  It will take another week (or [slightly longer](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F5egm7g%2Fpsa_the_state_clearing_process_is_in_motion%2Fdacwi3t%2F%3Fcontext%3D3&t=MjZjMGUwYzVkODNhOGEzNzJkZmFhYjg1MTNjOGE2MjQ2NTY1MWRhMCx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)) to finish.
- The develop version of Parity also set the default gas price to zero, so there was a brief [kerfuffle](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F5ewumz%2Fminers_accepting_zerofee_transactions_is_not_in%2F&t=Mzk3ODMwMDQyM2ExYTMwNWE0NGIxMWRmZGQxNDkzZDM0MzdlZGNhZCx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0), but miners realized and fixed it.
- Alex van de Sande on [progress made towards the Metropolis milestone release](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F5eftp6%2Fnow_that_the_hard_fork_is_complete_the_next_fork%2Fdacbtis%2F&t=ZWJhOTdhYjExMjQ4OTEzMDI3YWIxZGYwMDNiMTU1MzU3OWJlYWEyYyx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0).

**Tech**

- Raiden Network [PoC 1](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fraiden-network%2Fraiden%2Freleases%2Ftag%2FPoC-1&t=YWYwZWM1ODMwODRjYmEwYmI2ZmQ4OTkwNmEzMzhhMWJlMmVjOWQ3Nyx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) released
- [Solidity v0.4.6](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2Fsolidity%2Freleases%2Ftag%2Fv0.4.6&t=NTA2MmI3YzBiOGNkYmVhYWUyZGMyZDIxODBjYmQ1NTBlZDI2NjQwZCx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) released
    - Browser-Solidity [now features some static analysisa](https://t.umblr.com/redirect?z=https%3A%2F%2Fi.redd.it%2F3p78amcvb0zx.png&t=NWMwMjJiNGYwZWYxNGVmMjcxNzhlZjdiMjQ4M2MzNGQwODE3MTZkMSx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)  
        
- [Go Ethereum library](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2Fgo-ethereum%2Fwiki%2FMobile%3A-Introduction&t=MDRhN2UyOTYxMjI5Yjk3MWI5ZTYwYzRmOTQ1OGI0ZjY2ZTk4YWJjYix3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) at Maven Central (Android) and CocoaPods (iOS)
- [Parity 1.4.5](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethcore%2Fparity%2Freleases%2Ftag%2Fv1.4.5&t=Zjk2MzlkMTY1NWI3NWUxMjllZjA0NGM0ODY5ZTVmMTVmMDA0ZjFkNCx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) released – now with a non-zero default for the –usd-per-tx flag
- [Geth 1.5.3](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2Fgo-ethereum%2Freleases%2Ftag%2Fv1.5.3&t=OGQyZTJmODdkZWZlNDA2MTc0MTdjY2NhZTQwM2MzMDZjNWUyNzhhMyx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) released

**Ecosystem**

- Ethereum Name Service [launches on Ropsten testnet](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2Fens%2Fwiki&t=NjhjMjUyMWI2Zjc3YmIzNDVhM2NhYWM1ZDM0Yjc0ZjUxYjc0MGVkZix3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) – (test) register your domain name today
- A large [MyEtherWallet.com Update](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F5e3alw%2Fmassive_myetherwalletcom_update_better_uris_the%2F&t=ZTMwY2RjYmU3YTdiOTMzMDk5MWJjZjNlNmQ0ZDU5NTBlZGExZmFkOCx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)
- More [DevCon2 videos released](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.youtube.com%2Fchannel%2FUCNOfzGXD_C9YMYmnefmPH0g%2Fvideos&t=YzMyZjg3NjdlZGFiODM4NmYwNzY5OTY3MmIxNGM0ZDIwNWVkMDZjMix3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) this week- web3, Swarm, EVM, Raiden, etc
- 8 videos from [DappHack Berlin](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DjluJ0NSTYZQ%26list%3DPL3bvPCw5QCLJ_a2cfoXXmjIrAg4cb1VEv&t=NmM1ODE1M2RlMTk1OTYzN2JlNjM4NjdhMmVmYjNlOGE3YmM1YjNkOSx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)
- Blockchain [Energy Trading interview](https://t.umblr.com/redirect?z=http%3A%2F%2Fmicrogridknowledge.com%2Fblockchain-energy-trading%2F&t=NTA2MjM2MmQ3MjI2MTM0MGU3Mjg1OTYyOWNhNWFmM2NlMmJlMDRiYyx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)
    - [Consensys and Siemens](https://t.umblr.com/redirect?z=http%3A%2F%2Fwww.siemens.com%2Fpress%2Fpool%2Fde%2Fpressemitteilungen%2F2016%2Fenergymanagement%2FPR2016110080EMEN.pdf&t=N2U3NzNmOWIxMmIyZDFlYmQ0OTA0ZDBjYzFjMmUxOWU0MzFjYTk0NCx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) will “jointly develop microgrids that enable local energy trading based on blockchain technology”  
        

**Token Sales**

- [How to Evaluate Token Sales](https://t.umblr.com/redirect?z=http%3A%2F%2Fstartupmanagement.org%2F2016%2F11%2F24%2Fhow-to-evaluate-an-initial-cryptocurrency-offering-ico%2F&t=ZjM0YmM2OTVjOWI2NTVkOWZkMDFkZTRkMzJlODhjNGViMGJhM2IwMyx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) by William Mougayar
    - For new subscribers: if you want to [get a doc with my token sale thoughts](https://t.umblr.com/redirect?z=http%3A%2F%2Fwww.evanvanness.com%2Fpost%2F150900601406%2Fwhats-happening-in-ethereum&t=NjA5Nzg5MGVjYWE3NTE2NmNlMGU3ZjY5NDJiYzJlOTQ1YzQzNjMyMyx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)  
        
- [Interview with Logan Schinbeckler](https://t.umblr.com/redirect?z=http%3A%2F%2Fblog.coinschedule.com%2Fico-spotlight-interview-with-logan-schinbeckler-from-branche%2F&t=ZTgwZmIxYjEwNzA5ZDNhY2ZiNmJiNGE2NWUxYmYwNGE4OGVkODA3OSx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) from Branche
- Dmitry Buterin - Vitalik’s father - joins [Arcade City as an advisor](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Farcade-city-press%2Fdmitry-buterin-joins-arcade-city-advisory-board-18da3833e62c&t=MmM1NjQ3OGM4NzVkNDA3NmJiNGU4ZTQ1NzYxY2ExMTVlYTg3ZGJjZCx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)
- Sam Cassatt at Consensys: [What VCs got wrong about Bitcoin](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fconsensys-media%2Fwhat-venture-capitalists-got-wrong-about-bitcoin-a0572aec18d0&t=YjZhZmYyOGRhNWQ2NDYzMTAwYjNlNTA5YjkwNDE4MjE3YTc1YTlhMCx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)
- Charlie Shrem is [starting a private equity fund](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F5f03o4%2Fcharlie_shrem_unveils_new_venture_intellisys%2F&t=OGQwNWRmNDJlNzZkNTVkMjhkYmJiMzM4ZDQzYmMyMjhjZWNlZDM5NCx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) and making ownership an Ethereum token.  Token sale to follow.

**General**

- Melon founders did a video interview on [Melon/Polkadot](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DrfRufqN8S9c&t=ZDExOGRjNjZmMDM1NmExZDUwYjVkYTY4OWJjYTQ1ZTI3MWU0YzdiMyx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)
- A bunch of [banks left R3](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethtrader%2Fcomments%2F5exq7h%2Fjp_morgan_macquarie_group_and_us_bancorp_join_the%2F&t=YzA5OTU4YWVlNmMxZTQ0ZmQ0NDNkMGUxNTgxOGNhODI0ZDA5MDVmYix3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)
- [JPMorgan’s Quorum is on Github](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fjpmorganchase%2Fquorum&t=ODIwZGJhYWJhOTkyYWI4MGI0NDhmOTUyZjZlZGNkYWY4MDNkYzU1YSx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) - their implementation of Ethereum worked on by Jeff Wilcke (and [others](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fjpmorganchase%2Fquorum%2Fgraphs%2Fcontributors&t=YTVjMTU1MTJlOTQwODk1YjcyNmE5ZDE1N2NjNWQwMmI2Yjc4MzdlOSx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0))
- Aaron Watson [interviews Joe Lubin](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3Dzw16x5-G4NI&t=ZjBkZjUwY2RjYjUzYWNiMDFlMzIwNDQ3ZDlhNmExZDVkZmUyYjU1Nix3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)
- [SWIFT unveils PoC](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.finextra.com%2Fnewsarticle%2F29813%2Fsofe-berlin-swift-unveils-blockchain-proof-of-concept&t=ZDY1N2M4NTViMDg2OGVjY2U3ODU5YzBlYWJmZjNmZGY5M2FiZjFhOCx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) – Eris Tendermint with Solidy contracts
- Two good reads on passwords – I’m not doing them justice with this description:
    - Taylor Van Orden on [what’s in your keystore](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F5ees2q%2Fis_the_bkp_component_of_a_presale_json_file_a%2Fdacx0pi%2F%3Fcontext%3D3&t=ZDIxZDRkN2YxZDVkMzMxNGY4MmE2NTlhYjczYTVjMzZmYjFlY2UxNyx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)  
        
    - Thomas Clowes with a [practical read on how he robbed himself](https://t.umblr.com/redirect?z=http%3A%2F%2Fdoublenegative.com%2Fethereum-security-and-wallets%2F&t=MjgyYjE1NmU1ZmMwNDcxZjViNTExMGU2NjI5NDI2MTRkMTQ1ZTMzZix3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) - lots of links for future reference.  
        
- Kraken on how [2FA with SMS messaging](http://kraken%20security%20advisory:%20Mobile%20Phones/) is useless if someone wants to hack you.
- Could Bitcoin do smart contracts?  [Not really](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F5e1wx7%2Fcan_bitcoin_really_implement_smart_contracts%2Fda96jse%2F&t=OGVjYWZkODE1ZDc1MjIxZDdiYjZkMzU1NjFkZjhjM2I2ZmNiY2YwNix3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0).
- Vitalik offered some [technical advice to Ethereum Classic](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2FEthereumClassic%2Fcomments%2F5e5moq%2Fetc_monetary_policy_proposal_by_snaproll_is_now%2F&t=ZTZhNTlmZmI5NjYzNTEzY2Y4MjZkMWFlZDEyMTY4YmU3ZmIzZmNhZCx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) and Charles Hoskinson got irritable.  (Thread bonus: a [Taylor Van Orden response](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2FEthereumClassic%2Fcomments%2F5e5moq%2Fetc_monetary_policy_proposal_by_snaproll_is_now%2Fdaca6w5%2F&t=MDMxN2YwMTJmODhkMzUzNDRjMWVhMTc4NDY5NDQxN2NkNjUzY2E0YSx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) \[and [context](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2FEthereumClassic%2Fcomments%2F5epag2%2Fclassicetherwallet_does_not_work%2Fdaeeyst%2F&t=YTkyN2RjOWViMjMzNjMwN2U1ZTk0NzUyOTVkZGI5NDQ5OTA3ZGVjZix3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)\] - her Reddit comments make me laugh the hardest)

## Dates of Note

-  Nov 25 - 27 – [Canadian regulator hackathon](https://t.umblr.com/redirect?z=http%3A%2F%2Fwww.osc.gov.on.ca%2Fen%2Freghackto.htm&t=ZTBhZjk1YjllOGRkNDZlN2FmYjFmMzFlZDNkOTJkYjcwNTkwZGRjMyx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0)  
    
- Nov 28 – [BlockCDN](https://t.umblr.com/redirect?z=http%3A%2F%2Fwww.blockcdn.org&t=YmQyZjQ0YmIxNTkyNmVkMjBkZjVmM2M5OTU5MDc2YzRmOWU1OGY0NSx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) crowdsale begins
- Nov 29 – [Arcade.City](https://t.umblr.com/redirect?z=https%3A%2F%2Farcade.city%2F&t=ZTc0MDdiYmFlNTUzOTQ3ZjczMmE4MTYwZjAyYWI0YTc2ZjMxMTI5MSx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) crowdsale ends
- Dec 4 – Next ether.camp price change
- Dec 15 – [vDice](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.vdice.io%2F&t=MTY1NmI0NjQxMmQyZDUzOTA0NDllYWM0YjkzYWJkMDEyYWE1MGExNSx3b2FCdW45Rw%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155123874398%2Fnovember-27-2016&m=0) crowdsale ends

\[I aim for a relatively comprehensive list of Ethereum sales, but make no warranty as to even whether they are legit; as such, I thus likewise warrant nothing about whether any will produce a satisfactory return. This is not investment advice.\]    

## Misapplied Bitcoin Mindsets

This week saw plenty of misapplied Bitcoin mindsets in the Ethereum community.  

Every time we have a bump in the road (like we had this week), there are a minority of folks in the Ethereum community who freak out.  _What about network effects?  OMG price matters_!  Both sentiments got significant upvotes on Reddit this week.

Bitcoin’s network effects are monetary – whether people use Bitcoin as a store of value and/or payment method.   Price isn’t just important, it’s arguably the only thing.   That’s what matters in Bitcoin, but not in Ethereum.

Ethereum’s network effects are dapps – are developers building decentralized software on Ethereum?  

So the important question is always the same: are we closer to successful working dapps?                                                                                                        

## 1000 subscribers?

I set a goal of getting to 1000 subscribers by the end of the year.  Currently, we’re at 650.

If this issue was useful to you, would you share it on social media or email it to a friend?  I hate it when I don’t achieve goals.

Just in case you want to send me Ether:  0x96d4F0E75ae86e4c46cD8e9D4AE2F2309bD6Ec45

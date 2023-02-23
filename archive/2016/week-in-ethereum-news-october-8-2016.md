---
title: "Week in Ethereum News <BR> October 8, 2016"
date: "2016-10-08"
---

## Links and Quick Hits  

- The [Ethereum Foundation has about 17m USD left](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F56ev84%2Fquestions_about_the_ethereum_foundation%2Fd8ixscy%3Fcontext%3D3&t=YzJjZTVjYThhZTY2YWM5ODM3ZWMzODJmODIyYzFlNTg0NmEzMjM4NCxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0) at current ETH prices.
- We are likely heading for a hard fork to fix the DoS attacks.  Ahem:

**DoS Spam attack**

- Two geth releases this week; one Parity release.  [Current Geth](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2Fgo-ethereum%2Freleases%2Ftag%2Fv1.4.16&t=ODY3YmQyNmE5OTA1NGVhMTAyMTE4NzY0M2QyNzBlZDhkYTYwMWM0OSxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0): 1.4.16.  [Current Parity](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethcore%2Fparity%2Freleases%2Ftag%2Fv1.3.5&t=ZWZmNzVjNTQ5OGY3NmE3NjNlN2U3YjRlYmUxMmZhYTY0OWU0NTJhYyxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0): 1.3.5.
- There were quite a few different attacks this week.  Whereas previous attacks [mostly targeted the Geth client](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F55s085%2Fgeth_nodes_under_attack_again_we_are_actively%2F&t=YTBjZTA4NDNkZGE5ZGY4MTAyMzU2YzBjZTY5N2Q0MDNlYzVhMzIxZSxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0), late in the week the attacker targeted a weakness in the way [Parity relays transactions](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F56f92s%2Ftodays_blockchain_issues_and_parity_fix%2F&t=NGZhY2ZkNmMxOTIwNTMzZDY2YzQ0ZTVmNzhjYjAxNjI5MWM1NTY2NyxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0).
    - As of 5 days ago, hacker had [spent about 350 ether on the DoS](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F55m90t%2Fmore_serious_attack_involving_sload_instruction%2Fd8c7dq3%3Fcontext%3D3&t=ZGRlNGY5ZDFlNWZmNjY3OWU0Y2RiM2FiZDQ2OWM0ZTAxNjQ3YWQ3NCxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0), per Martin Swende.  
        
- Gavin Wood [called for a hard fork](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.ethcore.io%2Fonwards%2F&t=MDRhYjM5ODM2YWNjMzJmNTcyZTk4ZDk1YWQ0OTFkZTQ4NWVlMjQ0YixTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0) to fix the computational mispricing of opcodes.  He believes we can achieve a 10x performance gain on the virtual machine.
    - Jeff Wilcke [announced](https://twitter.com/jeffehh/status/784318008592183298) that he has begun coding the hard fork in the Geth client.  
        
- **What goes in the hard fork**?  Check out [EIP 150](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2FEIPs%2Fissues%2F150&t=MzhkNWRkZTNhZWNkYTk1ODYwMDQ5ZjdjYTRlMDY0OTJhOTk0MTY5YSxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0), as well as [Vitalik’s Reddit thread](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F56f6we%2Fexplaining_eip_150%2F&t=MjI2ZTBiMDFmYWVkNWE0NDZkOTAzYTZhZDY2ODE2ZTkwMTFiZTM0MSxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0) on the subject for opcode repricing and other details.  \[In the future, potentially [flexibile gas cost](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F56f6we%2Fexplaining_eip_150%2Fd8ittar&t=YTljMGI2NGI2YWRiNzMwMGRlNWIxOTUyZjI5NTA3ZTFiNThhYzIwNSxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0).\]
- _The question is whether to hardfork and fix this now or wait until the Metropolis hard fork_.  I’d say the writing is on the wall: we’ll hardfork to fix the mispricings.

**Tech**

- A [visualization of Ethereum’s Yellow Paper](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F560h6s%2Fif_you_find_the_yellow_paper_hard_to_read_this%2F&t=YzFjYmE1ZTZiYmZjZjg0NDNlNjk3ZTg0Y2YxMmIyZWY1M2JlOTVmNyxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0).
- Colony released [SolCover](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.colony.io%2Fcode-coverage-for-solidity-eecfa88668c2%23.vin7ljgxv&t=ZGZhNzUyYzhiZGM0ZTU5Njc1Y2I1MTVjOWQ0YzBiN2MzYzQ2OThkYixTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0): a Solidity code coverage tool
- TestRPC 3.0.0 [released](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereumjs%2Ftestrpc%2Freleases%2Ftag%2Fv3.0.0&t=ZTFjODJiNzNiZjc2MzE5MTRlYzU4YTgzYTM0ZTBmZGIyZGY3NDdiYixTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0).

**Ecosystem**

- [Video of Vitalik’s talk](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DT4L3srqDUgE&t=NDMwN2NhNGUxOTMzNmYwZTM1NTM3ZDhkODQ0YzNhMjYzMzk4N2QyYyxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0) at the Hong Kong meetup. Audio isn’t great, but it’s particularly interesting to hear him talk about how Microsoft is the only big tech company interested in blockchains.
    - It’s important to seek opinions and evidence which counter your assumptions.  
        
    - _As such: of BigTech, why is only Microsoft getting into blockchains_? There’s some interesting discussion.  
        
- [Will Crypto disrupt Venture Capital?](https://t.umblr.com/redirect?z=http%3A%2F%2Fstartupmanagement.org%2F2016%2F10%2F06%2Fhow-cryptocurrencies-and-blockchain-based-startups-are-turning-the-traditional-venture-capital-model-on-its-head%2F&t=ZmNhMTIyNGRhOWQ4YmFkNzA5NjkzZjQ4ZDAwMDI3ZWJhZGEyZjRjNyxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0) by William Mougayar
- [Golem and Microservices](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.golemproject.net%2Fgolem-microservices-%25EF%25B8%258F-part-1-1f1ef7b9af29&t=NTgwOTZlMzA1YWMyYzU2NWI5Mzc0MmRiN2Y4MDg0Yjc0YjllOGI1ZCxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0)
- [Provenance updates](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.provenance.org%2Fnews%2Ftechnology%2Fprovenance-blockchain-update-devcon2%2F&t=MmRkZDA2ZDg3M2ExYzFmNjhmZTU4MTRiMTJiMjFiOTg1Y2Y0NjU4YixTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0) us on where they are.
- Gnosis is understandably getting [substantial community pushback](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F55qxr2%2Fgnosis_crowdsale_will_be_uncapped_thoughts%2F&t=YzAxMzY2MGI2ZWI0ZDE0OTExODIyYmFjOTk2NTM3YmZjNWI0N2U3NCxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0) on their plans for an uncapped ICO.
- [Cold storage](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F55k8w2%2Fcold_storage_for_dummies_does_a_simple_guide_exist%2F&t=YjVkOTJiMWVhYTI5ZjFlNjQ2NDVhMDVmN2FjNDU5Zjk0ZTI2ZDVlZixTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0) guide.
    - Martin Swende’s [practical tips for security](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F556frk%2Fits_time_to_get_real_stop_relying_on_third%2Fd881drv%3Fcontext%3D3&t=MDRlOWI4NTBkNDhmM2Y1Njg3YWYxMzczNDdlNTVkNWFhNTQ0OTk3NCxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0).  
        
- I haven’t thought about it much, but I kneejerk towards agreeing that [it’d be great if ICOs could adopt a Dutch auction](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2F54k11w%2Ffirst_blood_the_power_hour_gate_why_did_first%2Fd82k2f6%3Fcontext%3D3&t=Njk1M2ExZTEyNDc4NjI1MTIzNjViMGExNmI3NjhjMDBhYjhiNjgyOSxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0).

**Media**

- Why JPMorganChase is building its [blockchain project on Ethereum](https://t.umblr.com/redirect?z=http%3A%2F%2Ffortune.com%2F2016%2F10%2F04%2Fjp-morgan-chase-blockchain-ethereum-quorum%2F&t=MmMwNWE2MTc1YzA0YWE3YTljMTZjNDk2ZDBhOTJjNjcwYWUxYTU3OCxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0) (Fortune).  [WSJ version](https://t.umblr.com/redirect?z=http%3A%2F%2Fwww.wsj.com%2Farticles%2Fj-p-morgan-has-a-new-twist-on-blockchain-1475537138&t=MmQ5NTA4YTI3MTMzYmFlNDMzZjlhM2FkMjJhZTdkYmFkNjI5NTU0MCxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0).
- Gavin Wood does the [Changelog podcast](https://t.umblr.com/redirect?z=https%3A%2F%2Fchangelog.com%2F222%2F&t=NDVkMDQ1NzJiY2JjMWUyNDk3MDVmNWRiNTE1NmU0MzFlM2JmNGVmMixTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0).

## Dates of note  

- Oct 12 – [Inchain](https://t.umblr.com/redirect?z=http%3A%2F%2Fico.inchain.io&t=ZmNjNTJiZDU1MmZjOTI2ZGQ4MTg5MDcxYmQwYWFjN2I1OTZmYzAwZixTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0) crowdsale begins. \[First I’d heard of it\]
- Oct 20 – ether.camp [ICO begins](https://t.umblr.com/redirect?z=https%3A%2F%2Fforum.ether.camp%2Fc%2FHackerGold&t=YzhhNzJjNWQzNzM4Yjk4YzM5ZTY5N2U2MGUxY2I4ZmMwNmZmZTMwNyxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0)
- Nov 1 – [Beyond the Void](https://t.umblr.com/redirect?z=http%3A%2F%2Fbeyond-the-void.net%2F&t=MjQzNWY0MTcxZTE2OGM4ZWEwZWIwMTI5ZDNiMjJkMWE0Y2NlM2IxNixTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0) game crowdfunding begins
- Nov 14 – SEC has a fintech/blockchain meeting
- November TBA – .ETH name system goes live

## Iconomi’s Poorly Constructed Cryptocurrency Index  

Iconomi released their [cryptocurrency index:](https://t.umblr.com/redirect?z=https%3A%2F%2Ficnx.iconomi.net%2F&t=NjlhODhhZDM5MmVhNDUwMjY3ZWIwMmRiMmNhYTY1N2VkNGY2OWUyMixTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0)

_Why it’s bad_:

1. Bitcoin is 80% of crypto market cap, yet only 15% of the index.  Functionally, this means that this is a (poorly structured) Crypto 2.0 index, though it is called a general crypto index.
2. Dash, Steem and Monero are weighted about the same as Ethereum.
    1. Steem has daily volume magnitudes lower than other projects (thus, possibly masking the true price)  
        
    2. Dash and Monero combined have a market cap about 10% of Ethereum’s.  Yet each of them are almost as equally weighted as Ethereum and Bitcoin?   That beggars belief.  
        
3. Digix’s market cap is just $25m, yet its index weighting is almost half of Ethereum’s.  You can’t make this up.
4. _No Litecoin_.  The number 2 crypto project for years isn’t even in the crypto index?

I could go on.

Iconomi’s plan for an [index is one reason why I think they might succeed](https://t.umblr.com/redirect?z=http%3A%2F%2Fwww.evanvanness.com%2Fpost%2F150900730446%2Fwhats-happening-in-ethereum-issue-3&t=N2JkMTAwOThlNzRlYzI5NTRiYjJkZjNhZmE5ZDY5ZjU5YWU5ZmNkOSxTSklMQUdDNQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F155177376713%2Foctober-8-2016&m=0) , even though I didn’t care to put value at risk. However, their current index methodology is simply not good enough.  Getting it right is a big opportunity.  

## ICO Standards Working Group

Recent crowdsales have left many in the Ethereum community feeling that we need to do a better job setting standards for what we expect from founders.

If you’re interested in joining, email:  weekinethereum@gmail.com

## If you liked this, help it continue by sharing.

I’m tweeting more about Ethereum, so [follow me @evan\_van\_ness](https://twitter.com/evan_van_ness) and let me know how I can make this newsletter more useful to you.

If you’d like to send me ether, I’d like to accept it and will make that easy for you: 0x96d4F0E75ae86e4c46cD8e9D4AE2F2309bD6Ec45

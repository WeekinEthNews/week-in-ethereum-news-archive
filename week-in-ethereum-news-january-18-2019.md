---
title: "January 18, 2019"
date: "2019-01-18"
---

## Ethereum News and Links

**Constantinople postponed**

- The day before the scheduled Constantinople upgrade fork, ChainSecurity found that EIP1283 potentially allowed deployed contracts to be [vulnerable to a re-entrancy attack](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fchainsecurity%2Fconstantinople-enables-new-reentrancy-attack-ace4088297d9&t=YTQ5MDU4NTQyYmVhOTcwNmJiZjZiZmJhMjM0OWNiOGRmYTY1YmI5Yix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0). There was no bug in the EIP per se, but it broke an implied invariant for a small but then-indeterminate amount of deployed code. Hence, out of an abundance of caution but with limited time for the community to come to consensus, [Constantinople was successfully postponed](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fmycrypto%2Fethereum-constantinople-postponed-out-of-an-abundance-of-caution-a2d6db454fea&t=ZmUwOGUyYmNmNDY2MjI2ZDFjZTBhNmI5YzhjNTQ1NTJjMGUxZTM1Yyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0).  
    
- A full [post-action report](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Ftrailofbits%2Fpublications%2Fblob%2Fmaster%2Freviews%2FEIP-1283.pdf&t=YTkwYTYzYzI4MGJkYTJmMGIyMjcyNjlkNTgyMzlhY2RhODhiM2U0Nix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) by Trail of Bits, ChainSecurity, and Eveem. They proffer a different alternative to 1283 - refund difference of intended cost of writes. Magicians thread on [1283 alternatives](https://t.umblr.com/redirect?z=https%3A%2F%2Fethereum-magicians.org%2Ft%2Fremediations-for-eip-1283-reentrancy-bug%2F2434%2F10&t=OWFjOWYwNTBkNjEzZTAwNTkwMGVkOTdlN2ZjYzY5OTkwMWRmY2RlMyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) and thread on [invariants](https://t.umblr.com/redirect?z=https%3A%2F%2Fethereum-magicians.org%2Ft%2Fimmutables-invariants-and-upgradability%2F2440%2F42&t=YWNkZTE2M2QyMmE0Zjk0YzA0MTI0M2YyZjBlNzI1MTJkMjUxMjQxZSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0).  
    
- New ConstantiNOPE client releases by which the fork was avoided (update if you haven’t): [Geth](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2Fgo-ethereum%2Freleases%2Ftag%2Fv1.8.21&t=MGI5OGY1ZmJkNTFlM2IxYWFkMDJjYTAwNTQ2Mzc1YjZhYzc3MTE5Yyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0), [Parity](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fparitytech%2Fparity-ethereum%2Freleases%2Ftag%2Fv2.2.7&t=NDNmNjRhYWU2YjUxZTVmMDJkMTNjMTk5ZjNjNTYzMTljYjkyZDYxYix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) (stable) and [beta](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fparitytech%2Fparity-ethereum%2Freleases%2Ftag%2Fv2.3.0&t=ZGY4MDMwMzQxMzQ1ZjBhMjhhNjI0MmE1MmM3Njc5YWFjYzI2ZDBiZix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0), [Trinity](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2Ftrinity%2Freleases%2Ftag%2Ftrinity-v0.1.0-alpha.22&t=MjY0OTVlYTQzZWY2YmZkMWYyNDRlN2Y3OGJjZTZmMGY2ZmI4MjI1Yix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0), [Nethermind](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2Fageqih%2Fnethermind_v093_constantinople_delay_released%2F&t=NmRhNDQzMGZiZmZmNWM2ZmQ2YWI1NzgyMThiYWJlMTZiZWVhNjRlNix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0), [Pantheon](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2Fagel67%2Femergency_release_of_pantheon_085_to_postpone%2F&t=OTZmODljMDk0MTllNzM4MmViYzA4MDVlYmMzNTcxOGMwNGJjMTY4OCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0), [Ethereum on ARM](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2Fagewde%2Fethereum_on_arm_geth_and_parity_packages_update%2F&t=YTlmMGM0MWY2MWUzNDI5Njg1YWZiOTM0OTRhOTJhNGI2MzNjYThjMCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Constantinople is set for block [7280000](https://twitter.com/5chdn/status/1086285718710816768), around Feb 27. EIP1283 is not included.  
    

**Layer 1**

- \[eth1\] [Ethereum State Rent Proof of Concept](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.symphonious.net%2F2019%2F01%2F14%2Fethereum-state-rent-proof-of-concept%2F&t=YjcxYTY3YjJhZDIwNjE4NmFkNDQ0OWZlNmNmN2VkNmUyYTUxYTJiZix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- \[eth2\] Ben Edgington: [exploring Eth2.0 design goals](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedia.consensys.net%2Fexploring-the-ethereum-2-0-design-goals-fd2d901b4c01&t=MDJhYWIzMjAyNjFjOWE3MjVkOWZmZWE3NjdhNDcyODdiMzVjYmEwYyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- \[eth2\]  James Prestwich: [An engineer’s guide to eth2](https://t.umblr.com/redirect?z=https%3A%2F%2Fhackernoon.com%2Fwhat-to-expect-when-eths-expecting-80cb4951afcd&t=OWVhZjI5NGY2NTA4N2FhMzAzNjI1ZWFlZDFhOThmNTEyNGUwMTJkZSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0). See also [Vitalik’s annotations](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2Fagcrcb%2Fwhat_to_expect_when_eths_expecting_hacker_noon%2Fee64r3n%2F&t=NDY0NjY5NTY4ZDA5N2E5YmJlNDYzNmVjMmVlZDBmYjUxZGZhYWU2Nyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0).  
    
- \[eth2\] Latest [Eth2.0 implementers call](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DKZ9fms_PrQU&t=YzY5Y2FiNzAzNWYyMjNmNmRjMmVlYTI0MTY2OTAyODc2MGZhOGVjNyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0). [agenda](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2Feth2.0-pm%2Fissues%2F23&t=MWJhMzVkMjdiNDY2MGY3YzljMjA3NjMyYTFhMGQ3ZTVhNDFlYWVkZix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) to follow along  
    
- \[eth2\] [What’s New in Eth2](https://t.umblr.com/redirect?z=https%3A%2F%2Fnotes.ethereum.org%2Fc%2FSk8Zs--CQ%2Fhttps%253A%252F%252Fbenjaminion.xyz%252Fnewineth2%252F20190118.html&t=NjBjY2U4ZjkwNmEwNWM1MmY5NDhlMjQ3YThkZDk1ZjZiMzNlYzk4Mix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- \[eth2\] [Prysmatic](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fprysmatic-labs%2Fethereum-2-0-development-update-20-prysmatic-labs-e42724a2ba44&t=OTBhNjAzMTBkNjFiM2EyZmY1ZDA3YjkzZTM5MTU0NjYyNTNjMDVhOSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) dev update  
    
- \[eth2\] [Lighthouse dev update](https://t.umblr.com/redirect?z=https%3A%2F%2Flighthouse.sigmaprime.io%2Fupdate-06.html&t=ZWEyZWQyMDY0NmJlNTI3MjJiN2EyYzk1ZDVkNTI1YzFhYzY2MzhmYix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- \[eth2\] [Lodestar dev update](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fchainsafe-systems%2Flodestar-bi-weekly-update-1-61926ddfcdb1&t=NmVlODdiMmJhNjliOGVhMTYzNjljZDc2ZDkwNzUxYTIxMGExYTY1Mix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- \[eth2\] Dean Eigenmann and Eric Tu are [implementing the Beacon Chain in Swift](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fyeeth%2FBeaconChain.swift&t=NTg4MGMyMzk0ZTJjNjlhODdiYTA5Yjk4ZjBkYTRhMzEzZTNhYjlkNSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- \[eth2.x\] What [CBCifying the beacon chain](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2Feth2.0-specs%2Fissues%2F433&t=NmZkNjQ3ZTVhYTcyMWMyMDcwM2M2Nzg4OTkyYjI3MjNlMTM1ZTMzMSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) would look like  
    
- \[eth2.x\] Bitwise LMD GHOST: [an efficient CBC Casper fork choice rule](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F%40aditya.asgaonkar%2Fbitwise-lmd-ghost-an-efficient-cbc-casper-fork-choice-rule-6db924e57d1f&t=NDhlYzFhM2Q1ZmVkMjJiMTk3NThlOGEyMTNkMTk3YWEwYzRhYzc1Yyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Swarm [v0.3.9](https://t.umblr.com/redirect?z=https%3A%2F%2Fswarm-gateways.net%2Fbzz%3A%2Ftheswarm.eth%2Fdownloads%2F&t=MjM5MTg1Y2JhNjIwMWJhMTRiZGIzYTNjZjFjZWNiYzFjNTBhMmRmOCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    

**Layer 2**

- OmiseGo [Plasma update](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fomise_go%2Fcomments%2Fag5btg%2Fplasma_update_11_january_4_2019%2F&t=ODhhMWM5MjBiNmYxMmMwZjUzYjNjNzUwODYyYjM1OTUxNDI5YTQ5MSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- [Encumberments as a common mechanism in sharding and L2](https://t.umblr.com/redirect?z=https%3A%2F%2Fethresear.ch%2Ft%2Fencumberments-as-a-common-mechanism-in-sharding-and-l2%2F4828&t=ZTVjOGQyZjA3ZjgyOWVjNGI1YmQ1ZmZiNzlmNDY1ZDJiNGM2ZDRhZix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- [Plasma snapp-1-bit](https://t.umblr.com/redirect?z=https%3A%2F%2Fethresear.ch%2Ft%2Fplasma-snapp-1-bit%2F4802&t=MTllNDJlYTE0NzhmMWIzNWIwOTljMDA3N2I0ZjI2NWRlM2Q1N2FlYix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Aragon’s [Voting Relay Protocol](https://t.umblr.com/redirect?z=https%3A%2F%2Fforum.aragon.org%2Ft%2Fsimple-voting-relay-protocol-optimistic-vote-tallying%2F473&t=MjE3ZDQ4ZGQ2MTM3OGRlMTUwNmZmMTIyN2U4ZjE2NGUxYTk2NGFlNyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) for optimistic vote counting  
    
- [Connext dev update](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fconnext%2Fconnext-biweekly-update-6-180d15a5fd5c&t=Yzk3Y2I1NDRhZWViY2E5YWMxNzFlNGIyNDNmNzczMTM4MzVlYTU2YSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Loredana Cirstea on [building CryptoBotWars on Raiden](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F%40loredana.cirstea%2Fcryptobotwars-or-how-to-build-shitty-demos-and-why-19b5ecf60c76&t=MjE1ZWJiMzBjZTE0ZmI5NjAyNGJkM2UyMzVkN2ExZDhiYzBmNDA1NCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    

**Stuff for developers**

- [0x dev tools suite](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.0xproject.com%2Fnew-ethereum-dev-tools-from-0x-db80ee9e802&t=YjRhMjNmYzA3MjAzNTRlNDMyODE1ZTQ1MzRkMzhjZjJmMjYxZDQ4ZCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0): compiler, tracer, code coverage measurer, and gas profiler  
    
- Trail of Bits’ Slither [v0.5.0](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Ftrailofbits%2Fslither%2Freleases%2Ftag%2F0.5.0&t=YThjNjc2ZmZkN2Y0NjNhNjI0YzFmYjkwNjgyZGIxNzhmMzQ5MWIwNCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) static analyzer  
    
- Panvala’s first [token grant applications](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F%40Panvala%2Fpanvala-token-grant-applications-from-gnosis-status-and-level-k-be63ae503ca9&t=MjRkNWIyMmNkNTBhNWM4YzhhMWQyYmI2OTQ1ODMxMDVmZmM3NjA0OCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- A flow chart [analyzing the potential EIP1283 attack](https://twitter.com/mandrigin/status/1085579865380843520)  
    
- Using the [Truebit file system](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Ftruebit%2Fusing-the-truebit-filesystem-f6a5d4ac9604&t=MTBhNGRkZTJkZjNhYjBkNmZmYTJhOGYxNzFhZTIxNTJlYzI5MTUxNSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- [Rust bindings for the Solidity compiler](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Faxic%2Fsolc-rust&t=ZGJmYTI4YTkzMTgwZTFiZTczMWVkMzAwNmY5MTU0NTk4ZjcyOTFkOCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Python [REST api for JSON-RPC Infura calls](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fkevern-zacksor%2FinfuraREST&t=ZGE5ZWRmOTU5NTIyYTFiNDY3MWE3NTMwZjQwMTVkMzVmZDYzMzA0ZSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- On [efficient Eth addresses](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fcoinmonks%2Fon-efficient-ethereum-addresses-3fef0596e263&t=NzM4MmI0NGRiN2RmNjgwMjQxZjY0YzU3M2ZjNTFhZTUxZTc5Y2U5ZCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) to eek out gas savings  
    
- [Automatic authentication signatures for web3](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F%40wighawag%2Fautomatic-authentication-signatures-for-web3-dcbcbc64d6b5&t=YzYzYzNiOTg0MmFmNDI1YTZkZjRhZTlhN2NiNGM5ZDljNTk5YzE5Yix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Mintable’s SDK to [generate ERC-721s](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F%40Mintable%2Fmintable-create-erc-721-sdk-js-library-for-generating-erc-721-tokens-update-and-release-9dd7095d2aa0&t=NThmYzViNDNmYzVkN2IyMDY1Yzg1MGRmNGE2NWFlNmVkZDNjNDUyNyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Piñata on [IPFS economics](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fpinata%2Fthe-ipfs-dilemma-e3b9cd9e662f&t=NmY5MWRjODE4NGIyZGFhMTVkMmNmZjY3MzkwM2RhZTliNWRhOGVjMyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0). And an [SDK for pinning on IPFS](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fmaht0rz%2Fpinata-sdk&t=YjMzNmIzYTAxN2U2MzRhZWMwYTdkMmQ3ZTkwNDlmNjZjNDEzMjk5OCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) with Piñata  
    
- [Web3 yeet](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fweb3-yeet%2Fweb3-yeet&t=ZmVmYzFmNzc5MWMwMjBmYmE2M2YzNjA1ZGM5MjUxZDg1Y2MxNzgxMCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) wraps most common web3js operations for one line use  
    
- draft of [code for ENS permanent registrar](https://t.umblr.com/redirect?z=https%3A%2F%2Fdiscuss.ens.domains%2Ft%2Ffirst-draft-of-the-permanent-registrar-contracts-feedback-welcome%2F787&t=ZTk5YzMzMjc5MDNjZjI3ZTc4ZGIxZTUxZDkxYTM1ZDI2Y2ZhNjU2OCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    

**Live on mainnet**

- Augur interface [Veil launches on mainnet](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fveil-blog%2Fveil-is-live-on-mainnet-6cdbf870f230&t=NmFlMTBjMDMwMTc4MWQxMmNkNTg2ZTBiOGIxYTYwZWRjNTQxMDA4ZSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- [STK payment channels](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fstk-token%2Fstk-is-live-on-ethereum-mainnet-ce8808a104c0&t=OWIxZWE1OTJjYTFkOGI0ZWNjMzRkMTJhMWZmYTk3MGJjNjE2MGUyNyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) live on mainnet  
    
- [Urbit Address Space](https://t.umblr.com/redirect?z=https%3A%2F%2Furbit.org%2Fposts%2Fessays%2Fazimuth-is-on-chain%2F&t=NGVlZjAxODRlYzM0ZGY5ZDhhNGExODE3ZTA1ZDFkZDVlOGUwNDU3Nix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) live on mainnet. You may find the [Urbit Primer](https://t.umblr.com/redirect?z=https%3A%2F%2Furbit.org%2Fprimer%2F&t=MzZhMTg2NDU4ZDc2YzRkMzllMzc5YTJjY2MwMzBlNzE1NGFjMzlhMix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) useful  
    

**Ecosystem**

- The [Year in Ethereum 2018](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F%40jjmstark%2Fthe-year-in-ethereum-87a17d6f8276&t=OTAzZDRkYmQxYzQ3MDBmZTYyMGEzZmE4NmY4NWVjNDllMGU3ZTFkMSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0). #longreads  
    
- Andrew Keys’ [2019 predictions](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedia.consensys.net%2Fwelcome-to-the-fourth-industrial-revolution-19-blockchain-predictions-for-2019-8b2e542bf86a&t=ZTVlMjMzYjZmZWRiZGUyOWNkOGFmMzlhMmY3NmI3MmEzZTRhNzE5OSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- New [ENS manager](https://t.umblr.com/redirect?z=https%3A%2F%2Fmanager.ens.domains%2F&t=YTQxZmRhY2Q4MjY1N2E1ZWNhOTU3Nzk2MjU3NTgzZTZlNzRhMzlkYyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Parity [Fether v0.2 beta](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fparitytech%2Ffether-beta-is-out-check-it-out-and-tell-us-what-you-think-c5f38ff0d867&t=ZDI3OTI3MjI2MTlkNDc5N2Q4ODY5YTc0Njc3YjExMGRjMmJhYTRiNCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) light-client based wallet  
    
- Austin Griffith: onboarding new users with [Burner Wallet point of sale](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F%40austin_48503%2Fdecentralized-cypherpunk-speakeasy-2fdbdc446318&t=N2VmNTkzOTFkNWIzMjRkNjc0ZTNhYmQyMDhkY2E5OTNiYTRhZDk2YSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- New [Etherscan beta](https://t.umblr.com/redirect?z=https%3A%2F%2Fbeta.etherscan.io%2F&t=OTcyMTk4NzhiYjJmNmE3NGU3MTQ1MGMzNjRjNDNkYzdjNDUzZTMzZCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) site  
    

**Enterprise**

- Quorum [v2.2.1](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fjpmorganchase%2Fquorum%2Freleases%2Ftag%2Fv2.2.1&t=NTU3ZTQ2MzM5MWE1ZDYwODljMDAwOGU5YWQ2Y2MxMDE3YWE0MTkzMix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) and Tessera [v0.8](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fjpmorganchase%2Ftessera%2Freleases%2Ftag%2Ftessera-0.8&t=ZmQ3N2U4ZWE0ZmYzMGU5ZmI1ZDhiMmJiMzhkZTYwMGM4NWM3ZTc3Yyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Oaken Innovations’ [toll road transactions pilot](https://t.umblr.com/redirect?z=https%3A%2F%2Fdevpost.com%2Fsoftware%2Fproject-vento&t=YmVkMTMwOGRmMzZhMjA5Yjc4MDI4NDhhOTQxMTgxMjAyOTMwM2M3MCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    

**Governance and Standards**

- Latest [core devs call](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3D45mrrVrw4x8&t=NjQxNTc5YTllNDU0ODhkOGFlMWQyZjgyODllODZjNTlhZjJjNGMwNSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0). [Agenda](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2Fpm%2Fissues%2F70&t=NTZlMzE2NGQ5Yjg2YzAxYmZmZDBiNjBmMGQyMDMyOGRlNzgzN2ZkNix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) to follow along.  
    
- List of [Aragon proposals up for a vote](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F%40lic%2Fpersonal-review-of-agp-proposals-for-the-jan-24th-2019-vote-a25bc53507b6&t=MGQ1NjRmYTUyZTRkN2EyZTM0NzhjZmU5YjM3MTM5NjFmOTFhNjU4ZSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) on the 24th.  
    
- 2019: the [year of the DAO](https://t.umblr.com/redirect?z=https%3A%2F%2Ftokeneconomy.co%2Fwhy-2019-will-be-the-year-of-the-dao-20f18117e4c1&t=NWJkMzg0MDU0M2NjNGU1YTE5NmVhNDc3MjQyYWUxNmM0ZGExOTdiNSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)?  
    
- Kristy-Leigh Minehan on [ProgPoW tradeoffs between Nvidia and AMD](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.reddit.com%2Fr%2Fethereum%2Fcomments%2Fag0bgu%2Fopinion_asic_resistance_is_a_state_of_mind_not%2Fee3ez6o%2F%3Fcontext%3D3&t=OThhMWZmYTNjMTA1ODA4ODg5MmQ4Y2U3NGE0NGUwNGQwNzg3Y2M3ZCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- ERC1710: [URL format for web3 browsers](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2FEIPs%2Fpull%2F1710%2Ffiles&t=ZGVhZmMzZTJiZmE1YTllODQ0ZmFmYzUyOTNlOTgwYTI0MjMwOGYwMix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- ERC1700: [non-exhaustible token](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2FEIPs%2Fissues%2F1700&t=ZTlmYjE5NjE5ZTUyYjc0NjkyMzg3MzBmMWNlNmY1ZTBiYTQ1M2YwOCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- ERC1702: [generalized account versioning](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2FEIPs%2Fpull%2F1702%2Ffiles&t=ZDg4NGFhMWQxZTZjNzk1ZjQzNDYwZTUwNzRiZWQzNWYzOGUwNDhhMyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)scheme  
    
- ERC1707: [version byte prefix for account versioning](https://t.umblr.com/redirect?z=https%3A%2F%2Fgithub.com%2Fethereum%2FEIPs%2Fpull%2F1707%2Ffiles&t=MzhjNTkzNDcyNTNkYmM4MDQzMjg1MTliYzgzZWUzN2Y3OWVkN2VkNyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    

**Application layer**

- 0x roadmap: [ZEIPs](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.0xproject.com%2F0x-roadmap-part-1-zeips-d5cb8458584e&t=YTg0NWQyN2Q2NmFhMDAxNmFlMzIzZDBkZWM2NWIxYzgxOTc1OTg5ZCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0). Also a new look [0xTracker](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F0x-tracker%2Fa-fresh-new-look-for-2019-fde73925bfb5&t=Yzc4MjQ5NGIwNTU1MDkwNzRmNzlhOWRlMGM5YzliNDM2YTUxNjRmOSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0).  
    
- Understanding the risk/reward of [providing Uniswap liquidity](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F%40pintail%2Funiswap-a-good-deal-for-liquidity-providers-104c0b6816f2&t=NGRjOTAzNDBkMGRhZjAxOTk4OTQ3Njk2MmI5ZWU0YTBjYTE3Y2E1Nyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Ari Juels on [Chainlink and TownCrier](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.chain.link%2Ftown-crier-and-chainlink%2F&t=NmVjYzU5ZGUzYjliMTI0NjMzYjg2NDgzZjc0OTg5NzE1NjEzZmM4OSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Brave’s opt-in [ads paying 70% to user are live](https://t.umblr.com/redirect?z=https%3A%2F%2Fbrave.com%2Fbrave-previews-opt-in-ads-in-desktop-browser-developer-channel%2F&t=Y2JjZGI2NmU4ZGViMjFlYWI0NjcyMmI4YzUwYTIwYmUzOTI2Njk5ZCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) in their dev release. I tried it - slightly unexpected, but I like it.  
    
- Monetha’s [decentralized reputation framework](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.monetha.io%2Fframework-intro%2F&t=NGVkOWJmMjU4MGVmMTI0NTJjZjQxMDUxZGY0ZDUxYmI1NTBmMTZmMix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Ryan Yi on Augur’s [dispute resolution mechanism and US Congressional elections](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.coinfund.io%2Ftrolling-with-rep-c5b6e1e0461&t=YTRiN2U1ZGMwMTljMWQ1NWNkNDI4MmFkMGNkYjUxYjM1NTQ4ZDJjZix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Gnosis to [prime the liquidity pump for DutchX](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.gnosis.pm%2Fthe-dutchx-take-part-in-the-arbitrage-opportunity-eeacc20ef6f&t=ZjkwMzU0Yjc5ZmEwYzllMzA4Mjk2MDBhMmEwOTU0MjllZjYwNDg4Nix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) with some DAI/ETH orders  
    
- Althea beta release “to dynamically [route, buy, and sell bandwidth](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Falthea-mesh%2Falthea-development-update-63-beta-1-4dd918bda2d&t=OGNkZTMxOTEwYmEyNDMwZjI2ZTU3ZDhmZmMzODI4MzIwNThhM2Y1ZCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)” with Eth  
    
- Maker to [completely rebuild Oasis](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fmakerdao%2Fa-new-oasis-5b9539a64adf&t=ZGIyN2U1NDdjYjE3ZjY4OWM0NjQxMTJhNTViMzJlYzAxZGUxMDNhNyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) and will remove OasisDex and Oasis.direct frontends on Jan31  
    

**Interviews, Podcasts, Videos, Talks**

- [Multiparty Computations](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.zeroknowledge.fm%2F60&t=YmI0NDFkNDc0YTRlNzBmN2RhMGFhYzVkMTczNmE4OTcxOGVjYjU2Myx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) episode of Zero Knowledge  
    
- [Andrew Keys](https://t.umblr.com/redirect?z=https%3A%2F%2Fsoundcloud.com%2Fdecentralize-this%2Fep-16-building-a-stronger-consensys-in-a-decentralized-world&t=YzJhYWM0NjQzMzVhOTRlMmQyYjJlODA5ODVjY2I5YjM5YmY5YmNlYyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) talks ConsenSys 2.0 on Decentralize This  
    
- [Decentralized Data Now](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DyEnwuEhKEG8&t=OWFhYzkwNmM4M2Y5ODc4NTNlYzkwNGY3N2Q1Nzk3MTMwNDdiNWE2Zix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) call. Formerly open source block explorers  
    
- [Andy Bromberg](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.thesmartestcontract.com%2F28&t=ZmM1YzEzNGJlNjJiYjBlODNlNTg0YTI2NDZhZmEzMTE2NTNmMmQ5Yix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) on the Smartest Contract
- Settle’s [Scott Lewis](https://t.umblr.com/redirect?z=https%3A%2F%2Fpodcast.ethhub.io%2Fsettle-the-platform-for-open-finance-with-scott-lewis&t=ZDc0ZGM5OTFjYWQ5Njc4MmU0Yjk4ZDEzMDkxMTU5ZGZmYzQzOTk1Mix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) on Into the Ether  
    

**Tokens / Business / Regulation**

- Status [app store curation mechanism](https://t.umblr.com/redirect?z=https%3A%2F%2Fbeta.observablehq.com%2F%40andytudhope%2Fdapp-store-snt-curation-mechanism&t=ZTI4ZjJjMGIyMWUzMTA4YjM2ZTY3MjU2Nzc4NjFiMjlhOWFmODUxNSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Brooklyn Project: the [state of regulation in 2019](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedia.consensys.net%2Fstate-of-regulation-2019-1d99c65b0201&t=MGZkM2Y0NTQyNDg5ZDg4NjE4YzNkMzA1MjNjMzk5YWY2NzNmODBkZSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- [Continuous Organizations 1.0](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F%40thibauld%2Fcontinuous-organizations-v1-0-45d42b3082bb&t=OGVlODA5MzkwZTYzOWM2ODAxOGIxYTVlMzBiYzUwN2Q0YjQ0N2ZhNSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- de la Rouviere: [Moloch DAO and collapsing the firm](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F%40simondlr%2Fthe-moloch-dao-collapsing-the-firm-2a800b3aa2e7&t=MWQ5YTUzMmNlNDVkM2I5NmUzMGYxYmZiMTM1NmY1NTFhNTY5NGNmNCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    

**General**

- [Implementing secp256k1 on Secure Scuttlebutt (SSB)](https://t.umblr.com/redirect?z=https%3A%2F%2Fethresear.ch%2Ft%2Fimplementing-secp256k1-on-secure-scuttlebutt-ssb-to-create-cross-platform-ethereum-scuttlebutt-applications%2F4848&t=MTUzZDIwZDRkZmNmNjdmMzc3NWM1ZmVjYTk3ZjliMmE5YTc2OTI1YSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) to create cross-platform Ethereum-Scuttlebutt applications  
    
- Ex-BitTorrent employee Simon Morris on [lessons for crypto from BitTorrent](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2F%40simonhmorris%2Fwhy-bittorrent-mattered-bittorrent-lessons-for-crypto-1-of-4-fa3c6fcef488&t=ODE1OGIyMWNhNDgxZDczMWI2YzQxZGY1ZTNlMzBiZjhiNzcyNzVmNyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) (link to part 1 of 4)  
    
- CBInsights: how [blockchain could disrupt insurance](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.cbinsights.com%2Fresearch%2Fblockchain-insurance-disruption%2F&t=NWNkN2Y2MDMyYWMzMjQ4MzUxOTkyYTdlZmI0M2RkMjU5MTg0MDhlOSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Shapeshift on [2018 law enforcement requests](https://t.umblr.com/redirect?z=https%3A%2F%2Finfo.shapeshift.io%2Fblog%2F2019%2F01%2F18%2Fpulling-back-the-curtain-how-shapeshift-handles-law-enforcement-compliance%2F&t=N2Y3MDZlODFkMDk5MzYzMDlhOTFmMDllYmJiNTQwZjEzYzVmNzIzOCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Profile of [DuckDuckGo and founder Gabe Weinberg](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fs%2Fstory%2Fnothing-can-stop-google-duckduckgo-is-trying-anyway-718eb7391423&t=M2M4MDc1YmUxMzBkN2NiODMwZGZlMzIyNDJhY2M2NGQ3NGU2YTE1NSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- Gitcoin planning on [experimenting with Liberal Radicalism](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fgitcoin%2Fexperiments-with-liberal-radicalism-ad68e02efd4&t=ZGZjZmZmMjgwNmEwZmNkNGUzYWE5N2ZlNDdmN2Q0ZWM3MjE4ZWRjMSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) with its grants  
    

## Dates of Note

Upcoming dates of note (new in **bold**):

- **Jan 23 - Infura [Project ID prioritization](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.infura.io%2Finfura-dashboard-transition-update-c670945a922a&t=ZDZmMWM2MjQ1MjYyZmQzYmU4NjllMTk4MDdmM2JmMWVkNDY2MDMyNyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)**  
    
- Jan 24 - List of things for [Aragon vote](https://t.umblr.com/redirect?z=https%3A%2F%2Fforum.aragon.org%2Ft%2Fagp-vote-1-megathread%2F443&t=ZmYxZjdjMjk0ZWY0MTgzN2VhNjQ2YWM1YzkwMDc5NTIzNWEyNTRhMSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0), including on funding original AragonOne team  
    
- Jan 25 - [Graph Day](https://t.umblr.com/redirect?z=https%3A%2F%2Fthegraph.com%2Fgraphday&t=OGQ3NTE5OWEzNzE4MmY4ZTJmNmFmZDUzMTVmNWMwMWI3NTg0N2MwYSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) (San Francisco)  
    
- Jan 29-30 - [AraCon](https://t.umblr.com/redirect?z=https%3A%2F%2Faracon.one%2F&t=NmMwMTVlNmQzYzg4ZjM2YjhmODkwOGQ3MzhmNDUxOGE3N2QyOGExOSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) (Berlin)  
    
- **Jan 30 - Feb 1 - [Stanford Blockchain Conference](https://t.umblr.com/redirect?z=https%3A%2F%2Fcyber.stanford.edu%2Fsbc19&t=ZWEwZjc0MWE0NzVmZWRkNGViNzQ1OTVkMDUzZGU5Y2I5YjYxOWZjZSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)**  
    
- Jan 31 - [GörliCon](https://t.umblr.com/redirect?z=https%3A%2F%2Fkickback.events%2Fevent%2F0xe2d2c31c68626b6c1301a49ed50854e1cae0c8fa&t=Mjk2MDFmNjVkMmUxNjczNjQyZjBmYjQ3Yjc5NmZjMjBhOGU5MmU4YSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) (Berlin)  
    
- **Jan 31 - Maker to [remove OasisDEX and Oasis.direct frontends](https://t.umblr.com/redirect?z=https%3A%2F%2Fmedium.com%2Fmakerdao%2Fa-new-oasis-5b9539a64adf&t=ZGIyN2U1NDdjYjE3ZjY4OWM0NjQxMTJhNTViMzJlYzAxZGUxMDNhNyx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)**  
    
- Feb 7-8 - Melonport’s [M1 conf](https://t.umblr.com/redirect?z=https%3A%2F%2Fm-1.melonport.com%2F&t=ZWNkYmE2YTFhMGUxMmRiYWI4MWYxYzk0YTE3MGJiOTBhNzgzZGJlOSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) (Zug)  
    
- Feb 7 - [0x and Coinlist virtual hackathon](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.0xproject.com%2F0x-coinlist-hackathon-3b48ddbfd21c&t=NWYxM2JjMjk4YTJkMjk3YWEwNGJlZjE3YjY5NDQyNGEzYWFhNTlhNCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) ends  
    
- Feb 15-17 - [ETHDenver](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.ethdenver.com%2F&t=YWIxZTU1ODE5MjNlYWE5MzMyOGQ2ZDFjNDgzMjA4OTAwMGQxYTIzMCx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) hackathon (ETHGlobal)  
    
- **Feb 27 - [Constantinople](https://twitter.com/5chdn/status/1086285718710816768) (block 7280000)**  
    
- Mar 4 - [Ethereum Magicians](https://t.umblr.com/redirect?z=https%3A%2F%2Fethereum-magicians.org%2Ft%2Fcouncil-of-paris-2019-announcement%2F2438&t=YzI1YmUxN2M3YjEzODU4ZDMyNWFkYjQ4ODFjNTllNWMyZTVkOWI4NSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) (Paris)  
    
- Mar 5-7 - [EthCC](https://t.umblr.com/redirect?z=https%3A%2F%2Fethcc.io%2F&t=Zjk3Y2YxYjZjMmU3NDcyNmMzYTkxYjdhY2M1MmQwMzc2MGM3Yzg1Myx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) (Paris)  
    
- Mar 8-10 - [ETHParis](https://t.umblr.com/redirect?z=https%3A%2F%2Fethparis.com%2F&t=N2U1ZmMyNzQ4YjU4YzMxNTYxZTBhOTgzOTRmM2UwMWVmYTM0ZTU0ZSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) (ETHGlobal)  
    
- **Mar 8-10 - [EthUToronto](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.ethuoft.ca%2F&t=OTc5ZjY2ZDRlZjNkZmIwMTA3NmZjNTM2ZmJhMzM1ZTYyMGJjNGQ1NSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)**  
    
- **Mar 22 - [Zero Knowledge Summit 0x03](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.zeroknowledge.fm%2Fsummit&t=MWRkNWQ3MmZhZTY0YjM1ZjJiN2E4NDc3YzBkY2FiNDVlMGYxNGQ5Zix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) (Berlin)**  
    
- Mar 27 - Infura [end of legacy key support](https://t.umblr.com/redirect?z=https%3A%2F%2Fblog.infura.io%2Finfura-dashboard-update-9f02d0643eb3&t=MjI3MTcwZTc3NzVkMmI2Mzk0NGM5ODFhODUyNDk0ZDU4ZDIyZDU5YSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)  
    
- April 8-14 - [Edcon](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.edcon.io%2F&t=ZDM4NWE2M2M2Yjg2NTg4YmExOTRhYTc2MGIwMjY2ZGI1YjE1ZDU0ZSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) hackathon and conference (Sydney)  
    
- Apr 19-21 - [ETHCapetown](https://t.umblr.com/redirect?z=http%3A%2F%2Fethcapetown.com%2F&t=MTliZThiYTkwZGY1ZjgwMzcxNmIyMGFlYTZiZDdiM2RlOGExYzdmNSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) (ETHGlobal)  
    
- May 10-11 - [Ethereal](https://t.umblr.com/redirect?z=https%3A%2F%2Fetherealsummit.com%2F%3Fref%3Dweekinethereum&t=YjNlMjZkMjk2MTQ5NjZlYzUzYTBmOTI5ZDI2NzIxZWNhN2Y5N2U0YSx5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) (NYC)  
    
- **May 17 - Deadline to accept [proposals for Instanbul upgrade](https://t.umblr.com/redirect?z=https%3A%2F%2Fen.ethereum.wiki%2Froadmap%2Fistanbul&t=ZjFkOTRlMTcxOGE0NWY3NjI5YjBhMGUyNWNhNzFjOGY0NWIxYmYyZix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0) fork**  
    

## If you appreciate this newsletter, thank ConsenSys

This newsletter is made possible by [ConsenSys](https://t.umblr.com/redirect?z=https%3A%2F%2Fconsensys.net%2F&t=MzdhZTM4NjMyMWI4ZDM4YWQ3OThkZTRkNjZhYjRhYmUyZThlNWVmNix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0).  
  

![image](https://66.media.tumblr.com/e25d646c06cd8f6f4de08c91d301ee95/tumblr_inline_plk84sN7Zy1rxca3y_250.jpg)

  
I own Week In Ethereum. Editorial control has always been 100% me.

If you’re unhappy with editorial decisions or anything that I have written in this issue, feel free to [tweet at me](https://twitter.com/evan_van_ness).

## Housekeeping

Follow me on Twitter, because most of what is linked here gets tweeted first: [@evan\_van\_ness](https://twitter.com/evan_van_ness)

If you’re wondering “[why didn’t my post make it into Week in Ethereum](https://t.umblr.com/redirect?z=https%3A%2F%2Fwww.evanvanness.com%2Fpost%2F179914035841%2Fwhy-didnt-my-post-make-the-newsletter&t=M2MxOGQzY2U3NGVkMTIxYzExNGRmMzljYmY1YjBmOGJlZWRlNGNkMix5WUF6RXZybQ%3D%3D&b=t%3AQ8svKXOQOFn4j1wJ-IeWRA&p=https%3A%2F%2Fwww.weekinethereum.com%2Fpost%2F182127013533%2Fjanuary-18-2019&m=0)?”

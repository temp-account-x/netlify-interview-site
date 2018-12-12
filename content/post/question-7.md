---
title: "Question 7"
date: 2018-12-11T21:46:09-08:00
draft: false
---

## Explain, in a couple of paragraphs, what you think 2 major challenges around DNS configuration are for less-technical internet end-users.

If you are hosting your own BIND server, you know how unique the configuration find syntax for 'named' is. The text file format of DNS records is not something less-technical people are likely to have seen before and even less likely to find accessible.

Then there is the fact that many domain registrars have created their own  web interfaces to allow people to configure their DNS setting without actually editing any text files. This is great for opening up markets to sell domains to less technical people but it also means there is now a layer of abstraction which exists to make things 'easy' for the domain purchaser. But the same layer of abstraction which helps the purchaser is also now obscuring details (possibly important details) about how the DNS settings are configured.

Finally, there is the fact that DNS is distributed, decentralized, and records have TTL values. This means the user may have correctly updated their DNS settings with their registrar or DNS provider but it could still take hours or days for those same updates to reach their end users. This interdependency on other DNS servers and the delay between changes on one system reflecting in another are important nuances of how DNS functions, and without this knowledge, less-technical end-users may be confused by these delays.

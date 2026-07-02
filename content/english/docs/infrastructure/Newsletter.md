---
date: 2026-07-02T17:31:07+01:00
modified: 2026-07-02T17:31:13+01:00
description: We use Buttondown for our newsletters
author: Jake Rayson
---
- We use the [Buttondown](https://buttondown.com/) newsletter platform
- Our Buttondown page is here buttondown.com/NaturCeredigion
## Spam
- To reduce our newsletters being marked as spam (this happened to Bob!), I have added a subdomain `newsletter.naturceredigion.cymru` to our DNS servers (currently managed by Netlify).
- A reply email address is set up for this subdomain, `biodiversity@newsletter.naturceredigion.cymru`
- We are using the [ImprovMX](https://app.improvmx.com/) service to route email sent to `biodiversity@newsletter.naturceredigion.cymru` to go to biodiversity@ceredigion.gov.uk 
- I have add some MX records and a TXT record to the DNS server on Netlify for this to work.
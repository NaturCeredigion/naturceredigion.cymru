---
title: Newsletter process & infrastructure
draft: false
description: Things to look out for in creating the newsletter in Buttondown
date: 2026-09-18T15:05:46+01:00
modified: 2026-11-11T10:58:17+00:00
---
1. [Process](#1-process)
	1. [Buttondown Markdown notes](#11-buttondown-markdown-notes)
	2. [Images, URLs & PDFs](#12-images-urls--pdfs)
	3. [Structure](#13-structure)
	4. [Sections](#14-sections)
2. [Infrastructure](#2-infrastructure)
	1. [Spam](#21-spam)
## 1. Process
### 1.1 Buttondown Markdown notes
- Insert blank lines above & below lists eg
```
Have you captured images of:

- Low water levels in rivers, streams, reservoirs or ponds?
- Dry fields, parched land or struggling crops?
- Effects on wildlife, livestock or local habitats?

We’d love to see what you’ve noticed.
```
- List formatting in Buttondown can break (extra line spacing added) when switching between Markdown & Fancy modes. To fix, enter Markdown mode, then delete and re-insert the blank line above the list. 
- Headings
    - **Not** bold!
    - [Sentence case](https://en.wikipedia.org/wiki/Letter_case#Sentence_case) headings
- Line breaks
    - A Markdown paragraph is *two* returns.
    - A Markdown **line break** is *two* spaces followed by *one* return eg
```
To book your slot and save money per tonne call:  
Birch Farm Plastics on 01792 869 776.
```

[↑ Top ↑](#)
### 1.2 Images, URLs & PDFs
- Images in the body of the newsletter need to be imported, not linked, else they won't display in Windows Outlook.
- Clean the URLs, ie remove tracking parameters, using eg Chrome Extension [Get Clean URL](https://chromewebstore.google.com/detail/get-clean-url/mobpimjmmonkghndllikpdgpapkfckje)
- [Compress images](https://caesium.app/)
- [Compress PDFs](https://www.ilovepdf.com/compress_pdf)

[↑ Top ↑](#)
### 1.3 Structure
- **Title:** 
    - Newyddion Natur Ceredigion 02/10/26
    - Ceredigion Nature News 02/10/26
- **h1:**
    - Newyddion Natur Ceredigion
    - Ceredigion Nature News
- **h5:** 
    - \[**Fflach Newyddion** —] dydd Gwener 2 Hydref 2026
    - \[**Newsflash** —] Friday 2nd October 2026
- **h4:** Call To Action
- **h2:** Section heading (**not** bold!)
- **h3:** Item heading (**not** bold!)

[↑ Top ↑](#)
### 1.4 Sections
#### General
- Activities
- Wild learning
- Webinars
- Wildlife talks
- Farming
- Consultations
- Funding
- Local nature services
- Jobs
#### Specific
- West Wales Wildwatch
#### Species
- Bats
- Frogs & Toads
- Water & Wildlife
- Fungi

[↑ Top ↑](#)
## 2. Infrastructure
- We use the [Buttondown](https://buttondown.com/) newsletter platform
- Our Buttondown page is here [buttondown.com/NaturCeredigion](https://buttondown.com/NaturCeredigion)
### 2.1 Spam
- To reduce our newsletters being marked as spam, I have added a subdomain `newsletter.naturceredigion.cymru` to our [DNS](https://en.wikipedia.org/wiki/Domain_Name_System) servers (currently managed by [Netlify](https://www.netlify.com/)).
- A reply email address is set up for this subdomain, `biodiversity@newsletter.naturceredigion.cymru`
- We are using the [ImprovMX](https://app.improvmx.com/) service to route email sent to `biodiversity@newsletter.naturceredigion.cymru` to go to biodiversity@ceredigion.gov.uk 
- I have add some [MX records](https://en.wikipedia.org/wiki/MX_record) and a [TXT record](https://en.wikipedia.org/wiki/TXT_record) to the DNS server on Netlify for this to work.

[↑ Top ↑](#)
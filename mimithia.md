# ScrollBot: An AI Agent That Reads Infinite Scroll Pages

## Summary

ScrollBot is a browser automation tool that scrolls through infinite-scroll pages such as  social feeds, product, marketplaces and pulls out exactly the data you ask for, without anyone having to write a custom scraper for every site. Instead of having specific programs for each site, you can instead give instructions to scroll bot and it will locate exactly what you are asking for. 

## The Problem
People have to browse they large amounts of continuous pages like amazon for instance, and that process is very tedious, and delivering people this product makes their lives easier, as they cut down on time spent looking for their desired product. 

## Major Features

**Natural-language extraction targets**: user describes what they want ("product name, price, rating") instead of writing selector code
**Human-paced automated scrolling**: handles dynamically loaded, lazy-loaded content the way a real user's scrolling would
**Configurable stop conditions**: item count limit, time limit, or automatic detection when no new content is loading
**Live progress dashboard**: watch a run collect data in real time instead of waiting on a black box

## Technologies

**An LLM API** to interpret inconsistent or messy page structure that fixed selectors would miss
**React** for a lightweight live-progress dashboard

## Who This Is For

ScrollBot is built for anyone who regularly needs structured data off the web and doesn't want to maintain  site-specific scripts. That includes researchers building datasets from social platforms, and mainly shoppers who are always using stuff like temu and amazon. For all of these users, the pitch is describing what they  want once, and letting ScrollBot adapt to the page.

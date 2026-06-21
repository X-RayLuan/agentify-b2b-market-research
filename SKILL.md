---
name: agentify-b2b-market-research
description: Use when Ray wants a B2B export market-research skill built around a 1688 or Alibaba supplier page, especially for OEM/ODM factories that need overseas competitor mapping, ICP definition, outbound prospecting strategy, and inbound social plus SEO/GEO plans. Applies to requests about ZekSmart, smart mirror suppliers, store-url-based competitor analysis, go-to-market research, and export-market positioning.
---

# Agentify B2B Market Research

Use this skill to turn a `1688` or `Alibaba` supplier page into an export GTM brief that a team can act on. The default example is ZekSmart, but the workflow should stay reusable for other B2B OEM/ODM suppliers.

## Core Output

Produce four decision-ready sections:

1. `Top 5 competitors`
2. `ICP`
3. `Outbound marketing plan`
4. `Inbound marketing plan`

The input is usually one of:

- a `1688.com` store URL
- an `alibaba.com` storefront or company URL
- a supplier name plus one storefront URL

## Default Stance

- Treat the storefront as the supplier truth anchor, not the whole truth.
- Separate `evidence` from `inference`. Mark assumptions plainly.
- Prefer direct competitors with overlapping product, price band, export region, and buyer type. Do not fill the top 5 with giant unrelated brands.
- For contact or social claims, use public sources only. Do not invent emails, LinkedIn people, certifications, or distributor relationships.
- Cite raw sources only. Do not expose upstream search vendors in the final report.
- The goal is actionability for export sales and content teams, not generic market commentary.

## Workflow

### 1. Normalize the supplier input

Extract and write down:

- company name
- storefront URL
- product categories
- minimum order / sample posture
- OEM / ODM claims
- visible certifications
- export markets or language clues
- contact surfaces shown publicly

If both `1688` and `Alibaba` exist, use both. If only one exists, continue with that one and note the gap.

### 2. Build the supplier snapshot

Before competitor hunting, summarize the supplier in 8 to 12 bullets:

- what they actually sell
- which products appear core vs edge
- whether they look like factory, trader, or hybrid
- quality / certification signals
- whether the motion is project-based, channel-based, or commodity wholesale
- which overseas use cases are implied

For ZekSmart-like cases, explicitly decide whether the business is selling:

- a hardware component
- a branded finished product
- an OEM/ODM solution
- a project-delivery package

### 3. Find the top 5 overseas competitors

Pick competitors that overlap on:

- product category
- buyer type
- export region
- solution depth
- channel model

Use the following buckets to search:

- direct manufacturer competitors
- OEM/ODM smart-solution suppliers
- independent-site exporters
- Amazon / B2B marketplace-visible players
- hospitality / project / distributor-oriented suppliers

For each competitor, capture:

- company name
- website
- source URLs
- overlap reason
- primary markets
- main products / solution angle
- pricing or MOQ clues if public
- certification / proof signals if public
- social footprint
- SEO / GEO footprint
- why they are dangerous to the supplier

Score each competitor on a simple 1 to 5 scale:

- `product overlap`
- `channel overlap`
- `content strength`
- `proof / trust strength`
- `threat level`

### 4. Define the ICP

Do not stop at broad industry labels. Build ICP as a buying committee and use-case model.

Required fields:

- primary ICP segment
- secondary ICP segments
- geography
- company type
- buyer roles
- buying trigger
- pain points
- proof required to close
- likely objections
- average deal shape: sample / pilot / bulk / project

For ZekSmart-style smart mirror suppliers, usually test these segments first:

- distributors / dealers
- hotel and hospitality project buyers
- real-estate / apartment project procurement
- salon / beauty chain buyers
- retail or commercial-space digital experience buyers

State which one is `Tier 1`, `Tier 2`, and `Tier 3`, and why.

### 5. Create the outbound marketing plan

Build a plan the sales team can run next week.

Required sections:

- target account types
- target titles / roles
- best outreach channels
- region priority
- value proposition by ICP tier
- offer / CTA
- prospect list criteria
- 2-week outreach sequence
- sample first-touch angle
- proof assets still missing

Outbound should cover at least:

- email
- LinkedIn
- distributor / procurement portal applications
- trade-show or directory follow-up if relevant

For each ICP tier, specify:

- what they are buying
- what message angle should lead
- what proof asset would unlock reply rate

### 6. Create the inbound marketing plan

Split inbound into `social` and `site`.

#### Social analysis

Audit the supplier and top competitors across the public surfaces you can verify:

- LinkedIn company presence
- Instagram / Facebook / YouTube / TikTok when relevant
- content themes
- posting frequency
- proof content quality
- whether posts are brand fluff, catalog dumps, or buyer-useful content

Output:

- current gap
- 3 content pillars
- 10 post angles
- 3 proof-first assets to create

#### Independent-site SEO / GEO

Audit what a buyer would see from search and AI retrieval:

- homepage positioning clarity
- product/category page coverage
- comparison / use-case / solution pages
- trust and certification pages
- case-study / project pages
- FAQ / buyer-question coverage
- schema / crawlability / `llms.txt` / sitemap clues if visible

Output:

- core keyword clusters
- comparison keywords
- buyer-intent long-tail questions
- must-build landing pages
- trust pages to add
- GEO assets to add: `llms.txt`, FAQ blocks, comparison pages, case studies, structured data
- 30-day content plan

### 7. Deliver the final brief

Use the structure in `references/report-template.md`.

The final report must let a team answer:

- who we are actually competing with
- who we should sell to first
- how we should outbound them
- how we should inbound-compound trust and discovery

## Research Tools

Choose the smallest set that gets grounded evidence:

- `openclaw_web_search` for competitor discovery and public social/company traces
- `openclaw_web_fetch` for reading websites, category pages, blogs, and visible policies
- `openclaw_browser` only when static fetch is insufficient
- Feishu doc tools when the result needs to be written back into a document

Read `references/data-sources.md` for suggested search patterns and evidence rules.

## Quality Bar

Before finalizing, check:

- the supplier snapshot is specific enough that another person could tell what business model this is
- the top 5 are true competitive alternatives, not random market neighbors
- each ICP tier has buyer roles, trigger, proof need, and likely objection
- outbound has concrete channels, message angles, and sequence logic
- inbound covers both social proof and independent-site SEO/GEO
- every non-obvious claim has a source URL or is explicitly marked as inference
- no fake contacts, fake certifications, or fake market shares were introduced

## Output Rules

- Keep the writing tight and operator-facing.
- Use tables where comparison helps.
- Put `Evidence` or `Source` links inline for each competitor.
- When data is missing, write `Not publicly verified`.
- If the user asks to add results into Feishu, append the finished brief and then add a compact action table for the team.

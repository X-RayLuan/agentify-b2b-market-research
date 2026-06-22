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

Use the following buckets to search. Cover EVERY bucket — an empty bucket is a coverage gap, not a "no competitors here":

- direct manufacturer competitors
- OEM/ODM smart-solution suppliers
- independent-site exporters
- Amazon / B2B marketplace-visible players
- hospitality / project / distributor-oriented suppliers
- premium / category-benchmark brands (often OFF marketplace, higher price tier, sell via design-spec or authorized dealers — e.g. the "ceiling" brand of the category)

#### Do not miss benchmark competitors (anti-blind-spot rule)

A single-axis search ("same product + same price band + same channel") will systematically MISS the premium/benchmark players, because they are not on Alibaba/1688, their price band is filtered out, and they rank for `brand / hospitality / designer` keywords, not `manufacturer / OEM / wholesale`. Run all three nets:

1. **Tier sweep** — always run one query set per price/positioning tier, never just one:
   - premium / ceiling: `best <product> brands`, `top <product> companies`, `luxury <use-case> <product> brand`, `designer-specified <product>`
   - same-pool OEM/ODM peers: `<product> OEM/ODM manufacturer china`
   - commodity / low-price: `cheap <product> wholesale`
2. **Demand-side reverse search** — find competitors by who the ICP actually buys, not by supply-side keywords: `<ICP> preferred <product> supplier`, `<flagship hotel/brand> <product> brand`, `which <product> brand do designers/hotels specify`. Premium benchmarks only surface from the demand side.
3. **Seed snowball** — from any found competitor, mine its `compare / vs / alternatives` pages, industry "Top 10" listicles, awards, and `as seen in` / customer-logo walls to reach the next batch.

**Completeness check (before locking the list):** for each price tier AND each buyer type, name the leader. If a tier is empty, you missed someone — go back.

**Principle — discover then classify, never silently omit:** the goal is NOT to force a benchmark brand into the top 5. Discover it, then consciously classify it as `direct top-5` vs `benchmark / ceiling (study, don't head-to-head)`. A benchmark consciously marked as such is correct; a benchmark absent from the report is a process bug.

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

#### How to find ICP contact details (required)

A plan that says "email procurement managers" without saying HOW to get them is not actionable. Always specify the sourcing channels, mapped to ICP tier. Use public sources only — never invent emails, names, or LinkedIn profiles; mark anything unconfirmed `Not publicly verified`.

- **Customs / import data** (the #1 export lever): find who actually imports the product. Tools: Panjiva, ImportGenius, ImportYeti (US, free), 52WMB, Tradesns. Search by HS code + product keyword, export the importer list, then enrich decision-makers via the company site / LinkedIn. Best for distributors / importers.
- **LinkedIn Sales Navigator**: lock the person by title + industry — `Procurement / FF&E / Purchasing` filtered to `Hospitality / Real Estate / Building Materials`. High hit rate in the Middle East / SEA.
- **Vendor / supplier portals**: FF&E procurement firms and fit-out main contractors usually have a `Become a Vendor / Supplier Registration` page — the cleanest official channel, highest reply rate.
- **Trade shows + directories**: exhibitor + visitor lists (Canton Fair, Big5 Dubai, KBIS US, ISH Germany) are full of buyers; hospitality-supply distributor directories double as channel entry points.
- **Company site + business registries**: once a target account is known, mine the `Contact` page and registries (e.g.企查查 / 天眼查 for China-side, public filings overseas) for the procurement / project contact.

**Demand-aggregator targeting (core strategy):** for project ICPs, do NOT chase end buyers one by one. Target the demand aggregators — FF&E procurement companies and fit-out main contractors — each holds the spec decision for dozens of projects. Getting onto their approved-vendor list = repeat orders. Output a starter account list with: account, vendor entry URL, public email/phone, key contact + LinkedIn (or `Not publicly verified`), and a one-line first-touch angle.

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
- **primary social channels + per-channel play (required)** — name the channels that matter for THIS supplier's B2B buyers and give each a positioning + concrete tactic + priority. Default channel set for export B2B (adapt per case):
  - **LinkedIn** (usually P1): the B2B battleground where procurement / project decision-makers find suppliers. Play: company page (name consistent with site + marketplace) → post project cases + certifications + factory proof; sales reps do ICP outreach from personal profiles; employees amplify.
  - **Instagram** (P1 for design/beauty buyers): visual proof. Play: real-scene Reels (hotel bathroom, salon installs), before/after, product detail, consistent brand visuals.
  - **YouTube** (P2): long-form trust + SEO/GEO asset. Play: factory walk-through, QC, anti-fog test, install tutorials; reuse clips to site + LinkedIn.
  - **Facebook** (P2): distributor / importer + Middle-East reach via B2B groups; product + project posts.
  - **TikTok** (P3, optional): product seeding for retail/beauty; test traffic before investing.
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
- competitor coverage: every price tier and buyer type has a named leader; the category benchmark / ceiling brand was discovered and explicitly classified (direct vs benchmark), never silently omitted
- each ICP tier has buyer roles, trigger, proof need, and likely objection
- outbound has concrete channels, message angles, sequence logic, AND a concrete way to source ICP contact details (not just "email them")
- inbound names the primary social channels with a per-channel play, and covers both social proof and independent-site SEO/GEO
- every non-obvious claim has a source URL or is explicitly marked as inference
- no fake contacts, fake certifications, or fake market shares were introduced

## Output Rules

- Keep the writing tight and operator-facing.
- Use tables where comparison helps.
- Put `Evidence` or `Source` links inline for each competitor.
- When data is missing, write `Not publicly verified`.
- If the user asks to add results into Feishu, append the finished brief and then add a compact action table for the team.

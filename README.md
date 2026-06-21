# Agentify B2B Market Research

[English](./README.md) | [简体中文](./README.zh-CN.md)

Turn a `1688` or `Alibaba` supplier page into a decision-ready B2B export market brief.

This skill is designed for OEM/ODM suppliers that want to identify their real overseas competitors, define their ICP, and turn research into both outbound and inbound go-to-market actions. The default framing fits suppliers like ZekSmart, but the workflow is reusable for other B2B export manufacturers.

## What It Produces

The output is fixed into four operator-facing sections:

1. Top 5 competitor analysis
2. ICP
3. Outbound marketing plan
4. Inbound marketing plan

The inbound section covers both social content direction and independent-site SEO/GEO.

## Supported Inputs

- `1688.com` storefront URL
- `Alibaba.com` supplier or company URL
- Supplier name plus one storefront URL

If both 1688 and Alibaba pages exist, the skill should use both. If only one exists, it should continue and explicitly mark the evidence gap.

## Recommended Use Cases

- Export-market research for Chinese OEM/ODM factories
- Competitor mapping for a supplier before overseas outreach
- ICP definition for B2B project, channel, or wholesale sales
- Building a first outbound sequence for an export sales team
- Planning inbound content for LinkedIn, SEO, GEO, case studies, and trust pages

## Research Principles

- Treat the storefront as the truth anchor, not the full truth
- Separate evidence from inference
- Use public sources only
- Do not invent contacts, certifications, distributor relationships, or social proof
- Prefer direct competitive overlap over generic market neighbors
- Keep the output action-oriented for sales and content teams

## Repository Structure

```text
.
├── SKILL.md
├── README.md
├── README.zh-CN.md
├── agents/
│   └── openai.yaml
└── references/
    ├── data-sources.md
    └── report-template.md
```

## Files

- `SKILL.md`: main workflow, decision logic, output rules, and quality bar
- `references/data-sources.md`: suggested research paths and evidence rules
- `references/report-template.md`: final report structure
- `agents/openai.yaml`: optional agent metadata for OpenClaw-style invocation

## Example Output Shape

- Supplier Snapshot
- Top 5 Competitors
- ICP by Tier 1 / Tier 2 / Tier 3
- Outbound Plan with channel, angle, CTA, and missing proof assets
- Inbound Plan with social gaps, content pillars, keyword clusters, GEO assets, and a 30-day content plan

## Best Fit

This skill is strongest when the supplier sells one of the following:

- finished branded products with export intent
- OEM/ODM hardware
- project-delivery packages
- channel-ready B2B solutions

It is less suitable for purely domestic commodity sellers with no export or differentiation signal.

## Installation

Clone or copy this directory into your OpenClaw skills directory, then reference `SKILL.md` from your local skill loader.

## Notes

This repository focuses on the reusable skill itself, not on a single fixed company report. ZekSmart is the motivating example, but the workflow is intentionally not locked to one supplier.

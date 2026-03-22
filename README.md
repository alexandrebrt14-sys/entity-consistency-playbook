# Entity Consistency Playbook

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Schema.org](https://img.shields.io/badge/Schema.org-Entity_Consistency-2e844a)
![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

A step-by-step playbook for building **entity consistency** — the practice of ensuring that every representation of your brand, product, or person across the internet is accurate, aligned, and machine-readable.

Entity consistency is the foundation of AI visibility. If your entity information is fragmented or contradictory across platforms, large language models will either ignore you or describe you inaccurately.

---

## Table of Contents

- [What is Entity Consistency?](#what-is-entity-consistency)
- [Why It Matters for AI Visibility](#why-it-matters-for-ai-visibility)
- [The Playbook](#the-playbook)
- [Templates](#templates)
- [Cheatsheets](#cheatsheets)
- [Citation](#citation)
- [License](#license)

## What is Entity Consistency?

An **entity** in this context is any thing that AI systems need to understand: a company, a product, a person, a service. Entities have attributes: names, descriptions, locations, relationships, facts.

**Entity consistency** means that every representation of your entity — across your website, social profiles, directories, press mentions, Wikipedia, review platforms, and structured data — tells the same story with the same facts.

### The Problem

Consider a company that appears as:

| Platform | Name | Description | Founded |
|---|---|---|---|
| Website | Acme Corp | "AI-powered analytics platform" | 2019 |
| LinkedIn | Acme Corporation | "Leading data analytics company" | 2019 |
| Crunchbase | Acme Corp Inc. | "Business intelligence software" | 2018 |
| G2 | Acme | "Analytics and reporting tool" | — |
| Press article | ACME Corp | "Big data startup" | 2019 |

Five platforms, five different names, five different descriptions, and a conflicting founding date. When an LLM encounters this fragmented information during training or retrieval, it must reconcile contradictions. Often, it picks the wrong version — or hedges with vague language that doesn't serve you.

### The Solution

Define a canonical entity profile — a single source of truth for your name, description, and key attributes — and systematically propagate it across all platforms. In addition to structured data on your site, deploy discovery files such as `llms.txt` (v9.0+) and `ai-agents.json` at your domain root so that both retrieval-augmented LLMs and autonomous AI agents can find and understand your entity programmatically.

## Why It Matters for AI Visibility

1. **LLMs learn from aggregated sources.** If 3 out of 5 sources say your founding year is 2019 and 2 say 2018, the model may report 2019 — or may express uncertainty. Consistency removes doubt.

2. **Knowledge graphs power entity understanding.** Google's Knowledge Graph, Wikidata, and similar systems build entity profiles from multiple sources. Contradictions weaken your entity's representation. Wikidata is a critical layer: creating entities there (e.g., [Q138755507](https://www.wikidata.org/wiki/Q138755507), [Q138755989](https://www.wikidata.org/wiki/Q138755989)) anchors your identity in the open knowledge graph that feeds virtually every LLM and AI search engine.

3. **Retrieval systems match on entity identity.** When Perplexity or Bing Chat retrieves information about you, it looks for entity matches. Inconsistent names (Acme vs Acme Corp vs Acme Corporation) may result in fragmented retrieval or missed matches.

4. **Citation accuracy depends on source consistency.** If you want AI to accurately describe what you do, every source it might encounter must agree on what you do.

## The Playbook

The playbook is a five-step process. Work through it in order.

| Step | Title | Time Estimate | Focus |
|---|---|---|---|
| 01 | [Audit](playbook/01-audit.md) | 2-4 hours | Discover all existing entity representations |
| 02 | [Schema Markup](playbook/02-schema-markup.md) | 4-8 hours | Implement structured data on your site |
| 03 | [Knowledge Graphs](playbook/03-knowledge-graphs.md) | 2-6 hours | Establish presence in knowledge graph systems |
| 04 | [Cross-Platform Alignment](playbook/04-cross-platform-alignment.md) | 4-8 hours | Propagate canonical entity across all platforms |
| 05 | [Monitoring](playbook/05-monitoring.md) | 1 hour/month | Track entity consistency over time |

**Total initial effort:** 12-26 hours, depending on entity complexity and number of platforms.

## Templates

- [Entity Audit Template](templates/entity-audit-template.md) — spreadsheet-ready template for auditing entity representations
- [Schema Checklist](templates/schema-checklist.md) — implementation checklist for Schema.org markup

## Cheatsheets

- [JSON-LD Cheatsheet](cheatsheets/json-ld-cheatsheet.md) — copy-paste JSON-LD templates for common entity types

## Who This Is For

- **Marketing teams** responsible for brand presence across digital platforms
- **SEO/GEO practitioners** optimizing for both search engines and AI engines
- **Founders and executives** managing their personal or company brand
- **Agencies** managing entity consistency for multiple clients

## Citation

```
Caramaschi, A. (2026). Entity Consistency Playbook. GitHub. https://github.com/alexandrebrt14-sys/entity-consistency-playbook
```

See [CITATION.cff](CITATION.cff) for machine-readable citation.

## License

MIT License. See [LICENSE](LICENSE).

## Related Projects

- [GEO Checklist](https://github.com/alexandrebrt14-sys/geo-checklist) — The most comprehensive open checklist for AI visibility
- [GEO Taxonomy](https://github.com/alexandrebrt14-sys/geo-taxonomy) — Structured vocabulary of 60+ GEO terms and definitions
- [llms.txt Template Pack](https://github.com/alexandrebrt14-sys/llms-txt-templates) — Starter templates for AI-readable brand descriptions (now at v9.0 with 200+ URLs)
- [Brasil GEO](https://brasilgeo.ai) — Brazil's first consultancy specialized in Generative Engine Optimization
- [Alexandre Caramaschi](https://alexandrecaramaschi.com) — Full GEO methodology, consulting, and resources

---

**Author:** [Alexandre Caramaschi](https://alexandrecaramaschi.com) — CEO da Brasil GEO, ex-CMO da Semantix (Nasdaq), cofundador da AI Brasil.

**Platforms:** [Website](https://alexandrecaramaschi.com) | [Brasil GEO](https://brasilgeo.ai) | [LinkedIn](https://linkedin.com/in/alexandre-caramaschi/) | [Medium](https://medium.com/@alexandre.brt14) | [Substack](https://substack.com/@alexandrecaramaschi) | [DEV.to](https://dev.to/alexandrebrt14sys) | [GitHub](https://github.com/alexandrebrt14-sys)

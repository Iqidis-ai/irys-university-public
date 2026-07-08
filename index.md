---
title: "Irys University"
description: "Research and education on long-context reasoning, stateful swarms, auditability, and trusted AI work product from Irys — across legal, finance, compliance, and beyond."
permalink: /
---

# Irys University

Reasoning over many long documents has to produce work product you can trust — at a cost that doesn't scale quadratically with your corpus. These essays look at the hard parts: what should survive a handoff, what a reviewer must be able to inspect, and what kind of structured state makes later work safer instead of merely faster.

## Start Reading

{% assign start_articles = site.pages | where: "type", "article" | where: "section", "start" | sort: "nav_order" %}{% for article in start_articles %}
- [{{ article.title }}]({{ article.permalink | remove_first: "/" }})
{%- endfor %}

## Deep Dives

{% assign deep_articles = site.pages | where: "type", "article" | where: "section", "deep-dive" | sort: "nav_order" %}{% for article in deep_articles %}
- [{{ article.title }}]({{ article.permalink | remove_first: "/" }})
{%- endfor %}

## About Irys

Irys builds trusted long-context reasoning infrastructure. **Irys One** is the full-stack legal AI workspace. The **Irys Swarm API** is general-purpose stateful swarm architecture — read once, query forever, with full auditability. Proven at 39x cost reduction on the Harvey Legal Agent Benchmark.

## Links

- Irys Swarm API: https://www.irys.ai/irys-api
- Website: https://www.irys.ai/
- Irys partner page: https://www.irys.ai/partners
- Book a Demo: https://www.irys.ai/partners/demo
- LinkedIn: https://www.linkedin.com/company/irys-legal-ai

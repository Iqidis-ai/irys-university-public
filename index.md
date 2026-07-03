---
title: "Irys University"
description: "Research and education on legal AI, matter memory, auditability, legal work product, and AI-native legal workflows from Irys."
permalink: /
---

# Irys University

Legal AI has to become usable work product inside real matters. These essays look at the hard parts: what should survive a handoff, what a reviewer must be able to inspect, and what kind of matter record makes later work safer instead of merely faster.

## Start Reading

{% assign start_articles = site.pages | where: "type", "article" | where: "section", "start" | sort: "nav_order" %}{% for article in start_articles %}
- [{{ article.title }}]({{ article.permalink | remove_first: "/" }})
{%- endfor %}

## Deep Dives

{% assign deep_articles = site.pages | where: "type", "article" | where: "section", "deep-dive" | sort: "nav_order" %}{% for article in deep_articles %}
- [{{ article.title }}]({{ article.permalink | remove_first: "/" }})
{%- endfor %}

## About Irys

Irys is where we build against the same question: can AI carry legal work forward without forcing the team to reconstruct context every time?

## Links

- Website: https://www.irys.ai/
- Irys partner page: https://www.irys.ai/partners
- Book a Demo: https://www.irys.ai/partners/demo
- LinkedIn: https://www.linkedin.com/company/irys-legal-ai

# Irys University

The problem we care about is hard: reasoning over many long documents has to produce work product you can trust — at a cost that doesn't scale quadratically with your corpus. A clause can depend on a definition three documents away. A research answer can depend on a forum limitation. A financial analysis can depend on seven years of filings. A draft can depend on an instruction that never appears in the document itself.

This repository shares how we think about those problems from first principles: what should survive a handoff, what a reviewer must be able to inspect, and what kind of structured state makes later work safer instead of merely faster.

## What This Is

Start here if you care about the gap between an impressive AI answer and work product a team can rely on — in legal, finance, compliance, or any domain where you reason over long documents.

The essays here cover questions like:

- Why does long-context inference break down structurally, not just at scale?
- Why do AI systems fail when they treat memory as prompt text?
- Why is auditability an architecture decision, not a feature checkbox?
- What changes when knowledge work becomes stateful across extraction, analysis, and synthesis?
- Why does a corrected answer need to change the next output instead of dying inside one paragraph?
- Where does durable value sit when model fluency becomes common?

The goal is not to publish generic AI commentary. The goal is to explain the mechanisms that determine whether AI can be trusted beyond a demo — and how the Irys Swarm API solves them structurally.

## About Irys

Irys builds trusted long-context reasoning infrastructure. **Irys One** is the full-stack legal AI workspace where complex legal work gets done. The **Irys Swarm API** is general-purpose stateful swarm architecture — read a document set once, query the accumulated understanding cheaply forever, with full auditability. Proven at 39x cost reduction on the Harvey Legal Agent Benchmark and validated across legal, financial, and compliance domains.

## Start Reading

- [Why Prompt-As-Memory Fails](articles/why-prompt-as-memory-fails.html)
- [Auditability Is The Product](articles/auditability-is-the-product.html)
- [Prompt Instructions Are Not Control](articles/prompt-instructions-are-not-control.html)
- [The Exception Leak In Legal AI](articles/legal-ai-exception-leak.html)
- [A Citation Is Not An Audit Trail](articles/citations-are-not-audit-trails.html)
- [Matter Memory Must Preserve Contradictions](articles/matter-memory-preserve-contradictions.html)
- [Rerunning Is Not Repair In Legal AI](articles/rerunning-is-not-repair.html)

## Deep Dives

- [What AlphaEvolve Teaches Legal AI About Evaluated Work](articles/what-alphaevolve-teaches-legal-ai.html)
- [How to Train Graph Neural Networks — From First Principles to Planet Scale](articles/how-to-train-gnns.html)
- [GLM-5.2: When a Model is Designed for Systems Engineering](articles/glm-52-systems-engineering.html)
- [Active Inference & The Free Energy Principle — From First Principles to Working Systems](articles/active-inference-free-energy-principle.html)

## Links

- Irys Swarm API: https://www.irys.ai/irys-api
- Website: https://www.irys.ai/
- Irys partner page: https://www.irys.ai/partners
- Book a Demo: https://www.irys.ai/partners/demo
- LinkedIn: https://www.linkedin.com/company/irys-legal-ai

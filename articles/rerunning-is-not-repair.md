---
title: "Rerunning Is Not Repair In Legal AI"
description: "Why legal AI systems should fix the broken step in a source-backed workflow instead of regenerating whole answers from scratch."
keywords: "legal AI repair, AI auditability, legal work product, matter memory, source-backed AI, Irys"
image: /images/auditability-is-the-product.png
permalink: /articles/rerunning-is-not-repair.html
date: 2026-06-24
last_modified_at: 2026-06-24
type: article
---

# Rerunning Is Not Repair In Legal AI

When a legal AI answer is wrong, asking again is often the weakest possible fix.

The new answer may be better. It may be worse. It may cite the same source with different wording. It may hide the same failure behind a cleaner paragraph. What it usually does not do is tell the legal team what broke.

That matters because different failures need different repairs.

If retrieval missed the document, the system needs the source. If extraction missed the clause, the system needs the missing span. If linking failed, the system needs a relation between two existing objects. If synthesis flattened a conflict, the system needs to rerun the answer from corrected state.

Treating all of those failures as "ask the model again" wastes useful work and hides the operation that needs to change.

Consider a contract answer. The system finds the agreement, extracts the indemnity obligation, and cites the right section. The answer says the cap applies. But the same section contains a fraud carve-out that should block that conclusion.

The whole workflow is not wrong. Retrieval worked. Part of extraction worked. The source is real. The claim exists. The failure is narrower: the carve-out was not connected to the claim that drove the answer.

That should be a local repair.

The reviewer should be able to open the answer path, find the missing relation, connect the fraud carve-out to the cap claim, mark the claim blocked, and rerun only the affected synthesis step.

The source should not disappear. The quote should not be re-extracted from scratch. The review history should not reset. Correct work should stay correct while the broken relation gets fixed.

This is where auditability becomes operational.

An audit trail is a control surface for repair. It shows where the answer came from, what supports it, what contradicts it, which worker produced it, what confidence attached to it, and what changed after review.

In Irys, the answer should remain connected to the work that produced it. A challenged sentence can point to a claim. The claim can point to an extracted fact. The fact can point to a quote. The quote can point to a source. A missing contradiction edge can be repaired without throwing away the entire matter.

That makes review compound.

When a lawyer fixes a relation, the fix becomes part of the matter memory. A later client update can reuse the corrected state. A draft can avoid repeating the same mistake. A partner can see what was changed and why.

Regeneration alone cannot give the team that.

It produces another answer, but it does not preserve the repair.

Legal work does not tolerate that kind of amnesia. A corrected answer should change the next draft. A reviewed caveat should govern the next summary. A repaired source link should remain available when the matter returns a week later.

The goal is not to make the model try again until the paragraph sounds right.

The goal is to make the workflow more trustworthy after every review.

If one source is missing, add the source.

If one clause was missed, extract the clause.

If one relation is broken, fix the relation.

If one branch needs synthesis, rerun the branch.

That is repair.

Rerunning is only a guess unless the system can show what changed.

Learn more about Irys at [irys.ai](https://www.irys.ai/) or visit the [Irys partner page](https://www.irys.ai/partners).

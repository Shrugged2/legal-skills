---
name: source-verification
description: Check a legal document's citations, quotations, facts, figures, dates, record cites, and identifiers against the source record before it goes out. Use for "verify this," "check the cites," "fact-check this brief," "does the quote match," "do these numbers tie out," "check the TOA," or "make sure nothing is made up." Checks support only. It does not draft, argue, or fill gaps.
---

# Source Verification

Confirm that what a document asserts is supported by the record, and flag anything that is not. This skill never improves the writing, strengthens the argument, or supplies a missing fact. It checks.

## The rule

Every fact, figure, name, date, quotation, and citation must trace to a specific location in a source you inspected. If it cannot be traced, it is flagged. It is never assumed, filled in from memory, or silently passed.

## Three labels

Every checked item gets exactly one:

- **Verified:** traced to a source, with the location (reporter page, transcript page, exhibit number, ledger line). "Verified" without a location is not verified.
- **Contradicted:** the source says something different, or the asserted content is absent. State what the document says and what the source says. Highest severity.
- **Unverified:** the source is unavailable, ambiguous, or the item turns on judgment. State exactly what is needed to resolve it.

An Unverified item is never promoted to Verified by guessing. A confident answer with no source behind it is the failure this skill exists to prevent.

## Process rules

1. **Get the source first.** If the source is not supplied or reachable, do not verify from memory. List what is needed and stop on that item.
2. **Recompute, don't trust.** Recompute every total and derived figure from its line items. A formula range that silently drops a row is the classic hidden error.
3. **Read the source, don't recall it.** Never confirm from memory that a holding supports a proposition or that a quote is verbatim.
4. **Good law needs a citator.** Unless a citator or a later opinion is actually available to you, subsequent history is Unverified. Say so.
5. **Lead with failures.** Contradicted and Unverified items go first. Verified items go below. Nothing important hides under a list of passes.

## How to work

1. Inventory the element types in the document. A brief holds citations, quotations, and factual assertions. A demand letter holds figures, dates, and identifiers. Route by element, not by document name.
2. Run each applicable protocol in `references/element-protocols.md`. Suggested order: identifiers and dates (fast, catch embarrassing errors), then numbers, factual assertions, quotations, and citations last.
3. Assemble the output below.

Headline checks by element:

- **Citations:** the authority exists as cited; reporter and pincite are right; the holding supports the proposition (read it); subsequent history; short forms point to the right antecedent; body and table of authorities match in both directions.
- **Quotations:** verbatim; ellipses and brackets honest; pincite right; context does not reverse the meaning; correct speaker.
- **Numbers:** each figure ties to a source; totals recomputed; subtotals reconcile; no double counting; out-of-scope items excluded.
- **Factual assertions:** each factual sentence traces to the record; characterizations presented as facts are flagged; certainty matches the record.
- **Record cites:** page mappings come from actual page markers, not estimates; ranges are continuous and resolve correctly.
- **Dates and deadlines:** the trigger date is sourced; the rule is named; the computation is shown.
- **Identifiers:** captions, party names, cause numbers, bar numbers, and contact details match exactly.

## Output

- **Brief, petition, or letter:** a findings summary with Contradicted and Unverified items first, each with its source location. If editing a Word file, add a margin comment at each flagged item.
- **Spreadsheet:** a separate audit tab, one row per checked item, the source beside it, and the recomputed value beside the document's value. Do not overwrite original cells.
- **Anything else:** a findings memo in the same order.

End by stating what could not be verified and which source would close each gap. If everything checks out, say so, but only after checking.

For anything filed with a court or sent to opposing counsel, include a short audit trail: what was checked, against which source, with what result.

## Handoffs within this suite

- This skill finds problems. It does not fix them.
- A wrong citation that changes the argument: **where-the-argument-breaks** for the user's own draft, **legal-logic** for an opponent's.
- What a cited case actually holds: **case-briefing**.
- Run verification last, on the near-final document, and again after any fix.

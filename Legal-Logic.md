---
name: legal-logic
description: Audit the reasoning in a legal document, including an opposing brief, motion, declaration, expert report, or opinion. Use to trace specific claims through their stated and implied premises, test inductive support and rival explanations, and identify the strongest defensible challenge or concession.
---

# Legal Logic

Given a document, reconstruct what a party needs the reader to infer. Show where the evidence moves the argument forward, how far it carries, and which further step would change the legal outcome. Default to an opposing-position audit. Use the same standard when reviewing the user's own position.

## 1. Identify the claims and the decision

Work from the supplied document. If it is missing, ask for it or a passage. Identify the speaker, requested decision, controlling question, posture, burden, and the materials you could inspect. Treat unknown legal standards conditionally. Verify any governing law you independently introduce against primary sources.

For a specified passage, audit its material claims. For a whole document, inventory each distinct outcome-bearing claim by heading, page or paragraph; group restatements and preserve the separate grounds for relief. Prioritize contested and dispositive claims for full analysis. List the disposition of the others, including those that survive or remain untested. Disclose unreadable pages or scope limits. Never imply complete review of an excerpt.

## 2. Reconstruct before attacking

Quote the shortest passage that captures the claim accurately. Preserve qualifications such as “may,” “ordinarily,” or “as a matter of law.” Distinguish the author's argument from testimony, allegations, quoted opponents, and a court's actual findings. Give a verifiable locator. When pagination is unavailable, use a heading and distinctive opening words.

Write the chain as numbered propositions in plain English. For each step give its role, its basis, and what follows from it. Label premises as **stated**, **supplied elsewhere** (give locator), or **implied** (your reconstruction). Follow the chain from observation or authority through intermediate conclusions to the legal result. Spell out the bridge between steps wherever a reasonable reader could accept one and reject the next. Distinguish cumulative evidence, premises that must work together, and independent routes to the result. Use the strongest reading consistent with the text. If two readings produce different outcomes, explain both.

## 3. Test the particular inference

First ask whether the claimed step is deductive, inductive, interpretive, or an exercise of legal judgment. For a deduction, try to construct a case in which every premise holds but the conclusion fails. Test the truth or authority of the premises separately. For induction, assess how strongly the evidence favors this conclusion over a meaningful rival. A possible exception defeats a universal claim; it may do little to a qualified prediction.

| Move in the document | Practical test |
|---|---|
| Observation to explanation, intent, or knowledge | Identify the strongest rival grounded in the materials or ordinary experience. Would this observation be more expected under one account? What feature distinguishes them? Explain any direction of support. If the record gives no basis to compare, leave the strength unresolved. |
| Sample to population | Identify the sampled group, target group, period, denominator, selection method, and missing cases. Does the selection process favor the claimed result? State the narrowest group the evidence actually describes. |
| Sequence or association to causation | Test temporal order, alternative causes, changes in measurement or exposure, and any credible comparison. Identify what observation would distinguish the proposed cause from its closest competitor. |
| Statistic about a group to a particular event | Write the conditional in words. Check whether the draft has switched the conditioning event, omitted the relevant base rate, or changed the reference population. Calculate only from supplied or verified inputs; label assumptions. |
| Several observations to corroboration | Trace each item to its original source. Repeated accounts may show dissemination while adding little independent support for the event. Evaluate the remaining independent evidence together before judging the complete inference. |
| Silence to nonoccurrence | Ask who would have perceived, recorded, retained, and produced the event if it happened. Check the actual coverage and exceptions. Assess how expected silence would be on either account. |
| Earlier case to present result | Identify the earlier court's operative reason, material fact, procedural posture, and actual holding. Test whether the same relationship exists here. A distinction matters only if it changes the reason for the result. |
| Text, rule, or policy to remedy | Identify the textual or authoritative basis, the disputed interpretation, and the conditions for relief. Expose value judgments as such. Test rival readings against the same sources. Evidence about likely consequences alone cannot supply an unstated legal rule. |

Never assign invented probabilities or convert a burden of proof into a percentage. Separate four questions: Is the premise supported? Does the evidence favor the inference? How strongly does the whole record favor it? Is that enough for the decision this court may make? When a source is unavailable, distinguish an unverified premise from an inference that would fail even if the premise were true.

## 4. Report findings a lawyer can use

Lead with the strongest challenge that could affect the decision, or explain why the central inference survives. For each material contested claim give:

- **Claim and chain.** Quote and locate the claim. Show the numbered steps and their sources. Identify exactly where the objection attaches.
- **Test and result.** Explain why the step holds, supports only a narrower claim, lacks necessary support, conflicts with the supplied material, or remains unverifiable. Identify a rival or counterexample only where it does analytical work.
- **Best reply.** State how a capable opponent could defend the inference, including other portions of the document and cumulative support. Say whether that reply answers the objection.
- **Litigation consequence.** Apply the supplied posture and burden. Identify any independent route that survives. Give a short rebuttal the user could use, or recommend conceding the point. Specify what additional fact or authority would most change the assessment.

Keep facts, source gaps, and hypothetical tests visibly separate. Never invent an exhibit, concession, quotation, or authority. Do not fault an advocate for omitting an irrelevant premise, demand certainty of a probabilistic claim, or treat every alternative explanation as equally likely. Use a compact coverage table for a long document and a short chain for a single passage.

## Worked example

Fictional motion, § II: “Complaints doubled after the redesign. The redesign therefore doubled the risk of failure, which warrants suspension.” Exhibit A shows 10 complaints in the prior quarter and 20 in the next. Shipments increased from 100 to 200. Assume the stipulated suspension rule requires an increase in per-unit failure risk.

1. **Stated, Exhibit A.** Complaint count doubled. Concede this.
2. **Implied.** The count comparison measures a change in risk for an individual unit. This requires comparable exposure and a defensible link between complaints and failures.
3. **Stated, § II.** The redesign caused a twofold risk increase. Even a demonstrated change in failure rate would leave attribution to the redesign to be tested.
4. **Stated, § II.** Suspend under the supplied rule. This ground depends on step 3 or independent evidence of increased risk.

**Test.** Both quarters produced ten complaints per hundred units shipped. Higher volume explains the count change without any increase in that crude ratio. Shipments may be a poor measure of units actually in use, and complaints may include duplicates or refer to older units. The calculation undermines the offered comparison; it cannot establish that true failure risk stayed constant.

**Best reply and response.** Complaint counts could still justify investigation. That narrower claim survives. To support suspension on this record, connect verified failures to exposed units by design cohort over comparable observation periods.

**Usable rebuttal.** “The company shipped twice as many units and received twice as many complaints. Those totals tell us how many complaints arrived. They do not establish that any one unit became more likely to fail.”

## Quick calibration

Run the same reviewer on both variants without showing the expected result. Draft: “The inspector could reasonably infer the seal had opened.” In A the only observation is a warning light equally common with an open or closed seal under the stipulated operating conditions. In B the inspector also saw the seal hanging free. In A the light supplies no comparative support. In B the direct observation supplies an independent route. A reviewer that repeats the same attack on the ultimate inference in both versions has missed the independent evidence.

## Method sources

The comparative-evidence and base-rate questions draw on the Stanford Encyclopedia of Philosophy entries [Inductive Logic](https://plato.stanford.edu/archives/spr2025/entries/logic-inductive/) and [Legal Probabilism](https://plato.stanford.edu/archives/sum2024/entries/legal-probabilism/), especially the latter's discussion of likelihood ratios. The legal analogy test draws on Linda L. Berger and Kathryn M. Stanchi, *Legal Persuasion*, ch. 11, pp. 88–89. The prompts and examples are original applications. These sources explain methods of reasoning; governing law comes from the matter being analyzed.

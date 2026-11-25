---
name: legal-logic
description: Audit the reasoning in someone else's legal document, such as an opposing brief or motion, a declaration, an expert report, or a court's opinion. Use for "how do I attack this," "what's wrong with their argument," "does their expert's opinion follow," or "what should we concede." Traces each claim through its stated and implied premises, tests the inferences against rival explanations, and finds the strongest challenge or concession. For the user's own draft, use where-the-argument-breaks.
---

# Legal Logic

Given a document, reconstruct what its author needs the reader to infer. Show where the evidence moves the argument forward, how far it carries, and which further step would change the legal outcome. The default is an audit of the opposing position. If the user asks for this audit of their own draft, run it, but suggest where-the-argument-breaks, which is built for repair.

## 1. Identify the claims and the decision

Work from the supplied document. If it is missing, ask for it or a passage. Identify the speaker, the decision requested, the controlling question, the posture, the burden, and the materials you could inspect. Treat unknown legal standards conditionally. Do not introduce governing law you have not verified against a primary source; mark it Unverified and say what to check.

For a specified passage, audit its material claims. For a whole document, inventory each distinct outcome-bearing claim by heading, page, or paragraph. Group restatements and keep separate grounds for relief separate. Give full analysis to the three most contested or dispositive claims by default, and list the disposition of the rest in a coverage table, including claims that survive or remain untested. Disclose unreadable pages and scope limits. Never imply complete review of an excerpt.

## 2. Reconstruct before attacking

Quote the shortest passage that captures the claim accurately. Preserve qualifications such as "may," "ordinarily," or "as a matter of law." Distinguish the author's argument from testimony, allegations, quoted opponents, and a court's actual findings. Give a verifiable locator. When pagination is unavailable, use a heading and distinctive opening words.

Write the chain as numbered propositions in plain English. For each step give its role, its basis, and what follows from it. Label premises as **stated**, **supplied elsewhere** (give locator), or **implied** (your reconstruction). Follow the chain from observation or authority through intermediate conclusions to the legal result. Spell out the bridge wherever a reasonable reader could accept one step and reject the next. Distinguish cumulative evidence, premises that must work together, and independent routes to the result. If two readings produce different outcomes, explain both.

## 3. Test the particular inference

First ask whether the step is deductive, inductive, interpretive, or an exercise of legal judgment. For a deduction, try to construct a case in which every premise holds but the conclusion fails, and test the truth or authority of the premises separately. For induction, assess how strongly the evidence favors this conclusion over a meaningful rival. A possible exception defeats a universal claim. It may do little to a qualified prediction.

| Move in the document | Practical test |
|---|---|
| Observation to explanation, intent, or knowledge | Identify the strongest rival grounded in the materials or ordinary experience. Would this observation be more expected under one account? What feature distinguishes them? If the record gives no basis to compare, leave the strength unresolved. |
| Sample to population | Identify the sampled group, target group, period, denominator, selection method, and missing cases. Does the selection process favor the claimed result? State the narrowest group the evidence actually describes. |
| Sequence or association to causation | Test temporal order, alternative causes, changes in measurement or exposure, and any credible comparison. Identify what observation would distinguish the proposed cause from its closest competitor. |
| Statistic about a group to a particular event | Write the conditional in words. Check whether the draft has switched the conditioning event, omitted the base rate, or changed the reference population. Calculate only from supplied or verified inputs, and label assumptions. |
| Several observations to corroboration | Trace each item to its original source. Repeated accounts may show dissemination while adding little independent support. Evaluate the remaining independent evidence together. |
| Silence to nonoccurrence | Ask who would have perceived, recorded, retained, and produced the event if it happened. Check the actual coverage and exceptions. Assess how expected silence would be on either account. |
| Expert opinion to case-specific conclusion | Identify what the expert actually examined, the method, and whether the method was applied to these facts or only to the general category. Locate the gap between the data and the opinion, and name the examination that would have closed it. The governing reliability standard comes from the matter. |
| Term used across steps | Check whether a key term ("defect," "control," "notice," "custody") keeps one meaning throughout. If step 2 proves one sense and step 4 relies on another, the chain breaks at the shift. Quote both uses. |
| Earlier case to present result | Identify the earlier court's operative reason, material facts, posture, and actual holding. Test whether the same relationship exists here. A distinction matters only if it changes the reason for the result. |
| Text, rule, or policy to remedy | Identify the textual basis, the disputed interpretation, and the conditions for relief. Expose value judgments as such. Test rival readings against the same sources. Evidence about consequences cannot by itself supply an unstated legal rule. |

Never assign invented probabilities or convert a burden of proof into a percentage. Keep four questions separate:

1. Is the premise supported?
2. Does the evidence favor the inference?
3. How strongly does the whole record favor it?
4. Is that enough for the decision this court may make?

When a source is unavailable, distinguish an Unverified premise from an inference that would fail even if the premise were true.

## 4. Report findings a lawyer can use

Lead with the strongest challenge that could affect the decision, or explain why the central inference survives. For each claim given full analysis:

- **Claim and chain.** Quote and locate the claim. Show the numbered steps and their sources. Identify exactly where the objection attaches.
- **Test and result.** Say whether the step holds, supports only a narrower claim, lacks necessary support, conflicts with the record, or remains Unverified. Name a rival or counterexample only where it does analytical work.
- **Best reply.** State how a capable opponent would defend the inference, including other portions of the document and cumulative support. Say whether that reply answers the objection.
- **Litigation consequence.** Apply the posture and burden. Identify any independent route that survives. Give a short rebuttal the user could use, or recommend conceding the point. Name the fact or authority that would most change the assessment.

Keep facts, source gaps, and hypothetical tests visibly separate. Never invent an exhibit, concession, quotation, or authority. Do not fault an advocate for omitting an irrelevant premise, demand certainty of a probabilistic claim, or treat every alternative explanation as equally likely. If the opponent's central inference holds, say so plainly and recommend where to concede.

When the same conclusion has an independent route (for example, direct observation alongside a weak circumstantial inference), defeating one route does not defeat the conclusion. Address each route, or say which one survives.

## Worked example

Fictional motion, § II: "Complaints doubled after the redesign. The redesign therefore doubled the risk of failure, which warrants suspension." Exhibit A shows 10 complaints in the prior quarter and 20 in the next. Shipments rose from 100 to 200. Assume a stipulated suspension rule requires an increase in per-unit failure risk.

1. **Stated, Exhibit A.** The complaint count doubled. Concede this.
2. **Implied.** The count comparison measures a change in risk for an individual unit. This requires comparable exposure and a defensible link between complaints and failures.
3. **Stated, § II.** The redesign caused a twofold risk increase. Even a demonstrated change in failure rate would leave attribution to the redesign to be tested.
4. **Stated, § II.** Suspend under the rule. This depends on step 3 or independent evidence of increased risk.

**Test.** Both quarters produced ten complaints per hundred units shipped. Higher volume explains the count change without any increase in that crude ratio. Shipments may be a poor measure of units in use, and complaints may include duplicates or older units. The calculation undermines the offered comparison. It cannot establish that true failure risk stayed constant.

**Best reply and response.** Complaint counts could still justify an investigation. That narrower claim survives. To support suspension, the movant must connect verified failures to exposed units by design cohort over comparable periods.

**Usable rebuttal.** "The company shipped twice as many units and received twice as many complaints. Those totals tell us how many complaints arrived. They do not show that any one unit became more likely to fail."

## Handoffs within this suite

- Opinions the document cites: **case-briefing**, to establish what each actually held before testing the analogy.
- Exhibits, quotations, and record cites the argument rests on: **source-verification**.
- Turning a finding into a response the court will accept: **legal-persuasion-tactics**.

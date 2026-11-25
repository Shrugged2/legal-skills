# Legal Reasoning Skills for Claude

Seven skills that teach Claude to review litigation documents the way a careful lawyer does: find the weak step, choose the response, and check every authority before anything gets filed.

## Why this exists

The best-known story about AI in legal practice is a sanctions order. In *Mata v. Avianca, Inc.*, No. 22-cv-1461 (S.D.N.Y. June 22, 2023), lawyers filed a brief citing cases that did not exist. A language model will produce a confident citation as readily as a real one. It has no internal signal for the difference.

These skills are built around that problem. Every skill sorts anything that depends on a source into one of three labels: **Verified** (traced to a source that was actually inspected, with its location), **Contradicted** (the source says otherwise), or **Unverified** (nobody has checked yet, and here is what would settle it). Nothing moves from Unverified to Verified because it sounds right. The last two skills in the sequence exist only to produce a list a lawyer can check by hand.

The rest of the suite does the analysis. It reconstructs what an argument needs the reader to accept, finds the step a skeptical judge could refuse, and picks the persuasive move that answers it. None of that is worth much if the citations underneath are fiction, so the checking is built in from the start.

## The skills

| Skill | What it does | Use it when |
|---|---|---|
| **legal-review** | Runs the others in the right order. | "Review this brief before I file." "Help me respond to their motion." |
| **case-briefing** | Extracts the holding, reasoning, and usable quotes from an opinion you supply, or reconciles a line of cases. | "What does this case actually hold?" "Can I cite it for this?" |
| **legal-logic** | Audits the other side's reasoning: each claim, its hidden premises, and the rival explanations it ignores. | "How do I attack this?" "Does their expert's opinion follow from what he looked at?" |
| **where-the-argument-breaks** | Reads your own draft as a skeptical judge would and proposes the smallest repair that works. | "Where is this weak?" "What will the court push back on?" |
| **legal-persuasion-tactics** | Chooses and drafts the persuasive move for a court, panel, agency, or counterparty, and says what it costs. | "How do I handle this bad fact?" "How should I answer that question at argument?" |
| **authority-checklist** | Lists every authority the document cites, quotes, or names, with the exact proposition the document says it supports. | The last step before filing. |
| **source-verification** | Checks citations, quotations, facts, figures, and dates against the sources you provide. | "Check the cites." "Do these numbers tie out?" |

## How a review runs

Ask Claude to help you respond to an opposing motion, and **legal-review** runs this sequence:

1. **case-briefing** on the opinions the motion leans on hardest, so the analysis starts from what those cases actually held.
2. **legal-logic** on the motion itself. You get each material claim broken into numbered steps, the step where it is weakest, the opponent's best defense of that step, and a recommendation to attack or concede.
3. **legal-persuasion-tactics** to choose how the response should lead.
4. **where-the-argument-breaks** on your draft response.
5. **authority-checklist** and **source-verification** on the final text.

Each skill also works on its own. If you only need one case briefed, ask for that.

## What the checklist looks like

The authority checklist is the piece most lawyers will use first. For every citation instance it records the location, the signal, the proposition in the document's own words, the pincite, whether the document quotes the authority, and a blank column for the person checking. It also lists every statement of law that has no citation at all.

The proposition column records what the brief *claims*. The skill is barred from writing what it believes the case holds, even when it suspects the brief is wrong. A suspected problem goes in a separate Notes column marked as an observation to check. A checklist that quietly corrected the brief would be one more unverified source.

## What these skills will not do

They do not find law. They work on the documents and opinions you supply. Any statement about governing law that has not been checked against a primary source is marked Unverified.

They are not a citator. Without access to a citation service, subsequent history is always Unverified.

They do not replace reading the cases. A good case brief tells you what to look for when you open the opinion. It does not mean you can skip opening it.

They do not address jury persuasion. Openings and closings to a jury follow different rules, and the persuasion skill says so if asked.

Nothing here is legal advice. A lawyer who signs a filing is responsible for every word in it, including the words a machine suggested.

## Installing

Each folder under `skills/` is a self-contained skill with a `SKILL.md` file. To use them in Claude, add the folders as skills following Anthropic's [Agent Skills documentation](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview). Install all seven for the full workflow. The specialist skills work without **legal-review**, and **legal-review** works at reduced depth if a specialist is missing.

## Testing

The `evals/` folder holds matched pairs of test cases. Each pair changes one material fact. In one version the argument has a real defect. In the other it holds. A skill passes only if it catches the defect and leaves the sound version alone. The second half is the harder test. A reviewer that objects to everything is as useless as one that objects to nothing.

The skills never see these cases. Results, including failures, are recorded in `evals/README.md`.

## Design choices

**Separate jobs, separate skills.** Auditing an opponent's argument and repairing your own draft call for different stances. One looks for the break and the other fixes it. Splitting them keeps each skill's instructions short and its output focused.

**Restraint is tested as hard as detection.** Several instructions exist only to stop Claude from inventing objections: credit fair inferences, read adjacent sentences together, and accept the requested ruling when the record supports it.

**Sources stay out of the skill files.** The books and articles behind the methods are listed in [SOURCES.md](SOURCES.md). They matter to a human reader. They do nothing for the model, so they are not loaded with the skills.

**All examples are fictional.** Every fact pattern in the skills and tests was invented for this repository.

## Sources

See [SOURCES.md](SOURCES.md).

## About

I'm Rick, a law student at Baylor Law School. I use AI to become a better lawyer, and to do so responsibly. That currently seems to revolve around making the model show its work: every skill here assumes Claude can be wrong and makes it state explicitly the spots where that can result in big issues. Questions and criticism are welcome.

## License

MIT. Use however you see fit. Your use of these tools are your responsibility.

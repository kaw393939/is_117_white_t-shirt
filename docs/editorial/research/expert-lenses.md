# Expert lenses: questions grounded in the work

Owner: #102. Research pass, checked 2026-09-23. Intended consumers: proposed Chapters 3, 17 and 21, and Appendix B. This is a bounded set of inspected practitioner sources, not a survey of everything these authors believe.

## Source ledger

| ID | Source and precise locator | Status and permitted use |
| --- | --- | --- |
| EX-01 | Steve Krug, [Don’t Make Me Think, Revisited](https://sensible.com/dont-make-me-think/), edition block: New Riders, 2014, third edition; [author-hosted sample](https://sensible.com/downloads/DMMT-Revisited-sample-chapter.pdf), Chapter 4, printed p. 43 (PDF page 2) | Edition and actual passage inspected. Source for the distinction between click count and uncertainty at a choice; do not generalize to unlimited steps or delays. |
| EX-02 | Steve Krug, [website usability script](https://sensible.com/downloads/test-script-web.pdf), copyright 2010, pages 1–2, “The instructions” | Actual script inspected. Source for thinking aloud, evaluating the site and limiting facilitator help. Link through [Krug’s downloads page](https://sensible.com/download-files/), which requests links instead of reposting his files. |
| EX-03 | Donald E. Knuth, [Literate Programming](https://www-cs-faculty.stanford.edu/~knuth/lp.html), publication block and opening description; CSLI, 1992, ISBN 0-937073-80-6 | Author’s explanation inspected. Supports his emphasis on programs written for human understanding and combining documentation with code. The linked book’s full contents have not been reviewed. |
| EX-04 | Robert C. Martin, [The Single Responsibility Principle](https://blog.cleancoder.com/uncle-bob/2014/05/08/SingleReponsibilityPrinciple.html), May 8, 2014; paragraphs following the Employee example and closing formulation | Original essay inspected. Connects responsibility to business functions and sources of requested change. It is a practitioner argument, not evidence that one architecture always outperforms alternatives. |
| EX-05 | Steve Krug, [downloads page](https://sensible.com/download-files/), “Demo test video,” linking to [the demonstration](https://www.youtube.com/watch?v=1UCDUOB_aS8) | Link provenance verified from the author’s site. Video itself not watched in this pass: no asserted transcript, runtime, timestamps or particular observed behavior. Candidate for #67/#125. |

No book pages, scripts or video files are reproduced. Short paraphrases below distinguish source ideas from the book’s own applications. The experiment and prompt examples are original and fictional.

## Krug: what makes the choice difficult?

Krug’s sample chapter argues that the effort and uncertainty involved in each choice matter more than a rigid click limit, while acknowledging costs such as repeated paths and slow loading. His test script invites participants to explain their thinking while trying the site. [EX-01](https://sensible.com/downloads/DMMT-Revisited-sample-chapter.pdf), [EX-02](https://sensible.com/downloads/test-script-web.pdf).

**Our application:** compare a single crowded checkout with several clearly labeled steps. Ask someone to find the total and explain what the next action will do. Record hesitation and errors when an actual session occurs. Choosing the shorter route in advance would bypass the question the comparison is meant to answer.

**Question we can teach:** “What must the shopper infer here, and how could we make that choice clearer?”

**Limit:** this lens does not tell us which color expresses the brand or prove that a particular arrangement increases sales. Those require other criteria and evidence.

## Knuth: can another person understand the work?

Knuth’s own introduction to literate programming places human readers at the center of explaining a program, bringing documentation and program text together. [EX-03](https://www-cs-faculty.stanford.edu/~knuth/lp.html).

**Our application:** beside a generated shirt-page component, explain what it is responsible for, what its input means, and what must stay true during revision. Ask a collaborator to locate the decision governing the price display. Compare the explanation against what the code actually does.

**Question we can teach:** “Can the next person reconstruct the intention and check it against the implementation?”

**Limit:** an explanation can be clear and wrong. This lens does not replace tests, nor does applying it require beginners to adopt Knuth’s historical tools. Avoid presenting generic comments as a complete implementation of his methodology.

## Martin: who needs this to change, and what else might break?

Martin’s essay explains responsibility in relation to the people or business functions requesting change. Its concern is that a change serving one responsibility should not unexpectedly disturb another. [EX-04](https://blog.cleancoder.com/uncle-bob/2014/05/08/SingleReponsibilityPrinciple.html).

**Our application:** the brand’s art direction changes while the fictional product record stays fixed. Identify where presentation and product facts are defined. Ask whether changing headline styling could accidentally change an order total or duplicate an inconsistent price. For the static prototype, answer at the level of the actual files and templates; do not invent a complex service architecture.

**Question we can teach:** “What changes together, who requests that change, and what should remain unaffected?”

**Limit:** more files and abstractions do not automatically make the small shop better. Separation should answer a real change concern. A page being hard to maintain and a page being hard to shop are different problems.

## One fictional decision, three inspections

A generated checkout combines a large decorative slogan, price information and form controls. These are our proposed inspections, not a staged conversation among the three practitioners:

| Inspection | What to examine | Evidence to collect |
| --- | --- | --- |
| Shopper’s decision | Can someone locate the total and anticipate the next step? | Actual task observation or a labeled preliminary walkthrough |
| Collaborator’s understanding | Can another person trace the displayed total and explain the component? | The explanation compared with files and output |
| Change responsibility | Can the visual treatment change without altering the fictional order facts? | A scoped diff and an appropriate regression check |

These perspectives can expose different failures in one artifact. They are not evidence that the authors personally disagreed about this checkout. The eventual choice belongs to the project and should cite the observations that informed it.

## An original briefing example

> Review this fictional shirt checkout against three explicit criteria: shoppers can find the total and understand the next action; another developer can explain how the displayed information is produced; and a visual revision preserves the order facts. Identify specific evidence in the page and files, list unknowns, and propose one bounded change. Do not impersonate an expert or invent test results.

This briefing translates source-informed questions into inspectable criteria. It does not ask the model to pronounce what Krug, Knuth or Martin would endorse. When the output offers a rationale, compare it with the artifact and test the consequential claim.

## Integration notes

- Chapter 3 introduces the method of reading a source and deriving a question.
- Chapter 17 returns to the choice/observation lens once a wireframe exists.
- Chapter 21 shows which evidence human observation and automated tests can supply.
- Appendix B can condense these into reference cards while retaining the links and limits.
- Additional typographic or historical experts should enter through specific works and objects under #103/#39. A longer roster alone adds no instructional value.

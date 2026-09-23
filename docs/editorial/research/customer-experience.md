# Customer experience: the person outside the page

Owner: #104. Research pass checked 2026-09-23. Supports proposed Chapters 6, 16, 17 and 21, journey/funnel figure #114 and reference-shop observation #137. All shirt scenarios below are original inventions. No interviews, usability sessions or customer analytics have been collected for this dossier.

## Source ledger

| ID | Source and locator | What it supports; limits |
| --- | --- | --- |
| CX-01 | GOV.UK Service Manual, [Learning about users and their needs](https://www.gov.uk/service-manual/user-research/start-by-learning-user-needs), “Researching,” “Validating” and “Share your user needs” | First-party service-design guidance: research needs, identify assumptions and summarize groups by behavior and needs. Government-service practice, not research on our fictional store. |
| CX-02 | Carol S. Pearson, [The Pearson 12-Archetype System](https://carolspearson.com/about/the-pearson-12-archetype-system-human-development-and-evolution), “12 Archetypes, Many Names” | The theorist's account of contextual naming and applications. Supports treating the framework flexibly, not inferring a shopper's personality from a purchase. |
| CX-03 | Sarah Gibbons, NN/g, [Journey Mapping 101](https://www.nngroup.com/articles/journey-mapping-101/), “Definition,” “Actor,” “Scenario + Expectations” and “Actions, Mindsets, and Emotions” | Practitioner explanation: a goal-oriented process from an actor's viewpoint; scenarios may be anticipated. Not evidence for any particular journey in this book. |
| CX-04 | Google Analytics Help, [Funnel exploration](https://support.google.com/analytics/answer/9327974?hl=en), introduction and “Make open funnel” | Vendor documentation for configured sequential analysis, including entry rules. Not a universal model of how people shop. No analytics installation is required for the book's demonstration. |
| CX-05 | W3C WAI, [Accessibility, Usability, and Inclusion](https://www.w3.org/WAI/fundamentals/accessibility-usability-inclusion/), “Distinctions and Overlaps” | Standards organization's explanatory guidance: related concerns, with accessibility specifically addressing barriers affecting disabled people. Not a conformance test result. |
| CX-06 | Steve Krug, [website test script](https://sensible.com/downloads/test-script-web.pdf), pages 1–2, “The instructions”; [downloads page](https://sensible.com/download-files/) | Author's own method: evaluate the site, invite thinking aloud, avoid coaching the route and obtain recording permission. Link to his downloads rather than republishing the script. |

## Four different questions

The book needs personas and archetypes, journeys and funnels. They do different work:

| Lens | Working question | Shirt-store application | What it cannot establish |
| --- | --- | --- | --- |
| Persona | Whose goal, behavior and circumstances are we designing around? | Someone replacing a familiar basic needs enough information to compare fit. | That an invented biography represents real customers. |
| Brand archetype | What story pattern informs this brand's expression? | Standard Issue's Everyperson direction informs its voice. | That everyone buying it has one personality type. |
| Customer journey | What happens as someone pursues a goal across encounters and time? | Discovery, comparison, purchase, wearing and possibly seeking help. | That the imagined sequence or emotions have been observed. |
| Funnel | How many measured entities satisfy defined stages? | Product view, cart addition, checkout and simulated completion. | Why someone left or how they felt. |

The persona distinction follows CX-01; the brand application uses CX-02 and our [fictional product record](../product-record.md). The journey and funnel distinction is our synthesis of CX-03 and CX-04, not a claim that those authors jointly proposed this table.

## A useful persona starts with a consequential uncertainty

GOV.UK recommends grounding needs in research and treating unsupported suggestions as assumptions [CX-01]. For the book, a provisional persona is a hypothesis to investigate, not a decorative portrait made credible by a name, age and stock photograph.

**Invented provisional persona: the replacement shopper.** They want another white shirt that fits as expected. We hypothesize that garment measurements, care information and a clear returns explanation matter to that decision. We do not know how often this need occurs, which information they consult first, or whether price outweighs fit uncertainty. We have no demographic evidence and add none.

The design implication is provisional: make those answers findable. Research would examine actual comparison behavior and ask what the person still needs to decide. If observations contradict the hypothesis, revise the persona rather than explaining the evidence away. An AI-generated interview transcript cannot validate it.

A second hypothetical situation—a gift buyer uncertain about another person's size—can reveal different questions without requiring a second invented life story. Neither situation predicts attraction to the Explorer or Jester brand. The brand's chosen voice and the shopper's practical needs are separate design inputs.

## One possible journey, including the inconvenient parts

Gibbons describes journeys around an actor and a scenario, with actions and thoughts across phases [CX-03]. Our example is deliberately an anticipated journey. Its questions are editorial hypotheses, not participant quotations. Do not draw an emotional curve as though feelings were measured.

| Possible encounter | Hypothesized question | Store response to prototype | Evidence still needed |
| --- | --- | --- | --- |
| Sees a shared image | What is this, and is it for me? | Consistent brand identification and an honest destination | What actual viewers understand |
| Opens the product page | Is this the shirt I need? | Fixed product facts, useful image and fit information | How shoppers compare alternatives |
| Leaves and returns later | Where was the information I wanted? | Stable navigation and recognizable product naming | Whether returning is common and what prompts it |
| Reviews the order | What will I pay, and what happens next? | Explicit example costs, delivery terms and edit controls | Whether people can explain the total and commitment |
| Receives and wears it | Does it match the promise? | Only a labeled story panel in the static prototype | Real fulfillment and product experience, unavailable here |
| Seeks help or a return | Can I resolve the problem? | Findable sample support and return-policy pages | Actual support behavior and outcomes |

Any new size chart, delivery charge or policy is an additional fictional fixture requiring its own label; it is not an established fact in the $28 product record. The prototype can show these interfaces without claiming to operate a business.

## A funnel counts a definition, not a mind

Google's documentation distinguishes an open funnel, allowing entry at any step, from a closed funnel, requiring entry at the first step; subsequent counting depends on the specified sequence [CX-04]. This matters before anyone celebrates a conversion percentage.

**Original synthetic arithmetic example:** within one invented measurement period, 100 distinct demo visitors view the product; of those, 40 add it to a cart; of those, 20 start checkout; of those, 10 reach simulated completion in that order. This is a closed, user-based funnel with four explicitly defined stages, not live GA4 output. Step continuation is 40%, 50% and 50%; overall completion is 10%. Each percentage needs its denominator. Do not label the final stage revenue or a real purchase.

Now ask what the chart omits. Leaving to consult a friend, discovering the shirt is unsuitable, encountering a broken control and postponing a purchase can all produce non-completion in this invented analysis. The counts alone cannot choose among those explanations. The journey suggests questions for observation; the funnel identifies a measured transition worth investigating. Neither replaces the other.

For #114, place this synthetic funnel beside the anticipated journey, not over it. Label the count unit, period, entry rule and fictional status next to the numbers. Use text labels as well as shape or color. For #135, define events and exclusions before generating any demonstration logs; keep automated test traffic separate from customer evidence.

## Usability and accessibility belong together, but are not synonyms

WAI distinguishes usability's concern with effective, efficient and satisfying use from accessibility's focus on disabled people's participation and barriers, while emphasizing overlap [CX-05]. Our practical implication: a successful session with one person cannot establish access for everyone, and a passing automated check cannot establish that someone understands the checkout.

Test an actual rendered prototype, not merely its explanation. Combine relevant technical checks with observation involving people with appropriate access needs when available. If participants are unavailable, label the work a preliminary walkthrough and keep the user-research question open. Do not impersonate disability through an AI persona and call the output lived experience.

## Questions for the reference-shop session

Krug's script models thinking aloud and a facilitator who does not supply the route [CX-06]. The tasks below are our original draft, not his wording. Run them only when the corresponding prototype states exist; show that no purchase or shipment will occur, provide dummy data, and never request a real address or payment credential.

| Original task prompt | Question investigated | What to record, without inventing results |
| --- | --- | --- |
| Decide whether this shirt would meet your needs. Show what you would check. | Can someone find relevant product information and identify missing evidence? | Route, information consulted, unanswered questions and assistance |
| Prepare an example order, then tell me what you expect to pay and receive. | Are quantity, costs and delivery assumptions understood? | Their explanation compared with the displayed fictional fixture |
| Change your mind about the quantity before completing the example. | Can someone recover and verify the revised order? | Actions, errors, revised total and whether help was needed |
| Continue using the supplied dummy details; explain what happens when something needs correction. | Are error messages findable and recovery instructions understandable? | Actual error state, focus behavior, interpretation and recovery |
| Complete the demonstration and explain what you think happened. | Does confirmation communicate simulation and next steps clearly? | Interpretation; distinguish a clicked button from understanding |
| Find out how you would get help if the shirt did not fit. | Does the presence serve people after conversion? | Support route and understanding of the labeled example policy |

Before a real session, explain participation, observers and data handling; obtain specific consent for recording and separate permission for any public quotation. Record only necessary information. A decision not to buy can be a valid shopper outcome, not a participant failure.

The observation record should identify prototype revision, task, device/access setup, factual observation, any verbatim words captured with permission, interpretation, proposed change and retest status. Keep these fields separate. An empty findings section is more truthful than a plausible invented success story.

## Editorial handoff

- Chapters 6, 16 and 17 receive the distinctions and examples; Chapter 21 connects observation to technical checks.
- #114 owns the finished journey/funnel comparison, not copied NN/g templates or screenshots.
- #128–133 own the actual store states and labeled fictional policies needed for these tasks.
- #137 owns recruitment, consent, observation or an explicitly labeled walkthrough. This dossier has conducted none of them.
- #56/#138 own implementation accessibility review; #108/#135 own fuller metric definitions and demonstration measurement.
- #67/#125 can use the Krug video candidate already recorded in [expert lenses](expert-lenses.md). Video content and timestamps still require viewing; a verified source link is not a completed video review.

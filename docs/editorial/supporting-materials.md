# Supporting materials: first-layer specification

## Appendices

| ID | Deliverable | Required content |
| --- | --- | --- |
| A | Working glossary | Plain definition; shirt/shop example; contrasting term; source where appropriate; chapter anchors. |
| B | Experts and their questions | Documented principle with exact source; context and limits; separately labeled application; competing perspective. |
| C | Visual reference atlas | Type, color, grids, hierarchy, imagery and garment placement; original comparisons beside attributed historical records. |
| D | Briefing and revision patterns | Intent, context, fixed facts, changes, examples, output expectations, evaluation; annotated failures and preservation prompts. |
| E | Brand and business dossier | Client brief, persona assumptions, product record, brand direction, journey, funnel, content inventory and decision log. |
| F | Web technology field guide | Request-to-render map, HTML/CSS essentials, browser tools, hosting, Git, optional behavior and production boundaries. |
| G | Testing field notes | Usability script, keyboard checks, test scenarios, issue report, explained end-to-end example; unit/integration context. |
| H | Marketing and store arithmetic | Metric definition and denominator, worked fictional inputs, margins and acquisition costs, attribution limits. |
| I | Read, watch, inspect | Small annotated selections, provenance and availability; Wikipedia orientation, source documents, museum objects and optional videos. |
| J | Credits and provenance | Claim sources, image/video rights, generated-asset disclosure, author recollections, corrections and update policy. |

Appendices are reference aids, not grading instruments. Essential explanations must remain readable without buying or watching external materials.

## Index and linking

Maintain an alphabetical subject/name/work index distinct from the glossary. Entries point to explanations, examples and counterexamples, with see/see-also relationships. Add a list of figures for visual retrieval. Give glossary terms stable anchors and explain them in context at first use. Link claim-level sources beside the claim; use small optional read/inspect/watch groups rather than excessive link density. Check backlinks and old paths during migration.

## Source register fields

Source ID; chapter/claim; exact claim supported; creator/title/date/edition; locator or artifact ID; stable URL; primary/secondary/company account/personal recollection; checked date; quotation text and locator if used; rights/reuse limits; unresolved questions. Source status: candidate, inspected, supports claim, needs corroboration, or rejected. These are production states, not guarantees of truth.

## Story register fields

Story ID; documented/personal/invented; protagonist; situation; decision; consequence; teaching purpose; shirt application; intended recurrence; sources; uncertainty. Real cases must distinguish a source author’s interpretation from a brand’s statements and independent facts. Ask the author for personal stories; leave an explicit request if unavailable.

Initial research candidates: Starbucks and selected brands actually documented in The Hero and the Outlaw; Helvetica interview perspectives; networking stories in Where Wizards Stay Up Late; practitioner disagreements involving usability and software craftsmanship. Verify editions, scenes and claims before selection. Middle Men is an optional media-literacy lead, not proof of an ecommerce origin claim.

## Figure and media register fields

Asset ID; chapter; concept; source or original/generated status; brief; fixed variables; changing variables; caption; alt text or longer equivalent; rights holder/license; source record; provenance; file path; mobile/print requirements; status. Prioritize approximately one essential comparison per chapter, reusing assets when appropriate instead of decorating every section.

Essential new families: garment placements; typography controls; color roles and contrast; grid/proportion alternatives; persona versus archetype; journey versus funnel; circuit versus packet switching; request to rendering; ecommerce/search timeline; campaign-to-destination continuity; annotated analytics; test failure/fix. Existing issues #59–#65 and #68 own overlapping illustrations and should be reused.

## Reference shop specification

Use Standard Issue as the initial complete reference shop, retaining the other brands as deliberate contrasts. All products, people, prices and orders are fictional. Preserve the three existing mockup URLs. Implement new pages within docs/examples/reference-shop/ using the existing small publishing stack; choose final file names in the implementation issue.

Required pages/states: home; collection; product detail; size/variant guidance; populated and empty cart; contact/shipping; delivery choice; simulated payment; review; confirmation; representative validation failure and recovery; about; help/contact; shipping/returns; care. Maintain consistent fictional product and order facts throughout.

Use real links for the static journey and native semantic controls where appropriate. Predetermined pages illustrate state rather than pretending to store it. Do not collect payment credentials or submit personal details. Explain which controls are illustrative; provide a deterministic route for automated tests. Optional JavaScript for local state is a separate extension, not a prerequisite.

The business package includes the brief, persona, brand guide, journey/funnel, campaign example, event/measurement plan and transparent fictional economics. No live tracking, ad spend, payments or backend deployment is required.

## Verification materials

Test the complete happy path, empty cart, an error/recovery path, navigation and total consistency. Include keyboard and small-screen review, automated accessibility checks with stated limits, and an actual human usability observation when available. If observations are unavailable, report a scripted demonstration, not invented participants or results. Unit tests are appropriate only when meaningful logic exists; integration tests concern actual component/data boundaries. External link outages should be reported separately from deterministic local build failures.

## Publication package

The first finished sample should connect a garment choice, a verified historical reference, an AI revision and an observable consequence. Use it to calibrate prose, figure density, citation style and technical depth before mass expansion. Later release work includes copyediting, a continuity check, specialist review, accessible rendered proof, credits, navigation, change notes and live-site verification.

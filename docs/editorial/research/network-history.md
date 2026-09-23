# Network history: how the message gets there

Owner: #105. Research pass checked 2026-09-23. Supports proposed Chapter 18, diagrams #115 and timeline #116. This is a bounded historical and technical dossier, not a complete Internet history. The shirt examples are original fictional demonstrations, not historical events or measurements of the site.

## Source ledger

| ID | Source and locator | Evidence and limits |
| --- | --- | --- |
| NH-01 | Claude E. Shannon, [A Mathematical Theory of Communication](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf), corrected reprint of the 1948 Bell System Technical Journal paper, Introduction, PDF pages 1–2 | Original research text inspected for communication, meaning, bits and the system diagram. Not a claim to have reviewed every proof. |
| NH-02 | Paul Baran, [On Distributed Communications, I](https://www.rand.org/pubs/research_memoranda/RM3420.html), 1964, RM-3420-PR; online text, “Diversity of Assignment” and “On a Future System Development” | Original report text hosted by RAND: paths, redundancy and survivability under stated models. Do not transfer its numerical simulation results to today's store. |
| NH-03 | Paul Baran and Sharla P. Boehm, [On Distributed Communications, II](https://www.rand.org/pubs/research_memoranda/RM3103.html), 1964, RM-3103-PR; author fields and abstract | Institutional record of original research on routing simulation. Metadata and abstract inspected, not the complete report. Supports crediting both authors; does not establish who performed each specific task. |
| NH-04 | NPL, [Donald Davies](https://www.npl.co.uk/about-us/history/famous/donald-davies), packet-switching paragraphs and linked resources; [institutional timeline](https://www.npl.co.uk/about-us/history/timeline), 1965 | Institutional retrospective, not Davies's original proposal. Supports NPL's account of Davies and his team. Its video link is a candidate, not a watched source. |
| NH-05 | Barry M. Leiner and colleagues, [A Brief History of the Internet](https://www.internetsociety.org/internet/history-internet/brief-history-internet/), “Origins,” “Initial Internetting Concepts” and transition discussion | Participant-authored retrospective. Valuable testimony, not an exhaustive or neutral adjudication of every priority claim. |
| NH-06 | Vinton Cerf, Yogen Dalal and Carl Sunshine, [RFC 675](https://www.rfc-editor.org/rfc/rfc675.html), December 1974, title and author block | Contemporary protocol document. Records collaborators and historical terminology; not today's TCP specification. |
| NH-07 | Jon Postel, [RFC 801: NCP/TCP Transition Plan](https://www.rfc-editor.org/rfc/rfc801.html), November 1981, Introduction and schedule | Contemporary plan for the January 1, 1983 transition. A plan alone does not prove execution; pair with NH-05's retrospective. |
| NH-08 | [RFC 791](https://www.rfc-editor.org/rfc/rfc791.html), September 1981, §§1.1–1.4; [RFC 9293](https://www.rfc-editor.org/rfc/rfc9293.html), §2.2 and §3.7 | Original technical specifications. RFC 791 describes IPv4; RFC 9293 supplies the modern TCP account. Distinguish IP delivery from transport behavior and application outcomes. |
| NH-09 | Katie Hafner, [author website](https://katiehafner.com/), “Books by Katie Hafner” | Author confirms *Where Wizards Stay Up Late: The Origins of the Internet*, with Matthew Lyon, Simon & Schuster, 1996. Metadata checked; book passages and page references remain unreviewed. |

## Start with two meanings of “message”

Shannon's introduction distinguishes the engineering problem of reproducing a selected message from its semantic meaning. It also credits earlier work by Nyquist and Hartley, and the short name *bit* to J. W. Tukey [NH-01]. Even the beginning of this story contains collaborators and predecessors.

**Our teaching connection:** the bytes of a shirt slogan might arrive intact while the shopper misunderstands the slogan. Successful communication engineering does not establish persuasive, truthful or understandable copy. Place the same sentence beside two questions: “Did the data arrive?” and “What did the person understand?” This returns the technology chapter to the book's concern with language and judgment without confusing Shannon's technical quantity with cultural significance.

## Circuit and packet switching: what is being shared?

For the introductory model, a circuit-switched connection reserves communication capacity along a path for the connection; this need not mean a separate physical wire for each conversation. Packet switching divides transmitted data into units that can share links with other traffic. Neither term alone tells us the whole routing, reliability or security design. These simplified models connect the historical discussion in NH-02/NH-05 to the IP and TCP specifications in NH-08.

**Original fictional demonstration:** two shoppers request shirt information. In a circuit model, shade the capacity reserved for each connection, including quiet periods. In a packet model, interleave labeled units from both requests on a shared link. Then introduce a queue and drop one unit. Explain the model's chosen assumptions; do not claim packet switching is always faster or that each packet necessarily takes a different route.

Vocabulary enters as a practical need: a *link* connects network points; a *packet* is a transmitted data unit; *routing* selects paths; a *queue* represents waiting work. The figures should make the distinction visible rather than substitute a road metaphor for the mechanism.

## Chronology without a lone hero

| Episode | Checked historical statement | Original connection to the shop |
| --- | --- | --- |
| 1948 | Shannon's paper develops a mathematical communication theory [NH-01]. | Separate accurate transmission from whether a product description makes sense. |
| 1964 | Baran's report examines distributed communication; the companion simulation report credits Baran and Boehm [NH-02/NH-03]. | Ask which failures a network model can tolerate, and under what assumptions. |
| 1965 | NPL dates Davies and his team's packet-switching development to this year [NH-04]. | A burst of product data need not occupy capacity like a continuous conversation. |
| 1967–1969 | The participant history describes Scantlebury sharing NPL/RAND work with Roberts, BBN's IMP team led by Frank Heart, and the first UCLA installation in September 1969 [NH-05]. | Working connections require proposals, equipment, integration and measurement—not just an idea. |
| 1970s | The same account describes Kahn and Cerf's internetworking work; RFC 675 names Cerf, Dalal and Sunshine in 1974 [NH-05/NH-06]. | The shopper and store need not belong to one internally identical network. |
| 1981–1983 | Postel's 1981 transition plan targets January 1, 1983; the participant history reports the NCP-to-TCP/IP transition [NH-07/NH-05]. | A shared protocol also requires coordinated adoption and migration. |

Keep Baran's survivability research distinct from a blanket assertion that the Internet was invented solely to survive nuclear war. Keep ARPANET, internetworking and the later Web distinct. This selection is a teaching route, not a claim that omitted contributors were unimportant. Avoid disputed “first inventor” rankings without a separate evidence review.

## Reliability is a responsibility, not magic

RFC 791 explicitly excludes end-to-end reliability, sequencing and flow control from IP's scope. RFC 9293 describes TCP's ordered byte-stream service, loss/error detection and retransmission; application writes need not correspond one-for-one to segments [NH-08].

**Our application:** in a simplified TCP-based shop exchange, show the requested data passing through networks and transport recovery when a unit is lost. Delivery can still fail if connectivity cannot be restored. A TCP acknowledgment is not proof that the shop accepted an order, charged correctly or shipped anything. Those are different questions at the application and business levels.

Do not teach that every Web exchange uses TCP. Chapter 19's protocol research (#106) should explain the selected modern HTTP transport and security context. This historical lesson intentionally omits those details rather than drawing an allegedly universal stack. In the actual book prototype, checkout remains simulated; network illustrations must not suggest live payments or fulfillment.

## Pair the narrative book with inspectable evidence

*Where Wizards Stay Up Late* remains the narrative companion the author already uses. Its publication details are verified through Hafner's account [NH-09]. Do not assign a scene, quotation or page number without reading the selected edition.

For the next editorial pass, pair a selected book episode with one document and one question:

- Distributed-network research: RAND's report and the question “What assumptions make this result possible?”
- Protocol collaboration: RFC 675's author block and the question “Who disappears when this becomes a one-person invention story?”
- Migration: RFC 801 and the question “What had to change for a shared standard to become operational?”

These are proposed reading pairings, not verified summaries of particular book passages. The chapter can stand on the checked sources above while passage selection remains with #125/#141. The NPL-linked video similarly needs viewing, transcript/caption checks and timestamps under #67/#125 before quotation or recommendation of an excerpt.

## Diagram handoff and safeguards

#115 should create original schematics, with text equivalents and non-color identifiers:

1. A circuit/packet comparison using the same two fictional requests and an explicit capacity assumption. Reserved capacity is not a dedicated physical wire; interleaving is not guaranteed speed.
2. A small network with a failed link and an available alternative. Label it a hypothetical topology, not an ARPANET map. Include a disconnected case so redundancy is not portrayed as invulnerability.
3. A TCP-based example distinguishing sending, routing, transport recovery and the application response. Label omissions; packet labels are teaching identifiers, not a claimed literal packet capture.

Source the technical captions to NH-02/NH-08 and have them reviewed before integration. Do not trace RAND figures or historical maps: RAND's record states reuse conditions, and no reproduction permission has been obtained. #116 can use the checked chronology but must retain the distinction between a proposal, implementation, specification and adoption date.

Remaining limits are explicit: no full RAND volume-II review, selected *Wizards* passage review, audiovisual review, packet capture, finished diagrams or live network experiment occurred here. Primary Web-history documents and Tim Berners-Lee belong to #106, not an unsupported epilogue added to this dossier.

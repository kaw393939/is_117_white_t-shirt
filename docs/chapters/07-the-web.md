---
title: "From a story to a screen"
order: 7
---
# From a story to a screen

A poster can ask you to look. A web page can ask you to *do* — and that changes everything about the design problem. The poster's job ends at attention. The page's job continues: orient, inform, build trust, offer a next step, and stay readable to every person and machine that arrives.

Everything from the earlier chapters now has a place to live. The persuasion, the archetype, the visual language, the brand rules — on the web they become specific, nameable parts of a page.

## The anatomy of a product page

Learn these names and you can discuss any storefront:

- **Hero** — the prominent opening area. It answers, in seconds: what is this, who is it for, why should I stay? A hero is the brand guide's promise made visible.
- **Navigation** — the map of where else the visitor could go. Good navigation is a trust signal: it says there is a whole considered world here.
- **Call to action** — the invitation to a next step. One page, one primary action. The brand guide should already have reserved a color for exactly this.
- **Product details** — where product *fact* lives: fiber, fit, care, origin. Chapter 1's discipline returns: this area must stay true even when the story soars.
- **Social proof and reassurance** — reviews, guarantees, return policies. Persuasion levers from chapter 2, placed where hesitation happens.
- **FAQ** — the objections section, written as questions the audience actually asks.
- **Footer** — the fine print that proves the brand is real: contact, policies, the unglamorous links that carry legal and ethical weight.

## Three materials

The web page is built from three materials, and each has one job:

- **HTML carries meaning.** A heading is marked as a heading because it *is* one — for readers, for screen readers, for search engines, for AI systems. This is **semantic HTML**: markup chosen for the meaning and role of the content.
- **CSS carries presentation.** Color, type, spacing, layout — the brand guide rendered as code. A **selector** is how CSS finds an element; the **box model** — content, padding, border, margin — is how the browser measures the space each element takes.
- **JavaScript carries behavior.** What responds: menus that open, images that zoom, carts that update.

Keep the jobs separate and the work stays changeable. Mix them — meaning smeared into presentation, behavior tangled into structure — and every revision costs more than it should.

## Clear to everyone who reads

A web page has more readers than the ones with eyes on a screen:

- **People** with varying vision, motor control, attention, and bandwidth. The [W3C's page structure tutorial](https://www.w3.org/WAI/tutorials/page-structure/) shows what structure gives them.
- **Assistive technology** — screen readers that navigate by headings and landmarks, which exist only if the HTML is semantic.
- **Search engines** — which read structure and text, not vibes.
- **AI systems** — which increasingly summarize, quote, and answer from pages. [Google's own guidance](https://developers.google.com/search/docs/appearance/ai-features) explains how its features use site content; read it as one company's documentation of its own systems, not a promise about all AI.

The through-line: **meaningful structure is the accessibility strategy, the search strategy, and the AI strategy at once.** Write real headings. Label real things. The [MDN semantic HTML curriculum](https://developer.mozilla.org/en-US/curriculum/core/semantic-html/) is the place to practice.

## The storefront as a final exam

Build a one-product storefront for our shirt and every chapter reports for duty. The hero expresses the archetype. The copy persuades without pressuring. The palette obeys the brand guide's tokens. The HTML is semantic, the CSS carries the visual language, and a partner can review the whole thing in a pull request — because a storefront, like this book, is something a team can build.

See it working: the [Standard Issue storefront mockup](../examples/storefront.md) is a complete, invented one-product page. Find each element from the anatomy above — the hero, the facts, the reassurance, the FAQ, the footer — and notice what the copy does *not* do: no timers, no pressure, no invented reviews.

**A question to carry out of the book:** the shirt was never the subject. Pick your own ordinary object. What story will you teach it to tell?

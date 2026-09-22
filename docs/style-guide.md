---
title: Style guide
order: 10
---
# The book's style, made visible

This page is a **living style guide**: the design decisions behind this book, shown working rather than merely described. It exists so a partner — human or AI — can see the system, discuss it, and build with it. The rules come from [Chapter 6](chapters/06-brand-guide.md); the page vocabulary from [Chapter 7](chapters/07-the-web.md).

## Design tokens

The book's repeated style decisions, as named values. These are the actual custom properties defined at the top of [book.css](assets/book.css).

| Token | Value | Role |
| --- | --- | --- |
| `--ink` | `#17202a` | Text and headings |
| `--paper` | `#ffffff` | Page background |
| `--accent` | `#b52b16` | Links, actions, the masthead rule — reserved for things that act |
| `--line` | `#d8dce0` | Borders and quiet structure |

The accent rule matters: red means *you can do something here*. Body text never uses it.

## Typography

Two voices, one job each. Georgia carries the large, reflective moments; the system sans carries the working text.

<h1 style="margin-top:0">The shirt stays. The story changes. (H1, Georgia)</h1>
<h2>A section heading (H2, system sans)</h2>
<h3>A sub-heading (H3, system sans)</h3>

Body copy runs at 1.0625rem with a 1.75 line height and a 48rem measure — sized for long-form reading, not skimming. Lists, like this one, keep a half-rem of air between items:

- Hierarchy signals importance before content does.
- Line length is a reading-comfort decision, not an accident.
- `code` gets a quiet gray chip, because code should look handled, not shouted.

## Components

**Links** are the only red text: [a link to the vocabulary page](vocabulary.md), with an offset underline and a thick hover state.

**Blockquotes** carry prompts, citations, and invented examples — set off with the accent rule and a gray ground:

> Write a 60-word product description for a plain white cotton T-shirt. Invite a feeling of relief from too many choices. No exclamation points, no superlatives. Do not invent product facts.

**Tables** present comparisons — like the token table above — with header rows on the gray ground and generous padding.

**Buttons and calls to action** do not yet exist as a component. When the book needs one, it should be a single red-action element per view, per the token rule above.

## Voice, in one paragraph

Curious, concrete, playful, intelligent. Sentences do real work. Scenes open chapters; questions close them. Invented brands are labeled invented. No urgency tricks, no superlatives without evidence, no invented quotations — ever.

## How to use this page

Proposing a design change? Quote the token or component in the issue or pull request ("change `--accent` to…", "the blockquote style should…"). The guide gives partners a shared vocabulary — which is the whole point of Chapter 6.

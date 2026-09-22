# The Plain White T-Shirt

A book about persuasion, identity, visual language, and sculpting with AI.

**[Read the book](https://kaw393939.github.io/is_117_white_t-shirt/)** · [Open the Markdown](docs/index.md)

## What is here

This is the basic skeleton of a book, ready to develop chapter by chapter. It contains a short opening, seven chapter outlines, a vocabulary page, and a source shelf. It is not a finished manuscript.

The framework: **persuasion shapes the response; archetypes shape the meaning; visual language shapes the expression; deliberate prompting shapes the result.** The recurring subject is the same plain white T-shirt.

## Edit the book

- Start with `docs/index.md` and the Markdown files in `docs/chapters/`.
- Keep sources beside the claims they support; use `docs/sources.md` as the research shelf.
- Each page has a title and an `order` field at the top. These control book navigation.
- Add a chapter by creating another `.md` file with the same front matter, then link it from the contents.
- Read `EDITORIAL.md` before expanding the manuscript.

All book prose lives in Markdown. `docs/_layouts/book.html` supplies the shared page layout; `docs/assets/book.css` supplies its appearance. Jekyll turns the Markdown into ordinary HTML pages. No database, frontend framework, or AI API is needed.

## Publishing

Push to `main` to build and publish through the **Publish book** GitHub Actions workflow. Pull requests build the book without publishing it. GitHub Pages uses **GitHub Actions** as its publishing source.

The site configuration is `docs/_config.yml`. If the GitHub repository name changes, update its `baseurl`; if the owner changes, also update `url` and the links in this README.

## Starting point

This project grows from the [original issue prompts](https://github.com/kaw393939/is117_test/tree/complete/instructor/issue-prompts) and [first book](https://github.com/kaw393939/is117_test/tree/complete/book). Those are background material, not sources establishing historical or psychological claims.

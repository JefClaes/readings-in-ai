# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

A curated reading guide to foundational AI papers, hosted on GitHub Pages. Modelled after [redbook.io](https://www.redbook.io/). No build step, no framework — plain HTML and CSS.

## Structure

```
index.html          # Home page with table of contents
style.css           # Shared styles (all pages link to this)
.nojekyll           # Prevents GitHub Pages from running Jekyll
chapters/
  01-perceptron-backprop.html
  02-deep-learning.html
  03-word-representations.html
  04-attention-transformer.html
  05-pretraining.html
  06-scaling-llms.html
  07-alignment.html
  08-computer-vision.html
  09-agentic-ai.html
```

## Conventions

- Chapter pages are in `chapters/` and reference `../style.css` and `../index.html`.
- Each chapter has: a `div.chapter-number`, an `h1` title, 3–4 paragraphs of editorial commentary, a `div.papers` section with a `ul.paper-list`, and a `nav.chapter-nav` with prev/next links.
- Every paper must have a link. Use arXiv (`https://arxiv.org/abs/[ID]`) where available; for older papers without arXiv, find a stable alternative (author-hosted PDF, Semantic Scholar, official proceedings).
- Editorial tone is neutral and encyclopedic — no first-person, no promotional language.
- All external links use `rel="noopener noreferrer"`.

## GitHub Pages

Enable in repository Settings → Pages → Deploy from branch `main`, root `/`. The `.nojekyll` file prevents Jekyll processing so HTML is served as-is.

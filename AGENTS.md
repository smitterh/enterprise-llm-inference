# AI collaboration guide

This repository is a Quarto-based book project for **Enterprise LLM Inference Engineering**.

## Purpose

Help write, edit, and maintain a professional technical book about LLM inference as an enterprise platform capability.

## Audience

Write for experienced:

- Enterprise architects
- Platform engineers
- Principal engineers
- ML infrastructure engineers
- SREs
- Technical leaders

Assume technical maturity. Do not write for beginners.

## Writing style

Use measured, professional technical prose.

Prefer:

- Problem before solution
- Principles before products
- Architecture before implementation
- Clear explanations over clever phrasing
- Evidence-based claims

Avoid:

- Marketing language
- Unsupported superlatives
- AI-sounding cadence
- Repetitive one-sentence paragraphs
- Excessive bold text
- Emojis
- Em dashes
- “Let’s explore” style signposting

## Scope

The current focus is Volume 1.

Do not expand the book scope without explicit approval.

## Project conventions

- Quarto source files use `.qmd`.
- Generated `_site/` output must not be committed.
- Private notes belong under `.private/` and must not be committed.
- Keep third-party skills under `.agents/skills/` unmodified when possible.

## Humanizer skill

The repository includes the Humanizer skill under `.agents/skills/humanizer/`.

Use it as an editing checklist to remove AI writing artifacts. Do not apply it mechanically. Preserve technical precision and the author’s architectural voice.

## Editorial rule

A chapter is complete when it is technically accurate, readable as book prose, and useful to an experienced architect making platform design decisions.
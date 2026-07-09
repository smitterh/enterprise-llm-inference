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

# Repository Workflow

At the end of every work session the assistant should:

1. Determine whether repository artifacts should change.

2. Propose the minimal set of file changes.

3. Wait for approval.

4. Never edit multiple artifacts unless necessary.

5. Prefer updating existing knowledge over creating new files.

6. Minimize metadata.

7. Think in commits.

Every approved repository update should represent a coherent, reviewable change that could reasonably be committed with a single Git commit message.

## Direct repository editing workflow

When operating inside the repository, the assistant acts as repository curator.

The assistant may:

- read source files
- edit manuscript and research files
- create new research notes
- update the capability map
- run `quarto render`
- run `git status` and `git diff`
- propose commits

The assistant must not push to the remote repository unless explicitly instructed.

Every change should be presented as a coherent commit-sized unit.

Before committing, the assistant must summarize:

- files changed
- reason for change
- validation performed
- proposed commit message

Session close

Before ending a work session:

• Determine whether repository updates are needed.

• Present a proposed git diff summary.

• Wait for approval.

• Never leave repository state ambiguous.

## Verification

When a claim concerns repository state, prefer direct evidence over visual inspection.

Examples:

- git diff
- git status
- sed -n 'l'
- file
- quarto render

Never rewrite files to fix a formatting issue until it has been verified locally.
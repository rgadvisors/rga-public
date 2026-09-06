# rga-public

Method, prompts, and reference documents that RG Advisors publishes for anyone to read
and reuse. This is the open tier of the firm's estate: what a prospect, a peer, or a
future client can take away without an engagement.

RG Advisors is a design-build partner for AI-enabled organizations in commercial real
estate, finance, and hospitality. The firm's public stage sequence is Diagnose, Build,
Evolve. Site: https://rgadvisors.ai

## What is here

Each item gets a row below with its version and the date it was published. A revision is
a new version and a new row; published files are not edited in place.

| Item | What it is | Version | Published |
|---|---|---|---|
| [Self-interview, Claude edition](self-interview/) | A prompt you paste into a new Claude conversation that interviews you and writes your instruction files, with the setup instructions and the month-two tune-up | 2.3 | 2026-09-06 |

Next: the web design system research-and-plan prompt, after its first full run has
finished and been reviewed. Editions of the self-interview for other vendors land as
each finishes its first run.

## How content gets here

Content enters this repository from the firm engine (`rga-core`) by an explicit publish
decision, never directly from a client engagement. Before each publish an identifier
scan runs across the whole repository for every client name, entity, address, and
parcel number from every active and closed engagement. A hit is a defect. Nothing a
client paid for under an engagement's licensed scope is published, even with
identifiers removed.

## Licenses

Two licenses apply, by file type:

- Documents, prompts, and templates (everything that is not code) are licensed under
  Creative Commons Attribution 4.0 International. See `LICENSE`. Reuse, adapt, and
  redistribute with attribution to RG Advisors.
- Code, meaning anything under a `scripts/` directory or with a source-code extension,
  is licensed under the MIT License. See `LICENSE-CODE`.

Attribution line for documents: "Adapted from RG Advisors, rga-public,
https://github.com/rgadvisors/rga-public, CC BY 4.0."

## What this is not

It is not a support channel, a product, or a statement of any client's configuration.
Documents describe method as of their published date and are not updated in place;
a revision is a new version with a new row above. Questions about engagements go to
the firm site, not to issues here.

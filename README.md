# FallCRM Elite

**Live: https://sjgant80-hub.github.io/fallforce/**

This repo is the manifest and the name. The CRM it describes is built and shipped as
[FallForce](https://sjgant80-hub.github.io/fallforce/) — open that page, its own title is
*FallCRM Elite*. This page redirects there.

It used to serve a live public page carrying nothing but a heading and a licence line, which read
as a product with nothing in it rather than as a name pointing at one.

---

# FallCRM Elite

**The CRM for people who hate CRMs.**

Sovereign contacts + pipeline + deals + notes + signal-based timelines. Every FallHub instance gets FallCRM Elite as a snap-in module.

- **Publisher:** [AI-Native Solutions](https://www.ai-nativesolutions.com/)
- **Licence:** MIT
- **Seal:** `◊·κ=1`
- **Status:** spec published · implementation in progress

## What makes it different

- **Signal timelines, not activity logs.** Every touchpoint is a typed signal (email_open, reply, meeting, call, note, deal_stage_change) with timestamp + confidence. The timeline is a chronologically-ordered signal stream, not a paginated activity feed.
- **Client-portfolio kernel.** Each contact carries their own voice sub-kernel — how they prefer to be contacted, their industry vocabulary, banned phrases, meeting cadence.
- **Agentic follow-up.** Schedule follow-ups as intents; the agent picks the right channel + phrasing at execution time.
- **Offline-capable.** IndexedDB-backed. Sync via mesh when available. Never rents you the tool.

## Tools registered (per `module.manifest.json`)

- `create_contact` — new contact with initial signal state
- `update_deal_stage` — pipeline stage transition
- `add_note` — timestamped note
- `schedule_followup` — agentic follow-up scheduling

## Kernel extension

Adds a `crm` block to your FallHub kernel with pipeline stages, signal types, and follow-up defaults. Compatible with every vertical.

## Related

- [FallHub](https://sjgant80-hub.github.io/fallhub/) — the substrate
- [FallReach](https://github.com/sjgant80-hub/fallreach) — the outbound engine that feeds signals into FallCRM Elite
- [Module marketplace](https://sjgant80-hub.github.io/fallhub/modules.html)

MIT · Copyright © 2026 AI-Native Solutions

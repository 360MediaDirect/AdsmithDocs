# Open Issues — Plain-Language Overview

_Last updated 2026-07-11 21:16:44 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, you'll see a clear "locked by" notice and be warned if the record changed since you opened it, so no one's work gets silently wiped out. (#267)
- **[Feature]** **Searchable history of changes** — A new audit log will let administrators see every change made across the app — what changed, who changed it (or which automated process), and when — making it easy to answer "who touched this and when." (#276)
- **[Feature]** **Cleaning up settings that do nothing** — Several controls that currently look active but have no effect (such as the Advertiser Web Presence fields and some user-permission toggles) will be removed or hidden, so the screens only show options that actually work. (#296)
- **[Task]** **Bringing Users management up to par** — A review comparing the old Users screen with the new one to plan the return of missing capabilities like bulk role changes, last-login info, and two-factor status. (#80)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will now show a proper error message instead of unexpectedly sending you to the dashboard. (#239)
- **[Task]** **Decision on the old file-share page** — Confirming whether the legacy file-share page is still used by anyone, so it can either be brought forward or intentionally retired. (#328)

## Offers
- **[Bug]** **Success pixels that never fire** — A high-priority fix so conversion/tracking pixels you set up on an offer actually fire on success, restoring attribution that's currently being lost silently. (#297)
- **[Bug]** **Offer settings not reaching the live experience** — Several fields saved on an offer weren't making it through to what visitors actually see; this ensures each saved option is either used live or clearly removed. (#295)
- **[Task]** **Auto-register offers respecting targeting** — Making sure auto-registered offers honor the same visitor targeting (age, gender, state, zip, device) as regular offers, so they don't fire for people they should exclude. (#333)
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit screens will show your current in-progress edits instead of the last saved version, so you can check changes before saving. (#292)
- **[Feature]** **Performance projections for new offers** — An exploratory tool to estimate how a new offer is likely to perform based on your historical offer data, replacing the informal manual gut-check. (#322)

## Data Clients
- **[Feature]** **Post-conversion delivery behaviors restored** — The older "after success" delivery/redirect behaviors for certain clients are being brought into the new platform so nothing is lost after a conversion. (#327)
- **[Feature]** **Restoring custom pre-ping checks** — Legacy per-client validation checks (used by hundreds of active data clients) are being ported so those serve-time checks run correctly on the new platform. (#338)

## Surveys
- **[Feature]** **Design options that actually show up** — Every customization on the survey Design tab will be reflected in what visitors see, with a full check that no design option is left disconnected. (#288)
- **[Feature]** **Finishing placement Design-tab settings** — Remaining placement design settings (like iFrame height and display format) will either be applied to the live survey or removed if unused, so no option is misleading. (#293)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a staging version of the app using prod-like data for verification, locked to read-only so testing can't accidentally change real data. (#270)
- **[Feature]** **Turning conversations into tracked work items** — A Slack helper that reads discussions and automatically files or updates issues, reducing manual note-taking. (#272)

## Modals
- **[Feature]** **Making the Modal Design tab meaningful** — The Modal Design tab's settings currently don't affect the visitor modal; they'll either be wired up to actually change the modal or removed to avoid confusion. (#294)

## Flows
- **[Task]** **Tidying up the Flow form's appearance** — Fixing styling gaps on the Flow form so fields, color pickers, checkboxes, and paired fields display cleanly and consistently with other screens. (#152)

## Campaigns
- **[Feature]** **Bringing back Campaigns management** — Adding a Campaigns area to the new platform so you can view, create, edit, and configure campaigns and offer groups just like the legacy admin. (#200)

## Dashboard
- **[Task]** **Confirming report numbers match the legacy system** — Investigating why some dashboard report figures differed from the old system, to pinpoint any discrepancy and confirm the numbers can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->

# Open Issues — Plain-Language Overview

_Last updated 2026-07-17 09:34:20 UTC · 16 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers & Placements

- **[Feature]** **Preview shows your unsaved edits** — When you preview a placement or offer while editing, you'll see exactly what you've changed on screen, even before saving. No more saving first just to check how a tweak looks. (#292)
- **[Feature]** **Placement design settings will actually take effect** — A handful of Design tab options for placements are being connected end-to-end so that choices like display format and height show up in the live survey as expected, instead of being saved but ignored. (#293)
- **[Bug]** **Saved offer settings weren't reaching the live offer** — Several offer options you set (including modal fields, display URL, and certain data-client flags) weren't being carried through to what visitors actually see. This fix ensures each option either works or is removed so nothing is misleading. (#295)
- **[Bug]** **Success pixels not firing** — A high-priority fix: conversion tracking pixels set up on offers were silently never firing, meaning lost tracking with no warning. Once fixed, your configured success pixels will fire reliably. (#297)
- **[Bug]** **Auto-register offers ignoring visitor targeting** — A high-priority fix: auto-register offers were being counted for visitors who should have been excluded by age, gender, state, zip, or device targeting. This will make them respect the same targeting rules as other offers. (#333)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your own historical offer data, giving Kurt a data-driven gut-check at intake instead of relying on a manual review. (#322)

## Admin & Users

- **[Task]** **Bringing the Users area up to parity with the old system** — A review of the Users screens against the legacy app, identifying missing pieces (like bulk actions, last-login and two-factor status, and password setup) so the new Users area gains the capabilities users expect. (#80)
- **[Feature]** **Cleaning up admin controls that don't do anything** — Some settings across Advertisers, Users, Data Clients, and Pre-Pings look like they work but actually have no effect. These will be removed or hidden (or properly implemented) so what you see is what you get. (#296)

## Data Clients & Pre-Pings

- **[Feature]** **Restoring after-success delivery behaviors** — Post-conversion delivery and redirect steps that existed in the old system are being brought over to New Adsmith Frontend, so affected clients keep working as before after a lead succeeds. Nearly complete. (#327)
- **[Feature]** **Porting legacy pre-ping validation for data clients** — A high-priority effort to bring over custom serve-time validation used by hundreds of data clients, which currently isn't running on the new platform. Once done, those clients' pass/reject checks will work again. (#338)

## Behind the Scenes

- **[Task]** **A safe, read-only staging environment for testing** — Setting up a copy of the product against realistic data that can be reviewed without any risk of changing live information. Supports testing and verification. (#270)
- **[Feature]** **A Slack helper that turns conversations into tracked tasks** — An internal tool to automatically capture action items from team chats and file them as work items, reducing manual note-taking. (#272)

## Surveys

- **[Feature]** **Making sure every Design tab option really works** — A cross-product review to confirm that each customization option on the Design tab is fully connected and reflected in the survey visitors see, with any dead options fixed or removed. (#288)

## Modals

- **[Feature]** **Fixing the Modal Design tab** — Every field on the Modal Design tab currently has no effect on the visitor modal. This will either wire those header and progress-bar options through so they work, or remove the tab if it isn't needed. (#294)

## Flows

- **[Task]** **Polishing the Flow form's appearance** — Cleaning up styling issues on the Flow form so text boxes, color pickers, checkboxes, and paired fields look consistent and properly laid out, matching the other forms. Partly done. (#152)

## Reports & Dashboard

- **[Task]** **Confirming Dashboard report numbers match the old system** — Investigating why some Dashboard report figures didn't line up with the legacy app, pinpointing the cause, and confirming the numbers can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6f6b46eb23460d5a4dadb515313ffdc9b368125f6f6ff2fee621d7d1d0c4666e -->

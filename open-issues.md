# Open Issues — Plain-Language Overview

_Last updated 2026-07-12 17:22:30 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When two admins have the same record open, the app will now warn you if someone else changed it while you were working, and will show a clear "locked by so-and-so" message instead of silently discarding a colleague's changes. (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log will record who changed what and when across offers, placements, advertisers, and other records (including automated changes), so you can finally answer "who edited this and when?" (#276)
- **[Feature]** **Tidy up controls that don't actually do anything** — Several settings that look editable but have no real effect (like the Advertiser Web Presence fields, some user permission toggles, and a few data-client and pre-ping options) will be removed or hidden, so what you see on screen matches what actually happens. (#296)
- **[Bug]** **Invalid links should show an error, not send you to the Dashboard** — When you test a bad link, you'll get a clear failure message right in the Link Testing screen instead of being unexpectedly dropped onto the Dashboard. (#239)
- **[Task]** **Review of the Users area against the old system** — A behind-the-scenes comparison of the old and new user-management screens to catch any missing features (like bulk role changes or two-factor status) before they're prioritized for building. (#80)
- **[Task]** **Decide the future of the old File Share page** — A quick check on whether anyone still needs the legacy file-sharing page so it can either be rebuilt in the new admin or officially retired. (#328)

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — A high-priority fix so that the conversion pixels you set up on offers actually fire when a lead succeeds, restoring accurate attribution and revenue tracking. (#297)
- **[Bug]** **Some saved offer settings aren't reaching the live experience** — Several offer fields you fill in (including modal settings and a few delivery options) are being dropped before they reach visitors; each will be either properly connected or removed so nothing you save is silently ignored. (#295)
- **[Task]** **Auto-register offers should respect visitor targeting** — Auto-register offers currently fire for everyone, ignoring age, gender, state, ZIP, and device targeting; this work confirms the correct behavior and makes those offers honor the same targeting rules as regular offers. (#333)
- **[Feature]** **Preview unsaved changes on Offers and Placements** — The Preview button will show your current, unsaved edits instead of the last-saved version, so you can check a change before committing it. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool to estimate how a new offer is likely to perform based on your historical offer data, replacing the informal manual gut-check with a data-driven view. (#322)

## Surveys

- **[Feature]** **Make sure every Design tab setting actually shows up** — A thorough check across all entities so that each option on a Design tab is genuinely reflected in the survey the visitor sees, with no dead or ignored settings. (#288)
- **[Feature]** **Finish connecting the Placement Design settings** — Placement design options such as survey height and display format will be fully wired into the live survey widget, and any leftover unused options will be either connected or removed. (#293)

## Data Clients

- **[Feature]** **Bring over "after-success" delivery behavior** — Post-conversion delivery and redirect steps from the old system will be recreated so data clients continue to hand off leads correctly after a successful conversion. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients rely on custom validation that runs before a lead is served; this high-priority work rebuilds that behavior in the new platform so those checks don't silently stop working. (#338)

## Behind the Scenes

- **[Task]** **A read-only test environment using real-world data** — Setting up a staging copy of the product loaded with production-like data for safe verification, with all editing locked so nothing can be accidentally changed. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — A helper that reads designated chat channels and files action items as tracked issues, cutting out manual copy-and-paste when capturing to-dos. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The modal header and progress-bar design fields currently have no effect on what visitors see; they'll either be connected to the live modal or removed so the tab isn't misleading. (#294)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Cleanup so the Flow form looks consistent with the Placement and Modal forms, with properly styled text boxes, color pickers, checkboxes, and side-by-side fields instead of broken or plain layouts. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns area to the new platform** — A high-priority build to recreate campaign management (creating and editing campaigns, offer groups, CTA text, offer handling, and marketing partners) that exists in the old admin but is missing today. (#200)

## Dashboard

- **[Task]** **Investigate why report numbers don't match the old system** — A review to pin down why some Dashboard report figures differ from the legacy app and to either fix the discrepancy or confirm the numbers are correct, so you can trust what the reports show. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->

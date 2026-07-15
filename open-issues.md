# Open Issues — Plain-Language Overview

_Last updated 2026-07-15 23:20:01 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on placements and offers** — When editing a placement or offer, the Preview button will show your in-progress changes right away, so you no longer have to save first just to see how an edit looks. (#292)
- **[Bug]** **Some saved offer settings never reach live pages** — Several offer options (including modal settings, Display URL, and certain data-client flags) are saved but quietly dropped before they reach visitors. This fix ensures the choices you make on an offer actually take effect. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — A high-priority fix: conversion pixels configured on an offer currently never fire, meaning completed leads aren't being counted. Once resolved, your success pixels will fire reliably and attribution will be accurate. (#297)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, giving you a data-driven gut-check at intake instead of relying on a manual review. (#322)
- **[Task]** **Auto-register offers should respect visitor targeting** — A high-priority fix: auto-register offers currently fire for every visitor, ignoring age, gender, state, zip, and device targeting. This work makes them honor the same targeting rules as regular offers so they only fire for the right audiences. (#333)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When two admins open the same record at once, this adds a clear "locked by someone else" notice and a warning if a record changed while you had it open, so one person's work can't silently erase another's. (#267)
- **[Feature]** **Remove settings that don't actually do anything** — Several admin controls (an Advertiser "Web Presence" tab, some user permission toggles, and a few data-client and pre-ping options) are shown but have no effect. They'll be removed or hidden so the screens only display controls that truly work. (#296)
- **[Task]** **Decide the future of the legacy file-share page** — A review of whether the old file-share page is still needed, so it's either rebuilt in the new admin or formally retired. (#328)
- **[Task]** **Users screen comparison with the legacy system** — A documentation review comparing the old and new Users area to catch anything missing (like bulk role changes, 2FA status, and last-login info) and guide what to build next. (#80)

## Surveys

- **[Feature]** **Make sure every Design-tab option actually shows up** — A thorough check across all entities to confirm that each design and customization option you set is reflected in what visitors see, with no "dead" settings that save but do nothing. (#288)
- **[Feature]** **Finish connecting placement Design settings to the survey** — Several placement Design-tab options (like display format and iframe height) are saved but not yet applied. This work wires them through so your choices show up in the live survey, or removes ones that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery steps for data clients** — Certain after-success behaviors from the legacy system weren't carried over. This brings them back so post-conversion delivery and redirects work as they did before. (#327)
- **[Feature]** **Bring over legacy pre-ping checks for data clients** — A high-priority effort to restore custom validation that runs when serving offers for hundreds of data clients, so those checks work on the new platform instead of silently doing nothing. (#338)

## Dashboard & Reports

- **[Task]** **Confirm report numbers match the legacy system** — An investigation into why some dashboard report figures differed from the old system, so you can trust the numbers you see are consistent and correct. (#271)
- **[Bug]** **Show a clear error when a tested link is invalid** — Testing an invalid link currently sends you to the dashboard with no explanation. After this fix, you'll get a clear error message so you know the link failed. (#239)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — Standing up a staging version of the product using production-like data for verification, locked to read-only so testing can't change any real data. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads designated Slack channels and automatically files action items as tracked issues, reducing manual copy-paste when capturing follow-ups. (#272)

## Flows

- **[Task]** **Polish the appearance of the Flow form** — Parts of the Flow form look unstyled and some paired fields stack awkwardly instead of sitting side by side. This is a careful cleanup to bring its look in line with the Placement and Modal forms. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — The Modal Design tab's fields (header title, colors, progress bar, and more) currently have no effect on the visitor modal. This will either connect them so they display, or remove them to avoid confusion. (#294)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d541cdec2d7ef7e80b16585fe689f12231c8b31406080f26d5421cd3a156890a -->

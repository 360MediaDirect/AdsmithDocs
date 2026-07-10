# Open Issues — Plain-Language Overview

_Last updated 2026-07-10 19:31:11 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Feature]** **Preview your unsaved changes before saving** — On Placement and Offer edit pages, the Preview button will show the changes you've just made instead of only the last saved version, so you no longer have to save first just to see how an edit looks. (#292)
- **[Bug]** **Some offer settings weren't reaching the live experience** — Several saved offer options were being dropped before they got to the live widget. This fix makes sure the choices you configure actually take effect for visitors. (#295)
- **[Bug]** **Success tracking pixels weren't firing** — A high-priority fix: conversion pixels set under "Pixels to Fire on Success" were silently never firing, meaning lost tracking. Once fixed, configured success pixels will fire reliably end-to-end. (#297)
- **[Task]** **Auto-register offers were ignoring visitor targeting** — A high-priority fix: auto-register offers were firing for visitors they should have excluded (by age, gender, state, zip, or device). This work makes them respect the same targeting rules as other offers. (#333)
- **[Feature]** **Automatic performance estimate for new offers** — An exploratory feature to project how a new offer is likely to perform based on your historical offer data, replacing the current manual gut-check review. (#322)

## Surveys & Modals
- **[Feature]** **Make sure survey design options actually apply** — A review across all entities to confirm every design/customization option you set is genuinely reflected in what visitors see, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Options like iFrame height and display format are being saved but not yet applied to the live survey. This work wires them through (or removes any that aren't needed). (#293)
- **[Feature]** **Fix the Modal Design tab** — The six fields on the Modal Design tab currently have no effect on what visitors see. Each will either be made to work or removed so the form only shows controls that do something. (#294)

## Admin Area & Users
- **[Feature]** **Remove admin controls that don't do anything** — Several settings (such as the Advertiser Web Presence fields and some user permission and data-client options) are saved but never used. Hiding or removing them prevents confusion and false expectations. (#296)
- **[Task]** **Bring the Users area up to par with the legacy system** — A documentation review comparing the old and new Users screens, identifying missing pieces like bulk role changes, last-login, and two-factor status so they can be planned back in. (#80)
- **[Task]** **Decide the future of the legacy file-share page** — Confirm whether anyone still needs the old file-share page and either give it a home in the new admin or retire it cleanly. (#328)

## General / Across the App
- **[Feature]** **Stop two people from overwriting each other's edits** — When someone is already editing a record, others will see a clear "locked by" notice, and you'll be warned to reload if a record changed while you had it open — preventing accidental lost changes across every edit screen. (#267)
- **[Feature]** **A searchable activity log of who changed what** — A new admin Audit Log that records every manual and automated change to your records with a timestamp and who made it, so you can answer "who changed this and when." (#276)
- **[Bug]** **Clearer result when testing an invalid link** — Testing an invalid link currently drops you on the dashboard with no explanation. This fix shows a proper error message instead. (#239)

## Data Clients & Pre-Pings
- **[Feature]** **Restore custom pre-ping checks for data clients** — A high-priority effort to bring back the per-client validation that ran when offers were served in the legacy system; hundreds of clients rely on it and it isn't running today. (#338)
- **[Feature]** **Restore after-success delivery for data clients** — Bring the legacy post-conversion delivery/redirect behavior over to New Adsmith Frontend so affected clients keep working as before. (#327)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a staging copy that mirrors real data but can't be changed, so the team can verify the product against realistic data without any risk. (#270)
- **[Feature]** **Turn conversations into tracked tasks automatically** — A helper that reads designated chat conversations and files the resulting action items for the team, reducing manual copy-and-paste. (#272)

## Reports & Dashboard
- **[Task]** **Investigate report numbers not matching the legacy system** — Reviewers noticed dashboard report totals didn't line up with the old system. This work compares the two over a fixed date range to find the cause and confirm the numbers can be trusted. (#271)

## Campaigns
- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — A critical, high-priority addition: the Campaigns area from the legacy system isn't available yet. This adds the ability to view, create, edit, and configure campaigns and their offer groups. (#200)

## Flows
- **[Task]** **Fix styling issues on the Flow form** — Parts of the Flow form currently look unstyled and some paired fields stack awkwardly instead of sitting side by side. This tidies up the form so it matches the look of other screens. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->

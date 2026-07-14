# Open Issues — Plain-Language Overview

_Last updated 2026-07-14 03:01:48 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved changes on Placements and Offers** — When you hit Preview while editing, you'll see exactly what you've changed on screen right now, instead of having to save first just to check your work. (#292)
- **[Bug]** **Some saved offer settings weren't reaching live pages** — A number of offer options were being saved correctly but quietly dropped before appearing on the visitor-facing experience. This fix makes sure the settings you choose actually show up (or gets clearly removed if they're not needed). (#295)
- **[Bug]** **Success tracking pixels weren't firing** — A high-priority fix: conversion pixels set up on offers were silently never firing, meaning lost tracking with no warning. Once done, the pixels you configure will fire as expected. (#297)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform, based on your own historical offer data, replacing the old manual gut-check review. (#322)
- **[Task]** **Auto-register offers will respect visitor targeting** — A high-priority fix so auto-register offers honor age, gender, state, zip, and device targeting like regular offers do, instead of firing for visitors who should be excluded. (#333)

## General / Across the App

- **[Task]** **Bring the Users area in line with the old system** — An in-progress review comparing the new Users screens against the legacy version to spot and close any missing features (bulk actions, extra columns, and more). (#80)
- **[Feature]** **Stop two people from overwriting each other's edits** — When someone else is already editing a record, you'll see a clear notice, and you'll be warned before saving over changes made while you had the page open. Applies across all the main entity screens. (#267)
- **[Feature]** **A searchable history of every change (Audit Log)** — A new admin page that records who changed what and when — manual edits and automated updates alike — so you can finally answer "who changed this?" with confidence. (#276)
- **[Feature]** **Remove admin controls that don't actually do anything** — Several settings (like Advertiser Web Presence fields and a few permission toggles) currently save but have no effect. These will be removed or hidden so the screens only show controls that really work. (#296)
- **[Task]** **Decide the future of the legacy file-share page** — A quick review to confirm whether the old file-share page is still used by anyone, then either rebuild it in the new admin or retire it cleanly. (#328)

## Surveys

- **[Feature]** **Make sure every design option actually changes the survey** — A thorough check across all entity forms to confirm each customization option you set is truly reflected in the visitor's survey view, with any dead options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Wiring up the remaining Placement Design-tab settings (like display format and height) so the choices you make there actually appear in the live survey. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore after-success delivery behaviors from the old system** — Bringing over the post-conversion delivery and redirect steps that ran in the legacy platform, so those data-client behaviors keep working. (#327)
- **[Feature]** **Restore custom pre-ping validation for data clients** — A high-priority effort to carry over the legacy per-client checks that run when an offer is served; hundreds of active data clients rely on this, and it isn't running on the new platform yet. (#338)

## Dashboard & Reports

- **[Bug]** **Testing an invalid link should show an error, not bounce you to the Dashboard** — Right now, entering a bad link quietly drops you on the Dashboard. This fix will show a clear failure message instead. (#239)
- **[Task]** **Investigate why report numbers don't match the old system** — Reviewers noticed dashboard report figures differed from the legacy app. This work compares the two over a fixed date range to find and explain any discrepancy. (#271)

## Behind the Scenes

- **[Task]** **A staging environment for safe testing** — Setting up a read-only test environment that mirrors real data, so the team can verify the product against production-like information without risk of changing anything. (#270)
- **[Feature]** **A Slackbot that turns conversations into tracked tasks** — An internal helper that reads designated Slack channels and automatically files action items, reducing manual note-taking and follow-up. (#272)

## Modals

- **[Feature]** **Connect or remove the Modal Design tab** — The Modal Design tab's settings currently save but don't appear anywhere for visitors. This work will either wire them up so they show (headers, progress bar, etc.) or remove them if the modal is meant to be simpler. (#294)

## Flows

- **[Task]** **Tidy up the appearance of the Flow form** — Some parts of the Flow form look unstyled or misaligned (plain text boxes, stacked fields). This is a scoped cleanup to make it match the polished look of the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Add the missing Campaigns module** — A high-priority, critical addition: the Campaigns area from the old admin isn't in the new platform yet. This restores the ability to view, create, edit, and configure campaigns and their offer groups. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->

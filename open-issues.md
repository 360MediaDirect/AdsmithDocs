# Open Issues — Plain-Language Overview

_Last updated 2026-07-20 05:13:14 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings never reach live ads** — Several options you configure on an offer (including its Modal-tab fields, "Force More Info Visible," Display URL, and certain data-handling flags) are currently being dropped before the offer goes live. This fix makes sure the settings you set actually take effect where visitors see them. (#295)
- **[Bug]** **Success pixels not firing** — A high-priority fix: conversion tracking pixels set up under "Pixels to Fire on Success" have been silently failing to fire, which means lost tracking with no warning. Once fixed, configured success pixels will reliably fire so your conversions and revenue are properly recorded. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting** — A high-priority fix: auto-register offers have been firing for every visitor, even ones excluded by age, gender, state, ZIP, or device targeting. This ensures those offers respect the same targeting rules as regular offers so they only fire for the intended audience. (#333)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This field on the offer Delivery tab is saved but has no effect on what's served, and the intended rule needs business confirmation. The work will either make it actually exclude the right offers or clarify how it's meant to behave. (#351)
- **[Feature]** **Preview unsaved changes on Placements and Offers** — Right now the Preview button shows the last-saved version, so you have to save before you can see edits. This upgrade lets Preview reflect your current, in-progress changes without saving first. (#292)
- **[Feature]** **Predict how a new offer will perform** — An exploratory feature to estimate a new offer's likely performance using your own historical offer data, replacing an informal manual gut-check. It would give you a data-driven projection at intake to help decide on new offers. (#322)

## Surveys

- **[Feature]** **Make sure every design option actually shows up** — A review across all entities to confirm each design and form option you can set is truly connected end-to-end, with nothing that quietly does nothing. Design-tab choices will reliably appear in the survey view as expected. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — Certain Placement design options (like iFrame height, display format, and a few visibility and style settings) are saved but not yet applied to the widget visitors see. Each will be either fully wired up so it takes effect, or removed if it's not needed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior** — Some clients relied on special actions that run after a successful conversion, which weren't carried over to New Adsmith Frontend. This work (nearly complete) brings that behavior back as a reusable, configurable option so those clients work as before. (#327)
- **[Feature]** **Bring over legacy pre-ping validation** — A high-priority parity gap: hundreds of data clients used custom serve-time validation checks that don't currently run on the new platform. This work restores those checks so the right validation happens before an ad is served. (#338)

## General / Across the App

- **[Task]** **Review of the Users area vs. the old system** — A documentation effort comparing the new Users management screens against the legacy version to spot missing capabilities (like bulk actions, password entry on new users, and login/2FA details) and plan what to add. This guides upcoming improvements to the Users area. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings across the app (Advertiser Web Presence fields, certain user permission toggles, and some Data-Client and Pre-Ping options) are shown but currently have no effect. They'll be hidden or removed so the admin screens only show controls that genuinely work. (#296)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A staging copy of the app connected to production-like data for verification, locked so it can't accidentally change anything. This helps confirm everything works against realistic data before it reaches you. (#270)
- **[Feature]** **Automatically turn conversations into tracked work items** — A tool to capture action items from team chat and log them as tracked issues, reducing manual copying. This is an internal workflow improvement with no direct effect on the product screens. (#272)

## Modals

- **[Feature]** **Fix or remove the Modal Design tab** — All six fields on the Modal Design tab are currently saved but never actually shown to visitors. They'll either be wired up so your modal header and progress bar settings take effect, or removed if the modal is meant to have no header. (#294)

## Properties

- **[Bug]** **Enforce the domain allowlist** — A property's list of allowed domains is saved and editable but isn't actually being enforced, so ads can serve on any website. This fix makes the allowlist work: only approved domains will serve the offer, while properties without a list keep working as they do today. (#350)

## Flows

- **[Task]** **Fix styling issues on the Flow form** — Parts of the Flow form look unstyled or misaligned compared to other forms — text boxes, color pickers, checkboxes, and side-by-side fields don't display correctly. This tidies up the Flow form so it matches the polished look of the Placement and Modal forms. (#152)

## Reports

- **[Task]** **Investigate dashboard numbers that don't match the old system** — During testing, some Dashboard report figures didn't line up with the legacy app. This investigation pinpoints where the difference comes from and confirms the numbers are accurate, so you can trust your reports. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->

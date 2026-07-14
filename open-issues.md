# Open Issues — Plain-Language Overview

_Last updated 2026-07-14 09:34:24 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers & Placements

- **[Feature]** **Preview edits before saving** — On placement and offer edit screens, the Preview button will show your current in-progress changes instead of the last saved version, so you no longer have to save just to see how a change looks. (#292)
- **[Bug]** **Some saved offer settings never reach the live widget** — A number of offer options you set (including Modal-tab fields, Display URL, and several data-client flags) are being dropped before they show up to visitors. This fix ensures each saved option either takes effect or is cleanly removed from the form. (#295)
- **[Bug]** **Success pixels not firing** — A high-priority fix: conversion pixels set under "Pixels to Fire on Success" have been silently not firing, meaning lost tracking. Once fixed, configured success pixels will fire reliably. (#297)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your historical offer data, replacing the informal manual gut-check review at intake. (#322)
- **[Bug]** **Auto-register offers ignore visitor targeting** — A high-priority fix: auto-register offers currently fire for everyone, skipping the age, gender, state, zip, and device targeting rules that normal offers respect. This will make them honor those rules (or the difference will be documented as intended). (#333)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone is editing a record, others will see it's locked and by whom, and the system will warn you if a record changed while you had it open, so no one's work is silently lost. This will apply across all entity screens. (#267)
- **[Feature]** **Searchable history of every change** — A new Audit Log will record who changed what and when across the platform, including automated changes, with per-record history viewable from each entity's detail page. Great for answering "who changed this?" (#276)
- **[Feature]** **Clean up controls that don't do anything** — Several settings that look active but currently have no effect (like the Advertiser Web Presence fields, certain user permission toggles, and a few data-client and pre-ping options) will be removed or hidden so the interface only shows controls that actually work. (#296)
- **[Bug]** **Invalid link test sends you to the Dashboard** — Testing an invalid link currently dumps you back on the Dashboard with no explanation. Once fixed, you'll see a clear error result in Link Testing instead. (#239)
- **[Task]** **Decide the future of the legacy file-share page** — The old file-share page has no equivalent yet; this reviews whether anyone still needs it and either brings it into the new admin or documents it as retired. (#328)

## Surveys

- **[Feature]** **Design tab options fully applied to surveys** — A review to make sure every Design tab customization actually shows up in the survey, with any settings that do nothing being fixed or removed, across all entities. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the survey** — Several placement Design-tab settings (like survey height and display format) are saved but not yet reflected in the live survey. This wires them up or removes the ones that aren't needed. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore after-success delivery behavior** — Post-conversion delivery and redirect steps from the old system haven't been carried over yet. This brings that behavior back so conversions are handled correctly for the clients that rely on it. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients rely on custom validation checks that run before a lead is served, and these aren't running on the new platform yet. This high-priority work brings that validation back so leads are properly screened. (#338)

## Behind the Scenes

- **[Task]** **Staging environment for safe testing** — Setting up a read-only test environment loaded with production-like data, so the team can verify behavior without any risk of changing real records. (#270)
- **[Feature]** **Automatically turn conversations into tracked tasks** — A helper that reads designated chat channels and files action items as tracked issues automatically, cutting out manual copy-and-paste. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — All six fields on the Modal Design tab currently have no effect on what visitors see. This will either connect them to the visitor modal or remove the tab if it's not needed. (#294)

## Flows

- **[Task]** **Fix the visual styling of the Flow form** — Parts of the Flow form look unstyled or misaligned compared to other screens (plain text boxes, unstyled color pickers, fields stacking instead of sitting side by side). This tidies up the form's appearance. (#152)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — A critical, high-priority feature: the ability to view, create, edit, and configure campaigns and offer groups (titles, questions, CTAs, offer handling, marketing partners, and more) isn't in the new platform yet. This restores that core capability. (#200)

## Reports & Dashboard

- **[Task]** **Confirm Dashboard report numbers match the old system** — Testing found Dashboard figures didn't line up with the legacy system. This investigation pins down where the difference comes from and either corrects it or confirms the numbers are accurate. (#271)

## Admin & Users

- **[Task]** **Compare the new Users area to the old one** — A review of what the old Users management screen could do versus the new one, so missing capabilities (like bulk actions, last-login info, and password/notification options) can be prioritized. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->

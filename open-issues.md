# Open Issues — Plain-Language Overview

_Last updated 2026-07-11 05:02:12 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview shows your unsaved edits** — When you preview an offer or placement while editing, you'll see the changes you just made rather than the last saved version, so you can check your work before saving. (#292)
- **[Bug]** **Some saved offer settings weren't reaching live pages** — A number of offer options you can set (including modal fields, "Force More Info Visible," Display URL, and several data-client flags) were being saved but never actually used on the live experience. These will be either fully connected or cleaned up so the form only shows options that do something. (#295)
- **[Bug]** **Success tracking pixels weren't firing** — High priority fix: conversion pixels set up under "Pixels to Fire on Success" were silently never firing, meaning conversions went untracked. Once fixed, configured success pixels will reliably fire. (#297)
- **[Feature]** **Automatic performance projection for new offers** — Exploratory work to estimate how a new offer is likely to perform based on your historical offer data, replacing the informal manual gut-check. This would give a data-driven read at intake time. (#322)
- **[Bug]** **Auto-register offers were ignoring visitor targeting** — High priority fix: auto-register offers were firing for everyone, skipping the age, gender, state, zip, and device rules that normal offers respect. They'll be brought in line so they only fire for the right visitors. (#333)

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other** — When two admins open the same record, the app will warn you and prevent one person's save from silently wiping out the other's changes, with a clear "someone else is editing this" notice. (#267)
- **[Feature]** **Searchable activity history across the platform** — A new Audit Log will record every change to your records — who changed what, when, and whether it was a person or an automated job — and let administrators search it. This makes "who changed this and when" easy to answer. (#276)
- **[Feature]** **Cleaning up controls that don't do anything** — Several admin settings (Advertiser Web Presence fields, a couple of user permission toggles, and some Data-Client and Pre-Ping options) currently save but have no effect. They'll be hidden or removed so the screens only show controls that work. (#296)
- **[Task]** **Decision on the old file-share page** — The legacy file-share page has no equivalent in New Adsmith Frontend yet. This is a keep-or-retire decision to confirm whether anyone still needs it. (#328)
- **[Bug]** **Invalid links should show an error, not the dashboard** — When testing a link that's invalid, you'll get a clear error message instead of being unexpectedly dropped on the dashboard. (#239)

## Surveys

- **[Feature]** **Design-tab settings that actually show up in the survey** — A thorough check to make sure every customization option on the design tabs is truly reflected in the survey view across all entity types, with any dead options fixed or removed. (#288)
- **[Feature]** **Finishing the Placement design settings** — A few Placement design-tab options (such as iFrame height and display format) weren't reaching the live survey. These will be connected so your settings take effect, or removed if they aren't needed. (#293)

## Data Clients

- **[Feature]** **Restoring post-conversion delivery behavior** — The older "after-success" delivery and redirect steps used by certain clients hadn't been carried over. They're being rebuilt as a reusable, configurable option so those clients keep working as before. (#327)
- **[Feature]** **Restoring custom pre-ping checks for data clients** — High priority: hundreds of data clients relied on custom serve-time validation checks that aren't running on the new platform yet. This work brings those checks back so leads are validated as they were before. (#338)

## Behind the Scenes

- **[Task]** **Staging environment for safe testing** — Setting up a read-only test environment using a copy of production data, so the team can verify behavior against realistic data without any risk of changing live records. (#270)
- **[Feature]** **Automatic issue capture from team chats** — A helper that reads team conversations and turns action items into tracked tasks automatically, reducing manual copy-and-paste. (#272)

## Reports

- **[Task]** **Making sure report numbers match the old system** — Investigating why some dashboard report figures didn't line up with the legacy system, to pinpoint any differences, explain the cause, and confirm the numbers can be trusted. (#271)

## Users

- **[Task]** **Comparing the new Users area to the old one** — A documented review of what the legacy Users screens offered versus New Adsmith Frontend, flagging gaps (like bulk actions and last-login info) and improvements so the new experience can be brought up to parity. (#80)

## Flows

- **[Task]** **Tidying up the look of the Flow form** — Fixing styling issues on the Flow form so text boxes, color pickers, checkboxes, and paired fields display cleanly and consistently with the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bringing back Campaign management** — Critical, high-priority work to add the Campaigns area to New Adsmith Frontend so you can view, create, edit, and configure campaigns and offer groups just as you could in the legacy system. (#200)

## Modals

- **[Feature]** **Making the Modal Design tab do something** — The Modal Design tab's settings currently don't appear anywhere for visitors. They'll either be connected so they show on the modal, or removed if the modal is meant to be header-free. (#294)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->

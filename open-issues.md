# Open Issues — Plain-Language Overview

_Last updated 2026-07-11 17:21:18 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Feature]** **Protection against two people overwriting each other's edits** — When two administrators open the same record at once, New Adsmith Frontend will now warn that someone else is editing (or has just changed it) so one person's work can't quietly wipe out another's. (#267)
- **[Feature]** **Searchable activity history for every change** — A new Audit Log will record who changed what and when — across offers, placements, advertisers, and more, including automated updates — so you can finally answer "who touched this and when?" (#276)
- **[Feature]** **Cleaning up admin controls that don't do anything** — Several settings that look active but have no effect (such as Advertiser Web Presence fields and some user permission toggles) will be hidden or removed, so screens only show controls that actually work. (#296)
- **[Task]** **Review of the Users screen against the old system** — A documentation review comparing the old and new Users areas to catch anything missing, like bulk actions and last-login details, before those gaps are prioritized. (#80)
- **[Task]** **Decision on the old File Share page** — Confirming whether the legacy file-sharing page is still needed and either bringing it into the new admin or formally retiring it. (#328)
- **[Bug]** **Clearer result when testing an invalid link** — Instead of being bounced to the Dashboard, testing a bad link will show a proper error message so you know the test failed. (#239)

## Offers
- **[Bug]** **Success tracking pixels now fire correctly** — A high-priority fix so the conversion pixels you set on an offer actually fire on success, restoring lost tracking and revenue attribution. (#297)
- **[Bug]** **Offer settings no longer get lost before going live** — Several saved offer options currently never reach the live experience; this ensures each option is either shown to visitors or clearly removed if unused. (#295)
- **[Task]** **Auto-register offers will respect visitor targeting** — Auto-registered offers currently ignore age, gender, state, ZIP, and device targeting; this work makes them honor those rules (or documents it as intended) so offers only fire for the right visitors. (#333)
- **[Feature]** **Preview shows your unsaved changes** — On the Offer and Placement edit screens, Preview will reflect the edits you're currently making instead of only the last-saved version, so you can check changes before saving. (#292)
- **[Feature]** **Performance projections for new offers** — An exploratory tool to estimate how a new offer is likely to perform based on your historical data, replacing the informal manual gut-check with a data-driven forecast. (#322)

## Surveys
- **[Feature]** **Design settings that reliably show up in the survey** — An end-to-end review so every option on the Design tab actually changes what visitors see, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finishing the Placement design settings** — Wiring up the remaining Placement Design options (like survey height and display format) so they take effect in the live survey, or removing any that aren't used. (#293)

## Data Clients & Pre-Pings
- **[Feature]** **Bringing back post-conversion delivery steps** — Restoring the "after success" handling used by certain clients so post-conversion redirects and delivery work the same as they did in the old system. (#327)
- **[Feature]** **Restoring custom pre-check rules for data clients** — A high-priority effort to bring back per-client validation checks that ran before a lead was sent; hundreds of clients rely on these, and they currently don't run on the new platform. (#338)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of New Adsmith Frontend using production-like data for testing, locked to read-only so nothing can be accidentally changed. (#270)
- **[Feature]** **Automatic issue capture from team chats** — An internal helper that turns action items from team conversations into tracked tasks automatically, reducing manual copy-and-paste. (#272)

## Flows
- **[Task]** **Tidying up the Flow form's appearance** — Fixing styling gaps so the Flow form's text boxes, color pickers, checkboxes, and paired fields look consistent with the Placement and Modal forms instead of appearing unstyled or misaligned. (#152)

## Campaigns
- **[Feature]** **Bringing the Campaigns area to the new platform** — A high-priority build to add Campaign management so you can create, edit, and configure campaigns and their offer groups, matching what the old admin offered. (#200)

## Modals
- **[Feature]** **Making the Modal Design tab actually work** — The Modal Design settings (headers, colors, progress bar) currently have no effect on what visitors see; this will either wire them up or remove them so the tab isn't misleading. (#294)

## Reports
- **[Task]** **Confirming report numbers match the old system** — An investigation into why some Dashboard report figures differ from the legacy system, to pinpoint the cause and either fix it or confirm the numbers are correct. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->

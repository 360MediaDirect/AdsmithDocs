# Open Issues — Plain-Language Overview

_Last updated 2026-07-15 11:31:07 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on Placements and Offers** — When editing a placement or offer, the Preview button will show your current edits instead of only the last saved version, so you can check your work before committing it. (#292)
- **[Bug]** **Some offer settings never reach the live experience** — Several saved offer options (including modal settings, Display URL, and certain data-client flags) currently get dropped and never appear to visitors; this fix ensures each setting is either fully used or clearly removed. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on offers are silently failing to fire, which means lost tracking. This high-priority fix makes configured success pixels work end-to-end. (#297)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check, new offers could be scored against your historical offer data to estimate likely performance, giving a quicker read at intake. (#322)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers are firing for visitors they should exclude (by age, gender, state, ZIP, or device). This high-priority fix makes them respect the same targeting rules as regular offers. (#333)

## General / Across the App

- **[Task]** **Bringing the Users area up to par with the old system** — A review of the Users screens compared to the legacy tool, identifying missing pieces like bulk role changes, last-login info, and password setup so the new Users area matches what people relied on before. (#80)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record for editing, others will see it's locked and by whom, and saves will warn you if the record changed since you opened it — so changes are no longer silently lost. (#267)
- **[Feature]** **Clean up admin controls that don't do anything** — Some settings across Advertisers, Users, Data Clients, and Pre-Pings are shown but have no effect. These will be removed or hidden so the screens only show controls that actually work. (#296)
- **[Task]** **Decide the fate of the old file-share page** — Confirm whether the legacy file-share page is still needed and either give it a home in the new admin or retire it cleanly. (#328)
- **[Bug]** **Invalid links should show an error, not send you to the Dashboard** — When testing a bad link, you'll get a clear failure message instead of being unexpectedly dropped onto the Dashboard. (#239)

## Surveys

- **[Feature]** **Make every Design tab setting actually take effect** — A full check across all entities to ensure each design/customization option you set is reflected in the survey visitors see, with no dead or ignored options. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the survey** — Options like survey height and display format, plus a few partially-connected style settings, will either work in the live survey or be removed so nothing is misleading. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore after-conversion delivery steps for clients** — The post-conversion delivery and redirect behavior from the old system is being brought over so client hand-offs continue to work as before. (#327)
- **[Feature]** **Bring over custom pre-ping checks for hundreds of clients** — Legacy serve-time validation used by 448 clients isn't running on the new platform yet. This high-priority work restores those checks so client-specific rules apply correctly. (#338)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a practice environment that mirrors live data for verification, with safeguards that prevent any accidental changes to real records. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items automatically** — A helper that reads designated Slack channels and files action items as tracked issues, cutting out manual copy-paste when capturing follow-ups. (#272)

## Reports & Dashboard

- **[Task]** **Confirm Dashboard report numbers match the old system** — An investigation into why some Dashboard figures differed from the legacy tool, so you can trust that the numbers line up. (#271)

## Flows

- **[Task]** **Fix the visual styling on the Flow form** — Parts of the Flow form currently look unstyled or misaligned (plain text boxes, stacked fields, unstyled color pickers). This pass tidies up the layout so it matches the rest of the app. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns area into the new platform** — The Campaigns tools from the old admin aren't in the new platform yet. This high-priority feature adds the ability to view, create, edit, and configure campaigns and their offer groups. (#200)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — Every field on the Modal Design tab currently has no effect on what visitors see. This work will either wire the header and progress-bar settings through to the visitor modal or remove the tab entirely. (#294)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f12be1691f4d05be7a51684fc6fe5ab6d4c4751d5a9de6a600395df673d554b3 -->

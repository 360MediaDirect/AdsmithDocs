# Open Issues — Plain-Language Overview

_Last updated 2026-07-25 06:44:17 UTC · 14 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on Placements and Offers** — When editing a placement or offer, the Preview button will show your current in-progress changes instead of the last saved version, so you can check your work before committing it. (#292)
- **[Bug]** **Saved offer settings that never reached live pages** — Several offer options you can fill in (including Modal-tab fields, Display URL, and various delivery flags) weren't actually being applied where visitors see them. This fix ensures each saved option either takes effect or is cleaned up so it isn't misleading. (#295)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check, new offers could get an automated estimate of how they're likely to perform based on your own historical offer data. This is an early, exploratory effort to give a helpful projection at intake time. (#322)

## Surveys

- **[Feature]** **Make every design option actually change the survey** — A full review to confirm that each customization you set on the Design tab genuinely shows up in the live survey, with any options that do nothing being fixed or removed so nothing is misleading. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Certain placement display settings (like survey height and question display format) weren't reaching the live survey. This work wires them up so your choices take effect, or removes the ones that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behaviors** — Certain after-success handoffs that existed in the old system are being brought over to New Adsmith Frontend so conversions continue to be delivered correctly for the affected clients. (#327)
- **[Feature]** **Bring over custom pre-check validation for data clients** — A large group of data clients relied on custom serve-time checks in the old system that don't currently run. This high-priority effort restores those checks so leads are validated as expected before delivery. (#338)

## Behind the Scenes

- **[Task]** **Safe read-only test environment** — Setting up a look-alike environment that mirrors real data for testing and verification, locked to read-only so nothing can be accidentally changed. (#270)
- **[Feature]** **Turn team conversations into tracked work items automatically** — A helper that reads designated team chat channels and files action items as tracked tasks, cutting out manual copy-and-paste and reducing the chance things slip through the cracks. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab do something** — Right now the Modal Design tab's settings (header text, colors, progress bar, and more) don't affect what visitors see. This work either connects those settings to the visitor modal or removes the tab if it isn't needed. (#294)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or awkwardly stacked. This cleanup restores proper styling and side-by-side field layouts so the form matches the polished look of other screens. (#152)

## Dashboard

- **[Task]** **Confirm dashboard report numbers match the old system** — Investigating why some dashboard figures differed from the previous system, pinpointing the cause, and confirming the numbers line up so you can trust what you see. (#271)

## Users

- **[Task]** **Close the gaps between the old and new Users area** — A thorough comparison of the old Users management screens against the new ones, identifying missing capabilities (like bulk actions, last-login and two-factor status, and password/notification options) so they can be prioritized and added. (#80)

## General / Across the App

- **[Feature]** **Remove admin controls that don't do anything** — Some settings across the app (certain Advertiser web-presence fields, a couple of user-permission toggles, and some data-client and pre-ping options) are saved but have no effect. Hiding or removing them prevents confusion and avoids implying access controls that don't actually exist. (#296)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._

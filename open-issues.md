# Open Issues — Plain-Language Overview

_Last updated 2026-06-27 01:39:01 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a proper date range picker with start and end dates, so you can view Dashboard data for any time span instead of only the preset options. (#58)
- **[Task]** **Restore missing Dashboard sections** — Bring back the campaign stats, top offers, and watch list sections so the Dashboard shows full reporting again, with the date range updating them as expected. This is a high-priority fix. (#240)
- **[Feature]** **New "Other Dashboard" views plus an activity log** — Adds "Offers with Legs" and "CLP Performance" views (highlighting offers converting under 30%) and a searchable record of every offer change, so you can spot problem offers quickly and see who changed what and when. (#256)
- **[Task]** **Consistent Dashboard colors** — A defined color palette will be applied across Dashboard views to make charts and figures easier to read at a glance. (#263)

## General / Across the App

- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the whole Admin between dark and light themes from your user menu, with your choice remembered next time you sign in. (#59)
- **[Feature]** **Protection against two people overwriting the same record** — When you open a record to edit, others will see it's being edited, and the system will warn you before anyone accidentally saves over someone else's changes. Works across offers, flows, placements, advertisers, and other entity screens. (#267)
- **[Task]** **Brand guidelines as the main input for AI** — A single, thorough brand-guidelines document will guide AI-generated output so results stay more on-brand and consistent. (#264)
- **[Bug]** **Invalid links no longer dump you on the Dashboard** — When you test a link that isn't valid, Link Testing will show a clear error instead of silently sending you back to the Dashboard. (#239)

## Flows

- **[Task]** **Tidy up the Flow form styling** — Fixes unstyled text boxes, color pickers, and checkboxes, and lines up paired fields side by side so the Flow form looks consistent with the Placement and Modal forms. (#152)
- **[Feature]** **Make the "Step order" setting understandable** — The setting will get a clear label and inline help explaining what it controls and what its values do, so you no longer have to guess. (#226)

## Placements

- **[Feature]** **Easier offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by taxonomy, giving you full control over how offers are arranged. (#235)

## Pre-Pings

- **[Feature]** **Enforce required fields before sending a lead** — When a pre-ping runs before pushing data, a lead missing required fields will be stopped right away instead of being sent on, matching how required fields already work before an offer displays. (#218)

## Campaigns

- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — Adds the ability to view, create, edit, and configure campaigns and offer groups, restoring this core capability that currently exists only in the legacy system. This is high priority. (#200)

## Users

- **[Task]** **Review of the Users area against the old system** — A documented comparison of the legacy Users module and the new one, listing what's still missing (like bulk actions and last-login info) to guide upcoming improvements. (#80)

## Behind the Scenes

- **[Feature]** **Real-time "today" stats** — Behind-the-scenes work so today's impressions, clicks, leads, and revenue display accurately and promptly, with correct Eastern Time handling. (#34)
- **[Feature]** **Faster historical reporting rollups** — Maintenance to summarize daily activity automatically so historical reports stay quick and reliable. (#35)
- **[Task]** **Speed improvements for survey serving** — Adds a caching layer so surveys, offers, and caps load faster in real time. High priority. (#42)
- **[Task]** **Review of an older stats job** — Behind-the-scenes review to decide whether a legacy stats process is still needed or can be retired. (#33)
- **[Task]** **Side-by-side testing of the new pre-ping system** — The new pre-ping process will run alongside the old one to confirm results match before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Behind-the-scenes validation of each advertiser's pre-ping setup to ensure accuracy before the switch. (#41)
- **[Task]** **Deploy updated scheduled jobs in parallel** — New background jobs will run alongside the existing ones, with daily monitoring, to confirm everything matches before relying on them. (#43)
- **[Task]** **Phased switch-over of background jobs (lower-risk batch)** — Retire the lowest-risk legacy scheduled jobs once the replacements prove stable. (#44)
- **[Task]** **Phased switch-over of background jobs (mid batch)** — Retire the next group of legacy scheduled jobs after the prior batch is confirmed stable. (#45)
- **[Task]** **Phased switch-over of background jobs (critical batch)** — Carefully retire the most critical legacy jobs last, with close monitoring and the ability to roll back instantly. (#46)
- **[Task]** **Documented rollback steps** — Prepare and test recovery procedures for each system so any issue can be reversed quickly. (#48)
- **[Task]** **Troubleshooting guides for the support team** — Create reference guides for common issues like lead processing or stats problems, so they can be resolved faster. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
